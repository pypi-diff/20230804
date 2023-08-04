# Comparing `tmp/ressimpy-1.0.0.tar.gz` & `tmp/ressimpy-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ressimpy-1.0.0.tar", max compression
+gzip compressed data, was "ressimpy-1.0.1.tar", max compression
```

## Comparing `ressimpy-1.0.0.tar` & `ressimpy-1.0.1.tar`

### file list

```diff
@@ -1,142 +1,142 @@
--rw-r--r--   0        0        0     1776 2023-08-03 13:20:35.338123 ressimpy-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     2229 2023-01-12 17:08:26.678300 ressimpy-1.0.0/README.rst
--rw-r--r--   0        0        0      257 2023-05-26 14:43:31.311764 ressimpy-1.0.0/ResSimpy/__init__.py
--rw-r--r--   0        0        0      410 2023-06-21 13:16:34.510743 ressimpy-1.0.0/ResSimpy/Aquifer.py
--rw-r--r--   0        0        0     7290 2023-08-03 13:05:05.275276 ressimpy-1.0.0/ResSimpy/Completion.py
--rw-r--r--   0        0        0     1302 2023-07-31 13:22:26.951125 ressimpy-1.0.0/ResSimpy/Constraint.py
--rw-r--r--   0        0        0     1638 2023-07-31 13:22:26.951674 ressimpy-1.0.0/ResSimpy/Constraints.py
--rw-r--r--   0        0        0     1994 2023-06-29 14:10:06.622077 ressimpy-1.0.0/ResSimpy/DynamicProperty.py
--rw-r--r--   0        0        0       65 2023-05-26 16:39:38.107926 ressimpy-1.0.0/ResSimpy/Enums/__init__.py
--rw-r--r--   0        0        0      177 2023-05-26 16:39:38.107926 ressimpy-1.0.0/ResSimpy/Enums/HowEnum.py
--rw-r--r--   0        0        0      745 2023-07-06 08:59:34.399687 ressimpy-1.0.0/ResSimpy/Enums/UnitsEnum.py
--rw-r--r--   0        0        0      428 2023-06-21 13:16:34.510743 ressimpy-1.0.0/ResSimpy/Equilibration.py
--rw-r--r--   0        0        0     2947 2023-08-03 13:05:05.275276 ressimpy-1.0.0/ResSimpy/File.py
--rw-r--r--   0        0        0     2121 2023-07-31 13:22:26.952696 ressimpy-1.0.0/ResSimpy/FileBase.py
--rw-r--r--   0        0        0      428 2023-06-21 13:16:34.510743 ressimpy-1.0.0/ResSimpy/Gaslift.py
--rw-r--r--   0        0        0     2729 2023-07-07 16:32:37.817449 ressimpy-1.0.0/ResSimpy/Grid.py
--rw-r--r--   0        0        0      407 2023-03-29 09:32:30.640231 ressimpy-1.0.0/ResSimpy/Grids.py
--rw-r--r--   0        0        0      419 2023-06-21 13:16:34.510743 ressimpy-1.0.0/ResSimpy/Hydraulics.py
--rw-r--r--   0        0        0     2219 2023-08-03 13:05:05.276275 ressimpy-1.0.0/ResSimpy/ISODateTime.py
--rw-r--r--   0        0        0      479 2023-07-07 15:23:57.951765 ressimpy-1.0.0/ResSimpy/Network.py
--rw-r--r--   0        0        0      410 2023-05-31 15:06:51.829745 ressimpy-1.0.0/ResSimpy/Nexus/__init__.py
--rw-r--r--   0        0        0    12635 2023-06-21 13:16:34.526365 ressimpy-1.0.0/ResSimpy/Nexus/array_function_operations.py
--rw-r--r--   0        0        0       81 2023-04-06 09:32:11.755169 ressimpy-1.0.0/ResSimpy/Nexus/constants.py
--rw-r--r--   0        0        0       78 2023-05-31 15:21:40.173752 ressimpy-1.0.0/ResSimpy/Nexus/DataModels/__init__.py
--rw-r--r--   0        0        0      562 2023-05-26 16:17:28.240277 ressimpy-1.0.0/ResSimpy/Nexus/DataModels/FcsConfig.py
--rw-r--r--   0        0        0    14530 2023-07-31 13:22:26.953697 ressimpy-1.0.0/ResSimpy/Nexus/DataModels/FcsFile.py
--rw-r--r--   0        0        0      266 2023-05-26 14:43:31.301664 ressimpy-1.0.0/ResSimpy/Nexus/DataModels/Network/__init__.py
--rw-r--r--   0        0        0    22354 2023-07-31 13:22:26.953697 ressimpy-1.0.0/ResSimpy/Nexus/DataModels/Network/NexusConstraint.py
--rw-r--r--   0        0        0    17370 2023-07-31 13:22:26.954698 ressimpy-1.0.0/ResSimpy/Nexus/DataModels/Network/NexusConstraints.py
--rw-r--r--   0        0        0     2806 2023-07-31 13:22:26.955700 ressimpy-1.0.0/ResSimpy/Nexus/DataModels/Network/NexusNode.py
--rw-r--r--   0        0        0     5126 2023-07-31 13:22:26.955700 ressimpy-1.0.0/ResSimpy/Nexus/DataModels/Network/NexusNodeConnection.py
--rw-r--r--   0        0        0     7391 2023-07-31 13:22:26.956697 ressimpy-1.0.0/ResSimpy/Nexus/DataModels/Network/NexusNodeConnections.py
--rw-r--r--   0        0        0     7498 2023-07-31 13:22:26.956697 ressimpy-1.0.0/ResSimpy/Nexus/DataModels/Network/NexusNodes.py
--rw-r--r--   0        0        0     3250 2023-07-31 13:22:26.958696 ressimpy-1.0.0/ResSimpy/Nexus/DataModels/Network/NexusWellbore.py
--rw-r--r--   0        0        0     3428 2023-07-31 13:22:26.958696 ressimpy-1.0.0/ResSimpy/Nexus/DataModels/Network/NexusWellbores.py
--rw-r--r--   0        0        0     6989 2023-07-31 13:22:26.957697 ressimpy-1.0.0/ResSimpy/Nexus/DataModels/Network/NexusWellConnection.py
--rw-r--r--   0        0        0     4547 2023-07-31 13:22:26.957697 ressimpy-1.0.0/ResSimpy/Nexus/DataModels/Network/NexusWellConnections.py
--rw-r--r--   0        0        0     5119 2023-07-31 13:22:26.958696 ressimpy-1.0.0/ResSimpy/Nexus/DataModels/Network/NexusWellhead.py
--rw-r--r--   0        0        0     3532 2023-07-31 13:22:26.959697 ressimpy-1.0.0/ResSimpy/Nexus/DataModels/Network/NexusWellheads.py
--rw-r--r--   0        0        0     6442 2023-07-06 08:59:34.399687 ressimpy-1.0.0/ResSimpy/Nexus/DataModels/NexusAquiferMethod.py
--rw-r--r--   0        0        0    14330 2023-08-03 13:05:05.277284 ressimpy-1.0.0/ResSimpy/Nexus/DataModels/NexusCompletion.py
--rw-r--r--   0        0        0     8671 2023-07-06 08:59:34.399687 ressimpy-1.0.0/ResSimpy/Nexus/DataModels/NexusEquilMethod.py
--rw-r--r--   0        0        0    30243 2023-07-31 13:22:26.960696 ressimpy-1.0.0/ResSimpy/Nexus/DataModels/NexusFile.py
--rw-r--r--   0        0        0     4946 2023-07-07 15:23:57.951765 ressimpy-1.0.0/ResSimpy/Nexus/DataModels/NexusGasliftMethod.py
--rw-r--r--   0        0        0    10701 2023-07-06 08:59:34.399687 ressimpy-1.0.0/ResSimpy/Nexus/DataModels/NexusHydraulicsMethod.py
--rw-r--r--   0        0        0    28105 2023-07-06 08:59:34.399687 ressimpy-1.0.0/ResSimpy/Nexus/DataModels/NexusPVTMethod.py
--rw-r--r--   0        0        0     2591 2023-05-31 15:21:29.026239 ressimpy-1.0.0/ResSimpy/Nexus/DataModels/NexusRelPermEndPoint.py
--rw-r--r--   0        0        0    18343 2023-07-06 08:59:34.399687 ressimpy-1.0.0/ResSimpy/Nexus/DataModels/NexusRelPermMethod.py
--rw-r--r--   0        0        0     8211 2023-07-06 08:59:34.415326 ressimpy-1.0.0/ResSimpy/Nexus/DataModels/NexusRockMethod.py
--rw-r--r--   0        0        0     7637 2023-07-06 08:59:34.415326 ressimpy-1.0.0/ResSimpy/Nexus/DataModels/NexusSeparatorMethod.py
--rw-r--r--   0        0        0     5264 2023-07-06 08:59:34.415326 ressimpy-1.0.0/ResSimpy/Nexus/DataModels/NexusValveMethod.py
--rw-r--r--   0        0        0    10125 2023-07-06 08:59:34.415326 ressimpy-1.0.0/ResSimpy/Nexus/DataModels/NexusWaterMethod.py
--rw-r--r--   0        0        0     9332 2023-07-24 13:48:55.819079 ressimpy-1.0.0/ResSimpy/Nexus/DataModels/NexusWell.py
--rw-r--r--   0        0        0        0 2023-03-29 09:32:30.644231 ressimpy-1.0.0/ResSimpy/Nexus/DataModels/StructuredGrid/__init__.py
--rw-r--r--   0        0        0    15038 2023-07-12 14:12:20.326094 ressimpy-1.0.0/ResSimpy/Nexus/DataModels/StructuredGrid/NexusGrid.py
--rw-r--r--   0        0        0    16018 2023-07-06 08:59:34.415326 ressimpy-1.0.0/ResSimpy/Nexus/load_wells.py
--rw-r--r--   0        0        0    14336 2023-07-07 15:23:57.951765 ressimpy-1.0.0/ResSimpy/Nexus/logfile_operations.py
--rw-r--r--   0        0        0    14832 2023-08-03 13:05:05.278188 ressimpy-1.0.0/ResSimpy/Nexus/nexus_add_new_object_to_file.py
--rw-r--r--   0        0        0     8100 2023-07-31 13:22:26.963699 ressimpy-1.0.0/ResSimpy/Nexus/nexus_collect_tables.py
--rw-r--r--   0        0        0     6970 2023-07-31 13:22:26.964697 ressimpy-1.0.0/ResSimpy/Nexus/nexus_constraint_operations.py
--rw-r--r--   0        0        0    40027 2023-07-12 14:15:09.035272 ressimpy-1.0.0/ResSimpy/Nexus/nexus_file_operations.py
--rw-r--r--   0        0        0     2002 2023-07-31 13:22:26.964697 ressimpy-1.0.0/ResSimpy/Nexus/nexus_modify_object_in_file.py
--rw-r--r--   0        0        0     5399 2023-07-31 13:22:26.965696 ressimpy-1.0.0/ResSimpy/Nexus/nexus_remove_object_from_file.py
--rw-r--r--   0        0        0     2948 2023-06-29 14:10:06.638013 ressimpy-1.0.0/ResSimpy/Nexus/NexusAquiferMethods.py
--rw-r--r--   0        0        0      109 2023-05-26 16:39:38.117951 ressimpy-1.0.0/ResSimpy/Nexus/NexusEnums/__init__.py
--rw-r--r--   0        0        0      149 2023-06-06 16:18:46.945539 ressimpy-1.0.0/ResSimpy/Nexus/NexusEnums/DateFormatEnum.py
--rw-r--r--   0        0        0     2927 2023-06-29 14:10:06.638982 ressimpy-1.0.0/ResSimpy/Nexus/NexusEquilMethods.py
--rw-r--r--   0        0        0     2938 2023-06-29 14:10:06.639415 ressimpy-1.0.0/ResSimpy/Nexus/NexusGasliftMethods.py
--rw-r--r--   0        0        0        0 2023-03-29 09:32:30.646233 ressimpy-1.0.0/ResSimpy/Nexus/NexusGrids.py
--rw-r--r--   0        0        0     3008 2023-06-29 14:10:06.639944 ressimpy-1.0.0/ResSimpy/Nexus/NexusHydraulicsMethods.py
--rw-r--r--   0        0        0        0 2023-03-01 12:41:43.871019 ressimpy-1.0.0/ResSimpy/Nexus/NexusKeywords/__init__.py
--rw-r--r--   0        0        0        0 2023-03-01 12:41:43.872017 ressimpy-1.0.0/ResSimpy/Nexus/NexusKeywords/adsorption_keywords.py
--rw-r--r--   0        0        0        0 2023-03-01 12:41:43.872017 ressimpy-1.0.0/ResSimpy/Nexus/NexusKeywords/alphaf_keywords.py
--rw-r--r--   0        0        0      769 2023-05-25 15:04:55.938102 ressimpy-1.0.0/ResSimpy/Nexus/NexusKeywords/aquifer_keywords.py
--rw-r--r--   0        0        0        0 2023-03-01 12:41:43.873016 ressimpy-1.0.0/ResSimpy/Nexus/NexusKeywords/choke_keywords.py
--rw-r--r--   0        0        0        0 2023-03-01 12:41:43.873016 ressimpy-1.0.0/ResSimpy/Nexus/NexusKeywords/compressor_keywords.py
--rw-r--r--   0        0        0        0 2023-03-01 12:41:43.873016 ressimpy-1.0.0/ResSimpy/Nexus/NexusKeywords/eos_defaults_keywords.py
--rw-r--r--   0        0        0     1226 2023-05-25 15:04:55.938102 ressimpy-1.0.0/ResSimpy/Nexus/NexusKeywords/equil_keywords.py
--rw-r--r--   0        0        0        0 2023-03-01 12:41:43.874019 ressimpy-1.0.0/ResSimpy/Nexus/NexusKeywords/esp_keywords.py
--rw-r--r--   0        0        0     1385 2023-03-01 12:41:43.875019 ressimpy-1.0.0/ResSimpy/Nexus/NexusKeywords/fcs_keywords.py
--rw-r--r--   0        0        0        0 2023-03-01 12:41:43.875019 ressimpy-1.0.0/ResSimpy/Nexus/NexusKeywords/fluxin_keywords.py
--rw-r--r--   0        0        0      175 2023-06-21 13:16:34.526365 ressimpy-1.0.0/ResSimpy/Nexus/NexusKeywords/gaslift_keywords.py
--rw-r--r--   0        0        0     1184 2023-06-07 14:25:28.385075 ressimpy-1.0.0/ResSimpy/Nexus/NexusKeywords/hyd_keywords.py
--rw-r--r--   0        0        0        0 2023-03-01 12:41:43.876020 ressimpy-1.0.0/ResSimpy/Nexus/NexusKeywords/icd_keywords.py
--rw-r--r--   0        0        0        0 2023-03-01 12:41:43.877020 ressimpy-1.0.0/ResSimpy/Nexus/NexusKeywords/ipr_keywords.py
--rw-r--r--   0        0        0     2697 2023-04-06 09:32:11.751171 ressimpy-1.0.0/ResSimpy/Nexus/NexusKeywords/nexus_keywords.py
--rw-r--r--   0        0        0      804 2023-07-12 09:38:44.641837 ressimpy-1.0.0/ResSimpy/Nexus/NexusKeywords/options_keywords.py
--rw-r--r--   0        0        0        0 2023-03-01 12:41:43.878025 ressimpy-1.0.0/ResSimpy/Nexus/NexusKeywords/polymer_keywords.py
--rw-r--r--   0        0        0        0 2023-03-01 12:41:43.878025 ressimpy-1.0.0/ResSimpy/Nexus/NexusKeywords/pump_keywords.py
--rw-r--r--   0        0        0     2579 2023-06-29 14:10:06.640425 ressimpy-1.0.0/ResSimpy/Nexus/NexusKeywords/pvt_keywords.py
--rw-r--r--   0        0        0     1600 2023-05-25 15:04:55.938102 ressimpy-1.0.0/ResSimpy/Nexus/NexusKeywords/relpm_keywords.py
--rw-r--r--   0        0        0      912 2023-05-25 15:04:55.938102 ressimpy-1.0.0/ResSimpy/Nexus/NexusKeywords/rock_keywords.py
--rw-r--r--   0        0        0     2891 2023-03-01 12:41:43.880020 ressimpy-1.0.0/ResSimpy/Nexus/NexusKeywords/runcontrol_keywords.py
--rw-r--r--   0        0        0      896 2023-05-10 13:07:36.258536 ressimpy-1.0.0/ResSimpy/Nexus/NexusKeywords/separator_keywords.py
--rw-r--r--   0        0        0     3124 2023-04-06 09:47:54.741802 ressimpy-1.0.0/ResSimpy/Nexus/NexusKeywords/structured_grid_keywords.py
--rw-r--r--   0        0        0     4535 2023-03-29 09:32:30.648231 ressimpy-1.0.0/ResSimpy/Nexus/NexusKeywords/surface_keywords.py
--rw-r--r--   0        0        0        0 2023-03-01 12:41:43.882022 ressimpy-1.0.0/ResSimpy/Nexus/NexusKeywords/tracer_init_keywords.py
--rw-r--r--   0        0        0      314 2023-05-25 15:04:55.938102 ressimpy-1.0.0/ResSimpy/Nexus/NexusKeywords/valve_keywords.py
--rw-r--r--   0        0        0      247 2023-03-01 12:41:43.882022 ressimpy-1.0.0/ResSimpy/Nexus/NexusKeywords/water_keywords.py
--rw-r--r--   0        0        0      912 2023-03-01 12:41:43.883018 ressimpy-1.0.0/ResSimpy/Nexus/NexusKeywords/wells_keywords.py
--rw-r--r--   0        0        0     9586 2023-07-31 13:22:26.961699 ressimpy-1.0.0/ResSimpy/Nexus/NexusNetwork.py
--rw-r--r--   0        0        0     2842 2023-06-29 14:10:06.641680 ressimpy-1.0.0/ResSimpy/Nexus/NexusPVTMethods.py
--rw-r--r--   0        0        0     3055 2023-06-29 14:10:06.642139 ressimpy-1.0.0/ResSimpy/Nexus/NexusRelPermMethods.py
--rw-r--r--   0        0        0     1651 2023-06-21 13:16:34.526365 ressimpy-1.0.0/ResSimpy/Nexus/NexusReporting.py
--rw-r--r--   0        0        0     2874 2023-06-29 14:10:06.642246 ressimpy-1.0.0/ResSimpy/Nexus/NexusRockMethods.py
--rw-r--r--   0        0        0     3141 2023-06-29 14:10:06.642984 ressimpy-1.0.0/ResSimpy/Nexus/NexusSeparatorMethods.py
--rw-r--r--   0        0        0    32387 2023-07-31 13:22:26.961699 ressimpy-1.0.0/ResSimpy/Nexus/NexusSimulator.py
--rw-r--r--   0        0        0     2911 2023-06-29 14:10:06.643714 ressimpy-1.0.0/ResSimpy/Nexus/NexusValveMethods.py
--rw-r--r--   0        0        0     2906 2023-06-29 14:10:06.644477 ressimpy-1.0.0/ResSimpy/Nexus/NexusWaterMethods.py
--rw-r--r--   0        0        0    22899 2023-07-31 13:22:26.962698 ressimpy-1.0.0/ResSimpy/Nexus/NexusWells.py
--rw-r--r--   0        0        0     5537 2023-06-21 13:16:34.537380 ressimpy-1.0.0/ResSimpy/Nexus/rel_perm_operations.py
--rw-r--r--   0        0        0    13966 2023-07-07 15:23:57.951765 ressimpy-1.0.0/ResSimpy/Nexus/runcontrol_operations.py
--rw-r--r--   0        0        0     9174 2023-07-12 14:05:19.173232 ressimpy-1.0.0/ResSimpy/Nexus/structured_grid_operations.py
--rw-r--r--   0        0        0      858 2023-07-31 13:22:26.965696 ressimpy-1.0.0/ResSimpy/Node.py
--rw-r--r--   0        0        0      703 2023-07-31 13:22:26.965696 ressimpy-1.0.0/ResSimpy/NodeConnection.py
--rw-r--r--   0        0        0      471 2023-07-31 13:22:26.966698 ressimpy-1.0.0/ResSimpy/NodeConnections.py
--rw-r--r--   0        0        0      413 2023-07-31 13:22:26.966698 ressimpy-1.0.0/ResSimpy/Nodes.py
--rw-r--r--   0        0        0     2221 2023-07-31 13:22:26.967698 ressimpy-1.0.0/ResSimpy/OperationsMixin.py
--rw-r--r--   0        0        0      398 2023-06-21 13:16:34.537380 ressimpy-1.0.0/ResSimpy/PVT.py
--rw-r--r--   0        0        0      482 2023-06-21 13:16:34.537380 ressimpy-1.0.0/ResSimpy/RelPerm.py
--rw-r--r--   0        0        0     3441 2023-05-31 15:17:40.025597 ressimpy-1.0.0/ResSimpy/RelPermEndPoint.py
--rw-r--r--   0        0        0      419 2023-06-21 13:16:34.537380 ressimpy-1.0.0/ResSimpy/Rock.py
--rw-r--r--   0        0        0      434 2023-06-21 13:16:34.537380 ressimpy-1.0.0/ResSimpy/Separator.py
--rw-r--r--   0        0        0     3540 2023-08-03 13:05:05.278981 ressimpy-1.0.0/ResSimpy/Simulator.py
--rw-r--r--   0        0        0       98 2023-05-26 16:39:38.117951 ressimpy-1.0.0/ResSimpy/Utils/__init__.py
--rw-r--r--   0        0        0     2278 2023-06-29 14:10:06.647732 ressimpy-1.0.0/ResSimpy/Utils/factory_methods.py
--rw-r--r--   0        0        0      584 2023-05-26 16:51:36.668030 ressimpy-1.0.0/ResSimpy/Utils/generic_repr.py
--rw-r--r--   0        0        0     1619 2023-05-26 16:44:46.870443 ressimpy-1.0.0/ResSimpy/Utils/invert_nexus_map.py
--rw-r--r--   0        0        0      467 2023-05-26 16:38:38.511398 ressimpy-1.0.0/ResSimpy/Utils/obj_to_dataframe.py
--rw-r--r--   0        0        0     1081 2023-07-31 13:22:26.968697 ressimpy-1.0.0/ResSimpy/Utils/obj_to_table_string.py
--rw-r--r--   0        0        0     2283 2023-07-24 13:48:55.819079 ressimpy-1.0.0/ResSimpy/Utils/to_dict_generic.py
--rw-r--r--   0        0        0      422 2023-06-21 13:16:34.537380 ressimpy-1.0.0/ResSimpy/Valve.py
--rw-r--r--   0        0        0      423 2023-06-21 13:16:34.537380 ressimpy-1.0.0/ResSimpy/Water.py
--rw-r--r--   0        0        0     2317 2023-07-06 08:59:34.415326 ressimpy-1.0.0/ResSimpy/Well.py
--rw-r--r--   0        0        0      775 2023-07-31 13:22:26.969696 ressimpy-1.0.0/ResSimpy/Wellbore.py
--rw-r--r--   0        0        0      441 2023-07-31 13:22:26.969696 ressimpy-1.0.0/ResSimpy/Wellbores.py
--rw-r--r--   0        0        0      639 2023-07-31 13:22:26.968697 ressimpy-1.0.0/ResSimpy/WellConnection.py
--rw-r--r--   0        0        0      449 2023-07-31 13:22:26.968697 ressimpy-1.0.0/ResSimpy/WellConnections.py
--rw-r--r--   0        0        0      830 2023-07-31 13:22:26.969696 ressimpy-1.0.0/ResSimpy/Wellhead.py
--rw-r--r--   0        0        0      441 2023-07-31 13:22:26.970706 ressimpy-1.0.0/ResSimpy/Wellheads.py
--rw-r--r--   0        0        0     1159 2023-07-31 13:22:26.970706 ressimpy-1.0.0/ResSimpy/Wells.py
--rw-r--r--   0        0        0     2919 1970-01-01 00:00:00.000000 ressimpy-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1521 2023-08-04 13:28:48.983296 ressimpy-1.0.1/README.md
+-rw-r--r--   0        0        0      395 2023-08-04 13:28:48.983296 ressimpy-1.0.1/ResSimpy/Aquifer.py
+-rw-r--r--   0        0        0     7082 2023-08-04 13:28:48.983296 ressimpy-1.0.1/ResSimpy/Completion.py
+-rw-r--r--   0        0        0     1263 2023-08-04 13:28:48.983296 ressimpy-1.0.1/ResSimpy/Constraint.py
+-rw-r--r--   0        0        0     1595 2023-08-04 13:28:48.983296 ressimpy-1.0.1/ResSimpy/Constraints.py
+-rw-r--r--   0        0        0     1945 2023-08-04 13:28:48.983296 ressimpy-1.0.1/ResSimpy/DynamicProperty.py
+-rw-r--r--   0        0        0      168 2023-08-04 13:28:48.983296 ressimpy-1.0.1/ResSimpy/Enums/HowEnum.py
+-rw-r--r--   0        0        0      722 2023-08-04 13:28:48.983296 ressimpy-1.0.1/ResSimpy/Enums/UnitsEnum.py
+-rw-r--r--   0        0        0       62 2023-08-04 13:28:48.983296 ressimpy-1.0.1/ResSimpy/Enums/__init__.py
+-rw-r--r--   0        0        0      413 2023-08-04 13:28:48.983296 ressimpy-1.0.1/ResSimpy/Equilibration.py
+-rw-r--r--   0        0        0     2880 2023-08-04 13:28:48.983296 ressimpy-1.0.1/ResSimpy/File.py
+-rw-r--r--   0        0        0     2068 2023-08-04 13:28:48.983296 ressimpy-1.0.1/ResSimpy/FileBase.py
+-rw-r--r--   0        0        0      413 2023-08-04 13:28:48.983296 ressimpy-1.0.1/ResSimpy/Gaslift.py
+-rw-r--r--   0        0        0     2631 2023-08-04 13:28:48.983296 ressimpy-1.0.1/ResSimpy/Grid.py
+-rw-r--r--   0        0        0      393 2023-08-04 13:28:48.983296 ressimpy-1.0.1/ResSimpy/Grids.py
+-rw-r--r--   0        0        0      404 2023-08-04 13:28:48.983296 ressimpy-1.0.1/ResSimpy/Hydraulics.py
+-rw-r--r--   0        0        0     2163 2023-08-04 13:28:48.983296 ressimpy-1.0.1/ResSimpy/ISODateTime.py
+-rw-r--r--   0        0        0      462 2023-08-04 13:28:48.983296 ressimpy-1.0.1/ResSimpy/Network.py
+-rw-r--r--   0        0        0      545 2023-08-04 13:28:48.983296 ressimpy-1.0.1/ResSimpy/Nexus/DataModels/FcsConfig.py
+-rw-r--r--   0        0        0    14289 2023-08-04 13:28:48.983296 ressimpy-1.0.1/ResSimpy/Nexus/DataModels/FcsFile.py
+-rw-r--r--   0        0        0    21922 2023-08-04 13:28:48.983296 ressimpy-1.0.1/ResSimpy/Nexus/DataModels/Network/NexusConstraint.py
+-rw-r--r--   0        0        0    17042 2023-08-04 13:28:48.983296 ressimpy-1.0.1/ResSimpy/Nexus/DataModels/Network/NexusConstraints.py
+-rw-r--r--   0        0        0     2736 2023-08-04 13:28:48.983296 ressimpy-1.0.1/ResSimpy/Nexus/DataModels/Network/NexusNode.py
+-rw-r--r--   0        0        0     5011 2023-08-04 13:28:48.983296 ressimpy-1.0.1/ResSimpy/Nexus/DataModels/Network/NexusNodeConnection.py
+-rw-r--r--   0        0        0     7241 2023-08-04 13:28:48.983296 ressimpy-1.0.1/ResSimpy/Nexus/DataModels/Network/NexusNodeConnections.py
+-rw-r--r--   0        0        0     7327 2023-08-04 13:28:48.983296 ressimpy-1.0.1/ResSimpy/Nexus/DataModels/Network/NexusNodes.py
+-rw-r--r--   0        0        0     6821 2023-08-04 13:28:48.983296 ressimpy-1.0.1/ResSimpy/Nexus/DataModels/Network/NexusWellConnection.py
+-rw-r--r--   0        0        0     4447 2023-08-04 13:28:48.983296 ressimpy-1.0.1/ResSimpy/Nexus/DataModels/Network/NexusWellConnections.py
+-rw-r--r--   0        0        0     3172 2023-08-04 13:28:48.983296 ressimpy-1.0.1/ResSimpy/Nexus/DataModels/Network/NexusWellbore.py
+-rw-r--r--   0        0        0     3340 2023-08-04 13:28:48.983296 ressimpy-1.0.1/ResSimpy/Nexus/DataModels/Network/NexusWellbores.py
+-rw-r--r--   0        0        0     5008 2023-08-04 13:28:48.983296 ressimpy-1.0.1/ResSimpy/Nexus/DataModels/Network/NexusWellhead.py
+-rw-r--r--   0        0        0     3445 2023-08-04 13:28:48.983296 ressimpy-1.0.1/ResSimpy/Nexus/DataModels/Network/NexusWellheads.py
+-rw-r--r--   0        0        0      263 2023-08-04 13:28:48.983296 ressimpy-1.0.1/ResSimpy/Nexus/DataModels/Network/__init__.py
+-rw-r--r--   0        0        0     6322 2023-08-04 13:28:48.983296 ressimpy-1.0.1/ResSimpy/Nexus/DataModels/NexusAquiferMethod.py
+-rw-r--r--   0        0        0    13983 2023-08-04 13:28:48.983296 ressimpy-1.0.1/ResSimpy/Nexus/DataModels/NexusCompletion.py
+-rw-r--r--   0        0        0     8514 2023-08-04 13:28:48.983296 ressimpy-1.0.1/ResSimpy/Nexus/DataModels/NexusEquilMethod.py
+-rw-r--r--   0        0        0    29623 2023-08-04 13:28:48.983296 ressimpy-1.0.1/ResSimpy/Nexus/DataModels/NexusFile.py
+-rw-r--r--   0        0        0     4843 2023-08-04 13:28:48.983296 ressimpy-1.0.1/ResSimpy/Nexus/DataModels/NexusGasliftMethod.py
+-rw-r--r--   0        0        0    10498 2023-08-04 13:28:48.983296 ressimpy-1.0.1/ResSimpy/Nexus/DataModels/NexusHydraulicsMethod.py
+-rw-r--r--   0        0        0    27650 2023-08-04 13:28:48.983296 ressimpy-1.0.1/ResSimpy/Nexus/DataModels/NexusPVTMethod.py
+-rw-r--r--   0        0        0     2543 2023-08-04 13:28:48.983296 ressimpy-1.0.1/ResSimpy/Nexus/DataModels/NexusRelPermEndPoint.py
+-rw-r--r--   0        0        0    18026 2023-08-04 13:28:48.983296 ressimpy-1.0.1/ResSimpy/Nexus/DataModels/NexusRelPermMethod.py
+-rw-r--r--   0        0        0     8056 2023-08-04 13:28:48.983296 ressimpy-1.0.1/ResSimpy/Nexus/DataModels/NexusRockMethod.py
+-rw-r--r--   0        0        0     7487 2023-08-04 13:28:48.983296 ressimpy-1.0.1/ResSimpy/Nexus/DataModels/NexusSeparatorMethod.py
+-rw-r--r--   0        0        0     5159 2023-08-04 13:28:48.983296 ressimpy-1.0.1/ResSimpy/Nexus/DataModels/NexusValveMethod.py
+-rw-r--r--   0        0        0     9929 2023-08-04 13:28:48.983296 ressimpy-1.0.1/ResSimpy/Nexus/DataModels/NexusWaterMethod.py
+-rw-r--r--   0        0        0     9125 2023-08-04 13:28:48.983296 ressimpy-1.0.1/ResSimpy/Nexus/DataModels/NexusWell.py
+-rw-r--r--   0        0        0    14736 2023-08-04 13:28:48.983296 ressimpy-1.0.1/ResSimpy/Nexus/DataModels/StructuredGrid/NexusGrid.py
+-rw-r--r--   0        0        0        0 2023-08-04 13:28:48.983296 ressimpy-1.0.1/ResSimpy/Nexus/DataModels/StructuredGrid/__init__.py
+-rw-r--r--   0        0        0       77 2023-08-04 13:28:48.983296 ressimpy-1.0.1/ResSimpy/Nexus/DataModels/__init__.py
+-rw-r--r--   0        0        0     2879 2023-08-04 13:28:48.983296 ressimpy-1.0.1/ResSimpy/Nexus/NexusAquiferMethods.py
+-rw-r--r--   0        0        0      142 2023-08-04 13:28:48.983296 ressimpy-1.0.1/ResSimpy/Nexus/NexusEnums/DateFormatEnum.py
+-rw-r--r--   0        0        0      106 2023-08-04 13:28:48.983296 ressimpy-1.0.1/ResSimpy/Nexus/NexusEnums/__init__.py
+-rw-r--r--   0        0        0     2858 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Nexus/NexusEquilMethods.py
+-rw-r--r--   0        0        0     2869 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Nexus/NexusGasliftMethods.py
+-rw-r--r--   0        0        0        0 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Nexus/NexusGrids.py
+-rw-r--r--   0        0        0     2939 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Nexus/NexusHydraulicsMethods.py
+-rw-r--r--   0        0        0        0 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Nexus/NexusKeywords/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Nexus/NexusKeywords/adsorption_keywords.py
+-rw-r--r--   0        0        0        0 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Nexus/NexusKeywords/alphaf_keywords.py
+-rw-r--r--   0        0        0      757 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Nexus/NexusKeywords/aquifer_keywords.py
+-rw-r--r--   0        0        0        0 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Nexus/NexusKeywords/choke_keywords.py
+-rw-r--r--   0        0        0        0 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Nexus/NexusKeywords/compressor_keywords.py
+-rw-r--r--   0        0        0        0 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Nexus/NexusKeywords/eos_defaults_keywords.py
+-rw-r--r--   0        0        0     1210 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Nexus/NexusKeywords/equil_keywords.py
+-rw-r--r--   0        0        0        0 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Nexus/NexusKeywords/esp_keywords.py
+-rw-r--r--   0        0        0     1368 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Nexus/NexusKeywords/fcs_keywords.py
+-rw-r--r--   0        0        0        0 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Nexus/NexusKeywords/fluxin_keywords.py
+-rw-r--r--   0        0        0      170 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Nexus/NexusKeywords/gaslift_keywords.py
+-rw-r--r--   0        0        0     1159 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Nexus/NexusKeywords/hyd_keywords.py
+-rw-r--r--   0        0        0        0 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Nexus/NexusKeywords/icd_keywords.py
+-rw-r--r--   0        0        0        0 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Nexus/NexusKeywords/ipr_keywords.py
+-rw-r--r--   0        0        0     2658 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Nexus/NexusKeywords/nexus_keywords.py
+-rw-r--r--   0        0        0      795 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Nexus/NexusKeywords/options_keywords.py
+-rw-r--r--   0        0        0        0 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Nexus/NexusKeywords/polymer_keywords.py
+-rw-r--r--   0        0        0        0 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Nexus/NexusKeywords/pump_keywords.py
+-rw-r--r--   0        0        0     2547 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Nexus/NexusKeywords/pvt_keywords.py
+-rw-r--r--   0        0        0     1579 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Nexus/NexusKeywords/relpm_keywords.py
+-rw-r--r--   0        0        0      896 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Nexus/NexusKeywords/rock_keywords.py
+-rw-r--r--   0        0        0     2864 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Nexus/NexusKeywords/runcontrol_keywords.py
+-rw-r--r--   0        0        0      880 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Nexus/NexusKeywords/separator_keywords.py
+-rw-r--r--   0        0        0     3082 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Nexus/NexusKeywords/structured_grid_keywords.py
+-rw-r--r--   0        0        0     4492 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Nexus/NexusKeywords/surface_keywords.py
+-rw-r--r--   0        0        0        0 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Nexus/NexusKeywords/tracer_init_keywords.py
+-rw-r--r--   0        0        0      306 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Nexus/NexusKeywords/valve_keywords.py
+-rw-r--r--   0        0        0      243 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Nexus/NexusKeywords/water_keywords.py
+-rw-r--r--   0        0        0      902 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Nexus/NexusKeywords/wells_keywords.py
+-rw-r--r--   0        0        0     9401 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Nexus/NexusNetwork.py
+-rw-r--r--   0        0        0     2773 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Nexus/NexusPVTMethods.py
+-rw-r--r--   0        0        0     2985 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Nexus/NexusRelPermMethods.py
+-rw-r--r--   0        0        0     1607 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Nexus/NexusReporting.py
+-rw-r--r--   0        0        0     2805 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Nexus/NexusRockMethods.py
+-rw-r--r--   0        0        0     3070 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Nexus/NexusSeparatorMethods.py
+-rw-r--r--   0        0        0    31715 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Nexus/NexusSimulator.py
+-rw-r--r--   0        0        0     2842 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Nexus/NexusValveMethods.py
+-rw-r--r--   0        0        0     2837 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Nexus/NexusWaterMethods.py
+-rw-r--r--   0        0        0    22484 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Nexus/NexusWells.py
+-rw-r--r--   0        0        0      404 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Nexus/__init__.py
+-rw-r--r--   0        0        0    12346 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Nexus/array_function_operations.py
+-rw-r--r--   0        0        0       77 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Nexus/constants.py
+-rw-r--r--   0        0        0    15687 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Nexus/load_wells.py
+-rw-r--r--   0        0        0    14023 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Nexus/logfile_operations.py
+-rw-r--r--   0        0        0    14562 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Nexus/nexus_add_new_object_to_file.py
+-rw-r--r--   0        0        0     7954 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Nexus/nexus_collect_tables.py
+-rw-r--r--   0        0        0     6838 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Nexus/nexus_constraint_operations.py
+-rw-r--r--   0        0        0    39152 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Nexus/nexus_file_operations.py
+-rw-r--r--   0        0        0     1963 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Nexus/nexus_modify_object_in_file.py
+-rw-r--r--   0        0        0     5297 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Nexus/nexus_remove_object_from_file.py
+-rw-r--r--   0        0        0     5387 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Nexus/rel_perm_operations.py
+-rw-r--r--   0        0        0    13632 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Nexus/runcontrol_operations.py
+-rw-r--r--   0        0        0     8982 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Nexus/structured_grid_operations.py
+-rw-r--r--   0        0        0      829 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Node.py
+-rw-r--r--   0        0        0      679 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/NodeConnection.py
+-rw-r--r--   0        0        0      456 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/NodeConnections.py
+-rw-r--r--   0        0        0      398 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Nodes.py
+-rw-r--r--   0        0        0     2158 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/OperationsMixin.py
+-rw-r--r--   0        0        0      383 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/PVT.py
+-rw-r--r--   0        0        0      467 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/RelPerm.py
+-rw-r--r--   0        0        0     3354 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/RelPermEndPoint.py
+-rw-r--r--   0        0        0      404 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Rock.py
+-rw-r--r--   0        0        0      419 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Separator.py
+-rw-r--r--   0        0        0     3402 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Simulator.py
+-rw-r--r--   0        0        0       95 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Utils/__init__.py
+-rw-r--r--   0        0        0     2213 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Utils/factory_methods.py
+-rw-r--r--   0        0        0      566 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Utils/generic_repr.py
+-rw-r--r--   0        0        0     1585 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Utils/invert_nexus_map.py
+-rw-r--r--   0        0        0      453 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Utils/obj_to_dataframe.py
+-rw-r--r--   0        0        0     1053 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Utils/obj_to_table_string.py
+-rw-r--r--   0        0        0     2234 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Utils/to_dict_generic.py
+-rw-r--r--   0        0        0      407 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Valve.py
+-rw-r--r--   0        0        0      408 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Water.py
+-rw-r--r--   0        0        0     2256 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Well.py
+-rw-r--r--   0        0        0      618 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/WellConnection.py
+-rw-r--r--   0        0        0      435 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/WellConnections.py
+-rw-r--r--   0        0        0      748 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Wellbore.py
+-rw-r--r--   0        0        0      427 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Wellbores.py
+-rw-r--r--   0        0        0      802 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Wellhead.py
+-rw-r--r--   0        0        0      426 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Wellheads.py
+-rw-r--r--   0        0        0     1119 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Wells.py
+-rw-r--r--   0        0        0      245 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/__init__.py
+-rw-r--r--   0        0        0     1859 2023-08-04 13:28:48.991296 ressimpy-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2315 1970-01-01 00:00:00.000000 ressimpy-1.0.1/PKG-INFO
```

### Comparing `ressimpy-1.0.0/pyproject.toml` & `ressimpy-1.0.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,111 +1,117 @@
-00000000: 5b74 6f6f 6c2e 706f 6574 7279 5d0d 0a6e  [tool.poetry]..n
-00000010: 616d 6520 3d20 2252 6573 5369 6d70 7922  ame = "ResSimpy"
-00000020: 0d0a 7665 7273 696f 6e20 3d20 2231 2e30  ..version = "1.0
-00000030: 2e30 220d 0a64 6573 6372 6970 7469 6f6e  .0"..description
-00000040: 203d 2022 4120 5079 7468 6f6e 206c 6962   = "A Python lib
-00000050: 7261 7279 2066 6f72 2077 6f72 6b69 6e67  rary for working
-00000060: 2077 6974 6820 5265 7365 7276 6f69 7220   with Reservoir 
-00000070: 5369 6d75 6c61 746f 7220 4d6f 6465 6c73  Simulator Models
-00000080: 2e22 0d0a 6175 7468 6f72 7320 3d20 5b22  ."..authors = ["
-00000090: 4250 225d 0d0a 7265 6164 6d65 203d 2022  BP"]..readme = "
-000000a0: 5245 4144 4d45 2e72 7374 220d 0a6b 6579  README.rst"..key
-000000b0: 776f 7264 7320 3d20 5b22 5265 7353 696d  words = ["ResSim
-000000c0: 7079 222c 2022 5265 7365 7276 6f69 7220  py", "Reservoir 
-000000d0: 456e 6769 6e65 6572 696e 6722 5d0d 0a63  Engineering"]..c
-000000e0: 6c61 7373 6966 6965 7273 203d 205b 0d0a  lassifiers = [..
-000000f0: 2020 2020 224f 7065 7261 7469 6e67 2053      "Operating S
-00000100: 7973 7465 6d20 3a3a 204f 5320 496e 6465  ystem :: OS Inde
-00000110: 7065 6e64 656e 7422 2c0d 0a20 2020 2022  pendent",..    "
-00000120: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
-00000130: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
-00000140: 3a20 332e 3130 222c 0d0a 2020 2020 2250  : 3.10",..    "P
-00000150: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
-00000160: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
-00000170: 2033 2e31 3122 2c0d 0a20 2020 2022 4465   3.11",..    "De
-00000180: 7665 6c6f 706d 656e 7420 5374 6174 7573  velopment Status
-00000190: 203a 3a20 3320 2d20 416c 7068 6122 2c0d   :: 3 - Alpha",.
-000001a0: 0a20 2020 2022 546f 7069 6320 3a3a 2053  .    "Topic :: S
-000001b0: 6369 656e 7469 6669 632f 456e 6769 6e65  cientific/Engine
-000001c0: 6572 696e 6722 2c0d 0a20 2020 2022 546f  ering",..    "To
-000001d0: 7069 6320 3a3a 2053 7973 7465 6d20 3a3a  pic :: System ::
-000001e0: 2046 696c 6573 7973 7465 6d73 222c 0d0a   Filesystems",..
-000001f0: 2020 2020 2254 6f70 6963 203a 3a20 5363      "Topic :: Sc
-00000200: 6965 6e74 6966 6963 2f45 6e67 696e 6565  ientific/Enginee
-00000210: 7269 6e67 203a 3a20 496e 666f 726d 6174  ring :: Informat
-00000220: 696f 6e20 416e 616c 7973 6973 220d 0a5d  ion Analysis"..]
-00000230: 0d0a 0d0a 5b74 6f6f 6c2e 706f 6574 7279  ....[tool.poetry
-00000240: 2e64 6570 656e 6465 6e63 6965 735d 0d0a  .dependencies]..
-00000250: 7079 7468 6f6e 203d 2022 3e3d 332e 3130  python = ">=3.10
-00000260: 2c20 3c33 2e31 3222 0d0a 7265 7371 7079  , <3.12"..resqpy
-00000270: 203d 2022 5e34 2e37 220d 0a6e 756d 7079   = "^4.7"..numpy
-00000280: 203d 2022 5e31 2e32 3322 0d0a 7061 6e64   = "^1.23"..pand
-00000290: 6173 203d 2022 5e31 2e35 220d 0a0d 0a5b  as = "^1.5"....[
-000002a0: 746f 6f6c 2e70 6f65 7472 792e 6772 6f75  tool.poetry.grou
-000002b0: 702e 6465 762e 6465 7065 6e64 656e 6369  p.dev.dependenci
-000002c0: 6573 5d0d 0a70 7974 6573 742d 6d6f 636b  es]..pytest-mock
-000002d0: 203d 2022 5e33 2e39 220d 0a70 7974 6573   = "^3.9"..pytes
-000002e0: 7420 3d20 225e 372e 3122 0d0a 636f 7665  t = "^7.1"..cove
-000002f0: 7261 6765 203d 2022 5e36 2e35 220d 0a66  rage = "^6.5"..f
-00000300: 6c61 6b65 3820 3d20 225e 3622 0d0a 6d79  lake8 = "^6"..my
-00000310: 7079 203d 2022 5e31 2e32 220d 0a70 7963  py = "^1.2"..pyc
-00000320: 6f64 6573 7479 6c65 203d 2022 5e32 2e39  odestyle = "^2.9
-00000330: 2e31 220d 0a70 7974 6573 742d 636f 7620  .1"..pytest-cov 
-00000340: 3d20 225e 342e 302e 3022 0d0a 7275 6666  = "^4.0.0"..ruff
-00000350: 203d 2022 5e30 2e30 2e32 3730 220d 0a0d   = "^0.0.270"...
-00000360: 0a5b 6275 696c 642d 7379 7374 656d 5d0d  .[build-system].
-00000370: 0a72 6571 7569 7265 7320 3d20 5b22 706f  .requires = ["po
-00000380: 6574 7279 2d63 6f72 6522 5d0d 0a62 7569  etry-core"]..bui
-00000390: 6c64 2d62 6163 6b65 6e64 203d 2022 706f  ld-backend = "po
-000003a0: 6574 7279 2e63 6f72 652e 6d61 736f 6e72  etry.core.masonr
-000003b0: 792e 6170 6922 0d0a 0d0a 5b74 6f6f 6c2e  y.api"....[tool.
-000003c0: 7275 6666 5d0d 0a6c 696e 652d 6c65 6e67  ruff]..line-leng
-000003d0: 7468 203d 2031 3230 0d0a 2320 5275 6c65  th = 120..# Rule
-000003e0: 2063 6f64 6573 2066 6f72 2072 7566 6620   codes for ruff 
-000003f0: 6361 6e20 6265 2066 6f75 6e64 2061 743a  can be found at:
-00000400: 2068 7474 7073 3a2f 2f62 6574 612e 7275   https://beta.ru
-00000410: 6666 2e72 732f 646f 6373 2f72 756c 6573  ff.rs/docs/rules
-00000420: 2f0d 0a73 656c 6563 7420 3d20 5b22 4522  /..select = ["E"
-00000430: 2c20 2246 222c 2022 5722 2c20 2243 3930  , "F", "W", "C90
-00000440: 222c 2022 4e22 2c20 2022 5550 222c 2022  ", "N",  "UP", "
-00000450: 5954 5422 2c20 2241 4e4e 222c 2022 5322  YTT", "ANN", "S"
-00000460: 2c20 2242 4c45 222c 2022 4422 2c20 2250  , "BLE", "D", "P
-00000470: 4c45 222c 2022 504c 5722 2c20 2252 5546  LE", "PLW", "RUF
-00000480: 222c 2022 424c 4522 2c20 2241 5247 222c  ", "BLE", "ARG",
-00000490: 2022 4922 2c0d 0a20 2020 2022 434f 4d22   "I",..    "COM"
-000004a0: 2c20 2243 3422 2c20 2246 4131 3030 222c  , "C4", "FA100",
-000004b0: 2022 5049 4522 2c20 2254 3230 222c 2022   "PIE", "T20", "
-000004c0: 5059 4922 2c20 2254 4944 222c 2022 494e  PYI", "TID", "IN
-000004d0: 5422 2c20 2245 5241 222c 2022 5044 222c  T", "ERA", "PD",
-000004e0: 2022 464c 5922 2c20 224e 5059 225d 2023   "FLY", "NPY"] #
-000004f0: 2054 6f20 6164 6420 6c61 7465 723a 2050   To add later: P
-00000500: 4c2c 2050 4c52 0d0a 6967 6e6f 7265 203d  L, PLR..ignore =
-00000510: 205b 2255 5030 3037 222c 2020 2241 4e4e   ["UP007",  "ANN
-00000520: 3130 3122 2c20 224e 3939 3922 2c20 2255  101", "N999", "U
-00000530: 5030 3335 222c 2022 5331 3035 222c 2022  P035", "S105", "
-00000540: 4e38 3032 222c 2022 5331 3036 222c 2022  N802", "S106", "
-00000550: 5331 3037 222c 2022 5550 3031 3522 2c20  S107", "UP015", 
-00000560: 2241 4e4e 3430 3122 2c20 2241 4e4e 3130  "ANN401", "ANN10
-00000570: 3222 2c20 2244 3230 3222 2c0d 0a20 2020  2", "D202",..   
-00000580: 2022 4431 3035 222c 2022 4432 3033 222c   "D105", "D203",
-00000590: 2022 4432 3133 222c 2022 5255 4630 3130   "D213", "RUF010
-000005a0: 222c 2022 4930 3031 222c 2022 4230 3238  ", "I001", "B028
-000005b0: 222c 2022 434f 4d38 3132 222c 2022 5044  ", "COM812", "PD
-000005c0: 3930 3122 2c0d 0a20 2020 2023 2054 6f20  901",..    # To 
-000005d0: 6669 7820 6c61 7465 723a 0d0a 2020 2020  fix later:..    
-000005e0: 2241 4e4e 3030 3122 2c20 2320 5479 7065  "ANN001", # Type
-000005f0: 730d 0a20 2020 2241 4e4e 3230 3122 2c20  s..   "ANN201", 
-00000600: 2320 5479 7065 730d 0a20 2020 2241 4e4e  # Types..   "ANN
-00000610: 3230 3222 2c20 2320 5479 7065 730d 0a20  202", # Types.. 
-00000620: 2020 2022 4339 3031 222c 2023 2043 6f6d     "C901", # Com
-00000630: 706c 6578 6974 790d 0a20 2020 2022 4431  plexity..    "D1
-00000640: 3032 222c 2022 4431 3030 222c 2022 4431  02", "D100", "D1
-00000650: 3033 222c 2022 4431 3037 222c 2022 4431  03", "D107", "D1
-00000660: 3031 222c 2022 4432 3035 222c 2022 4434  01", "D205", "D4
-00000670: 3031 222c 2022 4434 3137 222c 2022 4431  01", "D417", "D1
-00000680: 3034 222c 2022 4431 3036 2220 2320 446f  04", "D106" # Do
-00000690: 6373 7472 696e 6773 0d0a 2020 2020 5d0d  cstrings..    ].
-000006a0: 0a0d 0a5b 746f 6f6c 2e72 7566 662e 7079  ...[tool.ruff.py
-000006b0: 646f 6373 7479 6c65 5d0d 0a23 2055 7365  docstyle]..# Use
-000006c0: 2047 6f6f 676c 652d 7374 796c 6520 646f   Google-style do
-000006d0: 6373 7472 696e 6773 2e0d 0a63 6f6e 7665  cstrings...conve
-000006e0: 6e74 696f 6e20 3d20 2267 6f6f 676c 6522  ntion = "google"
+00000000: 5b74 6f6f 6c2e 706f 6574 7279 5d0a 6e61  [tool.poetry].na
+00000010: 6d65 203d 2022 5265 7353 696d 7079 220a  me = "ResSimpy".
+00000020: 7665 7273 696f 6e20 3d20 2231 2e30 2e31  version = "1.0.1
+00000030: 220a 6465 7363 7269 7074 696f 6e20 3d20  ".description = 
+00000040: 2241 2050 7974 686f 6e20 6c69 6272 6172  "A Python librar
+00000050: 7920 666f 7220 776f 726b 696e 6720 7769  y for working wi
+00000060: 7468 2052 6573 6572 766f 6972 2053 696d  th Reservoir Sim
+00000070: 756c 6174 6f72 204d 6f64 656c 732e 220a  ulator Models.".
+00000080: 6175 7468 6f72 7320 3d20 5b22 4250 225d  authors = ["BP"]
+00000090: 0a72 6561 646d 6520 3d20 2252 4541 444d  .readme = "READM
+000000a0: 452e 6d64 220a 6b65 7977 6f72 6473 203d  E.md".keywords =
+000000b0: 205b 2252 6573 5369 6d70 7922 2c20 2252   ["ResSimpy", "R
+000000c0: 6573 6572 766f 6972 2045 6e67 696e 6565  eservoir Enginee
+000000d0: 7269 6e67 225d 0a63 6c61 7373 6966 6965  ring"].classifie
+000000e0: 7273 203d 205b 0a20 2020 2022 4f70 6572  rs = [.    "Oper
+000000f0: 6174 696e 6720 5379 7374 656d 203a 3a20  ating System :: 
+00000100: 4f53 2049 6e64 6570 656e 6465 6e74 222c  OS Independent",
+00000110: 0a20 2020 2022 5072 6f67 7261 6d6d 696e  .    "Programmin
+00000120: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
+00000130: 7468 6f6e 203a 3a20 332e 3130 222c 0a20  thon :: 3.10",. 
+00000140: 2020 2022 5072 6f67 7261 6d6d 696e 6720     "Programming 
+00000150: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
+00000160: 6f6e 203a 3a20 332e 3131 222c 0a20 2020  on :: 3.11",.   
+00000170: 2022 4465 7665 6c6f 706d 656e 7420 5374   "Development St
+00000180: 6174 7573 203a 3a20 3320 2d20 416c 7068  atus :: 3 - Alph
+00000190: 6122 2c0a 2020 2020 2254 6f70 6963 203a  a",.    "Topic :
+000001a0: 3a20 5363 6965 6e74 6966 6963 2f45 6e67  : Scientific/Eng
+000001b0: 696e 6565 7269 6e67 222c 0a20 2020 2022  ineering",.    "
+000001c0: 546f 7069 6320 3a3a 2053 7973 7465 6d20  Topic :: System 
+000001d0: 3a3a 2046 696c 6573 7973 7465 6d73 222c  :: Filesystems",
+000001e0: 0a20 2020 2022 546f 7069 6320 3a3a 2053  .    "Topic :: S
+000001f0: 6369 656e 7469 6669 632f 456e 6769 6e65  cientific/Engine
+00000200: 6572 696e 6720 3a3a 2049 6e66 6f72 6d61  ering :: Informa
+00000210: 7469 6f6e 2041 6e61 6c79 7369 7322 0a5d  tion Analysis".]
+00000220: 0a70 6163 6b61 6765 7320 3d20 5b0a 2020  .packages = [.  
+00000230: 2020 7b20 696e 636c 7564 6520 3d20 2252    { include = "R
+00000240: 6573 5369 6d70 7922 207d 2023 204e 6565  esSimpy" } # Nee
+00000250: 6465 6420 6265 6361 7573 6520 7468 6520  ded because the 
+00000260: 6465 6661 756c 7420 6275 696c 6420 636f  default build co
+00000270: 6d6d 616e 6420 6967 6e6f 7265 7320 6361  mmand ignores ca
+00000280: 7069 7461 6c20 6c65 7474 6572 730a 5d0a  pital letters.].
+00000290: 0a5b 746f 6f6c 2e70 6f65 7472 792e 6465  .[tool.poetry.de
+000002a0: 7065 6e64 656e 6369 6573 5d0a 7079 7468  pendencies].pyth
+000002b0: 6f6e 203d 2022 3e3d 332e 3130 2c20 3c33  on = ">=3.10, <3
+000002c0: 2e31 3222 0a72 6573 7170 7920 3d20 225e  .12".resqpy = "^
+000002d0: 342e 3922 0a6e 756d 7079 203d 2022 5e31  4.9".numpy = "^1
+000002e0: 2e32 3422 0a70 616e 6461 7320 3d20 225e  .24".pandas = "^
+000002f0: 312e 3522 0a74 7970 696e 672d 6578 7465  1.5".typing-exte
+00000300: 6e73 696f 6e73 203d 2022 5e34 2e37 220a  nsions = "^4.7".
+00000310: 0a5b 746f 6f6c 2e70 6f65 7472 792e 6772  .[tool.poetry.gr
+00000320: 6f75 702e 6465 762e 6465 7065 6e64 656e  oup.dev.dependen
+00000330: 6369 6573 5d0a 7079 7465 7374 2d6d 6f63  cies].pytest-moc
+00000340: 6b20 3d20 225e 332e 3922 0a70 7974 6573  k = "^3.9".pytes
+00000350: 7420 3d20 225e 372e 3122 0a63 6f76 6572  t = "^7.1".cover
+00000360: 6167 6520 3d20 225e 362e 3522 0a66 6c61  age = "^6.5".fla
+00000370: 6b65 3820 3d20 225e 3622 0a6d 7970 7920  ke8 = "^6".mypy 
+00000380: 3d20 225e 312e 3222 0a70 7963 6f64 6573  = "^1.2".pycodes
+00000390: 7479 6c65 203d 2022 5e32 2e39 2e31 220a  tyle = "^2.9.1".
+000003a0: 7079 7465 7374 2d63 6f76 203d 2022 5e34  pytest-cov = "^4
+000003b0: 2e30 2e30 220a 7275 6666 203d 2022 5e30  .0.0".ruff = "^0
+000003c0: 2e30 2e32 3730 220a 0a5b 6275 696c 642d  .0.270"..[build-
+000003d0: 7379 7374 656d 5d0a 7265 7175 6972 6573  system].requires
+000003e0: 203d 205b 2270 6f65 7472 792d 636f 7265   = ["poetry-core
+000003f0: 225d 0a62 7569 6c64 2d62 6163 6b65 6e64  "].build-backend
+00000400: 203d 2022 706f 6574 7279 2e63 6f72 652e   = "poetry.core.
+00000410: 6d61 736f 6e72 792e 6170 6922 0a0a 5b74  masonry.api"..[t
+00000420: 6f6f 6c2e 7275 6666 5d0a 6c69 6e65 2d6c  ool.ruff].line-l
+00000430: 656e 6774 6820 3d20 3132 300a 2320 5275  ength = 120.# Ru
+00000440: 6c65 2063 6f64 6573 2066 6f72 2072 7566  le codes for ruf
+00000450: 6620 6361 6e20 6265 2066 6f75 6e64 2061  f can be found a
+00000460: 743a 2068 7474 7073 3a2f 2f62 6574 612e  t: https://beta.
+00000470: 7275 6666 2e72 732f 646f 6373 2f72 756c  ruff.rs/docs/rul
+00000480: 6573 2f0a 7365 6c65 6374 203d 205b 2245  es/.select = ["E
+00000490: 222c 2022 4622 2c20 2257 222c 2022 4339  ", "F", "W", "C9
+000004a0: 3022 2c20 224e 222c 2020 2255 5022 2c20  0", "N",  "UP", 
+000004b0: 2259 5454 222c 2022 414e 4e22 2c20 2253  "YTT", "ANN", "S
+000004c0: 222c 2022 424c 4522 2c20 2244 222c 2022  ", "BLE", "D", "
+000004d0: 504c 4522 2c20 2250 4c57 222c 2022 5255  PLE", "PLW", "RU
+000004e0: 4622 2c20 2242 4c45 222c 2022 4152 4722  F", "BLE", "ARG"
+000004f0: 2c20 2249 222c 0a20 2020 2022 434f 4d22  , "I",.    "COM"
+00000500: 2c20 2243 3422 2c20 2246 4131 3030 222c  , "C4", "FA100",
+00000510: 2022 5049 4522 2c20 2254 3230 222c 2022   "PIE", "T20", "
+00000520: 5059 4922 2c20 2254 4944 222c 2022 494e  PYI", "TID", "IN
+00000530: 5422 2c20 2245 5241 222c 2022 5044 222c  T", "ERA", "PD",
+00000540: 2022 464c 5922 2c20 224e 5059 225d 2023   "FLY", "NPY"] #
+00000550: 2054 6f20 6164 6420 6c61 7465 723a 2050   To add later: P
+00000560: 4c2c 2050 4c52 0a69 676e 6f72 6520 3d20  L, PLR.ignore = 
+00000570: 5b22 5550 3030 3722 2c20 2022 414e 4e31  ["UP007",  "ANN1
+00000580: 3031 222c 2022 4e39 3939 222c 2022 5550  01", "N999", "UP
+00000590: 3033 3522 2c20 2253 3130 3522 2c20 224e  035", "S105", "N
+000005a0: 3830 3222 2c20 2253 3130 3622 2c20 2253  802", "S106", "S
+000005b0: 3130 3722 2c20 2255 5030 3135 222c 2022  107", "UP015", "
+000005c0: 414e 4e34 3031 222c 2022 414e 4e31 3032  ANN401", "ANN102
+000005d0: 222c 2022 4432 3032 222c 0a20 2020 2022  ", "D202",.    "
+000005e0: 4431 3035 222c 2022 4432 3033 222c 2022  D105", "D203", "
+000005f0: 4432 3133 222c 2022 5255 4630 3130 222c  D213", "RUF010",
+00000600: 2022 4930 3031 222c 2022 4230 3238 222c   "I001", "B028",
+00000610: 2022 434f 4d38 3132 222c 2022 5044 3930   "COM812", "PD90
+00000620: 3122 2c0a 2020 2020 2320 546f 2066 6978  1",.    # To fix
+00000630: 206c 6174 6572 3a0a 2020 2020 2241 4e4e   later:.    "ANN
+00000640: 3030 3122 2c20 2320 5479 7065 730a 2020  001", # Types.  
+00000650: 2022 414e 4e32 3031 222c 2023 2054 7970   "ANN201", # Typ
+00000660: 6573 0a20 2020 2241 4e4e 3230 3222 2c20  es.   "ANN202", 
+00000670: 2320 5479 7065 730a 2020 2020 2243 3930  # Types.    "C90
+00000680: 3122 2c20 2320 436f 6d70 6c65 7869 7479  1", # Complexity
+00000690: 0a20 2020 2022 4431 3032 222c 2022 4431  .    "D102", "D1
+000006a0: 3030 222c 2022 4431 3033 222c 2022 4431  00", "D103", "D1
+000006b0: 3037 222c 2022 4431 3031 222c 2022 4432  07", "D101", "D2
+000006c0: 3035 222c 2022 4434 3031 222c 2022 4434  05", "D401", "D4
+000006d0: 3137 222c 2022 4431 3034 222c 2022 4431  17", "D104", "D1
+000006e0: 3036 2220 2320 446f 6373 7472 696e 6773  06" # Docstrings
+000006f0: 0a20 2020 205d 0a0a 5b74 6f6f 6c2e 7275  .    ]..[tool.ru
+00000700: 6666 2e70 7964 6f63 7374 796c 655d 0a23  ff.pydocstyle].#
+00000710: 2055 7365 2047 6f6f 676c 652d 7374 796c   Use Google-styl
+00000720: 6520 646f 6373 7472 696e 6773 2e0a 636f  e docstrings..co
+00000730: 6e76 656e 7469 6f6e 203d 2022 676f 6f67  nvention = "goog
+00000740: 6c65 22                                  le"
```

### Comparing `ressimpy-1.0.0/ResSimpy/Constraints.py` & `ressimpy-1.0.1/ResSimpy/OperationsMixin.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,43 +1,63 @@
-from dataclasses import dataclass, field
-from abc import ABC, abstractmethod
-import pandas as pd
-
-from ResSimpy.Constraint import Constraint
-from typing import Optional, Mapping, Sequence
-
-from ResSimpy.Enums.UnitsEnum import UnitSystem
-
-
-@dataclass(kw_only=True)
-class Constraints(ABC):
-    __constraints: dict[str, list[Constraint]] = field(default_factory=lambda: {})
-
-    @abstractmethod
-    def get_all(self, object_name: Optional[str] = None, date: Optional[str] = None) \
-            -> Mapping[str, Sequence[Constraint]]:
-        raise NotImplementedError("Implement this in the derived class")
-
-    @abstractmethod
-    def get_df(self) -> pd.DataFrame:
-        raise NotImplementedError("Implement this in the derived class")
-
-    @abstractmethod
-    def get_overview(self) -> str:
-        raise NotImplementedError("Implement this in the derived class")
-
-    @abstractmethod
-    def remove(self) -> None:
-        raise NotImplementedError("Implement this in the derived class")
-
-    @abstractmethod
-    def add(self, name: str,
-            constraint_to_add: dict[str, None | float | int | str | UnitSystem] | Constraint) -> None:
-        raise NotImplementedError("Implement this in the derived class")
-
-    @abstractmethod
-    def modify(self, name: str,
-               current_constraint: dict[str, None | float | int | str] | Constraint,
-               new_constraint_props: dict[str, None | float | int | str | UnitSystem] | Constraint,
-               comments: Optional[str] = None) \
-            -> None:
-        raise NotImplementedError("Implement this in the derived class")
+
+from abc import ABC, abstractmethod
+from typing import Any, Sequence, Optional
+from uuid import UUID
+
+import pandas as pd
+
+from ResSimpy.Enums.UnitsEnum import UnitSystem
+from ResSimpy.File import File
+
+
+class NetworkOperationsMixIn(ABC):
+    @abstractmethod
+    def get_all(self) -> Sequence[Any]:
+        raise NotImplementedError("Implement this in the derived class")
+
+    @abstractmethod
+    def get_by_name(self, name: str) -> Optional[Any]:
+        raise NotImplementedError("Implement this in the derived class")
+
+    @abstractmethod
+    def get_df(self) -> pd.DataFrame:
+        raise NotImplementedError("Implement this in the derived class")
+
+    @abstractmethod
+    def get_overview(self) -> str:
+        raise NotImplementedError("Implement this in the derived class")
+
+    @abstractmethod
+    def load(self, file: File, start_date: str, default_units: UnitSystem) -> None:
+        raise NotImplementedError("Implement this in the derived class")
+
+    @abstractmethod
+    def _add_to_memory(self, additional_objs: Optional[list[Any]]):
+        raise NotImplementedError("Implement this in the derived class")
+
+    @abstractmethod
+    def remove(self, obj_to_remove: UUID | dict[str, None | str | float | int]) -> None:
+        raise NotImplementedError("Implement this in the derived class")
+
+    @abstractmethod
+    def add(self, obj_to_add: dict[str, None | str | float | int]) -> None:
+        raise NotImplementedError("Implement this in the derived class")
+
+    @abstractmethod
+    def modify(self, obj_to_modify: dict[str, None | str | float | int],
+               new_properties: dict[str, None | str | float | int]) -> None:
+        raise NotImplementedError("Implement this in the derived class")
+
+    @property
+    @abstractmethod
+    def table_header(self) -> str:
+        raise NotImplementedError("Implement this in the derived class")
+
+    @property
+    @abstractmethod
+    def table_footer(self) -> str:
+        raise NotImplementedError("Implement this in the derived class")
+
+    @property
+    @abstractmethod
+    def _network_element_name(self) -> str:
+        raise NotImplementedError("Implement this in the derived class")
```

### Comparing `ressimpy-1.0.0/ResSimpy/DynamicProperty.py` & `ressimpy-1.0.1/ResSimpy/DynamicProperty.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,49 +1,49 @@
-from abc import ABC
-from dataclasses import dataclass
-from typing import Optional
-from ResSimpy.File import File
-
-
-@dataclass
-class DynamicProperty(ABC):
-    """The abstract base class for dynamic property simulator inputs, for use in inputs such as PVT, relperm, etc.
-
-    Attributes:
-        input_number (int): Method, table or input number, in order as entered in the simulation input deck.
-    """
-
-    input_number: int
-    file: File
-
-    def __init__(self, input_number: int, file: File) -> None:
-        self.input_number: int = input_number
-        self.file: File = file
-
-    def __repr__(self) -> str:
-        """Pretty printing dynamic property data."""
-        printable_str = f'\nFILE_PATH: {self.file.location}\n\n'
-        printable_str += self.to_string()
-        return printable_str
-
-    def to_string(self) -> str:
-        """Write dynamic property data to string."""
-        raise NotImplementedError('Implement in the derived class.')
-
-    def write_to_file(self, overwrite_existing: bool = False, new_file_location: Optional[str] = None) -> None:
-        """Write dynamic property data to file."""
-        printable_str = self.to_string()
-        new_file_contents = printable_str.splitlines(keepends=True)
-        if overwrite_existing is True and new_file_location is not None:
-            raise ValueError('Please specify only one of either overwrite_existing or new_file_location.')
-
-        if new_file_location is not None:
-            new_file = File(file_content_as_list=new_file_contents, location=new_file_location)
-            new_file.write_to_file()
-            return
-        elif overwrite_existing is False:
-            raise ValueError('Please specify either overwrite_existing as True or provide new_file_location.')
-
-        # Overwriting existing file contents
-        if overwrite_existing is True:
-            self.file.file_content_as_list = new_file_contents
-            self.file.write_to_file()
+from abc import ABC
+from dataclasses import dataclass
+from typing import Optional
+from ResSimpy.File import File
+
+
+@dataclass
+class DynamicProperty(ABC):
+    """The abstract base class for dynamic property simulator inputs, for use in inputs such as PVT, relperm, etc.
+
+    Attributes:
+        input_number (int): Method, table or input number, in order as entered in the simulation input deck.
+    """
+
+    input_number: int
+    file: File
+
+    def __init__(self, input_number: int, file: File) -> None:
+        self.input_number: int = input_number
+        self.file: File = file
+
+    def __repr__(self) -> str:
+        """Pretty printing dynamic property data."""
+        printable_str = f'\nFILE_PATH: {self.file.location}\n\n'
+        printable_str += self.to_string()
+        return printable_str
+
+    def to_string(self) -> str:
+        """Write dynamic property data to string."""
+        raise NotImplementedError('Implement in the derived class.')
+
+    def write_to_file(self, overwrite_existing: bool = False, new_file_location: Optional[str] = None) -> None:
+        """Write dynamic property data to file."""
+        printable_str = self.to_string()
+        new_file_contents = printable_str.splitlines(keepends=True)
+        if overwrite_existing is True and new_file_location is not None:
+            raise ValueError('Please specify only one of either overwrite_existing or new_file_location.')
+
+        if new_file_location is not None:
+            new_file = File(file_content_as_list=new_file_contents, location=new_file_location)
+            new_file.write_to_file()
+            return
+        elif overwrite_existing is False:
+            raise ValueError('Please specify either overwrite_existing as True or provide new_file_location.')
+
+        # Overwriting existing file contents
+        if overwrite_existing is True:
+            self.file.file_content_as_list = new_file_contents
+            self.file.write_to_file()
```

### Comparing `ressimpy-1.0.0/ResSimpy/FileBase.py` & `ressimpy-1.0.1/ResSimpy/FileBase.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,53 +1,53 @@
-from abc import ABC, abstractmethod
-from dataclasses import dataclass, field
-from typing import Optional
-from uuid import UUID
-
-
-@dataclass
-class FileBase(ABC):
-    """The abstract base class for simulator files.
-
-    Attributes:
-        location (str): Full path to file location
-        file_content_as_list (list[str]): List of lines in the file
-    """
-
-    location: Optional[str] = None
-    file_content_as_list: Optional[list[str]] = field(default=None, repr=False)
-
-    @abstractmethod
-    def write_to_file(self) -> None:
-        raise NotImplementedError("Implement this in the derived class")
-
-    @property
-    @abstractmethod
-    def get_flat_list_str_file(self) -> list[str]:
-        raise NotImplementedError("Implement this in the derived class")
-
-    @abstractmethod
-    def add_object_locations(self, obj_uuid: UUID, line_indices: list[int]) -> None:
-        raise NotImplementedError("Implement this in the derived class")
-
-    @abstractmethod
-    def insert_comments(self, additional_content: list[str], comments) -> list[str]:
-        raise NotImplementedError("Implement this in the derived class")
-
-    @abstractmethod
-    def get_object_locations_for_id(self, obj_id: UUID) -> list[int]:
-        raise NotImplementedError("Implement this in the derived class")
-
-    @abstractmethod
-    def remove_object_from_file_as_list(self, objects_to_remove: list[UUID]) -> None:
-        raise NotImplementedError("Implement this in the derived class")
-
-    @abstractmethod
-    def add_to_file_as_list(self, additional_content: list[str], index: int,
-                            additional_objects: Optional[dict[UUID, list[int]]] = None,
-                            comments: Optional[str] = None) -> None:
-        raise NotImplementedError("Implement this in the derived class")
-
-    @abstractmethod
-    def remove_from_file_as_list(self, index: int, objects_to_remove: Optional[list[UUID]] = None,
-                                 string_to_remove: Optional[str] = None) -> None:
-        raise NotImplementedError("Implement this in the derived class")
+from abc import ABC, abstractmethod
+from dataclasses import dataclass, field
+from typing import Optional
+from uuid import UUID
+
+
+@dataclass
+class FileBase(ABC):
+    """The abstract base class for simulator files.
+
+    Attributes:
+        location (str): Full path to file location
+        file_content_as_list (list[str]): List of lines in the file
+    """
+
+    location: Optional[str] = None
+    file_content_as_list: Optional[list[str]] = field(default=None, repr=False)
+
+    @abstractmethod
+    def write_to_file(self) -> None:
+        raise NotImplementedError("Implement this in the derived class")
+
+    @property
+    @abstractmethod
+    def get_flat_list_str_file(self) -> list[str]:
+        raise NotImplementedError("Implement this in the derived class")
+
+    @abstractmethod
+    def add_object_locations(self, obj_uuid: UUID, line_indices: list[int]) -> None:
+        raise NotImplementedError("Implement this in the derived class")
+
+    @abstractmethod
+    def insert_comments(self, additional_content: list[str], comments) -> list[str]:
+        raise NotImplementedError("Implement this in the derived class")
+
+    @abstractmethod
+    def get_object_locations_for_id(self, obj_id: UUID) -> list[int]:
+        raise NotImplementedError("Implement this in the derived class")
+
+    @abstractmethod
+    def remove_object_from_file_as_list(self, objects_to_remove: list[UUID]) -> None:
+        raise NotImplementedError("Implement this in the derived class")
+
+    @abstractmethod
+    def add_to_file_as_list(self, additional_content: list[str], index: int,
+                            additional_objects: Optional[dict[UUID, list[int]]] = None,
+                            comments: Optional[str] = None) -> None:
+        raise NotImplementedError("Implement this in the derived class")
+
+    @abstractmethod
+    def remove_from_file_as_list(self, index: int, objects_to_remove: Optional[list[UUID]] = None,
+                                 string_to_remove: Optional[str] = None) -> None:
+        raise NotImplementedError("Implement this in the derived class")
```

### Comparing `ressimpy-1.0.0/ResSimpy/ISODateTime.py` & `ressimpy-1.0.1/ResSimpy/ISODateTime.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,56 +1,56 @@
-from typing import Optional
-from ResSimpy.Nexus.NexusEnums.DateFormatEnum import DateFormat
-from datetime import datetime, timedelta
-
-
-class ISODateTime(datetime):
-    """A class representing an extension of datetime class,  returns back date in ISO datetime format."""
-
-    def __repr__(self) -> str:
-        """Return the object representation, but formatted in ISO format."""
-        basic_string = super().__repr__()
-        iso_string = basic_string.replace(' ', 'T')
-        return iso_string
-
-    def __str__(self) -> str:
-        """Return the string representation, but formatted in ISO format."""
-        basic_string = super().__str__()
-        iso_string = basic_string.replace(' ', 'T')
-        return iso_string
-
-    @staticmethod
-    def isfloat(no_of_days: str) -> bool:
-        if no_of_days is not None:
-            try:
-                float(no_of_days)
-                return True
-            except ValueError:
-                return False
-        else:
-            return False
-
-    @classmethod
-    def convert_to_iso(cls, date: str, date_format: str, start_date: Optional[str] = None) -> 'ISODateTime':
-        converted_date = None
-
-        if date_format is None:
-            raise ValueError('Please provide date format')
-
-        if ISODateTime.isfloat(date) and start_date is None:
-            raise ValueError('Please provide start date when date is numeric')
-        elif ISODateTime.isfloat(date) and start_date is not None:
-            if date_format == DateFormat.DD_MM_YYYY:
-                converted_date = ISODateTime.strptime(start_date, '%d/%m/%Y') + timedelta(days=float(date))
-            elif date_format == DateFormat.MM_DD_YYYY:
-                converted_date = ISODateTime.strptime(start_date, '%m/%d/%Y') + timedelta(days=float(date))
-
-        elif date_format == DateFormat.DD_MM_YYYY:
-            converted_date = ISODateTime.strptime(date, '%d/%m/%Y')
-
-        elif date_format == DateFormat.MM_DD_YYYY:
-            converted_date = ISODateTime.strptime(date, '%m/%d/%Y')
-
-        if converted_date is None:
-            raise ValueError('Invalid date format or missing start_date.')
-
-        return converted_date
+from typing import Optional
+from ResSimpy.Nexus.NexusEnums.DateFormatEnum import DateFormat
+from datetime import datetime, timedelta
+
+
+class ISODateTime(datetime):
+    """A class representing an extension of datetime class,  returns back date in ISO datetime format."""
+
+    def __repr__(self) -> str:
+        """Return the object representation, but formatted in ISO format."""
+        basic_string = super().__repr__()
+        iso_string = basic_string.replace(' ', 'T')
+        return iso_string
+
+    def __str__(self) -> str:
+        """Return the string representation, but formatted in ISO format."""
+        basic_string = super().__str__()
+        iso_string = basic_string.replace(' ', 'T')
+        return iso_string
+
+    @staticmethod
+    def isfloat(no_of_days: str) -> bool:
+        if no_of_days is not None:
+            try:
+                float(no_of_days)
+                return True
+            except ValueError:
+                return False
+        else:
+            return False
+
+    @classmethod
+    def convert_to_iso(cls, date: str, date_format: str, start_date: Optional[str] = None) -> 'ISODateTime':
+        converted_date = None
+
+        if date_format is None:
+            raise ValueError('Please provide date format')
+
+        if ISODateTime.isfloat(date) and start_date is None:
+            raise ValueError('Please provide start date when date is numeric')
+        elif ISODateTime.isfloat(date) and start_date is not None:
+            if date_format == DateFormat.DD_MM_YYYY:
+                converted_date = ISODateTime.strptime(start_date, '%d/%m/%Y') + timedelta(days=float(date))
+            elif date_format == DateFormat.MM_DD_YYYY:
+                converted_date = ISODateTime.strptime(start_date, '%m/%d/%Y') + timedelta(days=float(date))
+
+        elif date_format == DateFormat.DD_MM_YYYY:
+            converted_date = ISODateTime.strptime(date, '%d/%m/%Y')
+
+        elif date_format == DateFormat.MM_DD_YYYY:
+            converted_date = ISODateTime.strptime(date, '%m/%d/%Y')
+
+        if converted_date is None:
+            raise ValueError('Invalid date format or missing start_date.')
+
+        return converted_date
```

### Comparing `ressimpy-1.0.0/ResSimpy/Nexus/array_function_operations.py` & `ressimpy-1.0.1/ResSimpy/Nexus/array_function_operations.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,289 +1,289 @@
-import ResSimpy.Nexus.nexus_file_operations as nfo
-import pandas as pd
-from typing import Union
-import warnings
-from ResSimpy.Nexus.NexusKeywords.structured_grid_keywords import GRID_ARRAY_KEYWORDS
-
-
-def collect_all_function_blocks(file_as_list: list[str]) -> list[list[str]]:
-    """Collects all the function blocks within a grid file.
-
-    Args:
-    file_as_list (list[str] | NexusFile): a list of strings containing each line of the file as an item,
-
-    Returns:
-    list[list[str]]: list of function block lines as a list of strings.
-    """
-    function_list = []
-    function_body: list[str] = []
-    reading_function = False
-
-    for i, line in enumerate(file_as_list):
-        if nfo.check_token('FUNCTION', line):
-            function_body = []
-            reading_function = True
-        if reading_function:
-            # remove all comments following the first '!' in a line.
-            modified_line = line.split('!', 1)[0]
-            function_body.append(modified_line.strip())
-            if nfo.check_token('OUTPUT', modified_line) and not nfo.check_token('RANGE', modified_line):
-                function_list.append(function_body)
-                reading_function = False
-    # remove null values
-    function_list = [list(filter(None, x)) for x in function_list]
-
-    return function_list
-
-
-def create_function_parameters_df(function_list_to_parse: list[list[str]]) -> pd.DataFrame:
-    """Creates a dataframe to hold all the function properties and parameters.
-
-    Args:
-        function_list_to_parse (list[list[str]]): list of functions extracted as list of lines.
-
-    Returns:
-        pandas.DataFrame: a dataframe holding each function's parameters in a row.
-    """
-
-    functions_df = pd.DataFrame(
-        columns=['FUNCTION #', 'blocks [i1,i2,j1,j2,k1,k2]', 'region_type',
-                 'region_numbers',
-                 'func_type', 'func_coeff', 'grid', 'range_input', 'range_output', 'drange',
-                 'input_arrays', 'output_arrays', 'i1', 'i2', 'j1', 'j2', 'k1', 'k2'])
-
-    for b, block in enumerate(function_list_to_parse):
-
-        # set the empty default values for the parameters,
-        # so if they don't exist in dataframe they won't appear as NaN or give error,
-        # or repeat the last value for each row.
-        i1 = i2 = j1 = j2 = k1 = k2 = region_type = function_type = grid_name = ''
-        # set the lists as empty strings as well, otherwise they show up as [] on the dataframe.
-        region_number_list: Union[str, list[str], list[int]] = ''
-        function_coefficients: Union[str, list[str], list[float]] = ''
-        input_arrays_min_max_list: Union[str, list[str], list[float]] = ''
-        output_arrays_min_max_list: Union[str, list[str], list[float]] = ''
-        input_array_list: Union[str, list[str]] = ''
-        output_array_list: Union[str, list[str]] = ''
-        drange_list: Union[str, list[str]] = ''
-        blocks_list: Union[str, list[str], list[int]] = ''
-
-        for li, line in enumerate(block):
-            modified_line = line.upper()
-            words = modified_line.split()
-            if 'BLOCKS' in modified_line:
-                i1 = words[1]
-                i2 = words[2]
-                j1 = words[3]
-                j2 = words[4]
-                k1 = words[5]
-                k2 = words[6]
-                blocks_list = words[1:7]
-                blocks_list = [round(float(i)) for i in blocks_list]
-
-            if 'FUNCTION' in modified_line:
-                if len(words) == 1:
-                    continue
-                if len(words) == 2:
-                    if words[1] not in GRID_ARRAY_KEYWORDS:
-                        warnings.warn(f'Function {b + 1}:  Function table entries will be excluded from summary df.')
-                        function_type = 'function table'
-                    else:
-                        region_type = words[1]
-                        region_number_list = block[li + 1].split()
-                        try:
-                            region_number_list = [round(float(i)) for i in region_number_list]
-                        except ValueError:
-                            warnings.warn(f'ValueError at function {b + 1}: could not convert string to integer.')
-
-                if len(words) > 2:  # TODO: deal with tabular function option keywords
-                    warnings.warn(f'Function {b + 1}:  Function table entries will be excluded from summary df.')
-                    function_type = 'function table'
-            if 'ANALYT' in modified_line:
-                function_type = words[1]
-                if len(words) > 2:
-                    # remove the first 2 words in line, and set the rest to coefficients
-                    function_coefficients = words[2:]
-                    # convert string coefficient values to numerical, if possible:
-                    try:
-                        function_coefficients = [float(i) for i in function_coefficients]
-                    except ValueError:
-                        warnings.warn(f'ValueError at function {b + 1}: could not convert string to float.')
-
-            if 'GRID' in modified_line:
-                grid_name = words[1]
-            if 'RANGE' in modified_line and 'INPUT' in modified_line:
-                input_arrays_min_max_list = words[2:]
-                # convert string range_input values to numerical, if possible:
-                try:
-                    input_arrays_min_max_list = [float(i) for i in input_arrays_min_max_list]
-                except ValueError:
-                    warnings.warn(f'ValueError at function {b + 1}: could not convert string to float.')
-            if 'RANGE' in modified_line and 'OUTPUT' in modified_line:
-                output_arrays_min_max_list = words[2:]
-                # convert string range_input values to numerical, if possible:
-                try:
-                    output_arrays_min_max_list = [float(i) for i in output_arrays_min_max_list]
-                except ValueError:
-                    warnings.warn(f'ValueError at function {b + 1}: could not convert string to float.')
-            if 'DRANGE' in modified_line:
-                warnings.warn(f'Function {b + 1}: Function table entries will be excluded from summary df.')
-                drange_list = words[1:]
-                function_type = 'function table'
-            if 'OUTPUT' in modified_line and 'RANGE' not in modified_line:
-                input_array_list = words[:words.index('OUTPUT')]
-                output_array_list = words[words.index('OUTPUT') + 1:]
-        # Create the row that holds function data
-        function_row = [b + 1, blocks_list, region_type, region_number_list, function_type,
-                        function_coefficients,
-                        grid_name, input_arrays_min_max_list, output_arrays_min_max_list, drange_list, input_array_list,
-                        output_array_list, i1, i2, j1, j2, k1, k2]
-        # Append the function row to the dataframe
-        functions_df.loc[len(functions_df)] = function_row
-    return functions_df
-
-
-def summarize_model_functions(function_list_to_parse: list[list[str]]) -> pd.DataFrame:
-    """Extracts all function parameters into a df, with an added column of human-readable notations for each function.
-
-    Args:
-        function_list_to_parse (list[list[str]]): list of functions extracted as list of lines.
-
-    Returns:
-        pandas.DataFrame: a dataframe holding each function's translation/summary in a row.
-    """
-
-    # get the df from create_function_parameters_df, add a new column, and populate based on ANALYT function type:
-
-    function_summary_df = create_function_parameters_df(function_list_to_parse)
-    function_summary_df['notation'] = ''
-
-    for index, row in function_summary_df.iterrows():
-
-        formula = row['output_arrays'][0] + ' = '
-
-        match row['func_type'].upper():
-            # ANALYT POLYN
-            case 'POLYN':
-                # get number of coefficients, n
-                n = len(row['func_coeff'])
-
-                # For each coefficient (c), calculate the corresponding exponent -or power (p)
-                # Create polynomial function notation, term by term, for any number of coefficients (n)
-                # using the first item in input arrays list (arr),
-                # and the position (x) of the function term/portion we are creating.
-                for x in range(n):
-                    c = row['func_coeff'][x]
-                    p = n - x - 1
-                    arr = row['input_arrays'][0]
-
-                    if n == 1:
-                        f_portion = f'{c}'
-
-                    if p == 0 and x > 0:
-                        if c > 0:
-                            f_portion = f' +{c}'
-                        elif c < 0:
-                            f_portion = f'{c}'
-                        else:
-                            continue
-
-                    if p == 1 and x > 0:
-                        if c > 0:
-                            f_portion = f' +{c}*{arr}'
-                        elif c < 0:
-                            f_portion = f'{c}*{arr}'
-                        else:
-                            continue
-
-                    if p == 1 and x == 0:
-                        if c != 0:
-                            f_portion = f'{c}*{arr}'
-                        else:
-                            continue
-
-                    if p > 1 and x > 0:
-                        if c > 0:
-                            f_portion = f' +{c}*({arr}^{p})'
-                        elif c < 0:
-                            f_portion = f'{c}*({arr}^{p})'
-                        else:
-                            continue
-
-                    if p > 1 and x == 0:
-                        if c != 0:
-                            f_portion = f'{c}*({arr}^{p})'
-                        else:
-                            continue
-
-                    formula += f_portion
-
-            # ANALYT ABS
-            case 'ABS':
-                formula += f"| {row['input_arrays'][0]} |"
-
-            # ANALYT EXP
-            case 'EXP':
-                formula += f"e^{row['input_arrays'][0]}"
-
-            # ANALYT EXP10
-            case 'EXP10':
-                formula += f"10^{row['input_arrays'][0]}"
-
-            # ANALYT LOG
-            case 'LOG':
-                formula += f"ln|{row['input_arrays'][0]}|"
-
-            # ANALYT LOG10
-            case 'LOG10':
-                formula += f"log10|{row['input_arrays'][0]}|"
-
-            # ANALYT SQRT
-            case 'SQRT':
-                formula += f"SQRT|{row['input_arrays'][0]}|"
-
-            # ANALYT GE
-            case 'GE':
-                formula += f"({row['input_arrays'][0]} if {row['input_arrays'][0]} >= {row['func_coeff'][0]}; " \
-                           f"{row['func_coeff'][1]} otherwise)"
-
-            # ANALYT LE
-            case 'LE':
-                formula += f"({row['input_arrays'][0]} if {row['input_arrays'][0]} <= {row['func_coeff'][0]}; " \
-                           f"{row['func_coeff'][1]} otherwise)"
-
-            # ANALYT ADD
-            case 'ADD':
-                formula += f"{row['input_arrays'][0]} + {row['input_arrays'][1]}"
-
-            # ANALYT SUBT
-            case 'SUBT':
-                formula += f"{row['input_arrays'][0]} - {row['input_arrays'][1]}"
-
-            # ANALYT DIV
-            case 'DIV':
-                formula += f"({row['input_arrays'][0]} / {row['input_arrays'][1]} if {row['input_arrays'][1]} != 0; " \
-                           f"{row['input_arrays'][0]} otherwise)"
-
-            # ANALYT MULT
-            case 'MULT':
-                formula += f"{row['input_arrays'][0]} * {row['input_arrays'][1]}"
-
-            # ANALYT MIN
-            case 'MIN':
-                formula += f"min({row['input_arrays'][0]}, {row['input_arrays'][1]})"
-
-            # ANALYT MAX
-            case 'MAX':
-                formula += f"max({row['input_arrays'][0]}, {row['input_arrays'][1]})"
-
-        # fill in the notation value for the row
-        function_summary_df.loc[index, 'notation'] = formula
-
-    # move notation column to the beginning of table:
-    second_column = function_summary_df.pop('notation')
-    function_summary_df.insert(1, 'notation', second_column)
-
-    # set FUNCTION number as the index colum:
-    function_summary_df = function_summary_df.set_index('FUNCTION #')
-
-    return function_summary_df
+import ResSimpy.Nexus.nexus_file_operations as nfo
+import pandas as pd
+from typing import Union
+import warnings
+from ResSimpy.Nexus.NexusKeywords.structured_grid_keywords import GRID_ARRAY_KEYWORDS
+
+
+def collect_all_function_blocks(file_as_list: list[str]) -> list[list[str]]:
+    """Collects all the function blocks within a grid file.
+
+    Args:
+    file_as_list (list[str] | NexusFile): a list of strings containing each line of the file as an item,
+
+    Returns:
+    list[list[str]]: list of function block lines as a list of strings.
+    """
+    function_list = []
+    function_body: list[str] = []
+    reading_function = False
+
+    for i, line in enumerate(file_as_list):
+        if nfo.check_token('FUNCTION', line):
+            function_body = []
+            reading_function = True
+        if reading_function:
+            # remove all comments following the first '!' in a line.
+            modified_line = line.split('!', 1)[0]
+            function_body.append(modified_line.strip())
+            if nfo.check_token('OUTPUT', modified_line) and not nfo.check_token('RANGE', modified_line):
+                function_list.append(function_body)
+                reading_function = False
+    # remove null values
+    function_list = [list(filter(None, x)) for x in function_list]
+
+    return function_list
+
+
+def create_function_parameters_df(function_list_to_parse: list[list[str]]) -> pd.DataFrame:
+    """Creates a dataframe to hold all the function properties and parameters.
+
+    Args:
+        function_list_to_parse (list[list[str]]): list of functions extracted as list of lines.
+
+    Returns:
+        pandas.DataFrame: a dataframe holding each function's parameters in a row.
+    """
+
+    functions_df = pd.DataFrame(
+        columns=['FUNCTION #', 'blocks [i1,i2,j1,j2,k1,k2]', 'region_type',
+                 'region_numbers',
+                 'func_type', 'func_coeff', 'grid', 'range_input', 'range_output', 'drange',
+                 'input_arrays', 'output_arrays', 'i1', 'i2', 'j1', 'j2', 'k1', 'k2'])
+
+    for b, block in enumerate(function_list_to_parse):
+
+        # set the empty default values for the parameters,
+        # so if they don't exist in dataframe they won't appear as NaN or give error,
+        # or repeat the last value for each row.
+        i1 = i2 = j1 = j2 = k1 = k2 = region_type = function_type = grid_name = ''
+        # set the lists as empty strings as well, otherwise they show up as [] on the dataframe.
+        region_number_list: Union[str, list[str], list[int]] = ''
+        function_coefficients: Union[str, list[str], list[float]] = ''
+        input_arrays_min_max_list: Union[str, list[str], list[float]] = ''
+        output_arrays_min_max_list: Union[str, list[str], list[float]] = ''
+        input_array_list: Union[str, list[str]] = ''
+        output_array_list: Union[str, list[str]] = ''
+        drange_list: Union[str, list[str]] = ''
+        blocks_list: Union[str, list[str], list[int]] = ''
+
+        for li, line in enumerate(block):
+            modified_line = line.upper()
+            words = modified_line.split()
+            if 'BLOCKS' in modified_line:
+                i1 = words[1]
+                i2 = words[2]
+                j1 = words[3]
+                j2 = words[4]
+                k1 = words[5]
+                k2 = words[6]
+                blocks_list = words[1:7]
+                blocks_list = [round(float(i)) for i in blocks_list]
+
+            if 'FUNCTION' in modified_line:
+                if len(words) == 1:
+                    continue
+                if len(words) == 2:
+                    if words[1] not in GRID_ARRAY_KEYWORDS:
+                        warnings.warn(f'Function {b + 1}:  Function table entries will be excluded from summary df.')
+                        function_type = 'function table'
+                    else:
+                        region_type = words[1]
+                        region_number_list = block[li + 1].split()
+                        try:
+                            region_number_list = [round(float(i)) for i in region_number_list]
+                        except ValueError:
+                            warnings.warn(f'ValueError at function {b + 1}: could not convert string to integer.')
+
+                if len(words) > 2:  # TODO: deal with tabular function option keywords
+                    warnings.warn(f'Function {b + 1}:  Function table entries will be excluded from summary df.')
+                    function_type = 'function table'
+            if 'ANALYT' in modified_line:
+                function_type = words[1]
+                if len(words) > 2:
+                    # remove the first 2 words in line, and set the rest to coefficients
+                    function_coefficients = words[2:]
+                    # convert string coefficient values to numerical, if possible:
+                    try:
+                        function_coefficients = [float(i) for i in function_coefficients]
+                    except ValueError:
+                        warnings.warn(f'ValueError at function {b + 1}: could not convert string to float.')
+
+            if 'GRID' in modified_line:
+                grid_name = words[1]
+            if 'RANGE' in modified_line and 'INPUT' in modified_line:
+                input_arrays_min_max_list = words[2:]
+                # convert string range_input values to numerical, if possible:
+                try:
+                    input_arrays_min_max_list = [float(i) for i in input_arrays_min_max_list]
+                except ValueError:
+                    warnings.warn(f'ValueError at function {b + 1}: could not convert string to float.')
+            if 'RANGE' in modified_line and 'OUTPUT' in modified_line:
+                output_arrays_min_max_list = words[2:]
+                # convert string range_input values to numerical, if possible:
+                try:
+                    output_arrays_min_max_list = [float(i) for i in output_arrays_min_max_list]
+                except ValueError:
+                    warnings.warn(f'ValueError at function {b + 1}: could not convert string to float.')
+            if 'DRANGE' in modified_line:
+                warnings.warn(f'Function {b + 1}: Function table entries will be excluded from summary df.')
+                drange_list = words[1:]
+                function_type = 'function table'
+            if 'OUTPUT' in modified_line and 'RANGE' not in modified_line:
+                input_array_list = words[:words.index('OUTPUT')]
+                output_array_list = words[words.index('OUTPUT') + 1:]
+        # Create the row that holds function data
+        function_row = [b + 1, blocks_list, region_type, region_number_list, function_type,
+                        function_coefficients,
+                        grid_name, input_arrays_min_max_list, output_arrays_min_max_list, drange_list, input_array_list,
+                        output_array_list, i1, i2, j1, j2, k1, k2]
+        # Append the function row to the dataframe
+        functions_df.loc[len(functions_df)] = function_row
+    return functions_df
+
+
+def summarize_model_functions(function_list_to_parse: list[list[str]]) -> pd.DataFrame:
+    """Extracts all function parameters into a df, with an added column of human-readable notations for each function.
+
+    Args:
+        function_list_to_parse (list[list[str]]): list of functions extracted as list of lines.
+
+    Returns:
+        pandas.DataFrame: a dataframe holding each function's translation/summary in a row.
+    """
+
+    # get the df from create_function_parameters_df, add a new column, and populate based on ANALYT function type:
+
+    function_summary_df = create_function_parameters_df(function_list_to_parse)
+    function_summary_df['notation'] = ''
+
+    for index, row in function_summary_df.iterrows():
+
+        formula = row['output_arrays'][0] + ' = '
+
+        match row['func_type'].upper():
+            # ANALYT POLYN
+            case 'POLYN':
+                # get number of coefficients, n
+                n = len(row['func_coeff'])
+
+                # For each coefficient (c), calculate the corresponding exponent -or power (p)
+                # Create polynomial function notation, term by term, for any number of coefficients (n)
+                # using the first item in input arrays list (arr),
+                # and the position (x) of the function term/portion we are creating.
+                for x in range(n):
+                    c = row['func_coeff'][x]
+                    p = n - x - 1
+                    arr = row['input_arrays'][0]
+
+                    if n == 1:
+                        f_portion = f'{c}'
+
+                    if p == 0 and x > 0:
+                        if c > 0:
+                            f_portion = f' +{c}'
+                        elif c < 0:
+                            f_portion = f'{c}'
+                        else:
+                            continue
+
+                    if p == 1 and x > 0:
+                        if c > 0:
+                            f_portion = f' +{c}*{arr}'
+                        elif c < 0:
+                            f_portion = f'{c}*{arr}'
+                        else:
+                            continue
+
+                    if p == 1 and x == 0:
+                        if c != 0:
+                            f_portion = f'{c}*{arr}'
+                        else:
+                            continue
+
+                    if p > 1 and x > 0:
+                        if c > 0:
+                            f_portion = f' +{c}*({arr}^{p})'
+                        elif c < 0:
+                            f_portion = f'{c}*({arr}^{p})'
+                        else:
+                            continue
+
+                    if p > 1 and x == 0:
+                        if c != 0:
+                            f_portion = f'{c}*({arr}^{p})'
+                        else:
+                            continue
+
+                    formula += f_portion
+
+            # ANALYT ABS
+            case 'ABS':
+                formula += f"| {row['input_arrays'][0]} |"
+
+            # ANALYT EXP
+            case 'EXP':
+                formula += f"e^{row['input_arrays'][0]}"
+
+            # ANALYT EXP10
+            case 'EXP10':
+                formula += f"10^{row['input_arrays'][0]}"
+
+            # ANALYT LOG
+            case 'LOG':
+                formula += f"ln|{row['input_arrays'][0]}|"
+
+            # ANALYT LOG10
+            case 'LOG10':
+                formula += f"log10|{row['input_arrays'][0]}|"
+
+            # ANALYT SQRT
+            case 'SQRT':
+                formula += f"SQRT|{row['input_arrays'][0]}|"
+
+            # ANALYT GE
+            case 'GE':
+                formula += f"({row['input_arrays'][0]} if {row['input_arrays'][0]} >= {row['func_coeff'][0]}; " \
+                           f"{row['func_coeff'][1]} otherwise)"
+
+            # ANALYT LE
+            case 'LE':
+                formula += f"({row['input_arrays'][0]} if {row['input_arrays'][0]} <= {row['func_coeff'][0]}; " \
+                           f"{row['func_coeff'][1]} otherwise)"
+
+            # ANALYT ADD
+            case 'ADD':
+                formula += f"{row['input_arrays'][0]} + {row['input_arrays'][1]}"
+
+            # ANALYT SUBT
+            case 'SUBT':
+                formula += f"{row['input_arrays'][0]} - {row['input_arrays'][1]}"
+
+            # ANALYT DIV
+            case 'DIV':
+                formula += f"({row['input_arrays'][0]} / {row['input_arrays'][1]} if {row['input_arrays'][1]} != 0; " \
+                           f"{row['input_arrays'][0]} otherwise)"
+
+            # ANALYT MULT
+            case 'MULT':
+                formula += f"{row['input_arrays'][0]} * {row['input_arrays'][1]}"
+
+            # ANALYT MIN
+            case 'MIN':
+                formula += f"min({row['input_arrays'][0]}, {row['input_arrays'][1]})"
+
+            # ANALYT MAX
+            case 'MAX':
+                formula += f"max({row['input_arrays'][0]}, {row['input_arrays'][1]})"
+
+        # fill in the notation value for the row
+        function_summary_df.loc[index, 'notation'] = formula
+
+    # move notation column to the beginning of table:
+    second_column = function_summary_df.pop('notation')
+    function_summary_df.insert(1, 'notation', second_column)
+
+    # set FUNCTION number as the index colum:
+    function_summary_df = function_summary_df.set_index('FUNCTION #')
+
+    return function_summary_df
```

### Comparing `ressimpy-1.0.0/ResSimpy/Nexus/DataModels/FcsConfig.py` & `ressimpy-1.0.1/ResSimpy/Nexus/DataModels/FcsConfig.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-from dataclasses import dataclass
-
-
-@dataclass
-class FcsConfig:
-    def __init__(self, destination, nexus_data_name="data") -> None:
-        self.output_dir = destination
-        self.use_reservoir_names = True
-        self.abs_paths_to_keep: list[str] = []
-        self.use_one_dir = True
-        self.input_data_dir = ''
-        self.path_components_to_keep = None
-        self.locals_to_data = True
-        self.output_data_dir = nexus_data_name
-        self.dry_run = False
-        self.compress = False
-        self.output_log_file = False
+from dataclasses import dataclass
+
+
+@dataclass
+class FcsConfig:
+    def __init__(self, destination, nexus_data_name="data") -> None:
+        self.output_dir = destination
+        self.use_reservoir_names = True
+        self.abs_paths_to_keep: list[str] = []
+        self.use_one_dir = True
+        self.input_data_dir = ''
+        self.path_components_to_keep = None
+        self.locals_to_data = True
+        self.output_data_dir = nexus_data_name
+        self.dry_run = False
+        self.compress = False
+        self.output_log_file = False
```

### Comparing `ressimpy-1.0.0/ResSimpy/Nexus/DataModels/FcsFile.py` & `ressimpy-1.0.1/ResSimpy/Nexus/DataModels/FcsFile.py`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,241 +1,241 @@
-from __future__ import annotations
-from dataclasses import dataclass, field
-import os
-import warnings
-
-from ResSimpy.Nexus.DataModels.NexusFile import NexusFile
-from typing import Optional
-
-# Use correct Self type depending upon Python version
-import sys
-if sys.version_info >= (3, 11):
-    from typing import Self
-else:
-    from typing_extensions import Self
-
-from ResSimpy.Utils.factory_methods import get_empty_dict_int_nexus_file, get_empty_list_str, \
-    get_empty_list_nexus_file
-from ResSimpy.Nexus.NexusKeywords.fcs_keywords import FCS_KEYWORDS
-import ResSimpy.Nexus.nexus_file_operations as nfo
-from ResSimpy.Utils.generic_repr import generic_repr
-from datetime import datetime
-
-
-@dataclass(kw_only=True)
-class FcsNexusFile(NexusFile):
-    restart_file: Optional[NexusFile] = None
-    structured_grid_file: Optional[NexusFile] = None
-    options_file: Optional[NexusFile] = None
-    runcontrol_file: Optional[NexusFile] = None
-    override_file: Optional[NexusFile] = None
-    eos_default_file: Optional[NexusFile] = None
-    well_files: Optional[dict[int, NexusFile]] = field(default_factory=get_empty_dict_int_nexus_file)
-    surface_files: Optional[dict[int, NexusFile]] = field(default_factory=get_empty_dict_int_nexus_file)
-    rock_files: Optional[dict[int, NexusFile]] = field(default_factory=get_empty_dict_int_nexus_file)
-    relperm_files: Optional[dict[int, NexusFile]] = field(default_factory=get_empty_dict_int_nexus_file)
-    pvt_files: Optional[dict[int, NexusFile]] = field(default_factory=get_empty_dict_int_nexus_file)
-    water_files: Optional[dict[int, NexusFile]] = field(default_factory=get_empty_dict_int_nexus_file)
-    equil_files: Optional[dict[int, NexusFile]] = field(default_factory=get_empty_dict_int_nexus_file)
-    tracer_init_files: Optional[dict[int, NexusFile]] = field(default_factory=get_empty_dict_int_nexus_file)
-    aquifer_files: Optional[dict[int, NexusFile]] = field(default_factory=get_empty_dict_int_nexus_file)
-    hyd_files: Optional[dict[int, NexusFile]] = field(default_factory=get_empty_dict_int_nexus_file)
-    valve_files: Optional[dict[int, NexusFile]] = field(default_factory=get_empty_dict_int_nexus_file)
-    separator_files: Optional[dict[int, NexusFile]] = field(default_factory=get_empty_dict_int_nexus_file)
-    ipr_files: Optional[dict[int, NexusFile]] = field(default_factory=get_empty_dict_int_nexus_file)
-    gas_lift_files: Optional[dict[int, NexusFile]] = field(default_factory=get_empty_dict_int_nexus_file)
-    pump_files: Optional[dict[int, NexusFile]] = field(default_factory=get_empty_dict_int_nexus_file)
-    compressor_files: Optional[dict[int, NexusFile]] = field(default_factory=get_empty_dict_int_nexus_file)
-    choke_files: Optional[dict[int, NexusFile]] = field(default_factory=get_empty_dict_int_nexus_file)
-    icd_files: Optional[dict[int, NexusFile]] = field(default_factory=get_empty_dict_int_nexus_file)
-    esp_files: Optional[dict[int, NexusFile]] = field(default_factory=get_empty_dict_int_nexus_file)
-    polymer_files: Optional[dict[int, NexusFile]] = field(default_factory=get_empty_dict_int_nexus_file)
-    adsorption_files: Optional[dict[int, NexusFile]] = field(default_factory=get_empty_dict_int_nexus_file)
-    flux_in_files: Optional[dict[int, NexusFile]] = field(default_factory=get_empty_dict_int_nexus_file)
-    files_info: list[tuple[Optional[str], Optional[str], Optional[datetime]]]
-
-    def __init__(
-            self, location: Optional[str] = None,
-            include_locations: Optional[list[str]] = None,
-            origin: Optional[str] = None,
-            include_objects: Optional[list[NexusFile]] = None,
-            file_content_as_list: Optional[list[str]] = None,
-            restart_file: Optional[NexusFile] = None,
-            structured_grid_file: Optional[NexusFile] = None,
-            options_file: Optional[NexusFile] = None,
-            runcontrol_file: Optional[NexusFile] = None,
-            override_file: Optional[NexusFile] = None,
-            eos_default_file: Optional[NexusFile] = None,
-            well_files: Optional[dict[int, NexusFile]] = None,
-            surface_files: Optional[dict[int, NexusFile]] = None,
-            rock_files: Optional[dict[int, NexusFile]] = None,
-            relperm_files: Optional[dict[int, NexusFile]] = None,
-            pvt_files: Optional[dict[int, NexusFile]] = None,
-            water_files: Optional[dict[int, NexusFile]] = None,
-            equil_files: Optional[dict[int, NexusFile]] = None,
-            tracer_init_files: Optional[dict[int, NexusFile]] = None,
-            aquifer_files: Optional[dict[int, NexusFile]] = None,
-            hyd_files: Optional[dict[int, NexusFile]] = None,
-            valve_files: Optional[dict[int, NexusFile]] = None,
-            separator_files: Optional[dict[int, NexusFile]] = None,
-            ipr_files: Optional[dict[int, NexusFile]] = None,
-            gas_lift_files: Optional[dict[int, NexusFile]] = None,
-            pump_files: Optional[dict[int, NexusFile]] = None,
-            compressor_files: Optional[dict[int, NexusFile]] = None,
-            choke_files: Optional[dict[int, NexusFile]] = None,
-            icd_files: Optional[dict[int, NexusFile]] = None,
-            esp_files: Optional[dict[int, NexusFile]] = None,
-            polymer_files: Optional[dict[int, NexusFile]] = None,
-            adsorption_files: Optional[dict[int, NexusFile]] = None,
-            flux_in_files: Optional[dict[int, NexusFile]] = None
-            ) -> None:
-        self.restart_file = restart_file
-        self.structured_grid_file = structured_grid_file
-        self.options_file = options_file
-        self.runcontrol_file = runcontrol_file
-        self.override_file = override_file
-        self.eos_default_file = eos_default_file
-        self.surface_files = surface_files
-        self.well_files = well_files if well_files is not None else get_empty_dict_int_nexus_file()
-        self.rock_files = rock_files if rock_files is not None else get_empty_dict_int_nexus_file()
-        self.relperm_files = relperm_files if relperm_files is not None else get_empty_dict_int_nexus_file()
-        self.pvt_files = pvt_files if pvt_files is not None else get_empty_dict_int_nexus_file()
-        self.water_files = water_files if water_files is not None else get_empty_dict_int_nexus_file()
-        self.equil_files = equil_files if equil_files is not None else get_empty_dict_int_nexus_file()
-        self.tracer_init_files = tracer_init_files if tracer_init_files is not None else get_empty_dict_int_nexus_file()
-        self.aquifer_files = aquifer_files if aquifer_files is not None else get_empty_dict_int_nexus_file()
-        self.hyd_files = hyd_files if hyd_files is not None else get_empty_dict_int_nexus_file()
-        self.valve_files = valve_files if valve_files is not None else get_empty_dict_int_nexus_file()
-        self.separator_files = separator_files if separator_files is not None else get_empty_dict_int_nexus_file()
-        self.ipr_files = ipr_files if ipr_files is not None else get_empty_dict_int_nexus_file()
-        self.gas_lift_files = gas_lift_files if gas_lift_files is not None else get_empty_dict_int_nexus_file()
-        self.pump_files = pump_files if pump_files is not None else get_empty_dict_int_nexus_file()
-        self.compressor_files = compressor_files if compressor_files is not None else get_empty_dict_int_nexus_file()
-        self.choke_files = choke_files if choke_files is not None else get_empty_dict_int_nexus_file()
-        self.icd_files = icd_files if icd_files is not None else get_empty_dict_int_nexus_file()
-        self.esp_files = esp_files if esp_files is not None else get_empty_dict_int_nexus_file()
-        self.polymer_files = polymer_files if polymer_files is not None else get_empty_dict_int_nexus_file()
-        self.adsorption_files = adsorption_files if adsorption_files is not None else get_empty_dict_int_nexus_file()
-        self.flux_in_files = flux_in_files if flux_in_files is not None else get_empty_dict_int_nexus_file()
-        self.files_info = []
-        super().__init__(location=location, include_locations=include_locations, origin=origin,
-                         include_objects=include_objects, file_content_as_list=file_content_as_list)
-
-    def __repr__(self) -> str:
-        return generic_repr(self)
-
-    @classmethod
-    def generate_fcs_structure(cls, fcs_file_path: str, recursive: bool = True) -> Self:
-        """Creates an instance of the FcsNexusFile, populates it through looking through the different keywords \
-            in the FCS and assigning the paths to objects.
-
-        Args:
-        ----
-            fcs_file_path (str): path to the fcs file of interest
-            recursive (bool, optional): Whether the NexusFile structure will be recursively created. Defaults to True.
-
-        Raises:
-        ------
-            FileNotFoundError: if the fcs file cannot be found
-            ValueError: if no content can be found within the fcsfile
-
-        Returns:
-        -------
-            FcsNexusFile: instance of a FcsNexusFile for a given fcs file path
-        """
-        fcs_file = cls(location=fcs_file_path)
-        fcs_file.include_objects = get_empty_list_nexus_file()
-        fcs_file.file_content_as_list = get_empty_list_str()
-        fcs_file.include_locations = get_empty_list_str()
-
-        fcs_keyword_map_single = {
-            'STRUCTURED_GRID': 'structured_grid_file',
-            'OPTIONS': 'options_file',
-            'RUNCONTROL': 'runcontrol_file',
-            'OVERRIDE': 'override_file',
-            'EOS_DEFAULTS': 'eos_default_file',
-            }
-        fcs_keyword_map_multi = {
-            'EQUIL': 'equil_files',
-            'ROCK': 'rock_files',
-            'RELPM': 'relperm_files',
-            'SURFACE': 'surface_files',
-            'WELLS': 'well_files',
-            'PVT': 'pvt_files',
-            'AQUIFER': 'aquifer_files',
-            'HYD': 'hyd_files',
-            'VALVE': 'valve_files',
-            'WATER': 'water_files',
-            'SEPARATOR': 'separator_files',
-            'IPR': 'ipr_files',
-            'GASLIFT': 'gas_lift_files',
-            'PUMP': 'pump_files',
-            'COMPRESSOR': 'compressor_files',
-            'CHOKE': 'choke_files',
-            'ICD': 'icd_files',
-            'ESP': 'esp_files',
-            'POLYMER': 'polymer_files',
-            'ADSORPTION': 'adsorption_files',
-            'FLUXIN': 'flux_in_files',
-            'TRACER_INIT': 'tracer_init_files',
-            }
-
-        # guard against bad links/empty files:
-        if not os.path.isfile(fcs_file_path):
-            raise FileNotFoundError(f'fcs file not found for path {fcs_file_path}')
-        origin_path = fcs_file_path
-        fcs_nexus_file = NexusFile.generate_file_include_structure(
-            fcs_file_path, origin=None)
-        fcs_file.files_info.append((fcs_nexus_file.location, fcs_nexus_file.linked_user,
-                                   fcs_nexus_file.last_modified))
-        flat_fcs_file_content = fcs_nexus_file.get_flat_list_str_file
-        if flat_fcs_file_content is None or fcs_file.file_content_as_list is None:
-            raise ValueError(f'FCS file not found, no content for {fcs_file_path=}')
-        fcs_file.file_content_as_list = flat_fcs_file_content
-        for i, line in enumerate(flat_fcs_file_content):
-            if not nfo.nexus_token_found(line, valid_list=FCS_KEYWORDS):
-                continue
-            key = nfo.get_next_value(start_line_index=i, file_as_list=flat_fcs_file_content, search_string=line)
-            if key is None:
-                warnings.warn(f'get next value failed to find a suitable token in {line}')
-                continue
-            key = key.upper()
-            value = nfo.get_token_value(key, line, flat_fcs_file_content[i::])
-            if value is None:
-                warnings.warn(f'No value found for {key}, skipping file')
-                continue
-            # TODO handle methods / sets instead of getting full file path
-            if key in fcs_keyword_map_multi:
-                # for keywords that have multiple methods we store the value in a dictionary
-                # with the method number and the NexusFile object
-                _, method_string, method_number, value = (
-                    nfo.get_multiple_sequential_values(flat_fcs_file_content[i::], 4)
-                    )
-                full_file_path = nfo.get_full_file_path(value, origin_path)
-                nexus_file = NexusFile.generate_file_include_structure(
-                    value, origin=fcs_file_path, recursive=recursive, top_level_file=True)
-                fcs_property = getattr(fcs_file, fcs_keyword_map_multi[key])
-                # manually initialise if the property is still a None after class instantiation
-                if fcs_property is None:
-                    fcs_property = get_empty_dict_int_nexus_file()
-                # shallow copy to maintain list elements pointing to nexus_file that are
-                # stored in the file_content_as_list
-                fcs_property_list = fcs_property.copy()
-                fcs_property_list.update({int(method_number): nexus_file})
-                # set the attribute in the FcsNexusFile instance
-                setattr(fcs_file, fcs_keyword_map_multi[key], fcs_property_list)
-                fcs_file.include_objects.append(nexus_file)
-                fcs_file.include_locations.append(full_file_path)
-                fcs_file.files_info.append((nexus_file.location, nexus_file.linked_user,
-                                           nexus_file.last_modified))
-            elif key in fcs_keyword_map_single:
-                full_file_path = nfo.get_full_file_path(value, origin_path)
-                nexus_file = NexusFile.generate_file_include_structure(
-                    value, origin=fcs_file_path, recursive=recursive, top_level_file=True)
-                setattr(fcs_file, fcs_keyword_map_single[key], nexus_file)
-                fcs_file.include_objects.append(nexus_file)
-                fcs_file.include_locations.append(full_file_path)
-                fcs_file.files_info.append((nexus_file.location, nexus_file.linked_user,
-                                           nexus_file.last_modified))
-            else:
-                continue
-        return fcs_file
+from __future__ import annotations
+from dataclasses import dataclass, field
+import os
+import warnings
+
+from ResSimpy.Nexus.DataModels.NexusFile import NexusFile
+from typing import Optional
+
+# Use correct Self type depending upon Python version
+import sys
+if sys.version_info >= (3, 11):
+    from typing import Self
+else:
+    from typing_extensions import Self
+
+from ResSimpy.Utils.factory_methods import get_empty_dict_int_nexus_file, get_empty_list_str, \
+    get_empty_list_nexus_file
+from ResSimpy.Nexus.NexusKeywords.fcs_keywords import FCS_KEYWORDS
+import ResSimpy.Nexus.nexus_file_operations as nfo
+from ResSimpy.Utils.generic_repr import generic_repr
+from datetime import datetime
+
+
+@dataclass(kw_only=True)
+class FcsNexusFile(NexusFile):
+    restart_file: Optional[NexusFile] = None
+    structured_grid_file: Optional[NexusFile] = None
+    options_file: Optional[NexusFile] = None
+    runcontrol_file: Optional[NexusFile] = None
+    override_file: Optional[NexusFile] = None
+    eos_default_file: Optional[NexusFile] = None
+    well_files: Optional[dict[int, NexusFile]] = field(default_factory=get_empty_dict_int_nexus_file)
+    surface_files: Optional[dict[int, NexusFile]] = field(default_factory=get_empty_dict_int_nexus_file)
+    rock_files: Optional[dict[int, NexusFile]] = field(default_factory=get_empty_dict_int_nexus_file)
+    relperm_files: Optional[dict[int, NexusFile]] = field(default_factory=get_empty_dict_int_nexus_file)
+    pvt_files: Optional[dict[int, NexusFile]] = field(default_factory=get_empty_dict_int_nexus_file)
+    water_files: Optional[dict[int, NexusFile]] = field(default_factory=get_empty_dict_int_nexus_file)
+    equil_files: Optional[dict[int, NexusFile]] = field(default_factory=get_empty_dict_int_nexus_file)
+    tracer_init_files: Optional[dict[int, NexusFile]] = field(default_factory=get_empty_dict_int_nexus_file)
+    aquifer_files: Optional[dict[int, NexusFile]] = field(default_factory=get_empty_dict_int_nexus_file)
+    hyd_files: Optional[dict[int, NexusFile]] = field(default_factory=get_empty_dict_int_nexus_file)
+    valve_files: Optional[dict[int, NexusFile]] = field(default_factory=get_empty_dict_int_nexus_file)
+    separator_files: Optional[dict[int, NexusFile]] = field(default_factory=get_empty_dict_int_nexus_file)
+    ipr_files: Optional[dict[int, NexusFile]] = field(default_factory=get_empty_dict_int_nexus_file)
+    gas_lift_files: Optional[dict[int, NexusFile]] = field(default_factory=get_empty_dict_int_nexus_file)
+    pump_files: Optional[dict[int, NexusFile]] = field(default_factory=get_empty_dict_int_nexus_file)
+    compressor_files: Optional[dict[int, NexusFile]] = field(default_factory=get_empty_dict_int_nexus_file)
+    choke_files: Optional[dict[int, NexusFile]] = field(default_factory=get_empty_dict_int_nexus_file)
+    icd_files: Optional[dict[int, NexusFile]] = field(default_factory=get_empty_dict_int_nexus_file)
+    esp_files: Optional[dict[int, NexusFile]] = field(default_factory=get_empty_dict_int_nexus_file)
+    polymer_files: Optional[dict[int, NexusFile]] = field(default_factory=get_empty_dict_int_nexus_file)
+    adsorption_files: Optional[dict[int, NexusFile]] = field(default_factory=get_empty_dict_int_nexus_file)
+    flux_in_files: Optional[dict[int, NexusFile]] = field(default_factory=get_empty_dict_int_nexus_file)
+    files_info: list[tuple[Optional[str], Optional[str], Optional[datetime]]]
+
+    def __init__(
+            self, location: Optional[str] = None,
+            include_locations: Optional[list[str]] = None,
+            origin: Optional[str] = None,
+            include_objects: Optional[list[NexusFile]] = None,
+            file_content_as_list: Optional[list[str]] = None,
+            restart_file: Optional[NexusFile] = None,
+            structured_grid_file: Optional[NexusFile] = None,
+            options_file: Optional[NexusFile] = None,
+            runcontrol_file: Optional[NexusFile] = None,
+            override_file: Optional[NexusFile] = None,
+            eos_default_file: Optional[NexusFile] = None,
+            well_files: Optional[dict[int, NexusFile]] = None,
+            surface_files: Optional[dict[int, NexusFile]] = None,
+            rock_files: Optional[dict[int, NexusFile]] = None,
+            relperm_files: Optional[dict[int, NexusFile]] = None,
+            pvt_files: Optional[dict[int, NexusFile]] = None,
+            water_files: Optional[dict[int, NexusFile]] = None,
+            equil_files: Optional[dict[int, NexusFile]] = None,
+            tracer_init_files: Optional[dict[int, NexusFile]] = None,
+            aquifer_files: Optional[dict[int, NexusFile]] = None,
+            hyd_files: Optional[dict[int, NexusFile]] = None,
+            valve_files: Optional[dict[int, NexusFile]] = None,
+            separator_files: Optional[dict[int, NexusFile]] = None,
+            ipr_files: Optional[dict[int, NexusFile]] = None,
+            gas_lift_files: Optional[dict[int, NexusFile]] = None,
+            pump_files: Optional[dict[int, NexusFile]] = None,
+            compressor_files: Optional[dict[int, NexusFile]] = None,
+            choke_files: Optional[dict[int, NexusFile]] = None,
+            icd_files: Optional[dict[int, NexusFile]] = None,
+            esp_files: Optional[dict[int, NexusFile]] = None,
+            polymer_files: Optional[dict[int, NexusFile]] = None,
+            adsorption_files: Optional[dict[int, NexusFile]] = None,
+            flux_in_files: Optional[dict[int, NexusFile]] = None
+            ) -> None:
+        self.restart_file = restart_file
+        self.structured_grid_file = structured_grid_file
+        self.options_file = options_file
+        self.runcontrol_file = runcontrol_file
+        self.override_file = override_file
+        self.eos_default_file = eos_default_file
+        self.surface_files = surface_files
+        self.well_files = well_files if well_files is not None else get_empty_dict_int_nexus_file()
+        self.rock_files = rock_files if rock_files is not None else get_empty_dict_int_nexus_file()
+        self.relperm_files = relperm_files if relperm_files is not None else get_empty_dict_int_nexus_file()
+        self.pvt_files = pvt_files if pvt_files is not None else get_empty_dict_int_nexus_file()
+        self.water_files = water_files if water_files is not None else get_empty_dict_int_nexus_file()
+        self.equil_files = equil_files if equil_files is not None else get_empty_dict_int_nexus_file()
+        self.tracer_init_files = tracer_init_files if tracer_init_files is not None else get_empty_dict_int_nexus_file()
+        self.aquifer_files = aquifer_files if aquifer_files is not None else get_empty_dict_int_nexus_file()
+        self.hyd_files = hyd_files if hyd_files is not None else get_empty_dict_int_nexus_file()
+        self.valve_files = valve_files if valve_files is not None else get_empty_dict_int_nexus_file()
+        self.separator_files = separator_files if separator_files is not None else get_empty_dict_int_nexus_file()
+        self.ipr_files = ipr_files if ipr_files is not None else get_empty_dict_int_nexus_file()
+        self.gas_lift_files = gas_lift_files if gas_lift_files is not None else get_empty_dict_int_nexus_file()
+        self.pump_files = pump_files if pump_files is not None else get_empty_dict_int_nexus_file()
+        self.compressor_files = compressor_files if compressor_files is not None else get_empty_dict_int_nexus_file()
+        self.choke_files = choke_files if choke_files is not None else get_empty_dict_int_nexus_file()
+        self.icd_files = icd_files if icd_files is not None else get_empty_dict_int_nexus_file()
+        self.esp_files = esp_files if esp_files is not None else get_empty_dict_int_nexus_file()
+        self.polymer_files = polymer_files if polymer_files is not None else get_empty_dict_int_nexus_file()
+        self.adsorption_files = adsorption_files if adsorption_files is not None else get_empty_dict_int_nexus_file()
+        self.flux_in_files = flux_in_files if flux_in_files is not None else get_empty_dict_int_nexus_file()
+        self.files_info = []
+        super().__init__(location=location, include_locations=include_locations, origin=origin,
+                         include_objects=include_objects, file_content_as_list=file_content_as_list)
+
+    def __repr__(self) -> str:
+        return generic_repr(self)
+
+    @classmethod
+    def generate_fcs_structure(cls, fcs_file_path: str, recursive: bool = True) -> Self:
+        """Creates an instance of the FcsNexusFile, populates it through looking through the different keywords \
+            in the FCS and assigning the paths to objects.
+
+        Args:
+        ----
+            fcs_file_path (str): path to the fcs file of interest
+            recursive (bool, optional): Whether the NexusFile structure will be recursively created. Defaults to True.
+
+        Raises:
+        ------
+            FileNotFoundError: if the fcs file cannot be found
+            ValueError: if no content can be found within the fcsfile
+
+        Returns:
+        -------
+            FcsNexusFile: instance of a FcsNexusFile for a given fcs file path
+        """
+        fcs_file = cls(location=fcs_file_path)
+        fcs_file.include_objects = get_empty_list_nexus_file()
+        fcs_file.file_content_as_list = get_empty_list_str()
+        fcs_file.include_locations = get_empty_list_str()
+
+        fcs_keyword_map_single = {
+            'STRUCTURED_GRID': 'structured_grid_file',
+            'OPTIONS': 'options_file',
+            'RUNCONTROL': 'runcontrol_file',
+            'OVERRIDE': 'override_file',
+            'EOS_DEFAULTS': 'eos_default_file',
+            }
+        fcs_keyword_map_multi = {
+            'EQUIL': 'equil_files',
+            'ROCK': 'rock_files',
+            'RELPM': 'relperm_files',
+            'SURFACE': 'surface_files',
+            'WELLS': 'well_files',
+            'PVT': 'pvt_files',
+            'AQUIFER': 'aquifer_files',
+            'HYD': 'hyd_files',
+            'VALVE': 'valve_files',
+            'WATER': 'water_files',
+            'SEPARATOR': 'separator_files',
+            'IPR': 'ipr_files',
+            'GASLIFT': 'gas_lift_files',
+            'PUMP': 'pump_files',
+            'COMPRESSOR': 'compressor_files',
+            'CHOKE': 'choke_files',
+            'ICD': 'icd_files',
+            'ESP': 'esp_files',
+            'POLYMER': 'polymer_files',
+            'ADSORPTION': 'adsorption_files',
+            'FLUXIN': 'flux_in_files',
+            'TRACER_INIT': 'tracer_init_files',
+            }
+
+        # guard against bad links/empty files:
+        if not os.path.isfile(fcs_file_path):
+            raise FileNotFoundError(f'fcs file not found for path {fcs_file_path}')
+        origin_path = fcs_file_path
+        fcs_nexus_file = NexusFile.generate_file_include_structure(
+            fcs_file_path, origin=None)
+        fcs_file.files_info.append((fcs_nexus_file.location, fcs_nexus_file.linked_user,
+                                   fcs_nexus_file.last_modified))
+        flat_fcs_file_content = fcs_nexus_file.get_flat_list_str_file
+        if flat_fcs_file_content is None or fcs_file.file_content_as_list is None:
+            raise ValueError(f'FCS file not found, no content for {fcs_file_path=}')
+        fcs_file.file_content_as_list = flat_fcs_file_content
+        for i, line in enumerate(flat_fcs_file_content):
+            if not nfo.nexus_token_found(line, valid_list=FCS_KEYWORDS):
+                continue
+            key = nfo.get_next_value(start_line_index=i, file_as_list=flat_fcs_file_content, search_string=line)
+            if key is None:
+                warnings.warn(f'get next value failed to find a suitable token in {line}')
+                continue
+            key = key.upper()
+            value = nfo.get_token_value(key, line, flat_fcs_file_content[i::])
+            if value is None:
+                warnings.warn(f'No value found for {key}, skipping file')
+                continue
+            # TODO handle methods / sets instead of getting full file path
+            if key in fcs_keyword_map_multi:
+                # for keywords that have multiple methods we store the value in a dictionary
+                # with the method number and the NexusFile object
+                _, method_string, method_number, value = (
+                    nfo.get_multiple_sequential_values(flat_fcs_file_content[i::], 4)
+                    )
+                full_file_path = nfo.get_full_file_path(value, origin_path)
+                nexus_file = NexusFile.generate_file_include_structure(
+                    value, origin=fcs_file_path, recursive=recursive, top_level_file=True)
+                fcs_property = getattr(fcs_file, fcs_keyword_map_multi[key])
+                # manually initialise if the property is still a None after class instantiation
+                if fcs_property is None:
+                    fcs_property = get_empty_dict_int_nexus_file()
+                # shallow copy to maintain list elements pointing to nexus_file that are
+                # stored in the file_content_as_list
+                fcs_property_list = fcs_property.copy()
+                fcs_property_list.update({int(method_number): nexus_file})
+                # set the attribute in the FcsNexusFile instance
+                setattr(fcs_file, fcs_keyword_map_multi[key], fcs_property_list)
+                fcs_file.include_objects.append(nexus_file)
+                fcs_file.include_locations.append(full_file_path)
+                fcs_file.files_info.append((nexus_file.location, nexus_file.linked_user,
+                                           nexus_file.last_modified))
+            elif key in fcs_keyword_map_single:
+                full_file_path = nfo.get_full_file_path(value, origin_path)
+                nexus_file = NexusFile.generate_file_include_structure(
+                    value, origin=fcs_file_path, recursive=recursive, top_level_file=True)
+                setattr(fcs_file, fcs_keyword_map_single[key], nexus_file)
+                fcs_file.include_objects.append(nexus_file)
+                fcs_file.include_locations.append(full_file_path)
+                fcs_file.files_info.append((nexus_file.location, nexus_file.linked_user,
+                                           nexus_file.last_modified))
+            else:
+                continue
+        return fcs_file
```

### Comparing `ressimpy-1.0.0/ResSimpy/Nexus/DataModels/Network/NexusConstraint.py` & `ressimpy-1.0.1/ResSimpy/Nexus/DataModels/Network/NexusConstraint.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,432 +1,432 @@
-from dataclasses import dataclass
-from typing import Optional
-
-from ResSimpy.Constraint import Constraint
-from ResSimpy.Enums.UnitsEnum import UnitSystem
-from ResSimpy.Utils import to_dict_generic
-
-
-@dataclass
-class NexusConstraint(Constraint):
-    """Attributes:
-    name (str): name of the well (NAME)
-    max_surface_oil_rate (float): max surface oil rate (QOSMAX)
-    max_surface_gas_rate (float): max surface gas rate (QGSMAX)
-    max_surface_water_rate (float): max surface (QWSMAX)
-    max_surface_liquid_rate (float): max surface liquid rate (QLIQSMAX)
-    max_hc_molar_rate (float): Max hc molar rate (QMHCMAX)
-    max_reverse_surface_oil_rate (float): max reverse surface oil rate (QOSMAX-)
-    max_reverse_surface_gas_rate (float): max reverse surface gas rate (QGSMAX-)
-    max_reverse_surface_water_rate (float): max reverse surface water rate (QWSMAX-)
-    max_reverse_surface_liquid_rate (float): max reverse surface liquid rate (QLIQSMAX-)
-    max_reservoir_oil_rate (float): max reservoir oil rate (QOMAX)
-    max_reservoir_gas_rate (float): max reservoir gas rate (QGMAX)
-    max_reservoir_water_rate (float): max reservoir water rate (QWMAX)
-    max_reservoir_liquid_rate (float): max reservoir liquid rate (QLIQMAX)
-    max_reservoir_total_fluids_rate (float): max reservoir total fluids rate (QALLMAX)
-    max_reservoir_hc_rate (float): max reservoir hc rate (QHCMAX)
-    max_reverse_reservoir_oil_rate (float): max reverse reservoir oil rate (QOMAX-)
-    max_reverse_reservoir_gas_rate (float): max reverse reservoir gas rate (QGMAX-)
-    max_reverse_reservoir_water_rate (float): max reverse reservoir water rate (QWMAX-)
-    max_reverse_reservoir_liquid_rate (float): max reverse reservoir liquid rate (QLIQMAX-)
-    max_reverse_reservoir_total_fluids_rate (float): max reverse reservoir total fluids rate (QALLMAX-)
-    max_reverse_reservoir_hc_rate (float): max reverse reservoir hc rate (QHCMAX-)
-    min_pressure (float): min pressure (PMIN)
-    max_pressure (float): max pressure (PMAX)
-    max_wag_water_pressure (float): max wag water pressure (PWMAX)
-    max_wag_gas_pressure (float): max wag gas pressure (PGMAX)
-    bottom_hole_pressure (float): bottom hole pressure (BHP)
-    tubing_head_pressure (float): tubing head pressure (THP)
-    min_surface_oil_rate (float): min surface oil rate (QOSMIN)
-    min_surface_gas_rate (float): min surface gas rate (QGSMIN)
-    min_surface_water_rate (float): min surface water rate (QWSMIN)
-    min_surface_liquid_rate (float): min surface liquid rate (QLIQSMIN)
-    min_reservoir_oil_rate (float): min reservoir oil rate (QOMIN)
-    min_reservoir_gas_rate (float): min reservoir gas rate (QGMIN)
-    min_reservoir_water_rate (float): min reservoir water rate (QWMIN)
-    min_reservoir_liquid_rate (float): min reservoir liquid rate (QLIQMIN)
-    min_reservoir_total_fluids_rate (float): min reservoir total fluids rate (QALLMIN)
-    min_reservoir_hc_rate (float): min reservoir hc rate (QHCMIN)
-    min_reverse_surface_oil_rate (float): min reservoir oil rate (QOSMIN-)
-    min_reverse_surface_gas_rate (float): min reservoir gas rate (QGSMIN-)
-    min_reverse_surface_water_rate (float): min reservoir water rate (QWSMIN-)
-    min_reverse_surface_liquid_rate (float): min reservoir liquid rate (QLIQSMIN-)
-    min_reverse_reservoir_oil_rate (float): min reverse reservoir oil rate (QOMIN-)
-    min_reverse_reservoir_gas_rate (float): min reverse reservoir gas rate (QGMIN-)
-    min_reverse_reservoir_water_rate (float): min reverse reservoir water rate (QWMIN-)
-    min_reverse_reservoir_liquid_rate (float): min reverse reservoir liquid rate (QLIQMIN-)
-    min_reverse_reservoir_total_fluids_rate (float): min reverse reservoir total fluids rate (QALLMIN-)
-    min_reverse_reservoir_hc_rate (float): min reverse reservoir hc rate (QHCMIN-)
-    max_watercut (float): max watercut (WCUTMAX)
-    max_watercut_plug (float): max watercut plug (WCUTPLUG)
-    max_watercut_plugplus (float): max watercut plugplus (WCUTPLUGPLUS)
-    max_watercut_perf (float): max watercut perf (WCUTPERF)
-    max_watercut_perfplus (float): max watercut perfplus (WCUTPERFPLUS)
-    max_wor (float): max wor (WORMAX)
-    max_wor_plug (float): max wor plug (WORPLUG)
-    max_wor_plug_plus (float): max wor plug plus (WORPLUGPLUS)
-    max_wor_perf (float): max wor perf (WORPERF)
-    max_wor_perfplus (float): max wor perfplus (WORPERFPLUS)
-    max_gor (float): max gor (GORMAX)
-    max_gor_plug (float): max gor plug (GORPLUG)
-    max_gor_plug_plus (float): max gor plug plus (GORPLUGPLUS)
-    max_gor_perf (float): max gor perf (GORPERF)
-    max_gor_perfplus (float): max gor perfplus (GORPERFPLUS)
-    max_lgr (float): max lgr (LGRMAX)
-    max_lgr_plug (float): max lgr plug (LGRPLUG)
-    max_lgr_plug_plus (float): max lgr plug plus (LGRPLUGPLUS)
-    max_lgr_perf (float): max lgr perf (LGRPERF)
-    max_lgr_perfplus (float): max lgr perfplus (LGRPERFPLUS)
-    max_cum_gas_prod (float): max cum gas prod (CGLIM)
-    max_cum_water_prod (float): max cum water prod (CWLIM)
-    max_cum_oil_prod (float): max cum oil prod (COLIM).
-
-    artificial_lift_number (int): artificial lift number within the hydraulic table (ALQ)
-    max_choke_setting (float): maximum choke/ICD/valve setting (SETTING)
-    min_gas_lift_efficiency (float): minimum gas lift efficiency below which the connection will be shut in(GLEFMIN)
-    gl_additive_correction (float): additive correction term to value of gas/liquid ratio from optimal gl \
-            tables (GLRADD)
-    active_node (bool): active/inactive node/well (ACTIVATE)
-    pump_power (float): power for the pump (POWER)
-    pump_speed (float): maximum speed of the pump/esp/compressor (SPEED)
-    choke_limit (str): ON/OFF for whether the esp should exceed the choke limit (CHOKELIMIT)
-    manifold_position (int): position in the manifold for the well (POSITION)
-
-    """
-
-    name: Optional[str] = None
-    well_name: Optional[str] = None
-    max_surface_oil_rate: Optional[float] = None
-    max_surface_gas_rate: Optional[float] = None
-    max_surface_water_rate: Optional[float] = None
-    max_surface_liquid_rate: Optional[float] = None
-    max_hc_molar_rate: Optional[float] = None
-    max_reverse_surface_oil_rate: Optional[float] = None
-    max_reverse_surface_gas_rate: Optional[float] = None
-    max_reverse_surface_water_rate: Optional[float] = None
-    max_reverse_surface_liquid_rate: Optional[float] = None
-    max_reservoir_oil_rate: Optional[float] = None
-    max_reservoir_gas_rate: Optional[float] = None
-    max_reservoir_water_rate: Optional[float] = None
-    max_reservoir_liquid_rate: Optional[float] = None
-    max_reservoir_total_fluids_rate: Optional[float] = None
-    max_reservoir_hc_rate: Optional[float] = None
-    max_reverse_reservoir_oil_rate: Optional[float] = None
-    max_reverse_reservoir_gas_rate: Optional[float] = None
-    max_reverse_reservoir_water_rate: Optional[float] = None
-    max_reverse_reservoir_liquid_rate: Optional[float] = None
-    max_reverse_reservoir_total_fluids_rate: Optional[float] = None
-    max_reverse_reservoir_hc_rate: Optional[float] = None
-    max_avg_comp_dp: Optional[float] = None
-    max_comp_dp: Optional[float] = None
-
-    min_pressure: Optional[float] = None
-    max_pressure: Optional[float] = None
-    max_wag_water_pressure: Optional[float] = None
-    max_wag_gas_pressure: Optional[float] = None
-    bottom_hole_pressure: Optional[float] = None
-    tubing_head_pressure: Optional[float] = None
-    min_reverse_surface_oil_rate: Optional[float] = None
-    min_reverse_surface_gas_rate: Optional[float] = None
-    min_reverse_surface_water_rate: Optional[float] = None
-    min_reverse_surface_liquid_rate: Optional[float] = None
-    min_surface_oil_rate: Optional[float] = None
-    min_surface_gas_rate: Optional[float] = None
-    min_surface_water_rate: Optional[float] = None
-    min_surface_liquid_rate: Optional[float] = None
-    min_reservoir_oil_rate: Optional[float] = None
-    min_reservoir_gas_rate: Optional[float] = None
-    min_reservoir_water_rate: Optional[float] = None
-    min_reservoir_liquid_rate: Optional[float] = None
-    min_reservoir_total_fluids_rate: Optional[float] = None
-    min_reservoir_hc_rate: Optional[float] = None
-    min_reverse_reservoir_oil_rate: Optional[float] = None
-    min_reverse_reservoir_gas_rate: Optional[float] = None
-    min_reverse_reservoir_water_rate: Optional[float] = None
-    min_reverse_reservoir_liquid_rate: Optional[float] = None
-    min_reverse_reservoir_total_fluids_rate: Optional[float] = None
-    min_reverse_reservoir_hc_rate: Optional[float] = None
-    max_watercut: Optional[float] = None
-    max_watercut_plug: Optional[float] = None
-    max_watercut_plugplus: Optional[float] = None
-    max_watercut_perf: Optional[float] = None
-    max_watercut_perfplus: Optional[float] = None
-    max_wor: Optional[float] = None
-    max_wor_plug: Optional[float] = None
-    max_wor_plug_plus: Optional[float] = None
-    max_wor_perf: Optional[float] = None
-    max_wor_perfplus: Optional[float] = None
-    max_gor: Optional[float] = None
-    max_gor_plug: Optional[float] = None
-    max_gor_plug_plus: Optional[float] = None
-    max_gor_perf: Optional[float] = None
-    max_gor_perfplus: Optional[float] = None
-    gor_limit: Optional[float] = None
-    gor_limit_exponent: Optional[float] = None
-    gor_limit_frequency: Optional[float] = None
-    max_lgr: Optional[float] = None
-    max_lgr_plug: Optional[float] = None
-    max_lgr_plug_plus: Optional[float] = None
-    max_lgr_perf: Optional[float] = None
-    max_lgr_perfplus: Optional[float] = None
-    max_cum_gas_prod: Optional[float] = None
-    max_cum_water_prod: Optional[float] = None
-    max_cum_oil_prod: Optional[float] = None
-
-    max_qmult_total_reservoir_rate: Optional[float] = None
-    convert_qmult_to_reservoir_barrels: Optional[bool] = None
-    qmult_oil_rate: Optional[float] = None
-    qmult_water_rate: Optional[float] = None
-    qmult_gas_rate: Optional[float] = None
-    use_qmult_qoil_surface_rate: Optional[bool] = None
-    use_qmult_qwater_surface_rate: Optional[bool] = None
-    use_qmult_qgas_surface_rate: Optional[bool] = None
-    use_qmult_qoilqwat_surface_rate: Optional[bool] = None
-
-    artificial_lift_number: Optional[int] = None
-    max_choke_setting: Optional[float] = None
-    min_gas_lift_efficiency: Optional[float] = None
-    gl_additive_correction: Optional[float] = None
-    active_node: Optional[bool] = None
-    pump_power: Optional[float] = None
-    pump_speed: Optional[float] = None
-    choke_limit: Optional[str] = None
-    manifold_position: Optional[int] = None
-
-    clear_all: Optional[bool] = None
-    clear_q: Optional[bool] = None
-    clear_limit: Optional[bool] = None
-    clear_alq: Optional[bool] = None
-    clear_p: Optional[bool] = None
-
-    def __init__(self, properties_dict: dict[str, None | int | str | float | UnitSystem]) -> None:
-        super().__init__()
-        for key, prop in properties_dict.items():
-            self.__setattr__(key, prop)
-
-    @staticmethod
-    def get_nexus_mapping() -> dict[str, tuple[str, type]]:
-        """Gets the mapping of nexus keywords to attribute definitions."""
-        nexus_mapping: dict[str, tuple[str, type]] = {
-            'WELL': ('well_name', str),
-            'NAME': ('name', str),
-            # Specialkeywords - QMULT
-            'QALLRMAX_MULT': ('convert_qmult_to_reservoir_barrels', bool),
-            'QOSMAX_MULT': ('use_qmult_qoil_surface_rate', bool),
-            'QWSMAX_MULT': ('use_qmult_qwater_surface_rate', bool),
-            'QGSMAX_MULT': ('use_qmult_qgas_surface_rate', bool),
-            'QLIQSMAX_MULT': ('use_qmult_qoilqwat_surface_rate', bool),
-            # SpecialClearkeywords
-            'CLEAR': ('clear_all', bool),
-            'CLEARQ': ('clear_q', bool),
-            'CLEARP': ('clear_p', bool),
-            'CLEARLIMIT': ('clear_limit', bool),
-            'CLEARALQ': ('clear_alq', bool),
-            }
-        nexus_mapping.update(NexusConstraint.get_limit_constraints_map())
-        nexus_mapping.update(NexusConstraint.get_pressure_constraints_map())
-        nexus_mapping.update(NexusConstraint.get_rate_constraints_map())
-        nexus_mapping.update(NexusConstraint.get_alq_constraints_map())
-        return nexus_mapping
-
-    @staticmethod
-    def get_rate_constraints_map() -> dict[str, tuple[str, type]]:
-
-        nexus_mapping: dict[str, tuple[str, type]] = {
-            'QALLRMAX': ('max_qmult_total_reservoir_rate', float),
-
-            'QOSMAX': ('max_surface_oil_rate', float),
-            'QGSMAX': ('max_surface_gas_rate', float),
-            'QWSMAX': ('max_surface_water_rate', float),
-            'QLIQSMAX': ('max_surface_liquid_rate', float),
-            'QMHCMAX': ('max_hc_molar_rate', float),
-            'QOSMAX-': ('max_reverse_surface_oil_rate', float),
-            'QGSMAX-': ('max_reverse_surface_gas_rate', float),
-            'QWSMAX-': ('max_reverse_surface_water_rate', float),
-            'QLIQSMAX-': ('max_reverse_surface_liquid_rate', float),
-            'QOMAX': ('max_reservoir_oil_rate', float),
-            'QGMAX': ('max_reservoir_gas_rate', float),
-            'QWMAX': ('max_reservoir_water_rate', float),
-            'QLIQMAX': ('max_reservoir_liquid_rate', float),
-            'QALLMAX': ('max_reservoir_total_fluids_rate', float),
-            'QHCMAX': ('max_reservoir_hc_rate', float),
-            'QOMAX-': ('max_reverse_reservoir_oil_rate', float),
-            'QGMAX-': ('max_reverse_reservoir_gas_rate', float),
-            'QWMAX-': ('max_reverse_reservoir_water_rate', float),
-            'QLIQMAX-': ('max_reverse_reservoir_liquid_rate', float),
-            'QALLMAX-': ('max_reverse_reservoir_total_fluids_rate', float),
-            'QHCMAX-': ('max_reverse_reservoir_hc_rate', float),
-            'QOSMIN': ('min_surface_oil_rate', float),
-            'QGSMIN': ('min_surface_gas_rate', float),
-            'QWSMIN': ('min_surface_water_rate', float),
-            'QLIQSMIN': ('min_surface_liquid_rate', float),
-            'QOMIN': ('min_reservoir_oil_rate', float),
-            'QGMIN': ('min_reservoir_gas_rate', float),
-            'QWMIN': ('min_reservoir_water_rate', float),
-            'QLIQMIN': ('min_reservoir_liquid_rate', float),
-            'QALLMIN': ('min_reservoir_total_fluids_rate', float),
-            'QHCMIN': ('min_reservoir_hc_rate', float),
-            'QOSMIN-': ('min_reverse_surface_oil_rate', float),
-            'QGSMIN-': ('min_reverse_surface_gas_rate', float),
-            'QWSMIN-': ('min_reverse_surface_water_rate', float),
-            'QLIQSMIN-': ('min_reverse_surface_liquid_rate', float),
-            'QOMIN-': ('min_reverse_reservoir_oil_rate', float),
-            'QGMIN-': ('min_reverse_reservoir_gas_rate', float),
-            'QWMIN-': ('min_reverse_reservoir_water_rate', float),
-            'QLIQMIN-': ('min_reverse_reservoir_liquid_rate', float),
-            'QALLMIN-': ('min_reverse_reservoir_total_fluids_rate', float),
-            'QHCMIN-': ('min_reverse_reservoir_hc_rate', float),
-
-            'QOIL': ('qmult_oil_rate', float),
-            'QWATER': ('qmult_water_rate', float),
-            'QGAS': ('qmult_gas_rate', float),
-            'DPBHAVG': ('max_avg_comp_dp', float),
-            'DPBHMX': ('max_comp_dp', float),
-            }
-        return nexus_mapping
-
-    @staticmethod
-    def get_pressure_constraints_map() -> dict[str, tuple[str, type]]:
-        nexus_mapping: dict[str, tuple[str, type]] = {
-            'PMIN': ('min_pressure', float),
-            'PMAX': ('max_pressure', float),
-            'PWMAX': ('max_wag_water_pressure', float),
-            'PGMAX': ('max_wag_gas_pressure', float),
-            'BHP': ('bottom_hole_pressure', float),
-            'THP': ('tubing_head_pressure', float),
-            }
-        return nexus_mapping
-
-    @staticmethod
-    def get_limit_constraints_map() -> dict[str, tuple[str, type]]:
-        nexus_mapping: dict[str, tuple[str, type]] = {
-            'WCUTMAX': ('max_watercut', float),
-            'WCUTPLUG': ('max_watercut_plug', float),
-            'WCUTPLUGPLUS': ('max_watercut_plugplus', float),
-            'WCUTPERF': ('max_watercut_perf', float),
-            'WCUTPERFPLUS': ('max_watercut_perfplus', float),
-            'WORMAX': ('max_wor', float),
-            'WORPLUG': ('max_wor_plug', float),
-            'WORPLUGPLUS': ('max_wor_plug_plus', float),
-            'WORPERF': ('max_wor_perf', float),
-            'WORPERFPLUS': ('max_wor_perfplus', float),
-            'GORLIM': ('gor_limit', float),
-            'EXPONENT': ('gor_limit_exponent', float),
-            'FREQUENCY': ('gor_limit_frequency', float),
-            'GORMAX': ('max_gor', float),
-            'GORPLUG': ('max_gor_plug', float),
-            'GORPLUGPLUS': ('max_gor_plug_plus', float),
-            'GORPERF': ('max_gor_perf', float),
-            'GORPERFPLUS': ('max_gor_perfplus', float),
-            'LGRMAX': ('max_lgr', float),
-            'LGRPLUG': ('max_lgr_plug', float),
-            'LGRPLUGPLUS': ('max_lgr_plug_plus', float),
-            'LGRPERF': ('max_lgr_perf', float),
-            'LGRPERFPLUS': ('max_lgr_perfplus', float),
-            'CGLIM': ('max_cum_gas_prod', float),
-            'CWLIM': ('max_cum_water_prod', float),
-            'COLIM': ('max_cum_oil_prod', float),
-            }
-        return nexus_mapping
-
-    @staticmethod
-    def get_alq_constraints_map() -> dict[str, tuple[str, type]]:
-        """Gets the nexus mapping for artificial lift constraints."""
-        nexus_mapping: dict[str, tuple[str, type]] = {
-            'ALQ': ('artificial_lift_number', int),
-            'SETTING': ('max_choke_setting', float),
-            'GLEFMIN': ('min_gas_lift_efficiency', float),
-            'GLRADD': ('gl_additive_correction', float),
-            'ACTIVATE': ('active_node', bool),
-            'POWER': ('pump_power', float),
-            'SPEED': ('pump_speed', float),
-            'CHOKELIMIT': ('choke_limit', str),
-            'POSITION': ('manifold_position', int),
-            }
-        return nexus_mapping
-
-    def to_dict(self, keys_in_nexus_style: bool = False) -> dict[str, None | str | int | float]:
-        """Returns a dictionary of the attributes of the Constraint.
-
-        Args:
-            keys_in_nexus_style (bool): if True returns the key values in Nexus keywords, otherwise returns the \
-                attribute name as stored by ressimpy.
-
-        Returns:
-            a dictionary keyed by attributes and values as the value of the attribute
-        """
-        result_dict = to_dict_generic.to_dict(self, keys_in_nexus_style, add_date=True, add_units=True)
-        return result_dict
-
-    def update(self, new_data: dict[str, None | int | str | float | UnitSystem], nones_overwrite: bool = False):
-        """Updates attributes in the object based on the dictionary provided."""
-        for k, v in new_data.items():
-            if v is not None or nones_overwrite:
-                setattr(self, k, v)
-
-    def to_table_line(self) -> str:
-        """String representation of the constraint for entry to an inline constraint table."""
-        qmult_control_key_words = ['QALLRMAX_MULT', 'QOSMAX_MULT', 'QWSMAX_MULT', 'QGSMAX_MULT', 'QLIQSMAX_MULT']
-        skip_attributes = ['date', 'unit_system', 'NAME', 'ACTIVATE', 'QOIL', 'QWATER', 'QGAS', 'WELL']
-        clear_attributes = ['CLEAR', 'CLEARQ', 'CLEARP', 'CLEARLIMIT', 'CLEARALQ']
-
-        if self.name is not None:
-            constraint_string = self.name
-        elif self.well_name is not None:
-            constraint_string = self.well_name
-        else:
-            raise ValueError('Must have a well or node name for returning a constraint to a string')
-
-        for attribute, value in self.to_dict(keys_in_nexus_style=True).items():
-            if value and attribute in qmult_control_key_words:
-                constraint_string += (' ' + attribute.replace('_MULT', '') + ' MULT')
-            elif value is None or attribute in skip_attributes:
-                continue
-            elif value and attribute in clear_attributes:
-                constraint_string += ' ' + attribute
-            else:
-                constraint_string += (' ' + attribute + ' ' + str(value))
-
-        if self.active_node:
-            constraint_string += ' ACTIVATE'
-        elif self.active_node is not None:
-            # equivalent to active node being False
-            constraint_string += ' DEACTIVATE'
-
-        constraint_string += '\n'
-        return constraint_string
-
-    def write_qmult_table(self) -> list[str]:
-        """Writes out a QMULT table from a constraint that uses the following attributes.
-        'QOIL': ('qmult_oil_rate', float).
-        'QWATER': ('qmult_water_rate', float).
-        'QGAS': ('qmult_gas_rate', float).
-
-        Returns:
-            list[str] with a representation of the QMULT table with a new line as a new entry in the list.
-        """
-        table_to_return = ['QMULT\n', 'WELL QOIL QGAS QWATER\n']
-        qmult_values = self.write_qmult_values()
-        table_to_return.append(qmult_values)
-        table_to_return.append('ENDQMULT\n')
-
-        return table_to_return
-
-    def write_qmult_values(self) -> str:
-        """Writes out the values for a QMULT table, callable on its own or using the write_qmult_table method."""
-        qmult_values_keywords = ['qmult_oil_rate', 'qmult_gas_rate', 'qmult_water_rate']
-        if self.name is not None:
-            string_to_return = self.name
-        elif self.well_name is not None:
-            string_to_return = self.well_name
-        else:
-            raise ValueError('Must have a well or node name for returning a qmult table')
-
-        for keyword in qmult_values_keywords:
-            value = getattr(self, keyword, None)
-            if value is None:
-                string_to_return += ' NA'
-            else:
-                string_to_return += f' {str(value)}'
-        string_to_return += '\n'
-        return string_to_return
+from dataclasses import dataclass
+from typing import Optional
+
+from ResSimpy.Constraint import Constraint
+from ResSimpy.Enums.UnitsEnum import UnitSystem
+from ResSimpy.Utils import to_dict_generic
+
+
+@dataclass
+class NexusConstraint(Constraint):
+    """Attributes:
+    name (str): name of the well (NAME)
+    max_surface_oil_rate (float): max surface oil rate (QOSMAX)
+    max_surface_gas_rate (float): max surface gas rate (QGSMAX)
+    max_surface_water_rate (float): max surface (QWSMAX)
+    max_surface_liquid_rate (float): max surface liquid rate (QLIQSMAX)
+    max_hc_molar_rate (float): Max hc molar rate (QMHCMAX)
+    max_reverse_surface_oil_rate (float): max reverse surface oil rate (QOSMAX-)
+    max_reverse_surface_gas_rate (float): max reverse surface gas rate (QGSMAX-)
+    max_reverse_surface_water_rate (float): max reverse surface water rate (QWSMAX-)
+    max_reverse_surface_liquid_rate (float): max reverse surface liquid rate (QLIQSMAX-)
+    max_reservoir_oil_rate (float): max reservoir oil rate (QOMAX)
+    max_reservoir_gas_rate (float): max reservoir gas rate (QGMAX)
+    max_reservoir_water_rate (float): max reservoir water rate (QWMAX)
+    max_reservoir_liquid_rate (float): max reservoir liquid rate (QLIQMAX)
+    max_reservoir_total_fluids_rate (float): max reservoir total fluids rate (QALLMAX)
+    max_reservoir_hc_rate (float): max reservoir hc rate (QHCMAX)
+    max_reverse_reservoir_oil_rate (float): max reverse reservoir oil rate (QOMAX-)
+    max_reverse_reservoir_gas_rate (float): max reverse reservoir gas rate (QGMAX-)
+    max_reverse_reservoir_water_rate (float): max reverse reservoir water rate (QWMAX-)
+    max_reverse_reservoir_liquid_rate (float): max reverse reservoir liquid rate (QLIQMAX-)
+    max_reverse_reservoir_total_fluids_rate (float): max reverse reservoir total fluids rate (QALLMAX-)
+    max_reverse_reservoir_hc_rate (float): max reverse reservoir hc rate (QHCMAX-)
+    min_pressure (float): min pressure (PMIN)
+    max_pressure (float): max pressure (PMAX)
+    max_wag_water_pressure (float): max wag water pressure (PWMAX)
+    max_wag_gas_pressure (float): max wag gas pressure (PGMAX)
+    bottom_hole_pressure (float): bottom hole pressure (BHP)
+    tubing_head_pressure (float): tubing head pressure (THP)
+    min_surface_oil_rate (float): min surface oil rate (QOSMIN)
+    min_surface_gas_rate (float): min surface gas rate (QGSMIN)
+    min_surface_water_rate (float): min surface water rate (QWSMIN)
+    min_surface_liquid_rate (float): min surface liquid rate (QLIQSMIN)
+    min_reservoir_oil_rate (float): min reservoir oil rate (QOMIN)
+    min_reservoir_gas_rate (float): min reservoir gas rate (QGMIN)
+    min_reservoir_water_rate (float): min reservoir water rate (QWMIN)
+    min_reservoir_liquid_rate (float): min reservoir liquid rate (QLIQMIN)
+    min_reservoir_total_fluids_rate (float): min reservoir total fluids rate (QALLMIN)
+    min_reservoir_hc_rate (float): min reservoir hc rate (QHCMIN)
+    min_reverse_surface_oil_rate (float): min reservoir oil rate (QOSMIN-)
+    min_reverse_surface_gas_rate (float): min reservoir gas rate (QGSMIN-)
+    min_reverse_surface_water_rate (float): min reservoir water rate (QWSMIN-)
+    min_reverse_surface_liquid_rate (float): min reservoir liquid rate (QLIQSMIN-)
+    min_reverse_reservoir_oil_rate (float): min reverse reservoir oil rate (QOMIN-)
+    min_reverse_reservoir_gas_rate (float): min reverse reservoir gas rate (QGMIN-)
+    min_reverse_reservoir_water_rate (float): min reverse reservoir water rate (QWMIN-)
+    min_reverse_reservoir_liquid_rate (float): min reverse reservoir liquid rate (QLIQMIN-)
+    min_reverse_reservoir_total_fluids_rate (float): min reverse reservoir total fluids rate (QALLMIN-)
+    min_reverse_reservoir_hc_rate (float): min reverse reservoir hc rate (QHCMIN-)
+    max_watercut (float): max watercut (WCUTMAX)
+    max_watercut_plug (float): max watercut plug (WCUTPLUG)
+    max_watercut_plugplus (float): max watercut plugplus (WCUTPLUGPLUS)
+    max_watercut_perf (float): max watercut perf (WCUTPERF)
+    max_watercut_perfplus (float): max watercut perfplus (WCUTPERFPLUS)
+    max_wor (float): max wor (WORMAX)
+    max_wor_plug (float): max wor plug (WORPLUG)
+    max_wor_plug_plus (float): max wor plug plus (WORPLUGPLUS)
+    max_wor_perf (float): max wor perf (WORPERF)
+    max_wor_perfplus (float): max wor perfplus (WORPERFPLUS)
+    max_gor (float): max gor (GORMAX)
+    max_gor_plug (float): max gor plug (GORPLUG)
+    max_gor_plug_plus (float): max gor plug plus (GORPLUGPLUS)
+    max_gor_perf (float): max gor perf (GORPERF)
+    max_gor_perfplus (float): max gor perfplus (GORPERFPLUS)
+    max_lgr (float): max lgr (LGRMAX)
+    max_lgr_plug (float): max lgr plug (LGRPLUG)
+    max_lgr_plug_plus (float): max lgr plug plus (LGRPLUGPLUS)
+    max_lgr_perf (float): max lgr perf (LGRPERF)
+    max_lgr_perfplus (float): max lgr perfplus (LGRPERFPLUS)
+    max_cum_gas_prod (float): max cum gas prod (CGLIM)
+    max_cum_water_prod (float): max cum water prod (CWLIM)
+    max_cum_oil_prod (float): max cum oil prod (COLIM).
+
+    artificial_lift_number (int): artificial lift number within the hydraulic table (ALQ)
+    max_choke_setting (float): maximum choke/ICD/valve setting (SETTING)
+    min_gas_lift_efficiency (float): minimum gas lift efficiency below which the connection will be shut in(GLEFMIN)
+    gl_additive_correction (float): additive correction term to value of gas/liquid ratio from optimal gl \
+            tables (GLRADD)
+    active_node (bool): active/inactive node/well (ACTIVATE)
+    pump_power (float): power for the pump (POWER)
+    pump_speed (float): maximum speed of the pump/esp/compressor (SPEED)
+    choke_limit (str): ON/OFF for whether the esp should exceed the choke limit (CHOKELIMIT)
+    manifold_position (int): position in the manifold for the well (POSITION)
+
+    """
+
+    name: Optional[str] = None
+    well_name: Optional[str] = None
+    max_surface_oil_rate: Optional[float] = None
+    max_surface_gas_rate: Optional[float] = None
+    max_surface_water_rate: Optional[float] = None
+    max_surface_liquid_rate: Optional[float] = None
+    max_hc_molar_rate: Optional[float] = None
+    max_reverse_surface_oil_rate: Optional[float] = None
+    max_reverse_surface_gas_rate: Optional[float] = None
+    max_reverse_surface_water_rate: Optional[float] = None
+    max_reverse_surface_liquid_rate: Optional[float] = None
+    max_reservoir_oil_rate: Optional[float] = None
+    max_reservoir_gas_rate: Optional[float] = None
+    max_reservoir_water_rate: Optional[float] = None
+    max_reservoir_liquid_rate: Optional[float] = None
+    max_reservoir_total_fluids_rate: Optional[float] = None
+    max_reservoir_hc_rate: Optional[float] = None
+    max_reverse_reservoir_oil_rate: Optional[float] = None
+    max_reverse_reservoir_gas_rate: Optional[float] = None
+    max_reverse_reservoir_water_rate: Optional[float] = None
+    max_reverse_reservoir_liquid_rate: Optional[float] = None
+    max_reverse_reservoir_total_fluids_rate: Optional[float] = None
+    max_reverse_reservoir_hc_rate: Optional[float] = None
+    max_avg_comp_dp: Optional[float] = None
+    max_comp_dp: Optional[float] = None
+
+    min_pressure: Optional[float] = None
+    max_pressure: Optional[float] = None
+    max_wag_water_pressure: Optional[float] = None
+    max_wag_gas_pressure: Optional[float] = None
+    bottom_hole_pressure: Optional[float] = None
+    tubing_head_pressure: Optional[float] = None
+    min_reverse_surface_oil_rate: Optional[float] = None
+    min_reverse_surface_gas_rate: Optional[float] = None
+    min_reverse_surface_water_rate: Optional[float] = None
+    min_reverse_surface_liquid_rate: Optional[float] = None
+    min_surface_oil_rate: Optional[float] = None
+    min_surface_gas_rate: Optional[float] = None
+    min_surface_water_rate: Optional[float] = None
+    min_surface_liquid_rate: Optional[float] = None
+    min_reservoir_oil_rate: Optional[float] = None
+    min_reservoir_gas_rate: Optional[float] = None
+    min_reservoir_water_rate: Optional[float] = None
+    min_reservoir_liquid_rate: Optional[float] = None
+    min_reservoir_total_fluids_rate: Optional[float] = None
+    min_reservoir_hc_rate: Optional[float] = None
+    min_reverse_reservoir_oil_rate: Optional[float] = None
+    min_reverse_reservoir_gas_rate: Optional[float] = None
+    min_reverse_reservoir_water_rate: Optional[float] = None
+    min_reverse_reservoir_liquid_rate: Optional[float] = None
+    min_reverse_reservoir_total_fluids_rate: Optional[float] = None
+    min_reverse_reservoir_hc_rate: Optional[float] = None
+    max_watercut: Optional[float] = None
+    max_watercut_plug: Optional[float] = None
+    max_watercut_plugplus: Optional[float] = None
+    max_watercut_perf: Optional[float] = None
+    max_watercut_perfplus: Optional[float] = None
+    max_wor: Optional[float] = None
+    max_wor_plug: Optional[float] = None
+    max_wor_plug_plus: Optional[float] = None
+    max_wor_perf: Optional[float] = None
+    max_wor_perfplus: Optional[float] = None
+    max_gor: Optional[float] = None
+    max_gor_plug: Optional[float] = None
+    max_gor_plug_plus: Optional[float] = None
+    max_gor_perf: Optional[float] = None
+    max_gor_perfplus: Optional[float] = None
+    gor_limit: Optional[float] = None
+    gor_limit_exponent: Optional[float] = None
+    gor_limit_frequency: Optional[float] = None
+    max_lgr: Optional[float] = None
+    max_lgr_plug: Optional[float] = None
+    max_lgr_plug_plus: Optional[float] = None
+    max_lgr_perf: Optional[float] = None
+    max_lgr_perfplus: Optional[float] = None
+    max_cum_gas_prod: Optional[float] = None
+    max_cum_water_prod: Optional[float] = None
+    max_cum_oil_prod: Optional[float] = None
+
+    max_qmult_total_reservoir_rate: Optional[float] = None
+    convert_qmult_to_reservoir_barrels: Optional[bool] = None
+    qmult_oil_rate: Optional[float] = None
+    qmult_water_rate: Optional[float] = None
+    qmult_gas_rate: Optional[float] = None
+    use_qmult_qoil_surface_rate: Optional[bool] = None
+    use_qmult_qwater_surface_rate: Optional[bool] = None
+    use_qmult_qgas_surface_rate: Optional[bool] = None
+    use_qmult_qoilqwat_surface_rate: Optional[bool] = None
+
+    artificial_lift_number: Optional[int] = None
+    max_choke_setting: Optional[float] = None
+    min_gas_lift_efficiency: Optional[float] = None
+    gl_additive_correction: Optional[float] = None
+    active_node: Optional[bool] = None
+    pump_power: Optional[float] = None
+    pump_speed: Optional[float] = None
+    choke_limit: Optional[str] = None
+    manifold_position: Optional[int] = None
+
+    clear_all: Optional[bool] = None
+    clear_q: Optional[bool] = None
+    clear_limit: Optional[bool] = None
+    clear_alq: Optional[bool] = None
+    clear_p: Optional[bool] = None
+
+    def __init__(self, properties_dict: dict[str, None | int | str | float | UnitSystem]) -> None:
+        super().__init__()
+        for key, prop in properties_dict.items():
+            self.__setattr__(key, prop)
+
+    @staticmethod
+    def get_nexus_mapping() -> dict[str, tuple[str, type]]:
+        """Gets the mapping of nexus keywords to attribute definitions."""
+        nexus_mapping: dict[str, tuple[str, type]] = {
+            'WELL': ('well_name', str),
+            'NAME': ('name', str),
+            # Specialkeywords - QMULT
+            'QALLRMAX_MULT': ('convert_qmult_to_reservoir_barrels', bool),
+            'QOSMAX_MULT': ('use_qmult_qoil_surface_rate', bool),
+            'QWSMAX_MULT': ('use_qmult_qwater_surface_rate', bool),
+            'QGSMAX_MULT': ('use_qmult_qgas_surface_rate', bool),
+            'QLIQSMAX_MULT': ('use_qmult_qoilqwat_surface_rate', bool),
+            # SpecialClearkeywords
+            'CLEAR': ('clear_all', bool),
+            'CLEARQ': ('clear_q', bool),
+            'CLEARP': ('clear_p', bool),
+            'CLEARLIMIT': ('clear_limit', bool),
+            'CLEARALQ': ('clear_alq', bool),
+            }
+        nexus_mapping.update(NexusConstraint.get_limit_constraints_map())
+        nexus_mapping.update(NexusConstraint.get_pressure_constraints_map())
+        nexus_mapping.update(NexusConstraint.get_rate_constraints_map())
+        nexus_mapping.update(NexusConstraint.get_alq_constraints_map())
+        return nexus_mapping
+
+    @staticmethod
+    def get_rate_constraints_map() -> dict[str, tuple[str, type]]:
+
+        nexus_mapping: dict[str, tuple[str, type]] = {
+            'QALLRMAX': ('max_qmult_total_reservoir_rate', float),
+
+            'QOSMAX': ('max_surface_oil_rate', float),
+            'QGSMAX': ('max_surface_gas_rate', float),
+            'QWSMAX': ('max_surface_water_rate', float),
+            'QLIQSMAX': ('max_surface_liquid_rate', float),
+            'QMHCMAX': ('max_hc_molar_rate', float),
+            'QOSMAX-': ('max_reverse_surface_oil_rate', float),
+            'QGSMAX-': ('max_reverse_surface_gas_rate', float),
+            'QWSMAX-': ('max_reverse_surface_water_rate', float),
+            'QLIQSMAX-': ('max_reverse_surface_liquid_rate', float),
+            'QOMAX': ('max_reservoir_oil_rate', float),
+            'QGMAX': ('max_reservoir_gas_rate', float),
+            'QWMAX': ('max_reservoir_water_rate', float),
+            'QLIQMAX': ('max_reservoir_liquid_rate', float),
+            'QALLMAX': ('max_reservoir_total_fluids_rate', float),
+            'QHCMAX': ('max_reservoir_hc_rate', float),
+            'QOMAX-': ('max_reverse_reservoir_oil_rate', float),
+            'QGMAX-': ('max_reverse_reservoir_gas_rate', float),
+            'QWMAX-': ('max_reverse_reservoir_water_rate', float),
+            'QLIQMAX-': ('max_reverse_reservoir_liquid_rate', float),
+            'QALLMAX-': ('max_reverse_reservoir_total_fluids_rate', float),
+            'QHCMAX-': ('max_reverse_reservoir_hc_rate', float),
+            'QOSMIN': ('min_surface_oil_rate', float),
+            'QGSMIN': ('min_surface_gas_rate', float),
+            'QWSMIN': ('min_surface_water_rate', float),
+            'QLIQSMIN': ('min_surface_liquid_rate', float),
+            'QOMIN': ('min_reservoir_oil_rate', float),
+            'QGMIN': ('min_reservoir_gas_rate', float),
+            'QWMIN': ('min_reservoir_water_rate', float),
+            'QLIQMIN': ('min_reservoir_liquid_rate', float),
+            'QALLMIN': ('min_reservoir_total_fluids_rate', float),
+            'QHCMIN': ('min_reservoir_hc_rate', float),
+            'QOSMIN-': ('min_reverse_surface_oil_rate', float),
+            'QGSMIN-': ('min_reverse_surface_gas_rate', float),
+            'QWSMIN-': ('min_reverse_surface_water_rate', float),
+            'QLIQSMIN-': ('min_reverse_surface_liquid_rate', float),
+            'QOMIN-': ('min_reverse_reservoir_oil_rate', float),
+            'QGMIN-': ('min_reverse_reservoir_gas_rate', float),
+            'QWMIN-': ('min_reverse_reservoir_water_rate', float),
+            'QLIQMIN-': ('min_reverse_reservoir_liquid_rate', float),
+            'QALLMIN-': ('min_reverse_reservoir_total_fluids_rate', float),
+            'QHCMIN-': ('min_reverse_reservoir_hc_rate', float),
+
+            'QOIL': ('qmult_oil_rate', float),
+            'QWATER': ('qmult_water_rate', float),
+            'QGAS': ('qmult_gas_rate', float),
+            'DPBHAVG': ('max_avg_comp_dp', float),
+            'DPBHMX': ('max_comp_dp', float),
+            }
+        return nexus_mapping
+
+    @staticmethod
+    def get_pressure_constraints_map() -> dict[str, tuple[str, type]]:
+        nexus_mapping: dict[str, tuple[str, type]] = {
+            'PMIN': ('min_pressure', float),
+            'PMAX': ('max_pressure', float),
+            'PWMAX': ('max_wag_water_pressure', float),
+            'PGMAX': ('max_wag_gas_pressure', float),
+            'BHP': ('bottom_hole_pressure', float),
+            'THP': ('tubing_head_pressure', float),
+            }
+        return nexus_mapping
+
+    @staticmethod
+    def get_limit_constraints_map() -> dict[str, tuple[str, type]]:
+        nexus_mapping: dict[str, tuple[str, type]] = {
+            'WCUTMAX': ('max_watercut', float),
+            'WCUTPLUG': ('max_watercut_plug', float),
+            'WCUTPLUGPLUS': ('max_watercut_plugplus', float),
+            'WCUTPERF': ('max_watercut_perf', float),
+            'WCUTPERFPLUS': ('max_watercut_perfplus', float),
+            'WORMAX': ('max_wor', float),
+            'WORPLUG': ('max_wor_plug', float),
+            'WORPLUGPLUS': ('max_wor_plug_plus', float),
+            'WORPERF': ('max_wor_perf', float),
+            'WORPERFPLUS': ('max_wor_perfplus', float),
+            'GORLIM': ('gor_limit', float),
+            'EXPONENT': ('gor_limit_exponent', float),
+            'FREQUENCY': ('gor_limit_frequency', float),
+            'GORMAX': ('max_gor', float),
+            'GORPLUG': ('max_gor_plug', float),
+            'GORPLUGPLUS': ('max_gor_plug_plus', float),
+            'GORPERF': ('max_gor_perf', float),
+            'GORPERFPLUS': ('max_gor_perfplus', float),
+            'LGRMAX': ('max_lgr', float),
+            'LGRPLUG': ('max_lgr_plug', float),
+            'LGRPLUGPLUS': ('max_lgr_plug_plus', float),
+            'LGRPERF': ('max_lgr_perf', float),
+            'LGRPERFPLUS': ('max_lgr_perfplus', float),
+            'CGLIM': ('max_cum_gas_prod', float),
+            'CWLIM': ('max_cum_water_prod', float),
+            'COLIM': ('max_cum_oil_prod', float),
+            }
+        return nexus_mapping
+
+    @staticmethod
+    def get_alq_constraints_map() -> dict[str, tuple[str, type]]:
+        """Gets the nexus mapping for artificial lift constraints."""
+        nexus_mapping: dict[str, tuple[str, type]] = {
+            'ALQ': ('artificial_lift_number', int),
+            'SETTING': ('max_choke_setting', float),
+            'GLEFMIN': ('min_gas_lift_efficiency', float),
+            'GLRADD': ('gl_additive_correction', float),
+            'ACTIVATE': ('active_node', bool),
+            'POWER': ('pump_power', float),
+            'SPEED': ('pump_speed', float),
+            'CHOKELIMIT': ('choke_limit', str),
+            'POSITION': ('manifold_position', int),
+            }
+        return nexus_mapping
+
+    def to_dict(self, keys_in_nexus_style: bool = False) -> dict[str, None | str | int | float]:
+        """Returns a dictionary of the attributes of the Constraint.
+
+        Args:
+            keys_in_nexus_style (bool): if True returns the key values in Nexus keywords, otherwise returns the \
+                attribute name as stored by ressimpy.
+
+        Returns:
+            a dictionary keyed by attributes and values as the value of the attribute
+        """
+        result_dict = to_dict_generic.to_dict(self, keys_in_nexus_style, add_date=True, add_units=True)
+        return result_dict
+
+    def update(self, new_data: dict[str, None | int | str | float | UnitSystem], nones_overwrite: bool = False):
+        """Updates attributes in the object based on the dictionary provided."""
+        for k, v in new_data.items():
+            if v is not None or nones_overwrite:
+                setattr(self, k, v)
+
+    def to_table_line(self) -> str:
+        """String representation of the constraint for entry to an inline constraint table."""
+        qmult_control_key_words = ['QALLRMAX_MULT', 'QOSMAX_MULT', 'QWSMAX_MULT', 'QGSMAX_MULT', 'QLIQSMAX_MULT']
+        skip_attributes = ['date', 'unit_system', 'NAME', 'ACTIVATE', 'QOIL', 'QWATER', 'QGAS', 'WELL']
+        clear_attributes = ['CLEAR', 'CLEARQ', 'CLEARP', 'CLEARLIMIT', 'CLEARALQ']
+
+        if self.name is not None:
+            constraint_string = self.name
+        elif self.well_name is not None:
+            constraint_string = self.well_name
+        else:
+            raise ValueError('Must have a well or node name for returning a constraint to a string')
+
+        for attribute, value in self.to_dict(keys_in_nexus_style=True).items():
+            if value and attribute in qmult_control_key_words:
+                constraint_string += (' ' + attribute.replace('_MULT', '') + ' MULT')
+            elif value is None or attribute in skip_attributes:
+                continue
+            elif value and attribute in clear_attributes:
+                constraint_string += ' ' + attribute
+            else:
+                constraint_string += (' ' + attribute + ' ' + str(value))
+
+        if self.active_node:
+            constraint_string += ' ACTIVATE'
+        elif self.active_node is not None:
+            # equivalent to active node being False
+            constraint_string += ' DEACTIVATE'
+
+        constraint_string += '\n'
+        return constraint_string
+
+    def write_qmult_table(self) -> list[str]:
+        """Writes out a QMULT table from a constraint that uses the following attributes.
+        'QOIL': ('qmult_oil_rate', float).
+        'QWATER': ('qmult_water_rate', float).
+        'QGAS': ('qmult_gas_rate', float).
+
+        Returns:
+            list[str] with a representation of the QMULT table with a new line as a new entry in the list.
+        """
+        table_to_return = ['QMULT\n', 'WELL QOIL QGAS QWATER\n']
+        qmult_values = self.write_qmult_values()
+        table_to_return.append(qmult_values)
+        table_to_return.append('ENDQMULT\n')
+
+        return table_to_return
+
+    def write_qmult_values(self) -> str:
+        """Writes out the values for a QMULT table, callable on its own or using the write_qmult_table method."""
+        qmult_values_keywords = ['qmult_oil_rate', 'qmult_gas_rate', 'qmult_water_rate']
+        if self.name is not None:
+            string_to_return = self.name
+        elif self.well_name is not None:
+            string_to_return = self.well_name
+        else:
+            raise ValueError('Must have a well or node name for returning a qmult table')
+
+        for keyword in qmult_values_keywords:
+            value = getattr(self, keyword, None)
+            if value is None:
+                string_to_return += ' NA'
+            else:
+                string_to_return += f' {str(value)}'
+        string_to_return += '\n'
+        return string_to_return
```

### Comparing `ressimpy-1.0.0/ResSimpy/Nexus/DataModels/Network/NexusConstraints.py` & `ressimpy-1.0.1/ResSimpy/Nexus/DataModels/Network/NexusConstraints.py`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,328 +1,328 @@
-from __future__ import annotations
-
-from dataclasses import dataclass, field
-from typing import TYPE_CHECKING, Optional, Mapping, Sequence, cast
-from uuid import UUID
-
-import pandas as pd
-
-from ResSimpy.Constraint import Constraint
-from ResSimpy.Constraints import Constraints
-from ResSimpy.Nexus.nexus_collect_tables import collect_all_tables_to_objects
-from ResSimpy.Nexus.DataModels.Network.NexusConstraint import NexusConstraint
-from ResSimpy.Nexus.DataModels.NexusFile import NexusFile
-from ResSimpy.Enums.UnitsEnum import UnitSystem
-from ResSimpy.Utils.obj_to_dataframe import obj_to_dataframe
-import ResSimpy.Nexus.nexus_file_operations as nfo
-
-if TYPE_CHECKING:
-    from ResSimpy.Nexus.NexusNetwork import NexusNetwork
-    from ResSimpy.Nexus.NexusSimulator import NexusSimulator
-
-
-@dataclass
-class NexusConstraints(Constraints):
-    __constraints: dict[str, list[NexusConstraint]] = field(default_factory=lambda: {})
-
-    def __init__(self, parent_network: NexusNetwork, model: NexusSimulator) -> None:
-        self.__parent_network: NexusNetwork = parent_network
-        self.__constraints: dict[str, list[NexusConstraint]] = {}
-        self.__model: NexusSimulator = model
-
-    def get_all(self, object_name: Optional[str] = None, date: Optional[str] = None) -> \
-            Mapping[str, Sequence[NexusConstraint]]:
-        """Get the constraints of the existing model with optional parameters to filter for name and date
-        Args:
-            object_name (Optional[str]): name of the connection, node or wellname to return. Defaults to None.
-            date (Optional[str]): date in model format to filter the dates to in the constraints
-        Returns: dict[str, list[NexusConstraint]] dictionary of all constraints defined within a model, keyed by the \
-            name of the well/node.
-        """
-        self.__parent_network.get_load_status()
-
-        if object_name is None:
-            constraints_to_return = self.__constraints
-        else:
-            constraints_to_return = {k: v for k, v in self.__constraints.items() if k == object_name}
-
-        if date is None:
-            return constraints_to_return
-
-        date_filtered_constraints = {}
-        for constraint_name, constraint_list in constraints_to_return.items():
-            new_constraint_list = [x for x in constraint_list if x.date == date]
-            if len(new_constraint_list) > 0:
-                date_filtered_constraints[constraint_name] = new_constraint_list
-        return date_filtered_constraints
-
-    def get_df(self) -> pd.DataFrame:
-        """Creates a dataframe representing all processed constraint data in a surface file
-        Returns:
-            DataFrame: of the properties of the constraint through time with each row representing \
-                a change in constraint.
-        """
-        self.__parent_network.get_load_status()
-        list_constraints = []
-        for well_constraints in self.__constraints.values():
-            list_constraints.extend(well_constraints)
-        obj_to_dataframe(list_constraints)
-
-        return obj_to_dataframe(list_constraints)
-
-    def get_overview(self) -> str:
-        raise NotImplementedError('To be implemented')
-
-    def load(self, surface_file: NexusFile, start_date: str, default_units: UnitSystem) -> None:
-        # CONSTRAINT keyword represents a table with a header and columns.
-        # CONSTRAINTS keyword represents a list of semi structured constraints with a well_name and then constraints
-        new_constraints = collect_all_tables_to_objects(surface_file,
-                                                        {
-                                                            'CONSTRAINTS': NexusConstraint,
-                                                            'CONSTRAINT': NexusConstraint,
-                                                            'QMULT': NexusConstraint
-                                                        },
-                                                        start_date=start_date,
-                                                        default_units=default_units)
-        cons_list = new_constraints.get('CONSTRAINTS')
-        if isinstance(cons_list, list):
-            raise ValueError(
-                'Incompatible data format for additional constraints. Expected type "dict" instead got "list"')
-        self._add_to_memory(cons_list)
-
-    def _add_to_memory(self, additional_constraints: Optional[dict[str, list[NexusConstraint]]]) -> None:
-        """Adds additional constraints to memory within the NexusConstraints object.
-            If user adds constraints list this will not be reflected in the Nexus deck at this time.
-
-        Args:
-        ----
-            additional_constraints (list[NexusConstraint]): additional constraints to add as a list
-        """
-        if additional_constraints is None:
-            return
-        self.__constraints.update(additional_constraints)
-
-    def find_by_properties(self, object_name: str, constraint_dict: dict[str, None | float | str | int]) -> \
-            NexusConstraint:
-        """Finds a uniquely matching constraint from a given set of properties in a dictionary of attributes.
-
-        Args:
-            object_name (str): name of the node to which the constraint is applied (node name/well name)
-            constraint_dict (dict[str, float | str | int]): dictionary of attributes to match on. \
-            Allows for partial matches if it finds a unique constraint.
-
-        Returns:
-            NexusConstraint of an existing constraint in the model that uniquely matches the provided \
-            constraint_dict constraint
-        """
-        self.__parent_network.get_load_status()
-        found_object_from_network = self.__parent_network.find_network_element_with_dict(object_name, constraint_dict,
-                                                                                         'constraints')
-        # ensure typing is consistent
-        if isinstance(found_object_from_network, NexusConstraint):
-            return found_object_from_network
-        else:
-            raise TypeError(f'Wrong object type returned expected NexusConstraint, '
-                            f'instead returned {type(found_object_from_network)}')
-
-    def remove(self, constraint_dict: Optional[dict[str, None | float | str | int]] = None,
-               constraint_id: Optional[UUID] = None) -> None:
-        """Remove a constraint based on closest matching constraint, requires node name and date.\
-        Needs one of at least constraint dict or constraint id.
-
-        Args:
-            constraint_dict (Optional[dict[str, float | str | int]]): Constraint matching these attributes will be
-                removed. Defaults to None.
-            constraint_id (Optional[UUID]): Constraint matching this id will be removed.
-                Will not be used if constraint dict is provided. Defaults to None.
-        """
-        self.__parent_network.get_load_status()
-
-        if constraint_dict is None and constraint_id is None:
-            raise ValueError('no options provided for both constraint_id and constraint_dict')
-        if constraint_dict is not None:
-            name = constraint_dict.get('name', None)
-            if name is None:
-                raise ValueError(f'No well or node name provided instead got {name}')
-            name = str(name)
-            # check for wildcards
-            if '*' in name:
-                raise NotImplementedError(f'Removing constraints with wildcards is currently unsupported, for {name=}')
-            constraint_to_remove = self.find_by_properties(name, constraint_dict)
-            constraint_id = constraint_to_remove.id
-        if constraint_id is None:
-            raise ValueError(f'No constraint found with {constraint_id=}')
-        # find which file and remove from the file as list
-        surface_file = self.__find_which_surface_file_from_id(constraint_id)
-        surface_file.remove_object_from_file_as_list([constraint_id])
-        # remove from memory
-        for name, list_constraints in self.__constraints.items():
-            for i, constraint in enumerate(list_constraints):
-                if constraint.id == constraint_id:
-                    list_constraints.pop(i)
-
-    def __find_which_surface_file_from_id(self, constraint_id: UUID) -> NexusFile:
-        """Finds the surface file with the object id requested."""
-        # TODO: make this generic with the find_which_wellspec_file_from_completion_id.
-
-        if self.__model.model_files.surface_files is None:
-            raise ValueError(f'No surface file found in fcs file at {self.__model.model_files.location}')
-        surface_files = [x for x in self.__model.model_files.surface_files.values() if
-                         x.object_locations is not None and constraint_id in x.object_locations]
-        if len(surface_files) == 0:
-            raise FileNotFoundError(f'No surface file found with an existing constraint that has: {constraint_id=}')
-        surface_file = surface_files[0]
-        if surface_file.file_content_as_list is None:
-            raise FileNotFoundError(f'No file content found in file: {surface_file.location} '
-                                    f'with an existing constraint that has: {constraint_id=}')
-        return surface_file
-
-    def add(self,
-            name: str,
-            constraint_to_add: dict[str, None | float | int | str | UnitSystem] | Constraint,
-            comments: Optional[str] = None) -> None:
-        """Adds a constraint to the network and corresponding surface file.
-
-        Args:
-            name (str): name of the node to apply constraints to
-            constraint_to_add (dict[str, float | int | str | UnitSystem] | NexusConstraint): properties of \
-            the constraints or a constraint object
-        """
-        self.__parent_network.get_load_status()
-
-        # check for wildcards
-        if '*' in name:
-            raise NotImplementedError('Adding constraints with wildcards is currently unsupported')
-        # add to memory
-        if isinstance(constraint_to_add, dict):
-            new_constraint = NexusConstraint(constraint_to_add)
-        else:
-            new_constraint = cast(NexusConstraint, constraint_to_add)
-
-        self._add_to_memory({name: [new_constraint]})
-
-        # add to the file
-        if self.__model.model_files.surface_files is None:
-            raise FileNotFoundError('No well file found, cannot modify ')
-
-        file_to_add_to = self.__model.model_files.surface_files[1]
-
-        file_as_list = file_to_add_to.get_flat_list_str_file
-        if file_as_list is None:
-            raise ValueError(f'No file content found in the surface file specified at {file_to_add_to.location}')
-
-        constraint_date = new_constraint.date
-        if constraint_date is None:
-            raise ValueError(f'Require date for adding constraint to, instead got {new_constraint.date}')
-        new_constraint_text = []
-        date_comparison = -1
-        date_index = -1
-        new_constraint_index = -1
-        id_line_locs = []
-        new_table_needed = False
-        new_date_needed = False
-        new_qmults_table_needed = False
-        # check for need to add qmult table
-        qmult_keywords = ['qmult_oil_rate', 'qmult_gas_rate', 'qmult_water_rate']
-        # if any of the qmults are defined in the new constraint then add a qmult table
-        add_qmults = any(getattr(new_constraint, x, None) for x in qmult_keywords)
-
-        for index, line in enumerate(file_as_list):
-            if nfo.check_token('TIME', line):
-                constraint_date_from_file = nfo.get_expected_token_value('TIME', line, [line])
-                date_comparison = self.__model._sim_controls.compare_dates(constraint_date_from_file, constraint_date)
-                if date_comparison == 0:
-                    date_index = index
-                    continue
-
-                elif date_comparison > 0 and date_index >= 0:
-                    # if a date that is greater than the additional constraint then we have overshot and need to
-                    # add in a new table or time card
-                    # this is the case where we don't need to write a new time card
-                    new_table_needed = True
-                    new_constraint_index = index - 1
-                elif date_comparison > 0:
-                    new_table_needed = True
-                    new_date_needed = True
-                    new_constraint_index = index
-                else:
-                    continue
-            if nfo.check_token('ENDCONSTRAINTS', line) and date_comparison == 0:
-                # find the end of a constraint table and add the new constraint
-                new_constraint_index = index
-                constraint_string = new_constraint.to_table_line()
-                new_constraint_text.append(constraint_string)
-                id_line_locs = [new_constraint_index]
-            elif index == len(file_as_list) - 1 and date_index >= 0 and not nfo.check_token('ENDQMULT', line):
-                # if we're on the final line of the file and we haven't yet set a constraint index
-                new_table_needed = True
-                new_constraint_index = index
-                if add_qmults:
-                    new_qmults_table_needed = True
-
-            if new_date_needed:
-                # if the date card doesn't exist then add it to the file first
-                new_constraint_text.append(f'TIME {constraint_date}\n')
-
-            if new_table_needed:
-                new_constraint_text.append('CONSTRAINTS\n')
-                new_constraint_text.append(new_constraint.to_table_line())
-                new_constraint_text.append('ENDCONSTRAINTS\n')
-                id_line_locs = [new_constraint_index + len(new_constraint_text) - 2]
-
-            if add_qmults and new_qmults_table_needed:
-                new_constraint_text.extend(new_constraint.write_qmult_table())
-                # add id location for the qmult table as well
-                id_line_locs.append(new_constraint_index + len(new_constraint_text) - 2)
-                add_qmults = False
-            elif add_qmults and nfo.check_token('ENDQMULT', line) and date_comparison == 0:
-                # find the end of the table of qmults that already exist
-                new_qmult_index = index
-                qmult_string = new_constraint.write_qmult_values()
-                new_qmult_object_ids = {new_constraint.id: [new_qmult_index]}
-                file_to_add_to.add_to_file_as_list(additional_content=[qmult_string], index=new_qmult_index,
-                                                   additional_objects=new_qmult_object_ids)
-                add_qmults = False
-
-            if new_constraint_index >= 0 and not add_qmults:
-                # once we have found where to add constraint then add the constraint to file and update file ids
-                new_constraint_object_ids = {
-                    new_constraint.id: id_line_locs
-                }
-                file_to_add_to.add_to_file_as_list(additional_content=new_constraint_text, index=new_constraint_index,
-                                                   additional_objects=new_constraint_object_ids, comments=comments)
-                break
-
-    def modify(self, name: str,
-               current_constraint: dict[str, None | float | int | str] | Constraint,
-               new_constraint_props: dict[str, None | float | int | str | UnitSystem] | Constraint,
-               comments: Optional[str] = None) \
-            -> None:
-        """Modify an existing constraint. Retains existing constraint values that are not overridden by the new \
-        constraint properties.
-
-        Args:
-            name (str):
-            current_constraint (dict[str, None | float | int | str] | Constraint): dictionary or constraint object\
-                with enough attributes to identify a unique existing constraint in the model.
-            new_constraint_props (dict[str, None | float | int | str] | Constraint): dictionary or constraint to \
-            update the constraint with.
-        """
-
-        def clean_constraint_inputs(constraint: dict[str, None | float | int | str] | Constraint) -> \
-                dict[str, None | float | int | str]:
-            """Cleans up an input ensuring consistent type is returned."""
-            if isinstance(constraint, Constraint):
-                cleaned_dict = constraint.to_dict()
-            else:
-                cleaned_dict = constraint
-            return cleaned_dict
-
-        cleaned_current_constraint = clean_constraint_inputs(current_constraint)
-        cleaned_new_constraint = clean_constraint_inputs(new_constraint_props)
-
-        existing_constraint_obj = self.find_by_properties(name, cleaned_current_constraint)
-        self.remove(constraint_id=existing_constraint_obj.id)
-        combination_of_constraints = existing_constraint_obj.to_dict()
-        combination_of_constraints.update(cleaned_new_constraint)
-
-        self.add(name, combination_of_constraints, comments)
+from __future__ import annotations
+
+from dataclasses import dataclass, field
+from typing import TYPE_CHECKING, Optional, Mapping, Sequence, cast
+from uuid import UUID
+
+import pandas as pd
+
+from ResSimpy.Constraint import Constraint
+from ResSimpy.Constraints import Constraints
+from ResSimpy.Nexus.nexus_collect_tables import collect_all_tables_to_objects
+from ResSimpy.Nexus.DataModels.Network.NexusConstraint import NexusConstraint
+from ResSimpy.Nexus.DataModels.NexusFile import NexusFile
+from ResSimpy.Enums.UnitsEnum import UnitSystem
+from ResSimpy.Utils.obj_to_dataframe import obj_to_dataframe
+import ResSimpy.Nexus.nexus_file_operations as nfo
+
+if TYPE_CHECKING:
+    from ResSimpy.Nexus.NexusNetwork import NexusNetwork
+    from ResSimpy.Nexus.NexusSimulator import NexusSimulator
+
+
+@dataclass
+class NexusConstraints(Constraints):
+    __constraints: dict[str, list[NexusConstraint]] = field(default_factory=lambda: {})
+
+    def __init__(self, parent_network: NexusNetwork, model: NexusSimulator) -> None:
+        self.__parent_network: NexusNetwork = parent_network
+        self.__constraints: dict[str, list[NexusConstraint]] = {}
+        self.__model: NexusSimulator = model
+
+    def get_all(self, object_name: Optional[str] = None, date: Optional[str] = None) -> \
+            Mapping[str, Sequence[NexusConstraint]]:
+        """Get the constraints of the existing model with optional parameters to filter for name and date
+        Args:
+            object_name (Optional[str]): name of the connection, node or wellname to return. Defaults to None.
+            date (Optional[str]): date in model format to filter the dates to in the constraints
+        Returns: dict[str, list[NexusConstraint]] dictionary of all constraints defined within a model, keyed by the \
+            name of the well/node.
+        """
+        self.__parent_network.get_load_status()
+
+        if object_name is None:
+            constraints_to_return = self.__constraints
+        else:
+            constraints_to_return = {k: v for k, v in self.__constraints.items() if k == object_name}
+
+        if date is None:
+            return constraints_to_return
+
+        date_filtered_constraints = {}
+        for constraint_name, constraint_list in constraints_to_return.items():
+            new_constraint_list = [x for x in constraint_list if x.date == date]
+            if len(new_constraint_list) > 0:
+                date_filtered_constraints[constraint_name] = new_constraint_list
+        return date_filtered_constraints
+
+    def get_df(self) -> pd.DataFrame:
+        """Creates a dataframe representing all processed constraint data in a surface file
+        Returns:
+            DataFrame: of the properties of the constraint through time with each row representing \
+                a change in constraint.
+        """
+        self.__parent_network.get_load_status()
+        list_constraints = []
+        for well_constraints in self.__constraints.values():
+            list_constraints.extend(well_constraints)
+        obj_to_dataframe(list_constraints)
+
+        return obj_to_dataframe(list_constraints)
+
+    def get_overview(self) -> str:
+        raise NotImplementedError('To be implemented')
+
+    def load(self, surface_file: NexusFile, start_date: str, default_units: UnitSystem) -> None:
+        # CONSTRAINT keyword represents a table with a header and columns.
+        # CONSTRAINTS keyword represents a list of semi structured constraints with a well_name and then constraints
+        new_constraints = collect_all_tables_to_objects(surface_file,
+                                                        {
+                                                            'CONSTRAINTS': NexusConstraint,
+                                                            'CONSTRAINT': NexusConstraint,
+                                                            'QMULT': NexusConstraint
+                                                        },
+                                                        start_date=start_date,
+                                                        default_units=default_units)
+        cons_list = new_constraints.get('CONSTRAINTS')
+        if isinstance(cons_list, list):
+            raise ValueError(
+                'Incompatible data format for additional constraints. Expected type "dict" instead got "list"')
+        self._add_to_memory(cons_list)
+
+    def _add_to_memory(self, additional_constraints: Optional[dict[str, list[NexusConstraint]]]) -> None:
+        """Adds additional constraints to memory within the NexusConstraints object.
+            If user adds constraints list this will not be reflected in the Nexus deck at this time.
+
+        Args:
+        ----
+            additional_constraints (list[NexusConstraint]): additional constraints to add as a list
+        """
+        if additional_constraints is None:
+            return
+        self.__constraints.update(additional_constraints)
+
+    def find_by_properties(self, object_name: str, constraint_dict: dict[str, None | float | str | int]) -> \
+            NexusConstraint:
+        """Finds a uniquely matching constraint from a given set of properties in a dictionary of attributes.
+
+        Args:
+            object_name (str): name of the node to which the constraint is applied (node name/well name)
+            constraint_dict (dict[str, float | str | int]): dictionary of attributes to match on. \
+            Allows for partial matches if it finds a unique constraint.
+
+        Returns:
+            NexusConstraint of an existing constraint in the model that uniquely matches the provided \
+            constraint_dict constraint
+        """
+        self.__parent_network.get_load_status()
+        found_object_from_network = self.__parent_network.find_network_element_with_dict(object_name, constraint_dict,
+                                                                                         'constraints')
+        # ensure typing is consistent
+        if isinstance(found_object_from_network, NexusConstraint):
+            return found_object_from_network
+        else:
+            raise TypeError(f'Wrong object type returned expected NexusConstraint, '
+                            f'instead returned {type(found_object_from_network)}')
+
+    def remove(self, constraint_dict: Optional[dict[str, None | float | str | int]] = None,
+               constraint_id: Optional[UUID] = None) -> None:
+        """Remove a constraint based on closest matching constraint, requires node name and date.\
+        Needs one of at least constraint dict or constraint id.
+
+        Args:
+            constraint_dict (Optional[dict[str, float | str | int]]): Constraint matching these attributes will be
+                removed. Defaults to None.
+            constraint_id (Optional[UUID]): Constraint matching this id will be removed.
+                Will not be used if constraint dict is provided. Defaults to None.
+        """
+        self.__parent_network.get_load_status()
+
+        if constraint_dict is None and constraint_id is None:
+            raise ValueError('no options provided for both constraint_id and constraint_dict')
+        if constraint_dict is not None:
+            name = constraint_dict.get('name', None)
+            if name is None:
+                raise ValueError(f'No well or node name provided instead got {name}')
+            name = str(name)
+            # check for wildcards
+            if '*' in name:
+                raise NotImplementedError(f'Removing constraints with wildcards is currently unsupported, for {name=}')
+            constraint_to_remove = self.find_by_properties(name, constraint_dict)
+            constraint_id = constraint_to_remove.id
+        if constraint_id is None:
+            raise ValueError(f'No constraint found with {constraint_id=}')
+        # find which file and remove from the file as list
+        surface_file = self.__find_which_surface_file_from_id(constraint_id)
+        surface_file.remove_object_from_file_as_list([constraint_id])
+        # remove from memory
+        for name, list_constraints in self.__constraints.items():
+            for i, constraint in enumerate(list_constraints):
+                if constraint.id == constraint_id:
+                    list_constraints.pop(i)
+
+    def __find_which_surface_file_from_id(self, constraint_id: UUID) -> NexusFile:
+        """Finds the surface file with the object id requested."""
+        # TODO: make this generic with the find_which_wellspec_file_from_completion_id.
+
+        if self.__model.model_files.surface_files is None:
+            raise ValueError(f'No surface file found in fcs file at {self.__model.model_files.location}')
+        surface_files = [x for x in self.__model.model_files.surface_files.values() if
+                         x.object_locations is not None and constraint_id in x.object_locations]
+        if len(surface_files) == 0:
+            raise FileNotFoundError(f'No surface file found with an existing constraint that has: {constraint_id=}')
+        surface_file = surface_files[0]
+        if surface_file.file_content_as_list is None:
+            raise FileNotFoundError(f'No file content found in file: {surface_file.location} '
+                                    f'with an existing constraint that has: {constraint_id=}')
+        return surface_file
+
+    def add(self,
+            name: str,
+            constraint_to_add: dict[str, None | float | int | str | UnitSystem] | Constraint,
+            comments: Optional[str] = None) -> None:
+        """Adds a constraint to the network and corresponding surface file.
+
+        Args:
+            name (str): name of the node to apply constraints to
+            constraint_to_add (dict[str, float | int | str | UnitSystem] | NexusConstraint): properties of \
+            the constraints or a constraint object
+        """
+        self.__parent_network.get_load_status()
+
+        # check for wildcards
+        if '*' in name:
+            raise NotImplementedError('Adding constraints with wildcards is currently unsupported')
+        # add to memory
+        if isinstance(constraint_to_add, dict):
+            new_constraint = NexusConstraint(constraint_to_add)
+        else:
+            new_constraint = cast(NexusConstraint, constraint_to_add)
+
+        self._add_to_memory({name: [new_constraint]})
+
+        # add to the file
+        if self.__model.model_files.surface_files is None:
+            raise FileNotFoundError('No well file found, cannot modify ')
+
+        file_to_add_to = self.__model.model_files.surface_files[1]
+
+        file_as_list = file_to_add_to.get_flat_list_str_file
+        if file_as_list is None:
+            raise ValueError(f'No file content found in the surface file specified at {file_to_add_to.location}')
+
+        constraint_date = new_constraint.date
+        if constraint_date is None:
+            raise ValueError(f'Require date for adding constraint to, instead got {new_constraint.date}')
+        new_constraint_text = []
+        date_comparison = -1
+        date_index = -1
+        new_constraint_index = -1
+        id_line_locs = []
+        new_table_needed = False
+        new_date_needed = False
+        new_qmults_table_needed = False
+        # check for need to add qmult table
+        qmult_keywords = ['qmult_oil_rate', 'qmult_gas_rate', 'qmult_water_rate']
+        # if any of the qmults are defined in the new constraint then add a qmult table
+        add_qmults = any(getattr(new_constraint, x, None) for x in qmult_keywords)
+
+        for index, line in enumerate(file_as_list):
+            if nfo.check_token('TIME', line):
+                constraint_date_from_file = nfo.get_expected_token_value('TIME', line, [line])
+                date_comparison = self.__model._sim_controls.compare_dates(constraint_date_from_file, constraint_date)
+                if date_comparison == 0:
+                    date_index = index
+                    continue
+
+                elif date_comparison > 0 and date_index >= 0:
+                    # if a date that is greater than the additional constraint then we have overshot and need to
+                    # add in a new table or time card
+                    # this is the case where we don't need to write a new time card
+                    new_table_needed = True
+                    new_constraint_index = index - 1
+                elif date_comparison > 0:
+                    new_table_needed = True
+                    new_date_needed = True
+                    new_constraint_index = index
+                else:
+                    continue
+            if nfo.check_token('ENDCONSTRAINTS', line) and date_comparison == 0:
+                # find the end of a constraint table and add the new constraint
+                new_constraint_index = index
+                constraint_string = new_constraint.to_table_line()
+                new_constraint_text.append(constraint_string)
+                id_line_locs = [new_constraint_index]
+            elif index == len(file_as_list) - 1 and date_index >= 0 and not nfo.check_token('ENDQMULT', line):
+                # if we're on the final line of the file and we haven't yet set a constraint index
+                new_table_needed = True
+                new_constraint_index = index
+                if add_qmults:
+                    new_qmults_table_needed = True
+
+            if new_date_needed:
+                # if the date card doesn't exist then add it to the file first
+                new_constraint_text.append(f'TIME {constraint_date}\n')
+
+            if new_table_needed:
+                new_constraint_text.append('CONSTRAINTS\n')
+                new_constraint_text.append(new_constraint.to_table_line())
+                new_constraint_text.append('ENDCONSTRAINTS\n')
+                id_line_locs = [new_constraint_index + len(new_constraint_text) - 2]
+
+            if add_qmults and new_qmults_table_needed:
+                new_constraint_text.extend(new_constraint.write_qmult_table())
+                # add id location for the qmult table as well
+                id_line_locs.append(new_constraint_index + len(new_constraint_text) - 2)
+                add_qmults = False
+            elif add_qmults and nfo.check_token('ENDQMULT', line) and date_comparison == 0:
+                # find the end of the table of qmults that already exist
+                new_qmult_index = index
+                qmult_string = new_constraint.write_qmult_values()
+                new_qmult_object_ids = {new_constraint.id: [new_qmult_index]}
+                file_to_add_to.add_to_file_as_list(additional_content=[qmult_string], index=new_qmult_index,
+                                                   additional_objects=new_qmult_object_ids)
+                add_qmults = False
+
+            if new_constraint_index >= 0 and not add_qmults:
+                # once we have found where to add constraint then add the constraint to file and update file ids
+                new_constraint_object_ids = {
+                    new_constraint.id: id_line_locs
+                }
+                file_to_add_to.add_to_file_as_list(additional_content=new_constraint_text, index=new_constraint_index,
+                                                   additional_objects=new_constraint_object_ids, comments=comments)
+                break
+
+    def modify(self, name: str,
+               current_constraint: dict[str, None | float | int | str] | Constraint,
+               new_constraint_props: dict[str, None | float | int | str | UnitSystem] | Constraint,
+               comments: Optional[str] = None) \
+            -> None:
+        """Modify an existing constraint. Retains existing constraint values that are not overridden by the new \
+        constraint properties.
+
+        Args:
+            name (str):
+            current_constraint (dict[str, None | float | int | str] | Constraint): dictionary or constraint object\
+                with enough attributes to identify a unique existing constraint in the model.
+            new_constraint_props (dict[str, None | float | int | str] | Constraint): dictionary or constraint to \
+            update the constraint with.
+        """
+
+        def clean_constraint_inputs(constraint: dict[str, None | float | int | str] | Constraint) -> \
+                dict[str, None | float | int | str]:
+            """Cleans up an input ensuring consistent type is returned."""
+            if isinstance(constraint, Constraint):
+                cleaned_dict = constraint.to_dict()
+            else:
+                cleaned_dict = constraint
+            return cleaned_dict
+
+        cleaned_current_constraint = clean_constraint_inputs(current_constraint)
+        cleaned_new_constraint = clean_constraint_inputs(new_constraint_props)
+
+        existing_constraint_obj = self.find_by_properties(name, cleaned_current_constraint)
+        self.remove(constraint_id=existing_constraint_obj.id)
+        combination_of_constraints = existing_constraint_obj.to_dict()
+        combination_of_constraints.update(cleaned_new_constraint)
+
+        self.add(name, combination_of_constraints, comments)
```

### Comparing `ressimpy-1.0.0/ResSimpy/Nexus/DataModels/Network/NexusNode.py` & `ressimpy-1.0.1/ResSimpy/Nexus/DataModels/Network/NexusNode.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,70 +1,70 @@
-from __future__ import annotations
-from dataclasses import dataclass
-from typing import Optional
-
-from ResSimpy.Node import Node
-from ResSimpy.Utils import to_dict_generic
-from ResSimpy.Utils.generic_repr import generic_repr
-from ResSimpy.Utils.obj_to_table_string import to_table_line
-
-
-@dataclass(kw_only=True)
-class NexusNode(Node):
-    x_pos: Optional[float] = None
-    y_pos: Optional[float] = None
-    number: Optional[int] = None
-    temp: Optional[float] = None
-    station: Optional[str] = None
-
-    def __init__(self, properties_dict: dict[str, None | int | str | float]) -> None:
-        super().__init__()
-        for key, prop in properties_dict.items():
-            self.__setattr__(key, prop)
-
-    def __repr__(self) -> str:
-        return generic_repr(self)
-
-    @staticmethod
-    def get_nexus_mapping() -> dict[str, tuple[str, type]]:
-        """Gets the mapping of nexus keywords to attribute definitions."""
-        keywords = {
-            'NAME': ('name', str),
-            'TYPE': ('type', str),
-            'DEPTH': ('depth', float),
-            'TEMP': ('temp', float),
-            'X': ('x_pos', float),
-            'Y': ('y_pos', float),
-            'NUMBER': ('number', int),
-            'STATION': ('station', str),
-        }
-        return keywords
-
-    def to_dict(self, keys_in_nexus_style: bool = False, include_nones: bool = True) -> \
-            dict[str, None | str | int | float]:
-        """Returns a dictionary of the attributes of the Node.
-
-        Args:
-            keys_in_nexus_style (bool): if True returns the key values in Nexus keywords, otherwise returns the \
-                attribute name as stored by ressimpy.
-            include_nones (bool): If False filters the nones out of the dictionary. Defaults to True
-
-        Returns:
-            a dictionary keyed by attributes and values as the value of the attribute
-        """
-        result_dict = to_dict_generic.to_dict(self, keys_in_nexus_style, add_date=True, add_units=True,
-                                              include_nones=include_nones)
-        return result_dict
-
-    def to_table_line(self, headers: list[str]) -> str:
-        """Returns the string representation of a row in a table for a given set of headers."""
-        return to_table_line(self, headers)
-
-    def update(self, input_dictionary:  dict[str, None | float | int | str]) -> None:
-        """Updates a node based on a dictionary of attributes."""
-        for k, v in input_dictionary.items():
-            if v is None:
-                continue
-            if hasattr(self, '_NexusNode__' + k):
-                setattr(self, '_NexusNode__' + k, v)
-            elif hasattr(super(), '_Node__' + k):
-                setattr(self, '_Node__' + k, v)
+from __future__ import annotations
+from dataclasses import dataclass
+from typing import Optional
+
+from ResSimpy.Node import Node
+from ResSimpy.Utils import to_dict_generic
+from ResSimpy.Utils.generic_repr import generic_repr
+from ResSimpy.Utils.obj_to_table_string import to_table_line
+
+
+@dataclass(kw_only=True)
+class NexusNode(Node):
+    x_pos: Optional[float] = None
+    y_pos: Optional[float] = None
+    number: Optional[int] = None
+    temp: Optional[float] = None
+    station: Optional[str] = None
+
+    def __init__(self, properties_dict: dict[str, None | int | str | float]) -> None:
+        super().__init__()
+        for key, prop in properties_dict.items():
+            self.__setattr__(key, prop)
+
+    def __repr__(self) -> str:
+        return generic_repr(self)
+
+    @staticmethod
+    def get_nexus_mapping() -> dict[str, tuple[str, type]]:
+        """Gets the mapping of nexus keywords to attribute definitions."""
+        keywords = {
+            'NAME': ('name', str),
+            'TYPE': ('type', str),
+            'DEPTH': ('depth', float),
+            'TEMP': ('temp', float),
+            'X': ('x_pos', float),
+            'Y': ('y_pos', float),
+            'NUMBER': ('number', int),
+            'STATION': ('station', str),
+        }
+        return keywords
+
+    def to_dict(self, keys_in_nexus_style: bool = False, include_nones: bool = True) -> \
+            dict[str, None | str | int | float]:
+        """Returns a dictionary of the attributes of the Node.
+
+        Args:
+            keys_in_nexus_style (bool): if True returns the key values in Nexus keywords, otherwise returns the \
+                attribute name as stored by ressimpy.
+            include_nones (bool): If False filters the nones out of the dictionary. Defaults to True
+
+        Returns:
+            a dictionary keyed by attributes and values as the value of the attribute
+        """
+        result_dict = to_dict_generic.to_dict(self, keys_in_nexus_style, add_date=True, add_units=True,
+                                              include_nones=include_nones)
+        return result_dict
+
+    def to_table_line(self, headers: list[str]) -> str:
+        """Returns the string representation of a row in a table for a given set of headers."""
+        return to_table_line(self, headers)
+
+    def update(self, input_dictionary:  dict[str, None | float | int | str]) -> None:
+        """Updates a node based on a dictionary of attributes."""
+        for k, v in input_dictionary.items():
+            if v is None:
+                continue
+            if hasattr(self, '_NexusNode__' + k):
+                setattr(self, '_NexusNode__' + k, v)
+            elif hasattr(super(), '_Node__' + k):
+                setattr(self, '_Node__' + k, v)
```

### Comparing `ressimpy-1.0.0/ResSimpy/Nexus/DataModels/Network/NexusNodeConnection.py` & `ressimpy-1.0.1/ResSimpy/Nexus/DataModels/Network/NexusWellhead.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,115 +1,111 @@
-from __future__ import annotations
-from dataclasses import dataclass
-from typing import Optional
-from ResSimpy.Enums.UnitsEnum import UnitSystem
-from ResSimpy.NodeConnection import NodeConnection
-from ResSimpy.Utils import to_dict_generic
-from ResSimpy.Utils.generic_repr import generic_repr
-from ResSimpy.Utils.obj_to_table_string import to_table_line
-
-
-@dataclass
-class NexusNodeConnection(NodeConnection):
-    # TODO make list below comprehensive
-    """Attributes
-    hyd_method: hydraulic lift correlation method used (METHOD)
-    pvt_method: pvt method number (IPVT)
-    water_method: water method number (IWAT)
-    bat_method: bat method number (IBAT)
-    elevation_profile: elevation profile as a string (ELEVPR)
-    measured_depth_in: measured depth of the input node (MDIN)
-    measured_depth_out: measured depth of the output node (MDOUT)
-    diameter: diameter of the connecting pipe (DIAMETER)
-    inner_diameter: outer diameter of the pipe (INNERDIAM)
-    roughness: roughness of the pipe (ROUGHNESS)
-    heat_transfer_coeff: the heat transfer coefficient of the pipe (HTC)
-    temperature_profile: temperature profile used for the connection. (TEMPPR)
-    length: length of the connection (LENGTH)
-    delta_depth: change in depth between node_in and node_out (DDEPTH)
-    connection_number: used in place of name as a numbered connection (NUMBER)
-    seawater_profile: seawater profile used. (SEAWPR)
-    rate_mult: multiplier to the rate (RATEMULT)
-    polymer: whether polymer is a stream here (POLYMER)
-    dp_add: Additional delta pressure (DPADD).
-    """
-
-    hyd_method: Optional[str | int] = None
-    pvt_method: Optional[int] = None
-    bat_method: Optional[int] = None
-    water_method: Optional[int] = None
-    elevation_profile: Optional[str] = None
-    measured_depth_in: Optional[float] = None
-    measured_depth_out: Optional[float] = None
-    diameter: Optional[float] = None
-    inner_diameter: Optional[float] = None
-    roughness: Optional[float] = None
-    heat_transfer_coeff: Optional[float] = None
-    temperature_profile: Optional[float] = None
-    length: Optional[float] = None
-    delta_depth: Optional[float] = None
-    connection_number: Optional[int] = None
-    seawater_profile: Optional[str] = None
-    rate_mult: Optional[float] = None
-    polymer: Optional[str] = None
-    unit_system: Optional[UnitSystem] = None
-    dp_add: Optional[float] = None
-    dt_add: Optional[float] = None
-
-    def __init__(self, properties_dict: dict[str, None | int | str | float]) -> None:
-        super().__init__()
-        for key, prop in properties_dict.items():
-            self.__setattr__(key, prop)
-
-    def __repr__(self) -> str:
-        return generic_repr(self)
-
-    @staticmethod
-    def get_nexus_mapping() -> dict[str, tuple[str, type]]:
-        """Gets the mapping of nexus keywords to attribute definitions."""
-        nexus_mapping = {
-            'NAME': ('name', str),
-            'NODEIN': ('node_in', str),
-            'NODEOUT': ('node_out', str),
-            'TYPE': ('con_type', str),
-            'METHOD': ('hyd_method', str),
-            'IPVT': ('pvt_method', int),
-            'IWAT': ('water_method', int),
-            'IBAT': ('bat_method', int),
-            'ELEVPR': ('elevation_profile', str),
-            'MDIN': ('measured_depth_in', float),
-            'MDOUT': ('measured_depth_out', float),
-            'DIAM': ('diameter', float),
-            'INNERDIAM': ('inner_diameter', float),
-            'ROUGHNESS': ('roughness', float),
-            'HTC': ('heat_transfer_coeff', float),
-            'TEMPPR': ('temperature_profile', str),
-            'LENGTH': ('length', float),
-            'DDEPTH': ('delta_depth', float),
-            'NUMBER': ('connection_number', int),
-            'SEAWPR': ('seawater_profile', str),
-            'RATEMULT': ('rate_mult', float),
-            'POLYMER': ('polymer', str),
-            'DPADD': ('dp_add', float),
-            'DTADD': ('dt_add', float),
-            }
-        return nexus_mapping
-
-    def to_dict(self, keys_in_nexus_style: bool = False, include_nones: bool = True) -> \
-            dict[str, None | str | int | float]:
-        """Returns a dictionary of the attributes of the Connection.
-
-        Args:
-            keys_in_nexus_style (bool): if True returns the key values in Nexus keywords, otherwise returns the \
-                attribute name as stored by ressimpy.
-            include_nones (bool): If False filters the nones out of the dictionary. Defaults to True
-
-        Returns:
-            a dictionary keyed by attributes and values as the value of the attribute
-        """
-        result_dict = to_dict_generic.to_dict(self, keys_in_nexus_style, add_date=True, add_units=True,
-                                              include_nones=include_nones)
-        return result_dict
-
-    def to_table_line(self, headers: list[str]) -> str:
-        """Returns the string representation of a row in a table for a given set of headers."""
-        return to_table_line(self, headers)
+from dataclasses import dataclass
+from typing import Optional
+
+import ResSimpy.Utils.to_dict_generic as to_dict_generic
+from ResSimpy.Utils.generic_repr import generic_repr
+from ResSimpy.Wellhead import Wellhead
+
+
+@dataclass(kw_only=True)
+class NexusWellhead(Wellhead):
+    """Attributes
+    well (str):  Associates the wellhead to the well. (WELL)
+    name (str):  The name of the wellhead. (NAME)
+    type (str):  The type of well. (TYPE)
+    depth (float):  The depth of the wellhead  (DEPTH)
+    x_pos (float):  The x-coordinate location of the wellhead  (X)
+    y_pos (float):  The y-coordinate location of the wellhead  (Y)
+    pvt_method (int):  The PVT table numbers to be used for the well and wellhead connections. (IPVT)
+    water_method (int):  The Water PVT table numbers to be used for the well and wellhead connections. (IWAT)
+    bat_method (int):  The separator battery numbers associated with the well and wellhead connections. (IBAT)
+    measured_depth_in (float):  The measured depth at the start of the well interval  (MDIN)
+    measured_depth_out (float):  The measured depth at the end of the well interval  (MDOUT)
+    hyd_method (int):  The hydraulic method used. (METHOD)
+    number (int):  The well number. (NUMBER)
+    diameter (float):  The wellbore diameter  (DIAM)
+    inner_diameter (float):  The well inner diameter  (INNERDIAM)
+    roughness (float):  The well roughness. (ROUGHNESS)
+    length (float):  The length of the well  (LENGTH)
+    temperature (float):  The temperature of the fluid in the well  (TEMP)
+    elevation_profile (str):  The well elevation profile. (ELEVPR)
+    temperature_profile (str):  The well temperature profile. (TEMPPR)
+    dp_add (float):  The additional pressure drop across the well  (DPADD)
+    rate_mult (float):  The rate multiplier for the well. (RATEMULT)
+    delta_depth (float):  The depth difference between the two points in the connection  (DDEPTH)
+    heat_transfer_coeff (float):  The heat transfer coefficient for the well  (HTC)
+    dt_add (float):  The additional temperature difference across the well  (DTADD).
+
+    """
+
+    pvt_method: Optional[int] = None
+    water_method: Optional[int] = None
+    bat_method: Optional[int] = None
+    measured_depth_in: Optional[float] = None
+    measured_depth_out: Optional[float] = None
+    hyd_method: Optional[int] = None
+    number: Optional[int] = None
+    diameter: Optional[float] = None
+    inner_diameter: Optional[float] = None
+    roughness: Optional[float] = None
+    length: Optional[float] = None
+    temperature: Optional[float] = None
+    elevation_profile: Optional[str] = None
+    temperature_profile: Optional[str] = None
+    dp_add: Optional[float] = None
+    rate_mult: Optional[float] = None
+    delta_depth: Optional[float] = None
+    heat_transfer_coeff: Optional[float] = None
+    dt_add: Optional[float] = None
+
+    def __init__(self, properties_dict: dict[str, None | int | str | float]) -> None:
+        for key, prop in properties_dict.items():
+            self.__setattr__(key, prop)
+
+    @staticmethod
+    def get_nexus_mapping() -> dict[str, tuple[str, type]]:
+        """Gets the mapping of nexus keywords to attribute definitions."""
+        nexus_mapping = {
+            'WELL': ('well', str),
+            'NAME': ('name', str),
+            'TYPE': ('wellhead_type', str),
+            'DEPTH': ('depth', float),
+            'X': ('x_pos', float),
+            'Y': ('y_pos', float),
+            'IPVT': ('pvt_method', int),
+            'IWAT': ('water_method', int),
+            'IBAT': ('bat_method', int),
+            'MDIN': ('measured_depth_in', float),
+            'MDOUT': ('measured_depth_out', float),
+            'METHOD': ('hyd_method', int),
+            'NUMBER': ('number', int),
+            'DIAM': ('diameter', float),
+            'INNERDIAM': ('inner_diameter', float),
+            'ROUGHNESS': ('roughness', float),
+            'LENGTH': ('length', float),
+            'TEMP': ('temperature', float),
+            'ELEVPR': ('elevation_profile', str),
+            'TEMPPR': ('temperature_profile', str),
+            'DPADD': ('dp_add', float),
+            'RATEMULT': ('rate_mult', float),
+            'DDEPTH': ('delta_depth', float),
+            'HTC': ('heat_transfer_coeff', float),
+            'DTADD': ('dt_add', float),
+        }
+
+        return nexus_mapping
+
+    def to_dict(self, keys_in_nexus_style: bool = False) -> dict[str, None | str | int | float]:
+        """Returns a dictionary of the attributes of the well connection.
+
+        Args:
+            keys_in_nexus_style (bool): if True returns the key values in Nexus keywords, otherwise returns the \
+                attribute name as stored by ressimpy.
+
+        Returns:
+            a dictionary keyed by attributes and values as the value of the attribute
+        """
+        result_dict = to_dict_generic.to_dict(self, keys_in_nexus_style, add_date=True, add_units=True)
+        return result_dict
+
+    def __repr__(self) -> str:
+        return generic_repr(self)
```

### Comparing `ressimpy-1.0.0/ResSimpy/Nexus/DataModels/Network/NexusNodeConnections.py` & `ressimpy-1.0.1/ResSimpy/Nexus/DataModels/Network/NexusNodeConnections.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,150 +1,150 @@
-from __future__ import annotations
-from dataclasses import dataclass, field
-from uuid import UUID
-
-import pandas as pd
-from typing import Sequence, Optional, TYPE_CHECKING
-
-from ResSimpy.File import File
-from ResSimpy.Nexus.nexus_add_new_object_to_file import AddObjectOperations
-from ResSimpy.Nexus.nexus_collect_tables import collect_all_tables_to_objects
-
-from ResSimpy.Nexus.DataModels.Network.NexusNodeConnection import NexusNodeConnection
-from ResSimpy.Enums.UnitsEnum import UnitSystem
-from ResSimpy.Nexus.nexus_modify_object_in_file import ModifyObjectOperations
-from ResSimpy.Nexus.nexus_remove_object_from_file import RemoveObjectOperations
-from ResSimpy.NodeConnection import NodeConnection
-from ResSimpy.NodeConnections import NodeConnections
-from ResSimpy.Utils.obj_to_dataframe import obj_to_dataframe
-
-if TYPE_CHECKING:
-    from ResSimpy.Nexus.NexusNetwork import NexusNetwork
-
-
-@dataclass(kw_only=True)
-class NexusNodeConnections(NodeConnections):
-    __connections: list[NexusNodeConnection] = field(default_factory=list)
-
-    def __init__(self, parent_network: NexusNetwork) -> None:
-        self.__parent_network: NexusNetwork = parent_network
-        self.__connections: list[NexusNodeConnection] = []
-        self.__add_object_operations = AddObjectOperations(self.__parent_network.model, self.table_header,
-                                                           self.table_footer)
-        self.__remove_object_operations = RemoveObjectOperations(self.table_header, self.table_footer)
-        self.__modify_object_operations = ModifyObjectOperations(self)
-
-    @property
-    def table_header(self) -> str:
-        """Start of the Node definition table."""
-        return 'NODECON'
-
-    @property
-    def table_footer(self) -> str:
-        """End of the Node definition table."""
-        return 'END' + self.table_header
-
-    def get_all(self) -> Sequence[NexusNodeConnection]:
-        self.__parent_network.get_load_status()
-        return self.__connections
-
-    def get_by_name(self, connection_name: str) -> Optional[NodeConnection]:
-        self.__parent_network.get_load_status()
-        connections_to_return = filter(lambda x: False if x.name is None else x.name.upper() == connection_name.upper(),
-                                       self.__connections)
-        return next(connections_to_return, None)
-
-    def get_df(self) -> pd.DataFrame:
-        """Creates a dataframe representing all processed node connection data in a surface file
-        Returns:
-            DataFrame: of the properties of the connections through time with each row representing a node.
-        """
-        self.__parent_network.get_load_status()
-        return obj_to_dataframe(self.__connections)
-
-    def get_overview(self) -> str:
-        raise NotImplementedError('To be implemented')
-
-    def load(self, surface_file: File, start_date: str, default_units: UnitSystem) -> None:
-        """Calls load connections and appends the list of discovered NodeConnections into the NexusNodeConnection \
-            object.
-        """
-        new_connections = collect_all_tables_to_objects(surface_file, {self.table_header: NexusNodeConnection},
-                                                        start_date=start_date, default_units=default_units)
-        cons_list = new_connections.get(self.table_header)
-        if isinstance(cons_list, dict):
-            raise ValueError(
-                'Incompatible data format for additional nodecons. Expected type "list" instead got "dict"')
-        self._add_to_memory(cons_list)
-
-    def _add_to_memory(self, additional_list: Optional[Sequence[NexusNodeConnection]]):
-        """Extends the nodes object by a list of nodes provided to it.
-
-        Args:
-            additional_list (Sequence[NexusNodeConnection]): list of connections to add to the connection list.
-        """
-        if additional_list is None:
-            return
-        self.__connections.extend(additional_list)
-
-    def add(self, connection_to_add: dict[str, None | str | float | int]) -> None:
-        """Adds a nodeconnection to a network, taking a dictionary with properties for the new node.
-
-        Args:
-            connection_to_add (dict[str, None | str | float | int]): dictionary taking all the properties for the
-            new node connections. Requires date and a node name.
-        """
-        self.__parent_network.get_load_status()
-        name, date = self.__add_object_operations.check_name_date(connection_to_add)
-
-        new_object = NexusNodeConnection(connection_to_add)
-
-        self._add_to_memory([new_object])
-
-        file_to_add_to = self.__parent_network.get_network_file()
-
-        file_as_list = file_to_add_to.get_flat_list_str_file
-        if file_as_list is None:
-            raise ValueError(f'No file content found in the surface file specified at {file_to_add_to.location}')
-
-        self.__add_object_operations.add_object_to_file(date, file_as_list, file_to_add_to, new_object,
-                                                        connection_to_add)
-
-    def remove(self, connection_to_remove: UUID | dict[str, None | str | float | int]) -> None:
-        """Remove a connection from the network based on the properties matching a dictionary or id.
-
-        Args:
-            connection_to_remove (UUID | dict[str, None | str | float | int]): UUID of the connection to remove
-            or a dictionary with sufficient matching parameters to uniquely identify a node.
-        """
-        self.__parent_network.get_load_status()
-
-        network_file = self.__parent_network.get_network_file()
-
-        if isinstance(connection_to_remove, dict):
-            name = connection_to_remove.get('name', None)
-            if name is None:
-                raise ValueError(f'Require connection name to remove the connection instead got {name=}')
-            name = str(name)
-            network_element = self.__parent_network.find_network_element_with_dict(name, connection_to_remove,
-                                                                                   self._network_element_name)
-            network_element_id = network_element.id
-        else:
-            network_element_id = connection_to_remove
-
-        self.__remove_object_operations.remove_object_by_id(network_file, network_element_id, self.__connections)
-
-    def modify(self, connection_to_modify: dict[str, None | str | float | int],
-               new_properties: dict[str, None | str | float | int]) -> None:
-        """Modifies an existing connection based on a matching dictionary of properties (partial matches allowed if
-        precisely 1 matching connection is found).
-        Updates the properties with properties in the new_properties dictionary.
-
-        Args:
-            connection_to_modify (dict[str, None | str | float | int]): dictionary containing attributes to match in the
-            existing connection set.
-            new_properties (dict[str, None | str | float | int]): properties to switch to in the new connection
-        """
-        self.__parent_network.get_load_status()
-
-        self.__modify_object_operations.modify_network_object(connection_to_modify, new_properties,
-                                                              self.__parent_network)
+from __future__ import annotations
+from dataclasses import dataclass, field
+from uuid import UUID
+
+import pandas as pd
+from typing import Sequence, Optional, TYPE_CHECKING
+
+from ResSimpy.File import File
+from ResSimpy.Nexus.nexus_add_new_object_to_file import AddObjectOperations
+from ResSimpy.Nexus.nexus_collect_tables import collect_all_tables_to_objects
+
+from ResSimpy.Nexus.DataModels.Network.NexusNodeConnection import NexusNodeConnection
+from ResSimpy.Enums.UnitsEnum import UnitSystem
+from ResSimpy.Nexus.nexus_modify_object_in_file import ModifyObjectOperations
+from ResSimpy.Nexus.nexus_remove_object_from_file import RemoveObjectOperations
+from ResSimpy.NodeConnection import NodeConnection
+from ResSimpy.NodeConnections import NodeConnections
+from ResSimpy.Utils.obj_to_dataframe import obj_to_dataframe
+
+if TYPE_CHECKING:
+    from ResSimpy.Nexus.NexusNetwork import NexusNetwork
+
+
+@dataclass(kw_only=True)
+class NexusNodeConnections(NodeConnections):
+    __connections: list[NexusNodeConnection] = field(default_factory=list)
+
+    def __init__(self, parent_network: NexusNetwork) -> None:
+        self.__parent_network: NexusNetwork = parent_network
+        self.__connections: list[NexusNodeConnection] = []
+        self.__add_object_operations = AddObjectOperations(self.__parent_network.model, self.table_header,
+                                                           self.table_footer)
+        self.__remove_object_operations = RemoveObjectOperations(self.table_header, self.table_footer)
+        self.__modify_object_operations = ModifyObjectOperations(self)
+
+    @property
+    def table_header(self) -> str:
+        """Start of the Node definition table."""
+        return 'NODECON'
+
+    @property
+    def table_footer(self) -> str:
+        """End of the Node definition table."""
+        return 'END' + self.table_header
+
+    def get_all(self) -> Sequence[NexusNodeConnection]:
+        self.__parent_network.get_load_status()
+        return self.__connections
+
+    def get_by_name(self, connection_name: str) -> Optional[NodeConnection]:
+        self.__parent_network.get_load_status()
+        connections_to_return = filter(lambda x: False if x.name is None else x.name.upper() == connection_name.upper(),
+                                       self.__connections)
+        return next(connections_to_return, None)
+
+    def get_df(self) -> pd.DataFrame:
+        """Creates a dataframe representing all processed node connection data in a surface file
+        Returns:
+            DataFrame: of the properties of the connections through time with each row representing a node.
+        """
+        self.__parent_network.get_load_status()
+        return obj_to_dataframe(self.__connections)
+
+    def get_overview(self) -> str:
+        raise NotImplementedError('To be implemented')
+
+    def load(self, surface_file: File, start_date: str, default_units: UnitSystem) -> None:
+        """Calls load connections and appends the list of discovered NodeConnections into the NexusNodeConnection \
+            object.
+        """
+        new_connections = collect_all_tables_to_objects(surface_file, {self.table_header: NexusNodeConnection},
+                                                        start_date=start_date, default_units=default_units)
+        cons_list = new_connections.get(self.table_header)
+        if isinstance(cons_list, dict):
+            raise ValueError(
+                'Incompatible data format for additional nodecons. Expected type "list" instead got "dict"')
+        self._add_to_memory(cons_list)
+
+    def _add_to_memory(self, additional_list: Optional[Sequence[NexusNodeConnection]]):
+        """Extends the nodes object by a list of nodes provided to it.
+
+        Args:
+            additional_list (Sequence[NexusNodeConnection]): list of connections to add to the connection list.
+        """
+        if additional_list is None:
+            return
+        self.__connections.extend(additional_list)
+
+    def add(self, connection_to_add: dict[str, None | str | float | int]) -> None:
+        """Adds a nodeconnection to a network, taking a dictionary with properties for the new node.
+
+        Args:
+            connection_to_add (dict[str, None | str | float | int]): dictionary taking all the properties for the
+            new node connections. Requires date and a node name.
+        """
+        self.__parent_network.get_load_status()
+        name, date = self.__add_object_operations.check_name_date(connection_to_add)
+
+        new_object = NexusNodeConnection(connection_to_add)
+
+        self._add_to_memory([new_object])
+
+        file_to_add_to = self.__parent_network.get_network_file()
+
+        file_as_list = file_to_add_to.get_flat_list_str_file
+        if file_as_list is None:
+            raise ValueError(f'No file content found in the surface file specified at {file_to_add_to.location}')
+
+        self.__add_object_operations.add_object_to_file(date, file_as_list, file_to_add_to, new_object,
+                                                        connection_to_add)
+
+    def remove(self, connection_to_remove: UUID | dict[str, None | str | float | int]) -> None:
+        """Remove a connection from the network based on the properties matching a dictionary or id.
+
+        Args:
+            connection_to_remove (UUID | dict[str, None | str | float | int]): UUID of the connection to remove
+            or a dictionary with sufficient matching parameters to uniquely identify a node.
+        """
+        self.__parent_network.get_load_status()
+
+        network_file = self.__parent_network.get_network_file()
+
+        if isinstance(connection_to_remove, dict):
+            name = connection_to_remove.get('name', None)
+            if name is None:
+                raise ValueError(f'Require connection name to remove the connection instead got {name=}')
+            name = str(name)
+            network_element = self.__parent_network.find_network_element_with_dict(name, connection_to_remove,
+                                                                                   self._network_element_name)
+            network_element_id = network_element.id
+        else:
+            network_element_id = connection_to_remove
+
+        self.__remove_object_operations.remove_object_by_id(network_file, network_element_id, self.__connections)
+
+    def modify(self, connection_to_modify: dict[str, None | str | float | int],
+               new_properties: dict[str, None | str | float | int]) -> None:
+        """Modifies an existing connection based on a matching dictionary of properties (partial matches allowed if
+        precisely 1 matching connection is found).
+        Updates the properties with properties in the new_properties dictionary.
+
+        Args:
+            connection_to_modify (dict[str, None | str | float | int]): dictionary containing attributes to match in the
+            existing connection set.
+            new_properties (dict[str, None | str | float | int]): properties to switch to in the new connection
+        """
+        self.__parent_network.get_load_status()
+
+        self.__modify_object_operations.modify_network_object(connection_to_modify, new_properties,
+                                                              self.__parent_network)
```

### Comparing `ressimpy-1.0.0/ResSimpy/Nexus/DataModels/Network/NexusNodes.py` & `ressimpy-1.0.1/ResSimpy/Nexus/DataModels/Network/NexusNodes.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,171 +1,171 @@
-from __future__ import annotations
-from dataclasses import dataclass, field
-from uuid import UUID
-from typing import Sequence, Optional, TYPE_CHECKING
-
-import pandas as pd
-
-from ResSimpy.File import File
-from ResSimpy.Nexus.nexus_add_new_object_to_file import AddObjectOperations
-from ResSimpy.Nexus.nexus_collect_tables import collect_all_tables_to_objects
-from ResSimpy.Nexus.DataModels.Network.NexusNode import NexusNode
-from ResSimpy.Enums.UnitsEnum import UnitSystem
-from ResSimpy.Nexus.nexus_modify_object_in_file import ModifyObjectOperations
-from ResSimpy.Nexus.nexus_remove_object_from_file import RemoveObjectOperations
-from ResSimpy.Nodes import Nodes
-from ResSimpy.Utils.obj_to_dataframe import obj_to_dataframe
-
-if TYPE_CHECKING:
-    from ResSimpy.Nexus.NexusNetwork import NexusNetwork
-
-
-@dataclass(kw_only=True)
-class NexusNodes(Nodes):
-    __nodes: list[NexusNode] = field(default_factory=list)
-
-    def __init__(self, parent_network: NexusNetwork) -> None:
-        self.__parent_network: NexusNetwork = parent_network
-        self.__nodes: list[NexusNode] = []
-        self.__add_object_operations = AddObjectOperations(self.__parent_network.model, self.table_header,
-                                                           self.table_footer)
-        self.__remove_object_operations = RemoveObjectOperations(self.table_header, self.table_footer)
-        self.__modify_object_operations = ModifyObjectOperations(self)
-
-    @property
-    def table_header(self) -> str:
-        """Start of the Node definition table."""
-        return 'NODES'
-
-    @property
-    def table_footer(self) -> str:
-        """End of the Node definition table."""
-        return 'ENDNODES'
-
-    def get_all(self) -> Sequence[NexusNode]:
-        """Returns a list of nodes loaded from the simulator."""
-        self.__parent_network.get_load_status()
-        return self.__nodes
-
-    def get_by_name(self, node_name: str) -> Optional[NexusNode]:
-        """Returns a single node with the provided name loaded from the simulator.
-
-        Args:
-        ----
-            node_name (str): name of the requested node
-
-        Returns:
-        -------
-            NexusNode: which has the same name as the requested node_name
-
-        """
-        nodes_to_return = filter(lambda x: False if x.name is None else x.name.upper() == node_name.upper(),
-                                 self.__nodes)
-        return next(nodes_to_return, None)
-
-    def get_df(self) -> pd.DataFrame:
-        """Creates a dataframe representing all processed node data in a surface file
-        Returns:
-            DataFrame: of the properties of the nodes through time with each row representing a node.
-        """
-        df_store = obj_to_dataframe(self.__nodes)
-        return df_store
-
-    def get_overview(self) -> str:
-        raise NotImplementedError('To be implemented')
-
-    def load(self, surface_file: File, start_date: str, default_units: UnitSystem) -> None:
-        """Calls load nodes and appends the list of discovered nodes into the NexusNodes object.
-
-        Args:
-            surface_file (File): NexusFile representation of the surface file.
-            start_date (str): Starting date of the run
-            default_units (UnitSystem): Units used in case not specified by surface file.
-
-        Raises:
-            TypeError: if the unit system found in the property check is not a valid enum UnitSystem.
-
-        """
-        new_nodes = collect_all_tables_to_objects(surface_file, {'NODES': NexusNode},
-                                                  start_date=start_date,
-                                                  default_units=default_units)
-        cons_list = new_nodes.get('NODES')
-        if isinstance(cons_list, dict):
-            raise ValueError('Incompatible data format for additional wells. Expected type "list" instead got "dict"')
-        self._add_to_memory(cons_list)
-
-    def _add_to_memory(self, additional_list: Optional[list[NexusNode]]) -> None:
-        """Extends the nodes object by a list of nodes provided to it.
-
-        Args:
-        ----
-            additional_list (Sequence[NexusNode]): list of nexus nodes to add to the nodes list.
-
-        Returns:
-        -------
-            None
-        """
-        if additional_list is None:
-            return
-        self.__nodes.extend(additional_list)
-
-    def remove(self, node_to_remove: dict[str, None | str | float | int] | UUID) -> None:
-        """Remove a node from the network based on the properties matching a dictionary or id.
-
-        Args:
-            node_to_remove (UUID | dict[str, None | str | float | int]): UUID of the node to remove or a dictionary \
-            with sufficient matching parameters to uniquely identify a node
-
-        """
-        self.__parent_network.get_load_status()
-
-        network_file = self.__parent_network.get_network_file()
-
-        if isinstance(node_to_remove, dict):
-            name = node_to_remove.get('name', None)
-            if name is None:
-                raise ValueError(f'Require node name to remove the node instead got {name=}')
-            name = str(name)
-            node = self.__parent_network.find_network_element_with_dict(name, node_to_remove,
-                                                                        self._network_element_name)
-            node_id = node.id
-        else:
-            node_id = node_to_remove
-
-        self.__remove_object_operations.remove_object_by_id(network_file, node_id, self.__nodes)
-
-    def add(self, node_to_add: dict[str, None | str | float | int]) -> None:
-        """Adds a node to a network, taking a dictionary with properties for the new node.
-
-        Args:
-            node_to_add (dict[str, None | str | float | int]): dictionary taking all the properties for the new node.
-            Requires date and a node name.
-        """
-        self.__parent_network.get_load_status()
-        name, date = self.__add_object_operations.check_name_date(node_to_add)
-
-        new_object = NexusNode(node_to_add)
-
-        self._add_to_memory([new_object])
-
-        file_to_add_to = self.__parent_network.get_network_file()
-
-        file_as_list = file_to_add_to.get_flat_list_str_file
-        if file_as_list is None:
-            raise ValueError(f'No file content found in the surface file specified at {file_to_add_to.location}')
-
-        self.__add_object_operations.add_object_to_file(date, file_as_list, file_to_add_to, new_object, node_to_add)
-
-    def modify(self, node_to_modify: dict[str, None | str | float | int],
-               new_properties: dict[str, None | str | float | int]) -> None:
-        """Modifies an existing node based on a matching dictionary of properties (partial matches allowed if precisely
-         1 matching node is found). Updates the properties with properties in the new_properties dictionary.
-
-        Args:
-            node_to_modify (dict[str, None | str | float | int]): dictionary containing attributes to match in the
-            existing node set.
-            new_properties (dict[str, None | str | float | int]): properties to switch to in the new node
-        """
-        self.__parent_network.get_load_status()
-
-        self.__modify_object_operations.modify_network_object(node_to_modify, new_properties,
-                                                              self.__parent_network)
+from __future__ import annotations
+from dataclasses import dataclass, field
+from uuid import UUID
+from typing import Sequence, Optional, TYPE_CHECKING
+
+import pandas as pd
+
+from ResSimpy.File import File
+from ResSimpy.Nexus.nexus_add_new_object_to_file import AddObjectOperations
+from ResSimpy.Nexus.nexus_collect_tables import collect_all_tables_to_objects
+from ResSimpy.Nexus.DataModels.Network.NexusNode import NexusNode
+from ResSimpy.Enums.UnitsEnum import UnitSystem
+from ResSimpy.Nexus.nexus_modify_object_in_file import ModifyObjectOperations
+from ResSimpy.Nexus.nexus_remove_object_from_file import RemoveObjectOperations
+from ResSimpy.Nodes import Nodes
+from ResSimpy.Utils.obj_to_dataframe import obj_to_dataframe
+
+if TYPE_CHECKING:
+    from ResSimpy.Nexus.NexusNetwork import NexusNetwork
+
+
+@dataclass(kw_only=True)
+class NexusNodes(Nodes):
+    __nodes: list[NexusNode] = field(default_factory=list)
+
+    def __init__(self, parent_network: NexusNetwork) -> None:
+        self.__parent_network: NexusNetwork = parent_network
+        self.__nodes: list[NexusNode] = []
+        self.__add_object_operations = AddObjectOperations(self.__parent_network.model, self.table_header,
+                                                           self.table_footer)
+        self.__remove_object_operations = RemoveObjectOperations(self.table_header, self.table_footer)
+        self.__modify_object_operations = ModifyObjectOperations(self)
+
+    @property
+    def table_header(self) -> str:
+        """Start of the Node definition table."""
+        return 'NODES'
+
+    @property
+    def table_footer(self) -> str:
+        """End of the Node definition table."""
+        return 'ENDNODES'
+
+    def get_all(self) -> Sequence[NexusNode]:
+        """Returns a list of nodes loaded from the simulator."""
+        self.__parent_network.get_load_status()
+        return self.__nodes
+
+    def get_by_name(self, node_name: str) -> Optional[NexusNode]:
+        """Returns a single node with the provided name loaded from the simulator.
+
+        Args:
+        ----
+            node_name (str): name of the requested node
+
+        Returns:
+        -------
+            NexusNode: which has the same name as the requested node_name
+
+        """
+        nodes_to_return = filter(lambda x: False if x.name is None else x.name.upper() == node_name.upper(),
+                                 self.__nodes)
+        return next(nodes_to_return, None)
+
+    def get_df(self) -> pd.DataFrame:
+        """Creates a dataframe representing all processed node data in a surface file
+        Returns:
+            DataFrame: of the properties of the nodes through time with each row representing a node.
+        """
+        df_store = obj_to_dataframe(self.__nodes)
+        return df_store
+
+    def get_overview(self) -> str:
+        raise NotImplementedError('To be implemented')
+
+    def load(self, surface_file: File, start_date: str, default_units: UnitSystem) -> None:
+        """Calls load nodes and appends the list of discovered nodes into the NexusNodes object.
+
+        Args:
+            surface_file (File): NexusFile representation of the surface file.
+            start_date (str): Starting date of the run
+            default_units (UnitSystem): Units used in case not specified by surface file.
+
+        Raises:
+            TypeError: if the unit system found in the property check is not a valid enum UnitSystem.
+
+        """
+        new_nodes = collect_all_tables_to_objects(surface_file, {'NODES': NexusNode},
+                                                  start_date=start_date,
+                                                  default_units=default_units)
+        cons_list = new_nodes.get('NODES')
+        if isinstance(cons_list, dict):
+            raise ValueError('Incompatible data format for additional wells. Expected type "list" instead got "dict"')
+        self._add_to_memory(cons_list)
+
+    def _add_to_memory(self, additional_list: Optional[list[NexusNode]]) -> None:
+        """Extends the nodes object by a list of nodes provided to it.
+
+        Args:
+        ----
+            additional_list (Sequence[NexusNode]): list of nexus nodes to add to the nodes list.
+
+        Returns:
+        -------
+            None
+        """
+        if additional_list is None:
+            return
+        self.__nodes.extend(additional_list)
+
+    def remove(self, node_to_remove: dict[str, None | str | float | int] | UUID) -> None:
+        """Remove a node from the network based on the properties matching a dictionary or id.
+
+        Args:
+            node_to_remove (UUID | dict[str, None | str | float | int]): UUID of the node to remove or a dictionary \
+            with sufficient matching parameters to uniquely identify a node
+
+        """
+        self.__parent_network.get_load_status()
+
+        network_file = self.__parent_network.get_network_file()
+
+        if isinstance(node_to_remove, dict):
+            name = node_to_remove.get('name', None)
+            if name is None:
+                raise ValueError(f'Require node name to remove the node instead got {name=}')
+            name = str(name)
+            node = self.__parent_network.find_network_element_with_dict(name, node_to_remove,
+                                                                        self._network_element_name)
+            node_id = node.id
+        else:
+            node_id = node_to_remove
+
+        self.__remove_object_operations.remove_object_by_id(network_file, node_id, self.__nodes)
+
+    def add(self, node_to_add: dict[str, None | str | float | int]) -> None:
+        """Adds a node to a network, taking a dictionary with properties for the new node.
+
+        Args:
+            node_to_add (dict[str, None | str | float | int]): dictionary taking all the properties for the new node.
+            Requires date and a node name.
+        """
+        self.__parent_network.get_load_status()
+        name, date = self.__add_object_operations.check_name_date(node_to_add)
+
+        new_object = NexusNode(node_to_add)
+
+        self._add_to_memory([new_object])
+
+        file_to_add_to = self.__parent_network.get_network_file()
+
+        file_as_list = file_to_add_to.get_flat_list_str_file
+        if file_as_list is None:
+            raise ValueError(f'No file content found in the surface file specified at {file_to_add_to.location}')
+
+        self.__add_object_operations.add_object_to_file(date, file_as_list, file_to_add_to, new_object, node_to_add)
+
+    def modify(self, node_to_modify: dict[str, None | str | float | int],
+               new_properties: dict[str, None | str | float | int]) -> None:
+        """Modifies an existing node based on a matching dictionary of properties (partial matches allowed if precisely
+         1 matching node is found). Updates the properties with properties in the new_properties dictionary.
+
+        Args:
+            node_to_modify (dict[str, None | str | float | int]): dictionary containing attributes to match in the
+            existing node set.
+            new_properties (dict[str, None | str | float | int]): properties to switch to in the new node
+        """
+        self.__parent_network.get_load_status()
+
+        self.__modify_object_operations.modify_network_object(node_to_modify, new_properties,
+                                                              self.__parent_network)
```

### Comparing `ressimpy-1.0.0/ResSimpy/Nexus/DataModels/Network/NexusWellbore.py` & `ressimpy-1.0.1/ResSimpy/Nexus/DataModels/Network/NexusWellbore.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,78 +1,78 @@
-from dataclasses import dataclass
-from typing import Optional
-
-import ResSimpy.Utils.to_dict_generic as to_dict_generic
-from ResSimpy.Utils.generic_repr import generic_repr
-from ResSimpy.Wellbore import Wellbore
-
-
-@dataclass(kw_only=True)
-class NexusWellbore(Wellbore):
-    """Attributes
-    date (str): string representation of the last defined date
-    unit_system (UnitSystem): unit system enum
-    name (str): Name of the well. (WELL)
-    flowsect (int): Number of the flow section. (FLOWSECT)
-    diameter (float): Diameter of the well. (DIAM)
-    inner_diameter (float): Inner diameter of the well. (INNERDIAM)
-    roughness (float): Roughness of the well. (ROUGHNESS)
-    bore_type (str): Type of well. (TYPE)
-    hyd_method (str): hydraulic method. (METHOD)
-    temperature (float): Temperature of the well. (TEMP)
-    elevation_profile (str): Elevation profile of the well. (ELEVPR)
-    temperature_profile (str): Temperature profile of the well. (TEMPPR)
-    heat_transfer_coeff (float): Heat transfer coefficient of the well. (HTC)
-    pvt_method (int): Method number used for PVT. (IPVT)
-    water_method (int): Method number used for water. (IWAT).
-    """
-
-    flowsect: Optional[int] = None
-    bore_type: Optional[str] = None
-    hyd_method: Optional[str] = None
-    temperature: Optional[float] = None
-    elevation_profile: Optional[str] = None
-    temperature_profile: Optional[str] = None
-    heat_transfer_coeff: Optional[float] = None
-    pvt_method: Optional[int] = None
-    water_method: Optional[int] = None
-
-    def __init__(self, properties_dict: dict[str, None | int | str | float]) -> None:
-        for key, prop in properties_dict.items():
-            self.__setattr__(key, prop)
-
-    @staticmethod
-    def get_nexus_mapping() -> dict[str, tuple[str, type]]:
-        """Gets the mapping of nexus keywords to attribute definitions."""
-        nexus_mapping = {
-            'WELL': ('name', str),
-            'FLOWSECT': ('flowsect', int),
-            'DIAM': ('diameter', float),
-            'INNERDIAM': ('inner_diameter', float),
-            'ROUGHNESS': ('roughness', float),
-            'TYPE': ('bore_type', str),
-            'METHOD': ('hyd_method', str),
-            'TEMP': ('temperature', float),
-            'ELEVPR': ('elevation_profile', str),
-            'TEMPPR': ('temperature_profile', str),
-            'HTC': ('heat_transfer_coeff', float),
-            'IPVT': ('pvt_method', int),
-            'IWAT': ('water_method', int)
-        }
-
-        return nexus_mapping
-
-    def to_dict(self, keys_in_nexus_style: bool = False) -> dict[str, None | str | int | float]:
-        """Returns a dictionary of the attributes of the wellbore.
-
-        Args:
-            keys_in_nexus_style (bool): if True returns the key values in Nexus keywords, otherwise returns the \
-                attribute name as stored by ressimpy.
-
-        Returns:
-            a dictionary keyed by attributes and values as the value of the attribute
-        """
-        result_dict = to_dict_generic.to_dict(self, keys_in_nexus_style, add_date=True, add_units=True)
-        return result_dict
-
-    def __repr__(self) -> str:
-        return generic_repr(self)
+from dataclasses import dataclass
+from typing import Optional
+
+import ResSimpy.Utils.to_dict_generic as to_dict_generic
+from ResSimpy.Utils.generic_repr import generic_repr
+from ResSimpy.Wellbore import Wellbore
+
+
+@dataclass(kw_only=True)
+class NexusWellbore(Wellbore):
+    """Attributes
+    date (str): string representation of the last defined date
+    unit_system (UnitSystem): unit system enum
+    name (str): Name of the well. (WELL)
+    flowsect (int): Number of the flow section. (FLOWSECT)
+    diameter (float): Diameter of the well. (DIAM)
+    inner_diameter (float): Inner diameter of the well. (INNERDIAM)
+    roughness (float): Roughness of the well. (ROUGHNESS)
+    bore_type (str): Type of well. (TYPE)
+    hyd_method (str): hydraulic method. (METHOD)
+    temperature (float): Temperature of the well. (TEMP)
+    elevation_profile (str): Elevation profile of the well. (ELEVPR)
+    temperature_profile (str): Temperature profile of the well. (TEMPPR)
+    heat_transfer_coeff (float): Heat transfer coefficient of the well. (HTC)
+    pvt_method (int): Method number used for PVT. (IPVT)
+    water_method (int): Method number used for water. (IWAT).
+    """
+
+    flowsect: Optional[int] = None
+    bore_type: Optional[str] = None
+    hyd_method: Optional[str] = None
+    temperature: Optional[float] = None
+    elevation_profile: Optional[str] = None
+    temperature_profile: Optional[str] = None
+    heat_transfer_coeff: Optional[float] = None
+    pvt_method: Optional[int] = None
+    water_method: Optional[int] = None
+
+    def __init__(self, properties_dict: dict[str, None | int | str | float]) -> None:
+        for key, prop in properties_dict.items():
+            self.__setattr__(key, prop)
+
+    @staticmethod
+    def get_nexus_mapping() -> dict[str, tuple[str, type]]:
+        """Gets the mapping of nexus keywords to attribute definitions."""
+        nexus_mapping = {
+            'WELL': ('name', str),
+            'FLOWSECT': ('flowsect', int),
+            'DIAM': ('diameter', float),
+            'INNERDIAM': ('inner_diameter', float),
+            'ROUGHNESS': ('roughness', float),
+            'TYPE': ('bore_type', str),
+            'METHOD': ('hyd_method', str),
+            'TEMP': ('temperature', float),
+            'ELEVPR': ('elevation_profile', str),
+            'TEMPPR': ('temperature_profile', str),
+            'HTC': ('heat_transfer_coeff', float),
+            'IPVT': ('pvt_method', int),
+            'IWAT': ('water_method', int)
+        }
+
+        return nexus_mapping
+
+    def to_dict(self, keys_in_nexus_style: bool = False) -> dict[str, None | str | int | float]:
+        """Returns a dictionary of the attributes of the wellbore.
+
+        Args:
+            keys_in_nexus_style (bool): if True returns the key values in Nexus keywords, otherwise returns the \
+                attribute name as stored by ressimpy.
+
+        Returns:
+            a dictionary keyed by attributes and values as the value of the attribute
+        """
+        result_dict = to_dict_generic.to_dict(self, keys_in_nexus_style, add_date=True, add_units=True)
+        return result_dict
+
+    def __repr__(self) -> str:
+        return generic_repr(self)
```

### Comparing `ressimpy-1.0.0/ResSimpy/Nexus/DataModels/Network/NexusWellbores.py` & `ressimpy-1.0.1/ResSimpy/Nexus/DataModels/Network/NexusWellbores.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,88 +1,88 @@
-from __future__ import annotations
-
-from dataclasses import field, dataclass
-from typing import Optional, TYPE_CHECKING
-from uuid import UUID
-
-import pandas as pd
-
-from ResSimpy.File import File
-from ResSimpy.Nexus.nexus_collect_tables import collect_all_tables_to_objects
-from ResSimpy.Nexus.DataModels.Network.NexusWellbore import NexusWellbore
-from ResSimpy.Enums.UnitsEnum import UnitSystem
-from ResSimpy.Utils.obj_to_dataframe import obj_to_dataframe
-from ResSimpy.Wellbores import Wellbores
-
-if TYPE_CHECKING:
-    from ResSimpy.Nexus.NexusNetwork import NexusNetwork
-
-
-@dataclass
-class NexusWellbores(Wellbores):
-    __wellbores: list[NexusWellbore] = field(default_factory=list)
-
-    def __init__(self, parent_network: NexusNetwork) -> None:
-        self.__parent_network: NexusNetwork = parent_network
-        self.__wellbores: list[NexusWellbore] = []
-
-    def get_all(self) -> list[NexusWellbore]:
-        """Returns a list of wellbores loaded from the simulator."""
-        self.__parent_network.get_load_status()
-        return self.__wellbores
-
-    def get_by_name(self, name: str) -> Optional[NexusWellbore]:
-        """Returns a single well connection with the provided name loaded from the simulator.
-
-        Args:
-            name (str): name of the requested well connection
-
-        Returns:
-            NexusWellbore: which has the same name as requested
-        """
-        to_return = filter(lambda x: False if x.name is None else x.name.upper() == name.upper(),
-                           self.__wellbores)
-        return next(to_return, None)
-
-    def get_df(self) -> pd.DataFrame:
-        return obj_to_dataframe(self.__wellbores)
-
-    def get_overview(self) -> str:
-        raise NotImplementedError('To be implemented')
-
-    def load(self, surface_file: File, start_date: str, default_units: UnitSystem) -> None:
-        new_wellbores = collect_all_tables_to_objects(surface_file, {'WELLBORE': NexusWellbore},
-                                                      start_date=start_date,
-                                                      default_units=default_units)
-        cons_list = new_wellbores.get('WELLBORE')
-        if isinstance(cons_list, dict):
-            raise ValueError('Incompatible data format for additional wells. Expected type "list" instead got "dict"')
-        self._add_to_memory(cons_list)
-
-    def _add_to_memory(self, additional_list: Optional[list[NexusWellbore]]) -> None:
-        """Extends the nodes object by a list of wellbores provided to it.
-
-        Args:
-        ----
-            additional_list (list[NexusWellbore]): list of nexus wellbores to add to the nodes list.
-        """
-        if additional_list is None:
-            return
-        self.__wellbores.extend(additional_list)
-
-    def add(self, obj_to_add: dict[str, None | str | float | int]) -> None:
-        raise NotImplementedError
-
-    def remove(self, obj_to_remove: UUID | dict[str, None | str | float | int]) -> None:
-        raise NotImplementedError
-
-    def modify(self, obj_to_modify: dict[str, None | str | float | int],
-               new_properties: dict[str, None | str | float | int]) -> None:
-        raise NotImplementedError
-
-    @property
-    def table_header(self) -> str:
-        return 'WELLBORE'
-
-    @property
-    def table_footer(self) -> str:
-        return 'END' + self.table_header
+from __future__ import annotations
+
+from dataclasses import field, dataclass
+from typing import Optional, TYPE_CHECKING
+from uuid import UUID
+
+import pandas as pd
+
+from ResSimpy.File import File
+from ResSimpy.Nexus.nexus_collect_tables import collect_all_tables_to_objects
+from ResSimpy.Nexus.DataModels.Network.NexusWellbore import NexusWellbore
+from ResSimpy.Enums.UnitsEnum import UnitSystem
+from ResSimpy.Utils.obj_to_dataframe import obj_to_dataframe
+from ResSimpy.Wellbores import Wellbores
+
+if TYPE_CHECKING:
+    from ResSimpy.Nexus.NexusNetwork import NexusNetwork
+
+
+@dataclass
+class NexusWellbores(Wellbores):
+    __wellbores: list[NexusWellbore] = field(default_factory=list)
+
+    def __init__(self, parent_network: NexusNetwork) -> None:
+        self.__parent_network: NexusNetwork = parent_network
+        self.__wellbores: list[NexusWellbore] = []
+
+    def get_all(self) -> list[NexusWellbore]:
+        """Returns a list of wellbores loaded from the simulator."""
+        self.__parent_network.get_load_status()
+        return self.__wellbores
+
+    def get_by_name(self, name: str) -> Optional[NexusWellbore]:
+        """Returns a single well connection with the provided name loaded from the simulator.
+
+        Args:
+            name (str): name of the requested well connection
+
+        Returns:
+            NexusWellbore: which has the same name as requested
+        """
+        to_return = filter(lambda x: False if x.name is None else x.name.upper() == name.upper(),
+                           self.__wellbores)
+        return next(to_return, None)
+
+    def get_df(self) -> pd.DataFrame:
+        return obj_to_dataframe(self.__wellbores)
+
+    def get_overview(self) -> str:
+        raise NotImplementedError('To be implemented')
+
+    def load(self, surface_file: File, start_date: str, default_units: UnitSystem) -> None:
+        new_wellbores = collect_all_tables_to_objects(surface_file, {'WELLBORE': NexusWellbore},
+                                                      start_date=start_date,
+                                                      default_units=default_units)
+        cons_list = new_wellbores.get('WELLBORE')
+        if isinstance(cons_list, dict):
+            raise ValueError('Incompatible data format for additional wells. Expected type "list" instead got "dict"')
+        self._add_to_memory(cons_list)
+
+    def _add_to_memory(self, additional_list: Optional[list[NexusWellbore]]) -> None:
+        """Extends the nodes object by a list of wellbores provided to it.
+
+        Args:
+        ----
+            additional_list (list[NexusWellbore]): list of nexus wellbores to add to the nodes list.
+        """
+        if additional_list is None:
+            return
+        self.__wellbores.extend(additional_list)
+
+    def add(self, obj_to_add: dict[str, None | str | float | int]) -> None:
+        raise NotImplementedError
+
+    def remove(self, obj_to_remove: UUID | dict[str, None | str | float | int]) -> None:
+        raise NotImplementedError
+
+    def modify(self, obj_to_modify: dict[str, None | str | float | int],
+               new_properties: dict[str, None | str | float | int]) -> None:
+        raise NotImplementedError
+
+    @property
+    def table_header(self) -> str:
+        return 'WELLBORE'
+
+    @property
+    def table_footer(self) -> str:
+        return 'END' + self.table_header
```

### Comparing `ressimpy-1.0.0/ResSimpy/Nexus/DataModels/Network/NexusWellConnection.py` & `ressimpy-1.0.1/ResSimpy/Nexus/DataModels/Network/NexusWellConnection.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,168 +1,168 @@
-from dataclasses import dataclass
-from typing import Optional
-import ResSimpy.Utils.to_dict_generic as to_dict_generic
-from ResSimpy.Utils.generic_repr import generic_repr
-from ResSimpy.WellConnection import WellConnection
-
-
-@dataclass(kw_only=True)
-class NexusWellConnection(WellConnection):
-    """Attributes
-    stream (str): COMMENT (STREAM)
-    number (int): COMMENT (NUMBER)
-    scale (float): COMMENT (SCALE)
-    bhdepth (float): COMMENT (BHDEPTH)
-    datum_depth (float): COMMENT (DATUM)
-    x_pos (float): COMMENT (X)
-    y_pos (float): COMMENT (Y)
-    gradient_calc (str): COMMENT (DATGRAD)
-    length (float): COMMENT (LENGTH)
-    bottomhole_measured_depth (float): COMMENT (BHMD)
-    add_tubing (int): COMMENT (ADDTUBING)
-    diameter (float): COMMENT (DIAM)
-    inner_diameter (float): COMMENT (INNERDIAM)
-    roughness (float): COMMENT (ROUGHNESS)
-    tracer (str): COMMENT (TRACERS)
-    con_type (str): COMMENT (TYPE)
-    hyd_method (str): COMMENT (METHOD)
-    pvt_method (int): COMMENT (IPVT)
-    water_method (int): COMMENT (IWAT)
-    bat_method (int): COMMENT (IBAT)
-    temperature (float): COMMENT (TEMP)
-    elevation_profile (str): COMMENT (ELEVPR)
-    temperature_profile (str): COMMENT (TEMPPR)
-    inj_mobility (str): COMMENT (INJMOB)
-    crossshut_method (str): COMMENT (CROSS_SHUT)
-    crossflow (str): COMMENT (CROSSFLOW)
-    on_time (float): COMMENT (ONTIME)
-    heat_transfer_coeff (float): COMMENT (HTC)
-    water_inj_mult (float): COMMENT (WIMULT)
-    productivity_index (float): COMMENT (PI)
-    vip_productivity_index (float): COMMENT (VIPPI)
-    productivity_index_phase (float): COMMENT (PIPHASE)
-    d_factor (float): COMMENT (D)
-    non_darcy_flow_model (str): COMMENT (ND)
-    non_darcy_flow_method (str): COMMENT (DPERF)
-    gas_mobility (float): COMMENT (GASMOB)
-    capillary_number_model (str): COMMENT (CN)
-    dp_add (float): COMMENT (DPADD)
-    dt_add (float): COMMENT (DTADD)
-    rate_mult (float): COMMENT (RATEMULT)
-    polymer (str): COMMENT (POLYMER)
-    station (str): COMMENT (STATION)
-    drill_queue (str): COMMENT (ASSCDR)
-    drill_order_benefit (float): COMMENT (BENEFIT).
-    """
-
-    bh_node_name: Optional[str] = None
-    wh_node_name: Optional[str] = None
-
-    stream: Optional[str] = None
-    number: Optional[int] = None
-    scale: Optional[float] = None
-    gradient_calc: Optional[str] = None
-    bottomhole_measured_depth: Optional[float] = None
-    add_tubing: Optional[int] = None
-    tracer: Optional[str] = None
-    con_type: Optional[str] = None
-    hyd_method: Optional[str] = None
-    pvt_method: Optional[int] = None
-    water_method: Optional[int] = None
-    bat_method: Optional[int] = None
-    elevation_profile: Optional[str] = None
-    temperature_profile: Optional[str] = None
-    inj_mobility: Optional[str] = None
-    crossshut_method: Optional[str] = None
-    crossflow: Optional[str] = None
-    on_time: Optional[float] = None
-    heat_transfer_coeff: Optional[float] = None
-    water_inj_mult: Optional[float] = None
-    vip_productivity_index: Optional[float] = None
-    productivity_index_phase: Optional[float] = None
-    d_factor: Optional[float] = None
-    non_darcy_flow_model: Optional[str] = None
-    non_darcy_flow_method: Optional[str] = None
-    gas_mobility: Optional[float] = None
-    capillary_number_model: Optional[str] = None
-    dp_add: Optional[float] = None
-    dt_add: Optional[float] = None
-    rate_mult: Optional[float] = None
-    polymer: Optional[str] = None
-    station: Optional[str] = None
-    drill_queue: Optional[str] = None
-    drill_order_benefit: Optional[float] = None
-
-    def __init__(self, properties_dict: dict[str, None | int | str | float]) -> None:
-        for key, prop in properties_dict.items():
-            self.__setattr__(key, prop)
-        if self.name is not None:
-            self.bh_node_name = self.name + '%bh'
-            self.wh_node_name = self.name + '%wh'
-
-    def __repr__(self) -> str:
-        return generic_repr(self)
-
-    @staticmethod
-    def get_nexus_mapping() -> dict[str, tuple[str, type]]:
-        """Gets the mapping of nexus keywords to attribute definitions."""
-        nexus_mapping = {
-            'NAME': ('name', str),
-            'STREAM': ('stream', str),
-            'NUMBER': ('number', int),
-            'SCALE': ('scale', float),
-            'BHDEPTH': ('bhdepth', float),
-            'DATUM': ('datum_depth', float),
-            'X': ('x_pos', float),
-            'Y': ('y_pos', float),
-            'DATGRAD': ('gradient_calc', str),
-            'LENGTH': ('length', float),
-            'BHMD': ('bottomhole_measured_depth', float),
-            'ADDTUBING': ('add_tubing', int),
-            'DIAM': ('diameter', float),
-            'INNERDIAM': ('inner_diameter', float),
-            'ROUGHNESS': ('roughness', float),
-            'TRACERS': ('tracer', str),
-            'TYPE': ('con_type', str),
-            'METHOD': ('hyd_method', str),
-            'IPVT': ('pvt_method', int),
-            'IWAT': ('water_method', int),
-            'IBAT': ('bat_method', int),
-            'TEMP': ('temperature', float),
-            'ELEVPR': ('elevation_profile', str),
-            'TEMPPR': ('temperature_profile', str),
-            'INJMOB': ('inj_mobility', str),
-            'CROSS_SHUT': ('crossshut_method', str),
-            'CROSSFLOW': ('crossflow', str),
-            'ONTIME': ('on_time', float),
-            'HTC': ('heat_transfer_coeff', float),
-            'WIMULT': ('water_inj_mult', float),
-            'PI': ('productivity_index', float),
-            'VIPPI': ('vip_productivity_index', float),
-            'PIPHASE': ('productivity_index_phase', str),
-            'D': ('d_factor', float),
-            'ND': ('non_darcy_flow_model', str),
-            'DPERF': ('non_darcy_flow_method', str),
-            'GASMOB': ('gas_mobility', float),
-            'CN': ('capillary_number_model', str),
-            'DPADD': ('dp_add', float),
-            'DTADD': ('dt_add', float),
-            'RATEMULT': ('rate_mult', float),
-            'POLYMER': ('polymer', str),
-            'STATION': ('station', str),
-            'ASSCDR': ('drill_queue', str),
-            'BENEFIT': ('drill_order_benefit', float),
-            }
-        return nexus_mapping
-
-    def to_dict(self, keys_in_nexus_style: bool = False) -> dict[str, None | str | int | float]:
-        """Returns a dictionary of the attributes of the well connection.
-
-        Args:
-            keys_in_nexus_style (bool): if True returns the key values in Nexus keywords, otherwise returns the \
-                attribute name as stored by ressimpy.
-
-        Returns:
-            a dictionary keyed by attributes and values as the value of the attribute
-        """
-        result_dict = to_dict_generic.to_dict(self, keys_in_nexus_style, add_date=True, add_units=True)
-        return result_dict
+from dataclasses import dataclass
+from typing import Optional
+import ResSimpy.Utils.to_dict_generic as to_dict_generic
+from ResSimpy.Utils.generic_repr import generic_repr
+from ResSimpy.WellConnection import WellConnection
+
+
+@dataclass(kw_only=True)
+class NexusWellConnection(WellConnection):
+    """Attributes
+    stream (str): COMMENT (STREAM)
+    number (int): COMMENT (NUMBER)
+    scale (float): COMMENT (SCALE)
+    bhdepth (float): COMMENT (BHDEPTH)
+    datum_depth (float): COMMENT (DATUM)
+    x_pos (float): COMMENT (X)
+    y_pos (float): COMMENT (Y)
+    gradient_calc (str): COMMENT (DATGRAD)
+    length (float): COMMENT (LENGTH)
+    bottomhole_measured_depth (float): COMMENT (BHMD)
+    add_tubing (int): COMMENT (ADDTUBING)
+    diameter (float): COMMENT (DIAM)
+    inner_diameter (float): COMMENT (INNERDIAM)
+    roughness (float): COMMENT (ROUGHNESS)
+    tracer (str): COMMENT (TRACERS)
+    con_type (str): COMMENT (TYPE)
+    hyd_method (str): COMMENT (METHOD)
+    pvt_method (int): COMMENT (IPVT)
+    water_method (int): COMMENT (IWAT)
+    bat_method (int): COMMENT (IBAT)
+    temperature (float): COMMENT (TEMP)
+    elevation_profile (str): COMMENT (ELEVPR)
+    temperature_profile (str): COMMENT (TEMPPR)
+    inj_mobility (str): COMMENT (INJMOB)
+    crossshut_method (str): COMMENT (CROSS_SHUT)
+    crossflow (str): COMMENT (CROSSFLOW)
+    on_time (float): COMMENT (ONTIME)
+    heat_transfer_coeff (float): COMMENT (HTC)
+    water_inj_mult (float): COMMENT (WIMULT)
+    productivity_index (float): COMMENT (PI)
+    vip_productivity_index (float): COMMENT (VIPPI)
+    productivity_index_phase (float): COMMENT (PIPHASE)
+    d_factor (float): COMMENT (D)
+    non_darcy_flow_model (str): COMMENT (ND)
+    non_darcy_flow_method (str): COMMENT (DPERF)
+    gas_mobility (float): COMMENT (GASMOB)
+    capillary_number_model (str): COMMENT (CN)
+    dp_add (float): COMMENT (DPADD)
+    dt_add (float): COMMENT (DTADD)
+    rate_mult (float): COMMENT (RATEMULT)
+    polymer (str): COMMENT (POLYMER)
+    station (str): COMMENT (STATION)
+    drill_queue (str): COMMENT (ASSCDR)
+    drill_order_benefit (float): COMMENT (BENEFIT).
+    """
+
+    bh_node_name: Optional[str] = None
+    wh_node_name: Optional[str] = None
+
+    stream: Optional[str] = None
+    number: Optional[int] = None
+    scale: Optional[float] = None
+    gradient_calc: Optional[str] = None
+    bottomhole_measured_depth: Optional[float] = None
+    add_tubing: Optional[int] = None
+    tracer: Optional[str] = None
+    con_type: Optional[str] = None
+    hyd_method: Optional[str] = None
+    pvt_method: Optional[int] = None
+    water_method: Optional[int] = None
+    bat_method: Optional[int] = None
+    elevation_profile: Optional[str] = None
+    temperature_profile: Optional[str] = None
+    inj_mobility: Optional[str] = None
+    crossshut_method: Optional[str] = None
+    crossflow: Optional[str] = None
+    on_time: Optional[float] = None
+    heat_transfer_coeff: Optional[float] = None
+    water_inj_mult: Optional[float] = None
+    vip_productivity_index: Optional[float] = None
+    productivity_index_phase: Optional[float] = None
+    d_factor: Optional[float] = None
+    non_darcy_flow_model: Optional[str] = None
+    non_darcy_flow_method: Optional[str] = None
+    gas_mobility: Optional[float] = None
+    capillary_number_model: Optional[str] = None
+    dp_add: Optional[float] = None
+    dt_add: Optional[float] = None
+    rate_mult: Optional[float] = None
+    polymer: Optional[str] = None
+    station: Optional[str] = None
+    drill_queue: Optional[str] = None
+    drill_order_benefit: Optional[float] = None
+
+    def __init__(self, properties_dict: dict[str, None | int | str | float]) -> None:
+        for key, prop in properties_dict.items():
+            self.__setattr__(key, prop)
+        if self.name is not None:
+            self.bh_node_name = self.name + '%bh'
+            self.wh_node_name = self.name + '%wh'
+
+    def __repr__(self) -> str:
+        return generic_repr(self)
+
+    @staticmethod
+    def get_nexus_mapping() -> dict[str, tuple[str, type]]:
+        """Gets the mapping of nexus keywords to attribute definitions."""
+        nexus_mapping = {
+            'NAME': ('name', str),
+            'STREAM': ('stream', str),
+            'NUMBER': ('number', int),
+            'SCALE': ('scale', float),
+            'BHDEPTH': ('bhdepth', float),
+            'DATUM': ('datum_depth', float),
+            'X': ('x_pos', float),
+            'Y': ('y_pos', float),
+            'DATGRAD': ('gradient_calc', str),
+            'LENGTH': ('length', float),
+            'BHMD': ('bottomhole_measured_depth', float),
+            'ADDTUBING': ('add_tubing', int),
+            'DIAM': ('diameter', float),
+            'INNERDIAM': ('inner_diameter', float),
+            'ROUGHNESS': ('roughness', float),
+            'TRACERS': ('tracer', str),
+            'TYPE': ('con_type', str),
+            'METHOD': ('hyd_method', str),
+            'IPVT': ('pvt_method', int),
+            'IWAT': ('water_method', int),
+            'IBAT': ('bat_method', int),
+            'TEMP': ('temperature', float),
+            'ELEVPR': ('elevation_profile', str),
+            'TEMPPR': ('temperature_profile', str),
+            'INJMOB': ('inj_mobility', str),
+            'CROSS_SHUT': ('crossshut_method', str),
+            'CROSSFLOW': ('crossflow', str),
+            'ONTIME': ('on_time', float),
+            'HTC': ('heat_transfer_coeff', float),
+            'WIMULT': ('water_inj_mult', float),
+            'PI': ('productivity_index', float),
+            'VIPPI': ('vip_productivity_index', float),
+            'PIPHASE': ('productivity_index_phase', str),
+            'D': ('d_factor', float),
+            'ND': ('non_darcy_flow_model', str),
+            'DPERF': ('non_darcy_flow_method', str),
+            'GASMOB': ('gas_mobility', float),
+            'CN': ('capillary_number_model', str),
+            'DPADD': ('dp_add', float),
+            'DTADD': ('dt_add', float),
+            'RATEMULT': ('rate_mult', float),
+            'POLYMER': ('polymer', str),
+            'STATION': ('station', str),
+            'ASSCDR': ('drill_queue', str),
+            'BENEFIT': ('drill_order_benefit', float),
+            }
+        return nexus_mapping
+
+    def to_dict(self, keys_in_nexus_style: bool = False) -> dict[str, None | str | int | float]:
+        """Returns a dictionary of the attributes of the well connection.
+
+        Args:
+            keys_in_nexus_style (bool): if True returns the key values in Nexus keywords, otherwise returns the \
+                attribute name as stored by ressimpy.
+
+        Returns:
+            a dictionary keyed by attributes and values as the value of the attribute
+        """
+        result_dict = to_dict_generic.to_dict(self, keys_in_nexus_style, add_date=True, add_units=True)
+        return result_dict
```

### Comparing `ressimpy-1.0.0/ResSimpy/Nexus/DataModels/Network/NexusWellConnections.py` & `ressimpy-1.0.1/ResSimpy/Nexus/DataModels/Network/NexusWellConnections.py`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,100 +1,100 @@
-from __future__ import annotations
-from dataclasses import dataclass, field
-from typing import Optional, TYPE_CHECKING
-from uuid import UUID
-
-import pandas as pd
-
-from ResSimpy.File import File
-from ResSimpy.Nexus.nexus_add_new_object_to_file import AddObjectOperations
-from ResSimpy.Nexus.nexus_modify_object_in_file import ModifyObjectOperations
-from ResSimpy.Nexus.nexus_remove_object_from_file import RemoveObjectOperations
-from ResSimpy.Utils.obj_to_dataframe import obj_to_dataframe
-from ResSimpy.Nexus.DataModels.Network.NexusWellConnection import NexusWellConnection
-from ResSimpy.Enums.UnitsEnum import UnitSystem
-from ResSimpy.Nexus.nexus_collect_tables import collect_all_tables_to_objects
-from ResSimpy.WellConnections import WellConnections
-
-if TYPE_CHECKING:
-    from ResSimpy.Nexus.NexusNetwork import NexusNetwork
-
-
-@dataclass
-class NexusWellConnections(WellConnections):
-    __well_connections: list[NexusWellConnection] = field(default_factory=list)
-
-    def __init__(self, parent_network: NexusNetwork) -> None:
-        self.__parent_network: NexusNetwork = parent_network
-        self.__well_connections: list[NexusWellConnection] = []
-        self.__add_object_operations = AddObjectOperations(self.__parent_network.model, self.table_header,
-                                                           self.table_footer)
-        self.__remove_object_operations = RemoveObjectOperations(self.table_header, self.table_footer)
-        self.__modify_object_operations = ModifyObjectOperations(self)
-
-    def get_all(self) -> list[NexusWellConnection]:
-        """Returns a list of well connections loaded from the simulator."""
-        self.__parent_network.get_load_status()
-        return self.__well_connections
-
-    def get_by_name(self, name: str) -> Optional[NexusWellConnection]:
-        """Returns a single well connection with the provided name loaded from the simulator.
-
-        Args:
-            name (str): name of the requested well connection
-
-        Returns:
-            NexusWellConnection: which has the same name as requested
-        """
-        self.__parent_network.get_load_status()
-        to_return = filter(lambda x: False if x.name is None else x.name.upper() == name.upper(),
-                           self.__well_connections)
-        return next(to_return, None)
-
-    def get_df(self) -> pd.DataFrame:
-        """Creates a dataframe representing all processed well connections data in a surface file
-        Returns:
-            DataFrame: of the properties of the well connections through time with each row representing a single well \
-            connection.
-        """
-        self.__parent_network.get_load_status()
-        return obj_to_dataframe(self.__well_connections)
-
-    def get_overview(self) -> str:
-        raise NotImplementedError('To be implemented')
-
-    def _add_to_memory(self, additional_list: Optional[list[NexusWellConnection]]) -> None:
-        """Extends the nodes object by a list of connections provided to it.
-
-        Args:
-            additional_list (Sequence[NexusWellConnection]): list of nexus connections to add to the nodes list.
-        """
-        if additional_list is None:
-            return
-        self.__well_connections.extend(additional_list)
-
-    def load(self, surface_file: File, start_date: str, default_units: UnitSystem) -> None:
-        new_well_connections = collect_all_tables_to_objects(surface_file, {'WELLS': NexusWellConnection},
-                                                             start_date=start_date,
-                                                             default_units=default_units)
-        cons_list = new_well_connections.get('WELLS')
-        if isinstance(cons_list, dict):
-            raise ValueError('Incompatible data format for additional wells. Expected type "list" instead got "dict"')
-        self._add_to_memory(cons_list)
-
-    def add(self, obj_to_add: dict[str, None | str | float | int]) -> None:
-        raise NotImplementedError
-
-    def remove(self, obj_to_remove: UUID | dict[str, None | str | float | int]) -> None:
-        raise NotImplementedError
-
-    def modify(self, obj_to_modify: dict[str, None | str | float | int],
-               new_properties: dict[str, None | str | float | int]) -> None:
-        raise NotImplementedError
-
-    @property
-    def table_header(self) -> str:
-        return 'WELLS'
-
-    @property
-    def table_footer(self) -> str:
-        return 'END' + self.table_header
+from __future__ import annotations
+from dataclasses import dataclass, field
+from typing import Optional, TYPE_CHECKING
+from uuid import UUID
+
+import pandas as pd
+
+from ResSimpy.File import File
+from ResSimpy.Nexus.nexus_add_new_object_to_file import AddObjectOperations
+from ResSimpy.Nexus.nexus_modify_object_in_file import ModifyObjectOperations
+from ResSimpy.Nexus.nexus_remove_object_from_file import RemoveObjectOperations
+from ResSimpy.Utils.obj_to_dataframe import obj_to_dataframe
+from ResSimpy.Nexus.DataModels.Network.NexusWellConnection import NexusWellConnection
+from ResSimpy.Enums.UnitsEnum import UnitSystem
+from ResSimpy.Nexus.nexus_collect_tables import collect_all_tables_to_objects
+from ResSimpy.WellConnections import WellConnections
+
+if TYPE_CHECKING:
+    from ResSimpy.Nexus.NexusNetwork import NexusNetwork
+
+
+@dataclass
+class NexusWellConnections(WellConnections):
+    __well_connections: list[NexusWellConnection] = field(default_factory=list)
+
+    def __init__(self, parent_network: NexusNetwork) -> None:
+        self.__parent_network: NexusNetwork = parent_network
+        self.__well_connections: list[NexusWellConnection] = []
+        self.__add_object_operations = AddObjectOperations(self.__parent_network.model, self.table_header,
+                                                           self.table_footer)
+        self.__remove_object_operations = RemoveObjectOperations(self.table_header, self.table_footer)
+        self.__modify_object_operations = ModifyObjectOperations(self)
+
+    def get_all(self) -> list[NexusWellConnection]:
+        """Returns a list of well connections loaded from the simulator."""
+        self.__parent_network.get_load_status()
+        return self.__well_connections
+
+    def get_by_name(self, name: str) -> Optional[NexusWellConnection]:
+        """Returns a single well connection with the provided name loaded from the simulator.
+
+        Args:
+            name (str): name of the requested well connection
+
+        Returns:
+            NexusWellConnection: which has the same name as requested
+        """
+        self.__parent_network.get_load_status()
+        to_return = filter(lambda x: False if x.name is None else x.name.upper() == name.upper(),
+                           self.__well_connections)
+        return next(to_return, None)
+
+    def get_df(self) -> pd.DataFrame:
+        """Creates a dataframe representing all processed well connections data in a surface file
+        Returns:
+            DataFrame: of the properties of the well connections through time with each row representing a single well \
+            connection.
+        """
+        self.__parent_network.get_load_status()
+        return obj_to_dataframe(self.__well_connections)
+
+    def get_overview(self) -> str:
+        raise NotImplementedError('To be implemented')
+
+    def _add_to_memory(self, additional_list: Optional[list[NexusWellConnection]]) -> None:
+        """Extends the nodes object by a list of connections provided to it.
+
+        Args:
+            additional_list (Sequence[NexusWellConnection]): list of nexus connections to add to the nodes list.
+        """
+        if additional_list is None:
+            return
+        self.__well_connections.extend(additional_list)
+
+    def load(self, surface_file: File, start_date: str, default_units: UnitSystem) -> None:
+        new_well_connections = collect_all_tables_to_objects(surface_file, {'WELLS': NexusWellConnection},
+                                                             start_date=start_date,
+                                                             default_units=default_units)
+        cons_list = new_well_connections.get('WELLS')
+        if isinstance(cons_list, dict):
+            raise ValueError('Incompatible data format for additional wells. Expected type "list" instead got "dict"')
+        self._add_to_memory(cons_list)
+
+    def add(self, obj_to_add: dict[str, None | str | float | int]) -> None:
+        raise NotImplementedError
+
+    def remove(self, obj_to_remove: UUID | dict[str, None | str | float | int]) -> None:
+        raise NotImplementedError
+
+    def modify(self, obj_to_modify: dict[str, None | str | float | int],
+               new_properties: dict[str, None | str | float | int]) -> None:
+        raise NotImplementedError
+
+    @property
+    def table_header(self) -> str:
+        return 'WELLS'
+
+    @property
+    def table_footer(self) -> str:
+        return 'END' + self.table_header
```

### Comparing `ressimpy-1.0.0/ResSimpy/Nexus/DataModels/Network/NexusWellheads.py` & `ressimpy-1.0.1/ResSimpy/Nexus/DataModels/Network/NexusWellheads.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,87 +1,87 @@
-from __future__ import annotations
-from dataclasses import dataclass, field
-from typing import Optional, TYPE_CHECKING
-from uuid import UUID
-
-import pandas as pd
-
-from ResSimpy.File import File
-from ResSimpy.Nexus.nexus_collect_tables import collect_all_tables_to_objects
-from ResSimpy.Nexus.DataModels.Network.NexusWellhead import NexusWellhead
-from ResSimpy.Enums.UnitsEnum import UnitSystem
-from ResSimpy.Utils.obj_to_dataframe import obj_to_dataframe
-from ResSimpy.Wellheads import Wellheads
-
-if TYPE_CHECKING:
-    from ResSimpy.Nexus.NexusNetwork import NexusNetwork
-
-
-@dataclass
-class NexusWellheads(Wellheads):
-    __wellheads: list[NexusWellhead] = field(default_factory=list)
-
-    def __init__(self, parent_network: NexusNetwork) -> None:
-        self.__parent_network: NexusNetwork = parent_network
-        self.__wellheads: list[NexusWellhead] = []
-
-    def get_all(self) -> list[NexusWellhead]:
-        """Returns a list of wellheads loaded from the simulator."""
-        self.__parent_network.get_load_status()
-        return self.__wellheads
-
-    def get_by_name(self, name: str) -> Optional[NexusWellhead]:
-        """Returns a single wellhead with the provided name loaded from the simulator.
-
-        Args:
-            name (str): name of the requested well connection
-        Returns:
-            NexusWellhead: which has the same name as requested
-        """
-        to_return = filter(lambda x: False if x.name is None else x.name.upper() == name.upper(),
-                           self.__wellheads)
-        return next(to_return, None)
-
-    def get_df(self) -> pd.DataFrame:
-        return obj_to_dataframe(self.__wellheads)
-
-    def get_overview(self) -> str:
-        raise NotImplementedError('To be implemented')
-
-    def load(self, surface_file: File, start_date: str, default_units: UnitSystem) -> None:
-        new_wellheads = collect_all_tables_to_objects(surface_file, {'WELLHEAD': NexusWellhead},
-                                                      start_date=start_date,
-                                                      default_units=default_units)
-        wellheads_list = new_wellheads.get('WELLHEAD')
-        if isinstance(wellheads_list, dict):
-            raise ValueError('Incompatible data format for additional wells. Expected type "list" instead got "dict"')
-        self._add_to_memory(wellheads_list)
-
-    def _add_to_memory(self, additional_list: Optional[list[NexusWellhead]]) -> None:
-        """Extends the wellhead object by a list of wellheads provided to it.
-
-        Args:
-            additional_list (list[NexusWellhead]): list of nexus wellheads to add to the wellhead list.
-        """
-        if additional_list is None:
-            return
-        self.__wellheads.extend(additional_list)
-
-    def add(self, obj_to_add: dict[str, None | str | float | int]) -> None:
-        raise NotImplementedError
-
-    def remove(self, obj_to_remove: UUID | dict[str, None | str | float | int]) -> None:
-        raise NotImplementedError
-
-    def modify(self, obj_to_modify: dict[str, None | str | float | int],
-               new_properties: dict[str, None | str | float | int]) -> None:
-        raise NotImplementedError
-
-    @property
-    def table_header(self) -> str:
-        """Start of the wellhead definition table."""
-        return 'WELLHEAD'
-
-    @property
-    def table_footer(self) -> str:
-        """End of the wellhead definition table."""
-        return 'END' + self.table_header
+from __future__ import annotations
+from dataclasses import dataclass, field
+from typing import Optional, TYPE_CHECKING
+from uuid import UUID
+
+import pandas as pd
+
+from ResSimpy.File import File
+from ResSimpy.Nexus.nexus_collect_tables import collect_all_tables_to_objects
+from ResSimpy.Nexus.DataModels.Network.NexusWellhead import NexusWellhead
+from ResSimpy.Enums.UnitsEnum import UnitSystem
+from ResSimpy.Utils.obj_to_dataframe import obj_to_dataframe
+from ResSimpy.Wellheads import Wellheads
+
+if TYPE_CHECKING:
+    from ResSimpy.Nexus.NexusNetwork import NexusNetwork
+
+
+@dataclass
+class NexusWellheads(Wellheads):
+    __wellheads: list[NexusWellhead] = field(default_factory=list)
+
+    def __init__(self, parent_network: NexusNetwork) -> None:
+        self.__parent_network: NexusNetwork = parent_network
+        self.__wellheads: list[NexusWellhead] = []
+
+    def get_all(self) -> list[NexusWellhead]:
+        """Returns a list of wellheads loaded from the simulator."""
+        self.__parent_network.get_load_status()
+        return self.__wellheads
+
+    def get_by_name(self, name: str) -> Optional[NexusWellhead]:
+        """Returns a single wellhead with the provided name loaded from the simulator.
+
+        Args:
+            name (str): name of the requested well connection
+        Returns:
+            NexusWellhead: which has the same name as requested
+        """
+        to_return = filter(lambda x: False if x.name is None else x.name.upper() == name.upper(),
+                           self.__wellheads)
+        return next(to_return, None)
+
+    def get_df(self) -> pd.DataFrame:
+        return obj_to_dataframe(self.__wellheads)
+
+    def get_overview(self) -> str:
+        raise NotImplementedError('To be implemented')
+
+    def load(self, surface_file: File, start_date: str, default_units: UnitSystem) -> None:
+        new_wellheads = collect_all_tables_to_objects(surface_file, {'WELLHEAD': NexusWellhead},
+                                                      start_date=start_date,
+                                                      default_units=default_units)
+        wellheads_list = new_wellheads.get('WELLHEAD')
+        if isinstance(wellheads_list, dict):
+            raise ValueError('Incompatible data format for additional wells. Expected type "list" instead got "dict"')
+        self._add_to_memory(wellheads_list)
+
+    def _add_to_memory(self, additional_list: Optional[list[NexusWellhead]]) -> None:
+        """Extends the wellhead object by a list of wellheads provided to it.
+
+        Args:
+            additional_list (list[NexusWellhead]): list of nexus wellheads to add to the wellhead list.
+        """
+        if additional_list is None:
+            return
+        self.__wellheads.extend(additional_list)
+
+    def add(self, obj_to_add: dict[str, None | str | float | int]) -> None:
+        raise NotImplementedError
+
+    def remove(self, obj_to_remove: UUID | dict[str, None | str | float | int]) -> None:
+        raise NotImplementedError
+
+    def modify(self, obj_to_modify: dict[str, None | str | float | int],
+               new_properties: dict[str, None | str | float | int]) -> None:
+        raise NotImplementedError
+
+    @property
+    def table_header(self) -> str:
+        """Start of the wellhead definition table."""
+        return 'WELLHEAD'
+
+    @property
+    def table_footer(self) -> str:
+        """End of the wellhead definition table."""
+        return 'END' + self.table_header
```

### Comparing `ressimpy-1.0.0/ResSimpy/Nexus/DataModels/NexusAquiferMethod.py` & `ressimpy-1.0.1/ResSimpy/Nexus/DataModels/NexusAquiferMethod.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,120 +1,120 @@
-from dataclasses import dataclass, field
-from enum import Enum
-from typing import Optional, Union
-import pandas as pd
-from ResSimpy.Nexus.DataModels.NexusFile import NexusFile
-from ResSimpy.Nexus.NexusKeywords.aquifer_keywords import AQUIFER_SINGLE_KEYWORDS, AQUIFER_TABLE_KEYWORDS
-from ResSimpy.Nexus.NexusKeywords.aquifer_keywords import AQUIFER_KEYWORDS_VALUE_FLOAT, AQUIFER_KEYWORDS_VALUE_INT
-from ResSimpy.Nexus.NexusKeywords.aquifer_keywords import AQUIFER_KEYWORDS, AQUIFER_TYPE_KEYWORDS
-from ResSimpy.Enums.UnitsEnum import UnitSystem, SUnits, TemperatureUnits
-from ResSimpy.DynamicProperty import DynamicProperty
-
-from ResSimpy.Utils.factory_methods import get_empty_dict_union
-import ResSimpy.Nexus.nexus_file_operations as nfo
-
-
-@dataclass(kw_only=True, repr=False)  # Doesn't need to write an _init_, _eq_ methods, etc.
-class NexusAquiferMethod(DynamicProperty):
-    """Class to hold Nexus Aquifer properties.
-
-    Attributes:
-        file (NexusFile): Nexus aquifer properties file object
-        input_number (int): Aquifer properties method number in Nexus fcs file
-        properties (dict[str, Union[str, int, float, Enum, list[str], pd.DataFrame,
-                    dict[str, Union[float, pd.DataFrame]]]]):
-            Dictionary holding all properties for a specific aquifer properties method. Defaults to empty dictionary.
-    """
-
-    # General parameters
-    file: NexusFile
-    properties: dict[str, Union[str, int, float, Enum, list[str], pd.DataFrame,
-                                dict[str, Union[float, pd.DataFrame]]]] = field(default_factory=get_empty_dict_union)
-
-    def __init__(self, file: NexusFile, input_number: int,
-                 properties: Optional[dict[str, Union[str, int, float, Enum, list[str], pd.DataFrame,
-                                      dict[str, Union[float, pd.DataFrame]]]]] = None) -> None:
-        if properties is not None:
-            self.properties = properties
-        else:
-            self.properties = {}
-        super().__init__(input_number=input_number, file=file)
-
-    def to_string(self) -> str:
-        """Create string with aquifer data in Nexus file format."""
-        printable_str = ''
-        aquifer_dict = self.properties
-        for key, value in aquifer_dict.items():
-            if isinstance(value, pd.DataFrame):
-                printable_str += f'{key}\n'
-                printable_str += value.to_string(na_rep='', index=False) + '\n'
-                if key == 'TRACER':
-                    printable_str += 'ENDTRACER\n'
-                printable_str += '\n'
-            elif isinstance(value, Enum):
-                if isinstance(value, UnitSystem) or isinstance(value, TemperatureUnits):
-                    printable_str += f'{value.value}\n'
-                elif isinstance(value, SUnits):
-                    printable_str += f'SUNITS {value.value}\n'
-            elif key == 'DESC' and isinstance(value, list):
-                for desc_line in value:
-                    printable_str += 'DESC ' + desc_line + '\n'
-            elif key not in ['DESC']:
-                if value == '':
-                    printable_str += f'{key}\n'
-                else:
-                    printable_str += f'{key} {value}\n'
-        printable_str += '\n'
-        return printable_str
-
-    def read_properties(self) -> None:
-        """Read Nexus aquifer file contents and populate the NexusValveMethod object."""
-        file_as_list = self.file.get_flat_list_str_file
-
-        # Check for common input data
-        nfo.check_for_and_populate_common_input_data(file_as_list, self.properties)
-
-        # Initialize flags and containers to use to record properties as we iterate through aquifer file contents
-        # Dictionary to record start and ending indices for tables
-        aquifer_table_indices: dict[str, list[int]] = {}
-        # Dictionary of flags indicating which tables are being read
-        table_being_read: dict[str, bool] = {}
-        for table_name in AQUIFER_TABLE_KEYWORDS:
-            table_being_read[table_name] = False
-
-        line_indx = 0
-        for line in file_as_list:
-
-            # Find standalone aquifer keywords, such as CARTER_TRACY or LINEAR
-            if [i for i in line.split() if i in AQUIFER_TYPE_KEYWORDS + AQUIFER_SINGLE_KEYWORDS]:
-                for word in AQUIFER_TYPE_KEYWORDS + AQUIFER_SINGLE_KEYWORDS:
-                    if nfo.check_token(word, line):
-                        self.properties[word] = ''
-            # Find AQUIFER key-float value pairs, such as LINFAC 0.8 or BAQ 20.
-            if [i for i in line.split() if i in AQUIFER_KEYWORDS_VALUE_FLOAT]:
-                for key in AQUIFER_KEYWORDS_VALUE_FLOAT:
-                    if nfo.check_token(key, line):
-                        self.properties[key] = float(nfo.get_expected_token_value(key, line, file_as_list))
-            # Find AQUIFER key-int value pairs, such as ITDPD 1 or IWATER 2
-            if [i for i in line.split() if i in AQUIFER_KEYWORDS_VALUE_INT]:
-                for key in AQUIFER_KEYWORDS_VALUE_INT:
-                    if nfo.check_token(key, line):
-                        self.properties[key] = int(nfo.get_expected_token_value(key, line, file_as_list))
-
-            # Find beginning and ending indices of tables
-            for table_key in AQUIFER_TABLE_KEYWORDS:
-                if (table_key == 'TRACER' and table_being_read[table_key] and nfo.check_token('END' + table_key,
-                                                                                              line)) \
-                        or (table_key == 'TDPD' and table_being_read[table_key] and
-                            [i for i in line.split() if nfo.check_token(i, line) and i in AQUIFER_KEYWORDS]):
-                    table_being_read[table_key] = False
-                    aquifer_table_indices[table_key][1] = line_indx
-                if nfo.check_token(table_key, line):
-                    table_being_read[table_key] = True
-                    aquifer_table_indices[table_key] = [line_indx + 1, len(file_as_list)]
-
-            line_indx += 1
-
-        # Read in tables
-        for key in aquifer_table_indices.keys():
-            self.properties[key] = nfo.read_table_to_df(file_as_list[
-                                                        aquifer_table_indices[key][0]:aquifer_table_indices[key][1]])
+from dataclasses import dataclass, field
+from enum import Enum
+from typing import Optional, Union
+import pandas as pd
+from ResSimpy.Nexus.DataModels.NexusFile import NexusFile
+from ResSimpy.Nexus.NexusKeywords.aquifer_keywords import AQUIFER_SINGLE_KEYWORDS, AQUIFER_TABLE_KEYWORDS
+from ResSimpy.Nexus.NexusKeywords.aquifer_keywords import AQUIFER_KEYWORDS_VALUE_FLOAT, AQUIFER_KEYWORDS_VALUE_INT
+from ResSimpy.Nexus.NexusKeywords.aquifer_keywords import AQUIFER_KEYWORDS, AQUIFER_TYPE_KEYWORDS
+from ResSimpy.Enums.UnitsEnum import UnitSystem, SUnits, TemperatureUnits
+from ResSimpy.DynamicProperty import DynamicProperty
+
+from ResSimpy.Utils.factory_methods import get_empty_dict_union
+import ResSimpy.Nexus.nexus_file_operations as nfo
+
+
+@dataclass(kw_only=True, repr=False)  # Doesn't need to write an _init_, _eq_ methods, etc.
+class NexusAquiferMethod(DynamicProperty):
+    """Class to hold Nexus Aquifer properties.
+
+    Attributes:
+        file (NexusFile): Nexus aquifer properties file object
+        input_number (int): Aquifer properties method number in Nexus fcs file
+        properties (dict[str, Union[str, int, float, Enum, list[str], pd.DataFrame,
+                    dict[str, Union[float, pd.DataFrame]]]]):
+            Dictionary holding all properties for a specific aquifer properties method. Defaults to empty dictionary.
+    """
+
+    # General parameters
+    file: NexusFile
+    properties: dict[str, Union[str, int, float, Enum, list[str], pd.DataFrame,
+                                dict[str, Union[float, pd.DataFrame]]]] = field(default_factory=get_empty_dict_union)
+
+    def __init__(self, file: NexusFile, input_number: int,
+                 properties: Optional[dict[str, Union[str, int, float, Enum, list[str], pd.DataFrame,
+                                      dict[str, Union[float, pd.DataFrame]]]]] = None) -> None:
+        if properties is not None:
+            self.properties = properties
+        else:
+            self.properties = {}
+        super().__init__(input_number=input_number, file=file)
+
+    def to_string(self) -> str:
+        """Create string with aquifer data in Nexus file format."""
+        printable_str = ''
+        aquifer_dict = self.properties
+        for key, value in aquifer_dict.items():
+            if isinstance(value, pd.DataFrame):
+                printable_str += f'{key}\n'
+                printable_str += value.to_string(na_rep='', index=False) + '\n'
+                if key == 'TRACER':
+                    printable_str += 'ENDTRACER\n'
+                printable_str += '\n'
+            elif isinstance(value, Enum):
+                if isinstance(value, UnitSystem) or isinstance(value, TemperatureUnits):
+                    printable_str += f'{value.value}\n'
+                elif isinstance(value, SUnits):
+                    printable_str += f'SUNITS {value.value}\n'
+            elif key == 'DESC' and isinstance(value, list):
+                for desc_line in value:
+                    printable_str += 'DESC ' + desc_line + '\n'
+            elif key not in ['DESC']:
+                if value == '':
+                    printable_str += f'{key}\n'
+                else:
+                    printable_str += f'{key} {value}\n'
+        printable_str += '\n'
+        return printable_str
+
+    def read_properties(self) -> None:
+        """Read Nexus aquifer file contents and populate the NexusValveMethod object."""
+        file_as_list = self.file.get_flat_list_str_file
+
+        # Check for common input data
+        nfo.check_for_and_populate_common_input_data(file_as_list, self.properties)
+
+        # Initialize flags and containers to use to record properties as we iterate through aquifer file contents
+        # Dictionary to record start and ending indices for tables
+        aquifer_table_indices: dict[str, list[int]] = {}
+        # Dictionary of flags indicating which tables are being read
+        table_being_read: dict[str, bool] = {}
+        for table_name in AQUIFER_TABLE_KEYWORDS:
+            table_being_read[table_name] = False
+
+        line_indx = 0
+        for line in file_as_list:
+
+            # Find standalone aquifer keywords, such as CARTER_TRACY or LINEAR
+            if [i for i in line.split() if i in AQUIFER_TYPE_KEYWORDS + AQUIFER_SINGLE_KEYWORDS]:
+                for word in AQUIFER_TYPE_KEYWORDS + AQUIFER_SINGLE_KEYWORDS:
+                    if nfo.check_token(word, line):
+                        self.properties[word] = ''
+            # Find AQUIFER key-float value pairs, such as LINFAC 0.8 or BAQ 20.
+            if [i for i in line.split() if i in AQUIFER_KEYWORDS_VALUE_FLOAT]:
+                for key in AQUIFER_KEYWORDS_VALUE_FLOAT:
+                    if nfo.check_token(key, line):
+                        self.properties[key] = float(nfo.get_expected_token_value(key, line, file_as_list))
+            # Find AQUIFER key-int value pairs, such as ITDPD 1 or IWATER 2
+            if [i for i in line.split() if i in AQUIFER_KEYWORDS_VALUE_INT]:
+                for key in AQUIFER_KEYWORDS_VALUE_INT:
+                    if nfo.check_token(key, line):
+                        self.properties[key] = int(nfo.get_expected_token_value(key, line, file_as_list))
+
+            # Find beginning and ending indices of tables
+            for table_key in AQUIFER_TABLE_KEYWORDS:
+                if (table_key == 'TRACER' and table_being_read[table_key] and nfo.check_token('END' + table_key,
+                                                                                              line)) \
+                        or (table_key == 'TDPD' and table_being_read[table_key] and
+                            [i for i in line.split() if nfo.check_token(i, line) and i in AQUIFER_KEYWORDS]):
+                    table_being_read[table_key] = False
+                    aquifer_table_indices[table_key][1] = line_indx
+                if nfo.check_token(table_key, line):
+                    table_being_read[table_key] = True
+                    aquifer_table_indices[table_key] = [line_indx + 1, len(file_as_list)]
+
+            line_indx += 1
+
+        # Read in tables
+        for key in aquifer_table_indices.keys():
+            self.properties[key] = nfo.read_table_to_df(file_as_list[
+                                                        aquifer_table_indices[key][0]:aquifer_table_indices[key][1]])
```

### Comparing `ressimpy-1.0.0/ResSimpy/Nexus/DataModels/NexusEquilMethod.py` & `ressimpy-1.0.1/ResSimpy/Nexus/DataModels/NexusEquilMethod.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,157 +1,157 @@
-from dataclasses import dataclass, field
-from enum import Enum
-from typing import Union, Optional
-import pandas as pd
-from ResSimpy.Nexus.DataModels.NexusFile import NexusFile
-from ResSimpy.Enums.UnitsEnum import SUnits, TemperatureUnits, UnitSystem
-from ResSimpy.Nexus.NexusKeywords.equil_keywords import EQUIL_INTSAT_KEYWORDS, EQUIL_KEYWORDS_VALUE_FLOAT
-from ResSimpy.Nexus.NexusKeywords.equil_keywords import EQUIL_TABLE_KEYWORDS, EQUIL_SINGLE_KEYWORDS
-from ResSimpy.Nexus.NexusKeywords.equil_keywords import EQUIL_COMPOSITION_OPTIONS
-from ResSimpy.Nexus.NexusKeywords.equil_keywords import EQUIL_KEYWORDS
-from ResSimpy.DynamicProperty import DynamicProperty
-
-from ResSimpy.Utils.factory_methods import get_empty_dict_union
-import ResSimpy.Nexus.nexus_file_operations as nfo
-
-
-@dataclass(kw_only=True, repr=False)  # Doesn't need to write an _init_, _eq_ methods, etc.
-class NexusEquilMethod(DynamicProperty):
-    """Class to hold Nexus Equil properties.
-
-    Attributes:
-        file (NexusFile): Nexus equilibration file object
-        input_number (int): Equilibration method number in Nexus fcs file
-        properties (dict[str, Union[str, int, float, Enum, list[str], pd.DataFrame,
-                    dict[str, Union[float, pd.DataFrame]]]]):
-            Dictionary holding all properties for a specific equilibration method. Defaults to empty dictionary.
-    """
-
-    # General parameters
-    file: NexusFile
-    properties: dict[str, Union[str, int, float, Enum, list[str],
-                                pd.DataFrame, dict[str, Union[float, pd.DataFrame]]]] \
-        = field(default_factory=get_empty_dict_union)
-
-    def __init__(self, file: NexusFile, input_number: int,
-                 properties: Optional[dict[str, Union[str, int, float, Enum, list[str], pd.DataFrame,
-                                                      dict[str, Union[float, pd.DataFrame]]]]] = None) -> None:
-        if properties is not None:
-            self.properties = properties
-        else:
-            self.properties = {}
-        super().__init__(input_number=input_number, file=file)
-
-    def to_string(self) -> str:
-        """Create string with equilibration data in Nexus file format."""
-        printable_str = ''
-        equil_dict = self.properties
-        for key, value in equil_dict.items():
-            if isinstance(value, pd.DataFrame):
-                table_text = f'{key}'
-                if key == 'COMPOSITION':
-                    if 'X' in equil_dict.keys():
-                        table_text += f" X {equil_dict['X']}"
-                    if 'Y' in equil_dict.keys():
-                        table_text += f" Y {equil_dict['Y']}"
-                printable_str += f'{table_text}\n'
-                printable_str += value.to_string(na_rep='', index=False) + '\n'
-            elif isinstance(value, Enum):
-                if isinstance(value, UnitSystem) or isinstance(value, TemperatureUnits):
-                    printable_str += f'{value.value}\n'
-                elif isinstance(value, SUnits):
-                    printable_str += f'SUNITS {value.value}\n'
-            elif value == '':
-                printable_str += f'{key}\n'
-            elif key in ['INTSAT', 'VAITS']:
-                if value == 'MOBILE':
-                    printable_str += f'{key}\n    MOBILE\n'
-                    for mobkey in ['SORWMN', 'SORGMN', 'SGCMN']:
-                        if mobkey in equil_dict.keys():
-                            printable_str += f'        {mobkey} {equil_dict[mobkey]}\n'
-                for vaitkey in ['VAITS_TOLSG', 'VAITS_TOLSW']:
-                    if vaitkey in equil_dict.keys():
-                        printable_str += f'    {vaitkey} {equil_dict[vaitkey]}\n'
-            elif key == 'OVERREAD':
-                if isinstance(value, list):
-                    printable_str += f"OVERREAD {' '.join(value)}\n"
-            elif key not in ['SORWMN', 'SORGMN', 'SGCMN', 'VAITS_TOLSG', 'VAITS_TOLSW',
-                             'OVERREAD', 'INTSAT', 'VAITS', 'MOBILE', 'X', 'Y']:
-                printable_str += f'{key} {value}\n'
-        printable_str += '\n'
-        return printable_str
-
-    def read_properties(self) -> None:
-        """Read Nexus equilibration file contents and populate NexusEquilMethod object."""
-        file_as_list = self.file.get_flat_list_str_file
-
-        # Check for common input data
-        nfo.check_for_and_populate_common_input_data(file_as_list, self.properties)
-
-        # Initialize properties
-        equil_table_indices: dict[str, list[int]] = {}
-        # Flag to tell when to start reading a table
-        start_reading_table: bool = False
-        # Indicator of which of equilibration tables are being read
-        table_being_read = ''
-
-        line_indx = 0
-        for line in file_as_list:
-
-            # Find EQUIL key-value pairs, such as PINIT 3000, WOC 7000 or OVERREAD SW (list, multiple OVERREADs)
-            if [i for i in line.split() if i in EQUIL_KEYWORDS_VALUE_FLOAT]:
-                for key in EQUIL_KEYWORDS_VALUE_FLOAT:
-                    if nfo.check_token(key, line) and 'DEPTH' not in line.split():  # Ensure not a table header
-                        self.properties[key] = float(nfo.get_expected_token_value(key, line, file_as_list))
-            if nfo.check_token('AUTOGOC_COMP', line):
-                self.properties['AUTOGOC_COMP'] = nfo.get_expected_token_value('AUTOGOC_COMP', line, file_as_list)
-            if nfo.check_token('OVERREAD', line):
-                overread_vals = line.split('!')[0].split('OVERREAD')[1].split()
-                if 'OVERREAD' in self.properties.keys() and isinstance(self.properties['OVERREAD'], list):
-                    self.properties['OVERREAD'] += overread_vals
-                else:
-                    self.properties['OVERREAD'] = overread_vals
-            if nfo.check_token('VIP_INIT', line):
-                self.properties['VIP_INIT'] = ' '.join(line.split('!')[0].split()[1:])
-            # Find standalone equilibration keywords
-            if [i for i in line.split() if i in EQUIL_SINGLE_KEYWORDS]:
-                for word in EQUIL_SINGLE_KEYWORDS:
-                    if nfo.check_token(word, line):
-                        self.properties[word] = ''
-            # Handle integrated saturation initialization options
-            if [i for i in line.split() if i in EQUIL_INTSAT_KEYWORDS]:
-                for key in EQUIL_INTSAT_KEYWORDS:
-                    if nfo.check_token(key, line):
-                        if nfo.get_token_value(key, line, file_as_list) == 'MOBILE':
-                            self.properties[key] = 'MOBILE'
-                        else:
-                            self.properties[key] = ''
-
-            # Find starting index of an equil-related table. There is usually only one per equil file
-            if [i for i in line.split() if i in EQUIL_TABLE_KEYWORDS]:
-                for table_keyword in EQUIL_TABLE_KEYWORDS:
-                    if nfo.check_token(table_keyword, line):
-                        equil_table_indices[table_keyword] = [line_indx + 1, len(file_as_list)]
-                        table_being_read = table_keyword
-                        start_reading_table = True
-                        if table_keyword == 'COMPOSITION' and [i for i in line.split() if i in
-                                                               EQUIL_COMPOSITION_OPTIONS]:
-                            for comp_key in EQUIL_COMPOSITION_OPTIONS:
-                                if nfo.check_token(comp_key, line):
-                                    self.properties[comp_key] = float(nfo.get_expected_token_value(comp_key,
-                                                                                                   line, file_as_list))
-                line_indx += 1
-                continue
-            # Find ending index of an equil-related table. There is usually only one per equil file
-            if start_reading_table and 'DEPTH' not in line.split():
-                for potential_endkeyword in EQUIL_KEYWORDS:
-                    if nfo.check_token(potential_endkeyword, line):
-                        equil_table_indices[table_being_read][1] = line_indx
-                        start_reading_table = False
-                        break
-
-            line_indx += 1
-
-        # Read in table if there is one
-        for key in equil_table_indices.keys():
-            self.properties[key] = nfo.read_table_to_df(file_as_list[
-                equil_table_indices[key][0]:equil_table_indices[key][1]])
+from dataclasses import dataclass, field
+from enum import Enum
+from typing import Union, Optional
+import pandas as pd
+from ResSimpy.Nexus.DataModels.NexusFile import NexusFile
+from ResSimpy.Enums.UnitsEnum import SUnits, TemperatureUnits, UnitSystem
+from ResSimpy.Nexus.NexusKeywords.equil_keywords import EQUIL_INTSAT_KEYWORDS, EQUIL_KEYWORDS_VALUE_FLOAT
+from ResSimpy.Nexus.NexusKeywords.equil_keywords import EQUIL_TABLE_KEYWORDS, EQUIL_SINGLE_KEYWORDS
+from ResSimpy.Nexus.NexusKeywords.equil_keywords import EQUIL_COMPOSITION_OPTIONS
+from ResSimpy.Nexus.NexusKeywords.equil_keywords import EQUIL_KEYWORDS
+from ResSimpy.DynamicProperty import DynamicProperty
+
+from ResSimpy.Utils.factory_methods import get_empty_dict_union
+import ResSimpy.Nexus.nexus_file_operations as nfo
+
+
+@dataclass(kw_only=True, repr=False)  # Doesn't need to write an _init_, _eq_ methods, etc.
+class NexusEquilMethod(DynamicProperty):
+    """Class to hold Nexus Equil properties.
+
+    Attributes:
+        file (NexusFile): Nexus equilibration file object
+        input_number (int): Equilibration method number in Nexus fcs file
+        properties (dict[str, Union[str, int, float, Enum, list[str], pd.DataFrame,
+                    dict[str, Union[float, pd.DataFrame]]]]):
+            Dictionary holding all properties for a specific equilibration method. Defaults to empty dictionary.
+    """
+
+    # General parameters
+    file: NexusFile
+    properties: dict[str, Union[str, int, float, Enum, list[str],
+                                pd.DataFrame, dict[str, Union[float, pd.DataFrame]]]] \
+        = field(default_factory=get_empty_dict_union)
+
+    def __init__(self, file: NexusFile, input_number: int,
+                 properties: Optional[dict[str, Union[str, int, float, Enum, list[str], pd.DataFrame,
+                                                      dict[str, Union[float, pd.DataFrame]]]]] = None) -> None:
+        if properties is not None:
+            self.properties = properties
+        else:
+            self.properties = {}
+        super().__init__(input_number=input_number, file=file)
+
+    def to_string(self) -> str:
+        """Create string with equilibration data in Nexus file format."""
+        printable_str = ''
+        equil_dict = self.properties
+        for key, value in equil_dict.items():
+            if isinstance(value, pd.DataFrame):
+                table_text = f'{key}'
+                if key == 'COMPOSITION':
+                    if 'X' in equil_dict.keys():
+                        table_text += f" X {equil_dict['X']}"
+                    if 'Y' in equil_dict.keys():
+                        table_text += f" Y {equil_dict['Y']}"
+                printable_str += f'{table_text}\n'
+                printable_str += value.to_string(na_rep='', index=False) + '\n'
+            elif isinstance(value, Enum):
+                if isinstance(value, UnitSystem) or isinstance(value, TemperatureUnits):
+                    printable_str += f'{value.value}\n'
+                elif isinstance(value, SUnits):
+                    printable_str += f'SUNITS {value.value}\n'
+            elif value == '':
+                printable_str += f'{key}\n'
+            elif key in ['INTSAT', 'VAITS']:
+                if value == 'MOBILE':
+                    printable_str += f'{key}\n    MOBILE\n'
+                    for mobkey in ['SORWMN', 'SORGMN', 'SGCMN']:
+                        if mobkey in equil_dict.keys():
+                            printable_str += f'        {mobkey} {equil_dict[mobkey]}\n'
+                for vaitkey in ['VAITS_TOLSG', 'VAITS_TOLSW']:
+                    if vaitkey in equil_dict.keys():
+                        printable_str += f'    {vaitkey} {equil_dict[vaitkey]}\n'
+            elif key == 'OVERREAD':
+                if isinstance(value, list):
+                    printable_str += f"OVERREAD {' '.join(value)}\n"
+            elif key not in ['SORWMN', 'SORGMN', 'SGCMN', 'VAITS_TOLSG', 'VAITS_TOLSW',
+                             'OVERREAD', 'INTSAT', 'VAITS', 'MOBILE', 'X', 'Y']:
+                printable_str += f'{key} {value}\n'
+        printable_str += '\n'
+        return printable_str
+
+    def read_properties(self) -> None:
+        """Read Nexus equilibration file contents and populate NexusEquilMethod object."""
+        file_as_list = self.file.get_flat_list_str_file
+
+        # Check for common input data
+        nfo.check_for_and_populate_common_input_data(file_as_list, self.properties)
+
+        # Initialize properties
+        equil_table_indices: dict[str, list[int]] = {}
+        # Flag to tell when to start reading a table
+        start_reading_table: bool = False
+        # Indicator of which of equilibration tables are being read
+        table_being_read = ''
+
+        line_indx = 0
+        for line in file_as_list:
+
+            # Find EQUIL key-value pairs, such as PINIT 3000, WOC 7000 or OVERREAD SW (list, multiple OVERREADs)
+            if [i for i in line.split() if i in EQUIL_KEYWORDS_VALUE_FLOAT]:
+                for key in EQUIL_KEYWORDS_VALUE_FLOAT:
+                    if nfo.check_token(key, line) and 'DEPTH' not in line.split():  # Ensure not a table header
+                        self.properties[key] = float(nfo.get_expected_token_value(key, line, file_as_list))
+            if nfo.check_token('AUTOGOC_COMP', line):
+                self.properties['AUTOGOC_COMP'] = nfo.get_expected_token_value('AUTOGOC_COMP', line, file_as_list)
+            if nfo.check_token('OVERREAD', line):
+                overread_vals = line.split('!')[0].split('OVERREAD')[1].split()
+                if 'OVERREAD' in self.properties.keys() and isinstance(self.properties['OVERREAD'], list):
+                    self.properties['OVERREAD'] += overread_vals
+                else:
+                    self.properties['OVERREAD'] = overread_vals
+            if nfo.check_token('VIP_INIT', line):
+                self.properties['VIP_INIT'] = ' '.join(line.split('!')[0].split()[1:])
+            # Find standalone equilibration keywords
+            if [i for i in line.split() if i in EQUIL_SINGLE_KEYWORDS]:
+                for word in EQUIL_SINGLE_KEYWORDS:
+                    if nfo.check_token(word, line):
+                        self.properties[word] = ''
+            # Handle integrated saturation initialization options
+            if [i for i in line.split() if i in EQUIL_INTSAT_KEYWORDS]:
+                for key in EQUIL_INTSAT_KEYWORDS:
+                    if nfo.check_token(key, line):
+                        if nfo.get_token_value(key, line, file_as_list) == 'MOBILE':
+                            self.properties[key] = 'MOBILE'
+                        else:
+                            self.properties[key] = ''
+
+            # Find starting index of an equil-related table. There is usually only one per equil file
+            if [i for i in line.split() if i in EQUIL_TABLE_KEYWORDS]:
+                for table_keyword in EQUIL_TABLE_KEYWORDS:
+                    if nfo.check_token(table_keyword, line):
+                        equil_table_indices[table_keyword] = [line_indx + 1, len(file_as_list)]
+                        table_being_read = table_keyword
+                        start_reading_table = True
+                        if table_keyword == 'COMPOSITION' and [i for i in line.split() if i in
+                                                               EQUIL_COMPOSITION_OPTIONS]:
+                            for comp_key in EQUIL_COMPOSITION_OPTIONS:
+                                if nfo.check_token(comp_key, line):
+                                    self.properties[comp_key] = float(nfo.get_expected_token_value(comp_key,
+                                                                                                   line, file_as_list))
+                line_indx += 1
+                continue
+            # Find ending index of an equil-related table. There is usually only one per equil file
+            if start_reading_table and 'DEPTH' not in line.split():
+                for potential_endkeyword in EQUIL_KEYWORDS:
+                    if nfo.check_token(potential_endkeyword, line):
+                        equil_table_indices[table_being_read][1] = line_indx
+                        start_reading_table = False
+                        break
+
+            line_indx += 1
+
+        # Read in table if there is one
+        for key in equil_table_indices.keys():
+            self.properties[key] = nfo.read_table_to_df(file_as_list[
+                equil_table_indices[key][0]:equil_table_indices[key][1]])
```

### Comparing `ressimpy-1.0.0/ResSimpy/Nexus/DataModels/NexusFile.py` & `ressimpy-1.0.1/ResSimpy/Nexus/DataModels/NexusFile.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,620 +1,620 @@
-from __future__ import annotations
-
-import os.path
-import uuid
-from dataclasses import dataclass, field
-from typing import Optional, Generator
-
-# Use correct Self type depending upon Python version
-import sys
-
-if sys.version_info >= (3, 11):
-    from typing import Self
-else:
-    from typing_extensions import Self
-
-from uuid import UUID
-import re
-import ResSimpy.Nexus.nexus_file_operations as nfo
-import warnings
-from ResSimpy.Nexus.NexusKeywords.structured_grid_keywords import GRID_OPERATION_KEYWORDS, GRID_ARRAY_FORMAT_KEYWORDS, \
-    GRID_ARRAY_KEYWORDS
-from ResSimpy.Utils.factory_methods import get_empty_list_str, get_empty_list_nexus_file, \
-    get_empty_dict_uuid_list_int
-from ResSimpy.File import File
-import pathlib
-import os
-from datetime import datetime, timezone
-
-
-@dataclass(kw_only=True, repr=True)
-class NexusFile(File):
-    """Class to deal with origin and structure of Nexus files and preserve origin of include files.
-
-    Attributes:
-        location (Optional[str]): Path to the original file being opened. Defaults to None.
-        include_locations (Optional[list[str]]): list of file paths that the file contains. Defaults to None.
-        origin (Optional[str]): Where the file was opened from. Defaults to None.
-        include_objects (Optional[list[NexusFile]]): The include files but generated as a NexusFile instance. \
-            Defaults to None.
-        linked_user (Optional[str]): user or owner of the file. Defaults to None
-        last_modified (Optional[datetime]): last modified date of the file
-    """
-
-    include_locations: Optional[list[str]] = field(default=None)
-    origin: Optional[str] = None
-    include_objects: Optional[list[NexusFile]] = field(default=None, repr=False)
-    object_locations: Optional[dict[UUID, list[int]]] = field(default=None, repr=False)
-    line_locations: Optional[list[tuple[int, UUID]]] = field(default=None, repr=False)
-    linked_user: Optional[str] = field(default=None)
-    last_modified: Optional[datetime] = field(default=None)
-
-    def __init__(self, location: Optional[str] = None,
-                 include_locations: Optional[list[str]] = None,
-                 origin: Optional[str] = None,
-                 include_objects: Optional[list[NexusFile]] = None,
-                 file_content_as_list: Optional[list[str]] = None,
-                 linked_user: Optional[str] = None,
-                 last_modified: Optional[datetime] = None) -> None:
-        super().__init__(location=location, file_content_as_list=file_content_as_list)
-        if origin is not None and location is not None:
-            self.location = nfo.get_full_file_path(location, origin)
-        else:
-            self.location = location
-        self.input_file_location: Optional[str] = location
-        self.include_locations: Optional[list[str]] = get_empty_list_str() if include_locations is None else \
-            include_locations
-        self.origin: Optional[str] = origin
-        self.include_objects: Optional[list[NexusFile]] = get_empty_list_nexus_file() \
-            if include_objects is None else include_objects
-        if self.object_locations is None:
-            self.object_locations: dict[UUID, list[int]] = get_empty_dict_uuid_list_int()
-        if self.line_locations is None:
-            self.line_locations = []
-        self.file_id = uuid.uuid4()
-        self.linked_user = linked_user
-        self.last_modified = last_modified
-
-    @classmethod
-    def generate_file_include_structure(cls, file_path: str, origin: Optional[str] = None, recursive: bool = True,
-                                        skip_arrays: bool = True, top_level_file: bool = True) -> Self:
-        """Generates a nexus file instance for a provided text file with information storing the included files.
-
-        Args:
-            file_path (str): path to a file
-            origin (Optional[str], optional): Where the file was opened from. Defaults to None.
-            recursive (bool): Whether the method should recursively drill down multiple layers of include_locations.
-            skip_arrays (bool): If set True skips the INCLUDE arrays that come after property array and VALUE
-            top_level_file (bool): If set to True, the code assumes this is a 'top level' file rather than an included
-            one.
-
-        Returns:
-            NexusFile: a class instance for NexusFile with knowledge of include files
-        """
-        def __get_pathlib_path_details(full_file_path: str):
-            if full_file_path == "" or full_file_path is None:
-                return None
-            pathlib_path = pathlib.Path(full_file_path)
-            owner = pathlib_path.owner()
-            group = pathlib_path.group()
-            if owner is not None and group is not None:
-                return f"{owner}:{group}"
-            elif owner is not None:
-                return owner
-            return None
-
-        def __get_datetime_from_os_stat(full_file_path: str):
-            if full_file_path == "" or full_file_path is None:
-                return None
-            stat_obj = os.stat(full_file_path)
-            timestamp = stat_obj.st_mtime
-            if timestamp is None:
-                return None
-            return datetime.fromtimestamp(timestamp, tz=timezone.utc)
-
-        user = None
-        last_changed = None
-        full_file_path = file_path
-        if origin is not None:
-            full_file_path = nfo.get_full_file_path(file_path, origin)
-
-        user = __get_pathlib_path_details(full_file_path)
-        last_changed = __get_datetime_from_os_stat(full_file_path)
-        try:
-            file_as_list = nfo.load_file_as_list(full_file_path)
-        except FileNotFoundError:
-            # handle if a file can't be found
-            location = file_path
-
-            nexus_file_class = cls(location=location,
-                                   include_locations=None,
-                                   origin=origin,
-                                   include_objects=None,
-                                   file_content_as_list=None,
-                                   linked_user=user,
-                                   last_modified=last_changed)
-            warnings.warn(UserWarning(f'No file found for: {file_path} while loading {origin}'))
-            return nexus_file_class
-
-        # prevent python from mutating the lists that it's iterating over
-        modified_file_as_list: list[str] = []
-        # search for the INCLUDE keyword and append to a list:
-        inc_file_list: list[str] = []
-        includes_objects: Optional[list[NexusFile]] = []
-        skip_next_include = False
-        previous_line: str
-
-        for i, line in enumerate(file_as_list):
-            if len(modified_file_as_list) >= 1:
-                previous_line = modified_file_as_list[len(modified_file_as_list) - 1].rstrip('\n')
-                if previous_line.endswith('>'):
-                    modified_file_as_list[len(modified_file_as_list) - 1] = previous_line[:-1] + line
-                else:
-                    modified_file_as_list.append(line)
-            else:
-                modified_file_as_list.append(line)
-            if line.rstrip('\n').endswith('>'):
-                continue
-            if nfo.check_token("INCLUDE", line):
-                # Include found, check if we should skip loading it in (e.g. if it is a large array file)
-                ignore_keywords = ['NOLIST']
-                previous_value = nfo.get_previous_value(file_as_list=file_as_list[0: i + 1], search_before='INCLUDE',
-                                                        ignore_values=ignore_keywords)
-
-                keywords_to_skip_include = GRID_ARRAY_FORMAT_KEYWORDS + GRID_OPERATION_KEYWORDS + ["CORP"]
-                if previous_value is None:
-                    skip_next_include = False
-
-                elif previous_value.upper() in keywords_to_skip_include:
-                    skip_next_include = True
-
-            elif nfo.check_token("VALUE", line) and not top_level_file:
-                # Check if this is an 'embedded' grid array file. If it is, return this file with only the content up
-                # to this point to help with performance when analysing the files.
-                previous_value = nfo.get_previous_value(file_as_list=file_as_list[0: i + 1], search_before='VALUE')
-                next_value = nfo.get_next_value(start_line_index=0, file_as_list=file_as_list[i:],
-                                                search_string=line.upper().split('VALUE')[1])
-
-                if previous_value is None or next_value is None:
-                    continue
-
-                if next_value.upper() != 'INCLUDE' and previous_value.upper() in GRID_ARRAY_KEYWORDS:
-                    nexus_file_class = cls(
-                        location=file_path,
-                        include_locations=inc_file_list,
-                        origin=origin,
-                        include_objects=includes_objects,
-                        file_content_as_list=modified_file_as_list
-                    )
-
-                    return nexus_file_class
-                else:
-                    continue
-
-            else:
-                continue
-            inc_file_path = nfo.get_token_value('INCLUDE', line, file_as_list)
-            if inc_file_path is None:
-                continue
-            inc_full_path = nfo.get_full_file_path(inc_file_path, origin=full_file_path)
-            # store the included files as files inside the object
-            inc_file_list.append(inc_full_path)
-            if not recursive:
-                continue
-            elif skip_arrays and skip_next_include:
-                inc_file = cls(location=inc_file_path,
-                               include_locations=None,
-                               origin=full_file_path,
-                               include_objects=None,
-                               file_content_as_list=None,
-                               linked_user=user,
-                               last_modified=last_changed)
-                if includes_objects is None:
-                    raise ValueError('include_objects is None - recursion failure.')
-                skip_next_include = False
-            else:
-                inc_file = cls.generate_file_include_structure(inc_file_path, origin=full_file_path, recursive=True,
-                                                               skip_arrays=skip_arrays, top_level_file=False)
-                if includes_objects is None:
-                    raise ValueError('include_objects is None - recursion failure.')
-
-            includes_objects.append(inc_file)
-
-        includes_objects = None if not includes_objects else includes_objects
-
-        nexus_file_class = cls(
-            location=file_path,
-            include_locations=inc_file_list,
-            origin=origin,
-            include_objects=includes_objects,
-            file_content_as_list=modified_file_as_list,
-            linked_user=user,
-            last_modified=last_changed
-        )
-
-        return nexus_file_class
-
-    def export_network_lists(self):
-        """Exports lists of connections from and to for use in network graphs.
-
-        Raises:
-            ValueError: If the from and to lists are not the same length
-
-        Returns:
-            tuple[list]: list of to and from file paths where the equivalent indexes relate to a connection
-        """
-        from_list = [self.origin]
-        to_list = [self.location]
-        if not [self.origin]:
-            to_list = []
-        if self.include_locations is not None:
-            from_list += [self.location] * len(self.include_locations)
-            to_list += self.include_locations
-        if len(from_list) != len(to_list):
-            raise ValueError(
-                f"{from_list=} and {to_list=} are not the same length")
-
-        return from_list, to_list
-
-    @dataclass
-    class FileIndex:
-        index: int
-
-    def iterate_line(self, file_index: Optional[FileIndex] = None, max_depth: Optional[int] = None,
-                     parent: Optional[NexusFile] = None, prefix_line: Optional[str] = None,
-                     keep_include_references=False) -> \
-            Generator[str, None, None]:
-        """Generator object for iterating over a list of strings with nested NexusFile objects in them.
-
-        Yields:
-            str: sequential line from the file.
-        """
-
-        if file_index is None:
-            file_index = NexusFile.FileIndex(index=0)
-        if parent is None:
-            parent = self
-            parent.line_locations = []
-        if parent.line_locations is None:
-            parent.line_locations = []
-        if prefix_line is not None and prefix_line != ' ':
-            file_index.index += 1
-            yield prefix_line
-
-        new_entry = (file_index.index, self.file_id)
-        if new_entry not in parent.line_locations:
-            parent.line_locations.append(new_entry)
-        depth: int = 0
-        if max_depth is not None:
-            depth = max_depth
-        if self.file_content_as_list is None:
-            warnings.warn(f'No file content found for file: {self.location}')
-            return
-        for row in self.file_content_as_list:
-            if nfo.check_token('INCLUDE', row):
-                incfile_location = nfo.get_token_value('INCLUDE', row, self.file_content_as_list)
-                if incfile_location is None:
-                    continue
-                split_line = re.split(incfile_location, row, maxsplit=1, flags=re.IGNORECASE)
-                if len(split_line) == 2:
-                    prefix_line, suffix_line = split_line
-                    prefix_line = re.sub('INCLUDE', '', prefix_line, flags=re.IGNORECASE)
-                    prefix_line = prefix_line.rstrip() + ' '
-                    suffix_line = suffix_line.lstrip()
-                else:
-                    prefix_line = row.replace(incfile_location, '')
-                    suffix_line = None
-
-                include_file = None
-                if self.include_objects is None:
-                    raise ValueError(f'No include objects found in the nexusfile to expand over for file: '
-                                     f'{self.location}')
-                for obj in self.include_objects:
-                    if obj.location == incfile_location:
-                        include_file = obj
-                        break
-                    if self.origin is not None and \
-                            obj.location == nfo.get_full_file_path(incfile_location, self.origin):
-                        include_file = obj
-                        break
-                    if obj.location is not None and \
-                            os.path.basename(obj.location) == os.path.basename(incfile_location):
-                        include_file = obj
-                        break
-
-                if (max_depth is None or depth > 0) and include_file is not None:
-                    level_down_max_depth = None if max_depth is None else depth - 1
-
-                    if keep_include_references:
-                        yield row
-
-                    yield from include_file.iterate_line(file_index=file_index, max_depth=level_down_max_depth,
-                                                         parent=parent, prefix_line=prefix_line)
-
-                    new_entry = (file_index.index, self.file_id)
-                    if new_entry not in parent.line_locations:
-                        parent.line_locations.append(new_entry)
-                    if suffix_line:
-                        file_index.index += 1
-                        # Add in space between include location and the rest of the line
-                        suffix_line = ' ' + suffix_line
-                        yield suffix_line
-                else:
-                    continue
-            else:
-                file_index.index += 1
-                yield row
-
-    @property
-    def get_flat_list_str_file(self) -> list[str]:
-        if self.file_content_as_list is None:
-            raise ValueError(f'No file content found for {self.location}')
-        flat_list = list(self.iterate_line(file_index=None, keep_include_references=False))
-        return flat_list
-
-    @property
-    def get_flat_list_str_file_including_includes(self) -> list[str]:
-        if self.file_content_as_list is None:
-            raise ValueError(f'No file content found for {self.location}')
-        flat_list = list(self.iterate_line(file_index=None, keep_include_references=True))
-        return flat_list
-
-    # TODO write an output function using the iterate_line method
-    def get_full_network(self, max_depth: Optional[int] = None) -> tuple[list[str | None], list[str | None]]:
-        """Recursively constructs two lists of from and to nodes representing the connections between files.
-
-        Args:
-            max_depth (Optional[int], optional): depth of the iteration to construct the network down to. \
-                Defaults to None.
-
-        Returns:
-            tuple[list[str | None], list[str | None]]: two lists of from and to nodes where corresponding \
-                indices create an edge within a graph network. e.g. (from_list[i], to_list[i]) \
-                is a connection between two files.
-        """
-        depth: int = 0
-        from_list = [self.origin]
-        to_list = [self.location]
-        if max_depth is not None:
-            depth = max_depth
-        if self.file_content_as_list is None:
-            return from_list, to_list
-        for row in self.file_content_as_list:
-            if isinstance(row, NexusFile):
-                if (max_depth is None or depth > 0):
-                    level_down_max_depth = None if max_depth is None else depth - 1
-                    temp_from_list, temp_to_list = row.export_network_lists()
-                    from_list.extend(temp_from_list)
-                    to_list.extend(temp_to_list)
-                    temp_from_list, temp_to_list = row.get_full_network(max_depth=level_down_max_depth)
-                    from_list.extend(temp_from_list)
-                    to_list.extend(temp_to_list)
-        return from_list, to_list
-
-    def add_object_locations(self, obj_uuid: UUID, line_indices: list[int]) -> None:
-        """Adds a uuid to the object_locations dictionary. Used for storing the line numbers where objects are stored
-        within the flattened file_as_list.
-
-        Args:
-            obj_uuid (UUID): unique identifier of the object being created/stored.
-            line_indices (list[int]): line number in the flattened file_content_as_list
-                (i.e. from the get_flat_list_str_file method).
-        """
-        if self.object_locations is None:
-            self.object_locations: dict[UUID, list[int]] = get_empty_dict_uuid_list_int()
-        existing_line_locations = self.object_locations.get(obj_uuid, None)
-        if existing_line_locations is not None:
-            existing_line_locations.extend(line_indices)
-            existing_line_locations.sort()
-        else:
-            self.object_locations[obj_uuid] = line_indices
-
-    def __update_object_locations(self, line_number: int, number_additional_lines: int) -> None:
-        """Updates the object locations in a nexusfile by the additional lines. Used when files have been modified and
-        an addition/removal of lines has occurred. Ensures that the object locations are correct to the actual lines
-        in the file_as_list.
-
-        Args:
-            line_number (int): Line number at which the new lines have been added
-            number_additional_lines (int): number of new lines added.
-        """
-        if self.object_locations is None:
-            return
-        for object_id, list_indices in self.object_locations.items():
-            for i, obj_index in enumerate(list_indices):
-                if obj_index >= line_number:
-                    self.object_locations[object_id][i] = obj_index + number_additional_lines
-
-    def __remove_object_locations(self, obj_uuid: UUID) -> None:
-        """Removes an object location based on the obj_uuid provided. Used when removing objects in the file_as_list.
-
-        Args:
-            obj_uuid (UUID): id of the removed object.
-        """
-        if self.object_locations is None:
-            raise ValueError(f'No object locations found for file {self.location}')
-
-        if self.object_locations.get(obj_uuid, None) is None:
-            raise ValueError(f'No object with {obj_uuid=} found within the object locations')
-        self.object_locations.pop(obj_uuid, None)
-
-    def find_which_include_file(self, flattened_index: int) -> tuple[NexusFile, int]:
-        """Given a line index that relates to a position within the flattened file_as_list from the method
-        get_flat_file_as_list.
-
-        Args:
-            flattened_index (int): index in the flattened file as list structure
-
-        Returns:
-            tuple[NexusFile, int] where the first element is the file that the relevant line is in and the second
-            element is the relative index in that file.
-        """
-        if self.line_locations is None:
-            # call get_flat_list_str_file to ensure line locations are updated
-            self.get_flat_list_str_file
-            if self.line_locations is None:
-                raise ValueError("No include line locations found.")
-
-        line_locations = [x[0] for x in self.line_locations]
-        line_locations.sort()
-        uuid_index: Optional[UUID] = None
-        index_in_included_file = 0
-
-        # Find the Nexusfile containing the line we are looking for
-        for numlines, obj_id in self.line_locations:
-            if numlines <= flattened_index:
-                uuid_index = obj_id
-            if numlines >= flattened_index:
-                break
-
-        get_next_line_count = False
-        lines_already_included = 0
-        previous_lines_value = 0
-
-        # Add the previously included lines from the file (if any) to the location after it has been split
-        for numlines, obj_id in self.line_locations:
-            if obj_id == uuid_index:
-                get_next_line_count = True
-                previous_lines_value = numlines
-                continue
-            else:
-                # If we have gone beyond where the line is, calculate the location in the relevant file
-                if numlines >= flattened_index:
-                    lines_already_included += flattened_index - previous_lines_value
-                    break
-
-                if get_next_line_count:
-                    lines_already_included += numlines - previous_lines_value
-                    get_next_line_count = False
-                previous_lines_value = numlines
-
-        if flattened_index > line_locations[-1]:
-            lines_already_included += flattened_index - line_locations[-1]
-
-        index_in_included_file += lines_already_included
-
-        if uuid_index == self.file_id or self.include_objects is None:
-            return self, index_in_included_file
-
-        nexus_file = None
-        for file in self.include_objects:
-            if file.file_id == uuid_index:
-                nexus_file = file
-            elif file.include_objects is not None:
-                # CURRENTLY THIS ONLY SUPPORTS 2 LEVELS OF INCLUDES
-                for lvl_2_include in file.include_objects:
-                    if lvl_2_include.file_id == uuid_index:
-                        nexus_file = lvl_2_include
-        if nexus_file is None:
-            raise ValueError(f'No file with {uuid_index=} found within include objects')
-
-        return nexus_file, index_in_included_file
-
-    def add_to_file_as_list(self, additional_content: list[str], index: int,
-                            additional_objects: Optional[dict[UUID, list[int]]] = None,
-                            comments: Optional[str] = None) -> None:
-        """To add content to the file as list, also updates object numbers and optionally allows user \
-        to add several additional new objects.
-
-        Args:
-            additional_content (list[str]): Additional lines as a list of strings to be added.
-            index (int): index to insert the new lines at in the calling flat_file_as_list
-            additional_objects (Optional[dict[UUID, int]]): defaults to None. Otherwise, a dictionary keyed with the \
-            UUID of the new objects to add as well as the corresponding index of the object in the original \
-            calling NexusFile
-        """
-        if comments is not None:
-            additional_content = NexusFile.insert_comments(additional_content, comments)
-
-        nexusfile_to_write_to, relative_index = self.find_which_include_file(index)
-        if nexusfile_to_write_to.file_content_as_list is None:
-            raise ValueError(f'No file content to write to in file: {nexusfile_to_write_to}')
-        nexusfile_to_write_to.file_content_as_list = \
-            nexusfile_to_write_to.file_content_as_list[:relative_index] + \
-            additional_content + nexusfile_to_write_to.file_content_as_list[relative_index:]
-        # write straight to file
-        nexusfile_to_write_to.write_to_file()
-        # update object locations
-        self.__update_object_locations(line_number=index, number_additional_lines=len(additional_content))
-
-        if additional_objects is None:
-            return
-        for object_id, line_index in additional_objects.items():
-            self.add_object_locations(obj_uuid=object_id, line_indices=line_index)
-
-    def remove_object_from_file_as_list(self, objects_to_remove: list[UUID]) -> None:
-        """Removes all associated lines in the file as well as the object locations relating to a list of objects."""
-        if self.object_locations is None:
-            raise ValueError('Cannot remove object from object_locations as object_locations is None. '
-                             'Check object locations is being populated properly.')
-        for obj_to_remove in objects_to_remove:
-            # find all locations in the code that relate to the object
-            obj_locs = self.object_locations.get(obj_to_remove, None)
-            if obj_locs is None:
-                continue
-            # sort from highest to lowest to ensure line indices are not affected by removal of lines
-            sorted_obj_locs = sorted(obj_locs, reverse=True)
-            for i, index in enumerate(sorted_obj_locs):
-                if i == 0:
-                    # for the first removal remove the object location
-                    self.remove_from_file_as_list(index, objects_to_remove=[obj_to_remove])
-                else:
-                    # the remaining iterations remove just the lines
-                    self.remove_from_file_as_list(index)
-
-    def remove_from_file_as_list(self, index: int, objects_to_remove: Optional[list[UUID]] = None,
-                                 string_to_remove: Optional[str] = None) -> None:
-        """Remove an entry from the file as list. Also updates existing object locations and removes any \
-        specified objects from the object locations dictionary.
-
-        Args:
-            index (int): index n the calling flat_file_as_list to remove the entry from
-            objects_to_remove (Optional[list[UUID]]): list of object id's to remove from the object locations. \
-            Defaults to None
-            string_to_remove (Optional[str]): if specified will only remove the listed string from the entry \
-            at the index. Defaults to None, which removes the entire entry.
-
-        """
-        nexusfile_to_write_to, relative_index = self.find_which_include_file(index)
-
-        # remove the line in the file:
-        if nexusfile_to_write_to.file_content_as_list is None:
-            raise ValueError(
-                f'No file content in the file attempting to remove line from {nexusfile_to_write_to.location}')
-
-        if string_to_remove is None:
-            nexusfile_to_write_to.file_content_as_list.pop(relative_index)
-            self.__update_object_locations(line_number=index, number_additional_lines=-1)
-        else:
-            entry_to_replace = nexusfile_to_write_to.file_content_as_list[relative_index]
-            if isinstance(entry_to_replace, str):
-                nexusfile_to_write_to.file_content_as_list[relative_index] = \
-                    entry_to_replace.replace(string_to_remove, '', 1)
-            else:
-                raise ValueError(
-                    f'Tried to replace at non string value at index: {relative_index} in '
-                    f'file_as_list instead got {entry_to_replace}')
-
-        if objects_to_remove is not None:
-            for object_id in objects_to_remove:
-                self.__remove_object_locations(object_id)
-
-        nexusfile_to_write_to.write_to_file()
-
-    @staticmethod
-    def insert_comments(additional_content: list[str], comments) -> list[str]:
-        for index, element in enumerate(additional_content):
-            newline_index = element.find('\n')
-            if newline_index != -1:
-                modified_text = element[:newline_index] + ' ! ' + comments + element[newline_index:]
-                additional_content[index] = modified_text
-                return additional_content
-
-        additional_content[-1] += ' ! ' + comments + '\n'
-        return additional_content
-
-    def get_object_locations_for_id(self, id: UUID) -> list[int]:
-        """Gets the number of object locations for a specified id."""
-        if self.object_locations is None or len(self.object_locations[id]) == 0:
-            raise ValueError(f'No object locations specified, cannot find id: {id} in {self.object_locations}')
-        return self.object_locations[id]
+from __future__ import annotations
+
+import os.path
+import uuid
+from dataclasses import dataclass, field
+from typing import Optional, Generator
+
+# Use correct Self type depending upon Python version
+import sys
+
+if sys.version_info >= (3, 11):
+    from typing import Self
+else:
+    from typing_extensions import Self
+
+from uuid import UUID
+import re
+import ResSimpy.Nexus.nexus_file_operations as nfo
+import warnings
+from ResSimpy.Nexus.NexusKeywords.structured_grid_keywords import GRID_OPERATION_KEYWORDS, GRID_ARRAY_FORMAT_KEYWORDS, \
+    GRID_ARRAY_KEYWORDS
+from ResSimpy.Utils.factory_methods import get_empty_list_str, get_empty_list_nexus_file, \
+    get_empty_dict_uuid_list_int
+from ResSimpy.File import File
+import pathlib
+import os
+from datetime import datetime, timezone
+
+
+@dataclass(kw_only=True, repr=True)
+class NexusFile(File):
+    """Class to deal with origin and structure of Nexus files and preserve origin of include files.
+
+    Attributes:
+        location (Optional[str]): Path to the original file being opened. Defaults to None.
+        include_locations (Optional[list[str]]): list of file paths that the file contains. Defaults to None.
+        origin (Optional[str]): Where the file was opened from. Defaults to None.
+        include_objects (Optional[list[NexusFile]]): The include files but generated as a NexusFile instance. \
+            Defaults to None.
+        linked_user (Optional[str]): user or owner of the file. Defaults to None
+        last_modified (Optional[datetime]): last modified date of the file
+    """
+
+    include_locations: Optional[list[str]] = field(default=None)
+    origin: Optional[str] = None
+    include_objects: Optional[list[NexusFile]] = field(default=None, repr=False)
+    object_locations: Optional[dict[UUID, list[int]]] = field(default=None, repr=False)
+    line_locations: Optional[list[tuple[int, UUID]]] = field(default=None, repr=False)
+    linked_user: Optional[str] = field(default=None)
+    last_modified: Optional[datetime] = field(default=None)
+
+    def __init__(self, location: Optional[str] = None,
+                 include_locations: Optional[list[str]] = None,
+                 origin: Optional[str] = None,
+                 include_objects: Optional[list[NexusFile]] = None,
+                 file_content_as_list: Optional[list[str]] = None,
+                 linked_user: Optional[str] = None,
+                 last_modified: Optional[datetime] = None) -> None:
+        super().__init__(location=location, file_content_as_list=file_content_as_list)
+        if origin is not None and location is not None:
+            self.location = nfo.get_full_file_path(location, origin)
+        else:
+            self.location = location
+        self.input_file_location: Optional[str] = location
+        self.include_locations: Optional[list[str]] = get_empty_list_str() if include_locations is None else \
+            include_locations
+        self.origin: Optional[str] = origin
+        self.include_objects: Optional[list[NexusFile]] = get_empty_list_nexus_file() \
+            if include_objects is None else include_objects
+        if self.object_locations is None:
+            self.object_locations: dict[UUID, list[int]] = get_empty_dict_uuid_list_int()
+        if self.line_locations is None:
+            self.line_locations = []
+        self.file_id = uuid.uuid4()
+        self.linked_user = linked_user
+        self.last_modified = last_modified
+
+    @classmethod
+    def generate_file_include_structure(cls, file_path: str, origin: Optional[str] = None, recursive: bool = True,
+                                        skip_arrays: bool = True, top_level_file: bool = True) -> Self:
+        """Generates a nexus file instance for a provided text file with information storing the included files.
+
+        Args:
+            file_path (str): path to a file
+            origin (Optional[str], optional): Where the file was opened from. Defaults to None.
+            recursive (bool): Whether the method should recursively drill down multiple layers of include_locations.
+            skip_arrays (bool): If set True skips the INCLUDE arrays that come after property array and VALUE
+            top_level_file (bool): If set to True, the code assumes this is a 'top level' file rather than an included
+            one.
+
+        Returns:
+            NexusFile: a class instance for NexusFile with knowledge of include files
+        """
+        def __get_pathlib_path_details(full_file_path: str):
+            if full_file_path == "" or full_file_path is None:
+                return None
+            pathlib_path = pathlib.Path(full_file_path)
+            owner = pathlib_path.owner()
+            group = pathlib_path.group()
+            if owner is not None and group is not None:
+                return f"{owner}:{group}"
+            elif owner is not None:
+                return owner
+            return None
+
+        def __get_datetime_from_os_stat(full_file_path: str):
+            if full_file_path == "" or full_file_path is None:
+                return None
+            stat_obj = os.stat(full_file_path)
+            timestamp = stat_obj.st_mtime
+            if timestamp is None:
+                return None
+            return datetime.fromtimestamp(timestamp, tz=timezone.utc)
+
+        user = None
+        last_changed = None
+        full_file_path = file_path
+        if origin is not None:
+            full_file_path = nfo.get_full_file_path(file_path, origin)
+
+        user = __get_pathlib_path_details(full_file_path)
+        last_changed = __get_datetime_from_os_stat(full_file_path)
+        try:
+            file_as_list = nfo.load_file_as_list(full_file_path)
+        except FileNotFoundError:
+            # handle if a file can't be found
+            location = file_path
+
+            nexus_file_class = cls(location=location,
+                                   include_locations=None,
+                                   origin=origin,
+                                   include_objects=None,
+                                   file_content_as_list=None,
+                                   linked_user=user,
+                                   last_modified=last_changed)
+            warnings.warn(UserWarning(f'No file found for: {file_path} while loading {origin}'))
+            return nexus_file_class
+
+        # prevent python from mutating the lists that it's iterating over
+        modified_file_as_list: list[str] = []
+        # search for the INCLUDE keyword and append to a list:
+        inc_file_list: list[str] = []
+        includes_objects: Optional[list[NexusFile]] = []
+        skip_next_include = False
+        previous_line: str
+
+        for i, line in enumerate(file_as_list):
+            if len(modified_file_as_list) >= 1:
+                previous_line = modified_file_as_list[len(modified_file_as_list) - 1].rstrip('\n')
+                if previous_line.endswith('>'):
+                    modified_file_as_list[len(modified_file_as_list) - 1] = previous_line[:-1] + line
+                else:
+                    modified_file_as_list.append(line)
+            else:
+                modified_file_as_list.append(line)
+            if line.rstrip('\n').endswith('>'):
+                continue
+            if nfo.check_token("INCLUDE", line):
+                # Include found, check if we should skip loading it in (e.g. if it is a large array file)
+                ignore_keywords = ['NOLIST']
+                previous_value = nfo.get_previous_value(file_as_list=file_as_list[0: i + 1], search_before='INCLUDE',
+                                                        ignore_values=ignore_keywords)
+
+                keywords_to_skip_include = GRID_ARRAY_FORMAT_KEYWORDS + GRID_OPERATION_KEYWORDS + ["CORP"]
+                if previous_value is None:
+                    skip_next_include = False
+
+                elif previous_value.upper() in keywords_to_skip_include:
+                    skip_next_include = True
+
+            elif nfo.check_token("VALUE", line) and not top_level_file:
+                # Check if this is an 'embedded' grid array file. If it is, return this file with only the content up
+                # to this point to help with performance when analysing the files.
+                previous_value = nfo.get_previous_value(file_as_list=file_as_list[0: i + 1], search_before='VALUE')
+                next_value = nfo.get_next_value(start_line_index=0, file_as_list=file_as_list[i:],
+                                                search_string=line.upper().split('VALUE')[1])
+
+                if previous_value is None or next_value is None:
+                    continue
+
+                if next_value.upper() != 'INCLUDE' and previous_value.upper() in GRID_ARRAY_KEYWORDS:
+                    nexus_file_class = cls(
+                        location=file_path,
+                        include_locations=inc_file_list,
+                        origin=origin,
+                        include_objects=includes_objects,
+                        file_content_as_list=modified_file_as_list
+                    )
+
+                    return nexus_file_class
+                else:
+                    continue
+
+            else:
+                continue
+            inc_file_path = nfo.get_token_value('INCLUDE', line, file_as_list)
+            if inc_file_path is None:
+                continue
+            inc_full_path = nfo.get_full_file_path(inc_file_path, origin=full_file_path)
+            # store the included files as files inside the object
+            inc_file_list.append(inc_full_path)
+            if not recursive:
+                continue
+            elif skip_arrays and skip_next_include:
+                inc_file = cls(location=inc_file_path,
+                               include_locations=None,
+                               origin=full_file_path,
+                               include_objects=None,
+                               file_content_as_list=None,
+                               linked_user=user,
+                               last_modified=last_changed)
+                if includes_objects is None:
+                    raise ValueError('include_objects is None - recursion failure.')
+                skip_next_include = False
+            else:
+                inc_file = cls.generate_file_include_structure(inc_file_path, origin=full_file_path, recursive=True,
+                                                               skip_arrays=skip_arrays, top_level_file=False)
+                if includes_objects is None:
+                    raise ValueError('include_objects is None - recursion failure.')
+
+            includes_objects.append(inc_file)
+
+        includes_objects = None if not includes_objects else includes_objects
+
+        nexus_file_class = cls(
+            location=file_path,
+            include_locations=inc_file_list,
+            origin=origin,
+            include_objects=includes_objects,
+            file_content_as_list=modified_file_as_list,
+            linked_user=user,
+            last_modified=last_changed
+        )
+
+        return nexus_file_class
+
+    def export_network_lists(self):
+        """Exports lists of connections from and to for use in network graphs.
+
+        Raises:
+            ValueError: If the from and to lists are not the same length
+
+        Returns:
+            tuple[list]: list of to and from file paths where the equivalent indexes relate to a connection
+        """
+        from_list = [self.origin]
+        to_list = [self.location]
+        if not [self.origin]:
+            to_list = []
+        if self.include_locations is not None:
+            from_list += [self.location] * len(self.include_locations)
+            to_list += self.include_locations
+        if len(from_list) != len(to_list):
+            raise ValueError(
+                f"{from_list=} and {to_list=} are not the same length")
+
+        return from_list, to_list
+
+    @dataclass
+    class FileIndex:
+        index: int
+
+    def iterate_line(self, file_index: Optional[FileIndex] = None, max_depth: Optional[int] = None,
+                     parent: Optional[NexusFile] = None, prefix_line: Optional[str] = None,
+                     keep_include_references=False) -> \
+            Generator[str, None, None]:
+        """Generator object for iterating over a list of strings with nested NexusFile objects in them.
+
+        Yields:
+            str: sequential line from the file.
+        """
+
+        if file_index is None:
+            file_index = NexusFile.FileIndex(index=0)
+        if parent is None:
+            parent = self
+            parent.line_locations = []
+        if parent.line_locations is None:
+            parent.line_locations = []
+        if prefix_line is not None and prefix_line != ' ':
+            file_index.index += 1
+            yield prefix_line
+
+        new_entry = (file_index.index, self.file_id)
+        if new_entry not in parent.line_locations:
+            parent.line_locations.append(new_entry)
+        depth: int = 0
+        if max_depth is not None:
+            depth = max_depth
+        if self.file_content_as_list is None:
+            warnings.warn(f'No file content found for file: {self.location}')
+            return
+        for row in self.file_content_as_list:
+            if nfo.check_token('INCLUDE', row):
+                incfile_location = nfo.get_token_value('INCLUDE', row, self.file_content_as_list)
+                if incfile_location is None:
+                    continue
+                split_line = re.split(incfile_location, row, maxsplit=1, flags=re.IGNORECASE)
+                if len(split_line) == 2:
+                    prefix_line, suffix_line = split_line
+                    prefix_line = re.sub('INCLUDE', '', prefix_line, flags=re.IGNORECASE)
+                    prefix_line = prefix_line.rstrip() + ' '
+                    suffix_line = suffix_line.lstrip()
+                else:
+                    prefix_line = row.replace(incfile_location, '')
+                    suffix_line = None
+
+                include_file = None
+                if self.include_objects is None:
+                    raise ValueError(f'No include objects found in the nexusfile to expand over for file: '
+                                     f'{self.location}')
+                for obj in self.include_objects:
+                    if obj.location == incfile_location:
+                        include_file = obj
+                        break
+                    if self.origin is not None and \
+                            obj.location == nfo.get_full_file_path(incfile_location, self.origin):
+                        include_file = obj
+                        break
+                    if obj.location is not None and \
+                            os.path.basename(obj.location) == os.path.basename(incfile_location):
+                        include_file = obj
+                        break
+
+                if (max_depth is None or depth > 0) and include_file is not None:
+                    level_down_max_depth = None if max_depth is None else depth - 1
+
+                    if keep_include_references:
+                        yield row
+
+                    yield from include_file.iterate_line(file_index=file_index, max_depth=level_down_max_depth,
+                                                         parent=parent, prefix_line=prefix_line)
+
+                    new_entry = (file_index.index, self.file_id)
+                    if new_entry not in parent.line_locations:
+                        parent.line_locations.append(new_entry)
+                    if suffix_line:
+                        file_index.index += 1
+                        # Add in space between include location and the rest of the line
+                        suffix_line = ' ' + suffix_line
+                        yield suffix_line
+                else:
+                    continue
+            else:
+                file_index.index += 1
+                yield row
+
+    @property
+    def get_flat_list_str_file(self) -> list[str]:
+        if self.file_content_as_list is None:
+            raise ValueError(f'No file content found for {self.location}')
+        flat_list = list(self.iterate_line(file_index=None, keep_include_references=False))
+        return flat_list
+
+    @property
+    def get_flat_list_str_file_including_includes(self) -> list[str]:
+        if self.file_content_as_list is None:
+            raise ValueError(f'No file content found for {self.location}')
+        flat_list = list(self.iterate_line(file_index=None, keep_include_references=True))
+        return flat_list
+
+    # TODO write an output function using the iterate_line method
+    def get_full_network(self, max_depth: Optional[int] = None) -> tuple[list[str | None], list[str | None]]:
+        """Recursively constructs two lists of from and to nodes representing the connections between files.
+
+        Args:
+            max_depth (Optional[int], optional): depth of the iteration to construct the network down to. \
+                Defaults to None.
+
+        Returns:
+            tuple[list[str | None], list[str | None]]: two lists of from and to nodes where corresponding \
+                indices create an edge within a graph network. e.g. (from_list[i], to_list[i]) \
+                is a connection between two files.
+        """
+        depth: int = 0
+        from_list = [self.origin]
+        to_list = [self.location]
+        if max_depth is not None:
+            depth = max_depth
+        if self.file_content_as_list is None:
+            return from_list, to_list
+        for row in self.file_content_as_list:
+            if isinstance(row, NexusFile):
+                if (max_depth is None or depth > 0):
+                    level_down_max_depth = None if max_depth is None else depth - 1
+                    temp_from_list, temp_to_list = row.export_network_lists()
+                    from_list.extend(temp_from_list)
+                    to_list.extend(temp_to_list)
+                    temp_from_list, temp_to_list = row.get_full_network(max_depth=level_down_max_depth)
+                    from_list.extend(temp_from_list)
+                    to_list.extend(temp_to_list)
+        return from_list, to_list
+
+    def add_object_locations(self, obj_uuid: UUID, line_indices: list[int]) -> None:
+        """Adds a uuid to the object_locations dictionary. Used for storing the line numbers where objects are stored
+        within the flattened file_as_list.
+
+        Args:
+            obj_uuid (UUID): unique identifier of the object being created/stored.
+            line_indices (list[int]): line number in the flattened file_content_as_list
+                (i.e. from the get_flat_list_str_file method).
+        """
+        if self.object_locations is None:
+            self.object_locations: dict[UUID, list[int]] = get_empty_dict_uuid_list_int()
+        existing_line_locations = self.object_locations.get(obj_uuid, None)
+        if existing_line_locations is not None:
+            existing_line_locations.extend(line_indices)
+            existing_line_locations.sort()
+        else:
+            self.object_locations[obj_uuid] = line_indices
+
+    def __update_object_locations(self, line_number: int, number_additional_lines: int) -> None:
+        """Updates the object locations in a nexusfile by the additional lines. Used when files have been modified and
+        an addition/removal of lines has occurred. Ensures that the object locations are correct to the actual lines
+        in the file_as_list.
+
+        Args:
+            line_number (int): Line number at which the new lines have been added
+            number_additional_lines (int): number of new lines added.
+        """
+        if self.object_locations is None:
+            return
+        for object_id, list_indices in self.object_locations.items():
+            for i, obj_index in enumerate(list_indices):
+                if obj_index >= line_number:
+                    self.object_locations[object_id][i] = obj_index + number_additional_lines
+
+    def __remove_object_locations(self, obj_uuid: UUID) -> None:
+        """Removes an object location based on the obj_uuid provided. Used when removing objects in the file_as_list.
+
+        Args:
+            obj_uuid (UUID): id of the removed object.
+        """
+        if self.object_locations is None:
+            raise ValueError(f'No object locations found for file {self.location}')
+
+        if self.object_locations.get(obj_uuid, None) is None:
+            raise ValueError(f'No object with {obj_uuid=} found within the object locations')
+        self.object_locations.pop(obj_uuid, None)
+
+    def find_which_include_file(self, flattened_index: int) -> tuple[NexusFile, int]:
+        """Given a line index that relates to a position within the flattened file_as_list from the method
+        get_flat_file_as_list.
+
+        Args:
+            flattened_index (int): index in the flattened file as list structure
+
+        Returns:
+            tuple[NexusFile, int] where the first element is the file that the relevant line is in and the second
+            element is the relative index in that file.
+        """
+        if self.line_locations is None:
+            # call get_flat_list_str_file to ensure line locations are updated
+            self.get_flat_list_str_file
+            if self.line_locations is None:
+                raise ValueError("No include line locations found.")
+
+        line_locations = [x[0] for x in self.line_locations]
+        line_locations.sort()
+        uuid_index: Optional[UUID] = None
+        index_in_included_file = 0
+
+        # Find the Nexusfile containing the line we are looking for
+        for numlines, obj_id in self.line_locations:
+            if numlines <= flattened_index:
+                uuid_index = obj_id
+            if numlines >= flattened_index:
+                break
+
+        get_next_line_count = False
+        lines_already_included = 0
+        previous_lines_value = 0
+
+        # Add the previously included lines from the file (if any) to the location after it has been split
+        for numlines, obj_id in self.line_locations:
+            if obj_id == uuid_index:
+                get_next_line_count = True
+                previous_lines_value = numlines
+                continue
+            else:
+                # If we have gone beyond where the line is, calculate the location in the relevant file
+                if numlines >= flattened_index:
+                    lines_already_included += flattened_index - previous_lines_value
+                    break
+
+                if get_next_line_count:
+                    lines_already_included += numlines - previous_lines_value
+                    get_next_line_count = False
+                previous_lines_value = numlines
+
+        if flattened_index > line_locations[-1]:
+            lines_already_included += flattened_index - line_locations[-1]
+
+        index_in_included_file += lines_already_included
+
+        if uuid_index == self.file_id or self.include_objects is None:
+            return self, index_in_included_file
+
+        nexus_file = None
+        for file in self.include_objects:
+            if file.file_id == uuid_index:
+                nexus_file = file
+            elif file.include_objects is not None:
+                # CURRENTLY THIS ONLY SUPPORTS 2 LEVELS OF INCLUDES
+                for lvl_2_include in file.include_objects:
+                    if lvl_2_include.file_id == uuid_index:
+                        nexus_file = lvl_2_include
+        if nexus_file is None:
+            raise ValueError(f'No file with {uuid_index=} found within include objects')
+
+        return nexus_file, index_in_included_file
+
+    def add_to_file_as_list(self, additional_content: list[str], index: int,
+                            additional_objects: Optional[dict[UUID, list[int]]] = None,
+                            comments: Optional[str] = None) -> None:
+        """To add content to the file as list, also updates object numbers and optionally allows user \
+        to add several additional new objects.
+
+        Args:
+            additional_content (list[str]): Additional lines as a list of strings to be added.
+            index (int): index to insert the new lines at in the calling flat_file_as_list
+            additional_objects (Optional[dict[UUID, int]]): defaults to None. Otherwise, a dictionary keyed with the \
+            UUID of the new objects to add as well as the corresponding index of the object in the original \
+            calling NexusFile
+        """
+        if comments is not None:
+            additional_content = NexusFile.insert_comments(additional_content, comments)
+
+        nexusfile_to_write_to, relative_index = self.find_which_include_file(index)
+        if nexusfile_to_write_to.file_content_as_list is None:
+            raise ValueError(f'No file content to write to in file: {nexusfile_to_write_to}')
+        nexusfile_to_write_to.file_content_as_list = \
+            nexusfile_to_write_to.file_content_as_list[:relative_index] + \
+            additional_content + nexusfile_to_write_to.file_content_as_list[relative_index:]
+        # write straight to file
+        nexusfile_to_write_to.write_to_file()
+        # update object locations
+        self.__update_object_locations(line_number=index, number_additional_lines=len(additional_content))
+
+        if additional_objects is None:
+            return
+        for object_id, line_index in additional_objects.items():
+            self.add_object_locations(obj_uuid=object_id, line_indices=line_index)
+
+    def remove_object_from_file_as_list(self, objects_to_remove: list[UUID]) -> None:
+        """Removes all associated lines in the file as well as the object locations relating to a list of objects."""
+        if self.object_locations is None:
+            raise ValueError('Cannot remove object from object_locations as object_locations is None. '
+                             'Check object locations is being populated properly.')
+        for obj_to_remove in objects_to_remove:
+            # find all locations in the code that relate to the object
+            obj_locs = self.object_locations.get(obj_to_remove, None)
+            if obj_locs is None:
+                continue
+            # sort from highest to lowest to ensure line indices are not affected by removal of lines
+            sorted_obj_locs = sorted(obj_locs, reverse=True)
+            for i, index in enumerate(sorted_obj_locs):
+                if i == 0:
+                    # for the first removal remove the object location
+                    self.remove_from_file_as_list(index, objects_to_remove=[obj_to_remove])
+                else:
+                    # the remaining iterations remove just the lines
+                    self.remove_from_file_as_list(index)
+
+    def remove_from_file_as_list(self, index: int, objects_to_remove: Optional[list[UUID]] = None,
+                                 string_to_remove: Optional[str] = None) -> None:
+        """Remove an entry from the file as list. Also updates existing object locations and removes any \
+        specified objects from the object locations dictionary.
+
+        Args:
+            index (int): index n the calling flat_file_as_list to remove the entry from
+            objects_to_remove (Optional[list[UUID]]): list of object id's to remove from the object locations. \
+            Defaults to None
+            string_to_remove (Optional[str]): if specified will only remove the listed string from the entry \
+            at the index. Defaults to None, which removes the entire entry.
+
+        """
+        nexusfile_to_write_to, relative_index = self.find_which_include_file(index)
+
+        # remove the line in the file:
+        if nexusfile_to_write_to.file_content_as_list is None:
+            raise ValueError(
+                f'No file content in the file attempting to remove line from {nexusfile_to_write_to.location}')
+
+        if string_to_remove is None:
+            nexusfile_to_write_to.file_content_as_list.pop(relative_index)
+            self.__update_object_locations(line_number=index, number_additional_lines=-1)
+        else:
+            entry_to_replace = nexusfile_to_write_to.file_content_as_list[relative_index]
+            if isinstance(entry_to_replace, str):
+                nexusfile_to_write_to.file_content_as_list[relative_index] = \
+                    entry_to_replace.replace(string_to_remove, '', 1)
+            else:
+                raise ValueError(
+                    f'Tried to replace at non string value at index: {relative_index} in '
+                    f'file_as_list instead got {entry_to_replace}')
+
+        if objects_to_remove is not None:
+            for object_id in objects_to_remove:
+                self.__remove_object_locations(object_id)
+
+        nexusfile_to_write_to.write_to_file()
+
+    @staticmethod
+    def insert_comments(additional_content: list[str], comments) -> list[str]:
+        for index, element in enumerate(additional_content):
+            newline_index = element.find('\n')
+            if newline_index != -1:
+                modified_text = element[:newline_index] + ' ! ' + comments + element[newline_index:]
+                additional_content[index] = modified_text
+                return additional_content
+
+        additional_content[-1] += ' ! ' + comments + '\n'
+        return additional_content
+
+    def get_object_locations_for_id(self, id: UUID) -> list[int]:
+        """Gets the number of object locations for a specified id."""
+        if self.object_locations is None or len(self.object_locations[id]) == 0:
+            raise ValueError(f'No object locations specified, cannot find id: {id} in {self.object_locations}')
+        return self.object_locations[id]
```

### Comparing `ressimpy-1.0.0/ResSimpy/Nexus/DataModels/NexusGasliftMethod.py` & `ressimpy-1.0.1/ResSimpy/Nexus/DataModels/NexusGasliftMethod.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,103 +1,103 @@
-from dataclasses import dataclass, field
-from enum import Enum
-from typing import Optional, Union
-import pandas as pd
-from ResSimpy.Nexus.DataModels.NexusFile import NexusFile
-from ResSimpy.Enums.UnitsEnum import SUnits, TemperatureUnits, UnitSystem
-from ResSimpy.Nexus.NexusKeywords.gaslift_keywords import GL_ARRAY_KEYWORDS, GASLIFT_KEYWORDS, GL_TABLE_HEADER_COLS
-from ResSimpy.DynamicProperty import DynamicProperty
-
-from ResSimpy.Utils.factory_methods import get_empty_dict_union
-import ResSimpy.Nexus.nexus_file_operations as nfo
-
-
-@dataclass(kw_only=True, repr=False)  # Doesn't need to write an _init_, _eq_ methods, etc.
-class NexusGasliftMethod(DynamicProperty):
-    """Class to hold Nexus gaslift properties.
-
-    Attributes:
-        file (NexusFile): Nexus gaslift properties file object
-        input_number (int): Gaslift properties method number in Nexus fcs file
-        properties (dict[str, Union[str, int, float, Enum, list[str], pd.DataFrame,
-                    dict[str, Union[float, pd.DataFrame]]]]):
-            Dictionary holding all properties for a specific gaslift properties method. Defaults to empty dictionary.
-    """
-
-    # General parameters
-    file: NexusFile
-    properties: dict[str, Union[str, int, float, Enum, list[str], pd.DataFrame,
-                     dict[str, Union[float, pd.DataFrame]]]] = field(default_factory=get_empty_dict_union)
-
-    def __init__(self, file: NexusFile, input_number: int,
-                 properties: Optional[dict[str, Union[str, int, float, Enum, list[str], pd.DataFrame,
-                                      dict[str, Union[float, pd.DataFrame]]]]] = None) -> None:
-        if properties is not None:
-            self.properties = properties
-        else:
-            self.properties = {}
-        super().__init__(input_number=input_number, file=file)
-
-    def to_string(self) -> str:
-        """Create string with gaslift data in Nexus file format."""
-        printable_str = ''
-        gl_dict = self.properties
-        for key, value in gl_dict.items():
-            if isinstance(value, pd.DataFrame):
-                printable_str += value.to_string(na_rep='', index=False) + '\n'
-            elif isinstance(value, Enum):
-                if isinstance(value, UnitSystem | TemperatureUnits):
-                    printable_str += f'{value.value}\n'
-                elif isinstance(value, SUnits):
-                    printable_str += f'SUNITS {value.value}\n'
-            elif key == 'DESC' and isinstance(value, list):
-                for desc_line in value:
-                    printable_str += 'DESC ' + desc_line + '\n'
-            elif value == '':
-                printable_str += f'{key}\n'
-            else:
-                printable_str += f'{key} {value}\n'
-        printable_str += '\n'
-        return printable_str
-
-    def read_properties(self) -> None:
-        """Read Nexus gaslift file contents and populate the NexusGasliftMethod object."""
-        file_as_list = self.file.get_flat_list_str_file
-
-        # Check for common input data
-        nfo.check_for_and_populate_common_input_data(file_as_list, self.properties)
-
-        # Initialize flags and containers to use to record properties as we iterate through aquifer file contents
-        # Dictionary to record start and ending indices for tables
-        gl_table_indices: dict[str, list[int]] = {}
-        # Dictionary of flags indicating which tables are being read
-        start_reading_table = False
-
-        line_indx = 0
-        for line in file_as_list:
-
-            # Find arrays of parameters, e.g., QOIL 1.0 10. 100., or WCUT 0.0 0.1 0.2
-            potential_keyword = nfo.check_list_tokens(GL_ARRAY_KEYWORDS, line)
-            if potential_keyword is not None:
-                line_elems = line.split('!')[0].split()
-                keyword_index = line_elems.index(potential_keyword)
-                self.properties[potential_keyword] = ' '.join(line_elems[keyword_index+1:])
-
-            # Find ending index of gaslift table
-            if start_reading_table:
-                for potential_endkeyword in GASLIFT_KEYWORDS:
-                    if nfo.check_token(potential_endkeyword, line):
-                        gl_table_indices['GL_TABLE'][1] = line_indx
-                        start_reading_table = False
-                        break
-            # Find starting index of gaslift table
-            for header_keyword in GL_TABLE_HEADER_COLS:
-                if nfo.check_token(header_keyword, line):
-                    gl_table_indices['GL_TABLE'] = [line_indx, len(file_as_list)]
-                    start_reading_table = True
-
-            line_indx += 1
-
-        # Read in gaslift tables
-        for key in gl_table_indices.keys():
-            self.properties[key] = nfo.read_table_to_df(file_as_list[
-                gl_table_indices[key][0]:gl_table_indices[key][1]])
+from dataclasses import dataclass, field
+from enum import Enum
+from typing import Optional, Union
+import pandas as pd
+from ResSimpy.Nexus.DataModels.NexusFile import NexusFile
+from ResSimpy.Enums.UnitsEnum import SUnits, TemperatureUnits, UnitSystem
+from ResSimpy.Nexus.NexusKeywords.gaslift_keywords import GL_ARRAY_KEYWORDS, GASLIFT_KEYWORDS, GL_TABLE_HEADER_COLS
+from ResSimpy.DynamicProperty import DynamicProperty
+
+from ResSimpy.Utils.factory_methods import get_empty_dict_union
+import ResSimpy.Nexus.nexus_file_operations as nfo
+
+
+@dataclass(kw_only=True, repr=False)  # Doesn't need to write an _init_, _eq_ methods, etc.
+class NexusGasliftMethod(DynamicProperty):
+    """Class to hold Nexus gaslift properties.
+
+    Attributes:
+        file (NexusFile): Nexus gaslift properties file object
+        input_number (int): Gaslift properties method number in Nexus fcs file
+        properties (dict[str, Union[str, int, float, Enum, list[str], pd.DataFrame,
+                    dict[str, Union[float, pd.DataFrame]]]]):
+            Dictionary holding all properties for a specific gaslift properties method. Defaults to empty dictionary.
+    """
+
+    # General parameters
+    file: NexusFile
+    properties: dict[str, Union[str, int, float, Enum, list[str], pd.DataFrame,
+                     dict[str, Union[float, pd.DataFrame]]]] = field(default_factory=get_empty_dict_union)
+
+    def __init__(self, file: NexusFile, input_number: int,
+                 properties: Optional[dict[str, Union[str, int, float, Enum, list[str], pd.DataFrame,
+                                      dict[str, Union[float, pd.DataFrame]]]]] = None) -> None:
+        if properties is not None:
+            self.properties = properties
+        else:
+            self.properties = {}
+        super().__init__(input_number=input_number, file=file)
+
+    def to_string(self) -> str:
+        """Create string with gaslift data in Nexus file format."""
+        printable_str = ''
+        gl_dict = self.properties
+        for key, value in gl_dict.items():
+            if isinstance(value, pd.DataFrame):
+                printable_str += value.to_string(na_rep='', index=False) + '\n'
+            elif isinstance(value, Enum):
+                if isinstance(value, UnitSystem | TemperatureUnits):
+                    printable_str += f'{value.value}\n'
+                elif isinstance(value, SUnits):
+                    printable_str += f'SUNITS {value.value}\n'
+            elif key == 'DESC' and isinstance(value, list):
+                for desc_line in value:
+                    printable_str += 'DESC ' + desc_line + '\n'
+            elif value == '':
+                printable_str += f'{key}\n'
+            else:
+                printable_str += f'{key} {value}\n'
+        printable_str += '\n'
+        return printable_str
+
+    def read_properties(self) -> None:
+        """Read Nexus gaslift file contents and populate the NexusGasliftMethod object."""
+        file_as_list = self.file.get_flat_list_str_file
+
+        # Check for common input data
+        nfo.check_for_and_populate_common_input_data(file_as_list, self.properties)
+
+        # Initialize flags and containers to use to record properties as we iterate through aquifer file contents
+        # Dictionary to record start and ending indices for tables
+        gl_table_indices: dict[str, list[int]] = {}
+        # Dictionary of flags indicating which tables are being read
+        start_reading_table = False
+
+        line_indx = 0
+        for line in file_as_list:
+
+            # Find arrays of parameters, e.g., QOIL 1.0 10. 100., or WCUT 0.0 0.1 0.2
+            potential_keyword = nfo.check_list_tokens(GL_ARRAY_KEYWORDS, line)
+            if potential_keyword is not None:
+                line_elems = line.split('!')[0].split()
+                keyword_index = line_elems.index(potential_keyword)
+                self.properties[potential_keyword] = ' '.join(line_elems[keyword_index+1:])
+
+            # Find ending index of gaslift table
+            if start_reading_table:
+                for potential_endkeyword in GASLIFT_KEYWORDS:
+                    if nfo.check_token(potential_endkeyword, line):
+                        gl_table_indices['GL_TABLE'][1] = line_indx
+                        start_reading_table = False
+                        break
+            # Find starting index of gaslift table
+            for header_keyword in GL_TABLE_HEADER_COLS:
+                if nfo.check_token(header_keyword, line):
+                    gl_table_indices['GL_TABLE'] = [line_indx, len(file_as_list)]
+                    start_reading_table = True
+
+            line_indx += 1
+
+        # Read in gaslift tables
+        for key in gl_table_indices.keys():
+            self.properties[key] = nfo.read_table_to_df(file_as_list[
+                gl_table_indices[key][0]:gl_table_indices[key][1]])
```

### Comparing `ressimpy-1.0.0/ResSimpy/Nexus/DataModels/NexusHydraulicsMethod.py` & `ressimpy-1.0.1/ResSimpy/Nexus/DataModels/NexusHydraulicsMethod.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,203 +1,203 @@
-from dataclasses import dataclass, field
-from enum import Enum
-import re
-from typing import Optional, Union
-import pandas as pd
-from ResSimpy.Nexus.DataModels.NexusFile import NexusFile
-from ResSimpy.Nexus.NexusKeywords.hyd_keywords import HYD_ARRAY_KEYWORDS, HYD_TABLE_HEADER_COLS, HYD_KEYWORDS
-from ResSimpy.Nexus.NexusKeywords.hyd_keywords import HYD_PRESSURE_KEYWORDS, HYD_SINGLE_KEYWORDS
-from ResSimpy.Nexus.NexusKeywords.hyd_keywords import HYD_KEYWORDS_VALUE_FLOAT, HYD_WATINJ_KEYWORDS_VALUE_FLOAT
-from ResSimpy.Nexus.NexusKeywords.hyd_keywords import HYD_ALQ_KEYWORD, HYD_ALQ_OPTIONS
-from ResSimpy.Enums.UnitsEnum import UnitSystem, SUnits, TemperatureUnits
-from ResSimpy.DynamicProperty import DynamicProperty
-
-from ResSimpy.Utils.factory_methods import get_empty_dict_union
-import ResSimpy.Nexus.nexus_file_operations as nfo
-
-
-@dataclass(kw_only=True, repr=False)  # Doesn't need to write an _init_, _eq_ methods, etc.
-class NexusHydraulicsMethod(DynamicProperty):
-    """Class to hold Nexus Hydraulics properties.
-
-    Attributes:
-        file (NexusFile): Nexus hydraulics properties file object
-        input_number (int): Hydraulics properties method number in Nexus fcs file
-        properties (dict[str, Union[str, int, float, Enum, list[str], pd.DataFrame,
-                    dict[str, Union[float, pd.DataFrame]]]]):
-            Dictionary holding all properties for a specific hydraulics properties method. Defaults to empty dictionary.
-    """
-
-    # General parameters
-    file: NexusFile
-    properties: dict[str, Union[str, int, float, Enum, list[str], pd.DataFrame,
-                     dict[str, Union[float, pd.DataFrame]]]] = field(default_factory=get_empty_dict_union)
-
-    def __init__(self, file: NexusFile, input_number: int,
-                 properties: Optional[dict[str, Union[str, int, float, Enum, list[str], pd.DataFrame,
-                                      dict[str, Union[float, pd.DataFrame]]]]] = None) -> None:
-        if properties is not None:
-            self.properties = properties
-        else:
-            self.properties = {}
-        super().__init__(input_number=input_number, file=file)
-
-    def to_string(self) -> str:
-        """Create string with hydraulics data in Nexus file format."""
-        printable_str = ''
-        hyd_dict = self.properties
-        for key, value in hyd_dict.items():
-            if isinstance(value, pd.DataFrame):
-                if key not in ['HYD_TABLE']:
-                    printable_str += f'{key}\n'
-                printable_str += value.to_string(na_rep='', index=False) + '\n'
-                if key == 'LIMITS':
-                    printable_str += 'ENDLIMITS\n'
-                printable_str += '\n'
-            elif key == 'DESC' and isinstance(value, list):
-                for desc_line in value:
-                    printable_str += 'DESC ' + desc_line + '\n'
-            elif isinstance(value, Enum):
-                if isinstance(value, UnitSystem) or isinstance(value, TemperatureUnits):
-                    printable_str += f'{value.value}\n'
-                elif isinstance(value, SUnits):
-                    printable_str += f'SUNITS {value.value}\n'
-            elif key == 'ALQ':
-                printable_str += f'{key}'
-                if 'ALQ_PARAM' in hyd_dict.keys():
-                    printable_str += f" {hyd_dict['ALQ_PARAM']}"
-                printable_str += f' {value}\n'
-            elif key == 'WATINJ' and isinstance(value, dict):
-                printable_str += f'{key}\n'
-                for watinj_key in value.keys():
-                    printable_str += f'    {watinj_key} {value[watinj_key]}\n'
-            elif key not in ['ALQ', 'ALQ_PARAM', 'WATINJ']:
-                if value == '':
-                    printable_str += f'{key}\n'
-                else:
-                    printable_str += f'{key} {value}\n'
-        printable_str += '\n'
-        return printable_str
-
-    def read_properties(self) -> None:
-        """Read Nexus hydraulics file contents and populate the NexusHydraulicsMethod object."""
-        file_as_list0 = self.file.get_flat_list_str_file
-
-        # Loop through file_as_list and fix any line continuations that use '>' at the end of the line
-        file_as_list: list[str] = []
-        if len(file_as_list0) > 0:
-            file_as_list = [file_as_list0[0]]
-            line_indx = 1
-            while line_indx < len(file_as_list0):
-                prev_line = file_as_list[-1]
-                line = file_as_list0[line_indx]
-                if prev_line.endswith(('>', '>\n')):
-                    file_as_list[-1] = prev_line.split('>')[0] + ' ' + line.strip()
-                else:
-                    file_as_list.append(line)
-                line_indx += 1
-
-        # Check for common input data
-        nfo.check_for_and_populate_common_input_data(file_as_list, self.properties)
-
-        # Initialize flags and containers to use to record properties as we iterate through aquifer file contents
-        # Dictionary to record start and ending indices for tables
-        hyd_table_indices: dict[str, list[int]] = {}
-        # Dictionary of flags indicating which tables are being read
-        table_being_read: dict[str, bool] = {'HYD_TABLE': False, 'LIMITS': False}
-        start_reading_table = False
-        # Containers for handling WATERINJ data
-        watinj_dict: dict[str, float] = {}
-        found_waterinj = False
-
-        line_indx = 0
-        for line in file_as_list:
-
-            # Find arrays of parameters, e.g., QOIL 1.0 10. 100., or GOR 0.0 0.5 1.0
-            potential_keyword = nfo.check_list_tokens(HYD_ARRAY_KEYWORDS + HYD_ALQ_KEYWORD, line)
-            if potential_keyword is not None and not table_being_read['LIMITS']:
-                line_elems = line.split('!')[0].split()
-                next_val = nfo.get_expected_token_value(potential_keyword, line, file_as_list)
-                if potential_keyword == 'ALQ' and next_val in HYD_ALQ_OPTIONS:
-                    self.properties['ALQ_PARAM'] = next_val
-                    keyword_index = line_elems.index(next_val)
-                else:
-                    keyword_index = line_elems.index(potential_keyword)
-                self.properties[potential_keyword] = ' '.join(line_elems[keyword_index+1:])
-
-            # Create WATINJ property if needed
-            if nfo.check_token('WATINJ', line):
-                found_waterinj = True
-
-            # Handle DATGRAD property
-            if nfo.check_token('DATGRAD', line):
-                self.properties['DATGRAD'] = nfo.get_expected_token_value('DATGRAD', line, file_as_list)
-
-            # Find HYD key-value pairs, such as LENGTH 3000, DATUM 7000 or DATGRAD GRAD
-            potential_keyword = nfo.check_list_tokens(HYD_KEYWORDS_VALUE_FLOAT + HYD_WATINJ_KEYWORDS_VALUE_FLOAT, line)
-            if potential_keyword is not None:
-                if found_waterinj and potential_keyword in HYD_WATINJ_KEYWORDS_VALUE_FLOAT:
-                    watinj_dict[potential_keyword] = float(
-                        nfo.get_expected_token_value(potential_keyword, line, file_as_list))
-                elif potential_keyword in HYD_KEYWORDS_VALUE_FLOAT:
-                    self.properties[potential_keyword] = float(
-                        nfo.get_expected_token_value(potential_keyword, line, file_as_list))
-
-            # Find standalone hydraulics keywords
-            potential_keyword = nfo.check_list_tokens(HYD_SINGLE_KEYWORDS, line)
-            if potential_keyword is not None:
-                self.properties[potential_keyword] = ''
-
-            # Find starting and ending indices for hydraulic limits table
-            if nfo.check_token('LIMITS', line):
-                hyd_table_indices['LIMITS'] = [line_indx+1, len(file_as_list)]
-                table_being_read['LIMITS'] = True
-                start_reading_table = True
-            if nfo.check_token('ENDLIMITS', line):
-                hyd_table_indices['LIMITS'][1] = line_indx
-                table_being_read['LIMITS'] = False
-                start_reading_table = False
-
-            # Find ending index of hydraulics table
-            if start_reading_table and table_being_read['HYD_TABLE']:
-                for potential_endkeyword in HYD_KEYWORDS:
-                    if nfo.check_token(potential_endkeyword, line):
-                        hyd_table_indices['HYD_TABLE'][1] = line_indx
-                        start_reading_table = False
-                        table_being_read['HYD_TABLE'] = False
-                        break
-            # Find starting index of hydraulics table
-            for header_keyword in HYD_TABLE_HEADER_COLS:
-                if nfo.check_token(header_keyword, line):
-                    hyd_table_indices['HYD_TABLE'] = [line_indx, len(file_as_list)]
-                    table_being_read['HYD_TABLE'] = True
-                    start_reading_table = True
-
-            line_indx += 1
-
-        # Read in hydraulics tables
-        for key in hyd_table_indices.keys():
-            if key == 'HYD_TABLE':
-                # Get hydraulic table data
-                hyd_df: pd.DataFrame = nfo.read_table_to_df(file_as_list[
-                    hyd_table_indices[key][0]+1:hyd_table_indices[key][1]], noheader=True)
-                # Resolve hydraulic table header
-                hyd_df_header_names = [header_name for header_name in file_as_list[
-                    hyd_table_indices[key][0]].split('!')[0].split() if not re.search('BHP', header_name)]
-                pressure_keyword_map = {'PIN': 'POUT', 'POUT': 'PIN', 'THP': 'BHP'}
-                hyd_table_pressure_key = ''  # Determines what type of pressures are in table, i.e., PIN, POUT or BHP
-                for pkey in HYD_PRESSURE_KEYWORDS:
-                    if pkey in self.properties.keys():
-                        hyd_table_pressure_key = pressure_keyword_map[pkey]
-                        break
-                hyd_df_header_names = hyd_df_header_names + \
-                    [hyd_table_pressure_key+str(i) for i in range(hyd_df.shape[1] - len(hyd_df_header_names))]
-                hyd_df.columns = hyd_df_header_names
-                # Set appropriate hydraulic table property
-                self.properties[key] = hyd_df
-            else:
-                self.properties[key] = nfo.read_table_to_df(file_as_list[
-                    hyd_table_indices[key][0]:hyd_table_indices[key][1]])
-
-        # Correctly set WATINJ properties, if needed
-        if found_waterinj:
-            self.properties['WATINJ'] = watinj_dict
+from dataclasses import dataclass, field
+from enum import Enum
+import re
+from typing import Optional, Union
+import pandas as pd
+from ResSimpy.Nexus.DataModels.NexusFile import NexusFile
+from ResSimpy.Nexus.NexusKeywords.hyd_keywords import HYD_ARRAY_KEYWORDS, HYD_TABLE_HEADER_COLS, HYD_KEYWORDS
+from ResSimpy.Nexus.NexusKeywords.hyd_keywords import HYD_PRESSURE_KEYWORDS, HYD_SINGLE_KEYWORDS
+from ResSimpy.Nexus.NexusKeywords.hyd_keywords import HYD_KEYWORDS_VALUE_FLOAT, HYD_WATINJ_KEYWORDS_VALUE_FLOAT
+from ResSimpy.Nexus.NexusKeywords.hyd_keywords import HYD_ALQ_KEYWORD, HYD_ALQ_OPTIONS
+from ResSimpy.Enums.UnitsEnum import UnitSystem, SUnits, TemperatureUnits
+from ResSimpy.DynamicProperty import DynamicProperty
+
+from ResSimpy.Utils.factory_methods import get_empty_dict_union
+import ResSimpy.Nexus.nexus_file_operations as nfo
+
+
+@dataclass(kw_only=True, repr=False)  # Doesn't need to write an _init_, _eq_ methods, etc.
+class NexusHydraulicsMethod(DynamicProperty):
+    """Class to hold Nexus Hydraulics properties.
+
+    Attributes:
+        file (NexusFile): Nexus hydraulics properties file object
+        input_number (int): Hydraulics properties method number in Nexus fcs file
+        properties (dict[str, Union[str, int, float, Enum, list[str], pd.DataFrame,
+                    dict[str, Union[float, pd.DataFrame]]]]):
+            Dictionary holding all properties for a specific hydraulics properties method. Defaults to empty dictionary.
+    """
+
+    # General parameters
+    file: NexusFile
+    properties: dict[str, Union[str, int, float, Enum, list[str], pd.DataFrame,
+                     dict[str, Union[float, pd.DataFrame]]]] = field(default_factory=get_empty_dict_union)
+
+    def __init__(self, file: NexusFile, input_number: int,
+                 properties: Optional[dict[str, Union[str, int, float, Enum, list[str], pd.DataFrame,
+                                      dict[str, Union[float, pd.DataFrame]]]]] = None) -> None:
+        if properties is not None:
+            self.properties = properties
+        else:
+            self.properties = {}
+        super().__init__(input_number=input_number, file=file)
+
+    def to_string(self) -> str:
+        """Create string with hydraulics data in Nexus file format."""
+        printable_str = ''
+        hyd_dict = self.properties
+        for key, value in hyd_dict.items():
+            if isinstance(value, pd.DataFrame):
+                if key not in ['HYD_TABLE']:
+                    printable_str += f'{key}\n'
+                printable_str += value.to_string(na_rep='', index=False) + '\n'
+                if key == 'LIMITS':
+                    printable_str += 'ENDLIMITS\n'
+                printable_str += '\n'
+            elif key == 'DESC' and isinstance(value, list):
+                for desc_line in value:
+                    printable_str += 'DESC ' + desc_line + '\n'
+            elif isinstance(value, Enum):
+                if isinstance(value, UnitSystem) or isinstance(value, TemperatureUnits):
+                    printable_str += f'{value.value}\n'
+                elif isinstance(value, SUnits):
+                    printable_str += f'SUNITS {value.value}\n'
+            elif key == 'ALQ':
+                printable_str += f'{key}'
+                if 'ALQ_PARAM' in hyd_dict.keys():
+                    printable_str += f" {hyd_dict['ALQ_PARAM']}"
+                printable_str += f' {value}\n'
+            elif key == 'WATINJ' and isinstance(value, dict):
+                printable_str += f'{key}\n'
+                for watinj_key in value.keys():
+                    printable_str += f'    {watinj_key} {value[watinj_key]}\n'
+            elif key not in ['ALQ', 'ALQ_PARAM', 'WATINJ']:
+                if value == '':
+                    printable_str += f'{key}\n'
+                else:
+                    printable_str += f'{key} {value}\n'
+        printable_str += '\n'
+        return printable_str
+
+    def read_properties(self) -> None:
+        """Read Nexus hydraulics file contents and populate the NexusHydraulicsMethod object."""
+        file_as_list0 = self.file.get_flat_list_str_file
+
+        # Loop through file_as_list and fix any line continuations that use '>' at the end of the line
+        file_as_list: list[str] = []
+        if len(file_as_list0) > 0:
+            file_as_list = [file_as_list0[0]]
+            line_indx = 1
+            while line_indx < len(file_as_list0):
+                prev_line = file_as_list[-1]
+                line = file_as_list0[line_indx]
+                if prev_line.endswith(('>', '>\n')):
+                    file_as_list[-1] = prev_line.split('>')[0] + ' ' + line.strip()
+                else:
+                    file_as_list.append(line)
+                line_indx += 1
+
+        # Check for common input data
+        nfo.check_for_and_populate_common_input_data(file_as_list, self.properties)
+
+        # Initialize flags and containers to use to record properties as we iterate through aquifer file contents
+        # Dictionary to record start and ending indices for tables
+        hyd_table_indices: dict[str, list[int]] = {}
+        # Dictionary of flags indicating which tables are being read
+        table_being_read: dict[str, bool] = {'HYD_TABLE': False, 'LIMITS': False}
+        start_reading_table = False
+        # Containers for handling WATERINJ data
+        watinj_dict: dict[str, float] = {}
+        found_waterinj = False
+
+        line_indx = 0
+        for line in file_as_list:
+
+            # Find arrays of parameters, e.g., QOIL 1.0 10. 100., or GOR 0.0 0.5 1.0
+            potential_keyword = nfo.check_list_tokens(HYD_ARRAY_KEYWORDS + HYD_ALQ_KEYWORD, line)
+            if potential_keyword is not None and not table_being_read['LIMITS']:
+                line_elems = line.split('!')[0].split()
+                next_val = nfo.get_expected_token_value(potential_keyword, line, file_as_list)
+                if potential_keyword == 'ALQ' and next_val in HYD_ALQ_OPTIONS:
+                    self.properties['ALQ_PARAM'] = next_val
+                    keyword_index = line_elems.index(next_val)
+                else:
+                    keyword_index = line_elems.index(potential_keyword)
+                self.properties[potential_keyword] = ' '.join(line_elems[keyword_index+1:])
+
+            # Create WATINJ property if needed
+            if nfo.check_token('WATINJ', line):
+                found_waterinj = True
+
+            # Handle DATGRAD property
+            if nfo.check_token('DATGRAD', line):
+                self.properties['DATGRAD'] = nfo.get_expected_token_value('DATGRAD', line, file_as_list)
+
+            # Find HYD key-value pairs, such as LENGTH 3000, DATUM 7000 or DATGRAD GRAD
+            potential_keyword = nfo.check_list_tokens(HYD_KEYWORDS_VALUE_FLOAT + HYD_WATINJ_KEYWORDS_VALUE_FLOAT, line)
+            if potential_keyword is not None:
+                if found_waterinj and potential_keyword in HYD_WATINJ_KEYWORDS_VALUE_FLOAT:
+                    watinj_dict[potential_keyword] = float(
+                        nfo.get_expected_token_value(potential_keyword, line, file_as_list))
+                elif potential_keyword in HYD_KEYWORDS_VALUE_FLOAT:
+                    self.properties[potential_keyword] = float(
+                        nfo.get_expected_token_value(potential_keyword, line, file_as_list))
+
+            # Find standalone hydraulics keywords
+            potential_keyword = nfo.check_list_tokens(HYD_SINGLE_KEYWORDS, line)
+            if potential_keyword is not None:
+                self.properties[potential_keyword] = ''
+
+            # Find starting and ending indices for hydraulic limits table
+            if nfo.check_token('LIMITS', line):
+                hyd_table_indices['LIMITS'] = [line_indx+1, len(file_as_list)]
+                table_being_read['LIMITS'] = True
+                start_reading_table = True
+            if nfo.check_token('ENDLIMITS', line):
+                hyd_table_indices['LIMITS'][1] = line_indx
+                table_being_read['LIMITS'] = False
+                start_reading_table = False
+
+            # Find ending index of hydraulics table
+            if start_reading_table and table_being_read['HYD_TABLE']:
+                for potential_endkeyword in HYD_KEYWORDS:
+                    if nfo.check_token(potential_endkeyword, line):
+                        hyd_table_indices['HYD_TABLE'][1] = line_indx
+                        start_reading_table = False
+                        table_being_read['HYD_TABLE'] = False
+                        break
+            # Find starting index of hydraulics table
+            for header_keyword in HYD_TABLE_HEADER_COLS:
+                if nfo.check_token(header_keyword, line):
+                    hyd_table_indices['HYD_TABLE'] = [line_indx, len(file_as_list)]
+                    table_being_read['HYD_TABLE'] = True
+                    start_reading_table = True
+
+            line_indx += 1
+
+        # Read in hydraulics tables
+        for key in hyd_table_indices.keys():
+            if key == 'HYD_TABLE':
+                # Get hydraulic table data
+                hyd_df: pd.DataFrame = nfo.read_table_to_df(file_as_list[
+                    hyd_table_indices[key][0]+1:hyd_table_indices[key][1]], noheader=True)
+                # Resolve hydraulic table header
+                hyd_df_header_names = [header_name for header_name in file_as_list[
+                    hyd_table_indices[key][0]].split('!')[0].split() if not re.search('BHP', header_name)]
+                pressure_keyword_map = {'PIN': 'POUT', 'POUT': 'PIN', 'THP': 'BHP'}
+                hyd_table_pressure_key = ''  # Determines what type of pressures are in table, i.e., PIN, POUT or BHP
+                for pkey in HYD_PRESSURE_KEYWORDS:
+                    if pkey in self.properties.keys():
+                        hyd_table_pressure_key = pressure_keyword_map[pkey]
+                        break
+                hyd_df_header_names = hyd_df_header_names + \
+                    [hyd_table_pressure_key+str(i) for i in range(hyd_df.shape[1] - len(hyd_df_header_names))]
+                hyd_df.columns = hyd_df_header_names
+                # Set appropriate hydraulic table property
+                self.properties[key] = hyd_df
+            else:
+                self.properties[key] = nfo.read_table_to_df(file_as_list[
+                    hyd_table_indices[key][0]:hyd_table_indices[key][1]])
+
+        # Correctly set WATINJ properties, if needed
+        if found_waterinj:
+            self.properties['WATINJ'] = watinj_dict
```

### Comparing `ressimpy-1.0.0/ResSimpy/Nexus/DataModels/NexusPVTMethod.py` & `ressimpy-1.0.1/ResSimpy/Nexus/DataModels/NexusPVTMethod.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,455 +1,455 @@
-from dataclasses import dataclass, field
-from enum import Enum
-from typing import Optional, Union
-import pandas as pd
-from ResSimpy.Nexus.DataModels.NexusFile import NexusFile
-from ResSimpy.Nexus.NexusKeywords.pvt_keywords import PVT_BLACKOIL_PRIMARY_KEYWORDS, PVT_TYPE_KEYWORDS, PVT_KEYWORDS
-from ResSimpy.Nexus.NexusKeywords.pvt_keywords import PVT_EOS_METHODS, PVT_EOSOPTIONS_PRIMARY_WORDS
-from ResSimpy.Nexus.NexusKeywords.pvt_keywords import PVT_EOSOPTIONS_PRIMARY_KEYS_INT, PVT_TABLE_KEYWORDS
-from ResSimpy.Nexus.NexusKeywords.pvt_keywords import PVT_TABLES_WITH_ENDWORDS, PVT_TABLES_WITHOUT_ENDWORDS
-from ResSimpy.Nexus.NexusKeywords.pvt_keywords import PVT_EOSOPTIONS_PRIMARY_KEYS_FLOAT, PVT_EOSOPTIONS_TRANS_KEYS
-from ResSimpy.Nexus.NexusKeywords.pvt_keywords import PVT_EOSOPTIONS_TRANS_TEST_KEYS, PVT_EOSOPTIONS_PHASEID_KEYS
-from ResSimpy.Nexus.NexusKeywords.pvt_keywords import PVT_EOSOPTIONS_TERTIARY_KEYS, PVT_ALL_TABLE_KEYWORDS
-from ResSimpy.Nexus.NexusKeywords.pvt_keywords import PVT_UNSAT_TABLE_INDICES
-from ResSimpy.Enums.UnitsEnum import UnitSystem, SUnits, TemperatureUnits
-from ResSimpy.DynamicProperty import DynamicProperty
-
-from ResSimpy.Utils.factory_methods import get_empty_dict_union, get_empty_list_str, get_empty_eosopt_dict_union
-import ResSimpy.Nexus.nexus_file_operations as nfo
-
-
-@dataclass(kw_only=True, repr=False)  # Doesn't need to write an _init_, _eq_ methods, etc.
-class NexusPVTMethod(DynamicProperty):
-    """Class to hold Nexus PVT properties.
-
-    Attributes:
-        file (NexusFile): Nexus PVT file object
-        input_number (int): PVT method number in Nexus fcs file
-        pvt_type (Optional[str]): Type of PVT method, e.g., BLACKOIL, GASWATER or EOS. Defaults to None
-        eos_nhc (Optional[int]): Number of hydrocarbon components. Defaults to None
-        eos_temp (Optional[float]): Default temperature for EOS method. Defaults to None
-        eos_components (Optional[list[str]]): Specifies component names
-        eos_options (dict[str, Union[str, int, float, pd.DataFrame, list[str], dict[str, float],
-            tuple[str, dict[str, float]], dict[str, pd.DataFrame]]]): Dictionary containing various EOS options
-            as specified in the PVT file. Defaults to empty dictionary.
-        properties (dict[str, Union[str, int, float, Enum, list[str], pd.DataFrame,
-                    dict[str, Union[float, pd.DataFrame]]]]):
-            Dictionary holding all properties for a specific PVT method. Defaults to empty dictionary.
-    """
-
-    # General parameters
-    file: NexusFile
-    pvt_type: Optional[str] = None
-    eos_nhc: Optional[int] = None  # Number of hydrocarbon components
-    eos_temp: Optional[float] = None  # Default temperature for EOS method
-    eos_components: Optional[list[str]] = field(default_factory=get_empty_list_str)
-    eos_options: dict[str, Union[
-        str, int, float, pd.DataFrame, list[str], dict[str, float], tuple[str, dict[str, float]], dict[
-            str, pd.DataFrame]]] \
-        = field(default_factory=get_empty_eosopt_dict_union)
-    properties: dict[str, Union[str, int, float, Enum, list[str],
-                                pd.DataFrame, dict[str, Union[float, pd.DataFrame]]]] \
-        = field(default_factory=get_empty_dict_union)
-
-    def __init__(self, file: NexusFile, input_number: int, pvt_type: Optional[str] = None,
-                 eos_nhc: Optional[int] = None, eos_temp: Optional[float] = None,
-                 eos_components: Optional[list[str]] = None,
-                 eos_options: Optional[dict[str, Union[str, int, float, pd.DataFrame, list[str], dict[str, float],
-                                       tuple[str, dict[str, float]], dict[str, pd.DataFrame]]]] = None,
-                 properties: Optional[dict[str, Union[str, int, float, Enum, list[str], pd.DataFrame,
-                                      dict[str, Union[float, pd.DataFrame]]]]] = None) -> None:
-        if pvt_type is not None:
-            self.pvt_type = pvt_type
-        if eos_nhc is not None:
-            self.eos_nhc = eos_nhc
-        if eos_temp is not None:
-            self.eos_temp = eos_temp
-        if eos_components is not None:
-            self.eos_components = eos_components
-        else:
-            self.eos_components = []
-        if eos_options is not None:
-            self.eos_options = eos_options
-        else:
-            self.eos_options = {}
-        if properties is not None:
-            self.properties = properties
-        else:
-            self.properties = {}
-        super().__init__(input_number=input_number, file=file)
-
-    def to_string(self) -> str:
-        """Create string with PVT data in Nexus file format."""
-        printable_str = ''
-        pvt_dict = self.properties
-        # Print description if present
-        if 'DESC' in pvt_dict.keys() and isinstance(pvt_dict['DESC'], list):
-            for desc_line in pvt_dict['DESC']:
-                printable_str += 'DESC ' + desc_line + '\n'
-        # Print PVT type and associated properties
-        printable_str += f'{self.pvt_type}'
-        if self.eos_nhc is not None:
-            printable_str += f' NHC {self.eos_nhc}'
-        for pvt_key in PVT_BLACKOIL_PRIMARY_KEYWORDS:
-            if pvt_key in pvt_dict.keys():
-                printable_str += f' {pvt_key} {pvt_dict[pvt_key]}'
-        printable_str += '\n'
-        if 'DRYGAS_MFP' in pvt_dict.keys():
-            printable_str += 'DRYGAS_MFP\n'
-        # Print EOS-specific required parameters, if present
-        if self.eos_components is not None:
-            if len(self.eos_components) > 0:
-                printable_str += f"COMPONENTS {' '.join(self.eos_components)}\n"
-        if self.eos_temp is not None:
-            printable_str += f'TEMP {self.eos_temp}\n'
-        for key, value in pvt_dict.items():
-            if isinstance(value, pd.DataFrame):
-                printable_str += f'{key}\n'
-                if key == 'IGS_CP':
-                    printable_str += value.to_string(na_rep='', index=False, header=False) + '\n'
-                else:
-                    printable_str += value.to_string(na_rep='', index=False) + '\n'
-                if key in PVT_TABLES_WITH_ENDWORDS:
-                    printable_str += 'END'+key+'\n'
-                printable_str += '\n'
-            elif isinstance(value, dict):
-                for subkey in value.keys():
-                    printable_str += f"{key.replace('_',' ')} {subkey}\n"
-                    df = value[subkey]
-                    if isinstance(df, pd.DataFrame):
-                        printable_str += df.to_string(na_rep='', index=False) + '\n'
-                    printable_str += '\n'
-            elif isinstance(value, Enum):
-                if isinstance(value, UnitSystem) or isinstance(value, TemperatureUnits):
-                    printable_str += f'{value.value}\n'
-                elif isinstance(value, SUnits):
-                    printable_str += f'SUNITS {value.value}\n'
-            elif key not in [*PVT_BLACKOIL_PRIMARY_KEYWORDS, 'NHC', 'DESC', 'DRYGAS_MFP']:
-                if value == '':
-                    printable_str += f'{key}\n'
-                else:
-                    printable_str += f'{key} {value}\n'
-        if len(self.eos_options.keys()) > 0:
-            pvt_dict = self.eos_options
-            printable_str += 'EOSOPTIONS'
-            if 'EOS_METHOD' in pvt_dict.keys():
-                printable_str += f" {pvt_dict['EOS_METHOD']}"
-            printable_str += '\n'
-            for key, value in pvt_dict.items():
-                if key == 'EOS_OPT_PRIMARY_LIST' and isinstance(value, list):
-                    for token in value:
-                        printable_str += f'    {token}\n'
-                elif isinstance(value, tuple):
-                    printable_str += f'    {key} {value[0]}'
-                    val_dict: dict[str, float] = value[1]
-                    for val_key, val_val in val_dict.items():
-                        printable_str += f' {val_key} {val_val}'
-                    printable_str += '\n'
-                elif isinstance(value, dict):
-                    printable_str += f'    {key}'
-                    for subkey, subvalue in value.items():
-                        printable_str += f' {subkey} {subvalue}'
-                    printable_str += '\n'
-                elif key not in ['EOS_METHOD']:
-                    printable_str += f'    {key} {value}\n'
-        return printable_str
-
-    def __populate_eos_opts_to_tertiary_keys(self, primary_key: str, primary_key_default_val: str, single_line: str,
-                                             line_list: list[str], list_of_secondary_keys: list[str]):
-        """Utility function to populate complex EOS options structures, from primary to tertiary keyword level.
-        Applies to TRANSITION, TRANS_TEST and PHASEID Nexus EOS options.
-
-        Args:
-            primary_key (str): primary keyword, e.g., TRANSITION or PHASEID
-            primary_key_default_val (str): default secondary keyword, or primary key value, e.g., TEST
-            single_line (str): single line as read from input PVT file
-            line_list (list[str]): list of strings that comprise input PVT file
-            list_of_secondary_keys (list[str]): list of secondary keywords associated with the given primary keyword
-        """
-        if nfo.check_token(primary_key, single_line):
-            self.eos_options[primary_key] = primary_key_default_val  # Set default value
-            if nfo.get_expected_token_value(primary_key, single_line, line_list) in list_of_secondary_keys:
-                self.eos_options[primary_key] = nfo.get_expected_token_value(primary_key, single_line, line_list)
-        if [i for i in single_line.split() if i in list_of_secondary_keys]:
-            for secondary_key in list_of_secondary_keys:
-                if nfo.check_token(secondary_key, single_line):
-                    self.eos_options[primary_key] = secondary_key
-                    for tertiary_key in PVT_EOSOPTIONS_TERTIARY_KEYS:
-                        if nfo.check_token(tertiary_key, single_line):
-                            if isinstance(self.eos_options[primary_key], str):  # Convert to tuple
-                                self.eos_options[primary_key] = (secondary_key, {})
-
-                            secondary_eos_option = self.eos_options[primary_key]
-                            if type(secondary_eos_option) is not tuple or type(secondary_eos_option[1]) is not dict:
-                                raise ValueError(f"EOS secondary key invalid: {secondary_key}")
-                            secondary_eos_option[1][tertiary_key] = float(
-                                nfo.get_expected_token_value(tertiary_key, single_line, line_list))
-
-    def __find_pvt_table_starting_index(self, table_key: str, single_line: str, line_list: list[str],
-                                        table_indices: dict[str, list[int]],
-                                        table_indices_dict: dict[str, dict[str, list[int]]],
-                                        table_flag: dict[str, bool], l_index: int,
-                                        unsat_obj: dict[str, list[str]] = {}) -> Optional[int]:
-        """Utility function to find the starting line index of a specified PVT table.
-
-        Args:
-            table_key (str): specified PVT table name or undersaturated index, such as, PSAT or RSSAT or PRES
-            single_line (str): single line as read from input PVT file
-            line_list (list[str]): list of strings that comprise input PVT file
-            table_indices ([dict[str, list[int]]): dictionary to store the
-                starting and ending line index of tables
-            table_indices_dict (dict[str, dict[str, list[int]]]): dictionary to store the
-                starting and ending line index of tables, for undersaturated tables
-            table_flag (bool): flag to tell if a table is currently being read (True) or not (False)
-            l_index (int): current line index
-            unsat_obj (dict[str, list[str]]): track saturation pressures from which undersaturated branches emanate
-
-        Raises:
-            ValueError: If a property table key does not have a numerical value
-
-        Returns:
-            int: Updated line index
-        """
-        if table_key not in PVT_UNSAT_TABLE_INDICES:  # All tables except undersaturated tables
-            if nfo.check_token(table_key, single_line):
-                table_indices[table_key] = [l_index + 1, len(line_list)]
-                table_flag[table_key] = True
-                return l_index + 1
-        else:  # Handle undersaturated tables
-            if table_key == 'PRES':
-                table_name = 'UNSATGAS'
-                full_table_name = table_name + '_PRES'
-            else:
-                table_name = 'UNSATOIL'
-                full_table_name = table_name + '_' + table_key
-            if nfo.check_token(table_name, single_line) and nfo.check_token(table_key, single_line):
-                if nfo.get_token_value(table_key, single_line, line_list) is None:
-                    raise ValueError(f'Property {table_key} does not have a numerical value.')
-                unsat_obj[table_key].append(nfo.get_expected_token_value(table_key, single_line, line_list))
-                if full_table_name in table_indices_dict.keys():
-                    table_indices_dict[full_table_name][unsat_obj[table_key][-1]] = [l_index + 1, len(line_list)]
-                else:
-                    table_indices_dict[full_table_name] = {unsat_obj[table_key][-1]: [l_index + 1, len(line_list)]}
-                table_flag[table_name] = True
-                return l_index + 1
-        return None
-
-    def __find_pvt_table_ending_index(self, table_key: str, single_line: str,
-                                      table_indices: dict[str, list[int]],
-                                      table_indices_dict: dict[str, dict[str, list[int]]],
-                                      l_index: int, table_flag: dict[str, bool],
-                                      table_has_endkeyword: bool, reading_flag: bool,
-                                      unsat_obj: dict[str, list[str]] = {}) -> bool:
-        """Utility function to find the ending line index of a specified PVT table.
-
-        Args:
-            table_key (str): specified PVT table name or undersaturated index, such as, PSAT or RSSAT or PRES
-            single_line (str): single line as read from input PVT file
-            table_indices ([dict[str, list[int]]): dictionary to store the
-                starting and ending line index of tables
-            table_indices_dict (dict[str, dict[str, list[int]]]): dictionary to store the
-                starting and ending line index of tables, for undersaturated tables
-            l_index (int): current line index
-            table_flag (dict[str, bool]): flag to tell if a table is currently being read (True) or not (False)
-            table_has_endkeyword (bool): True if table name, e.g., PROPS, has end keyword, i.e., ENDPROPS, else False
-            reading_flag (bool): True if any table is being read, otherwise False
-            unsat_obj (dict[str, list[str]]): track saturation pressures from which undersaturated branches emanate
-
-        Returns:
-            bool: True if still reading table, but if identified the ending line index, return False
-        """
-        end_flag_found = False
-        if table_key not in PVT_UNSAT_TABLE_INDICES:  # All tables except undersaturated tables
-            table_name = table_key
-            full_table_name = table_key
-        else:  # Handle undersaturated tables
-            if table_key == 'PRES':
-                table_name = 'UNSATGAS'
-                full_table_name = table_name + '_PRES'
-            else:
-                table_name = 'UNSATOIL'
-                full_table_name = table_name + '_' + table_key
-        # if not table_has_endkeyword and [i for i in single_line.split() if i in PVT_KEYWORDS]:
-        if not table_has_endkeyword:
-            for keyword in PVT_KEYWORDS:
-                if nfo.check_token(keyword, single_line):
-                    end_flag_found = True
-        if table_has_endkeyword and nfo.check_token('END' + table_name, single_line):
-            end_flag_found = True
-        if (full_table_name in table_indices.keys() or full_table_name in table_indices_dict.keys()) and \
-                end_flag_found and table_flag[table_name]:
-            if table_key not in PVT_UNSAT_TABLE_INDICES:  # All tables except undersaturated tables
-                table_indices[table_name][1] = l_index
-            else:  # Handle undersaturated tables
-                table_indices_dict[full_table_name][unsat_obj[table_key][-1]][1] = l_index
-            table_flag[table_name] = False
-            reading_flag = False
-        return reading_flag
-
-    def read_properties(self) -> None:
-        """Read Nexus PVT file contents and populate the NexusPVTMethod object."""
-        file_as_list = self.file.get_flat_list_str_file
-
-        # Check for common input data
-        nfo.check_for_and_populate_common_input_data(file_as_list, self.properties)
-
-        # Initialize flags and containers used to record properties as we iterate through pvt file contents
-        # Dictionary to record start and ending indices for tables
-        pvt_table_indices: dict[str, list[int]] = {}
-        pvt_table_indices_dict: dict[str, dict[str, list[int]]] = {}
-        # Flag to tell when to start reading a table
-        start_reading_table: bool = False
-        trans_flag = False
-        # Dictionary of flags indicating which tables are being read
-        table_being_read: dict[str, bool] = {}
-        for table_name in PVT_ALL_TABLE_KEYWORDS:
-            table_being_read[table_name] = False
-        # Dictionary of lists to track saturation pressures from which undersaturated branches emanate
-        pvt_unsat_keys: dict[str, list[str]] = {}
-        for indx in PVT_UNSAT_TABLE_INDICES:
-            pvt_unsat_keys[indx] = []
-
-        line_indx = 0
-        for line in file_as_list:
-
-            # Determine PVT type, i.e., BLACKOIL, WATEROIL, EOS, etc.
-            for pvt_type in PVT_TYPE_KEYWORDS:
-                if nfo.check_token(pvt_type, line):
-                    self.pvt_type = pvt_type
-
-            # Extract blackoil fluid density parameters
-            for fluid_param in PVT_BLACKOIL_PRIMARY_KEYWORDS:
-                if nfo.check_token(fluid_param, line):
-                    self.properties[fluid_param] = float(nfo.get_expected_token_value(
-                        fluid_param, line, file_as_list, custom_message=f"Property {fluid_param} does \
-                        not have a numerical value."))
-            if nfo.check_token('DRYGAS_MFP', line):
-                self.properties['DRYGAS_MFP'] = True
-
-            # For EOS or compositional models, get required parameters
-            if nfo.check_token('NHC', line):  # Get number of components
-                self.eos_nhc = int(nfo.get_expected_token_value('NHC', line,
-                                                                file_as_list,
-                                                                custom_message="Property NHC does not \
-                                                                have a numerical value."))
-            if nfo.check_token('COMPONENTS', line):  # Get NHC components
-                elems = line.split()
-                components_index = elems.index('COMPONENTS')
-                if self.eos_nhc and self.eos_nhc > 0:
-                    self.eos_components = elems[components_index + 1:components_index + 1 + int(self.eos_nhc)]
-            if nfo.check_token('TEMP', line):  # Get default EOS temperature
-                self.eos_temp = float(nfo.get_expected_token_value(
-                    'TEMP', line, file_as_list, custom_message="Property TEMP does not have a numerical value."))
-
-            # Check for EOS options
-            if nfo.check_token('EOSOPTIONS', line):
-                if nfo.get_expected_token_value('EOSOPTIONS', line, file_as_list) in PVT_EOS_METHODS:
-                    self.eos_options['EOS_METHOD'] = nfo.get_expected_token_value('EOSOPTIONS', line, file_as_list)
-                else:
-                    self.eos_options['EOS_METHOD'] = 'PR'
-            # Find EOS single-word options, like CAPILLARYFLASH and add to list
-            if [i for i in line.split() if i in PVT_EOSOPTIONS_PRIMARY_WORDS]:
-                if 'EOS_OPT_PRIMARY_LIST' not in self.eos_options.keys():
-                    self.eos_options['EOS_OPT_PRIMARY_LIST'] = []
-                if not isinstance(self.eos_options['EOS_OPT_PRIMARY_LIST'], list):
-                    raise ValueError(f"EOS_OPT_PRIMARY_LIST should be a list, instead \
-                                     got {self.eos_options['EOS_OPT_PRIMARY_LIST']}")
-                self.eos_options['EOS_OPT_PRIMARY_LIST'].extend([i for i in line.split() if i
-                                                                 in PVT_EOSOPTIONS_PRIMARY_WORDS])
-            # Find EOS key-value pairs, like LI_FACT 0.9 or FUGERR 5
-            if [i for i in line.split() if i in PVT_EOSOPTIONS_PRIMARY_KEYS_FLOAT]:
-                for key in PVT_EOSOPTIONS_PRIMARY_KEYS_FLOAT:
-                    if nfo.check_token(key, line):
-                        self.eos_options[key] = float(nfo.get_expected_token_value(key, line, file_as_list))
-            if [i for i in line.split() if i in PVT_EOSOPTIONS_PRIMARY_KEYS_INT]:
-                for key in PVT_EOSOPTIONS_PRIMARY_KEYS_INT:
-                    if nfo.check_token(key, line):
-                        self.eos_options[key] = int(nfo.get_expected_token_value(key, line, file_as_list))
-            # Read TRANSITION, TRANS_TEST and PHASEID eos options, if present
-            primary_keys2populate = ['TRANSITION', 'TRANS_TEST', 'PHASEID']
-            primary_keys2populate_defaults = ['TEST', 'INCRP', '']
-            secondary_keys = [PVT_EOSOPTIONS_TRANS_KEYS, PVT_EOSOPTIONS_TRANS_TEST_KEYS, PVT_EOSOPTIONS_PHASEID_KEYS]
-            if [i for i in line.split() if i in primary_keys2populate]:
-                trans_flag = True
-            if trans_flag:
-                for index in range(len(primary_keys2populate)):
-                    pkey = primary_keys2populate[index]
-                    p2key = primary_keys2populate_defaults[index]
-                    sec_key = secondary_keys[index]
-                    self.__populate_eos_opts_to_tertiary_keys(pkey, p2key, line, file_as_list, sec_key)
-            # Read TRANS_OPTIMIZATION eos options, if present
-            if nfo.check_token('TRANS_OPTIMIZATION', line):
-                new_dict: dict[str, float] = {}
-                for tert_key in PVT_EOSOPTIONS_TERTIARY_KEYS:
-                    if nfo.check_token(tert_key, line):
-                        potential_value = float(nfo.get_expected_token_value(tert_key, line, file_as_list))
-                        if isinstance(potential_value, float):
-                            new_dict[tert_key] = potential_value
-                            self.eos_options['TRANS_OPTIMIZATION'] = new_dict
-
-            # Identify beginning and ending line indices for different kinds tables in PVT file
-            if start_reading_table:  # Figure out ending line indices for tables
-                for table in PVT_TABLES_WITHOUT_ENDWORDS:
-                    start_reading_table = self.__find_pvt_table_ending_index(table, line, pvt_table_indices,
-                                                                             pvt_table_indices_dict,
-                                                                             line_indx, table_being_read, False,
-                                                                             start_reading_table)
-                for table in PVT_TABLES_WITH_ENDWORDS:
-                    start_reading_table = self.__find_pvt_table_ending_index(table, line, pvt_table_indices,
-                                                                             pvt_table_indices_dict,
-                                                                             line_indx, table_being_read, True,
-                                                                             start_reading_table)
-                for table in PVT_UNSAT_TABLE_INDICES:
-                    start_reading_table = self.__find_pvt_table_ending_index(table, line, pvt_table_indices,
-                                                                             pvt_table_indices_dict,
-                                                                             line_indx, table_being_read, False,
-                                                                             start_reading_table, pvt_unsat_keys)
-            # Figure out beginning line indices for tables
-            table_found = False
-            for table in PVT_TABLE_KEYWORDS + PVT_UNSAT_TABLE_INDICES:
-                if table in PVT_UNSAT_TABLE_INDICES:  # Work on undersaturated tables
-                    new_line_indx = self.__find_pvt_table_starting_index(table, line, file_as_list, pvt_table_indices,
-                                                                         pvt_table_indices_dict, table_being_read,
-                                                                         line_indx, pvt_unsat_keys)
-                else:  # All other tables
-                    new_line_indx = self.__find_pvt_table_starting_index(table, line, file_as_list, pvt_table_indices,
-                                                                         pvt_table_indices_dict, table_being_read,
-                                                                         line_indx)
-                if new_line_indx is not None:
-                    line_indx = new_line_indx
-                    table_found = True
-                    break
-            if table_found:
-                continue
-            # Check if this line represents the header of a PVT table
-            table_header_row_options = ['PRES', 'DP', 'RV', 'INDEX', 'COMPONENT']
-            header_row_flag = False
-            for hr in table_header_row_options:
-                if nfo.check_token(hr, line):
-                    header_row_flag = True
-            reading_a_table_flag = False
-            for table_name in PVT_ALL_TABLE_KEYWORDS:
-                if table_being_read[table_name]:
-                    reading_a_table_flag = True
-            if header_row_flag and reading_a_table_flag and not start_reading_table:
-                start_reading_table = True  # If header row, start reading
-
-            line_indx += 1
-
-        # Read in tables
-        for key in pvt_table_indices.keys():
-            if key == 'IGS_CP':
-                self.properties[key] = nfo.read_table_to_df(file_as_list[
-                    pvt_table_indices[key][0]:pvt_table_indices[key][1]], noheader=True)
-            else:
-                self.properties[key] = nfo.read_table_to_df(file_as_list[
-                    pvt_table_indices[key][0]:pvt_table_indices[key][1]])
-        for key in pvt_table_indices_dict.keys():
-            self.properties[key] = {}
-            for subkey in pvt_table_indices_dict[key].keys():
-                property_key = self.properties[key]
-                if not isinstance(property_key, dict):
-                    raise ValueError(f"Property is not a dictionary: {str(self.properties[key])}")
-                property_key[subkey] = nfo.read_table_to_df(file_as_list[
-                                                            pvt_table_indices_dict[key][subkey][0]:
-                                                            pvt_table_indices_dict[key][subkey][1]])
+from dataclasses import dataclass, field
+from enum import Enum
+from typing import Optional, Union
+import pandas as pd
+from ResSimpy.Nexus.DataModels.NexusFile import NexusFile
+from ResSimpy.Nexus.NexusKeywords.pvt_keywords import PVT_BLACKOIL_PRIMARY_KEYWORDS, PVT_TYPE_KEYWORDS, PVT_KEYWORDS
+from ResSimpy.Nexus.NexusKeywords.pvt_keywords import PVT_EOS_METHODS, PVT_EOSOPTIONS_PRIMARY_WORDS
+from ResSimpy.Nexus.NexusKeywords.pvt_keywords import PVT_EOSOPTIONS_PRIMARY_KEYS_INT, PVT_TABLE_KEYWORDS
+from ResSimpy.Nexus.NexusKeywords.pvt_keywords import PVT_TABLES_WITH_ENDWORDS, PVT_TABLES_WITHOUT_ENDWORDS
+from ResSimpy.Nexus.NexusKeywords.pvt_keywords import PVT_EOSOPTIONS_PRIMARY_KEYS_FLOAT, PVT_EOSOPTIONS_TRANS_KEYS
+from ResSimpy.Nexus.NexusKeywords.pvt_keywords import PVT_EOSOPTIONS_TRANS_TEST_KEYS, PVT_EOSOPTIONS_PHASEID_KEYS
+from ResSimpy.Nexus.NexusKeywords.pvt_keywords import PVT_EOSOPTIONS_TERTIARY_KEYS, PVT_ALL_TABLE_KEYWORDS
+from ResSimpy.Nexus.NexusKeywords.pvt_keywords import PVT_UNSAT_TABLE_INDICES
+from ResSimpy.Enums.UnitsEnum import UnitSystem, SUnits, TemperatureUnits
+from ResSimpy.DynamicProperty import DynamicProperty
+
+from ResSimpy.Utils.factory_methods import get_empty_dict_union, get_empty_list_str, get_empty_eosopt_dict_union
+import ResSimpy.Nexus.nexus_file_operations as nfo
+
+
+@dataclass(kw_only=True, repr=False)  # Doesn't need to write an _init_, _eq_ methods, etc.
+class NexusPVTMethod(DynamicProperty):
+    """Class to hold Nexus PVT properties.
+
+    Attributes:
+        file (NexusFile): Nexus PVT file object
+        input_number (int): PVT method number in Nexus fcs file
+        pvt_type (Optional[str]): Type of PVT method, e.g., BLACKOIL, GASWATER or EOS. Defaults to None
+        eos_nhc (Optional[int]): Number of hydrocarbon components. Defaults to None
+        eos_temp (Optional[float]): Default temperature for EOS method. Defaults to None
+        eos_components (Optional[list[str]]): Specifies component names
+        eos_options (dict[str, Union[str, int, float, pd.DataFrame, list[str], dict[str, float],
+            tuple[str, dict[str, float]], dict[str, pd.DataFrame]]]): Dictionary containing various EOS options
+            as specified in the PVT file. Defaults to empty dictionary.
+        properties (dict[str, Union[str, int, float, Enum, list[str], pd.DataFrame,
+                    dict[str, Union[float, pd.DataFrame]]]]):
+            Dictionary holding all properties for a specific PVT method. Defaults to empty dictionary.
+    """
+
+    # General parameters
+    file: NexusFile
+    pvt_type: Optional[str] = None
+    eos_nhc: Optional[int] = None  # Number of hydrocarbon components
+    eos_temp: Optional[float] = None  # Default temperature for EOS method
+    eos_components: Optional[list[str]] = field(default_factory=get_empty_list_str)
+    eos_options: dict[str, Union[
+        str, int, float, pd.DataFrame, list[str], dict[str, float], tuple[str, dict[str, float]], dict[
+            str, pd.DataFrame]]] \
+        = field(default_factory=get_empty_eosopt_dict_union)
+    properties: dict[str, Union[str, int, float, Enum, list[str],
+                                pd.DataFrame, dict[str, Union[float, pd.DataFrame]]]] \
+        = field(default_factory=get_empty_dict_union)
+
+    def __init__(self, file: NexusFile, input_number: int, pvt_type: Optional[str] = None,
+                 eos_nhc: Optional[int] = None, eos_temp: Optional[float] = None,
+                 eos_components: Optional[list[str]] = None,
+                 eos_options: Optional[dict[str, Union[str, int, float, pd.DataFrame, list[str], dict[str, float],
+                                       tuple[str, dict[str, float]], dict[str, pd.DataFrame]]]] = None,
+                 properties: Optional[dict[str, Union[str, int, float, Enum, list[str], pd.DataFrame,
+                                      dict[str, Union[float, pd.DataFrame]]]]] = None) -> None:
+        if pvt_type is not None:
+            self.pvt_type = pvt_type
+        if eos_nhc is not None:
+            self.eos_nhc = eos_nhc
+        if eos_temp is not None:
+            self.eos_temp = eos_temp
+        if eos_components is not None:
+            self.eos_components = eos_components
+        else:
+            self.eos_components = []
+        if eos_options is not None:
+            self.eos_options = eos_options
+        else:
+            self.eos_options = {}
+        if properties is not None:
+            self.properties = properties
+        else:
+            self.properties = {}
+        super().__init__(input_number=input_number, file=file)
+
+    def to_string(self) -> str:
+        """Create string with PVT data in Nexus file format."""
+        printable_str = ''
+        pvt_dict = self.properties
+        # Print description if present
+        if 'DESC' in pvt_dict.keys() and isinstance(pvt_dict['DESC'], list):
+            for desc_line in pvt_dict['DESC']:
+                printable_str += 'DESC ' + desc_line + '\n'
+        # Print PVT type and associated properties
+        printable_str += f'{self.pvt_type}'
+        if self.eos_nhc is not None:
+            printable_str += f' NHC {self.eos_nhc}'
+        for pvt_key in PVT_BLACKOIL_PRIMARY_KEYWORDS:
+            if pvt_key in pvt_dict.keys():
+                printable_str += f' {pvt_key} {pvt_dict[pvt_key]}'
+        printable_str += '\n'
+        if 'DRYGAS_MFP' in pvt_dict.keys():
+            printable_str += 'DRYGAS_MFP\n'
+        # Print EOS-specific required parameters, if present
+        if self.eos_components is not None:
+            if len(self.eos_components) > 0:
+                printable_str += f"COMPONENTS {' '.join(self.eos_components)}\n"
+        if self.eos_temp is not None:
+            printable_str += f'TEMP {self.eos_temp}\n'
+        for key, value in pvt_dict.items():
+            if isinstance(value, pd.DataFrame):
+                printable_str += f'{key}\n'
+                if key == 'IGS_CP':
+                    printable_str += value.to_string(na_rep='', index=False, header=False) + '\n'
+                else:
+                    printable_str += value.to_string(na_rep='', index=False) + '\n'
+                if key in PVT_TABLES_WITH_ENDWORDS:
+                    printable_str += 'END'+key+'\n'
+                printable_str += '\n'
+            elif isinstance(value, dict):
+                for subkey in value.keys():
+                    printable_str += f"{key.replace('_',' ')} {subkey}\n"
+                    df = value[subkey]
+                    if isinstance(df, pd.DataFrame):
+                        printable_str += df.to_string(na_rep='', index=False) + '\n'
+                    printable_str += '\n'
+            elif isinstance(value, Enum):
+                if isinstance(value, UnitSystem) or isinstance(value, TemperatureUnits):
+                    printable_str += f'{value.value}\n'
+                elif isinstance(value, SUnits):
+                    printable_str += f'SUNITS {value.value}\n'
+            elif key not in [*PVT_BLACKOIL_PRIMARY_KEYWORDS, 'NHC', 'DESC', 'DRYGAS_MFP']:
+                if value == '':
+                    printable_str += f'{key}\n'
+                else:
+                    printable_str += f'{key} {value}\n'
+        if len(self.eos_options.keys()) > 0:
+            pvt_dict = self.eos_options
+            printable_str += 'EOSOPTIONS'
+            if 'EOS_METHOD' in pvt_dict.keys():
+                printable_str += f" {pvt_dict['EOS_METHOD']}"
+            printable_str += '\n'
+            for key, value in pvt_dict.items():
+                if key == 'EOS_OPT_PRIMARY_LIST' and isinstance(value, list):
+                    for token in value:
+                        printable_str += f'    {token}\n'
+                elif isinstance(value, tuple):
+                    printable_str += f'    {key} {value[0]}'
+                    val_dict: dict[str, float] = value[1]
+                    for val_key, val_val in val_dict.items():
+                        printable_str += f' {val_key} {val_val}'
+                    printable_str += '\n'
+                elif isinstance(value, dict):
+                    printable_str += f'    {key}'
+                    for subkey, subvalue in value.items():
+                        printable_str += f' {subkey} {subvalue}'
+                    printable_str += '\n'
+                elif key not in ['EOS_METHOD']:
+                    printable_str += f'    {key} {value}\n'
+        return printable_str
+
+    def __populate_eos_opts_to_tertiary_keys(self, primary_key: str, primary_key_default_val: str, single_line: str,
+                                             line_list: list[str], list_of_secondary_keys: list[str]):
+        """Utility function to populate complex EOS options structures, from primary to tertiary keyword level.
+        Applies to TRANSITION, TRANS_TEST and PHASEID Nexus EOS options.
+
+        Args:
+            primary_key (str): primary keyword, e.g., TRANSITION or PHASEID
+            primary_key_default_val (str): default secondary keyword, or primary key value, e.g., TEST
+            single_line (str): single line as read from input PVT file
+            line_list (list[str]): list of strings that comprise input PVT file
+            list_of_secondary_keys (list[str]): list of secondary keywords associated with the given primary keyword
+        """
+        if nfo.check_token(primary_key, single_line):
+            self.eos_options[primary_key] = primary_key_default_val  # Set default value
+            if nfo.get_expected_token_value(primary_key, single_line, line_list) in list_of_secondary_keys:
+                self.eos_options[primary_key] = nfo.get_expected_token_value(primary_key, single_line, line_list)
+        if [i for i in single_line.split() if i in list_of_secondary_keys]:
+            for secondary_key in list_of_secondary_keys:
+                if nfo.check_token(secondary_key, single_line):
+                    self.eos_options[primary_key] = secondary_key
+                    for tertiary_key in PVT_EOSOPTIONS_TERTIARY_KEYS:
+                        if nfo.check_token(tertiary_key, single_line):
+                            if isinstance(self.eos_options[primary_key], str):  # Convert to tuple
+                                self.eos_options[primary_key] = (secondary_key, {})
+
+                            secondary_eos_option = self.eos_options[primary_key]
+                            if type(secondary_eos_option) is not tuple or type(secondary_eos_option[1]) is not dict:
+                                raise ValueError(f"EOS secondary key invalid: {secondary_key}")
+                            secondary_eos_option[1][tertiary_key] = float(
+                                nfo.get_expected_token_value(tertiary_key, single_line, line_list))
+
+    def __find_pvt_table_starting_index(self, table_key: str, single_line: str, line_list: list[str],
+                                        table_indices: dict[str, list[int]],
+                                        table_indices_dict: dict[str, dict[str, list[int]]],
+                                        table_flag: dict[str, bool], l_index: int,
+                                        unsat_obj: dict[str, list[str]] = {}) -> Optional[int]:
+        """Utility function to find the starting line index of a specified PVT table.
+
+        Args:
+            table_key (str): specified PVT table name or undersaturated index, such as, PSAT or RSSAT or PRES
+            single_line (str): single line as read from input PVT file
+            line_list (list[str]): list of strings that comprise input PVT file
+            table_indices ([dict[str, list[int]]): dictionary to store the
+                starting and ending line index of tables
+            table_indices_dict (dict[str, dict[str, list[int]]]): dictionary to store the
+                starting and ending line index of tables, for undersaturated tables
+            table_flag (bool): flag to tell if a table is currently being read (True) or not (False)
+            l_index (int): current line index
+            unsat_obj (dict[str, list[str]]): track saturation pressures from which undersaturated branches emanate
+
+        Raises:
+            ValueError: If a property table key does not have a numerical value
+
+        Returns:
+            int: Updated line index
+        """
+        if table_key not in PVT_UNSAT_TABLE_INDICES:  # All tables except undersaturated tables
+            if nfo.check_token(table_key, single_line):
+                table_indices[table_key] = [l_index + 1, len(line_list)]
+                table_flag[table_key] = True
+                return l_index + 1
+        else:  # Handle undersaturated tables
+            if table_key == 'PRES':
+                table_name = 'UNSATGAS'
+                full_table_name = table_name + '_PRES'
+            else:
+                table_name = 'UNSATOIL'
+                full_table_name = table_name + '_' + table_key
+            if nfo.check_token(table_name, single_line) and nfo.check_token(table_key, single_line):
+                if nfo.get_token_value(table_key, single_line, line_list) is None:
+                    raise ValueError(f'Property {table_key} does not have a numerical value.')
+                unsat_obj[table_key].append(nfo.get_expected_token_value(table_key, single_line, line_list))
+                if full_table_name in table_indices_dict.keys():
+                    table_indices_dict[full_table_name][unsat_obj[table_key][-1]] = [l_index + 1, len(line_list)]
+                else:
+                    table_indices_dict[full_table_name] = {unsat_obj[table_key][-1]: [l_index + 1, len(line_list)]}
+                table_flag[table_name] = True
+                return l_index + 1
+        return None
+
+    def __find_pvt_table_ending_index(self, table_key: str, single_line: str,
+                                      table_indices: dict[str, list[int]],
+                                      table_indices_dict: dict[str, dict[str, list[int]]],
+                                      l_index: int, table_flag: dict[str, bool],
+                                      table_has_endkeyword: bool, reading_flag: bool,
+                                      unsat_obj: dict[str, list[str]] = {}) -> bool:
+        """Utility function to find the ending line index of a specified PVT table.
+
+        Args:
+            table_key (str): specified PVT table name or undersaturated index, such as, PSAT or RSSAT or PRES
+            single_line (str): single line as read from input PVT file
+            table_indices ([dict[str, list[int]]): dictionary to store the
+                starting and ending line index of tables
+            table_indices_dict (dict[str, dict[str, list[int]]]): dictionary to store the
+                starting and ending line index of tables, for undersaturated tables
+            l_index (int): current line index
+            table_flag (dict[str, bool]): flag to tell if a table is currently being read (True) or not (False)
+            table_has_endkeyword (bool): True if table name, e.g., PROPS, has end keyword, i.e., ENDPROPS, else False
+            reading_flag (bool): True if any table is being read, otherwise False
+            unsat_obj (dict[str, list[str]]): track saturation pressures from which undersaturated branches emanate
+
+        Returns:
+            bool: True if still reading table, but if identified the ending line index, return False
+        """
+        end_flag_found = False
+        if table_key not in PVT_UNSAT_TABLE_INDICES:  # All tables except undersaturated tables
+            table_name = table_key
+            full_table_name = table_key
+        else:  # Handle undersaturated tables
+            if table_key == 'PRES':
+                table_name = 'UNSATGAS'
+                full_table_name = table_name + '_PRES'
+            else:
+                table_name = 'UNSATOIL'
+                full_table_name = table_name + '_' + table_key
+        # if not table_has_endkeyword and [i for i in single_line.split() if i in PVT_KEYWORDS]:
+        if not table_has_endkeyword:
+            for keyword in PVT_KEYWORDS:
+                if nfo.check_token(keyword, single_line):
+                    end_flag_found = True
+        if table_has_endkeyword and nfo.check_token('END' + table_name, single_line):
+            end_flag_found = True
+        if (full_table_name in table_indices.keys() or full_table_name in table_indices_dict.keys()) and \
+                end_flag_found and table_flag[table_name]:
+            if table_key not in PVT_UNSAT_TABLE_INDICES:  # All tables except undersaturated tables
+                table_indices[table_name][1] = l_index
+            else:  # Handle undersaturated tables
+                table_indices_dict[full_table_name][unsat_obj[table_key][-1]][1] = l_index
+            table_flag[table_name] = False
+            reading_flag = False
+        return reading_flag
+
+    def read_properties(self) -> None:
+        """Read Nexus PVT file contents and populate the NexusPVTMethod object."""
+        file_as_list = self.file.get_flat_list_str_file
+
+        # Check for common input data
+        nfo.check_for_and_populate_common_input_data(file_as_list, self.properties)
+
+        # Initialize flags and containers used to record properties as we iterate through pvt file contents
+        # Dictionary to record start and ending indices for tables
+        pvt_table_indices: dict[str, list[int]] = {}
+        pvt_table_indices_dict: dict[str, dict[str, list[int]]] = {}
+        # Flag to tell when to start reading a table
+        start_reading_table: bool = False
+        trans_flag = False
+        # Dictionary of flags indicating which tables are being read
+        table_being_read: dict[str, bool] = {}
+        for table_name in PVT_ALL_TABLE_KEYWORDS:
+            table_being_read[table_name] = False
+        # Dictionary of lists to track saturation pressures from which undersaturated branches emanate
+        pvt_unsat_keys: dict[str, list[str]] = {}
+        for indx in PVT_UNSAT_TABLE_INDICES:
+            pvt_unsat_keys[indx] = []
+
+        line_indx = 0
+        for line in file_as_list:
+
+            # Determine PVT type, i.e., BLACKOIL, WATEROIL, EOS, etc.
+            for pvt_type in PVT_TYPE_KEYWORDS:
+                if nfo.check_token(pvt_type, line):
+                    self.pvt_type = pvt_type
+
+            # Extract blackoil fluid density parameters
+            for fluid_param in PVT_BLACKOIL_PRIMARY_KEYWORDS:
+                if nfo.check_token(fluid_param, line):
+                    self.properties[fluid_param] = float(nfo.get_expected_token_value(
+                        fluid_param, line, file_as_list, custom_message=f"Property {fluid_param} does \
+                        not have a numerical value."))
+            if nfo.check_token('DRYGAS_MFP', line):
+                self.properties['DRYGAS_MFP'] = True
+
+            # For EOS or compositional models, get required parameters
+            if nfo.check_token('NHC', line):  # Get number of components
+                self.eos_nhc = int(nfo.get_expected_token_value('NHC', line,
+                                                                file_as_list,
+                                                                custom_message="Property NHC does not \
+                                                                have a numerical value."))
+            if nfo.check_token('COMPONENTS', line):  # Get NHC components
+                elems = line.split()
+                components_index = elems.index('COMPONENTS')
+                if self.eos_nhc and self.eos_nhc > 0:
+                    self.eos_components = elems[components_index + 1:components_index + 1 + int(self.eos_nhc)]
+            if nfo.check_token('TEMP', line):  # Get default EOS temperature
+                self.eos_temp = float(nfo.get_expected_token_value(
+                    'TEMP', line, file_as_list, custom_message="Property TEMP does not have a numerical value."))
+
+            # Check for EOS options
+            if nfo.check_token('EOSOPTIONS', line):
+                if nfo.get_expected_token_value('EOSOPTIONS', line, file_as_list) in PVT_EOS_METHODS:
+                    self.eos_options['EOS_METHOD'] = nfo.get_expected_token_value('EOSOPTIONS', line, file_as_list)
+                else:
+                    self.eos_options['EOS_METHOD'] = 'PR'
+            # Find EOS single-word options, like CAPILLARYFLASH and add to list
+            if [i for i in line.split() if i in PVT_EOSOPTIONS_PRIMARY_WORDS]:
+                if 'EOS_OPT_PRIMARY_LIST' not in self.eos_options.keys():
+                    self.eos_options['EOS_OPT_PRIMARY_LIST'] = []
+                if not isinstance(self.eos_options['EOS_OPT_PRIMARY_LIST'], list):
+                    raise ValueError(f"EOS_OPT_PRIMARY_LIST should be a list, instead \
+                                     got {self.eos_options['EOS_OPT_PRIMARY_LIST']}")
+                self.eos_options['EOS_OPT_PRIMARY_LIST'].extend([i for i in line.split() if i
+                                                                 in PVT_EOSOPTIONS_PRIMARY_WORDS])
+            # Find EOS key-value pairs, like LI_FACT 0.9 or FUGERR 5
+            if [i for i in line.split() if i in PVT_EOSOPTIONS_PRIMARY_KEYS_FLOAT]:
+                for key in PVT_EOSOPTIONS_PRIMARY_KEYS_FLOAT:
+                    if nfo.check_token(key, line):
+                        self.eos_options[key] = float(nfo.get_expected_token_value(key, line, file_as_list))
+            if [i for i in line.split() if i in PVT_EOSOPTIONS_PRIMARY_KEYS_INT]:
+                for key in PVT_EOSOPTIONS_PRIMARY_KEYS_INT:
+                    if nfo.check_token(key, line):
+                        self.eos_options[key] = int(nfo.get_expected_token_value(key, line, file_as_list))
+            # Read TRANSITION, TRANS_TEST and PHASEID eos options, if present
+            primary_keys2populate = ['TRANSITION', 'TRANS_TEST', 'PHASEID']
+            primary_keys2populate_defaults = ['TEST', 'INCRP', '']
+            secondary_keys = [PVT_EOSOPTIONS_TRANS_KEYS, PVT_EOSOPTIONS_TRANS_TEST_KEYS, PVT_EOSOPTIONS_PHASEID_KEYS]
+            if [i for i in line.split() if i in primary_keys2populate]:
+                trans_flag = True
+            if trans_flag:
+                for index in range(len(primary_keys2populate)):
+                    pkey = primary_keys2populate[index]
+                    p2key = primary_keys2populate_defaults[index]
+                    sec_key = secondary_keys[index]
+                    self.__populate_eos_opts_to_tertiary_keys(pkey, p2key, line, file_as_list, sec_key)
+            # Read TRANS_OPTIMIZATION eos options, if present
+            if nfo.check_token('TRANS_OPTIMIZATION', line):
+                new_dict: dict[str, float] = {}
+                for tert_key in PVT_EOSOPTIONS_TERTIARY_KEYS:
+                    if nfo.check_token(tert_key, line):
+                        potential_value = float(nfo.get_expected_token_value(tert_key, line, file_as_list))
+                        if isinstance(potential_value, float):
+                            new_dict[tert_key] = potential_value
+                            self.eos_options['TRANS_OPTIMIZATION'] = new_dict
+
+            # Identify beginning and ending line indices for different kinds tables in PVT file
+            if start_reading_table:  # Figure out ending line indices for tables
+                for table in PVT_TABLES_WITHOUT_ENDWORDS:
+                    start_reading_table = self.__find_pvt_table_ending_index(table, line, pvt_table_indices,
+                                                                             pvt_table_indices_dict,
+                                                                             line_indx, table_being_read, False,
+                                                                             start_reading_table)
+                for table in PVT_TABLES_WITH_ENDWORDS:
+                    start_reading_table = self.__find_pvt_table_ending_index(table, line, pvt_table_indices,
+                                                                             pvt_table_indices_dict,
+                                                                             line_indx, table_being_read, True,
+                                                                             start_reading_table)
+                for table in PVT_UNSAT_TABLE_INDICES:
+                    start_reading_table = self.__find_pvt_table_ending_index(table, line, pvt_table_indices,
+                                                                             pvt_table_indices_dict,
+                                                                             line_indx, table_being_read, False,
+                                                                             start_reading_table, pvt_unsat_keys)
+            # Figure out beginning line indices for tables
+            table_found = False
+            for table in PVT_TABLE_KEYWORDS + PVT_UNSAT_TABLE_INDICES:
+                if table in PVT_UNSAT_TABLE_INDICES:  # Work on undersaturated tables
+                    new_line_indx = self.__find_pvt_table_starting_index(table, line, file_as_list, pvt_table_indices,
+                                                                         pvt_table_indices_dict, table_being_read,
+                                                                         line_indx, pvt_unsat_keys)
+                else:  # All other tables
+                    new_line_indx = self.__find_pvt_table_starting_index(table, line, file_as_list, pvt_table_indices,
+                                                                         pvt_table_indices_dict, table_being_read,
+                                                                         line_indx)
+                if new_line_indx is not None:
+                    line_indx = new_line_indx
+                    table_found = True
+                    break
+            if table_found:
+                continue
+            # Check if this line represents the header of a PVT table
+            table_header_row_options = ['PRES', 'DP', 'RV', 'INDEX', 'COMPONENT']
+            header_row_flag = False
+            for hr in table_header_row_options:
+                if nfo.check_token(hr, line):
+                    header_row_flag = True
+            reading_a_table_flag = False
+            for table_name in PVT_ALL_TABLE_KEYWORDS:
+                if table_being_read[table_name]:
+                    reading_a_table_flag = True
+            if header_row_flag and reading_a_table_flag and not start_reading_table:
+                start_reading_table = True  # If header row, start reading
+
+            line_indx += 1
+
+        # Read in tables
+        for key in pvt_table_indices.keys():
+            if key == 'IGS_CP':
+                self.properties[key] = nfo.read_table_to_df(file_as_list[
+                    pvt_table_indices[key][0]:pvt_table_indices[key][1]], noheader=True)
+            else:
+                self.properties[key] = nfo.read_table_to_df(file_as_list[
+                    pvt_table_indices[key][0]:pvt_table_indices[key][1]])
+        for key in pvt_table_indices_dict.keys():
+            self.properties[key] = {}
+            for subkey in pvt_table_indices_dict[key].keys():
+                property_key = self.properties[key]
+                if not isinstance(property_key, dict):
+                    raise ValueError(f"Property is not a dictionary: {str(self.properties[key])}")
+                property_key[subkey] = nfo.read_table_to_df(file_as_list[
+                                                            pvt_table_indices_dict[key][subkey][0]:
+                                                            pvt_table_indices_dict[key][subkey][1]])
```

### Comparing `ressimpy-1.0.0/ResSimpy/Nexus/DataModels/NexusRelPermEndPoint.py` & `ressimpy-1.0.1/ResSimpy/Nexus/DataModels/NexusRelPermEndPoint.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,48 +1,48 @@
-from dataclasses import dataclass
-from typing import Optional
-from ResSimpy.RelPermEndPoint import RelPermEndPoint
-
-
-@dataclass
-class NexusRelPermEndPoint(RelPermEndPoint):
-    def __init__(self, swl: Optional[float] = None, swr: Optional[float] = None, swu: Optional[float] = None,
-                 sgl: Optional[float] = None, sgr: Optional[float] = None, sgu: Optional[float] = None,
-                 swro: Optional[float] = None, sgro: Optional[float] = None, sgrw: Optional[float] = None,
-                 krw_swro: Optional[float] = None, krw_swu: Optional[float] = None, krg_sgro: Optional[float] = None,
-                 krg_sgu: Optional[float] = None, kro_swl: Optional[float] = None, kro_swr: Optional[float] = None,
-                 kro_sgl: Optional[float] = None, kro_sgr: Optional[float] = None, krw_sgl: Optional[float] = None,
-                 krw_sgr: Optional[float] = None, krg_sgrw: Optional[float] = None, sgtr: Optional[float] = None,
-                 sotr: Optional[float] = None) -> None:
-        super().__init__(swl=swl, swr=swr, swu=swu, sgl=sgl, sgr=sgr, sgu=sgu, swro=swro, sgro=sgro,
-                         sgrw=sgrw, krw_swro=krw_swro, krw_swu=krw_swu, krg_sgro=krg_sgro, krg_sgu=krg_sgu,
-                         kro_swl=kro_swl, kro_swr=kro_swr, kro_sgl=kro_sgl, kro_sgr=kro_sgr, krw_sgl=krw_sgl,
-                         krw_sgr=krw_sgr, krg_sgrw=krg_sgrw, sgtr=sgtr, sotr=sotr)
-
-    @staticmethod
-    def nexus_mapping() -> dict[str, tuple[str, type]]:
-        """Returns a dictionary of mapping from nexus keyword to attribute name."""
-        nexus_mapping: dict[str, tuple[str, type]] = {
-            'SWL': ('swl', float),
-            'SWR': ('swr', float),
-            'SWU': ('swu', float),
-            'SGL': ('sgl', float),
-            'SGR': ('sgr', float),
-            'SGU': ('sgu', float),
-            'SWRO': ('swro', float),
-            'SGRO': ('sgro', float),
-            'SGRW': ('sgrw', float),
-            'KRW_SWRO': ('krw_swro', float),
-            'KRW_SWU': ('krw_swu', float),
-            'KRG_SGRO': ('krg_sgro', float),
-            'KRG_SGU': ('krg_sgu', float),
-            'KRO_SWL': ('kro_swl', float),
-            'KRO_SWR': ('kro_swr', float),
-            'KRO_SGL': ('kro_sgl', float),
-            'KRO_SGR': ('kro_sgr', float),
-            'KRW_SGL': ('krw_sgl', float),
-            'KRW_SGR': ('krw_sgr', float),
-            'KRG_SGRW': ('krg_sgrw', float),
-            'SGTR': ('sgtr', float),
-            'SOTR': ('sotr', float),
-        }
-        return nexus_mapping
+from dataclasses import dataclass
+from typing import Optional
+from ResSimpy.RelPermEndPoint import RelPermEndPoint
+
+
+@dataclass
+class NexusRelPermEndPoint(RelPermEndPoint):
+    def __init__(self, swl: Optional[float] = None, swr: Optional[float] = None, swu: Optional[float] = None,
+                 sgl: Optional[float] = None, sgr: Optional[float] = None, sgu: Optional[float] = None,
+                 swro: Optional[float] = None, sgro: Optional[float] = None, sgrw: Optional[float] = None,
+                 krw_swro: Optional[float] = None, krw_swu: Optional[float] = None, krg_sgro: Optional[float] = None,
+                 krg_sgu: Optional[float] = None, kro_swl: Optional[float] = None, kro_swr: Optional[float] = None,
+                 kro_sgl: Optional[float] = None, kro_sgr: Optional[float] = None, krw_sgl: Optional[float] = None,
+                 krw_sgr: Optional[float] = None, krg_sgrw: Optional[float] = None, sgtr: Optional[float] = None,
+                 sotr: Optional[float] = None) -> None:
+        super().__init__(swl=swl, swr=swr, swu=swu, sgl=sgl, sgr=sgr, sgu=sgu, swro=swro, sgro=sgro,
+                         sgrw=sgrw, krw_swro=krw_swro, krw_swu=krw_swu, krg_sgro=krg_sgro, krg_sgu=krg_sgu,
+                         kro_swl=kro_swl, kro_swr=kro_swr, kro_sgl=kro_sgl, kro_sgr=kro_sgr, krw_sgl=krw_sgl,
+                         krw_sgr=krw_sgr, krg_sgrw=krg_sgrw, sgtr=sgtr, sotr=sotr)
+
+    @staticmethod
+    def nexus_mapping() -> dict[str, tuple[str, type]]:
+        """Returns a dictionary of mapping from nexus keyword to attribute name."""
+        nexus_mapping: dict[str, tuple[str, type]] = {
+            'SWL': ('swl', float),
+            'SWR': ('swr', float),
+            'SWU': ('swu', float),
+            'SGL': ('sgl', float),
+            'SGR': ('sgr', float),
+            'SGU': ('sgu', float),
+            'SWRO': ('swro', float),
+            'SGRO': ('sgro', float),
+            'SGRW': ('sgrw', float),
+            'KRW_SWRO': ('krw_swro', float),
+            'KRW_SWU': ('krw_swu', float),
+            'KRG_SGRO': ('krg_sgro', float),
+            'KRG_SGU': ('krg_sgu', float),
+            'KRO_SWL': ('kro_swl', float),
+            'KRO_SWR': ('kro_swr', float),
+            'KRO_SGL': ('kro_sgl', float),
+            'KRO_SGR': ('kro_sgr', float),
+            'KRW_SGL': ('krw_sgl', float),
+            'KRW_SGR': ('krw_sgr', float),
+            'KRG_SGRW': ('krg_sgrw', float),
+            'SGTR': ('sgtr', float),
+            'SOTR': ('sotr', float),
+        }
+        return nexus_mapping
```

### Comparing `ressimpy-1.0.0/ResSimpy/Nexus/DataModels/NexusRockMethod.py` & `ressimpy-1.0.1/ResSimpy/Nexus/DataModels/NexusRockMethod.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,155 +1,155 @@
-from dataclasses import dataclass, field
-from enum import Enum
-from typing import Optional, Union
-import pandas as pd
-from ResSimpy.Nexus.DataModels.NexusFile import NexusFile
-from ResSimpy.Nexus.NexusKeywords.rock_keywords import ROCK_ALL_TABLE_KEYWORDS, ROCK_KEYWORDS_VALUE_FLOAT
-from ResSimpy.Nexus.NexusKeywords.rock_keywords import ROCK_SINGLE_KEYWORDS, ROCK_KEYWORDS_VALUE_STR
-from ResSimpy.Nexus.NexusKeywords.rock_keywords import ROCK_KEYWORDS, ROCK_REV_IRREV_OPTIONS
-from ResSimpy.DynamicProperty import DynamicProperty
-from ResSimpy.Enums.UnitsEnum import UnitSystem, SUnits, TemperatureUnits
-from ResSimpy.Utils.factory_methods import get_empty_dict_union
-import ResSimpy.Nexus.nexus_file_operations as nfo
-
-
-@dataclass(kw_only=True, repr=False)  # Doesn't need to write an _init_, _eq_ methods, etc.
-class NexusRockMethod(DynamicProperty):
-    """Class to hold Nexus Rock properties.
-
-    Attributes:
-        file (NexusFile): Nexus rock properties file object
-        input_number (int): Rock properties method number in Nexus fcs file
-        properties (dict[str, Union[str, int, float, Enum, list[str], pd.DataFrame,
-                    dict[str, Union[float, pd.DataFrame]]]]):
-            Dictionary holding all properties for a specific rock properties method. Defaults to empty dictionary.
-    """
-
-    # General parameters
-    file: NexusFile
-    properties: dict[str, Union[str, int, float, Enum, list[str], pd.DataFrame,
-                                dict[str, Union[float, pd.DataFrame]]]] = field(default_factory=get_empty_dict_union)
-
-    def __init__(self, file: NexusFile, input_number: int,
-                 properties: Optional[dict[str, Union[str, int, float, Enum, list[str], pd.DataFrame,
-                                                      dict[str, Union[float, pd.DataFrame]]]]] = None) -> None:
-        if properties is not None:
-            self.properties = properties
-        else:
-            self.properties = {}
-        super().__init__(input_number=input_number, file=file)
-
-    def to_string(self) -> str:
-        """Create string with rock properties data, in Nexus file format."""
-        printable_str = ''
-        rock_dict = self.properties
-        for key, value in rock_dict.items():
-            if key == 'DESC' and isinstance(value, list):
-                for desc_line in value:
-                    printable_str += 'DESC ' + desc_line + '\n'
-            elif isinstance(value, pd.DataFrame):
-                printable_str += f'{key}\n'
-                printable_str += value.to_string(na_rep='', index=False) + '\n\n'
-            elif isinstance(value, dict):
-                printable_str += f"{key.replace('_',' ')}\n"
-                for subkey in value.keys():
-                    printable_str += f"SWINIT {subkey}\n"
-                    df = value[subkey]
-                    if isinstance(df, pd.DataFrame):
-                        printable_str += df.to_string(na_rep='', index=False) + '\n'
-                    printable_str += '\n'
-            elif isinstance(value, Enum):
-                if isinstance(value, UnitSystem) or isinstance(value, TemperatureUnits):
-                    printable_str += f'{value.value}\n'
-                elif isinstance(value, SUnits):
-                    printable_str += f'SUNITS {value.value}\n'
-            elif value == '':
-                printable_str += f'{key}\n'
-            else:
-                printable_str += f'{key} {value}\n'
-        return printable_str
-
-    def read_properties(self) -> None:
-        """Read Nexus rock properties file contents and populate NexusRockMethod object."""
-        file_as_list = self.file.get_flat_list_str_file
-
-        # Check for common input data
-        nfo.check_for_and_populate_common_input_data(file_as_list, self.properties)
-
-        # Initialize properties
-        cmt_indices: list[int] = []
-        wirct_indices_dict: dict[str, dict[str, list[int]]] = {}
-        # Flag to tell when to start reading a table
-        start_reading_table: bool = False
-        swinit_key = ''
-        # Dictionary of flags indicating which tables are being read
-        table_being_read: dict[str, bool] = {}
-        for table_name in ROCK_ALL_TABLE_KEYWORDS:
-            table_being_read[table_name] = False
-
-        line_indx = 0
-        for line in file_as_list:
-
-            # Find ROCK key-value pairs, such as PREF 2000 or CR 1e-6
-            if [i for i in line.split() if i in ROCK_KEYWORDS_VALUE_FLOAT]:
-                for key in ROCK_KEYWORDS_VALUE_FLOAT:
-                    if nfo.check_token(key, line):
-                        self.properties[key] = float(nfo.get_expected_token_value(key, line, file_as_list))
-            # Find standalone rock property keywords, such as COMPR or KPMULT
-            if [i for i in line.split() if i in ROCK_SINGLE_KEYWORDS]:
-                for word in ROCK_SINGLE_KEYWORDS:
-                    if nfo.check_token(word, line):
-                        self.properties[word] = ''
-            # Handle REVERSIBLE or IRREVERSIBLE keywords
-            if [i for i in line.split() if i in ROCK_KEYWORDS_VALUE_STR]:
-                for key in ROCK_KEYWORDS_VALUE_STR:
-                    if nfo.check_token(key, line):
-                        if nfo.get_token_value(key, line, file_as_list) in ROCK_REV_IRREV_OPTIONS:
-                            self.properties[key] = nfo.get_expected_token_value(key, line, file_as_list)
-                        else:
-                            self.properties[key] = ''
-            # Find starting index of rock compaction table
-            if nfo.check_token('CMT', line):
-                cmt_indices = [line_indx + 1, len(file_as_list)]
-                table_being_read['CMT'] = True
-                start_reading_table = True
-                line_indx += 1
-                continue
-            # Find ending index of rock compaction table
-            if start_reading_table and table_being_read['CMT']:
-                for potential_endkeyword in ROCK_KEYWORDS:
-                    if nfo.check_token(potential_endkeyword, line):
-                        cmt_indices[1] = line_indx
-                        start_reading_table = False
-                        table_being_read['CMT'] = False
-                        break
-            # Find ending index of a water-induced rock compaction table
-            if start_reading_table and table_being_read['WIRCT']:
-                for potential_endkeyword in ROCK_KEYWORDS:
-                    if nfo.check_token(potential_endkeyword, line):
-                        wirct_indices_dict['WIRCT'][swinit_key][1] = line_indx
-                        start_reading_table = False
-                        table_being_read['WIRCT'] = False
-                        break
-            # Find starting index of a water-induced rock compaction table
-            if nfo.check_token('WIRCT', line):
-                wirct_indices_dict['WIRCT'] = {}
-            if nfo.check_token('SWINIT', line):
-                swinit_key = nfo.get_expected_token_value('SWINIT', line, file_as_list)
-                wirct_indices_dict['WIRCT'][swinit_key] = [line_indx+1, len(file_as_list)]
-                table_being_read['WIRCT'] = True
-                start_reading_table = True
-
-            line_indx += 1
-
-        # Read in compaction table(s) if there are any
-        if len(cmt_indices) > 0:
-            self.properties['CMT'] = nfo.read_table_to_df(file_as_list[cmt_indices[0]:cmt_indices[1]])
-        for key in wirct_indices_dict.keys():
-            self.properties[key] = {}
-            for subkey in wirct_indices_dict[key].keys():
-                property_key = self.properties[key]
-                if not isinstance(property_key, dict):
-                    raise ValueError(f"Property is not a dictionary: {str(self.properties[key])}")
-                property_key[subkey] = nfo.read_table_to_df(file_as_list[
-                                                            wirct_indices_dict[key][subkey][0]:
-                                                            wirct_indices_dict[key][subkey][1]])
+from dataclasses import dataclass, field
+from enum import Enum
+from typing import Optional, Union
+import pandas as pd
+from ResSimpy.Nexus.DataModels.NexusFile import NexusFile
+from ResSimpy.Nexus.NexusKeywords.rock_keywords import ROCK_ALL_TABLE_KEYWORDS, ROCK_KEYWORDS_VALUE_FLOAT
+from ResSimpy.Nexus.NexusKeywords.rock_keywords import ROCK_SINGLE_KEYWORDS, ROCK_KEYWORDS_VALUE_STR
+from ResSimpy.Nexus.NexusKeywords.rock_keywords import ROCK_KEYWORDS, ROCK_REV_IRREV_OPTIONS
+from ResSimpy.DynamicProperty import DynamicProperty
+from ResSimpy.Enums.UnitsEnum import UnitSystem, SUnits, TemperatureUnits
+from ResSimpy.Utils.factory_methods import get_empty_dict_union
+import ResSimpy.Nexus.nexus_file_operations as nfo
+
+
+@dataclass(kw_only=True, repr=False)  # Doesn't need to write an _init_, _eq_ methods, etc.
+class NexusRockMethod(DynamicProperty):
+    """Class to hold Nexus Rock properties.
+
+    Attributes:
+        file (NexusFile): Nexus rock properties file object
+        input_number (int): Rock properties method number in Nexus fcs file
+        properties (dict[str, Union[str, int, float, Enum, list[str], pd.DataFrame,
+                    dict[str, Union[float, pd.DataFrame]]]]):
+            Dictionary holding all properties for a specific rock properties method. Defaults to empty dictionary.
+    """
+
+    # General parameters
+    file: NexusFile
+    properties: dict[str, Union[str, int, float, Enum, list[str], pd.DataFrame,
+                                dict[str, Union[float, pd.DataFrame]]]] = field(default_factory=get_empty_dict_union)
+
+    def __init__(self, file: NexusFile, input_number: int,
+                 properties: Optional[dict[str, Union[str, int, float, Enum, list[str], pd.DataFrame,
+                                                      dict[str, Union[float, pd.DataFrame]]]]] = None) -> None:
+        if properties is not None:
+            self.properties = properties
+        else:
+            self.properties = {}
+        super().__init__(input_number=input_number, file=file)
+
+    def to_string(self) -> str:
+        """Create string with rock properties data, in Nexus file format."""
+        printable_str = ''
+        rock_dict = self.properties
+        for key, value in rock_dict.items():
+            if key == 'DESC' and isinstance(value, list):
+                for desc_line in value:
+                    printable_str += 'DESC ' + desc_line + '\n'
+            elif isinstance(value, pd.DataFrame):
+                printable_str += f'{key}\n'
+                printable_str += value.to_string(na_rep='', index=False) + '\n\n'
+            elif isinstance(value, dict):
+                printable_str += f"{key.replace('_',' ')}\n"
+                for subkey in value.keys():
+                    printable_str += f"SWINIT {subkey}\n"
+                    df = value[subkey]
+                    if isinstance(df, pd.DataFrame):
+                        printable_str += df.to_string(na_rep='', index=False) + '\n'
+                    printable_str += '\n'
+            elif isinstance(value, Enum):
+                if isinstance(value, UnitSystem) or isinstance(value, TemperatureUnits):
+                    printable_str += f'{value.value}\n'
+                elif isinstance(value, SUnits):
+                    printable_str += f'SUNITS {value.value}\n'
+            elif value == '':
+                printable_str += f'{key}\n'
+            else:
+                printable_str += f'{key} {value}\n'
+        return printable_str
+
+    def read_properties(self) -> None:
+        """Read Nexus rock properties file contents and populate NexusRockMethod object."""
+        file_as_list = self.file.get_flat_list_str_file
+
+        # Check for common input data
+        nfo.check_for_and_populate_common_input_data(file_as_list, self.properties)
+
+        # Initialize properties
+        cmt_indices: list[int] = []
+        wirct_indices_dict: dict[str, dict[str, list[int]]] = {}
+        # Flag to tell when to start reading a table
+        start_reading_table: bool = False
+        swinit_key = ''
+        # Dictionary of flags indicating which tables are being read
+        table_being_read: dict[str, bool] = {}
+        for table_name in ROCK_ALL_TABLE_KEYWORDS:
+            table_being_read[table_name] = False
+
+        line_indx = 0
+        for line in file_as_list:
+
+            # Find ROCK key-value pairs, such as PREF 2000 or CR 1e-6
+            if [i for i in line.split() if i in ROCK_KEYWORDS_VALUE_FLOAT]:
+                for key in ROCK_KEYWORDS_VALUE_FLOAT:
+                    if nfo.check_token(key, line):
+                        self.properties[key] = float(nfo.get_expected_token_value(key, line, file_as_list))
+            # Find standalone rock property keywords, such as COMPR or KPMULT
+            if [i for i in line.split() if i in ROCK_SINGLE_KEYWORDS]:
+                for word in ROCK_SINGLE_KEYWORDS:
+                    if nfo.check_token(word, line):
+                        self.properties[word] = ''
+            # Handle REVERSIBLE or IRREVERSIBLE keywords
+            if [i for i in line.split() if i in ROCK_KEYWORDS_VALUE_STR]:
+                for key in ROCK_KEYWORDS_VALUE_STR:
+                    if nfo.check_token(key, line):
+                        if nfo.get_token_value(key, line, file_as_list) in ROCK_REV_IRREV_OPTIONS:
+                            self.properties[key] = nfo.get_expected_token_value(key, line, file_as_list)
+                        else:
+                            self.properties[key] = ''
+            # Find starting index of rock compaction table
+            if nfo.check_token('CMT', line):
+                cmt_indices = [line_indx + 1, len(file_as_list)]
+                table_being_read['CMT'] = True
+                start_reading_table = True
+                line_indx += 1
+                continue
+            # Find ending index of rock compaction table
+            if start_reading_table and table_being_read['CMT']:
+                for potential_endkeyword in ROCK_KEYWORDS:
+                    if nfo.check_token(potential_endkeyword, line):
+                        cmt_indices[1] = line_indx
+                        start_reading_table = False
+                        table_being_read['CMT'] = False
+                        break
+            # Find ending index of a water-induced rock compaction table
+            if start_reading_table and table_being_read['WIRCT']:
+                for potential_endkeyword in ROCK_KEYWORDS:
+                    if nfo.check_token(potential_endkeyword, line):
+                        wirct_indices_dict['WIRCT'][swinit_key][1] = line_indx
+                        start_reading_table = False
+                        table_being_read['WIRCT'] = False
+                        break
+            # Find starting index of a water-induced rock compaction table
+            if nfo.check_token('WIRCT', line):
+                wirct_indices_dict['WIRCT'] = {}
+            if nfo.check_token('SWINIT', line):
+                swinit_key = nfo.get_expected_token_value('SWINIT', line, file_as_list)
+                wirct_indices_dict['WIRCT'][swinit_key] = [line_indx+1, len(file_as_list)]
+                table_being_read['WIRCT'] = True
+                start_reading_table = True
+
+            line_indx += 1
+
+        # Read in compaction table(s) if there are any
+        if len(cmt_indices) > 0:
+            self.properties['CMT'] = nfo.read_table_to_df(file_as_list[cmt_indices[0]:cmt_indices[1]])
+        for key in wirct_indices_dict.keys():
+            self.properties[key] = {}
+            for subkey in wirct_indices_dict[key].keys():
+                property_key = self.properties[key]
+                if not isinstance(property_key, dict):
+                    raise ValueError(f"Property is not a dictionary: {str(self.properties[key])}")
+                property_key[subkey] = nfo.read_table_to_df(file_as_list[
+                                                            wirct_indices_dict[key][subkey][0]:
+                                                            wirct_indices_dict[key][subkey][1]])
```

### Comparing `ressimpy-1.0.0/ResSimpy/Nexus/DataModels/NexusSeparatorMethod.py` & `ressimpy-1.0.1/ResSimpy/Nexus/DataModels/NexusSeparatorMethod.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,150 +1,150 @@
-from dataclasses import dataclass, field
-from enum import Enum
-from typing import Optional, Union
-import pandas as pd
-from ResSimpy.Nexus.DataModels.NexusFile import NexusFile
-from ResSimpy.Utils.factory_methods import get_empty_dict_union
-import ResSimpy.Nexus.nexus_file_operations as nfo
-from ResSimpy.Nexus.NexusKeywords.separator_keywords import SEPARATOR_KEYS_INT, SEPARATOR_KEYS_FLOAT
-from ResSimpy.Nexus.NexusKeywords.separator_keywords import SEPARATOR_KEYWORDS
-from ResSimpy.DynamicProperty import DynamicProperty
-from ResSimpy.Enums.UnitsEnum import UnitSystem, SUnits, TemperatureUnits
-
-
-@dataclass(kw_only=True, repr=False)  # Doesn't need to write an _init_, _eq_ methods, etc.
-class NexusSeparatorMethod(DynamicProperty):
-    """Class to hold data input for a Nexus Separator method.
-
-    Attributes:
-        file (NexusFile): Nexus Separator file object
-        input_number (int): Separator method number in Nexus fcs file
-        separator_type (Optional[str]): Type of separator method, e.g., BLACKOIL, GASPLANT or EOS. Defaults to None
-        properties (dict[str, Union[str, int, float, Enum, list[str], pd.DataFrame,
-                    dict[str, Union[float, pd.DataFrame]]]]):
-            Dictionary holding all properties for a specific separator method. Defaults to empty dictionary.
-    """
-
-    file: NexusFile
-    separator_type: Optional[str] = None
-    properties: dict[str, Union[str, int, float, Enum, list[str],
-                     pd.DataFrame, dict[str, Union[float, pd.DataFrame]]]] \
-        = field(default_factory=get_empty_dict_union)
-
-    def __init__(self, file: NexusFile, input_number: int, separator_type: Optional[str] = None,
-                 properties: Optional[dict[str, Union[str, int, float, Enum, list[str], pd.DataFrame,
-                                      dict[str, Union[float, pd.DataFrame]]]]] = None) -> None:
-        if separator_type is not None:
-            self.separator_type = separator_type
-        if properties is not None:
-            self.properties = properties
-        else:
-            self.properties = {}
-        super().__init__(input_number=input_number, file=file)
-
-    def to_string(self) -> str:
-        """Create string with separator data in Nexus file format."""
-        printable_str = ''
-        sep_dict = self.properties
-        for key, value in sep_dict.items():
-            if key == 'DESC' and isinstance(value, list):
-                for desc_line in value:
-                    printable_str += 'DESC ' + desc_line + '\n'
-            elif key == 'SEPARATOR_TABLE' and isinstance(value, pd.DataFrame):
-                if self.separator_type == 'GASPLANT':
-                    printable_str += 'RECFAC_TABLE\n'
-                printable_str += value.to_string(na_rep='', index=False) + '\n'
-                if self.separator_type == 'GASPLANT':
-                    printable_str += 'ENDRECFAC_TABLE\n'
-                printable_str += '\n'
-            elif isinstance(value, Enum):
-                if isinstance(value, UnitSystem) or isinstance(value, TemperatureUnits):
-                    printable_str += f'{value.value}\n'
-                elif isinstance(value, SUnits):
-                    printable_str += f'SUNITS {value.value}\n'
-            elif key == 'KEYCPTLIST' and isinstance(value, list):
-                printable_str += f"{key} {' '.join(value)}\n"
-            elif value == '':
-                printable_str += f'{key}\n'
-            else:
-                printable_str += f'{key} {value}\n'
-        return printable_str
-
-    def read_properties(self) -> None:
-        """Read Nexus Separator file contents and populate NexusSeparatorMethod object."""
-        file_as_list = self.file.get_flat_list_str_file
-
-        # Check for common input data
-        nfo.check_for_and_populate_common_input_data(file_as_list, self.properties)
-
-        # Initialize flags and containers used to record properties as we iterate through separator file contents
-        # List to record start and ending indices for tables
-        sep_table_indices: list[int] = [0, len(file_as_list)]
-        # Flag to tell when to start reading a table
-        start_reading_table: bool = False
-
-        line_indx = 0
-        for line in file_as_list:
-
-            # Determine separator type, i.e., EOS multistage, gas plant data or black oil
-            if nfo.check_token('TEMP', line):  # EOS multistage separator table
-                self.separator_type = 'EOS'
-                sep_table_indices[0] = line_indx  # Specify EOS multistage separator table starting index
-                start_reading_table = True
-                line_indx += 1
-                continue
-            elif nfo.check_token('KEYCPTLIST', line):  # Gas plant data
-                self.separator_type = 'GASPLANT'
-                elems = line.split('!')[0].split()
-                cpt_index = elems.index('KEYCPTLIST')
-                if 'KEYCPTLIST' not in self.properties.keys():
-                    self.properties['KEYCPTLIST'] = elems[cpt_index + 1:]
-                line_indx += 1
-                continue
-            elif nfo.check_token('BOSEP', line):  # Black oil separator table
-                self.separator_type = 'BLACKOIL'
-                self.properties['BOSEP'] = ''
-                line_indx += 1
-                continue
-
-            # Find SEPARATOR key-value pairs, such as WATERMETHOD 1 or PRES_STD 14.7
-            if [i for i in line.split() if i in SEPARATOR_KEYS_FLOAT]:
-                for key in SEPARATOR_KEYS_FLOAT:
-                    if nfo.check_token(key, line):
-                        self.properties[key] = float(nfo.get_expected_token_value(key, line, file_as_list))
-            if [i for i in line.split() if i in SEPARATOR_KEYS_INT]:
-                for key in SEPARATOR_KEYS_INT:
-                    if nfo.check_token(key, line):
-                        self.properties[key] = int(nfo.get_expected_token_value(key, line, file_as_list))
-
-            # Find starting index for black oil separator table
-            if self.separator_type == 'BLACKOIL':
-                if nfo.check_token('KVOIL', line):
-                    sep_table_indices[0] = line_indx
-                    start_reading_table = True
-                    line_indx += 1
-                    continue
-
-            # Find ending index for EOS multistage and black oil separator tables
-            if start_reading_table:
-                if self.separator_type in ['EOS', 'BLACKOIL']:
-                    for keyword in SEPARATOR_KEYWORDS:
-                        if nfo.check_token(keyword, line):
-                            sep_table_indices[1] = line_indx
-                            start_reading_table = False
-                            break
-
-            # Find starting and ending indices for gas plant separator table
-            if self.separator_type == 'GASPLANT':
-                if nfo.check_token('RECFAC_TABLE', line):
-                    sep_table_indices[0] = line_indx + 1
-                    start_reading_table = True
-                if nfo.check_token('ENDRECFAC_TABLE', line):
-                    sep_table_indices[1] = line_indx
-                    start_reading_table = False
-
-            line_indx += 1
-
-        # Read in separator table
-        if self.separator_type is not None:
-            self.properties['SEPARATOR_TABLE'] = nfo.read_table_to_df(file_as_list[sep_table_indices[0]:
-                                                                                   sep_table_indices[1]])
+from dataclasses import dataclass, field
+from enum import Enum
+from typing import Optional, Union
+import pandas as pd
+from ResSimpy.Nexus.DataModels.NexusFile import NexusFile
+from ResSimpy.Utils.factory_methods import get_empty_dict_union
+import ResSimpy.Nexus.nexus_file_operations as nfo
+from ResSimpy.Nexus.NexusKeywords.separator_keywords import SEPARATOR_KEYS_INT, SEPARATOR_KEYS_FLOAT
+from ResSimpy.Nexus.NexusKeywords.separator_keywords import SEPARATOR_KEYWORDS
+from ResSimpy.DynamicProperty import DynamicProperty
+from ResSimpy.Enums.UnitsEnum import UnitSystem, SUnits, TemperatureUnits
+
+
+@dataclass(kw_only=True, repr=False)  # Doesn't need to write an _init_, _eq_ methods, etc.
+class NexusSeparatorMethod(DynamicProperty):
+    """Class to hold data input for a Nexus Separator method.
+
+    Attributes:
+        file (NexusFile): Nexus Separator file object
+        input_number (int): Separator method number in Nexus fcs file
+        separator_type (Optional[str]): Type of separator method, e.g., BLACKOIL, GASPLANT or EOS. Defaults to None
+        properties (dict[str, Union[str, int, float, Enum, list[str], pd.DataFrame,
+                    dict[str, Union[float, pd.DataFrame]]]]):
+            Dictionary holding all properties for a specific separator method. Defaults to empty dictionary.
+    """
+
+    file: NexusFile
+    separator_type: Optional[str] = None
+    properties: dict[str, Union[str, int, float, Enum, list[str],
+                     pd.DataFrame, dict[str, Union[float, pd.DataFrame]]]] \
+        = field(default_factory=get_empty_dict_union)
+
+    def __init__(self, file: NexusFile, input_number: int, separator_type: Optional[str] = None,
+                 properties: Optional[dict[str, Union[str, int, float, Enum, list[str], pd.DataFrame,
+                                      dict[str, Union[float, pd.DataFrame]]]]] = None) -> None:
+        if separator_type is not None:
+            self.separator_type = separator_type
+        if properties is not None:
+            self.properties = properties
+        else:
+            self.properties = {}
+        super().__init__(input_number=input_number, file=file)
+
+    def to_string(self) -> str:
+        """Create string with separator data in Nexus file format."""
+        printable_str = ''
+        sep_dict = self.properties
+        for key, value in sep_dict.items():
+            if key == 'DESC' and isinstance(value, list):
+                for desc_line in value:
+                    printable_str += 'DESC ' + desc_line + '\n'
+            elif key == 'SEPARATOR_TABLE' and isinstance(value, pd.DataFrame):
+                if self.separator_type == 'GASPLANT':
+                    printable_str += 'RECFAC_TABLE\n'
+                printable_str += value.to_string(na_rep='', index=False) + '\n'
+                if self.separator_type == 'GASPLANT':
+                    printable_str += 'ENDRECFAC_TABLE\n'
+                printable_str += '\n'
+            elif isinstance(value, Enum):
+                if isinstance(value, UnitSystem) or isinstance(value, TemperatureUnits):
+                    printable_str += f'{value.value}\n'
+                elif isinstance(value, SUnits):
+                    printable_str += f'SUNITS {value.value}\n'
+            elif key == 'KEYCPTLIST' and isinstance(value, list):
+                printable_str += f"{key} {' '.join(value)}\n"
+            elif value == '':
+                printable_str += f'{key}\n'
+            else:
+                printable_str += f'{key} {value}\n'
+        return printable_str
+
+    def read_properties(self) -> None:
+        """Read Nexus Separator file contents and populate NexusSeparatorMethod object."""
+        file_as_list = self.file.get_flat_list_str_file
+
+        # Check for common input data
+        nfo.check_for_and_populate_common_input_data(file_as_list, self.properties)
+
+        # Initialize flags and containers used to record properties as we iterate through separator file contents
+        # List to record start and ending indices for tables
+        sep_table_indices: list[int] = [0, len(file_as_list)]
+        # Flag to tell when to start reading a table
+        start_reading_table: bool = False
+
+        line_indx = 0
+        for line in file_as_list:
+
+            # Determine separator type, i.e., EOS multistage, gas plant data or black oil
+            if nfo.check_token('TEMP', line):  # EOS multistage separator table
+                self.separator_type = 'EOS'
+                sep_table_indices[0] = line_indx  # Specify EOS multistage separator table starting index
+                start_reading_table = True
+                line_indx += 1
+                continue
+            elif nfo.check_token('KEYCPTLIST', line):  # Gas plant data
+                self.separator_type = 'GASPLANT'
+                elems = line.split('!')[0].split()
+                cpt_index = elems.index('KEYCPTLIST')
+                if 'KEYCPTLIST' not in self.properties.keys():
+                    self.properties['KEYCPTLIST'] = elems[cpt_index + 1:]
+                line_indx += 1
+                continue
+            elif nfo.check_token('BOSEP', line):  # Black oil separator table
+                self.separator_type = 'BLACKOIL'
+                self.properties['BOSEP'] = ''
+                line_indx += 1
+                continue
+
+            # Find SEPARATOR key-value pairs, such as WATERMETHOD 1 or PRES_STD 14.7
+            if [i for i in line.split() if i in SEPARATOR_KEYS_FLOAT]:
+                for key in SEPARATOR_KEYS_FLOAT:
+                    if nfo.check_token(key, line):
+                        self.properties[key] = float(nfo.get_expected_token_value(key, line, file_as_list))
+            if [i for i in line.split() if i in SEPARATOR_KEYS_INT]:
+                for key in SEPARATOR_KEYS_INT:
+                    if nfo.check_token(key, line):
+                        self.properties[key] = int(nfo.get_expected_token_value(key, line, file_as_list))
+
+            # Find starting index for black oil separator table
+            if self.separator_type == 'BLACKOIL':
+                if nfo.check_token('KVOIL', line):
+                    sep_table_indices[0] = line_indx
+                    start_reading_table = True
+                    line_indx += 1
+                    continue
+
+            # Find ending index for EOS multistage and black oil separator tables
+            if start_reading_table:
+                if self.separator_type in ['EOS', 'BLACKOIL']:
+                    for keyword in SEPARATOR_KEYWORDS:
+                        if nfo.check_token(keyword, line):
+                            sep_table_indices[1] = line_indx
+                            start_reading_table = False
+                            break
+
+            # Find starting and ending indices for gas plant separator table
+            if self.separator_type == 'GASPLANT':
+                if nfo.check_token('RECFAC_TABLE', line):
+                    sep_table_indices[0] = line_indx + 1
+                    start_reading_table = True
+                if nfo.check_token('ENDRECFAC_TABLE', line):
+                    sep_table_indices[1] = line_indx
+                    start_reading_table = False
+
+            line_indx += 1
+
+        # Read in separator table
+        if self.separator_type is not None:
+            self.properties['SEPARATOR_TABLE'] = nfo.read_table_to_df(file_as_list[sep_table_indices[0]:
+                                                                                   sep_table_indices[1]])
```

### Comparing `ressimpy-1.0.0/ResSimpy/Nexus/DataModels/NexusWaterMethod.py` & `ressimpy-1.0.1/ResSimpy/Nexus/DataModels/NexusWaterMethod.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,196 +1,196 @@
-from dataclasses import dataclass, field
-from enum import Enum
-from typing import Optional, Union
-import pandas as pd
-from ResSimpy.Nexus.DataModels.NexusFile import NexusFile
-from ResSimpy.DynamicProperty import DynamicProperty
-from ResSimpy.Enums.UnitsEnum import UnitSystem, SUnits, TemperatureUnits
-from ResSimpy.Utils.factory_methods import get_empty_dict_union, get_empty_list_nexus_water_params
-import ResSimpy.Nexus.nexus_file_operations as nfo
-from ResSimpy.Utils.invert_nexus_map import invert_nexus_map
-
-
-@dataclass  # Doesn't need to write an _init_, _eq_ methods, etc.
-class NexusWaterParams:
-    """Class to hold a single set of water property parameters, i.e., density, compressibility, etc.
-
-    Attributes:
-        temperature (Optional[float]): Temperature at which the rest of the water property parameters apply
-        salinity (Optional[float]): Salinity at which the rest of the water property parameters apply
-        density (Optional[float]): Water density at standard conditions
-        compressibility (float): Water compressibility
-        formation_volume_factor (float): Water formation volume factor at the given temperature and reference pressure
-        viscosity (float): Water viscosity at the given temperature and reference pressure
-        viscosity_compressibility (Optional[float]): Water viscosity compressibility.
-    """
-
-    # General parameters
-    compressibility: Optional[float] = None
-    formation_volume_factor: Optional[float] = None
-    viscosity: Optional[float] = None
-    viscosity_compressibility: Optional[float] = None
-    temperature: Optional[float] = None
-    salinity: Optional[float] = None
-    density: Optional[float] = None
-
-
-@dataclass(kw_only=True, repr=False)  # Doesn't need to write an _init_, _eq_ methods, etc.
-class NexusWaterMethod(DynamicProperty):
-    """Class to hold Nexus Water properties.
-
-    Attributes:
-        file (NexusFile): Nexus water file object
-        input_number (int): Water method number in Nexus fcs file
-        reference_pressure (float): Reference pressure for BW and, if CVW is present, for VISW
-        properties (dict[str, Union[str, int, float, Enum, list[str], pd.DataFrame,
-                    dict[str, Union[float, pd.DataFrame]]]]):
-            Dictionary holding properties for generic dynamic method. Defaults to empty dictionary.
-        parameters (list[NexusWaterParams]): list of water parameters, such as density, viscosity, etc.
-    """
-
-    file: NexusFile
-    reference_pressure: Optional[float] = None
-    properties: dict[str, Union[str, int, float, Enum, list[str],
-                     pd.DataFrame, dict[str, Union[float, pd.DataFrame]]]] \
-        = field(default_factory=get_empty_dict_union)
-    parameters: list[NexusWaterParams] = field(default_factory=get_empty_list_nexus_water_params)
-
-    def __init__(self, file: NexusFile, input_number: int, reference_pressure: Optional[float] = None,
-                 properties: Optional[dict[str, Union[str, int, float, Enum, list[str], pd.DataFrame,
-                                      dict[str, Union[float, pd.DataFrame]]]]] = None,
-                 parameters: Optional[list[NexusWaterParams]] = None) -> None:
-        self.reference_pressure = reference_pressure
-        if properties is not None:
-            self.properties = properties
-        else:
-            self.properties = {}
-        if parameters is not None:
-            self.parameters = parameters
-        else:
-            self.parameters = []
-        super().__init__(input_number=input_number, file=file)
-
-    @staticmethod
-    def nexus_mapping() -> dict[str, tuple[str, type]]:
-        """Returns a dictionary of mapping from nexus keyword to attribute name."""
-
-        nexus_mapping: dict[str, tuple[str, type]] = {
-            'DENW': ('density', float),
-            'CW': ('compressibility', float),
-            'BW': ('formation_volume_factor', float),
-            'VISW': ('viscosity', float),
-            'CVW': ('viscosity_compressibility', float)
-            }
-        return nexus_mapping
-
-    def to_string(self) -> str:
-        """Create string with water data, in Nexus file format."""
-        param_to_nexus_keyword_map = invert_nexus_map(NexusWaterMethod.nexus_mapping())
-
-        printable_str = ''
-        water_dict = self.properties
-        # Print description if present
-        if 'DESC' in water_dict.keys() and isinstance(water_dict['DESC'], list):
-            for desc_line in water_dict['DESC']:
-                printable_str += 'DESC ' + desc_line + '\n'
-        if self.reference_pressure is not None:
-            printable_str += f'PREF {self.reference_pressure}\n'
-        for key, value in water_dict.items():
-            if isinstance(value, Enum):
-                if isinstance(value, UnitSystem) or isinstance(value, TemperatureUnits):
-                    printable_str += f'{value.value}\n'
-                elif isinstance(value, SUnits):
-                    printable_str += f'SUNITS {value.value}\n'
-            elif key not in ['DESC']:
-                if value == '':
-                    printable_str += f'{key}\n'
-                else:
-                    printable_str += f'{key} {value}\n'
-        water_params = self.parameters
-        temp_val = None
-        sal_val = None
-        for i in range(len(water_params)):
-            water_param_dict = water_params[i].__dict__
-            space_prefix = ''
-            if water_param_dict['temperature']:
-                if water_param_dict['temperature'] != temp_val:
-                    printable_str += f"TEMP {water_param_dict['temperature']}\n"
-                    temp_val = water_param_dict['temperature']
-                space_prefix += '    '
-            if water_param_dict['salinity']:
-                if water_param_dict['salinity'] != sal_val:
-                    printable_str += f"{space_prefix}SALINITY {water_param_dict['salinity']}\n"
-                    sal_val = water_param_dict['salinity']
-                space_prefix += '    '
-            for key in param_to_nexus_keyword_map.keys():
-                if water_param_dict[key]:
-                    printable_str += f'{space_prefix}{param_to_nexus_keyword_map[key]} {water_param_dict[key]}\n'
-        return printable_str
-
-    def read_properties(self) -> None:
-        """Read Nexus Water file contents and populate NexusWaterMethod object."""
-        file_as_list = self.file.get_flat_list_str_file
-
-        # Check for common input data
-        nfo.check_for_and_populate_common_input_data(file_as_list, self.properties)
-
-        # Initialize properties
-        water_props_dict_none: dict[str, Optional[float]] = {'DENW': None, 'CW': None, 'BW': None,
-                                                             'VISW': None, 'CVW': None}
-        water_props_dict: dict[str, Optional[float]] = water_props_dict_none.copy()
-
-        line_indx = 0
-        reading_props = False  # Flag indicating if actively reading a property section
-        found_params = False  # Flag inidicating if identified any WATER keywords
-        temp: Optional[float] = None  # Variable to hold temperature for property section
-        sal: Optional[float] = None  # Variable to hold salinity for property section
-        for line in file_as_list:
-
-            # Read in reference pressure
-            if nfo.check_token('PREF', line):  # Reference pressure
-                self.reference_pressure = float(nfo.get_expected_token_value('PREF', line, file_as_list))
-
-            # Check if reading properties
-            if nfo.check_token('CW', line):
-                reading_props = True
-                found_params = True
-
-            # If found a new property section based on TEMP or SALINITY repeat
-            if reading_props and (nfo.check_token('TEMP', line) or nfo.check_token('SALINITY', line)):
-                reading_props = False
-                # Append new parameters to list of water parameters
-                params = NexusWaterParams(temperature=temp,
-                                          salinity=sal,
-                                          density=water_props_dict['DENW'],
-                                          compressibility=water_props_dict['CW'],
-                                          formation_volume_factor=water_props_dict['BW'],
-                                          viscosity=water_props_dict['VISW'],
-                                          viscosity_compressibility=water_props_dict['CVW']
-                                          )
-                self.parameters.append(params)
-                # Reset property dictionary
-                water_props_dict = water_props_dict_none.copy()  # Reset
-
-            # Read in relevant water properties in line
-            if nfo.check_token('TEMP', line):
-                temp = float(nfo.get_expected_token_value('TEMP', line, file_as_list))
-            if nfo.check_token('SALINITY', line):
-                sal = float(nfo.get_expected_token_value('SALINITY', line, file_as_list))
-            for key in water_props_dict.keys():
-                if nfo.check_token(key, line):
-                    found_params = True
-                    water_props_dict[key] = float(nfo.get_expected_token_value(key, line, file_as_list))
-
-            line_indx += 1
-
-        if found_params:
-            # Append new parameters to list of water parameters
-            params = NexusWaterParams(temperature=temp,
-                                      salinity=sal,
-                                      density=water_props_dict['DENW'],
-                                      compressibility=water_props_dict['CW'],
-                                      formation_volume_factor=water_props_dict['BW'],
-                                      viscosity=water_props_dict['VISW'],
-                                      viscosity_compressibility=water_props_dict['CVW']
-                                      )
-            self.parameters.append(params)
+from dataclasses import dataclass, field
+from enum import Enum
+from typing import Optional, Union
+import pandas as pd
+from ResSimpy.Nexus.DataModels.NexusFile import NexusFile
+from ResSimpy.DynamicProperty import DynamicProperty
+from ResSimpy.Enums.UnitsEnum import UnitSystem, SUnits, TemperatureUnits
+from ResSimpy.Utils.factory_methods import get_empty_dict_union, get_empty_list_nexus_water_params
+import ResSimpy.Nexus.nexus_file_operations as nfo
+from ResSimpy.Utils.invert_nexus_map import invert_nexus_map
+
+
+@dataclass  # Doesn't need to write an _init_, _eq_ methods, etc.
+class NexusWaterParams:
+    """Class to hold a single set of water property parameters, i.e., density, compressibility, etc.
+
+    Attributes:
+        temperature (Optional[float]): Temperature at which the rest of the water property parameters apply
+        salinity (Optional[float]): Salinity at which the rest of the water property parameters apply
+        density (Optional[float]): Water density at standard conditions
+        compressibility (float): Water compressibility
+        formation_volume_factor (float): Water formation volume factor at the given temperature and reference pressure
+        viscosity (float): Water viscosity at the given temperature and reference pressure
+        viscosity_compressibility (Optional[float]): Water viscosity compressibility.
+    """
+
+    # General parameters
+    compressibility: Optional[float] = None
+    formation_volume_factor: Optional[float] = None
+    viscosity: Optional[float] = None
+    viscosity_compressibility: Optional[float] = None
+    temperature: Optional[float] = None
+    salinity: Optional[float] = None
+    density: Optional[float] = None
+
+
+@dataclass(kw_only=True, repr=False)  # Doesn't need to write an _init_, _eq_ methods, etc.
+class NexusWaterMethod(DynamicProperty):
+    """Class to hold Nexus Water properties.
+
+    Attributes:
+        file (NexusFile): Nexus water file object
+        input_number (int): Water method number in Nexus fcs file
+        reference_pressure (float): Reference pressure for BW and, if CVW is present, for VISW
+        properties (dict[str, Union[str, int, float, Enum, list[str], pd.DataFrame,
+                    dict[str, Union[float, pd.DataFrame]]]]):
+            Dictionary holding properties for generic dynamic method. Defaults to empty dictionary.
+        parameters (list[NexusWaterParams]): list of water parameters, such as density, viscosity, etc.
+    """
+
+    file: NexusFile
+    reference_pressure: Optional[float] = None
+    properties: dict[str, Union[str, int, float, Enum, list[str],
+                     pd.DataFrame, dict[str, Union[float, pd.DataFrame]]]] \
+        = field(default_factory=get_empty_dict_union)
+    parameters: list[NexusWaterParams] = field(default_factory=get_empty_list_nexus_water_params)
+
+    def __init__(self, file: NexusFile, input_number: int, reference_pressure: Optional[float] = None,
+                 properties: Optional[dict[str, Union[str, int, float, Enum, list[str], pd.DataFrame,
+                                      dict[str, Union[float, pd.DataFrame]]]]] = None,
+                 parameters: Optional[list[NexusWaterParams]] = None) -> None:
+        self.reference_pressure = reference_pressure
+        if properties is not None:
+            self.properties = properties
+        else:
+            self.properties = {}
+        if parameters is not None:
+            self.parameters = parameters
+        else:
+            self.parameters = []
+        super().__init__(input_number=input_number, file=file)
+
+    @staticmethod
+    def nexus_mapping() -> dict[str, tuple[str, type]]:
+        """Returns a dictionary of mapping from nexus keyword to attribute name."""
+
+        nexus_mapping: dict[str, tuple[str, type]] = {
+            'DENW': ('density', float),
+            'CW': ('compressibility', float),
+            'BW': ('formation_volume_factor', float),
+            'VISW': ('viscosity', float),
+            'CVW': ('viscosity_compressibility', float)
+            }
+        return nexus_mapping
+
+    def to_string(self) -> str:
+        """Create string with water data, in Nexus file format."""
+        param_to_nexus_keyword_map = invert_nexus_map(NexusWaterMethod.nexus_mapping())
+
+        printable_str = ''
+        water_dict = self.properties
+        # Print description if present
+        if 'DESC' in water_dict.keys() and isinstance(water_dict['DESC'], list):
+            for desc_line in water_dict['DESC']:
+                printable_str += 'DESC ' + desc_line + '\n'
+        if self.reference_pressure is not None:
+            printable_str += f'PREF {self.reference_pressure}\n'
+        for key, value in water_dict.items():
+            if isinstance(value, Enum):
+                if isinstance(value, UnitSystem) or isinstance(value, TemperatureUnits):
+                    printable_str += f'{value.value}\n'
+                elif isinstance(value, SUnits):
+                    printable_str += f'SUNITS {value.value}\n'
+            elif key not in ['DESC']:
+                if value == '':
+                    printable_str += f'{key}\n'
+                else:
+                    printable_str += f'{key} {value}\n'
+        water_params = self.parameters
+        temp_val = None
+        sal_val = None
+        for i in range(len(water_params)):
+            water_param_dict = water_params[i].__dict__
+            space_prefix = ''
+            if water_param_dict['temperature']:
+                if water_param_dict['temperature'] != temp_val:
+                    printable_str += f"TEMP {water_param_dict['temperature']}\n"
+                    temp_val = water_param_dict['temperature']
+                space_prefix += '    '
+            if water_param_dict['salinity']:
+                if water_param_dict['salinity'] != sal_val:
+                    printable_str += f"{space_prefix}SALINITY {water_param_dict['salinity']}\n"
+                    sal_val = water_param_dict['salinity']
+                space_prefix += '    '
+            for key in param_to_nexus_keyword_map.keys():
+                if water_param_dict[key]:
+                    printable_str += f'{space_prefix}{param_to_nexus_keyword_map[key]} {water_param_dict[key]}\n'
+        return printable_str
+
+    def read_properties(self) -> None:
+        """Read Nexus Water file contents and populate NexusWaterMethod object."""
+        file_as_list = self.file.get_flat_list_str_file
+
+        # Check for common input data
+        nfo.check_for_and_populate_common_input_data(file_as_list, self.properties)
+
+        # Initialize properties
+        water_props_dict_none: dict[str, Optional[float]] = {'DENW': None, 'CW': None, 'BW': None,
+                                                             'VISW': None, 'CVW': None}
+        water_props_dict: dict[str, Optional[float]] = water_props_dict_none.copy()
+
+        line_indx = 0
+        reading_props = False  # Flag indicating if actively reading a property section
+        found_params = False  # Flag inidicating if identified any WATER keywords
+        temp: Optional[float] = None  # Variable to hold temperature for property section
+        sal: Optional[float] = None  # Variable to hold salinity for property section
+        for line in file_as_list:
+
+            # Read in reference pressure
+            if nfo.check_token('PREF', line):  # Reference pressure
+                self.reference_pressure = float(nfo.get_expected_token_value('PREF', line, file_as_list))
+
+            # Check if reading properties
+            if nfo.check_token('CW', line):
+                reading_props = True
+                found_params = True
+
+            # If found a new property section based on TEMP or SALINITY repeat
+            if reading_props and (nfo.check_token('TEMP', line) or nfo.check_token('SALINITY', line)):
+                reading_props = False
+                # Append new parameters to list of water parameters
+                params = NexusWaterParams(temperature=temp,
+                                          salinity=sal,
+                                          density=water_props_dict['DENW'],
+                                          compressibility=water_props_dict['CW'],
+                                          formation_volume_factor=water_props_dict['BW'],
+                                          viscosity=water_props_dict['VISW'],
+                                          viscosity_compressibility=water_props_dict['CVW']
+                                          )
+                self.parameters.append(params)
+                # Reset property dictionary
+                water_props_dict = water_props_dict_none.copy()  # Reset
+
+            # Read in relevant water properties in line
+            if nfo.check_token('TEMP', line):
+                temp = float(nfo.get_expected_token_value('TEMP', line, file_as_list))
+            if nfo.check_token('SALINITY', line):
+                sal = float(nfo.get_expected_token_value('SALINITY', line, file_as_list))
+            for key in water_props_dict.keys():
+                if nfo.check_token(key, line):
+                    found_params = True
+                    water_props_dict[key] = float(nfo.get_expected_token_value(key, line, file_as_list))
+
+            line_indx += 1
+
+        if found_params:
+            # Append new parameters to list of water parameters
+            params = NexusWaterParams(temperature=temp,
+                                      salinity=sal,
+                                      density=water_props_dict['DENW'],
+                                      compressibility=water_props_dict['CW'],
+                                      formation_volume_factor=water_props_dict['BW'],
+                                      viscosity=water_props_dict['VISW'],
+                                      viscosity_compressibility=water_props_dict['CVW']
+                                      )
+            self.parameters.append(params)
```

### Comparing `ressimpy-1.0.0/ResSimpy/Nexus/DataModels/StructuredGrid/NexusGrid.py` & `ressimpy-1.0.1/ResSimpy/Nexus/DataModels/StructuredGrid/NexusGrid.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,302 +1,302 @@
-from __future__ import annotations
-
-import copy
-import pandas as pd
-from dataclasses import dataclass
-from typing import Optional, TYPE_CHECKING
-
-from ResSimpy.Grid import Grid, VariableEntry
-from ResSimpy.Nexus.DataModels.NexusFile import NexusFile
-from ResSimpy.Nexus.structured_grid_operations import StructuredGridOperations
-import ResSimpy.Nexus.nexus_file_operations as nfo
-import ResSimpy.Nexus.array_function_operations as afo
-
-from resqpy.olio.read_nexus_fault import load_nexus_fault_mult_table_from_list
-
-if TYPE_CHECKING:
-    from ResSimpy.Nexus.NexusSimulator import NexusSimulator
-
-
-@dataclass
-class PropertyToLoad:
-    token: str
-    modifiers: list[str]
-    property: VariableEntry
-
-
-@dataclass(kw_only=True)
-class NexusGrid(Grid):
-    __array_functions_list: Optional[list[list[str]]] = None
-    __array_functions_df: Optional[pd.DataFrame] = None
-    __array_functions_loaded: bool = False
-    __grid_file_contents: Optional[list[str]] = None
-    __grid_file_nested: Optional[list[str]] = None
-    __faults_df: Optional[pd.DataFrame] = None
-    __grid_faults_loaded: bool = False
-    __grid_properties_loaded: bool = False
-    __grid_nexus_file: Optional[NexusFile] = None
-
-    def __init__(self, grid_nexus_file: Optional[NexusFile] = None) -> None:
-        super().__init__()
-        self.__array_functions_list: Optional[list[str]] = None
-        self.__array_functions_df: Optional[pd.DataFrame] = None
-        self.__array_functions_loaded: bool = False
-        self.__grid_file_contents: Optional[list[str]] = None if grid_nexus_file is None else \
-            grid_nexus_file.get_flat_list_str_file_including_includes
-        self.__grid_file_nested: Optional[list[str]] = None if grid_nexus_file is None else \
-            grid_nexus_file.file_content_as_list
-        self.__faults_df: Optional[pd.DataFrame] = None
-        self.__grid_faults_loaded: bool = False
-        self.__grid_properties_loaded: bool = False
-        self.__grid_nexus_file: Optional[NexusFile] = grid_nexus_file
-
-    def __wrap(self, value):
-        if isinstance(value, tuple | list | set | frozenset):
-            return type(value)([self.__wrap(v) for v in value])
-        else:
-            return value
-
-    def update_properties_from_dict(self, data: dict[str, int | VariableEntry]) -> None:
-        """Allows you to update properties on the class using the provided dict of values.
-
-        Args:
-        ----
-                data dict[str, int | VariableEntry]: the dictionary of values to update on the class
-        """
-        # Use the dict provided to populate the properties in the class
-        if data is not None:
-            for name, value in data.items():
-                private_name = '_' + name
-                setattr(self, private_name, self.__wrap(value))
-
-        # Prevent reload from disk
-        self.__grid_properties_loaded = True
-
-    def to_dict(self) -> dict[str, Optional[int] | VariableEntry]:
-        self.load_grid_properties_if_not_loaded()
-
-        original_dict = self.__dict__
-        new_dict: dict[str, Optional[int] | VariableEntry] = {}
-        for key in original_dict.keys():
-            new_key = key
-            if new_key[0] == '_':
-                new_key = new_key.replace('_', '', 1)
-            if new_key[0] == '_':
-                new_key = new_key.replace('_', '', 1)
-            new_dict[new_key] = original_dict[key]
-
-        return new_dict
-
-    def load_grid_properties_if_not_loaded(self) -> None:
-        def move_next_value(next_line: str) -> tuple[str, str]:
-            """Finds the next value and then strips out the value from the line.
-
-            Args:
-            ----
-                next_line (str): the line to search through for the value
-
-            Raises:
-            ------
-                ValueError: if no value is found within the line provided
-
-            Returns:
-            -------
-                tuple[str, str]: the next value found in the line, the line with the value stripped out.
-            """
-            value = nfo.get_next_value(0, [next_line], next_line)
-            if value is None:
-                raise ValueError(f"No value found within the provided line: {next_line}")
-            next_line = next_line.replace(value, "", 1)
-            return value, next_line
-
-        # If we've already loaded the grid properties, don't do so again.
-        if self.__grid_properties_loaded:
-            return
-
-        if self.__grid_nexus_file is None or self.__grid_file_contents is None or self.__grid_file_nested is None:
-            raise ValueError("Grid file not found, cannot load grid properties")
-
-        file_as_list = self.__grid_file_contents
-        for line in file_as_list:
-
-            # Load in the basic properties
-            properties_to_load = [
-                PropertyToLoad('NETGRS', ['VALUE', 'CON'], self._netgrs),
-                PropertyToLoad('POROSITY', ['VALUE', 'CON'], self._porosity),
-                PropertyToLoad('SW', ['VALUE', 'CON'], self._sw),
-                PropertyToLoad('KX', ['VALUE', 'MULT', 'CON'], self._kx),
-                PropertyToLoad('PERMX', ['VALUE', 'MULT', 'CON'], self._kx),
-                PropertyToLoad('PERMI', ['VALUE', 'MULT', 'CON'], self._kx),
-                PropertyToLoad('KI', ['VALUE', 'MULT', 'CON'], self._kx),
-                PropertyToLoad('KY', ['VALUE', 'MULT', 'CON'], self._ky),
-                PropertyToLoad('PERMY', ['VALUE', 'MULT', 'CON'], self._ky),
-                PropertyToLoad('PERMJ', ['VALUE', 'MULT', 'CON'], self._ky),
-                PropertyToLoad('KJ', ['VALUE', 'MULT', 'CON'], self._ky),
-                PropertyToLoad('KZ', ['VALUE', 'MULT', 'CON'], self._kz),
-                PropertyToLoad('PERMZ', ['VALUE', 'MULT', 'CON'], self._kz),
-                PropertyToLoad('PERMK', ['VALUE', 'MULT', 'CON'], self._kz),
-                PropertyToLoad('KK', ['VALUE', 'MULT', 'CON'], self._kz),
-            ]
-
-            for token_property in properties_to_load:
-                for modifier in token_property.modifiers:
-                    StructuredGridOperations.load_token_value_if_present(
-                        token_property.token, modifier, token_property.property, line, file_as_list, ['INCLUDE'])
-
-            # Load in grid dimensions
-            if nfo.check_token('NX', line):
-                # Check that the format of the grid is NX followed by NY followed by NZ
-                current_line = file_as_list[file_as_list.index(line)]
-                remaining_line = current_line[current_line.index('NX') + 2:]
-                if nfo.get_next_value(0, [remaining_line], remaining_line) != 'NY':
-                    continue
-                remaining_line = remaining_line[remaining_line.index('NY') + 2:]
-                if nfo.get_next_value(0, [remaining_line], remaining_line) != 'NZ':
-                    continue
-
-                # Avoid loading in a comment
-                if "!" in line and line.index("!") < line.index('NX'):
-                    continue
-                next_line = file_as_list[file_as_list.index(line) + 1]
-                first_value, next_line = move_next_value(next_line)
-                second_value, next_line = move_next_value(next_line)
-                third_value, next_line = move_next_value(next_line)
-
-                self._range_x = int(first_value)
-                self._range_y = int(second_value)
-                self._range_z = int(third_value)
-
-        self.__grid_properties_loaded = True
-
-    @classmethod
-    def load_structured_grid_file(cls: type[NexusGrid], structured_grid_file: NexusFile,
-                                  lazy_loading: bool = True) -> NexusGrid:
-        """Loads in a structured grid file with all grid properties, and the array functions defined with 'FUNCTION'.
-        Other grid modifiers are currently not supported.
-
-        Args:
-        ----
-            structured_grid_file (NexusFile): the NexusFile representation of a structured grid file for converting \
-                into a structured grid file class
-        Raises:
-            AttributeError: if no value is found for the structured grid file path
-            ValueError: if when loading the grid no values can be found for the NX NY NZ line.
-        """
-        if structured_grid_file.location is None:
-            raise ValueError(f"No file path given or found for structured grid file path. \
-                Instead got {structured_grid_file.location}")
-
-        loaded_structured_grid_file = cls(grid_nexus_file=structured_grid_file)
-
-        if not lazy_loading:
-            loaded_structured_grid_file.load_grid_properties_if_not_loaded()
-            loaded_structured_grid_file.load_faults()
-            loaded_structured_grid_file.load_array_functions()
-
-        return loaded_structured_grid_file
-
-    @staticmethod
-    def update_structured_grid_file(grid_dict: dict[str, VariableEntry | int], model: NexusSimulator) -> None:
-        """Save values passed from the front end to the structured grid file and update the class.
-
-        Args:
-        ----
-            grid_dict (dict[str, Union[VariableEntry, int]]): dictionary containing grid properties to be replaced
-            model (NexusSimulator): an instance of a NexusSimulator object
-        Raises:
-            ValueError: If no structured grid file is in the instance of the Simulator class
-        """
-        # Convert the dictionary back to a class, and update the properties on our class
-        structured_grid = model.grid
-        if structured_grid is None or model.model_files.structured_grid_file is None:
-            raise ValueError("Model does not contain a structured grid")
-        original_structured_grid_file = copy.deepcopy(structured_grid)
-
-        # replace the structured grid with a new object with an updated dictionary
-        structured_grid.update_properties_from_dict(grid_dict)
-
-        # change it in the text file for nexus:
-        grid_file_path = model.model_files.structured_grid_file.location
-        if grid_file_path is None:
-            raise ValueError("No path found for structured grid file path.")
-        structured_grid_contents = nfo.load_file_as_list(grid_file_path)
-        # Get the existing file as a list
-        if structured_grid_contents is None:
-            raise ValueError("No path found for structured grid file path. \
-                Please provide a path to the structured grid")
-        # Update each value in the file
-        StructuredGridOperations.replace_value(structured_grid_contents, original_structured_grid_file.netgrs,
-                                               structured_grid.netgrs, 'NETGRS')
-        StructuredGridOperations.replace_value(structured_grid_contents, original_structured_grid_file.porosity,
-                                               structured_grid.porosity, 'POROSITY')
-        StructuredGridOperations.replace_value(structured_grid_contents, original_structured_grid_file.sw,
-                                               structured_grid.sw, 'SW')
-        StructuredGridOperations.replace_value(structured_grid_contents, original_structured_grid_file.kx,
-                                               structured_grid.kx, 'KX')
-        StructuredGridOperations.replace_value(structured_grid_contents, original_structured_grid_file.ky,
-                                               structured_grid.ky, 'KY')
-        StructuredGridOperations.replace_value(structured_grid_contents, original_structured_grid_file.kz,
-                                               structured_grid.kz, 'KZ')
-
-        # Save the new file contents
-        new_file_str = "".join(structured_grid_contents)
-        with open(grid_file_path, "w") as text_file:
-            text_file.write(new_file_str)
-
-    def load_array_functions(self) -> None:
-        if self.__grid_file_contents is None:
-            raise ValueError("Cannot load array functions as grid file cannot not found")
-        self.__array_functions_list = afo.collect_all_function_blocks(self.__grid_file_contents)
-        self.__array_functions_df = afo.summarize_model_functions(self.__array_functions_list)
-        self.__array_functions_loaded = True
-
-    def get_array_functions_list(self) -> Optional[list[list[str]]]:
-        """Returns the grid array functions as a list of function lines."""
-        if not self.__array_functions_loaded:
-            self.load_array_functions()
-        return self.__array_functions_list
-
-    def get_array_functions_df(self) -> Optional[pd.DataFrame]:
-        """Returns the grid array functions as a dataframe."""
-        if not self.__array_functions_loaded:
-            self.load_array_functions()
-        return self.__array_functions_df
-
-    def load_faults(self) -> None:
-        """Function to read faults in Nexus grid file defined using MULT and FNAME keywords."""
-        file_content_as_list = self.__grid_file_contents
-        if file_content_as_list is None:
-            raise ValueError('Grid file contents have not been loaded')
-        df = load_nexus_fault_mult_table_from_list(file_content_as_list)
-
-        if not df.empty:
-            # Ensure resulting dataframe has uppercase column names
-            df.columns = [col.upper() for col in df.columns]
-
-            # Check if any multfls have been used in grid file and update fault trans multipliers accordingly
-            f_names = df['NAME'].unique()
-            f_mults = [1.] * len(f_names)
-            mult_dict = dict(zip(f_names, f_mults))
-            for line in file_content_as_list:
-                if nfo.check_token('MULTFL', line):
-                    fname = str(nfo.get_expected_token_value(
-                        'MULTFL', line, file_content_as_list,
-                        custom_message=f'{line} does not have a fault name following MULTFL'))
-                    if fname in df['NAME'].unique():
-                        tmult = float(str(nfo.get_expected_token_value(
-                            fname, line, file_content_as_list,
-                            custom_message=f'MULTFL {fname} does not have a numerical tmult value')))
-                        mult_dict[fname] *= tmult
-            mult_df = pd.DataFrame.from_dict(mult_dict, orient='index').reset_index()
-            mult_df.columns = ['NAME', 'TMULT']
-            new_df = df.merge(mult_df, how='left', on='NAME', validate='many_to_one')
-            new_df['MULT'] = new_df['MULT'] * new_df['TMULT']
-            self.__faults_df = new_df.drop(['TMULT'], axis=1)
-        self.__grid_faults_loaded = True
-
-    def get_faults_df(self) -> Optional[pd.DataFrame]:
-        """Returns the fault definition and transmissility multiplier information as a dataframe."""
-
-        if not self.__grid_faults_loaded:
-            self.load_faults()
-        return self.__faults_df
+from __future__ import annotations
+
+import copy
+import pandas as pd
+from dataclasses import dataclass
+from typing import Optional, TYPE_CHECKING
+
+from ResSimpy.Grid import Grid, VariableEntry
+from ResSimpy.Nexus.DataModels.NexusFile import NexusFile
+from ResSimpy.Nexus.structured_grid_operations import StructuredGridOperations
+import ResSimpy.Nexus.nexus_file_operations as nfo
+import ResSimpy.Nexus.array_function_operations as afo
+
+from resqpy.olio.read_nexus_fault import load_nexus_fault_mult_table_from_list
+
+if TYPE_CHECKING:
+    from ResSimpy.Nexus.NexusSimulator import NexusSimulator
+
+
+@dataclass
+class PropertyToLoad:
+    token: str
+    modifiers: list[str]
+    property: VariableEntry
+
+
+@dataclass(kw_only=True)
+class NexusGrid(Grid):
+    __array_functions_list: Optional[list[list[str]]] = None
+    __array_functions_df: Optional[pd.DataFrame] = None
+    __array_functions_loaded: bool = False
+    __grid_file_contents: Optional[list[str]] = None
+    __grid_file_nested: Optional[list[str]] = None
+    __faults_df: Optional[pd.DataFrame] = None
+    __grid_faults_loaded: bool = False
+    __grid_properties_loaded: bool = False
+    __grid_nexus_file: Optional[NexusFile] = None
+
+    def __init__(self, grid_nexus_file: Optional[NexusFile] = None) -> None:
+        super().__init__()
+        self.__array_functions_list: Optional[list[str]] = None
+        self.__array_functions_df: Optional[pd.DataFrame] = None
+        self.__array_functions_loaded: bool = False
+        self.__grid_file_contents: Optional[list[str]] = None if grid_nexus_file is None else \
+            grid_nexus_file.get_flat_list_str_file_including_includes
+        self.__grid_file_nested: Optional[list[str]] = None if grid_nexus_file is None else \
+            grid_nexus_file.file_content_as_list
+        self.__faults_df: Optional[pd.DataFrame] = None
+        self.__grid_faults_loaded: bool = False
+        self.__grid_properties_loaded: bool = False
+        self.__grid_nexus_file: Optional[NexusFile] = grid_nexus_file
+
+    def __wrap(self, value):
+        if isinstance(value, tuple | list | set | frozenset):
+            return type(value)([self.__wrap(v) for v in value])
+        else:
+            return value
+
+    def update_properties_from_dict(self, data: dict[str, int | VariableEntry]) -> None:
+        """Allows you to update properties on the class using the provided dict of values.
+
+        Args:
+        ----
+                data dict[str, int | VariableEntry]: the dictionary of values to update on the class
+        """
+        # Use the dict provided to populate the properties in the class
+        if data is not None:
+            for name, value in data.items():
+                private_name = '_' + name
+                setattr(self, private_name, self.__wrap(value))
+
+        # Prevent reload from disk
+        self.__grid_properties_loaded = True
+
+    def to_dict(self) -> dict[str, Optional[int] | VariableEntry]:
+        self.load_grid_properties_if_not_loaded()
+
+        original_dict = self.__dict__
+        new_dict: dict[str, Optional[int] | VariableEntry] = {}
+        for key in original_dict.keys():
+            new_key = key
+            if new_key[0] == '_':
+                new_key = new_key.replace('_', '', 1)
+            if new_key[0] == '_':
+                new_key = new_key.replace('_', '', 1)
+            new_dict[new_key] = original_dict[key]
+
+        return new_dict
+
+    def load_grid_properties_if_not_loaded(self) -> None:
+        def move_next_value(next_line: str) -> tuple[str, str]:
+            """Finds the next value and then strips out the value from the line.
+
+            Args:
+            ----
+                next_line (str): the line to search through for the value
+
+            Raises:
+            ------
+                ValueError: if no value is found within the line provided
+
+            Returns:
+            -------
+                tuple[str, str]: the next value found in the line, the line with the value stripped out.
+            """
+            value = nfo.get_next_value(0, [next_line], next_line)
+            if value is None:
+                raise ValueError(f"No value found within the provided line: {next_line}")
+            next_line = next_line.replace(value, "", 1)
+            return value, next_line
+
+        # If we've already loaded the grid properties, don't do so again.
+        if self.__grid_properties_loaded:
+            return
+
+        if self.__grid_nexus_file is None or self.__grid_file_contents is None or self.__grid_file_nested is None:
+            raise ValueError("Grid file not found, cannot load grid properties")
+
+        file_as_list = self.__grid_file_contents
+        for line in file_as_list:
+
+            # Load in the basic properties
+            properties_to_load = [
+                PropertyToLoad('NETGRS', ['VALUE', 'CON'], self._netgrs),
+                PropertyToLoad('POROSITY', ['VALUE', 'CON'], self._porosity),
+                PropertyToLoad('SW', ['VALUE', 'CON'], self._sw),
+                PropertyToLoad('KX', ['VALUE', 'MULT', 'CON'], self._kx),
+                PropertyToLoad('PERMX', ['VALUE', 'MULT', 'CON'], self._kx),
+                PropertyToLoad('PERMI', ['VALUE', 'MULT', 'CON'], self._kx),
+                PropertyToLoad('KI', ['VALUE', 'MULT', 'CON'], self._kx),
+                PropertyToLoad('KY', ['VALUE', 'MULT', 'CON'], self._ky),
+                PropertyToLoad('PERMY', ['VALUE', 'MULT', 'CON'], self._ky),
+                PropertyToLoad('PERMJ', ['VALUE', 'MULT', 'CON'], self._ky),
+                PropertyToLoad('KJ', ['VALUE', 'MULT', 'CON'], self._ky),
+                PropertyToLoad('KZ', ['VALUE', 'MULT', 'CON'], self._kz),
+                PropertyToLoad('PERMZ', ['VALUE', 'MULT', 'CON'], self._kz),
+                PropertyToLoad('PERMK', ['VALUE', 'MULT', 'CON'], self._kz),
+                PropertyToLoad('KK', ['VALUE', 'MULT', 'CON'], self._kz),
+            ]
+
+            for token_property in properties_to_load:
+                for modifier in token_property.modifiers:
+                    StructuredGridOperations.load_token_value_if_present(
+                        token_property.token, modifier, token_property.property, line, file_as_list, ['INCLUDE'])
+
+            # Load in grid dimensions
+            if nfo.check_token('NX', line):
+                # Check that the format of the grid is NX followed by NY followed by NZ
+                current_line = file_as_list[file_as_list.index(line)]
+                remaining_line = current_line[current_line.index('NX') + 2:]
+                if nfo.get_next_value(0, [remaining_line], remaining_line) != 'NY':
+                    continue
+                remaining_line = remaining_line[remaining_line.index('NY') + 2:]
+                if nfo.get_next_value(0, [remaining_line], remaining_line) != 'NZ':
+                    continue
+
+                # Avoid loading in a comment
+                if "!" in line and line.index("!") < line.index('NX'):
+                    continue
+                next_line = file_as_list[file_as_list.index(line) + 1]
+                first_value, next_line = move_next_value(next_line)
+                second_value, next_line = move_next_value(next_line)
+                third_value, next_line = move_next_value(next_line)
+
+                self._range_x = int(first_value)
+                self._range_y = int(second_value)
+                self._range_z = int(third_value)
+
+        self.__grid_properties_loaded = True
+
+    @classmethod
+    def load_structured_grid_file(cls: type[NexusGrid], structured_grid_file: NexusFile,
+                                  lazy_loading: bool = True) -> NexusGrid:
+        """Loads in a structured grid file with all grid properties, and the array functions defined with 'FUNCTION'.
+        Other grid modifiers are currently not supported.
+
+        Args:
+        ----
+            structured_grid_file (NexusFile): the NexusFile representation of a structured grid file for converting \
+                into a structured grid file class
+        Raises:
+            AttributeError: if no value is found for the structured grid file path
+            ValueError: if when loading the grid no values can be found for the NX NY NZ line.
+        """
+        if structured_grid_file.location is None:
+            raise ValueError(f"No file path given or found for structured grid file path. \
+                Instead got {structured_grid_file.location}")
+
+        loaded_structured_grid_file = cls(grid_nexus_file=structured_grid_file)
+
+        if not lazy_loading:
+            loaded_structured_grid_file.load_grid_properties_if_not_loaded()
+            loaded_structured_grid_file.load_faults()
+            loaded_structured_grid_file.load_array_functions()
+
+        return loaded_structured_grid_file
+
+    @staticmethod
+    def update_structured_grid_file(grid_dict: dict[str, VariableEntry | int], model: NexusSimulator) -> None:
+        """Save values passed from the front end to the structured grid file and update the class.
+
+        Args:
+        ----
+            grid_dict (dict[str, Union[VariableEntry, int]]): dictionary containing grid properties to be replaced
+            model (NexusSimulator): an instance of a NexusSimulator object
+        Raises:
+            ValueError: If no structured grid file is in the instance of the Simulator class
+        """
+        # Convert the dictionary back to a class, and update the properties on our class
+        structured_grid = model.grid
+        if structured_grid is None or model.model_files.structured_grid_file is None:
+            raise ValueError("Model does not contain a structured grid")
+        original_structured_grid_file = copy.deepcopy(structured_grid)
+
+        # replace the structured grid with a new object with an updated dictionary
+        structured_grid.update_properties_from_dict(grid_dict)
+
+        # change it in the text file for nexus:
+        grid_file_path = model.model_files.structured_grid_file.location
+        if grid_file_path is None:
+            raise ValueError("No path found for structured grid file path.")
+        structured_grid_contents = nfo.load_file_as_list(grid_file_path)
+        # Get the existing file as a list
+        if structured_grid_contents is None:
+            raise ValueError("No path found for structured grid file path. \
+                Please provide a path to the structured grid")
+        # Update each value in the file
+        StructuredGridOperations.replace_value(structured_grid_contents, original_structured_grid_file.netgrs,
+                                               structured_grid.netgrs, 'NETGRS')
+        StructuredGridOperations.replace_value(structured_grid_contents, original_structured_grid_file.porosity,
+                                               structured_grid.porosity, 'POROSITY')
+        StructuredGridOperations.replace_value(structured_grid_contents, original_structured_grid_file.sw,
+                                               structured_grid.sw, 'SW')
+        StructuredGridOperations.replace_value(structured_grid_contents, original_structured_grid_file.kx,
+                                               structured_grid.kx, 'KX')
+        StructuredGridOperations.replace_value(structured_grid_contents, original_structured_grid_file.ky,
+                                               structured_grid.ky, 'KY')
+        StructuredGridOperations.replace_value(structured_grid_contents, original_structured_grid_file.kz,
+                                               structured_grid.kz, 'KZ')
+
+        # Save the new file contents
+        new_file_str = "".join(structured_grid_contents)
+        with open(grid_file_path, "w") as text_file:
+            text_file.write(new_file_str)
+
+    def load_array_functions(self) -> None:
+        if self.__grid_file_contents is None:
+            raise ValueError("Cannot load array functions as grid file cannot not found")
+        self.__array_functions_list = afo.collect_all_function_blocks(self.__grid_file_contents)
+        self.__array_functions_df = afo.summarize_model_functions(self.__array_functions_list)
+        self.__array_functions_loaded = True
+
+    def get_array_functions_list(self) -> Optional[list[list[str]]]:
+        """Returns the grid array functions as a list of function lines."""
+        if not self.__array_functions_loaded:
+            self.load_array_functions()
+        return self.__array_functions_list
+
+    def get_array_functions_df(self) -> Optional[pd.DataFrame]:
+        """Returns the grid array functions as a dataframe."""
+        if not self.__array_functions_loaded:
+            self.load_array_functions()
+        return self.__array_functions_df
+
+    def load_faults(self) -> None:
+        """Function to read faults in Nexus grid file defined using MULT and FNAME keywords."""
+        file_content_as_list = self.__grid_file_contents
+        if file_content_as_list is None:
+            raise ValueError('Grid file contents have not been loaded')
+        df = load_nexus_fault_mult_table_from_list(file_content_as_list)
+
+        if not df.empty:
+            # Ensure resulting dataframe has uppercase column names
+            df.columns = [col.upper() for col in df.columns]
+
+            # Check if any multfls have been used in grid file and update fault trans multipliers accordingly
+            f_names = df['NAME'].unique()
+            f_mults = [1.] * len(f_names)
+            mult_dict = dict(zip(f_names, f_mults))
+            for line in file_content_as_list:
+                if nfo.check_token('MULTFL', line):
+                    fname = str(nfo.get_expected_token_value(
+                        'MULTFL', line, file_content_as_list,
+                        custom_message=f'{line} does not have a fault name following MULTFL'))
+                    if fname in df['NAME'].unique():
+                        tmult = float(str(nfo.get_expected_token_value(
+                            fname, line, file_content_as_list,
+                            custom_message=f'MULTFL {fname} does not have a numerical tmult value')))
+                        mult_dict[fname] *= tmult
+            mult_df = pd.DataFrame.from_dict(mult_dict, orient='index').reset_index()
+            mult_df.columns = ['NAME', 'TMULT']
+            new_df = df.merge(mult_df, how='left', on='NAME', validate='many_to_one')
+            new_df['MULT'] = new_df['MULT'] * new_df['TMULT']
+            self.__faults_df = new_df.drop(['TMULT'], axis=1)
+        self.__grid_faults_loaded = True
+
+    def get_faults_df(self) -> Optional[pd.DataFrame]:
+        """Returns the fault definition and transmissility multiplier information as a dataframe."""
+
+        if not self.__grid_faults_loaded:
+            self.load_faults()
+        return self.__faults_df
```

### Comparing `ressimpy-1.0.0/ResSimpy/Nexus/load_wells.py` & `ressimpy-1.0.1/ResSimpy/Nexus/load_wells.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,331 +1,331 @@
-from typing import Optional
-from ResSimpy.Nexus.NexusEnums.DateFormatEnum import DateFormat
-
-import ResSimpy.Nexus.nexus_file_operations as nfo
-from ResSimpy.Nexus.DataModels.NexusFile import NexusFile
-from ResSimpy.Nexus.DataModels.NexusWell import NexusWell
-from ResSimpy.Nexus.DataModels.NexusCompletion import NexusCompletion
-from ResSimpy.Nexus.DataModels.NexusRelPermEndPoint import NexusRelPermEndPoint
-
-from ResSimpy.Enums.UnitsEnum import UnitSystem
-from ResSimpy.Nexus.NexusKeywords.wells_keywords import WELLS_KEYWORDS
-
-
-def load_wells(nexus_file: NexusFile, start_date: str, default_units: UnitSystem,
-               date_format: DateFormat) -> list[NexusWell]:
-    """Loads a list of Nexus Well instances and populates it with the wells completions over time from a wells file.
-
-    Args:
-        nexus_file (NexusFile): NexusFile containing the wellspec files.
-        start_date (str): starting date of the wellspec file as a string.
-        default_units (UnitSystem): default units to use if no units are found.
-        date_format (DateFormat): Date format specified in the FCS file.
-
-    Raises:
-        ValueError: If no value is found after a TIME card.
-        ValueError: If no well name is found after a WELLSPEC keyword.
-        ValueError: If no valid wells are found in the wellspec file.
-
-    Returns:
-        list[NexusWell]: list of Nexus well classes contained within a wellspec file.
-    """
-
-    file_as_list = nexus_file.get_flat_list_str_file
-    well_name: Optional[str] = None
-    wellspec_file_units: Optional[UnitSystem] = None
-
-    iw: Optional[str] = None
-    jw: Optional[str] = None
-    kw: Optional[str] = None
-    md: Optional[str] = None
-    skin: Optional[str] = None
-    depth: Optional[str] = None
-    x_value: Optional[str] = None
-    y_value: Optional[str] = None
-    angla: Optional[str] = None
-    anglv: Optional[str] = None
-    grid: Optional[str] = None
-    wi: Optional[str] = None
-    dtop: Optional[str] = None
-    dbot: Optional[str] = None
-    partial_perf: Optional[str] = None
-    well_radius: Optional[str] = None
-
-    perm_thickness_ovr: Optional[str] = None
-    dfactor: Optional[str] = None
-    rel_perm_method: Optional[str] = None
-    status: Optional[str] = None
-
-    cell_number: Optional[str] = None
-    bore_radius: Optional[str] = None
-    portype: Optional[str] = None
-    fracture_mult: Optional[str] = None
-    sector: Optional[str] = None
-    well_group: Optional[str] = None
-    zone: Optional[str] = None
-    angle_open_flow: Optional[str] = None
-    temperature: Optional[str] = None
-    flowsector: Optional[str] = None
-    parent_node: Optional[str] = None
-    mdcon: Optional[str] = None
-    pressure_avg_pattern: Optional[str] = None
-    length: Optional[str] = None
-    permeability: Optional[str] = None
-    non_darcy_model: Optional[str] = None
-    comp_dz: Optional[str] = None
-    layer_assignment: Optional[str] = None
-    polymer_bore_radius: Optional[str] = None
-    polymer_well_radius: Optional[str] = None
-    kh_mult: Optional[float] = None
-
-    # End point values:
-    swl: Optional[str] = None
-    swr: Optional[str] = None
-    swu: Optional[str] = None
-    sgl: Optional[str] = None
-    sgr: Optional[str] = None
-    sgu: Optional[str] = None
-    swro: Optional[str] = None
-    sgro: Optional[str] = None
-    sgrw: Optional[str] = None
-    krw_swro: Optional[str] = None
-    krw_swu: Optional[str] = None
-    krg_sgro: Optional[str] = None
-    krg_sgu: Optional[str] = None
-    kro_swl: Optional[str] = None
-    kro_swr: Optional[str] = None
-    kro_sgl: Optional[str] = None
-    kro_sgr: Optional[str] = None
-    krw_sgl: Optional[str] = None
-    krw_sgr: Optional[str] = None
-    krg_sgrw: Optional[str] = None
-    sgtr: Optional[str] = None
-    sotr: Optional[str] = None
-    header_values: dict[str, None | int | float | str] = {
-        'IW': iw, 'JW': jw, 'L': kw, 'MD': md, 'SKIN': skin, 'DEPTH': depth, 'X': x_value, 'Y': y_value,
-        'ANGLA': angla, 'ANGLV': anglv, 'GRID': grid, 'WI': wi, 'DTOP': dtop, 'DBOT': dbot, 'RADW': well_radius,
-        'PPERF': partial_perf, 'CELL': cell_number, 'KH': perm_thickness_ovr, 'D': dfactor, 'IRELPM': rel_perm_method,
-        'STAT': status, 'RADB': bore_radius, 'PORTYPE': portype, 'FM': fracture_mult, 'SECT': sector,
-        'GROUP': well_group, 'ZONE': zone, 'ANGLE': angle_open_flow, 'TEMP': temperature, 'FLOWSECT': flowsector,
-        'PARENT': parent_node, 'MDCON': mdcon, 'IPTN': pressure_avg_pattern, 'LENGTH': length, 'K': permeability,
-        'ND': non_darcy_model, 'DZ': comp_dz, 'LAYER': layer_assignment, 'RADBP': polymer_bore_radius,
-        'RADWP': polymer_well_radius, 'KHMULT': kh_mult
-        }
-    end_point_scaling_header_values: dict[str, None | int | float | str] = {
-        'SWL': swl, 'SWR': swr, 'SWU': swu, 'SGL': sgl, 'SGR': sgr, 'SGU': sgu,
-        'SWRO': swro, 'SGRO': sgro, 'SGRW': sgrw, 'KRW_SWRO': krw_swro, 'KRW_SWU': krw_swu, 'KRG_SGRO': krg_sgro,
-        'KRG_SGU': krg_sgu, 'KRO_SWL': kro_swl, 'KRO_SWR': kro_swr, 'KRO_SGL': kro_sgl, 'KRO_SGR': kro_sgr,
-        'KRW_SGL': krw_sgl, 'KRW_SGR': krw_sgr, 'KRG_SGRW': krg_sgrw, 'SGTR': sgtr, 'SOTR': sotr,
-        }
-    # add end point scaling header to the header values we search for:
-    header_values.update(end_point_scaling_header_values)
-
-    header_index: int = -1
-    wellspec_found: bool = False
-    current_date: Optional[str] = None
-    wells: list[NexusWell] = []
-    well_name_list: list[str] = []
-
-    for index, line in enumerate(file_as_list):
-        uppercase_line = line.upper()
-
-        # If we haven't got the units yet, check to see if this line contains a declaration for them.
-        if wellspec_file_units is None:
-            for unit in UnitSystem:
-                if unit.value in uppercase_line and (line.find('!') > line.find(unit.value) or line.find('!') == -1):
-                    wellspec_file_units = unit
-
-        if nfo.check_token('TIME', line):
-            current_date = nfo.get_token_value(token='TIME', token_line=line, file_list=file_as_list)
-            if current_date is None:
-                raise ValueError(f"Cannot find the date associated with the TIME card in {line=} at line number \
-                                 {index}")
-
-        if nfo.check_token('WELLSPEC', uppercase_line):
-            initial_well_name = nfo.get_expected_token_value(token='WELLSPEC', token_line=line, file_list=file_as_list,
-                                                             custom_message="Cannot find well name following WELLSPEC "
-                                                                            "keyword")
-            well_name = initial_well_name.strip('\"')
-            wellspec_found = True
-            continue
-
-        # Load in the column headings, which appear after the well name
-        header_index, headers = __load_wellspec_table_headings(header_index, header_values, index, line, well_name)
-
-        if header_index == -1:
-            continue
-
-        if well_name is None:
-            raise ValueError(f"No wells found in file: {nexus_file.location}")
-
-        if wellspec_found:
-            if current_date is None:
-                current_date = start_date
-            # reset the storage dictionary to prevent completion properties being carried forward from earlier timestep
-            header_values = {k: None for k in header_values}
-            # Load in each line of the table
-            completions = __load_wellspec_table_completions(
-                nexus_file, header_index, header_values, headers, current_date, end_point_scaling_header_values,
-                date_format)
-
-            if wellspec_file_units is None:
-                wellspec_file_units = default_units
-
-            if well_name in well_name_list:
-                wells[well_name_list.index(well_name)].completions.extend(completions)
-            else:
-                new_well = NexusWell(completions=completions, well_name=well_name, units=wellspec_file_units)
-                well_name_list.append(well_name)
-                wells.append(new_well)
-            wellspec_found = False
-    return wells
-
-
-def __load_wellspec_table_completions(nexus_file: NexusFile, header_index: int,
-                                      header_values: dict[str, None | int | float | str],
-                                      headers: list[str], start_date: str,
-                                      end_point_scaling_header_values: dict[str, None | int | float | str],
-                                      date_format: DateFormat
-                                      ) -> list[NexusCompletion]:
-    """Loads a completion table in for a single WELLSPEC keyword. \
-        Loads in the next available completions following a WELLSPEC keyword and a header line.
-
-    Args:
-        header_index (int): index number of the header in the file as list parameter
-        header_values (dict[str, Union[Optional[int], Optional[float], Optional[str]]]): dictionary of column \
-            headings to populate from the table
-        headers (list[str]): list of strings containing the headers from the wellspec table
-        start_date (str): date to populate the completion class with.
-
-    Returns:
-        list[NexusCompletion]: list of nexus completions for a given table.
-    """
-
-    def convert_header_value_float(key: str) -> Optional[float]:
-        value = header_values[key]
-        if value == 'NA':
-            value = None
-        return None if value is None else float(value)
-
-    def convert_header_value_int(key: str) -> Optional[int]:
-        value = header_values[key]
-        if value == 'NA':
-            value = None
-        return None if value is None else int(value)
-
-    completions: list[NexusCompletion] = []
-    file_as_list: list[str] = nexus_file.get_flat_list_str_file
-
-    for index, line in enumerate(file_as_list[header_index + 1:]):
-        # check for end of table lines:
-        # TODO update with a more robust table end checker function
-        end_of_table = nfo.nexus_token_found(line, WELLS_KEYWORDS)
-        if end_of_table:
-            return completions
-        valid_line, header_values = nfo.table_line_reader(header_values, headers, line)
-        # if a valid line is found load a completion otherwise continue
-        if not valid_line:
-            continue
-
-        # create a rel perm end point scaling object if it exists for a given completion
-        rel_perm_dict = {key.lower(): convert_header_value_float(key) for key
-                         in header_values if key in end_point_scaling_header_values}
-        if any(rel_perm_dict.values()):
-            new_rel_perm_end_point = NexusRelPermEndPoint(**rel_perm_dict)
-        else:
-            new_rel_perm_end_point = None
-
-        new_completion = NexusCompletion(
-            i=convert_header_value_int('IW'),
-            j=convert_header_value_int('JW'),
-            k=convert_header_value_int('L'),
-            # keep grid = 'NA' as 'NA' and not None
-            grid=(None if header_values['GRID'] is None else str(header_values['GRID'])),
-            well_radius=convert_header_value_float('RADW'),
-            measured_depth=convert_header_value_float('MD'),
-            skin=convert_header_value_float('SKIN'),
-            depth=convert_header_value_float('DEPTH'),
-            x=convert_header_value_float('X'),
-            y=convert_header_value_float('Y'),
-            angle_a=convert_header_value_float('ANGLA'),
-            angle_v=convert_header_value_float('ANGLV'),
-            well_indices=convert_header_value_float('WI'),
-            depth_to_top=convert_header_value_float('DTOP'),
-            depth_to_bottom=convert_header_value_float('DBOT'),
-            partial_perf=convert_header_value_float('PPERF'),
-            cell_number=convert_header_value_int('CELL'),
-            perm_thickness_ovr=convert_header_value_float('KH'),
-            dfactor=convert_header_value_float('D'),
-            rel_perm_method=convert_header_value_int('IRELPM'),
-            status=(None if header_values['STAT'] is None else str(header_values['STAT'])),
-            bore_radius=convert_header_value_float('RADB'),
-            portype=(None if header_values['PORTYPE'] is None else str(header_values['PORTYPE'])),
-            fracture_mult=convert_header_value_float('FM'),
-            sector=convert_header_value_int('SECT'),
-            well_group=(None if header_values['GROUP'] is None else str(header_values['GROUP'])),
-            zone=convert_header_value_int('ZONE'),
-            angle_open_flow=convert_header_value_float('ANGLE'),
-            temperature=convert_header_value_float('TEMP'),
-            flowsector=convert_header_value_int('FLOWSECT'),
-            parent_node=(None if header_values['PARENT'] is None else str(header_values['PARENT'])),
-            mdcon=convert_header_value_float('MDCON'),
-            pressure_avg_pattern=convert_header_value_int('IPTN'),
-            length=convert_header_value_float('LENGTH'),
-            permeability=convert_header_value_float('K'),
-            non_darcy_model=(None if header_values['ND'] is None else str(header_values['ND'])),
-            comp_dz=convert_header_value_float('DZ'),
-            layer_assignment=convert_header_value_int('LAYER'),
-            polymer_bore_radius=convert_header_value_float('RADBP'),
-            polymer_well_radius=convert_header_value_float('RADWP'),
-            rel_perm_end_point=new_rel_perm_end_point,
-            date=start_date,
-            kh_mult=convert_header_value_float('KHMULT'),
-            date_format=date_format
-            )
-
-        nexus_file.add_object_locations(new_completion.id, [index + header_index + 1])
-
-        completions.append(new_completion)
-
-    return completions
-
-
-def __load_wellspec_table_headings(header_index: int, header_values: dict[str, None | int | float | str],
-                                   index: int, line: str, well_name: Optional[str],
-                                   headers: Optional[list[str]] = None) -> tuple[int, list[str]]:
-    """Loads in the wellspec headers from a line in a file.
-
-    Args:
-        header_index (int): index of the header
-        header_values (dict[str, Union[Optional[int], Optional[float], Optional[str]]]): dictionary of column \
-            headings to populate from the table
-        index (int): starting index to search from
-        line (str): line to extract header values from
-        well_name (Optional[str]): well name from the previous WELLSPEC keyword
-        headers (Optional[list[str]], optional): list of headers to append the next set of found headers to. \
-            Defaults to None and will create a new list to return if None.
-
-    Returns:
-        tuple[int, list[str]]: index in the file as list for the header, list of headers found in the file
-    """
-    headers = [] if headers is None else headers
-    next_column_heading: Optional[str]
-    if well_name is None:
-        return header_index, headers
-
-    for key in header_values.keys():
-        if nfo.check_token(key, line):
-            header_line = line.upper()
-            header_index = index
-            # Map the headers (first time get the expected value as check token guarantees at least 1 value)
-            next_column_heading = nfo.get_expected_next_value(start_line_index=0, file_as_list=[line]).upper()
-            trimmed_line = header_line
-
-            while next_column_heading is not None:
-                headers.append(next_column_heading)
-                trimmed_line = trimmed_line.replace(next_column_heading, "", 1)
-                next_column_heading = nfo.get_next_value(0, [trimmed_line], trimmed_line)
-
-            if len(headers) > 0:
-                break
-    return header_index, headers
+from typing import Optional
+from ResSimpy.Nexus.NexusEnums.DateFormatEnum import DateFormat
+
+import ResSimpy.Nexus.nexus_file_operations as nfo
+from ResSimpy.Nexus.DataModels.NexusFile import NexusFile
+from ResSimpy.Nexus.DataModels.NexusWell import NexusWell
+from ResSimpy.Nexus.DataModels.NexusCompletion import NexusCompletion
+from ResSimpy.Nexus.DataModels.NexusRelPermEndPoint import NexusRelPermEndPoint
+
+from ResSimpy.Enums.UnitsEnum import UnitSystem
+from ResSimpy.Nexus.NexusKeywords.wells_keywords import WELLS_KEYWORDS
+
+
+def load_wells(nexus_file: NexusFile, start_date: str, default_units: UnitSystem,
+               date_format: DateFormat) -> list[NexusWell]:
+    """Loads a list of Nexus Well instances and populates it with the wells completions over time from a wells file.
+
+    Args:
+        nexus_file (NexusFile): NexusFile containing the wellspec files.
+        start_date (str): starting date of the wellspec file as a string.
+        default_units (UnitSystem): default units to use if no units are found.
+        date_format (DateFormat): Date format specified in the FCS file.
+
+    Raises:
+        ValueError: If no value is found after a TIME card.
+        ValueError: If no well name is found after a WELLSPEC keyword.
+        ValueError: If no valid wells are found in the wellspec file.
+
+    Returns:
+        list[NexusWell]: list of Nexus well classes contained within a wellspec file.
+    """
+
+    file_as_list = nexus_file.get_flat_list_str_file
+    well_name: Optional[str] = None
+    wellspec_file_units: Optional[UnitSystem] = None
+
+    iw: Optional[str] = None
+    jw: Optional[str] = None
+    kw: Optional[str] = None
+    md: Optional[str] = None
+    skin: Optional[str] = None
+    depth: Optional[str] = None
+    x_value: Optional[str] = None
+    y_value: Optional[str] = None
+    angla: Optional[str] = None
+    anglv: Optional[str] = None
+    grid: Optional[str] = None
+    wi: Optional[str] = None
+    dtop: Optional[str] = None
+    dbot: Optional[str] = None
+    partial_perf: Optional[str] = None
+    well_radius: Optional[str] = None
+
+    perm_thickness_ovr: Optional[str] = None
+    dfactor: Optional[str] = None
+    rel_perm_method: Optional[str] = None
+    status: Optional[str] = None
+
+    cell_number: Optional[str] = None
+    bore_radius: Optional[str] = None
+    portype: Optional[str] = None
+    fracture_mult: Optional[str] = None
+    sector: Optional[str] = None
+    well_group: Optional[str] = None
+    zone: Optional[str] = None
+    angle_open_flow: Optional[str] = None
+    temperature: Optional[str] = None
+    flowsector: Optional[str] = None
+    parent_node: Optional[str] = None
+    mdcon: Optional[str] = None
+    pressure_avg_pattern: Optional[str] = None
+    length: Optional[str] = None
+    permeability: Optional[str] = None
+    non_darcy_model: Optional[str] = None
+    comp_dz: Optional[str] = None
+    layer_assignment: Optional[str] = None
+    polymer_bore_radius: Optional[str] = None
+    polymer_well_radius: Optional[str] = None
+    kh_mult: Optional[float] = None
+
+    # End point values:
+    swl: Optional[str] = None
+    swr: Optional[str] = None
+    swu: Optional[str] = None
+    sgl: Optional[str] = None
+    sgr: Optional[str] = None
+    sgu: Optional[str] = None
+    swro: Optional[str] = None
+    sgro: Optional[str] = None
+    sgrw: Optional[str] = None
+    krw_swro: Optional[str] = None
+    krw_swu: Optional[str] = None
+    krg_sgro: Optional[str] = None
+    krg_sgu: Optional[str] = None
+    kro_swl: Optional[str] = None
+    kro_swr: Optional[str] = None
+    kro_sgl: Optional[str] = None
+    kro_sgr: Optional[str] = None
+    krw_sgl: Optional[str] = None
+    krw_sgr: Optional[str] = None
+    krg_sgrw: Optional[str] = None
+    sgtr: Optional[str] = None
+    sotr: Optional[str] = None
+    header_values: dict[str, None | int | float | str] = {
+        'IW': iw, 'JW': jw, 'L': kw, 'MD': md, 'SKIN': skin, 'DEPTH': depth, 'X': x_value, 'Y': y_value,
+        'ANGLA': angla, 'ANGLV': anglv, 'GRID': grid, 'WI': wi, 'DTOP': dtop, 'DBOT': dbot, 'RADW': well_radius,
+        'PPERF': partial_perf, 'CELL': cell_number, 'KH': perm_thickness_ovr, 'D': dfactor, 'IRELPM': rel_perm_method,
+        'STAT': status, 'RADB': bore_radius, 'PORTYPE': portype, 'FM': fracture_mult, 'SECT': sector,
+        'GROUP': well_group, 'ZONE': zone, 'ANGLE': angle_open_flow, 'TEMP': temperature, 'FLOWSECT': flowsector,
+        'PARENT': parent_node, 'MDCON': mdcon, 'IPTN': pressure_avg_pattern, 'LENGTH': length, 'K': permeability,
+        'ND': non_darcy_model, 'DZ': comp_dz, 'LAYER': layer_assignment, 'RADBP': polymer_bore_radius,
+        'RADWP': polymer_well_radius, 'KHMULT': kh_mult
+        }
+    end_point_scaling_header_values: dict[str, None | int | float | str] = {
+        'SWL': swl, 'SWR': swr, 'SWU': swu, 'SGL': sgl, 'SGR': sgr, 'SGU': sgu,
+        'SWRO': swro, 'SGRO': sgro, 'SGRW': sgrw, 'KRW_SWRO': krw_swro, 'KRW_SWU': krw_swu, 'KRG_SGRO': krg_sgro,
+        'KRG_SGU': krg_sgu, 'KRO_SWL': kro_swl, 'KRO_SWR': kro_swr, 'KRO_SGL': kro_sgl, 'KRO_SGR': kro_sgr,
+        'KRW_SGL': krw_sgl, 'KRW_SGR': krw_sgr, 'KRG_SGRW': krg_sgrw, 'SGTR': sgtr, 'SOTR': sotr,
+        }
+    # add end point scaling header to the header values we search for:
+    header_values.update(end_point_scaling_header_values)
+
+    header_index: int = -1
+    wellspec_found: bool = False
+    current_date: Optional[str] = None
+    wells: list[NexusWell] = []
+    well_name_list: list[str] = []
+
+    for index, line in enumerate(file_as_list):
+        uppercase_line = line.upper()
+
+        # If we haven't got the units yet, check to see if this line contains a declaration for them.
+        if wellspec_file_units is None:
+            for unit in UnitSystem:
+                if unit.value in uppercase_line and (line.find('!') > line.find(unit.value) or line.find('!') == -1):
+                    wellspec_file_units = unit
+
+        if nfo.check_token('TIME', line):
+            current_date = nfo.get_token_value(token='TIME', token_line=line, file_list=file_as_list)
+            if current_date is None:
+                raise ValueError(f"Cannot find the date associated with the TIME card in {line=} at line number \
+                                 {index}")
+
+        if nfo.check_token('WELLSPEC', uppercase_line):
+            initial_well_name = nfo.get_expected_token_value(token='WELLSPEC', token_line=line, file_list=file_as_list,
+                                                             custom_message="Cannot find well name following WELLSPEC "
+                                                                            "keyword")
+            well_name = initial_well_name.strip('\"')
+            wellspec_found = True
+            continue
+
+        # Load in the column headings, which appear after the well name
+        header_index, headers = __load_wellspec_table_headings(header_index, header_values, index, line, well_name)
+
+        if header_index == -1:
+            continue
+
+        if well_name is None:
+            raise ValueError(f"No wells found in file: {nexus_file.location}")
+
+        if wellspec_found:
+            if current_date is None:
+                current_date = start_date
+            # reset the storage dictionary to prevent completion properties being carried forward from earlier timestep
+            header_values = {k: None for k in header_values}
+            # Load in each line of the table
+            completions = __load_wellspec_table_completions(
+                nexus_file, header_index, header_values, headers, current_date, end_point_scaling_header_values,
+                date_format)
+
+            if wellspec_file_units is None:
+                wellspec_file_units = default_units
+
+            if well_name in well_name_list:
+                wells[well_name_list.index(well_name)].completions.extend(completions)
+            else:
+                new_well = NexusWell(completions=completions, well_name=well_name, units=wellspec_file_units)
+                well_name_list.append(well_name)
+                wells.append(new_well)
+            wellspec_found = False
+    return wells
+
+
+def __load_wellspec_table_completions(nexus_file: NexusFile, header_index: int,
+                                      header_values: dict[str, None | int | float | str],
+                                      headers: list[str], start_date: str,
+                                      end_point_scaling_header_values: dict[str, None | int | float | str],
+                                      date_format: DateFormat
+                                      ) -> list[NexusCompletion]:
+    """Loads a completion table in for a single WELLSPEC keyword. \
+        Loads in the next available completions following a WELLSPEC keyword and a header line.
+
+    Args:
+        header_index (int): index number of the header in the file as list parameter
+        header_values (dict[str, Union[Optional[int], Optional[float], Optional[str]]]): dictionary of column \
+            headings to populate from the table
+        headers (list[str]): list of strings containing the headers from the wellspec table
+        start_date (str): date to populate the completion class with.
+
+    Returns:
+        list[NexusCompletion]: list of nexus completions for a given table.
+    """
+
+    def convert_header_value_float(key: str) -> Optional[float]:
+        value = header_values[key]
+        if value == 'NA':
+            value = None
+        return None if value is None else float(value)
+
+    def convert_header_value_int(key: str) -> Optional[int]:
+        value = header_values[key]
+        if value == 'NA':
+            value = None
+        return None if value is None else int(value)
+
+    completions: list[NexusCompletion] = []
+    file_as_list: list[str] = nexus_file.get_flat_list_str_file
+
+    for index, line in enumerate(file_as_list[header_index + 1:]):
+        # check for end of table lines:
+        # TODO update with a more robust table end checker function
+        end_of_table = nfo.nexus_token_found(line, WELLS_KEYWORDS)
+        if end_of_table:
+            return completions
+        valid_line, header_values = nfo.table_line_reader(header_values, headers, line)
+        # if a valid line is found load a completion otherwise continue
+        if not valid_line:
+            continue
+
+        # create a rel perm end point scaling object if it exists for a given completion
+        rel_perm_dict = {key.lower(): convert_header_value_float(key) for key
+                         in header_values if key in end_point_scaling_header_values}
+        if any(rel_perm_dict.values()):
+            new_rel_perm_end_point = NexusRelPermEndPoint(**rel_perm_dict)
+        else:
+            new_rel_perm_end_point = None
+
+        new_completion = NexusCompletion(
+            i=convert_header_value_int('IW'),
+            j=convert_header_value_int('JW'),
+            k=convert_header_value_int('L'),
+            # keep grid = 'NA' as 'NA' and not None
+            grid=(None if header_values['GRID'] is None else str(header_values['GRID'])),
+            well_radius=convert_header_value_float('RADW'),
+            measured_depth=convert_header_value_float('MD'),
+            skin=convert_header_value_float('SKIN'),
+            depth=convert_header_value_float('DEPTH'),
+            x=convert_header_value_float('X'),
+            y=convert_header_value_float('Y'),
+            angle_a=convert_header_value_float('ANGLA'),
+            angle_v=convert_header_value_float('ANGLV'),
+            well_indices=convert_header_value_float('WI'),
+            depth_to_top=convert_header_value_float('DTOP'),
+            depth_to_bottom=convert_header_value_float('DBOT'),
+            partial_perf=convert_header_value_float('PPERF'),
+            cell_number=convert_header_value_int('CELL'),
+            perm_thickness_ovr=convert_header_value_float('KH'),
+            dfactor=convert_header_value_float('D'),
+            rel_perm_method=convert_header_value_int('IRELPM'),
+            status=(None if header_values['STAT'] is None else str(header_values['STAT'])),
+            bore_radius=convert_header_value_float('RADB'),
+            portype=(None if header_values['PORTYPE'] is None else str(header_values['PORTYPE'])),
+            fracture_mult=convert_header_value_float('FM'),
+            sector=convert_header_value_int('SECT'),
+            well_group=(None if header_values['GROUP'] is None else str(header_values['GROUP'])),
+            zone=convert_header_value_int('ZONE'),
+            angle_open_flow=convert_header_value_float('ANGLE'),
+            temperature=convert_header_value_float('TEMP'),
+            flowsector=convert_header_value_int('FLOWSECT'),
+            parent_node=(None if header_values['PARENT'] is None else str(header_values['PARENT'])),
+            mdcon=convert_header_value_float('MDCON'),
+            pressure_avg_pattern=convert_header_value_int('IPTN'),
+            length=convert_header_value_float('LENGTH'),
+            permeability=convert_header_value_float('K'),
+            non_darcy_model=(None if header_values['ND'] is None else str(header_values['ND'])),
+            comp_dz=convert_header_value_float('DZ'),
+            layer_assignment=convert_header_value_int('LAYER'),
+            polymer_bore_radius=convert_header_value_float('RADBP'),
+            polymer_well_radius=convert_header_value_float('RADWP'),
+            rel_perm_end_point=new_rel_perm_end_point,
+            date=start_date,
+            kh_mult=convert_header_value_float('KHMULT'),
+            date_format=date_format
+            )
+
+        nexus_file.add_object_locations(new_completion.id, [index + header_index + 1])
+
+        completions.append(new_completion)
+
+    return completions
+
+
+def __load_wellspec_table_headings(header_index: int, header_values: dict[str, None | int | float | str],
+                                   index: int, line: str, well_name: Optional[str],
+                                   headers: Optional[list[str]] = None) -> tuple[int, list[str]]:
+    """Loads in the wellspec headers from a line in a file.
+
+    Args:
+        header_index (int): index of the header
+        header_values (dict[str, Union[Optional[int], Optional[float], Optional[str]]]): dictionary of column \
+            headings to populate from the table
+        index (int): starting index to search from
+        line (str): line to extract header values from
+        well_name (Optional[str]): well name from the previous WELLSPEC keyword
+        headers (Optional[list[str]], optional): list of headers to append the next set of found headers to. \
+            Defaults to None and will create a new list to return if None.
+
+    Returns:
+        tuple[int, list[str]]: index in the file as list for the header, list of headers found in the file
+    """
+    headers = [] if headers is None else headers
+    next_column_heading: Optional[str]
+    if well_name is None:
+        return header_index, headers
+
+    for key in header_values.keys():
+        if nfo.check_token(key, line):
+            header_line = line.upper()
+            header_index = index
+            # Map the headers (first time get the expected value as check token guarantees at least 1 value)
+            next_column_heading = nfo.get_expected_next_value(start_line_index=0, file_as_list=[line]).upper()
+            trimmed_line = header_line
+
+            while next_column_heading is not None:
+                headers.append(next_column_heading)
+                trimmed_line = trimmed_line.replace(next_column_heading, "", 1)
+                next_column_heading = nfo.get_next_value(0, [trimmed_line], trimmed_line)
+
+            if len(headers) > 0:
+                break
+    return header_index, headers
```

### Comparing `ressimpy-1.0.0/ResSimpy/Nexus/logfile_operations.py` & `ressimpy-1.0.1/ResSimpy/Nexus/logfile_operations.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,313 +1,313 @@
-from __future__ import annotations
-
-import os
-from datetime import datetime
-from typing import Optional, TYPE_CHECKING
-import ResSimpy.Nexus.nexus_file_operations as nfo
-
-if TYPE_CHECKING:
-    from ResSimpy.Nexus.NexusSimulator import NexusSimulator
-
-
-class Logging:
-    def __init__(self, model: NexusSimulator) -> None:
-        """Class for controlling all logging and logfile (*.log) related functionality.
-
-        Args:
-            model: NexusSimulator instance
-            __job_id (int): Run job ID for executed runs
-            __simulation_start_time (Optional[str]): Execution start time of the simulation when submitted \
-                to calculation engine
-            __simulation_end_time (Optional[str]): Execution end time of the last time the simulation was run
-            __previous_run_time (Optional[str]): Difference between simulation execution start time and end time.
-        """
-        self.__model = model
-        self.__job_id: int = -1
-        self.__simulation_start_time: Optional[str] = None
-        self.__simulation_end_time: Optional[str] = None
-        self.__previous_run_time: Optional[str] = None
-
-    @staticmethod
-    def get_simulation_time(line: str) -> str:
-        """Searches for the simulation time in a line.
-
-        Args:
-            line (str): line to search for the simulation time
-
-        Raises:
-            ValueError: Throws error if get_next_value doesn't find any subsequent value in the line
-
-        Returns:
-            str: value found after TIME card in a line
-        """
-        value_found = False
-        value = ''
-        line_string = line
-        while value_found is False:
-            next_value = nfo.get_next_value(0, [line_string], line_string)
-            if next_value is None:
-                raise ValueError(
-                    f'No next value found in the line supplied, line: {line_string}')
-            if next_value == 'on':
-                line_string = line_string.replace(next_value, '', 1)
-                next_value = nfo.get_next_value(0, [line_string], line_string)
-                if next_value is None:
-                    raise ValueError(
-                        f'No next value found in the line supplied, line: {line_string}')
-                for c in range(6):
-                    line_string = line_string.replace(next_value, '', 1)
-                    next_value = nfo.get_next_value(0, [line_string], line_string)
-                    if next_value is None:
-                        raise ValueError(
-                            f'No next value found in the line supplied, line: {line_string}')
-                    value += next_value + (' ' if c < 5 else '')
-                value_found = True
-            line_string = line_string.replace(next_value, '', 1)
-        return value
-
-    @staticmethod
-    def convert_server_date(original_date: str) -> datetime:
-        """Convert a datetime string from the server for when the simulation was started to a strptime object.
-
-        Args:
-            original_date (str): string of a date with format: "Mon Jan 01 00:00:00 CST 2020"
-
-        Returns:
-            datetime: datetime object derived from the input string
-        """
-
-        date_format = '%a %b %d %X %Z %Y'
-        converted_date = original_date
-
-        # Convert CDT and CST timezones as Python doesn't work with CDT for some reason
-        if 'CDT' in original_date:
-            converted_date = converted_date.replace('CDT', '-0500', 1)
-            date_format = '%a %b %d %X %z %Y'
-        elif 'CST' in original_date:
-            converted_date = converted_date.replace('CST', '-0600', 1)
-            date_format = '%a %b %d %X %z %Y'
-
-        return datetime.strptime(converted_date, date_format)
-
-    @staticmethod
-    def get_errors_warnings_string(log_file_line_list: list[str]) -> Optional[str]:
-        """Retrieves the number of warnings and errors from the simulation log output,
-        and formats them as a string.
-
-        Args:
-            log_file_line_list (list[str]): log file formatted as a list of strings with \
-                a new list entry per line
-
-        Returns:
-            Optional[str]: string containing the errors and warnings from the simulation log. \
-                None if error/warning set is too short
-        """
-        error_warning = ""
-        for line in log_file_line_list:
-            modified_line = line.lower()
-            if "errors" in modified_line and "warnings" in modified_line:
-                error_warning = modified_line
-
-        error_warning_list = [x for x in error_warning.split(" ") if x != ""]
-
-        error_warning_list = [nfo.clean_up_string(x) for x in error_warning_list]
-
-        if len(error_warning_list) < 4:
-            return None
-
-        errors = error_warning_list[1]
-        warnings = error_warning_list[3]
-
-        error_warning_str = f"Simulation complete - Errors: {errors} and Warnings: {warnings}"
-        return error_warning_str
-
-    def get_simulation_start_time(self) -> str:
-        """Get the start time of an executed simulation run, if no simulation start time returns '-'."""
-        self.get_simulation_status()
-        if self.__simulation_start_time is not None:
-            return self.__simulation_start_time
-        else:
-            return '-'
-
-    def get_simulation_end_time(self) -> str:
-        """Get the end time of an executed simulation run if it has completed, if no simulation end time returns '-'."""
-        self.get_simulation_status()
-        if self.__simulation_end_time is not None:
-            return self.__simulation_end_time
-        else:
-            return '-'
-
-    def get_job_id(self) -> int:
-        """Get the job Id of a simulation run."""
-        return self.__job_id
-
-    def __get_log_path(self, from_startup: bool = False) -> Optional[str]:
-        """Returns the path of the log file for the simulation.
-
-        Args:
-            from_startup (bool, optional): Searches the same directory as the original_fcs_file_path if True. \
-            Otherwise searches the destination folder path, failing this then searches the \
-            original_fcs_file_path if False. Defaults to False.
-
-        Returns:
-            Optional[str]: The path of the .log file from the simulation if found. If not found returns None.
-        """
-        folder_path = os.path.dirname(
-            self.__model.original_fcs_file_path) if from_startup else os.path.dirname(self.__model.origin)
-        files = os.listdir(folder_path)
-        original_fcs_file_location = os.path.basename(self.__model.original_fcs_file_path)
-        log_file_name = os.path.splitext(original_fcs_file_location)[
-                            0] + ".log" if from_startup else self.__model.root_name + ".log"
-
-        if log_file_name in files:
-            if from_startup:
-                file_location = folder_path
-            else:
-                file_location = self.__model.destination if self.__model.destination is not None else folder_path
-
-            log_file_path = file_location + "/" + log_file_name
-            return log_file_path
-        else:
-            return None
-
-    def __update_simulation_start_and_end_times(self, log_file_line_list: list[str]) -> None:
-        """Updates the stored simulation execution start and end times from the log files.
-
-        Args:
-            log_file_line_list (list[str]): log file information represented with a new entry per line of the file.
-        """
-        for line in log_file_line_list:
-            if nfo.check_token('start generic pdsh   prolog', line):
-                value = self.get_simulation_time(line)
-                self.__simulation_start_time = value
-
-            if nfo.check_token('end generic pdsh   epilog', line):
-                value = self.get_simulation_time(line)
-                self.__simulation_end_time = value
-
-    def get_simulation_status(self, from_startup: bool = False) -> Optional[str]:
-        """Gets the run status of the latest simulation run.
-
-        Args:
-            from_startup (bool, optional): Searches the same directory as the original_fcs_file_path if True. \
-            Otherwise searches the destination folder path, failing this then searches the \
-            original_fcs_file_path if False. Defaults to False.
-
-        Raises:
-            NotImplementedError: If log file is not found - only supporting simulation status from log files
-
-        Returns:
-            Optional[str]: the error/warning string if the simulation has finished, otherwise \
-                returns the running job ID. Empty string if a logfile is not found and from_start up is True
-        """
-        log_file = self.__get_log_path(from_startup)
-        if log_file is None:
-            if from_startup:
-                return ''
-            raise NotImplementedError(
-                "Only retrieving status from a log file is supported at the moment")
-        else:
-            log_file_line_list = nfo.load_file_as_list(log_file)
-            self.__update_simulation_start_and_end_times(log_file_line_list)
-            job_finished = 'Nexus finished\n' in log_file_line_list
-            if job_finished:
-                self.__previous_run_time = self.__get_start_end_difference() if from_startup \
-                    else self.__previous_run_time
-                return self.get_errors_warnings_string(log_file_line_list=log_file_line_list)
-            else:
-                job_number_line = [
-                    x for x in log_file_line_list if 'Job number:' in x]
-                if len(job_number_line) > 0:
-                    self.__job_id = int(job_number_line[0].split(":")[1])
-                    return f"Job Running, ID: {self.__job_id}"
-        return None
-
-    def __get_start_end_difference(self) -> Optional[str]:
-        """Returns a string with the previous time taken when the base case was run.
-
-        Returns:
-            Optional[str]: returns a human readable string of how long the simulation took to run
-        """
-        if self.__simulation_start_time is None or self.__simulation_end_time is None:
-            return None
-
-        start_date = self.convert_server_date(self.__simulation_start_time)
-        end_date = self.convert_server_date(self.__simulation_end_time)
-
-        total_difference = (end_date - start_date)
-        days = int(total_difference.days)
-        hours = int(total_difference.seconds / (60 * 60))
-        minutes = int((total_difference.seconds / 60) - (hours * 60))
-        seconds = int(total_difference.seconds -
-                      (hours * 60 * 60) - (minutes * 60))
-
-        return f"{days} Days, {hours} Hours, {minutes} Minutes {seconds} Seconds"
-
-    def get_base_case_run_time(self) -> str:
-        """Get the time taken for the base case to run. Returns '-' if no run time found."""
-        if self.__previous_run_time is not None:
-            return self.__previous_run_time
-        else:
-            return '-'
-
-    def get_simulation_progress(self) -> float:
-        """Returns the simulation progress from log files.
-
-        Raises:
-            NotImplementedError: Only retrieving status from a log file is supported at the moment
-            ValueError: if no times from the runcontrol file are read in
-
-        Returns:
-            Optional[float]: how long through a simulation run as a proportion of the number of days \
-                simulated as stated in the runcontrol
-        """
-        log_file_path = self.__get_log_path()
-        if log_file_path is None:
-            raise NotImplementedError("Only retrieving status from a log file is supported at the moment")
-        log_file = nfo.load_file_as_list(log_file_path)
-
-        read_in_times = False
-        time_heading_location = None
-        last_time = None
-        for line in log_file:
-            case_name_string = f"Case Name = {self.__model.root_name}"
-            if case_name_string in line:
-                read_in_times = True
-                continue
-            if read_in_times and nfo.check_token('TIME', line):
-                heading_location = 0
-                line_string = line
-                while len(line_string) > 0:
-                    next_value = nfo.get_next_value(0, [line_string], line_string)
-                    if next_value is None:
-                        break
-
-                    line_string = line_string.replace(next_value, '', 1)
-                    if next_value == 'TIME':
-                        time_heading_location = heading_location
-                    heading_location += 1
-
-            if read_in_times and time_heading_location is not None:
-                line_string = line
-                next_value = nfo.get_next_value(0, [line_string], line_string)
-                if next_value is not None and next_value.replace('.', '', 1).isdigit():
-                    if time_heading_location == 0 and (last_time is None or float(next_value) > float(last_time)):
-                        last_time = next_value
-                    for x in range(0, time_heading_location):
-                        line_string = line_string.replace(next_value, '', 1)
-                        next_value = nfo.get_next_value(0, [line_string], line_string)
-                        if next_value is None:
-                            break
-                        # When we reach the time column, read in the time value.
-                        if x == (time_heading_location - 1) and \
-                                (last_time is None or float(next_value) > float(last_time)):
-                            last_time = next_value
-
-        if last_time is not None:
-            days_completed = self.__model._sim_controls.convert_date_to_number(last_time)
-            if self.__model._sim_controls.times is None:
-                raise ValueError("No times provided in the instance - please read them in from runcontrol file")
-            total_days = self.__model._sim_controls.convert_date_to_number(self.__model._sim_controls.times[-1])
-            return round((days_completed / total_days) * 100, 1)
-
-        return 0
+from __future__ import annotations
+
+import os
+from datetime import datetime
+from typing import Optional, TYPE_CHECKING
+import ResSimpy.Nexus.nexus_file_operations as nfo
+
+if TYPE_CHECKING:
+    from ResSimpy.Nexus.NexusSimulator import NexusSimulator
+
+
+class Logging:
+    def __init__(self, model: NexusSimulator) -> None:
+        """Class for controlling all logging and logfile (*.log) related functionality.
+
+        Args:
+            model: NexusSimulator instance
+            __job_id (int): Run job ID for executed runs
+            __simulation_start_time (Optional[str]): Execution start time of the simulation when submitted \
+                to calculation engine
+            __simulation_end_time (Optional[str]): Execution end time of the last time the simulation was run
+            __previous_run_time (Optional[str]): Difference between simulation execution start time and end time.
+        """
+        self.__model = model
+        self.__job_id: int = -1
+        self.__simulation_start_time: Optional[str] = None
+        self.__simulation_end_time: Optional[str] = None
+        self.__previous_run_time: Optional[str] = None
+
+    @staticmethod
+    def get_simulation_time(line: str) -> str:
+        """Searches for the simulation time in a line.
+
+        Args:
+            line (str): line to search for the simulation time
+
+        Raises:
+            ValueError: Throws error if get_next_value doesn't find any subsequent value in the line
+
+        Returns:
+            str: value found after TIME card in a line
+        """
+        value_found = False
+        value = ''
+        line_string = line
+        while value_found is False:
+            next_value = nfo.get_next_value(0, [line_string], line_string)
+            if next_value is None:
+                raise ValueError(
+                    f'No next value found in the line supplied, line: {line_string}')
+            if next_value == 'on':
+                line_string = line_string.replace(next_value, '', 1)
+                next_value = nfo.get_next_value(0, [line_string], line_string)
+                if next_value is None:
+                    raise ValueError(
+                        f'No next value found in the line supplied, line: {line_string}')
+                for c in range(6):
+                    line_string = line_string.replace(next_value, '', 1)
+                    next_value = nfo.get_next_value(0, [line_string], line_string)
+                    if next_value is None:
+                        raise ValueError(
+                            f'No next value found in the line supplied, line: {line_string}')
+                    value += next_value + (' ' if c < 5 else '')
+                value_found = True
+            line_string = line_string.replace(next_value, '', 1)
+        return value
+
+    @staticmethod
+    def convert_server_date(original_date: str) -> datetime:
+        """Convert a datetime string from the server for when the simulation was started to a strptime object.
+
+        Args:
+            original_date (str): string of a date with format: "Mon Jan 01 00:00:00 CST 2020"
+
+        Returns:
+            datetime: datetime object derived from the input string
+        """
+
+        date_format = '%a %b %d %X %Z %Y'
+        converted_date = original_date
+
+        # Convert CDT and CST timezones as Python doesn't work with CDT for some reason
+        if 'CDT' in original_date:
+            converted_date = converted_date.replace('CDT', '-0500', 1)
+            date_format = '%a %b %d %X %z %Y'
+        elif 'CST' in original_date:
+            converted_date = converted_date.replace('CST', '-0600', 1)
+            date_format = '%a %b %d %X %z %Y'
+
+        return datetime.strptime(converted_date, date_format)
+
+    @staticmethod
+    def get_errors_warnings_string(log_file_line_list: list[str]) -> Optional[str]:
+        """Retrieves the number of warnings and errors from the simulation log output,
+        and formats them as a string.
+
+        Args:
+            log_file_line_list (list[str]): log file formatted as a list of strings with \
+                a new list entry per line
+
+        Returns:
+            Optional[str]: string containing the errors and warnings from the simulation log. \
+                None if error/warning set is too short
+        """
+        error_warning = ""
+        for line in log_file_line_list:
+            modified_line = line.lower()
+            if "errors" in modified_line and "warnings" in modified_line:
+                error_warning = modified_line
+
+        error_warning_list = [x for x in error_warning.split(" ") if x != ""]
+
+        error_warning_list = [nfo.clean_up_string(x) for x in error_warning_list]
+
+        if len(error_warning_list) < 4:
+            return None
+
+        errors = error_warning_list[1]
+        warnings = error_warning_list[3]
+
+        error_warning_str = f"Simulation complete - Errors: {errors} and Warnings: {warnings}"
+        return error_warning_str
+
+    def get_simulation_start_time(self) -> str:
+        """Get the start time of an executed simulation run, if no simulation start time returns '-'."""
+        self.get_simulation_status()
+        if self.__simulation_start_time is not None:
+            return self.__simulation_start_time
+        else:
+            return '-'
+
+    def get_simulation_end_time(self) -> str:
+        """Get the end time of an executed simulation run if it has completed, if no simulation end time returns '-'."""
+        self.get_simulation_status()
+        if self.__simulation_end_time is not None:
+            return self.__simulation_end_time
+        else:
+            return '-'
+
+    def get_job_id(self) -> int:
+        """Get the job Id of a simulation run."""
+        return self.__job_id
+
+    def __get_log_path(self, from_startup: bool = False) -> Optional[str]:
+        """Returns the path of the log file for the simulation.
+
+        Args:
+            from_startup (bool, optional): Searches the same directory as the original_fcs_file_path if True. \
+            Otherwise searches the destination folder path, failing this then searches the \
+            original_fcs_file_path if False. Defaults to False.
+
+        Returns:
+            Optional[str]: The path of the .log file from the simulation if found. If not found returns None.
+        """
+        folder_path = os.path.dirname(
+            self.__model.original_fcs_file_path) if from_startup else os.path.dirname(self.__model.origin)
+        files = os.listdir(folder_path)
+        original_fcs_file_location = os.path.basename(self.__model.original_fcs_file_path)
+        log_file_name = os.path.splitext(original_fcs_file_location)[
+                            0] + ".log" if from_startup else self.__model.root_name + ".log"
+
+        if log_file_name in files:
+            if from_startup:
+                file_location = folder_path
+            else:
+                file_location = self.__model.destination if self.__model.destination is not None else folder_path
+
+            log_file_path = file_location + "/" + log_file_name
+            return log_file_path
+        else:
+            return None
+
+    def __update_simulation_start_and_end_times(self, log_file_line_list: list[str]) -> None:
+        """Updates the stored simulation execution start and end times from the log files.
+
+        Args:
+            log_file_line_list (list[str]): log file information represented with a new entry per line of the file.
+        """
+        for line in log_file_line_list:
+            if nfo.check_token('start generic pdsh   prolog', line):
+                value = self.get_simulation_time(line)
+                self.__simulation_start_time = value
+
+            if nfo.check_token('end generic pdsh   epilog', line):
+                value = self.get_simulation_time(line)
+                self.__simulation_end_time = value
+
+    def get_simulation_status(self, from_startup: bool = False) -> Optional[str]:
+        """Gets the run status of the latest simulation run.
+
+        Args:
+            from_startup (bool, optional): Searches the same directory as the original_fcs_file_path if True. \
+            Otherwise searches the destination folder path, failing this then searches the \
+            original_fcs_file_path if False. Defaults to False.
+
+        Raises:
+            NotImplementedError: If log file is not found - only supporting simulation status from log files
+
+        Returns:
+            Optional[str]: the error/warning string if the simulation has finished, otherwise \
+                returns the running job ID. Empty string if a logfile is not found and from_start up is True
+        """
+        log_file = self.__get_log_path(from_startup)
+        if log_file is None:
+            if from_startup:
+                return ''
+            raise NotImplementedError(
+                "Only retrieving status from a log file is supported at the moment")
+        else:
+            log_file_line_list = nfo.load_file_as_list(log_file)
+            self.__update_simulation_start_and_end_times(log_file_line_list)
+            job_finished = 'Nexus finished\n' in log_file_line_list
+            if job_finished:
+                self.__previous_run_time = self.__get_start_end_difference() if from_startup \
+                    else self.__previous_run_time
+                return self.get_errors_warnings_string(log_file_line_list=log_file_line_list)
+            else:
+                job_number_line = [
+                    x for x in log_file_line_list if 'Job number:' in x]
+                if len(job_number_line) > 0:
+                    self.__job_id = int(job_number_line[0].split(":")[1])
+                    return f"Job Running, ID: {self.__job_id}"
+        return None
+
+    def __get_start_end_difference(self) -> Optional[str]:
+        """Returns a string with the previous time taken when the base case was run.
+
+        Returns:
+            Optional[str]: returns a human readable string of how long the simulation took to run
+        """
+        if self.__simulation_start_time is None or self.__simulation_end_time is None:
+            return None
+
+        start_date = self.convert_server_date(self.__simulation_start_time)
+        end_date = self.convert_server_date(self.__simulation_end_time)
+
+        total_difference = (end_date - start_date)
+        days = int(total_difference.days)
+        hours = int(total_difference.seconds / (60 * 60))
+        minutes = int((total_difference.seconds / 60) - (hours * 60))
+        seconds = int(total_difference.seconds -
+                      (hours * 60 * 60) - (minutes * 60))
+
+        return f"{days} Days, {hours} Hours, {minutes} Minutes {seconds} Seconds"
+
+    def get_base_case_run_time(self) -> str:
+        """Get the time taken for the base case to run. Returns '-' if no run time found."""
+        if self.__previous_run_time is not None:
+            return self.__previous_run_time
+        else:
+            return '-'
+
+    def get_simulation_progress(self) -> float:
+        """Returns the simulation progress from log files.
+
+        Raises:
+            NotImplementedError: Only retrieving status from a log file is supported at the moment
+            ValueError: if no times from the runcontrol file are read in
+
+        Returns:
+            Optional[float]: how long through a simulation run as a proportion of the number of days \
+                simulated as stated in the runcontrol
+        """
+        log_file_path = self.__get_log_path()
+        if log_file_path is None:
+            raise NotImplementedError("Only retrieving status from a log file is supported at the moment")
+        log_file = nfo.load_file_as_list(log_file_path)
+
+        read_in_times = False
+        time_heading_location = None
+        last_time = None
+        for line in log_file:
+            case_name_string = f"Case Name = {self.__model.root_name}"
+            if case_name_string in line:
+                read_in_times = True
+                continue
+            if read_in_times and nfo.check_token('TIME', line):
+                heading_location = 0
+                line_string = line
+                while len(line_string) > 0:
+                    next_value = nfo.get_next_value(0, [line_string], line_string)
+                    if next_value is None:
+                        break
+
+                    line_string = line_string.replace(next_value, '', 1)
+                    if next_value == 'TIME':
+                        time_heading_location = heading_location
+                    heading_location += 1
+
+            if read_in_times and time_heading_location is not None:
+                line_string = line
+                next_value = nfo.get_next_value(0, [line_string], line_string)
+                if next_value is not None and next_value.replace('.', '', 1).isdigit():
+                    if time_heading_location == 0 and (last_time is None or float(next_value) > float(last_time)):
+                        last_time = next_value
+                    for x in range(0, time_heading_location):
+                        line_string = line_string.replace(next_value, '', 1)
+                        next_value = nfo.get_next_value(0, [line_string], line_string)
+                        if next_value is None:
+                            break
+                        # When we reach the time column, read in the time value.
+                        if x == (time_heading_location - 1) and \
+                                (last_time is None or float(next_value) > float(last_time)):
+                            last_time = next_value
+
+        if last_time is not None:
+            days_completed = self.__model._sim_controls.convert_date_to_number(last_time)
+            if self.__model._sim_controls.times is None:
+                raise ValueError("No times provided in the instance - please read them in from runcontrol file")
+            total_days = self.__model._sim_controls.convert_date_to_number(self.__model._sim_controls.times[-1])
+            return round((days_completed / total_days) * 100, 1)
+
+        return 0
```

### Comparing `ressimpy-1.0.0/ResSimpy/Nexus/nexus_collect_tables.py` & `ressimpy-1.0.1/ResSimpy/Nexus/nexus_collect_tables.py`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,146 +1,146 @@
-from __future__ import annotations
-
-from typing import Any, Optional
-
-from ResSimpy.File import File
-from ResSimpy.Nexus.DataModels.Network.NexusConstraint import NexusConstraint
-from ResSimpy.Enums.UnitsEnum import UnitSystem
-from ResSimpy.Nexus.nexus_constraint_operations import load_inline_constraints
-from ResSimpy.Nexus.nexus_file_operations import check_property_in_line, check_token, get_expected_token_value, \
-    check_list_tokens, load_table_to_objects
-
-
-def collect_all_tables_to_objects(nexus_file: File, table_object_map: dict[str, Any], start_date: Optional[str],
-                                  default_units: Optional[UnitSystem]) -> \
-        dict[str, list[Any] | dict[str, list[NexusConstraint]]]:
-    """Loads all tables from a given file.
-
-    Args:
-    ----
-    nexus_file (File): NexusFile representation of the file.
-    table_object_map (dict[str, Storage_Object]): dictionary containing the name of the table as keys and \
-                the object type to store the data from each row into. Require objects to have a get_nexus_mapping \
-                function
-    model: (NexusSimulator): main simulator object
-
-    Raises:
-    ------
-    TypeError: if the unit system found in the property check is not a valid enum UnitSystem.
-
-    Returns:
-    -------
-    dict[str, list[Storage_Object]]: a dictionary of lists of arbitrary objects populated \
-                with properties from the file provided, keyed with the NexusTable name associated with table_object_map.
-    """
-    current_date = start_date
-    nexus_object_results: dict[str, list[Any] | dict[str, list[NexusConstraint]]] = {x: [] for x in table_object_map}
-    nexus_constraints: dict[str, list[NexusConstraint]] = {}
-    nexus_object_results['CONSTRAINTS'] = nexus_constraints
-    file_as_list: list[str] = nexus_file.get_flat_list_str_file
-    table_start: int = -1
-    table_end: int = -1
-    property_dict: dict = {}
-    token_found: Optional[str] = None
-    network_names: list[str] = []
-    for index, line in enumerate(file_as_list):
-        # check for changes in unit system
-        check_property_in_line(line, property_dict, file_as_list)
-        unit_system = property_dict.get('UNIT_SYSTEM', default_units)
-        if not isinstance(unit_system, UnitSystem):
-            raise TypeError(f"Value found for {unit_system=} of type {type(unit_system)} \
-                                not compatible, expected type UnitSystem Enum")
-        if check_token('TIME', line):
-            current_date = get_expected_token_value(
-                token='TIME', token_line=line, file_list=file_as_list,
-                custom_message=f"Cannot find the date associated with the TIME card in {line=} at line number {index}")
-            continue
-        if table_start < 0:
-            token_found = check_list_tokens(list(table_object_map.keys()), line)
-            if token_found is None or check_token('WELLCONTROL', line):
-                continue
-            # if a token is found get the starting index of the table
-            table_start = index + 1
-        if token_found is None:
-            continue
-        token_found = token_found.upper()
-
-        if table_start > 0 and check_token('END' + token_found, line):
-            table_end = index
-        # if we have a complete table to read in start reading it into objects
-        if 0 < table_start <= table_end:
-            # cover for the case where we aren't currently reading in the table to an object.
-            # if no object is provided by the map for the token found then skip the keyword and reset the tracking vars
-            if table_object_map[token_found] is None:
-                table_start = -1
-                table_end = -1
-                token_found = None
-                continue
-            list_objects = None
-            property_map = table_object_map[token_found].get_nexus_mapping()
-            if token_found == 'CONSTRAINTS':
-                load_inline_constraints(file_as_list=file_as_list[table_start:table_end],
-                                        constraint=table_object_map[token_found],
-                                        current_date=current_date,
-                                        unit_system=unit_system,
-                                        property_map=property_map,
-                                        existing_constraints=nexus_constraints,
-                                        nexus_file=nexus_file,
-                                        start_line_index=table_start,
-                                        network_names=network_names,
-                                        )
-
-            elif token_found == 'QMULT' or token_found == 'CONSTRAINT':
-                list_objects = load_table_to_objects(file_as_list=file_as_list[table_start:table_end],
-                                                     row_object=table_object_map[token_found],
-                                                     property_map=property_map,
-                                                     current_date=current_date,
-                                                     unit_system=unit_system,
-                                                     nexus_obj_dict=nexus_constraints,
-                                                     preserve_previous_object_attributes=True)
-
-            else:
-                list_objects = load_table_to_objects(file_as_list=file_as_list[table_start:table_end],
-                                                     row_object=table_object_map[token_found],
-                                                     property_map=property_map,
-                                                     current_date=current_date,
-                                                     unit_system=unit_system)
-
-            # store objects found into right dictionary
-            list_of_token_obj = nexus_object_results[token_found]
-            # This statement ensures that CONSTRAINT that are found in tables are actually added to the dictionary
-            # under the same key as constraints to preserve their order
-            if (token_found == 'CONSTRAINT' or token_found == 'QMULT') and list_objects is not None:
-                for constraint, id_index in list_objects:
-                    if isinstance(constraint, NexusConstraint):
-                        obj_id = constraint.id
-                        well_name = constraint.name
-                    else:
-                        obj_id = constraint
-                        well_name = None
-                    correct_line_index = id_index + table_start
-                    nexus_file.add_object_locations(obj_id, [correct_line_index])
-                    if well_name is None:
-                        continue
-                    if nexus_constraints.get(well_name, None) is not None:
-                        nexus_constraints[well_name].append(constraint)
-                    else:
-                        nexus_constraints[well_name] = [constraint]
-            elif list_objects is not None and isinstance(list_of_token_obj, list):
-                list_of_token_obj.extend([x[0] for x in list_objects])
-                # add the names from the nodes into the network names for wildcards
-                network_names.extend([x.name for x in list_of_token_obj])
-                for new_object, id_index in list_objects:
-                    correct_line_index = id_index + table_start
-                    # temporary try statement until all objects have an id property
-                    try:
-                        obj_id = new_object.id
-                        nexus_file.add_object_locations(obj_id, [correct_line_index])
-                    except AttributeError:
-                        pass
-            else:
-                list_of_token_obj = nexus_constraints
-            # reset indices for further tables
-            table_start = -1
-            table_end = -1
-            token_found = None
-    return nexus_object_results
+from __future__ import annotations
+
+from typing import Any, Optional
+
+from ResSimpy.File import File
+from ResSimpy.Nexus.DataModels.Network.NexusConstraint import NexusConstraint
+from ResSimpy.Enums.UnitsEnum import UnitSystem
+from ResSimpy.Nexus.nexus_constraint_operations import load_inline_constraints
+from ResSimpy.Nexus.nexus_file_operations import check_property_in_line, check_token, get_expected_token_value, \
+    check_list_tokens, load_table_to_objects
+
+
+def collect_all_tables_to_objects(nexus_file: File, table_object_map: dict[str, Any], start_date: Optional[str],
+                                  default_units: Optional[UnitSystem]) -> \
+        dict[str, list[Any] | dict[str, list[NexusConstraint]]]:
+    """Loads all tables from a given file.
+
+    Args:
+    ----
+    nexus_file (File): NexusFile representation of the file.
+    table_object_map (dict[str, Storage_Object]): dictionary containing the name of the table as keys and \
+                the object type to store the data from each row into. Require objects to have a get_nexus_mapping \
+                function
+    model: (NexusSimulator): main simulator object
+
+    Raises:
+    ------
+    TypeError: if the unit system found in the property check is not a valid enum UnitSystem.
+
+    Returns:
+    -------
+    dict[str, list[Storage_Object]]: a dictionary of lists of arbitrary objects populated \
+                with properties from the file provided, keyed with the NexusTable name associated with table_object_map.
+    """
+    current_date = start_date
+    nexus_object_results: dict[str, list[Any] | dict[str, list[NexusConstraint]]] = {x: [] for x in table_object_map}
+    nexus_constraints: dict[str, list[NexusConstraint]] = {}
+    nexus_object_results['CONSTRAINTS'] = nexus_constraints
+    file_as_list: list[str] = nexus_file.get_flat_list_str_file
+    table_start: int = -1
+    table_end: int = -1
+    property_dict: dict = {}
+    token_found: Optional[str] = None
+    network_names: list[str] = []
+    for index, line in enumerate(file_as_list):
+        # check for changes in unit system
+        check_property_in_line(line, property_dict, file_as_list)
+        unit_system = property_dict.get('UNIT_SYSTEM', default_units)
+        if not isinstance(unit_system, UnitSystem):
+            raise TypeError(f"Value found for {unit_system=} of type {type(unit_system)} \
+                                not compatible, expected type UnitSystem Enum")
+        if check_token('TIME', line):
+            current_date = get_expected_token_value(
+                token='TIME', token_line=line, file_list=file_as_list,
+                custom_message=f"Cannot find the date associated with the TIME card in {line=} at line number {index}")
+            continue
+        if table_start < 0:
+            token_found = check_list_tokens(list(table_object_map.keys()), line)
+            if token_found is None or check_token('WELLCONTROL', line):
+                continue
+            # if a token is found get the starting index of the table
+            table_start = index + 1
+        if token_found is None:
+            continue
+        token_found = token_found.upper()
+
+        if table_start > 0 and check_token('END' + token_found, line):
+            table_end = index
+        # if we have a complete table to read in start reading it into objects
+        if 0 < table_start <= table_end:
+            # cover for the case where we aren't currently reading in the table to an object.
+            # if no object is provided by the map for the token found then skip the keyword and reset the tracking vars
+            if table_object_map[token_found] is None:
+                table_start = -1
+                table_end = -1
+                token_found = None
+                continue
+            list_objects = None
+            property_map = table_object_map[token_found].get_nexus_mapping()
+            if token_found == 'CONSTRAINTS':
+                load_inline_constraints(file_as_list=file_as_list[table_start:table_end],
+                                        constraint=table_object_map[token_found],
+                                        current_date=current_date,
+                                        unit_system=unit_system,
+                                        property_map=property_map,
+                                        existing_constraints=nexus_constraints,
+                                        nexus_file=nexus_file,
+                                        start_line_index=table_start,
+                                        network_names=network_names,
+                                        )
+
+            elif token_found == 'QMULT' or token_found == 'CONSTRAINT':
+                list_objects = load_table_to_objects(file_as_list=file_as_list[table_start:table_end],
+                                                     row_object=table_object_map[token_found],
+                                                     property_map=property_map,
+                                                     current_date=current_date,
+                                                     unit_system=unit_system,
+                                                     nexus_obj_dict=nexus_constraints,
+                                                     preserve_previous_object_attributes=True)
+
+            else:
+                list_objects = load_table_to_objects(file_as_list=file_as_list[table_start:table_end],
+                                                     row_object=table_object_map[token_found],
+                                                     property_map=property_map,
+                                                     current_date=current_date,
+                                                     unit_system=unit_system)
+
+            # store objects found into right dictionary
+            list_of_token_obj = nexus_object_results[token_found]
+            # This statement ensures that CONSTRAINT that are found in tables are actually added to the dictionary
+            # under the same key as constraints to preserve their order
+            if (token_found == 'CONSTRAINT' or token_found == 'QMULT') and list_objects is not None:
+                for constraint, id_index in list_objects:
+                    if isinstance(constraint, NexusConstraint):
+                        obj_id = constraint.id
+                        well_name = constraint.name
+                    else:
+                        obj_id = constraint
+                        well_name = None
+                    correct_line_index = id_index + table_start
+                    nexus_file.add_object_locations(obj_id, [correct_line_index])
+                    if well_name is None:
+                        continue
+                    if nexus_constraints.get(well_name, None) is not None:
+                        nexus_constraints[well_name].append(constraint)
+                    else:
+                        nexus_constraints[well_name] = [constraint]
+            elif list_objects is not None and isinstance(list_of_token_obj, list):
+                list_of_token_obj.extend([x[0] for x in list_objects])
+                # add the names from the nodes into the network names for wildcards
+                network_names.extend([x.name for x in list_of_token_obj])
+                for new_object, id_index in list_objects:
+                    correct_line_index = id_index + table_start
+                    # temporary try statement until all objects have an id property
+                    try:
+                        obj_id = new_object.id
+                        nexus_file.add_object_locations(obj_id, [correct_line_index])
+                    except AttributeError:
+                        pass
+            else:
+                list_of_token_obj = nexus_constraints
+            # reset indices for further tables
+            table_start = -1
+            table_end = -1
+            token_found = None
+    return nexus_object_results
```

### Comparing `ressimpy-1.0.0/ResSimpy/Nexus/nexus_constraint_operations.py` & `ressimpy-1.0.1/ResSimpy/Nexus/nexus_constraint_operations.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,132 +1,132 @@
-from __future__ import annotations
-
-from typing import Optional, TYPE_CHECKING
-
-from ResSimpy.Nexus.DataModels.Network.NexusConstraint import NexusConstraint
-from ResSimpy.Enums.UnitsEnum import UnitSystem
-from ResSimpy.Nexus.nexus_file_operations import get_next_value, correct_datatypes
-from ResSimpy.Utils.invert_nexus_map import nexus_keyword_to_attribute_name
-import fnmatch
-if TYPE_CHECKING:
-    from ResSimpy.File import File
-
-
-def load_inline_constraints(file_as_list: list[str], constraint: type[NexusConstraint], current_date: Optional[str],
-                            unit_system: UnitSystem, property_map: dict[str, tuple[str, type]],
-                            existing_constraints: dict[str, list[NexusConstraint]], nexus_file: File,
-                            start_line_index: int, network_names: Optional[list[str]] = None) -> None:
-    """Loads table of constraints with the wellname/node first and the constraints following inline
-        uses previous set of constraints as still applied to the well.
-
-    Args:
-    ----
-        file_as_list (list[str]): file represented as a list of strings
-        constraint (NexusConstraint): object to store the attributes extracted from each row.
-        current_date (str): the current date in the table
-        unit_system (UnitSystem): Unit system enum
-        property_map (dict[str, tuple[str, type]]): Mapping of nexus keywords to attributes
-        existing_constraints (dict[str, NexusConstraint]): all existing constraints from previous lines of the \
-            surface file
-        network_names (Optional[list[str]]): list of names for all nodes, wells and connections in a nexus network.
-            Used in deriving constraints from wildcards. Defaults to None
-
-    Returns:
-    -------
-        dict[UUID, int]: dictionary of object locations derived from inline table.
-    """
-
-    for index, line in enumerate(file_as_list):
-        properties_dict: dict[str, str | float | UnitSystem | None] = {'date': current_date, 'unit_system': unit_system}
-        # first value in the line has to be the node/wellname
-        name = get_next_value(0, [line])
-        nones_overwrite = False
-        constraint_names_to_add: list[str] = []
-        if name is None:
-            continue
-        properties_dict['name'] = name
-        if '*' in name:
-            if network_names is None:
-                raise ValueError('No existing nodes found to add wildcards to')
-            else:
-                # filter names that match the pattern
-                constraint_names_to_add = fnmatch.filter(network_names, name)
-        else:
-            constraint_names_to_add.append(name)
-
-        trimmed_line = line.replace(name, "", 1)
-        next_value = get_next_value(0, [trimmed_line])
-        # loop through the line for each set of constraints
-        while next_value is not None:
-            token_value = next_value.upper()
-            if token_value in ['CLEAR', 'CLEARP', 'CLEARQ', 'CLEARLIMIT', 'CLEARALQ']:
-                properties_dict[nexus_keyword_to_attribute_name(constraint.get_nexus_mapping(), token_value)] = True
-                nones_overwrite = True
-                # break out of the while loop as the next value will not be there
-                break
-            elif token_value == 'ACTIVATE' or token_value == 'DEACTIVATE':
-                properties_dict.update({'active_node': token_value == 'ACTIVATE'})
-                trimmed_line = trimmed_line.replace(next_value, "", 1)
-                next_value = get_next_value(0, [trimmed_line])
-                if next_value is None:
-                    break
-                token_value = next_value.upper()
-
-            trimmed_line = trimmed_line.replace(next_value, "", 1)
-            # extract the attribute name for the given nexus constraint token
-            attribute = property_map[token_value][0]
-            next_value = get_next_value(0, [trimmed_line])
-            if next_value is None:
-                raise ValueError(f'No value found after {token_value} in {line}')
-            elif next_value == 'MULT':
-                try:
-                    attribute = property_map[token_value + '_MULT'][0]
-                except AttributeError:
-                    raise AttributeError(f'Unexpected MULT keyword following {token_value}')
-                properties_dict[attribute] = True
-
-            else:
-                properties_dict[attribute] = correct_datatypes(next_value, float)
-            trimmed_line = trimmed_line.replace(next_value, "", 1)
-            next_value = get_next_value(0, [trimmed_line])
-
-        # first check if there are any existing constraints created for the well this timestep
-        for name_of_node in constraint_names_to_add:
-            properties_dict['name'] = name_of_node
-            well_constraints = existing_constraints.get(name_of_node, None)
-            if well_constraints is not None:
-                latest_constraint = well_constraints[-1]
-                if latest_constraint.date == current_date:
-                    latest_constraint.update(properties_dict, nones_overwrite)
-                    nexus_file.add_object_locations(latest_constraint.id, [index + start_line_index])
-                else:
-                    # otherwise take a copy of the previous constraint and add the additional properties
-                    new_constraint = constraint(properties_dict)
-                    well_constraints.append(new_constraint)
-                    nexus_file.add_object_locations(new_constraint.id, [index + start_line_index])
-            else:
-                nexus_constraint = constraint(properties_dict)
-
-                existing_constraints[name_of_node] = [nexus_constraint]
-                nexus_file.add_object_locations(nexus_constraint.id, [index + start_line_index])
-
-
-def __clear_constraints(token_value, constraint) -> dict[str, None]:
-    """Replicates behaviour of the clear keyword in nexus constraints by creating a dictionary filled with
-    Nones for the relevant parameters.
-    """
-    match token_value:
-        case 'CLEAR':
-            constraint_clearing_dict = constraint.get_rate_constraints_map()
-            constraint_clearing_dict.update(constraint.get_pressure_constraints_map())
-            constraint_clearing_dict.update(constraint.get_limit_constraints_map())
-        case 'CLEARQ':
-            constraint_clearing_dict = constraint.get_rate_constraints_map()
-        case 'CLEARLIMIT':
-            constraint_clearing_dict = constraint.get_limit_constraints_map()
-        case 'CLEARP':
-            constraint_clearing_dict = constraint.get_pressure_constraints_map()
-        case 'CLEARALQ':
-            constraint_clearing_dict = constraint.get_alq_constraints_map()
-        case _:
-            constraint_clearing_dict = {}
-    return {x[0]: None for x in constraint_clearing_dict.values()}
+from __future__ import annotations
+
+from typing import Optional, TYPE_CHECKING
+
+from ResSimpy.Nexus.DataModels.Network.NexusConstraint import NexusConstraint
+from ResSimpy.Enums.UnitsEnum import UnitSystem
+from ResSimpy.Nexus.nexus_file_operations import get_next_value, correct_datatypes
+from ResSimpy.Utils.invert_nexus_map import nexus_keyword_to_attribute_name
+import fnmatch
+if TYPE_CHECKING:
+    from ResSimpy.File import File
+
+
+def load_inline_constraints(file_as_list: list[str], constraint: type[NexusConstraint], current_date: Optional[str],
+                            unit_system: UnitSystem, property_map: dict[str, tuple[str, type]],
+                            existing_constraints: dict[str, list[NexusConstraint]], nexus_file: File,
+                            start_line_index: int, network_names: Optional[list[str]] = None) -> None:
+    """Loads table of constraints with the wellname/node first and the constraints following inline
+        uses previous set of constraints as still applied to the well.
+
+    Args:
+    ----
+        file_as_list (list[str]): file represented as a list of strings
+        constraint (NexusConstraint): object to store the attributes extracted from each row.
+        current_date (str): the current date in the table
+        unit_system (UnitSystem): Unit system enum
+        property_map (dict[str, tuple[str, type]]): Mapping of nexus keywords to attributes
+        existing_constraints (dict[str, NexusConstraint]): all existing constraints from previous lines of the \
+            surface file
+        network_names (Optional[list[str]]): list of names for all nodes, wells and connections in a nexus network.
+            Used in deriving constraints from wildcards. Defaults to None
+
+    Returns:
+    -------
+        dict[UUID, int]: dictionary of object locations derived from inline table.
+    """
+
+    for index, line in enumerate(file_as_list):
+        properties_dict: dict[str, str | float | UnitSystem | None] = {'date': current_date, 'unit_system': unit_system}
+        # first value in the line has to be the node/wellname
+        name = get_next_value(0, [line])
+        nones_overwrite = False
+        constraint_names_to_add: list[str] = []
+        if name is None:
+            continue
+        properties_dict['name'] = name
+        if '*' in name:
+            if network_names is None:
+                raise ValueError('No existing nodes found to add wildcards to')
+            else:
+                # filter names that match the pattern
+                constraint_names_to_add = fnmatch.filter(network_names, name)
+        else:
+            constraint_names_to_add.append(name)
+
+        trimmed_line = line.replace(name, "", 1)
+        next_value = get_next_value(0, [trimmed_line])
+        # loop through the line for each set of constraints
+        while next_value is not None:
+            token_value = next_value.upper()
+            if token_value in ['CLEAR', 'CLEARP', 'CLEARQ', 'CLEARLIMIT', 'CLEARALQ']:
+                properties_dict[nexus_keyword_to_attribute_name(constraint.get_nexus_mapping(), token_value)] = True
+                nones_overwrite = True
+                # break out of the while loop as the next value will not be there
+                break
+            elif token_value == 'ACTIVATE' or token_value == 'DEACTIVATE':
+                properties_dict.update({'active_node': token_value == 'ACTIVATE'})
+                trimmed_line = trimmed_line.replace(next_value, "", 1)
+                next_value = get_next_value(0, [trimmed_line])
+                if next_value is None:
+                    break
+                token_value = next_value.upper()
+
+            trimmed_line = trimmed_line.replace(next_value, "", 1)
+            # extract the attribute name for the given nexus constraint token
+            attribute = property_map[token_value][0]
+            next_value = get_next_value(0, [trimmed_line])
+            if next_value is None:
+                raise ValueError(f'No value found after {token_value} in {line}')
+            elif next_value == 'MULT':
+                try:
+                    attribute = property_map[token_value + '_MULT'][0]
+                except AttributeError:
+                    raise AttributeError(f'Unexpected MULT keyword following {token_value}')
+                properties_dict[attribute] = True
+
+            else:
+                properties_dict[attribute] = correct_datatypes(next_value, float)
+            trimmed_line = trimmed_line.replace(next_value, "", 1)
+            next_value = get_next_value(0, [trimmed_line])
+
+        # first check if there are any existing constraints created for the well this timestep
+        for name_of_node in constraint_names_to_add:
+            properties_dict['name'] = name_of_node
+            well_constraints = existing_constraints.get(name_of_node, None)
+            if well_constraints is not None:
+                latest_constraint = well_constraints[-1]
+                if latest_constraint.date == current_date:
+                    latest_constraint.update(properties_dict, nones_overwrite)
+                    nexus_file.add_object_locations(latest_constraint.id, [index + start_line_index])
+                else:
+                    # otherwise take a copy of the previous constraint and add the additional properties
+                    new_constraint = constraint(properties_dict)
+                    well_constraints.append(new_constraint)
+                    nexus_file.add_object_locations(new_constraint.id, [index + start_line_index])
+            else:
+                nexus_constraint = constraint(properties_dict)
+
+                existing_constraints[name_of_node] = [nexus_constraint]
+                nexus_file.add_object_locations(nexus_constraint.id, [index + start_line_index])
+
+
+def __clear_constraints(token_value, constraint) -> dict[str, None]:
+    """Replicates behaviour of the clear keyword in nexus constraints by creating a dictionary filled with
+    Nones for the relevant parameters.
+    """
+    match token_value:
+        case 'CLEAR':
+            constraint_clearing_dict = constraint.get_rate_constraints_map()
+            constraint_clearing_dict.update(constraint.get_pressure_constraints_map())
+            constraint_clearing_dict.update(constraint.get_limit_constraints_map())
+        case 'CLEARQ':
+            constraint_clearing_dict = constraint.get_rate_constraints_map()
+        case 'CLEARLIMIT':
+            constraint_clearing_dict = constraint.get_limit_constraints_map()
+        case 'CLEARP':
+            constraint_clearing_dict = constraint.get_pressure_constraints_map()
+        case 'CLEARALQ':
+            constraint_clearing_dict = constraint.get_alq_constraints_map()
+        case _:
+            constraint_clearing_dict = {}
+    return {x[0]: None for x in constraint_clearing_dict.values()}
```

### Comparing `ressimpy-1.0.0/ResSimpy/Nexus/nexus_modify_object_in_file.py` & `ressimpy-1.0.1/ResSimpy/Nexus/nexus_modify_object_in_file.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-from __future__ import annotations
-
-from typing import Any, TYPE_CHECKING
-
-if TYPE_CHECKING:
-    from ResSimpy.Nexus.NexusNetwork import NexusNetwork
-
-
-class ModifyObjectOperations:
-    def __init__(self, object_to_modify: Any) -> None:
-        self.object_to_modify = object_to_modify
-
-    def modify_network_object(self, object_to_modify: dict[str, None | str | float | int],
-                              new_properties: dict[str, None | str | float | int], network: NexusNetwork) -> None:
-        """Modifies an existing object based on a matching dictionary of properties (partial matches allowed if
-        precisely 1 matching object is found).
-        Updates the properties with properties in the new_properties dictionary.
-        Applies primarily to network based objects.
-
-        Args:
-            object_to_modify (dict[str, None | str | float | int]): dictionary containing attributes to match in the
-            existing object set. Requires an implemented add, remove
-            new_properties (dict[str, None | str | float | int]): properties to switch to in the new object
-        """
-        # TODO apply this to more of the network attributes through the Base Class
-        network_attribute_name = self.object_to_modify._network_element_name
-        name = object_to_modify.get('name', None)
-        if name is None:
-            raise ValueError(f'Name is required for modifying {network_attribute_name}, '
-                             f'instead got {name}')
-        name = str(name)
-        network_element = network.find_network_element_with_dict(name, object_to_modify,
-                                                                 network_attribute_name)
-        existing_properties = network_element.to_dict(include_nones=False)
-        # do the union of the two dicts
-        existing_properties.update(new_properties)
-
-        self.object_to_modify.remove(object_to_modify)
-        self.object_to_modify.add(existing_properties)
+from __future__ import annotations
+
+from typing import Any, TYPE_CHECKING
+
+if TYPE_CHECKING:
+    from ResSimpy.Nexus.NexusNetwork import NexusNetwork
+
+
+class ModifyObjectOperations:
+    def __init__(self, object_to_modify: Any) -> None:
+        self.object_to_modify = object_to_modify
+
+    def modify_network_object(self, object_to_modify: dict[str, None | str | float | int],
+                              new_properties: dict[str, None | str | float | int], network: NexusNetwork) -> None:
+        """Modifies an existing object based on a matching dictionary of properties (partial matches allowed if
+        precisely 1 matching object is found).
+        Updates the properties with properties in the new_properties dictionary.
+        Applies primarily to network based objects.
+
+        Args:
+            object_to_modify (dict[str, None | str | float | int]): dictionary containing attributes to match in the
+            existing object set. Requires an implemented add, remove
+            new_properties (dict[str, None | str | float | int]): properties to switch to in the new object
+        """
+        # TODO apply this to more of the network attributes through the Base Class
+        network_attribute_name = self.object_to_modify._network_element_name
+        name = object_to_modify.get('name', None)
+        if name is None:
+            raise ValueError(f'Name is required for modifying {network_attribute_name}, '
+                             f'instead got {name}')
+        name = str(name)
+        network_element = network.find_network_element_with_dict(name, object_to_modify,
+                                                                 network_attribute_name)
+        existing_properties = network_element.to_dict(include_nones=False)
+        # do the union of the two dicts
+        existing_properties.update(new_properties)
+
+        self.object_to_modify.remove(object_to_modify)
+        self.object_to_modify.add(existing_properties)
```

### Comparing `ressimpy-1.0.0/ResSimpy/Nexus/nexus_remove_object_from_file.py` & `ressimpy-1.0.1/ResSimpy/Nexus/nexus_remove_object_from_file.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,102 +1,102 @@
-from typing import Any
-from uuid import UUID
-
-from ResSimpy.Nexus.DataModels.NexusFile import NexusFile
-
-
-class RemoveObjectOperations:
-    def __init__(self, table_header: str, table_footer: str) -> None:
-        self.table_header = table_header
-        self.table_footer = table_footer
-
-    @staticmethod
-    def remove_object_from_memory_by_id(list_obj: list[Any], id_to_remove: UUID) -> tuple[Any, list[Any]]:
-        """Directly removes an object from a list of objects based on the id attribute of that object."""
-        if len(list_obj) == 0:
-            raise ValueError('Tried to remove object from empty list. Cannot remove object.')
-
-        if not hasattr(list_obj[0], 'id'):
-            raise AttributeError(f'Objects provided in {list_obj} has no attribute id.')
-
-        index_to_remove = [x.id for x in list_obj].index(id_to_remove)
-        object_removed = list_obj.pop(index_to_remove)
-        return object_removed, list_obj
-
-    def check_for_empty_table(self, file: NexusFile, line_numbers_in_file_to_remove: list[int], obj_id: UUID) \
-            -> list[int]:
-        """Identifies the lines needed to be removed if the table is empty.
-
-        Args:
-            file (NexusFile): file to check
-            line_numbers_in_file_to_remove (list[int]): list of line indices for the object being removed
-            obj_id (UUID): id of the object being removed
-
-        Returns:
-            A list of integers with the lines to remove from the file if the resulting table is empty after the lines\
-             associated with the removed object is removed
-        """
-        first_obj_index = line_numbers_in_file_to_remove[0]
-        last_obj_index = line_numbers_in_file_to_remove[-1]
-        additional_indices_to_remove = []
-        remove_table = True
-        # get all the indices for the tables:
-        file_content = file.get_flat_list_str_file
-        start_node_keyword_index_to_remove = max([i for i, x in enumerate(file_content) if self.table_header in x and
-                                                  i < first_obj_index])
-        end_node_keyword_index_to_remove = min([i for i, x in enumerate(file_content) if self.table_footer in x and
-                                                i > last_obj_index])
-        # check there are any nodes left in the specified table
-        if file.object_locations is None:
-            raise ValueError(f'No object locations specified, cannot find id: {obj_id} in {file.object_locations}')
-
-        for obj_uuid, line_locations_list in file.object_locations.items():
-            if obj_uuid == obj_id:
-                # ignore the uuid's for the node that we want to remove
-                continue
-            for value in line_locations_list:
-                # if we find an object in the middle of the table then don't remove it
-                if start_node_keyword_index_to_remove <= value <= end_node_keyword_index_to_remove:
-                    remove_table = False
-                    break
-        if remove_table:
-            additional_indices_to_remove = list(range(start_node_keyword_index_to_remove,
-                                                      end_node_keyword_index_to_remove + 1))
-        return additional_indices_to_remove
-
-    def remove_lines_from_file(self, line_numbers_in_file_to_remove: list[int], file: NexusFile, obj_id: UUID) -> None:
-        """Removes lines from the file content and removes any references to the object in the line locations in the \
-        file.
-
-        Args:
-            line_numbers_in_file_to_remove (list[int]): line indices to be removed. Relative to the flattened file.
-            file (NexusFile): NexusFile to remove the lines from. Lines nested in files will be resolved correctly.
-            obj_id (UUID): id of the object being removed
-        """
-        # get unique line numbers + sort them in descending order
-        line_numbers_in_file_to_remove = list(set(line_numbers_in_file_to_remove))
-        line_numbers_in_file_to_remove.sort(reverse=True)
-        # remove the lines
-        for index, line_in_file in enumerate(line_numbers_in_file_to_remove):
-            if index == 0:
-                file.remove_from_file_as_list(line_in_file, [obj_id])
-            else:
-                file.remove_from_file_as_list(line_in_file)
-
-    def remove_object_by_id(self, file: NexusFile, obj_id: UUID, obj_list: list[Any]) -> None:
-        """Remove an object from a file and from the list of stored objects.
-
-        Args:
-            file (NexusFile): file to remove the lines associated with the obj from.
-            obj_id (UUID): id of the object being removed.
-            obj_list (list[Any]): list of corresponding objects.
-        """
-        # remove from memory
-        self.remove_object_from_memory_by_id(obj_list, id_to_remove=obj_id)
-        # remove from file
-        line_numbers_in_file_to_remove = file.get_object_locations_for_id(obj_id)
-        # get table_header and footers
-        remove_empty_table_indices = self.check_for_empty_table(
-            file, line_numbers_in_file_to_remove, obj_id)
-        # remove the table if there aren't any more remaining
-        line_numbers_in_file_to_remove.extend(remove_empty_table_indices)
-        self.remove_lines_from_file(line_numbers_in_file_to_remove, file, obj_id)
+from typing import Any
+from uuid import UUID
+
+from ResSimpy.Nexus.DataModels.NexusFile import NexusFile
+
+
+class RemoveObjectOperations:
+    def __init__(self, table_header: str, table_footer: str) -> None:
+        self.table_header = table_header
+        self.table_footer = table_footer
+
+    @staticmethod
+    def remove_object_from_memory_by_id(list_obj: list[Any], id_to_remove: UUID) -> tuple[Any, list[Any]]:
+        """Directly removes an object from a list of objects based on the id attribute of that object."""
+        if len(list_obj) == 0:
+            raise ValueError('Tried to remove object from empty list. Cannot remove object.')
+
+        if not hasattr(list_obj[0], 'id'):
+            raise AttributeError(f'Objects provided in {list_obj} has no attribute id.')
+
+        index_to_remove = [x.id for x in list_obj].index(id_to_remove)
+        object_removed = list_obj.pop(index_to_remove)
+        return object_removed, list_obj
+
+    def check_for_empty_table(self, file: NexusFile, line_numbers_in_file_to_remove: list[int], obj_id: UUID) \
+            -> list[int]:
+        """Identifies the lines needed to be removed if the table is empty.
+
+        Args:
+            file (NexusFile): file to check
+            line_numbers_in_file_to_remove (list[int]): list of line indices for the object being removed
+            obj_id (UUID): id of the object being removed
+
+        Returns:
+            A list of integers with the lines to remove from the file if the resulting table is empty after the lines\
+             associated with the removed object is removed
+        """
+        first_obj_index = line_numbers_in_file_to_remove[0]
+        last_obj_index = line_numbers_in_file_to_remove[-1]
+        additional_indices_to_remove = []
+        remove_table = True
+        # get all the indices for the tables:
+        file_content = file.get_flat_list_str_file
+        start_node_keyword_index_to_remove = max([i for i, x in enumerate(file_content) if self.table_header in x and
+                                                  i < first_obj_index])
+        end_node_keyword_index_to_remove = min([i for i, x in enumerate(file_content) if self.table_footer in x and
+                                                i > last_obj_index])
+        # check there are any nodes left in the specified table
+        if file.object_locations is None:
+            raise ValueError(f'No object locations specified, cannot find id: {obj_id} in {file.object_locations}')
+
+        for obj_uuid, line_locations_list in file.object_locations.items():
+            if obj_uuid == obj_id:
+                # ignore the uuid's for the node that we want to remove
+                continue
+            for value in line_locations_list:
+                # if we find an object in the middle of the table then don't remove it
+                if start_node_keyword_index_to_remove <= value <= end_node_keyword_index_to_remove:
+                    remove_table = False
+                    break
+        if remove_table:
+            additional_indices_to_remove = list(range(start_node_keyword_index_to_remove,
+                                                      end_node_keyword_index_to_remove + 1))
+        return additional_indices_to_remove
+
+    def remove_lines_from_file(self, line_numbers_in_file_to_remove: list[int], file: NexusFile, obj_id: UUID) -> None:
+        """Removes lines from the file content and removes any references to the object in the line locations in the \
+        file.
+
+        Args:
+            line_numbers_in_file_to_remove (list[int]): line indices to be removed. Relative to the flattened file.
+            file (NexusFile): NexusFile to remove the lines from. Lines nested in files will be resolved correctly.
+            obj_id (UUID): id of the object being removed
+        """
+        # get unique line numbers + sort them in descending order
+        line_numbers_in_file_to_remove = list(set(line_numbers_in_file_to_remove))
+        line_numbers_in_file_to_remove.sort(reverse=True)
+        # remove the lines
+        for index, line_in_file in enumerate(line_numbers_in_file_to_remove):
+            if index == 0:
+                file.remove_from_file_as_list(line_in_file, [obj_id])
+            else:
+                file.remove_from_file_as_list(line_in_file)
+
+    def remove_object_by_id(self, file: NexusFile, obj_id: UUID, obj_list: list[Any]) -> None:
+        """Remove an object from a file and from the list of stored objects.
+
+        Args:
+            file (NexusFile): file to remove the lines associated with the obj from.
+            obj_id (UUID): id of the object being removed.
+            obj_list (list[Any]): list of corresponding objects.
+        """
+        # remove from memory
+        self.remove_object_from_memory_by_id(obj_list, id_to_remove=obj_id)
+        # remove from file
+        line_numbers_in_file_to_remove = file.get_object_locations_for_id(obj_id)
+        # get table_header and footers
+        remove_empty_table_indices = self.check_for_empty_table(
+            file, line_numbers_in_file_to_remove, obj_id)
+        # remove the table if there aren't any more remaining
+        line_numbers_in_file_to_remove.extend(remove_empty_table_indices)
+        self.remove_lines_from_file(line_numbers_in_file_to_remove, file, obj_id)
```

### Comparing `ressimpy-1.0.0/ResSimpy/Nexus/NexusAquiferMethods.py` & `ressimpy-1.0.1/ResSimpy/Nexus/NexusAquiferMethods.py`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,69 +1,69 @@
-from dataclasses import dataclass
-import os
-from typing import Optional, MutableMapping
-from ResSimpy.Nexus.DataModels.NexusFile import NexusFile
-from ResSimpy.Nexus.DataModels.NexusAquiferMethod import NexusAquiferMethod
-from ResSimpy.Aquifer import Aquifer
-
-
-@dataclass(kw_only=True)
-class NexusAquiferMethods(Aquifer):
-    """Class for collection of Nexus aquifer methods.
-
-    Attributes:
-        inputs (dict[int, NexusAquiferMethod]): Collection of Nexus aquifer methods, as a dictionary
-        files (dict[int, NexusFile]): Dictionary collection of aquifer files, as defined in Nexus fcs file.
-    """
-
-    __inputs: MutableMapping[int, NexusAquiferMethod]
-    __files: dict[int, NexusFile]
-    __properties_loaded: bool = False  # Used in lazy loading
-
-    def __init__(self, inputs: Optional[MutableMapping[int, NexusAquiferMethod]] = None,
-                 files: Optional[dict[int, NexusFile]] = None) -> None:
-        if inputs:
-            self.__inputs = inputs
-        else:
-            self.__inputs: MutableMapping[int, NexusAquiferMethod] = {}
-        if files:
-            self.__files = files
-        else:
-            self.__files = {}
-        super().__init__()
-
-    def __repr__(self) -> str:
-        """Pretty printing aquifer methods."""
-        if not self.__properties_loaded:
-            self.load_aquifer_methods()
-        printable_str = ''
-        for table_num in self.__inputs.keys():
-            printable_str += '\n--------------------------------\n'
-            printable_str += f'AQUIFER method {table_num}\n'
-            printable_str += '--------------------------------\n'
-            printable_str += self.__inputs[table_num].__repr__()
-            printable_str += '\n'
-
-        return printable_str
-
-    @property
-    def inputs(self) -> MutableMapping[int, NexusAquiferMethod]:
-        if not self.__properties_loaded:
-            self.load_aquifer_methods()
-        return self.__inputs
-
-    @property
-    def files(self) -> dict[int, NexusFile]:
-        return self.__files
-
-    def load_aquifer_methods(self):
-        # Read in aquifer properties from Nexus aquifer method files
-        if self.__files is not None and len(self.__files) > 0:  # Check if aquifer files exist
-            for table_num in self.__files.keys():  # For each aquifer property method
-                aquifer_file = self.__files[table_num]
-                if aquifer_file.location is None:
-                    raise ValueError(f'Unable to find aquifer file: {aquifer_file.location}')
-                if os.path.isfile(aquifer_file.location):
-                    # Create NexusAquifer object
-                    self.__inputs[table_num] = NexusAquiferMethod(file=aquifer_file, input_number=table_num)
-                    self.__inputs[table_num].read_properties()  # Populate object with aquifer properties from file
-        self.__properties_loaded = True
+from dataclasses import dataclass
+import os
+from typing import Optional, MutableMapping
+from ResSimpy.Nexus.DataModels.NexusFile import NexusFile
+from ResSimpy.Nexus.DataModels.NexusAquiferMethod import NexusAquiferMethod
+from ResSimpy.Aquifer import Aquifer
+
+
+@dataclass(kw_only=True)
+class NexusAquiferMethods(Aquifer):
+    """Class for collection of Nexus aquifer methods.
+
+    Attributes:
+        inputs (dict[int, NexusAquiferMethod]): Collection of Nexus aquifer methods, as a dictionary
+        files (dict[int, NexusFile]): Dictionary collection of aquifer files, as defined in Nexus fcs file.
+    """
+
+    __inputs: MutableMapping[int, NexusAquiferMethod]
+    __files: dict[int, NexusFile]
+    __properties_loaded: bool = False  # Used in lazy loading
+
+    def __init__(self, inputs: Optional[MutableMapping[int, NexusAquiferMethod]] = None,
+                 files: Optional[dict[int, NexusFile]] = None) -> None:
+        if inputs:
+            self.__inputs = inputs
+        else:
+            self.__inputs: MutableMapping[int, NexusAquiferMethod] = {}
+        if files:
+            self.__files = files
+        else:
+            self.__files = {}
+        super().__init__()
+
+    def __repr__(self) -> str:
+        """Pretty printing aquifer methods."""
+        if not self.__properties_loaded:
+            self.load_aquifer_methods()
+        printable_str = ''
+        for table_num in self.__inputs.keys():
+            printable_str += '\n--------------------------------\n'
+            printable_str += f'AQUIFER method {table_num}\n'
+            printable_str += '--------------------------------\n'
+            printable_str += self.__inputs[table_num].__repr__()
+            printable_str += '\n'
+
+        return printable_str
+
+    @property
+    def inputs(self) -> MutableMapping[int, NexusAquiferMethod]:
+        if not self.__properties_loaded:
+            self.load_aquifer_methods()
+        return self.__inputs
+
+    @property
+    def files(self) -> dict[int, NexusFile]:
+        return self.__files
+
+    def load_aquifer_methods(self):
+        # Read in aquifer properties from Nexus aquifer method files
+        if self.__files is not None and len(self.__files) > 0:  # Check if aquifer files exist
+            for table_num in self.__files.keys():  # For each aquifer property method
+                aquifer_file = self.__files[table_num]
+                if aquifer_file.location is None:
+                    raise ValueError(f'Unable to find aquifer file: {aquifer_file.location}')
+                if os.path.isfile(aquifer_file.location):
+                    # Create NexusAquifer object
+                    self.__inputs[table_num] = NexusAquiferMethod(file=aquifer_file, input_number=table_num)
+                    self.__inputs[table_num].read_properties()  # Populate object with aquifer properties from file
+        self.__properties_loaded = True
```

### Comparing `ressimpy-1.0.0/ResSimpy/Nexus/NexusEquilMethods.py` & `ressimpy-1.0.1/ResSimpy/Nexus/NexusEquilMethods.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,69 +1,69 @@
-from dataclasses import dataclass
-import os
-from typing import Optional, MutableMapping
-from ResSimpy.Nexus.DataModels.NexusFile import NexusFile
-from ResSimpy.Nexus.DataModels.NexusEquilMethod import NexusEquilMethod
-from ResSimpy.Equilibration import Equilibration
-
-
-@dataclass(kw_only=True)
-class NexusEquilMethods(Equilibration):
-    """Class for collection of Nexus equilibration methods.
-
-    Attributes:
-        inputs (dict[int, NexusEquilMethod]): Collection of Nexus equilibration methods, as a dictionary
-        files (dict[int, NexusFile]): Dictionary collection of equilibration files, as defined in Nexus fcs file.
-    """
-
-    __inputs: MutableMapping[int, NexusEquilMethod]
-    __files: dict[int, NexusFile]
-    __properties_loaded: bool = False  # Used in lazy loading
-
-    def __init__(self, inputs: Optional[MutableMapping[int, NexusEquilMethod]] = None,
-                 files: Optional[dict[int, NexusFile]] = None) -> None:
-        if inputs:
-            self.__inputs = inputs
-        else:
-            self.__inputs: MutableMapping[int, NexusEquilMethod] = {}
-        if files:
-            self.__files = files
-        else:
-            self.__files = {}
-        super().__init__()
-
-    def __repr__(self) -> str:
-        """Pretty printing equil methods."""
-        if not self.__properties_loaded:
-            self.load_equil_methods()
-        printable_str = ''
-        for table_num in self.__inputs.keys():
-            printable_str += '\n--------------------------------\n'
-            printable_str += f'EQUIL method {table_num}\n'
-            printable_str += '--------------------------------\n'
-            printable_str += self.__inputs[table_num].__repr__()
-            printable_str += '\n'
-
-        return printable_str
-
-    @property
-    def inputs(self) -> MutableMapping[int, NexusEquilMethod]:
-        if not self.__properties_loaded:
-            self.load_equil_methods()
-        return self.__inputs
-
-    @property
-    def files(self) -> dict[int, NexusFile]:
-        return self.__files
-
-    def load_equil_methods(self):
-        # Read in equil properties from Nexus equil method files
-        if self.__files is not None and len(self.__files) > 0:  # Check if equil files exist
-            for table_num in self.__files.keys():  # For each equil property method
-                equil_file = self.__files[table_num]
-                if equil_file.location is None:
-                    raise ValueError(f'Unable to find equil file: {equil_file}')
-                if os.path.isfile(equil_file.location):
-                    # Create NexusEquilMethod object
-                    self.__inputs[table_num] = NexusEquilMethod(file=equil_file, input_number=table_num)
-                    self.__inputs[table_num].read_properties()  # Populate object with equil properties in file
-        self.__properties_loaded = True
+from dataclasses import dataclass
+import os
+from typing import Optional, MutableMapping
+from ResSimpy.Nexus.DataModels.NexusFile import NexusFile
+from ResSimpy.Nexus.DataModels.NexusEquilMethod import NexusEquilMethod
+from ResSimpy.Equilibration import Equilibration
+
+
+@dataclass(kw_only=True)
+class NexusEquilMethods(Equilibration):
+    """Class for collection of Nexus equilibration methods.
+
+    Attributes:
+        inputs (dict[int, NexusEquilMethod]): Collection of Nexus equilibration methods, as a dictionary
+        files (dict[int, NexusFile]): Dictionary collection of equilibration files, as defined in Nexus fcs file.
+    """
+
+    __inputs: MutableMapping[int, NexusEquilMethod]
+    __files: dict[int, NexusFile]
+    __properties_loaded: bool = False  # Used in lazy loading
+
+    def __init__(self, inputs: Optional[MutableMapping[int, NexusEquilMethod]] = None,
+                 files: Optional[dict[int, NexusFile]] = None) -> None:
+        if inputs:
+            self.__inputs = inputs
+        else:
+            self.__inputs: MutableMapping[int, NexusEquilMethod] = {}
+        if files:
+            self.__files = files
+        else:
+            self.__files = {}
+        super().__init__()
+
+    def __repr__(self) -> str:
+        """Pretty printing equil methods."""
+        if not self.__properties_loaded:
+            self.load_equil_methods()
+        printable_str = ''
+        for table_num in self.__inputs.keys():
+            printable_str += '\n--------------------------------\n'
+            printable_str += f'EQUIL method {table_num}\n'
+            printable_str += '--------------------------------\n'
+            printable_str += self.__inputs[table_num].__repr__()
+            printable_str += '\n'
+
+        return printable_str
+
+    @property
+    def inputs(self) -> MutableMapping[int, NexusEquilMethod]:
+        if not self.__properties_loaded:
+            self.load_equil_methods()
+        return self.__inputs
+
+    @property
+    def files(self) -> dict[int, NexusFile]:
+        return self.__files
+
+    def load_equil_methods(self):
+        # Read in equil properties from Nexus equil method files
+        if self.__files is not None and len(self.__files) > 0:  # Check if equil files exist
+            for table_num in self.__files.keys():  # For each equil property method
+                equil_file = self.__files[table_num]
+                if equil_file.location is None:
+                    raise ValueError(f'Unable to find equil file: {equil_file}')
+                if os.path.isfile(equil_file.location):
+                    # Create NexusEquilMethod object
+                    self.__inputs[table_num] = NexusEquilMethod(file=equil_file, input_number=table_num)
+                    self.__inputs[table_num].read_properties()  # Populate object with equil properties in file
+        self.__properties_loaded = True
```

### Comparing `ressimpy-1.0.0/ResSimpy/Nexus/NexusHydraulicsMethods.py` & `ressimpy-1.0.1/ResSimpy/Nexus/NexusHydraulicsMethods.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,69 +1,69 @@
-from dataclasses import dataclass
-import os
-from typing import Optional, MutableMapping
-from ResSimpy.Nexus.DataModels.NexusFile import NexusFile
-from ResSimpy.Nexus.DataModels.NexusHydraulicsMethod import NexusHydraulicsMethod
-from ResSimpy.Hydraulics import Hydraulics
-
-
-@dataclass(kw_only=True)
-class NexusHydraulicsMethods(Hydraulics):
-    """Class for collection of Nexus hydraulics methods.
-
-    Attributes:
-        inputs (dict[int, NexusHydraulicsMethod]): Collection of Nexus hydraulics methods, as a dictionary
-        files (dict[int, NexusFile]): Dictionary collection of hydraulics files, in Nexus fcs file.
-    """
-
-    __inputs: MutableMapping[int, NexusHydraulicsMethod]
-    __files: dict[int, NexusFile]
-    __properties_loaded: bool = False  # Used in lazy loading
-
-    def __init__(self, inputs: Optional[MutableMapping[int, NexusHydraulicsMethod]] = None,
-                 files: Optional[dict[int, NexusFile]] = None) -> None:
-        if inputs:
-            self.__inputs = inputs
-        else:
-            self.__inputs: MutableMapping[int, NexusHydraulicsMethod] = {}
-        if files:
-            self.__files = files
-        else:
-            self.__files = {}
-        super().__init__()
-
-    def __repr__(self) -> str:
-        """Pretty printing hydraulics methods."""
-        if not self.__properties_loaded:
-            self.load_hydraulics_methods()
-        printable_str = ''
-        for table_num in self.__inputs.keys():
-            printable_str += '\n--------------------------------\n'
-            printable_str += f'HYD method {table_num}\n'
-            printable_str += '--------------------------------\n'
-            printable_str += self.__inputs[table_num].__repr__()
-            printable_str += '\n'
-
-        return printable_str
-
-    @property
-    def inputs(self) -> MutableMapping[int, NexusHydraulicsMethod]:
-        if not self.__properties_loaded:
-            self.load_hydraulics_methods()
-        return self.__inputs
-
-    @property
-    def files(self) -> dict[int, NexusFile]:
-        return self.__files
-
-    def load_hydraulics_methods(self):
-        # Read in hydraulics properties from Nexus hydraulics method files
-        if self.__files is not None and len(self.__files) > 0:  # Check if hydraulics files exist
-            for table_num in self.__files.keys():  # For each hydraulics property method
-                hydraulics_file = self.__files[table_num]
-                if hydraulics_file.location is None:
-                    raise ValueError(f'Unable to find hydraulics file: {hydraulics_file}')
-                if os.path.isfile(hydraulics_file.location):
-                    # Create NexusHydraulicsMethod object
-                    self.__inputs[table_num] = NexusHydraulicsMethod(file=hydraulics_file, input_number=table_num)
-                    self.__inputs[table_num].read_properties()  # Populate object with hydraulics props
-        self.__properties_loaded = True
+from dataclasses import dataclass
+import os
+from typing import Optional, MutableMapping
+from ResSimpy.Nexus.DataModels.NexusFile import NexusFile
+from ResSimpy.Nexus.DataModels.NexusHydraulicsMethod import NexusHydraulicsMethod
+from ResSimpy.Hydraulics import Hydraulics
+
+
+@dataclass(kw_only=True)
+class NexusHydraulicsMethods(Hydraulics):
+    """Class for collection of Nexus hydraulics methods.
+
+    Attributes:
+        inputs (dict[int, NexusHydraulicsMethod]): Collection of Nexus hydraulics methods, as a dictionary
+        files (dict[int, NexusFile]): Dictionary collection of hydraulics files, in Nexus fcs file.
+    """
+
+    __inputs: MutableMapping[int, NexusHydraulicsMethod]
+    __files: dict[int, NexusFile]
+    __properties_loaded: bool = False  # Used in lazy loading
+
+    def __init__(self, inputs: Optional[MutableMapping[int, NexusHydraulicsMethod]] = None,
+                 files: Optional[dict[int, NexusFile]] = None) -> None:
+        if inputs:
+            self.__inputs = inputs
+        else:
+            self.__inputs: MutableMapping[int, NexusHydraulicsMethod] = {}
+        if files:
+            self.__files = files
+        else:
+            self.__files = {}
+        super().__init__()
+
+    def __repr__(self) -> str:
+        """Pretty printing hydraulics methods."""
+        if not self.__properties_loaded:
+            self.load_hydraulics_methods()
+        printable_str = ''
+        for table_num in self.__inputs.keys():
+            printable_str += '\n--------------------------------\n'
+            printable_str += f'HYD method {table_num}\n'
+            printable_str += '--------------------------------\n'
+            printable_str += self.__inputs[table_num].__repr__()
+            printable_str += '\n'
+
+        return printable_str
+
+    @property
+    def inputs(self) -> MutableMapping[int, NexusHydraulicsMethod]:
+        if not self.__properties_loaded:
+            self.load_hydraulics_methods()
+        return self.__inputs
+
+    @property
+    def files(self) -> dict[int, NexusFile]:
+        return self.__files
+
+    def load_hydraulics_methods(self):
+        # Read in hydraulics properties from Nexus hydraulics method files
+        if self.__files is not None and len(self.__files) > 0:  # Check if hydraulics files exist
+            for table_num in self.__files.keys():  # For each hydraulics property method
+                hydraulics_file = self.__files[table_num]
+                if hydraulics_file.location is None:
+                    raise ValueError(f'Unable to find hydraulics file: {hydraulics_file}')
+                if os.path.isfile(hydraulics_file.location):
+                    # Create NexusHydraulicsMethod object
+                    self.__inputs[table_num] = NexusHydraulicsMethod(file=hydraulics_file, input_number=table_num)
+                    self.__inputs[table_num].read_properties()  # Populate object with hydraulics props
+        self.__properties_loaded = True
```

### Comparing `ressimpy-1.0.0/ResSimpy/Nexus/NexusKeywords/equil_keywords.py` & `ressimpy-1.0.1/ResSimpy/Nexus/NexusKeywords/equil_keywords.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-
-EQUIL_KEYWORDS_VALUE_FLOAT = ['PINIT', 'DINIT', 'TINIT', 'GOC', 'WOC', 'PCGOC', 'PCWOC', 'PSAT', 'API', 'GWC',
-                              'PCGWC', 'SALINITY', 'CHLORIDE', 'CALCIUM', 'LI_FACTOR', 'LI_AUTO',
-                              'SORWMN', 'SORGMN', 'SGCMN', 'VAITS_TOLSG', 'VAITS_TOLSW',
-                              'WOC_PALEO', 'GOC_PALEO']
-EQUIL_KEYWORDS_VALUE_STR = ['OVERREAD', 'AUTOGOC_COMP', 'VIP_INIT']
-EQUIL_OVERREAD_VALUES = ['PRESSURE', 'SW', 'SG', 'MOLEFRACTION']
-EQUIL_SINGLE_KEYWORDS = ['WATERZONE_NEW_INIT', 'LI_AUTO_GAS', 'KEEPSG', 'KEEPSW', 'HONOR_GZONE', 'HONOR_WZONE',
-                         'PCADJ_SCALING', 'NONEQ', 'SEDIMENTATION', 'MATCHVIPPRES', 'NOMATCHVIPPRES', 'CRINIT',
-                         'HONOR_GASPRESSURE_GWC', 'POROSITY_INDEPENDENCE', 'POROSITY_DEPENDENCE']
-EQUIL_INTSAT_KEYWORDS = ['INTSAT', 'VAITS']
-EQUIL_TABLE_KEYWORDS = ['DEPTHVAR', 'OILMF', 'GASMF', 'COMPOSITION']
-EQUIL_COMPOSITION_OPTIONS = ['X', 'Y']
-EQUIL_TABLE_HEADERS = ['DEPTH', 'PSAT', 'TEMP', 'API', 'SALINITY', 'CHLORIDE', 'CALCIUM', 'X', 'Y']
-EQUIL_KEYWORDS = EQUIL_KEYWORDS_VALUE_FLOAT + EQUIL_KEYWORDS_VALUE_STR + EQUIL_SINGLE_KEYWORDS + \
-    EQUIL_INTSAT_KEYWORDS + EQUIL_TABLE_KEYWORDS
+
+EQUIL_KEYWORDS_VALUE_FLOAT = ['PINIT', 'DINIT', 'TINIT', 'GOC', 'WOC', 'PCGOC', 'PCWOC', 'PSAT', 'API', 'GWC',
+                              'PCGWC', 'SALINITY', 'CHLORIDE', 'CALCIUM', 'LI_FACTOR', 'LI_AUTO',
+                              'SORWMN', 'SORGMN', 'SGCMN', 'VAITS_TOLSG', 'VAITS_TOLSW',
+                              'WOC_PALEO', 'GOC_PALEO']
+EQUIL_KEYWORDS_VALUE_STR = ['OVERREAD', 'AUTOGOC_COMP', 'VIP_INIT']
+EQUIL_OVERREAD_VALUES = ['PRESSURE', 'SW', 'SG', 'MOLEFRACTION']
+EQUIL_SINGLE_KEYWORDS = ['WATERZONE_NEW_INIT', 'LI_AUTO_GAS', 'KEEPSG', 'KEEPSW', 'HONOR_GZONE', 'HONOR_WZONE',
+                         'PCADJ_SCALING', 'NONEQ', 'SEDIMENTATION', 'MATCHVIPPRES', 'NOMATCHVIPPRES', 'CRINIT',
+                         'HONOR_GASPRESSURE_GWC', 'POROSITY_INDEPENDENCE', 'POROSITY_DEPENDENCE']
+EQUIL_INTSAT_KEYWORDS = ['INTSAT', 'VAITS']
+EQUIL_TABLE_KEYWORDS = ['DEPTHVAR', 'OILMF', 'GASMF', 'COMPOSITION']
+EQUIL_COMPOSITION_OPTIONS = ['X', 'Y']
+EQUIL_TABLE_HEADERS = ['DEPTH', 'PSAT', 'TEMP', 'API', 'SALINITY', 'CHLORIDE', 'CALCIUM', 'X', 'Y']
+EQUIL_KEYWORDS = EQUIL_KEYWORDS_VALUE_FLOAT + EQUIL_KEYWORDS_VALUE_STR + EQUIL_SINGLE_KEYWORDS + \
+    EQUIL_INTSAT_KEYWORDS + EQUIL_TABLE_KEYWORDS
```

### Comparing `ressimpy-1.0.0/ResSimpy/Nexus/NexusKeywords/fcs_keywords.py` & `ressimpy-1.0.1/ResSimpy/Nexus/NexusKeywords/fcs_keywords.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-FCS_KEYWORDS = ['RESERVOIR', 'EQUIL', 'EOS_DEFAULTS', 'TRACER_INIT', 'STRUCTURED_GRID', 'OPTIONS', 'ROCK', 'RELPM',
-                'ADSORPTION', 'PVT', 'SEPARATOR', 'ALPHAF', 'POLYMER', 'WATER', 'AQUIFER', 'FLUXIN', 'RUNCONTROL',
-                'WELLS', 'SURFACE', 'IPR', 'GASLIFT', 'VALVE', 'HYD', 'PUMP', 'COMPRESSOR', 'CHOKE', 'ICD', 'ESP']
-
-# TODO: Not a complete list. Check manual for missing keywords.
-# TODO: Delete the keywords that are not tokens (i.e. that are only values in a table)
-
-FCS_ALL_KEYWORDS = ['ADSORPTION', 'ALPHA', 'ALPHAF', 'AQUIFER', 'AQUIFER_FILES', 'CASE', 'CHOKE', 'COMPRESSOR',
-                    'DATEFORMAT', 'DD/MM/YYYY', 'DEFAULT_SUNITS', 'DEFAULT_UNITS', 'DESC', 'ENGLISH', 'EOS_DEFAULTS',
-                    'EQUIL', 'ESP', 'FIELD', 'FLUXIN', 'GASLIFT', 'GRID_FILES', 'HYD', 'ICD',
-                    'INITIALIZATION_FILES', 'IPR', 'LGR', 'METBAR', 'METHOD', 'MM/DD/YYYY', 'NET_METHOD_FILES', 'ON',
-                    'OPTIONS', 'OVERRIDE', 'POLYMER', 'PPM', 'PROPERTY_FILES', 'PUMP', 'PVT', 'PVT_FILES',
-                    'RECURRENT_FILES', 'RELPM', 'RESERVOIR', 'RESTART', 'ROCK', 'ROCK_FILES', 'RUNCONTROL',
-                    'RUN_SUNITS',
-                    'RUN_UNITS', 'SEPARATOR', 'STRUCTURED_GRID', 'SURFACE', 'TIME', 'TRACER_INIT', 'VALVE', 'VIP',
-                    'WATER',
-                    'WELLS', 'X']
+FCS_KEYWORDS = ['RESERVOIR', 'EQUIL', 'EOS_DEFAULTS', 'TRACER_INIT', 'STRUCTURED_GRID', 'OPTIONS', 'ROCK', 'RELPM',
+                'ADSORPTION', 'PVT', 'SEPARATOR', 'ALPHAF', 'POLYMER', 'WATER', 'AQUIFER', 'FLUXIN', 'RUNCONTROL',
+                'WELLS', 'SURFACE', 'IPR', 'GASLIFT', 'VALVE', 'HYD', 'PUMP', 'COMPRESSOR', 'CHOKE', 'ICD', 'ESP']
+
+# TODO: Not a complete list. Check manual for missing keywords.
+# TODO: Delete the keywords that are not tokens (i.e. that are only values in a table)
+
+FCS_ALL_KEYWORDS = ['ADSORPTION', 'ALPHA', 'ALPHAF', 'AQUIFER', 'AQUIFER_FILES', 'CASE', 'CHOKE', 'COMPRESSOR',
+                    'DATEFORMAT', 'DD/MM/YYYY', 'DEFAULT_SUNITS', 'DEFAULT_UNITS', 'DESC', 'ENGLISH', 'EOS_DEFAULTS',
+                    'EQUIL', 'ESP', 'FIELD', 'FLUXIN', 'GASLIFT', 'GRID_FILES', 'HYD', 'ICD',
+                    'INITIALIZATION_FILES', 'IPR', 'LGR', 'METBAR', 'METHOD', 'MM/DD/YYYY', 'NET_METHOD_FILES', 'ON',
+                    'OPTIONS', 'OVERRIDE', 'POLYMER', 'PPM', 'PROPERTY_FILES', 'PUMP', 'PVT', 'PVT_FILES',
+                    'RECURRENT_FILES', 'RELPM', 'RESERVOIR', 'RESTART', 'ROCK', 'ROCK_FILES', 'RUNCONTROL',
+                    'RUN_SUNITS',
+                    'RUN_UNITS', 'SEPARATOR', 'STRUCTURED_GRID', 'SURFACE', 'TIME', 'TRACER_INIT', 'VALVE', 'VIP',
+                    'WATER',
+                    'WELLS', 'X']
```

### Comparing `ressimpy-1.0.0/ResSimpy/Nexus/NexusKeywords/hyd_keywords.py` & `ressimpy-1.0.1/ResSimpy/Nexus/NexusKeywords/hyd_keywords.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-HYD_RATE_KEYWORDS = ['QOIL', 'QLIQ', 'QGAS', 'QWAT', 'QWGAS']
-HYD_GAS_RATIO_KEYWORDS = ['GOR', 'GLR', 'OGR', 'GWR', 'MMW']
-HYD_WATER_RATIO_KEYWORDS = ['WCUT', 'WGR', 'OCUT', 'WWGR']
-HYD_PRESSURE_KEYWORDS = ['PIN', 'POUT', 'THP']
-HYD_ARRAY_KEYWORDS = HYD_RATE_KEYWORDS + HYD_GAS_RATIO_KEYWORDS + HYD_WATER_RATIO_KEYWORDS + HYD_GAS_RATIO_KEYWORDS + \
-    HYD_PRESSURE_KEYWORDS
-HYD_ALQ_KEYWORD = ['ALQ']
-HYD_ALQ_OPTIONS = ['GASRATE', 'NOTGLIFT']
-
-HYD_CORRECTION_KEYWORD = ['DATGRAD']
-HYD_CORRECTION_OPTIONS = ['GRAD', 'OILGRAD', 'GASGRAD', 'WATERGRAD']
-
-HYD_KEYWORDS_VALUE_FLOAT = ['LENGTH', 'DATUM', 'DZW']
-HYD_SINGLE_KEYWORDS = ['NOCHK']
-
-HYD_TABLE_HEADER_COLS = ['IGOR', 'IWCUT', 'IQOIL', 'IALG', 'BHP(ITHP)', 'IGLR', 'IQLIQ', 'IOGR', 'IWGR', 'IQGAS',
-                         'IGWR', 'IOCUT', 'IQWAT', 'IMMW', 'IWWGR', 'IQWGAS']
-
-HYD_LIMITS_KEYWORD = ['LIMITS']
-
-HYD_WATINJ_KEYWORD = ['WATINJ']
-HYD_WATINJ_KEYWORDS_VALUE_FLOAT = ['GRAD', 'VISC', 'DIAM', 'LENGTH', 'DZ', 'ROUGHNESS']
-
-HYD_KEYWORDS = HYD_ARRAY_KEYWORDS + HYD_ALQ_KEYWORD + HYD_CORRECTION_KEYWORD + HYD_KEYWORDS_VALUE_FLOAT + \
-    HYD_SINGLE_KEYWORDS + HYD_LIMITS_KEYWORD + HYD_WATINJ_KEYWORD
+HYD_RATE_KEYWORDS = ['QOIL', 'QLIQ', 'QGAS', 'QWAT', 'QWGAS']
+HYD_GAS_RATIO_KEYWORDS = ['GOR', 'GLR', 'OGR', 'GWR', 'MMW']
+HYD_WATER_RATIO_KEYWORDS = ['WCUT', 'WGR', 'OCUT', 'WWGR']
+HYD_PRESSURE_KEYWORDS = ['PIN', 'POUT', 'THP']
+HYD_ARRAY_KEYWORDS = HYD_RATE_KEYWORDS + HYD_GAS_RATIO_KEYWORDS + HYD_WATER_RATIO_KEYWORDS + HYD_GAS_RATIO_KEYWORDS + \
+    HYD_PRESSURE_KEYWORDS
+HYD_ALQ_KEYWORD = ['ALQ']
+HYD_ALQ_OPTIONS = ['GASRATE', 'NOTGLIFT']
+
+HYD_CORRECTION_KEYWORD = ['DATGRAD']
+HYD_CORRECTION_OPTIONS = ['GRAD', 'OILGRAD', 'GASGRAD', 'WATERGRAD']
+
+HYD_KEYWORDS_VALUE_FLOAT = ['LENGTH', 'DATUM', 'DZW']
+HYD_SINGLE_KEYWORDS = ['NOCHK']
+
+HYD_TABLE_HEADER_COLS = ['IGOR', 'IWCUT', 'IQOIL', 'IALG', 'BHP(ITHP)', 'IGLR', 'IQLIQ', 'IOGR', 'IWGR', 'IQGAS',
+                         'IGWR', 'IOCUT', 'IQWAT', 'IMMW', 'IWWGR', 'IQWGAS']
+
+HYD_LIMITS_KEYWORD = ['LIMITS']
+
+HYD_WATINJ_KEYWORD = ['WATINJ']
+HYD_WATINJ_KEYWORDS_VALUE_FLOAT = ['GRAD', 'VISC', 'DIAM', 'LENGTH', 'DZ', 'ROUGHNESS']
+
+HYD_KEYWORDS = HYD_ARRAY_KEYWORDS + HYD_ALQ_KEYWORD + HYD_CORRECTION_KEYWORD + HYD_KEYWORDS_VALUE_FLOAT + \
+    HYD_SINGLE_KEYWORDS + HYD_LIMITS_KEYWORD + HYD_WATINJ_KEYWORD
```

### Comparing `ressimpy-1.0.0/ResSimpy/Nexus/NexusKeywords/nexus_keywords.py` & `ressimpy-1.0.1/ResSimpy/Nexus/NexusKeywords/nexus_keywords.py`

 * *Ordering differences only*

 * *Files 5% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-# A list of valid Nexus Tokens. Please add to this as you find / use them.
-from ResSimpy.Nexus.NexusKeywords.aquifer_keywords import AQUIFER_KEYWORDS
-from ResSimpy.Nexus.NexusKeywords.equil_keywords import EQUIL_KEYWORDS
-from ResSimpy.Nexus.NexusKeywords.fcs_keywords import FCS_ALL_KEYWORDS
-from ResSimpy.Nexus.NexusKeywords.gaslift_keywords import GASLIFT_KEYWORDS
-from ResSimpy.Nexus.NexusKeywords.hyd_keywords import HYD_KEYWORDS
-from ResSimpy.Nexus.NexusKeywords.options_keywords import OPTIONS_KEYWORDS
-from ResSimpy.Nexus.NexusKeywords.pvt_keywords import PVT_KEYWORDS
-from ResSimpy.Nexus.NexusKeywords.relpm_keywords import RELPM_KEYWORDS
-from ResSimpy.Nexus.NexusKeywords.rock_keywords import ROCK_KEYWORDS
-from ResSimpy.Nexus.NexusKeywords.runcontrol_keywords import RUNCONTROL_KEYWORDS
-from ResSimpy.Nexus.NexusKeywords.separator_keywords import SEPARATOR_KEYWORDS
-from ResSimpy.Nexus.NexusKeywords.structured_grid_keywords import GRID_ARRAY_KEYWORDS, STRUCTURED_GRID_KEYWORDS
-from ResSimpy.Nexus.NexusKeywords.surface_keywords import SURFACE_KEYWORDS, CONNECTION_KEYWORDS
-from ResSimpy.Nexus.NexusKeywords.valve_keywords import VALVE_KEYWORDS
-from ResSimpy.Nexus.NexusKeywords.water_keywords import WATER_KEYWORDS
-from ResSimpy.Nexus.NexusKeywords.wells_keywords import WELLS_KEYWORDS
-
-GENERAL_KEYWORDS = ['DESC', 'LABEL']
-
-RELPERM_ENDPT_KEYWORDS = ['SWL', 'SWR', 'SWU', 'SGL', 'SGR', 'SGU', 'SWRO', 'SGRO', 'SGRW', 'KRW_SWRO', 'KRW_SWU',
-                          'KRG_SGRO', 'KRG_SGU', 'KRO_SWL', 'KRO_SWR', 'KRO_SGL', 'KRO_SGR', 'KRW_SGL', 'KRW_SGR',
-                          'KRG_SGRW', 'SGTR', 'SOTR']
-
-UNIT_KEYWORDS = ['ENGLISH', 'METRIC', 'METKG/CM2', 'METBAR', 'LAB', 'FAHR', 'CELSIUS', 'KELVIN', 'RANKINE']
-
-# Keywords that sometimes follow other keywords before the value
-INTERMEDIATE_KEYWORDS = ['SET', 'METHOD', 'NETWORK']  # always followed by an int, then a file path
-
-# Keywords that require another keyword after their declaration
-STARTING_KEYWORDS = ['RESTART']
-
-# Combine all lists into the complete list
-VALID_NEXUS_KEYWORDS = GENERAL_KEYWORDS + RUNCONTROL_KEYWORDS + UNIT_KEYWORDS \
-                       + INTERMEDIATE_KEYWORDS + STARTING_KEYWORDS + RELPERM_ENDPT_KEYWORDS + PVT_KEYWORDS \
-                       + FCS_ALL_KEYWORDS + WELLS_KEYWORDS + WATER_KEYWORDS + VALVE_KEYWORDS + SURFACE_KEYWORDS + \
-                       CONNECTION_KEYWORDS + GRID_ARRAY_KEYWORDS + STRUCTURED_GRID_KEYWORDS + SEPARATOR_KEYWORDS + \
-                       ROCK_KEYWORDS + AQUIFER_KEYWORDS + EQUIL_KEYWORDS + GASLIFT_KEYWORDS + HYD_KEYWORDS + \
-                       OPTIONS_KEYWORDS + PVT_KEYWORDS + RELPM_KEYWORDS + WELLS_KEYWORDS
+# A list of valid Nexus Tokens. Please add to this as you find / use them.
+from ResSimpy.Nexus.NexusKeywords.aquifer_keywords import AQUIFER_KEYWORDS
+from ResSimpy.Nexus.NexusKeywords.equil_keywords import EQUIL_KEYWORDS
+from ResSimpy.Nexus.NexusKeywords.fcs_keywords import FCS_ALL_KEYWORDS
+from ResSimpy.Nexus.NexusKeywords.gaslift_keywords import GASLIFT_KEYWORDS
+from ResSimpy.Nexus.NexusKeywords.hyd_keywords import HYD_KEYWORDS
+from ResSimpy.Nexus.NexusKeywords.options_keywords import OPTIONS_KEYWORDS
+from ResSimpy.Nexus.NexusKeywords.pvt_keywords import PVT_KEYWORDS
+from ResSimpy.Nexus.NexusKeywords.relpm_keywords import RELPM_KEYWORDS
+from ResSimpy.Nexus.NexusKeywords.rock_keywords import ROCK_KEYWORDS
+from ResSimpy.Nexus.NexusKeywords.runcontrol_keywords import RUNCONTROL_KEYWORDS
+from ResSimpy.Nexus.NexusKeywords.separator_keywords import SEPARATOR_KEYWORDS
+from ResSimpy.Nexus.NexusKeywords.structured_grid_keywords import GRID_ARRAY_KEYWORDS, STRUCTURED_GRID_KEYWORDS
+from ResSimpy.Nexus.NexusKeywords.surface_keywords import SURFACE_KEYWORDS, CONNECTION_KEYWORDS
+from ResSimpy.Nexus.NexusKeywords.valve_keywords import VALVE_KEYWORDS
+from ResSimpy.Nexus.NexusKeywords.water_keywords import WATER_KEYWORDS
+from ResSimpy.Nexus.NexusKeywords.wells_keywords import WELLS_KEYWORDS
+
+GENERAL_KEYWORDS = ['DESC', 'LABEL']
+
+RELPERM_ENDPT_KEYWORDS = ['SWL', 'SWR', 'SWU', 'SGL', 'SGR', 'SGU', 'SWRO', 'SGRO', 'SGRW', 'KRW_SWRO', 'KRW_SWU',
+                          'KRG_SGRO', 'KRG_SGU', 'KRO_SWL', 'KRO_SWR', 'KRO_SGL', 'KRO_SGR', 'KRW_SGL', 'KRW_SGR',
+                          'KRG_SGRW', 'SGTR', 'SOTR']
+
+UNIT_KEYWORDS = ['ENGLISH', 'METRIC', 'METKG/CM2', 'METBAR', 'LAB', 'FAHR', 'CELSIUS', 'KELVIN', 'RANKINE']
+
+# Keywords that sometimes follow other keywords before the value
+INTERMEDIATE_KEYWORDS = ['SET', 'METHOD', 'NETWORK']  # always followed by an int, then a file path
+
+# Keywords that require another keyword after their declaration
+STARTING_KEYWORDS = ['RESTART']
+
+# Combine all lists into the complete list
+VALID_NEXUS_KEYWORDS = GENERAL_KEYWORDS + RUNCONTROL_KEYWORDS + UNIT_KEYWORDS \
+                       + INTERMEDIATE_KEYWORDS + STARTING_KEYWORDS + RELPERM_ENDPT_KEYWORDS + PVT_KEYWORDS \
+                       + FCS_ALL_KEYWORDS + WELLS_KEYWORDS + WATER_KEYWORDS + VALVE_KEYWORDS + SURFACE_KEYWORDS + \
+                       CONNECTION_KEYWORDS + GRID_ARRAY_KEYWORDS + STRUCTURED_GRID_KEYWORDS + SEPARATOR_KEYWORDS + \
+                       ROCK_KEYWORDS + AQUIFER_KEYWORDS + EQUIL_KEYWORDS + GASLIFT_KEYWORDS + HYD_KEYWORDS + \
+                       OPTIONS_KEYWORDS + PVT_KEYWORDS + RELPM_KEYWORDS + WELLS_KEYWORDS
```

### Comparing `ressimpy-1.0.0/ResSimpy/Nexus/NexusKeywords/options_keywords.py` & `ressimpy-1.0.1/ResSimpy/Nexus/NexusKeywords/options_keywords.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# TODO: Not a complete list. Check manual for missing keywords.
-# TODO: Delete the keywords that are not tokens (i.e. that are only values in a table)
-
-OPTIONS_KEYWORDS = ['ALL', 'AQUIFER', 'AUTO', 'CENTER', 'DATUM', 'DEF_DATUM', 'DESC', 'DP',
-                    'ENDGLOBAL_METHOD_OVERRIDES', 'ENDGRIDTOPROC', 'ENDREGBLK', 'ENDREGDATA', 'ENDSUBREGIONS',
-                    'EQ_LIST', 'FLEXDP', 'GLOBAL_METHOD_OVERRIDES', 'GRID', 'GRIDBLOCKS', 'GRIDTOPROC', 'INTSAT',
-                    'NAME', 'NOCHK_SAL_TEMP', 'NONEQ', 'NUMBER', 'OFF', 'OVERREAD', 'PATTERN', 'PC', 'PD',
-                    'POROSITY_INDEPENDENCE', 'PROCESS', 'PSTD', 'REGBLK', 'REGDATA', 'RESERVOIR', 'RES_TEMP', 'SOMOPT1',
-                    'STONE1', 'SUBREGION', 'SUBREGIONS', 'SW', 'TSTD', 'VIP_INJ_PERF_KR_SCALING']
+# TODO: Not a complete list. Check manual for missing keywords.
+# TODO: Delete the keywords that are not tokens (i.e. that are only values in a table)
+
+OPTIONS_KEYWORDS = ['ALL', 'AQUIFER', 'AUTO', 'CENTER', 'DATUM', 'DEF_DATUM', 'DESC', 'DP',
+                    'ENDGLOBAL_METHOD_OVERRIDES', 'ENDGRIDTOPROC', 'ENDREGBLK', 'ENDREGDATA', 'ENDSUBREGIONS',
+                    'EQ_LIST', 'FLEXDP', 'GLOBAL_METHOD_OVERRIDES', 'GRID', 'GRIDBLOCKS', 'GRIDTOPROC', 'INTSAT',
+                    'NAME', 'NOCHK_SAL_TEMP', 'NONEQ', 'NUMBER', 'OFF', 'OVERREAD', 'PATTERN', 'PC', 'PD',
+                    'POROSITY_INDEPENDENCE', 'PROCESS', 'PSTD', 'REGBLK', 'REGDATA', 'RESERVOIR', 'RES_TEMP', 'SOMOPT1',
+                    'STONE1', 'SUBREGION', 'SUBREGIONS', 'SW', 'TSTD', 'VIP_INJ_PERF_KR_SCALING']
```

### Comparing `ressimpy-1.0.0/ResSimpy/Nexus/NexusKeywords/pvt_keywords.py` & `ressimpy-1.0.1/ResSimpy/Nexus/NexusKeywords/pvt_keywords.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-# TODO: Delete the keywords that are not tokens (i.e. that are only values in a table)
-
-PVT_TYPE_KEYWORDS = ['BLACKOIL', 'WATEROIL', 'GASWATER', 'EOS']
-PVT_BLACKOIL_PRIMARY_KEYWORDS = ['DENOIL', 'API', 'GOR', 'OGR', 'DENGAS', 'SPECG', 'MWOR']
-PVT_EOS_METHODS = ['PR', 'PR_OLD', 'SRK', 'RK']
-PVT_EOSOPTIONS_PRIMARY_WORDS = ['ZGIBBS', 'ZGIBBS_OFF', 'FLASH_GIBBS_ON', 'FLASH_GIBBS_OFF', 'VSHIFTOFF',
-                                'STKATZOFF', 'CAPILLARYFLASH', 'VISPE']
-PVT_EOSOPTIONS_PRIMARY_KEYS_FLOAT = ['LI_FACT', 'LI_GAS', 'LI_GAS_TEST', 'LI_OIL', 'LI_OIL_TEST', 'TOL', 'TOLSS',
-                                     'TOLCRIT', 'ALPHAMU', 'LBC1', 'LBC2', 'LBC3', 'LBC4', 'LBC5', 'LBC6']
-PVT_EOSOPTIONS_PRIMARY_KEYS_INT = ['MCO2', 'FUGERR']
-PVT_EOSOPTIONS_TRANS_KEYS = ['NEIGHBOR', 'TEST', 'DELTA', 'VIP', 'B', 'ALL']
-PVT_EOSOPTIONS_TRANS_TEST_KEYS = ['GIBBS', 'INCRP', 'PSAT']
-PVT_EOSOPTIONS_PHASEID_KEYS = ['PREVIOUS', 'DENSITY', 'FLASH', 'OIL', 'GAS', 'PSAT', 'LI']
-PVT_EOSOPTIONS_TERTIARY_KEYS = ['TCRIT', 'TDELZ', 'TDELP', 'PHASEFRAC', 'THRESHOLD']
-PVT_TABLES_WITH_ENDWORDS = ['PROPS', 'BINA', 'PEDTUNE', 'VISKJ', 'VISKK', 'VISKKIJ',
-                            'IGS_CP', 'BINB', 'DIFF_OIL', 'DIFF_GAS']
-PVT_TABLES_WITHOUT_ENDWORDS = ['SATURATED', 'OIL', 'GAS']
-PVT_TABLE_KEYWORDS = PVT_TABLES_WITHOUT_ENDWORDS + PVT_TABLES_WITH_ENDWORDS
-PVT_UNSAT_TABLE_KEYWORDS = ['UNSATOIL', 'UNSATGAS']
-PVT_UNSAT_TABLE_INDICES = ['PSAT', 'RSSAT', 'PRES']
-PVT_ALL_TABLE_KEYWORDS = PVT_TABLE_KEYWORDS + PVT_UNSAT_TABLE_KEYWORDS
-PVT_GENERAL_KEYWORDS = ['ACENTR', 'API', 'APIGROUP', 'BG', 'BGFAC', 'BINA', 'BO', 'BOFAC', 'COMPONENT',
-                        'COMPONENTS', 'DENGAS', 'DENOIL', 'DP', 'ENDBINA', 'ENDPROPS', 'ENGLISH', 'EOSOPTIONS',
-                        'FAHR', 'GAS', 'INCLUDE', 'MOLWT', 'NHC', 'NOCHK', 'OIL', 'TRANSITION',
-                        'TRANS_OPTIMIZATION' + 'TRANS_TEST', 'OMEGAA', 'OMEGAB', 'PC', 'PR', 'PRES', 'PROPS',
-                        'PSAT', 'RS', 'RSSAT', 'RV', 'SATURATED', 'SPECG', 'TC', 'TEMP', 'UNSATGAS', 'UNSATOIL',
-                        'VG', 'VGFAC', 'VO', 'VOFAC', 'VSHIFT', 'ZC']
-PVT_KEYWORDS = PVT_TYPE_KEYWORDS + PVT_BLACKOIL_PRIMARY_KEYWORDS + PVT_EOS_METHODS + PVT_EOSOPTIONS_PRIMARY_WORDS + \
-               PVT_EOSOPTIONS_PRIMARY_KEYS_FLOAT + PVT_EOSOPTIONS_PRIMARY_KEYS_INT + PVT_EOSOPTIONS_TRANS_KEYS + \
-               PVT_ALL_TABLE_KEYWORDS + \
-               PVT_EOSOPTIONS_TRANS_TEST_KEYS + PVT_EOSOPTIONS_PHASEID_KEYS + PVT_EOSOPTIONS_TERTIARY_KEYS + \
-               PVT_GENERAL_KEYWORDS
+# TODO: Delete the keywords that are not tokens (i.e. that are only values in a table)
+
+PVT_TYPE_KEYWORDS = ['BLACKOIL', 'WATEROIL', 'GASWATER', 'EOS']
+PVT_BLACKOIL_PRIMARY_KEYWORDS = ['DENOIL', 'API', 'GOR', 'OGR', 'DENGAS', 'SPECG', 'MWOR']
+PVT_EOS_METHODS = ['PR', 'PR_OLD', 'SRK', 'RK']
+PVT_EOSOPTIONS_PRIMARY_WORDS = ['ZGIBBS', 'ZGIBBS_OFF', 'FLASH_GIBBS_ON', 'FLASH_GIBBS_OFF', 'VSHIFTOFF',
+                                'STKATZOFF', 'CAPILLARYFLASH', 'VISPE']
+PVT_EOSOPTIONS_PRIMARY_KEYS_FLOAT = ['LI_FACT', 'LI_GAS', 'LI_GAS_TEST', 'LI_OIL', 'LI_OIL_TEST', 'TOL', 'TOLSS',
+                                     'TOLCRIT', 'ALPHAMU', 'LBC1', 'LBC2', 'LBC3', 'LBC4', 'LBC5', 'LBC6']
+PVT_EOSOPTIONS_PRIMARY_KEYS_INT = ['MCO2', 'FUGERR']
+PVT_EOSOPTIONS_TRANS_KEYS = ['NEIGHBOR', 'TEST', 'DELTA', 'VIP', 'B', 'ALL']
+PVT_EOSOPTIONS_TRANS_TEST_KEYS = ['GIBBS', 'INCRP', 'PSAT']
+PVT_EOSOPTIONS_PHASEID_KEYS = ['PREVIOUS', 'DENSITY', 'FLASH', 'OIL', 'GAS', 'PSAT', 'LI']
+PVT_EOSOPTIONS_TERTIARY_KEYS = ['TCRIT', 'TDELZ', 'TDELP', 'PHASEFRAC', 'THRESHOLD']
+PVT_TABLES_WITH_ENDWORDS = ['PROPS', 'BINA', 'PEDTUNE', 'VISKJ', 'VISKK', 'VISKKIJ',
+                            'IGS_CP', 'BINB', 'DIFF_OIL', 'DIFF_GAS']
+PVT_TABLES_WITHOUT_ENDWORDS = ['SATURATED', 'OIL', 'GAS']
+PVT_TABLE_KEYWORDS = PVT_TABLES_WITHOUT_ENDWORDS + PVT_TABLES_WITH_ENDWORDS
+PVT_UNSAT_TABLE_KEYWORDS = ['UNSATOIL', 'UNSATGAS']
+PVT_UNSAT_TABLE_INDICES = ['PSAT', 'RSSAT', 'PRES']
+PVT_ALL_TABLE_KEYWORDS = PVT_TABLE_KEYWORDS + PVT_UNSAT_TABLE_KEYWORDS
+PVT_GENERAL_KEYWORDS = ['ACENTR', 'API', 'APIGROUP', 'BG', 'BGFAC', 'BINA', 'BO', 'BOFAC', 'COMPONENT',
+                        'COMPONENTS', 'DENGAS', 'DENOIL', 'DP', 'ENDBINA', 'ENDPROPS', 'ENGLISH', 'EOSOPTIONS',
+                        'FAHR', 'GAS', 'INCLUDE', 'MOLWT', 'NHC', 'NOCHK', 'OIL', 'TRANSITION',
+                        'TRANS_OPTIMIZATION' + 'TRANS_TEST', 'OMEGAA', 'OMEGAB', 'PC', 'PR', 'PRES', 'PROPS',
+                        'PSAT', 'RS', 'RSSAT', 'RV', 'SATURATED', 'SPECG', 'TC', 'TEMP', 'UNSATGAS', 'UNSATOIL',
+                        'VG', 'VGFAC', 'VO', 'VOFAC', 'VSHIFT', 'ZC']
+PVT_KEYWORDS = PVT_TYPE_KEYWORDS + PVT_BLACKOIL_PRIMARY_KEYWORDS + PVT_EOS_METHODS + PVT_EOSOPTIONS_PRIMARY_WORDS + \
+               PVT_EOSOPTIONS_PRIMARY_KEYS_FLOAT + PVT_EOSOPTIONS_PRIMARY_KEYS_INT + PVT_EOSOPTIONS_TRANS_KEYS + \
+               PVT_ALL_TABLE_KEYWORDS + \
+               PVT_EOSOPTIONS_TRANS_TEST_KEYS + PVT_EOSOPTIONS_PHASEID_KEYS + PVT_EOSOPTIONS_TERTIARY_KEYS + \
+               PVT_GENERAL_KEYWORDS
```

### Comparing `ressimpy-1.0.0/ResSimpy/Nexus/NexusKeywords/relpm_keywords.py` & `ressimpy-1.0.1/ResSimpy/Nexus/NexusKeywords/relpm_keywords.py`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-# Currently ignoring functional form rel perm inputs, only tabular keywords are handled.
-# Also currently ignoring spline options
-
-RELPM_TABLE_KEYWORDS = ['WOTABLE', 'GOTABLE', 'GWTABLE', 'WOTABLE_IMB', 'GOTABLE_IMB', 'GWTABLE_IMB',
-                        'WAGTABLE_WIMB', 'GRMTABLE_SGTR', 'GRMTABLE', 'GDWTABLE', 'LOW_SALTAB',
-                        'PRSTAB', 'WAGTEST']
-RELPM_SINGLE_KEYWORDS = ['KROINT', 'STONE2', 'STONE1', 'SOMOPT1', 'SOMOPT3', 'LOW_SAL', 'GW3PHASE',
-                         'NOCHK', 'VIP_INJ_PERF_KR_SCALING', 'VEGO', 'VEGO_PC', 'VEWO', 'VEWO_PC',
-                         'IRELPM_LOWIFT', 'KRWINT', 'STONE2_WAT', 'STONE1_WAT', 'SWMOPT1',
-                         'FREEZE_PCGO', 'FREEZE_PCWO', 'FREEZE_PCGW', 'LOW_SAL_IRR', 'VIP_RELPM']
-RELPM_HYSTERESIS_PRIMARY_KEYWORDS = ['NONE', 'KRW', 'KRG', 'KROW', 'PCWO', 'PCGO', 'WAG',
-                                     'TOLREV', 'TOLHYS', 'NOCHK_HYS']
-RELPM_KEYWORDS_VALUE_FLOAT = ['SOMOPT2', 'ST1EXP', 'ST1EPS', 'ST1NU', 'GRMDSW', 'PERMBASIS', 'PORBASIS', 'DRELPM',
-                              'TENTHR', 'XEX', 'TENI', 'SWMOPT2']
-RELPM_KEYWORDS_VALUE_STR = ['HYSTERESIS', 'JFUNC', 'SCALING', 'SCALING_PC', 'IFT', 'NEARCRIT', 'DERIVATIVES',
-                            'RECONSTRUCT']
-RELPM_NONDARCY_KEYWORDS = ['NONDARCY_GAS', 'NONDARCY_OIL']
-RELPM_NONDARCY_PARAMS = ['BETA', 'BETA0', 'BETA1', 'BETA2', 'BETA3', 'BETA4', 'BETA5', 'IFT_THRES']
-
-RELPM_KEYWORDS = RELPM_TABLE_KEYWORDS + RELPM_SINGLE_KEYWORDS + RELPM_KEYWORDS_VALUE_FLOAT + \
-                 RELPM_KEYWORDS_VALUE_STR + RELPM_NONDARCY_KEYWORDS
+# Currently ignoring functional form rel perm inputs, only tabular keywords are handled.
+# Also currently ignoring spline options
+
+RELPM_TABLE_KEYWORDS = ['WOTABLE', 'GOTABLE', 'GWTABLE', 'WOTABLE_IMB', 'GOTABLE_IMB', 'GWTABLE_IMB',
+                        'WAGTABLE_WIMB', 'GRMTABLE_SGTR', 'GRMTABLE', 'GDWTABLE', 'LOW_SALTAB',
+                        'PRSTAB', 'WAGTEST']
+RELPM_SINGLE_KEYWORDS = ['KROINT', 'STONE2', 'STONE1', 'SOMOPT1', 'SOMOPT3', 'LOW_SAL', 'GW3PHASE',
+                         'NOCHK', 'VIP_INJ_PERF_KR_SCALING', 'VEGO', 'VEGO_PC', 'VEWO', 'VEWO_PC',
+                         'IRELPM_LOWIFT', 'KRWINT', 'STONE2_WAT', 'STONE1_WAT', 'SWMOPT1',
+                         'FREEZE_PCGO', 'FREEZE_PCWO', 'FREEZE_PCGW', 'LOW_SAL_IRR', 'VIP_RELPM']
+RELPM_HYSTERESIS_PRIMARY_KEYWORDS = ['NONE', 'KRW', 'KRG', 'KROW', 'PCWO', 'PCGO', 'WAG',
+                                     'TOLREV', 'TOLHYS', 'NOCHK_HYS']
+RELPM_KEYWORDS_VALUE_FLOAT = ['SOMOPT2', 'ST1EXP', 'ST1EPS', 'ST1NU', 'GRMDSW', 'PERMBASIS', 'PORBASIS', 'DRELPM',
+                              'TENTHR', 'XEX', 'TENI', 'SWMOPT2']
+RELPM_KEYWORDS_VALUE_STR = ['HYSTERESIS', 'JFUNC', 'SCALING', 'SCALING_PC', 'IFT', 'NEARCRIT', 'DERIVATIVES',
+                            'RECONSTRUCT']
+RELPM_NONDARCY_KEYWORDS = ['NONDARCY_GAS', 'NONDARCY_OIL']
+RELPM_NONDARCY_PARAMS = ['BETA', 'BETA0', 'BETA1', 'BETA2', 'BETA3', 'BETA4', 'BETA5', 'IFT_THRES']
+
+RELPM_KEYWORDS = RELPM_TABLE_KEYWORDS + RELPM_SINGLE_KEYWORDS + RELPM_KEYWORDS_VALUE_FLOAT + \
+                 RELPM_KEYWORDS_VALUE_STR + RELPM_NONDARCY_KEYWORDS
```

### Comparing `ressimpy-1.0.0/ResSimpy/Nexus/NexusKeywords/rock_keywords.py` & `ressimpy-1.0.1/ResSimpy/Nexus/NexusKeywords/rock_keywords.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-
-ROCK_KEYWORDS_VALUE_FLOAT = ['CR', 'KP', 'PREF', 'TOLREV_P', 'TOLREV_SW', 'CR_REPRESSURE', 'KP_REPRESSURE',
-                             'DPMIN', 'CREEPB', 'CREEPC', 'CREEPM']
-ROCK_KEYWORDS_VALUE_STR = ['REVERSIBLE', 'IRREVERSIBLE']
-ROCK_REV_IRREV_OPTIONS = ['ALL', 'CMTONLY', 'WIRCTONLY']
-ROCK_SINGLE_KEYWORDS = ['COMPR', 'KPMULT', 'CREEP', 'TAMULTONLY']
-ROCK_CMT = ['CMT']
-ROCK_WATER_INDUCED_CMT = ['WIRCT', 'SWINIT']
-ROCK_ALL_TABLE_KEYWORDS = ROCK_CMT + ROCK_WATER_INDUCED_CMT
-
-# Apparent Permeability in Nano-porosity Rocks (Knudsen diffusion/slippage) options
-ROCK_KNUDSEN_DIFF_KEYWORDS = ['JAVADPOUR', 'CIVAN', 'KNUDSEN']
-ROCK_KNUDSEN_DIFF_OPTIONS = ['R', 'ALPHA', 'BETA', 'A', 'B']
-
-ROCK_KEYWORDS = ROCK_KEYWORDS_VALUE_FLOAT + ROCK_KEYWORDS_VALUE_STR + ROCK_SINGLE_KEYWORDS + \
-    ROCK_ALL_TABLE_KEYWORDS + ROCK_REV_IRREV_OPTIONS + ROCK_KNUDSEN_DIFF_KEYWORDS + ROCK_KNUDSEN_DIFF_OPTIONS
+
+ROCK_KEYWORDS_VALUE_FLOAT = ['CR', 'KP', 'PREF', 'TOLREV_P', 'TOLREV_SW', 'CR_REPRESSURE', 'KP_REPRESSURE',
+                             'DPMIN', 'CREEPB', 'CREEPC', 'CREEPM']
+ROCK_KEYWORDS_VALUE_STR = ['REVERSIBLE', 'IRREVERSIBLE']
+ROCK_REV_IRREV_OPTIONS = ['ALL', 'CMTONLY', 'WIRCTONLY']
+ROCK_SINGLE_KEYWORDS = ['COMPR', 'KPMULT', 'CREEP', 'TAMULTONLY']
+ROCK_CMT = ['CMT']
+ROCK_WATER_INDUCED_CMT = ['WIRCT', 'SWINIT']
+ROCK_ALL_TABLE_KEYWORDS = ROCK_CMT + ROCK_WATER_INDUCED_CMT
+
+# Apparent Permeability in Nano-porosity Rocks (Knudsen diffusion/slippage) options
+ROCK_KNUDSEN_DIFF_KEYWORDS = ['JAVADPOUR', 'CIVAN', 'KNUDSEN']
+ROCK_KNUDSEN_DIFF_OPTIONS = ['R', 'ALPHA', 'BETA', 'A', 'B']
+
+ROCK_KEYWORDS = ROCK_KEYWORDS_VALUE_FLOAT + ROCK_KEYWORDS_VALUE_STR + ROCK_SINGLE_KEYWORDS + \
+    ROCK_ALL_TABLE_KEYWORDS + ROCK_REV_IRREV_OPTIONS + ROCK_KNUDSEN_DIFF_KEYWORDS + ROCK_KNUDSEN_DIFF_OPTIONS
```

### Comparing `ressimpy-1.0.0/ResSimpy/Nexus/NexusKeywords/runcontrol_keywords.py` & `ressimpy-1.0.1/ResSimpy/Nexus/NexusKeywords/runcontrol_keywords.py`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-# TODO: Not a complete list. Check manual for missing keywords.
-# TODO: Delete the keywords that are not tokens (i.e. that are only values in a table)
-
-RUNCONTROL_KEYWORDS = ['2PHASE', 'ADJUSTTOTIME', 'ALL', 'ALLOW', 'AQFLUX', 'ARRAYS', 'AUTO', 'AVGSG', 'AVGSO', 'AVGSW',
-                       'BG', 'BHP', 'BOF', 'CGFLUX', 'CGI', 'CGLG', 'CGP', 'CLP', 'COFLUX', 'COMP', 'CONCENTRATION',
-                       'CONNECTFILE', 'COP', 'CPR_PRESSURE_EQUATION', 'CRGI', 'CRGP', 'CROP', 'CRWI', 'CRWP', 'CWFLUX',
-                       'CWI', 'CWP', 'DATE', 'DATEFORMAT', 'DCMAX', 'DD/MM/YYYY', 'DEBUG', 'DEN', 'DEPTHTAB',
-                       'DISALLOW', 'DRDN', 'DRMX', 'DRSDT', 'DSGLIM', 'DSLIM', 'DT', 'DUAL_SOLVER', 'DVOLLIM', 'DZLIM',
-                       'END', 'ENDDEBUG', 'ENDGRIDS', 'ENDMAPOUT', 'ENDOUTPUT', 'ENDOUTSTART', 'ENDPLOTOUT',
-                       'ENDPOINTS', 'ENDREGIONOUT', 'ENDSPREADSHEET', 'ENDSSOUT', 'EQUILREGION', 'EXTENDED',
-                       'FACILITIES', 'FIELD', 'FIELDPLOT', 'FREEGAS', 'FREQ', 'FULLMAPARRAYS', 'GAS', 'GLOBALTOL',
-                       'GOR', 'GRIDS', 'GRIDSOLVER', 'HYDMAX', 'HYDRAULICS', 'ILU', 'IMPES', 'IMPES_COUPLING',
-                       'IMPLICIT', 'IMPLICITMBAL', 'IMPLICIT_COUPLING', 'IMPLICIT_PRECON', 'IMPSTAB', 'INPLACE',
-                       'ITERATIONS', 'KMCMT', 'KR', 'LIMIT', 'LOGOUT', 'MAPBINARY', 'MAPFORM', 'MAPOUT', 'MAPS',
-                       'MAPVDB', 'MASS', 'MAX', 'MAXBADNETS', 'MAXINCREASE', 'MAXNEWTONS', 'METHOD', 'MIN', 'MOB',
-                       'MONTHLY', 'NAME', 'NETPLOT', 'NETSUM', 'NETWORK', 'NOCPUOUT', 'NOCUT', 'NONE', 'NORECOUT',
-                       'NSC', 'OFF', 'OIL', 'ON', 'ORDER2009', 'OREC', 'OUTPUT', 'OUTSTART', 'OVERSHOOT', 'P', 'PAVH',
-                       'PAVT', 'PC', 'PCELL', 'PDATUMHC', 'PDATUMT', 'PDCOR', 'PERF', 'PERFPLOT', 'PERFREV', 'PERFS',
-                       'PERFTRACER', 'PI', 'PIN', 'PLOTBINARY', 'PLOTFORM', 'PLOTOUT', 'PLOTVDB', 'PMAX', 'PMIN',
-                       'PNODE', 'POUT', 'PSAT', 'PV', 'PVMLT', 'QGI', 'QGLG', 'QGP', 'QLP', 'QMAXINJ', 'QMAXPROD',
-                       'QOP', 'QUARTERLY', 'QWI', 'QWP', 'REGIONOUT', 'REGIONPLOT', 'REGIONS', 'RESERVOIR', 'RESTART',
-                       'RFT', 'RFTFILE', 'RGI', 'RGP', 'ROCK', 'ROP', 'RS', 'RVG', 'RVO', 'RVPVH', 'RVPVT', 'RVW',
-                       'RWI', 'RWP', 'SAL', 'SAT', 'SEPARATOR', 'SOLVER', 'SPREADSHEET', 'SSCSV', 'SSNOSORT', 'SSOUT',
-                       'SSTAB', 'START', 'STAT', 'STGIP', 'STOIP', 'STOP', 'STREAMCALC', 'STWIP', 'SW', 'TARGETPLOT',
-                       'TARGETS', 'TC', 'THP', 'TIME', 'TIMES', 'TNEXT', 'TOLS', 'TOTAL', 'TRANS', 'TSNUM', 'VIPUNITS',
-                       'VISC', 'VOLCON', 'WATER', 'WCUT', 'WELL', 'WELLPLOT', 'WELLS', 'WOR', 'WPAVE', 'WPPV', 'WPWBC',
-                       'X', 'Y', 'YEARLY', 'Z']
+# TODO: Not a complete list. Check manual for missing keywords.
+# TODO: Delete the keywords that are not tokens (i.e. that are only values in a table)
+
+RUNCONTROL_KEYWORDS = ['2PHASE', 'ADJUSTTOTIME', 'ALL', 'ALLOW', 'AQFLUX', 'ARRAYS', 'AUTO', 'AVGSG', 'AVGSO', 'AVGSW',
+                       'BG', 'BHP', 'BOF', 'CGFLUX', 'CGI', 'CGLG', 'CGP', 'CLP', 'COFLUX', 'COMP', 'CONCENTRATION',
+                       'CONNECTFILE', 'COP', 'CPR_PRESSURE_EQUATION', 'CRGI', 'CRGP', 'CROP', 'CRWI', 'CRWP', 'CWFLUX',
+                       'CWI', 'CWP', 'DATE', 'DATEFORMAT', 'DCMAX', 'DD/MM/YYYY', 'DEBUG', 'DEN', 'DEPTHTAB',
+                       'DISALLOW', 'DRDN', 'DRMX', 'DRSDT', 'DSGLIM', 'DSLIM', 'DT', 'DUAL_SOLVER', 'DVOLLIM', 'DZLIM',
+                       'END', 'ENDDEBUG', 'ENDGRIDS', 'ENDMAPOUT', 'ENDOUTPUT', 'ENDOUTSTART', 'ENDPLOTOUT',
+                       'ENDPOINTS', 'ENDREGIONOUT', 'ENDSPREADSHEET', 'ENDSSOUT', 'EQUILREGION', 'EXTENDED',
+                       'FACILITIES', 'FIELD', 'FIELDPLOT', 'FREEGAS', 'FREQ', 'FULLMAPARRAYS', 'GAS', 'GLOBALTOL',
+                       'GOR', 'GRIDS', 'GRIDSOLVER', 'HYDMAX', 'HYDRAULICS', 'ILU', 'IMPES', 'IMPES_COUPLING',
+                       'IMPLICIT', 'IMPLICITMBAL', 'IMPLICIT_COUPLING', 'IMPLICIT_PRECON', 'IMPSTAB', 'INPLACE',
+                       'ITERATIONS', 'KMCMT', 'KR', 'LIMIT', 'LOGOUT', 'MAPBINARY', 'MAPFORM', 'MAPOUT', 'MAPS',
+                       'MAPVDB', 'MASS', 'MAX', 'MAXBADNETS', 'MAXINCREASE', 'MAXNEWTONS', 'METHOD', 'MIN', 'MOB',
+                       'MONTHLY', 'NAME', 'NETPLOT', 'NETSUM', 'NETWORK', 'NOCPUOUT', 'NOCUT', 'NONE', 'NORECOUT',
+                       'NSC', 'OFF', 'OIL', 'ON', 'ORDER2009', 'OREC', 'OUTPUT', 'OUTSTART', 'OVERSHOOT', 'P', 'PAVH',
+                       'PAVT', 'PC', 'PCELL', 'PDATUMHC', 'PDATUMT', 'PDCOR', 'PERF', 'PERFPLOT', 'PERFREV', 'PERFS',
+                       'PERFTRACER', 'PI', 'PIN', 'PLOTBINARY', 'PLOTFORM', 'PLOTOUT', 'PLOTVDB', 'PMAX', 'PMIN',
+                       'PNODE', 'POUT', 'PSAT', 'PV', 'PVMLT', 'QGI', 'QGLG', 'QGP', 'QLP', 'QMAXINJ', 'QMAXPROD',
+                       'QOP', 'QUARTERLY', 'QWI', 'QWP', 'REGIONOUT', 'REGIONPLOT', 'REGIONS', 'RESERVOIR', 'RESTART',
+                       'RFT', 'RFTFILE', 'RGI', 'RGP', 'ROCK', 'ROP', 'RS', 'RVG', 'RVO', 'RVPVH', 'RVPVT', 'RVW',
+                       'RWI', 'RWP', 'SAL', 'SAT', 'SEPARATOR', 'SOLVER', 'SPREADSHEET', 'SSCSV', 'SSNOSORT', 'SSOUT',
+                       'SSTAB', 'START', 'STAT', 'STGIP', 'STOIP', 'STOP', 'STREAMCALC', 'STWIP', 'SW', 'TARGETPLOT',
+                       'TARGETS', 'TC', 'THP', 'TIME', 'TIMES', 'TNEXT', 'TOLS', 'TOTAL', 'TRANS', 'TSNUM', 'VIPUNITS',
+                       'VISC', 'VOLCON', 'WATER', 'WCUT', 'WELL', 'WELLPLOT', 'WELLS', 'WOR', 'WPAVE', 'WPPV', 'WPWBC',
+                       'X', 'Y', 'YEARLY', 'Z']
```

### Comparing `ressimpy-1.0.0/ResSimpy/Nexus/NexusKeywords/separator_keywords.py` & `ressimpy-1.0.1/ResSimpy/Nexus/NexusKeywords/separator_keywords.py`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-# TODO: Not a complete list. Check manual for missing keywords.
-# TODO: Delete the keywords that are not tokens (i.e. that are only values in a table)
-
-EOS_SEPARATOR_KEYWORDS = ['STAGE', 'TEMP', 'PRES', 'METHOD', 'IDL1', 'IDL2', 'IDV1', 'IDV2', 'FDL1', 'FDV1', 'IGP',
-                          'WATERMETHOD']
-GAS_PLANT_KEYWORDS = ['KEYCPTLIST', 'GPTNUM', 'PRES_STD', 'TEMP_STD', 'EOSMETHOD', 'WATERMETHOD', 'RECFAC_TABLE'
-                      'ENDRECFAC_TABLE', 'KEYCPTMF']
-
-BLACKOIL_SEPARATOR_KEYWORDS = ['BOSEP', 'MWOIL', 'MWGAS', 'ZOIL', 'STAGE', 'KVOIL', 'KVGAS', 'IDL1', 'IDL2', 'IDV1',
-                               'IDV2', 'FDL1', 'FDV1']
-
-SEPARATOR_KEYS_INT = ['WATERMETHOD', 'EOSMETHOD', 'GPTNUM']
-
-SEPARATOR_KEYS_FLOAT = ['MWOIL', 'MWGAS', 'ZOIL', 'PRES_STD', 'TEMP_STD']
-
-SEPARATOR_KEYWORDS = EOS_SEPARATOR_KEYWORDS + GAS_PLANT_KEYWORDS + BLACKOIL_SEPARATOR_KEYWORDS
+# TODO: Not a complete list. Check manual for missing keywords.
+# TODO: Delete the keywords that are not tokens (i.e. that are only values in a table)
+
+EOS_SEPARATOR_KEYWORDS = ['STAGE', 'TEMP', 'PRES', 'METHOD', 'IDL1', 'IDL2', 'IDV1', 'IDV2', 'FDL1', 'FDV1', 'IGP',
+                          'WATERMETHOD']
+GAS_PLANT_KEYWORDS = ['KEYCPTLIST', 'GPTNUM', 'PRES_STD', 'TEMP_STD', 'EOSMETHOD', 'WATERMETHOD', 'RECFAC_TABLE'
+                      'ENDRECFAC_TABLE', 'KEYCPTMF']
+
+BLACKOIL_SEPARATOR_KEYWORDS = ['BOSEP', 'MWOIL', 'MWGAS', 'ZOIL', 'STAGE', 'KVOIL', 'KVGAS', 'IDL1', 'IDL2', 'IDV1',
+                               'IDV2', 'FDL1', 'FDV1']
+
+SEPARATOR_KEYS_INT = ['WATERMETHOD', 'EOSMETHOD', 'GPTNUM']
+
+SEPARATOR_KEYS_FLOAT = ['MWOIL', 'MWGAS', 'ZOIL', 'PRES_STD', 'TEMP_STD']
+
+SEPARATOR_KEYWORDS = EOS_SEPARATOR_KEYWORDS + GAS_PLANT_KEYWORDS + BLACKOIL_SEPARATOR_KEYWORDS
```

### Comparing `ressimpy-1.0.0/ResSimpy/Nexus/NexusKeywords/structured_grid_keywords.py` & `ressimpy-1.0.1/ResSimpy/Nexus/NexusKeywords/structured_grid_keywords.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-# TODO: Not a complete list. Check manual for missing keywords.
-# TODO: Delete the keywords that are not tokens (i.e. that are only values in a table)
-
-INTEGER_ARRAYS = ['ICOARS', 'IEQUIL', 'IPVT', 'IWATER', 'IALPHAF', 'IPOLYMER', 'IRELPM', 'IROCK', 'IREGION',
-                  'IADSORPTION', 'ITRAN', 'ITRACER', 'DEADCELL', 'LIVECELL', 'IGRID', 'ISECTOR']
-
-WORK_ARRAYS = ['WORKA1', 'WORKA2', 'WORKA3', 'WORKA4', 'WORKA5', 'WORKA6', 'WORKA7', 'WORKA8', 'WORKA9']
-
-ROCK_ARRAYS = ['SWL', 'SWR', 'SGL', 'SGR', 'SWRO', 'SWRO_LS', 'SGRO', 'SGRW', 'KRW_SWRO', 'KRWS_LS', 'KRW_SWU',
-               'KRG_SGRO', 'KRG_SGU', 'KRO_SWL', 'KRO_SGL', 'KRO_SGR', 'KRW_SGL', 'KRW_SGR', 'KRG_SGRW', 'SGTR',
-               'SOTR', 'SWLPC', 'SGLPC', 'PCW_SWL', 'PCG_SGU']
-
-USER_INIT_ARRAYS = ['SW', 'SG', 'PRESSURE', 'TEMPERATURE', 'CHLORIDE', 'CALCIUM', 'SALINITY', 'API',
-                    'WORKA1', 'WORKA2', 'WORKA3', 'WORKA4', 'WORKA5', 'WORKA6', 'WORKA7', 'WORKA8', 'WORKA9']
-
-MULTIPLIER_ARRAYS = ['TMX', 'TMY', 'TMZ', 'MULTBV']
-
-PROPERTY_ARRAYS = ['POROSITY', 'POR', 'POROSITY', 'PV', 'KX', 'KY', 'KZ', 'COMPR', 'CR', 'NETGRS', 'KWX',
-                   'KWY', 'KWZ', 'PEMDMAT', 'PEMGMAT', 'PEMKMAT', 'BW_SAL', 'BW_T']
-
-GRID_GEOMETRY_ARRAYS = ['CORP', 'EIGHT', 'DX', 'DY', 'DZ', 'DXB', 'DYB', 'DZB', 'MDEPTH', 'DEPTH', 'DBZNET']
-
-GRID_OPERATION_KEYWORDS = ['ADD', 'SUB', 'DIV', 'MULT', 'EQ']
-
-GRID_ARRAY_FORMAT_KEYWORDS = ['VALUE', 'XVAR', 'YVAR', 'ZVAR']
-
-GRID_ARRAY_KEYWORDS = INTEGER_ARRAYS + WORK_ARRAYS + ROCK_ARRAYS + USER_INIT_ARRAYS + MULTIPLIER_ARRAYS + \
-                      PROPERTY_ARRAYS + GRID_GEOMETRY_ARRAYS
-
-STRUCTURED_GRID_KEYWORDS = ['ADD', 'ALL', 'ANALYT', 'ARRAYS', 'B', 'BLOCKS', 'C', 'CARTREF', 'COARSEN', 'COMPR', 'CON',
-                            'CONCENTRATION', 'CORNER', 'CORP', 'CORTOL', 'DEADCELL', 'DECOMP', 'DEPTH', 'DIP', 'DIV',
-                            'DX', 'DY', 'DZ', 'END', 'ENDAQ', 'ENDDEC', 'ENDREF', 'EXP', 'FNAME', 'FRAC', 'FTRANS',
-                            'FUNCTION', 'GE', 'GRID', 'ID', 'IEQUIL', 'IINF', 'INCLUDE', 'INFLUX', 'IPVT', 'IREGION',
-                            'IRELPM', 'IROCK', 'ITRAN', 'IWATER', 'JINF', 'KINF', 'KRG_SGRW', 'KRO_SWL', 'KRW_SWRO',
-                            'KRW_SWU', 'KX', 'KXEFF', 'KY', 'KYEFF', 'KZ', 'KZEFF', 'LAYER', 'LE', 'LGR', 'LIVECELL',
-                            'LX', 'LY', 'LZ', 'MAPBINARY', 'MAPOUT', 'MAPVDB', 'MDEPTH', 'MIN', 'MINUS', 'MOD', 'MODX',
-                            'MODY', 'MODZ', 'MULT', 'MULTBV', 'MULTFL', 'MULTIR', 'NETGRS', 'NEWTRAN', 'NOLIST', 'NONE',
-                            'NONSTD', 'NX', 'NY', 'NZ', 'OMIT', 'OUTPUT', 'OVER', 'PINCHOUT', 'POR', 'POROSITY',
-                            'PRINT', 'PV', 'PVMULT', 'RANGE', 'RIGHTHANDED', 'ROOT', 'SALINITY', 'SG', 'SGL', 'SGR',
-                            'SGRO', 'SGRW', 'SGU', 'SINF', 'STD', 'SW', 'SWL', 'SWR', 'SWRO', 'SWRO_LS', 'SWU', 'TMX',
-                            'TMY', 'TMZ', 'TOLPV', 'TX', 'TY', 'TZ', 'V98', 'VALUE', 'WATER', 'WINDOW', 'WORKA1', 'X',
-                            'XREG', 'Z', 'ZVAR']
+# TODO: Not a complete list. Check manual for missing keywords.
+# TODO: Delete the keywords that are not tokens (i.e. that are only values in a table)
+
+INTEGER_ARRAYS = ['ICOARS', 'IEQUIL', 'IPVT', 'IWATER', 'IALPHAF', 'IPOLYMER', 'IRELPM', 'IROCK', 'IREGION',
+                  'IADSORPTION', 'ITRAN', 'ITRACER', 'DEADCELL', 'LIVECELL', 'IGRID', 'ISECTOR']
+
+WORK_ARRAYS = ['WORKA1', 'WORKA2', 'WORKA3', 'WORKA4', 'WORKA5', 'WORKA6', 'WORKA7', 'WORKA8', 'WORKA9']
+
+ROCK_ARRAYS = ['SWL', 'SWR', 'SGL', 'SGR', 'SWRO', 'SWRO_LS', 'SGRO', 'SGRW', 'KRW_SWRO', 'KRWS_LS', 'KRW_SWU',
+               'KRG_SGRO', 'KRG_SGU', 'KRO_SWL', 'KRO_SGL', 'KRO_SGR', 'KRW_SGL', 'KRW_SGR', 'KRG_SGRW', 'SGTR',
+               'SOTR', 'SWLPC', 'SGLPC', 'PCW_SWL', 'PCG_SGU']
+
+USER_INIT_ARRAYS = ['SW', 'SG', 'PRESSURE', 'TEMPERATURE', 'CHLORIDE', 'CALCIUM', 'SALINITY', 'API',
+                    'WORKA1', 'WORKA2', 'WORKA3', 'WORKA4', 'WORKA5', 'WORKA6', 'WORKA7', 'WORKA8', 'WORKA9']
+
+MULTIPLIER_ARRAYS = ['TMX', 'TMY', 'TMZ', 'MULTBV']
+
+PROPERTY_ARRAYS = ['POROSITY', 'POR', 'POROSITY', 'PV', 'KX', 'KY', 'KZ', 'COMPR', 'CR', 'NETGRS', 'KWX',
+                   'KWY', 'KWZ', 'PEMDMAT', 'PEMGMAT', 'PEMKMAT', 'BW_SAL', 'BW_T']
+
+GRID_GEOMETRY_ARRAYS = ['CORP', 'EIGHT', 'DX', 'DY', 'DZ', 'DXB', 'DYB', 'DZB', 'MDEPTH', 'DEPTH', 'DBZNET']
+
+GRID_OPERATION_KEYWORDS = ['ADD', 'SUB', 'DIV', 'MULT', 'EQ']
+
+GRID_ARRAY_FORMAT_KEYWORDS = ['VALUE', 'XVAR', 'YVAR', 'ZVAR']
+
+GRID_ARRAY_KEYWORDS = INTEGER_ARRAYS + WORK_ARRAYS + ROCK_ARRAYS + USER_INIT_ARRAYS + MULTIPLIER_ARRAYS + \
+                      PROPERTY_ARRAYS + GRID_GEOMETRY_ARRAYS
+
+STRUCTURED_GRID_KEYWORDS = ['ADD', 'ALL', 'ANALYT', 'ARRAYS', 'B', 'BLOCKS', 'C', 'CARTREF', 'COARSEN', 'COMPR', 'CON',
+                            'CONCENTRATION', 'CORNER', 'CORP', 'CORTOL', 'DEADCELL', 'DECOMP', 'DEPTH', 'DIP', 'DIV',
+                            'DX', 'DY', 'DZ', 'END', 'ENDAQ', 'ENDDEC', 'ENDREF', 'EXP', 'FNAME', 'FRAC', 'FTRANS',
+                            'FUNCTION', 'GE', 'GRID', 'ID', 'IEQUIL', 'IINF', 'INCLUDE', 'INFLUX', 'IPVT', 'IREGION',
+                            'IRELPM', 'IROCK', 'ITRAN', 'IWATER', 'JINF', 'KINF', 'KRG_SGRW', 'KRO_SWL', 'KRW_SWRO',
+                            'KRW_SWU', 'KX', 'KXEFF', 'KY', 'KYEFF', 'KZ', 'KZEFF', 'LAYER', 'LE', 'LGR', 'LIVECELL',
+                            'LX', 'LY', 'LZ', 'MAPBINARY', 'MAPOUT', 'MAPVDB', 'MDEPTH', 'MIN', 'MINUS', 'MOD', 'MODX',
+                            'MODY', 'MODZ', 'MULT', 'MULTBV', 'MULTFL', 'MULTIR', 'NETGRS', 'NEWTRAN', 'NOLIST', 'NONE',
+                            'NONSTD', 'NX', 'NY', 'NZ', 'OMIT', 'OUTPUT', 'OVER', 'PINCHOUT', 'POR', 'POROSITY',
+                            'PRINT', 'PV', 'PVMULT', 'RANGE', 'RIGHTHANDED', 'ROOT', 'SALINITY', 'SG', 'SGL', 'SGR',
+                            'SGRO', 'SGRW', 'SGU', 'SINF', 'STD', 'SW', 'SWL', 'SWR', 'SWRO', 'SWRO_LS', 'SWU', 'TMX',
+                            'TMY', 'TMZ', 'TOLPV', 'TX', 'TY', 'TZ', 'V98', 'VALUE', 'WATER', 'WINDOW', 'WORKA1', 'X',
+                            'XREG', 'Z', 'ZVAR']
```

### Comparing `ressimpy-1.0.0/ResSimpy/Nexus/NexusKeywords/surface_keywords.py` & `ressimpy-1.0.1/ResSimpy/Nexus/NexusKeywords/surface_keywords.py`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-# TODO: Not a complete list. Check manual for missing keywords.
-# TODO: Delete the keywords that are not tokens (i.e. that are only values in a table)
-
-SURFACE_KEYWORDS = ['A', 'ACPGCR', 'ACTIONS', 'ACTIVATE', 'ACTIVE', 'ADD', 'ADDVALUE', 'ALL', 'ALL1D', 'ALLOW_BHMOVE',
-                    'ANGLE', 'API', 'ARRAYBOUNDS', 'AVG', 'B', 'BACKFLOW', 'BEGGS', 'BHCON', 'BHDEPTH', 'BHP',
-                    'BLACKOIL', 'C', 'CALC', 'CALCCOND', 'CALCCONS', 'CALCMETHOD', 'CALCMULT', 'CELLAVG', 'CELLGRAD',
-                    'CLEAR', 'CLEARP', 'CLEARQ', 'COMPONENT', 'COMPONENTS', 'CON', 'CONCENTRATION', 'CONDEFAULTS',
-                    'CONLIST', 'CONNECTION', 'CONSTRAINT', 'CONSTRAINTS', 'CONTEST', 'CONTROL', 'CONTYPE',
-                    'CORRELATION', 'CROSSFLOW', 'CROSS_SHUT', 'CTRL', 'CTRLCOND', 'CTRLCONS', 'CTRLMETHOD', 'CWLIM',
-                    'CYCLE', 'D', 'DAMP', 'DATA', 'DATGRAD', 'DATUM', 'DAY', 'DAYS', 'DDEPTH', 'DEACTIVATE', 'DEN_TEMP',
-                    'DEPTH', 'DIAM', 'DO', 'DONTCLEAR', 'DP', 'DPADD', 'DPBHAVG', 'DPBHMX', 'DPERF', 'DT', 'DTMIN',
-                    'DUNROS', 'E', 'ELEVPR', 'ELSE', 'ELSEIF', 'END', 'ENDACTIVATE', 'ENDCONDEFAULTS', 'ENDCONLIST',
-                    'ENDCONSTRAINTS', 'ENDCONTEST', 'ENDDEACTIVATE', 'ENDDO', 'ENDELEVPR', 'ENDGASWELLS',
-                    'ENDGUIDERATE', 'ENDIF', 'ENDNODECON', 'ENDNODELIST', 'ENDNODES', 'ENDPDCORR', 'ENDPROCS', 'ENDPT',
-                    'ENDQMULT', 'ENDSKIP', 'ENDSTREAMS', 'ENDSTREAM_TRACER', 'ENDTARGET', 'ENDTEMPGR', 'ENDTEMPPR',
-                    'ENDTGTCON', 'ENDWELLBORE', 'ENDWELLHEAD', 'ENDWELLLIST', 'ENDWELLS', 'EOS', 'ESP', 'EXIT', 'F',
-                    'FLOW_UNSTABLE', 'FREQ', 'FRPGCR', 'GAS', 'GASLIFT', 'GASMOB', 'GASWATER', 'GASWELLS', 'GLIFT',
-                    'GOR', 'GORLIM', 'GORPERF', 'GORQMULT', 'GORWELL', 'GRADCALC', 'GROUP_PERFS', 'GRPGCR', 'GUIDERATE',
-                    'HAGEDORN', 'HAG_BEG', 'HEATTR', 'HTC', 'HYDRAULICS', 'HYDSTAB', 'IBAT', 'ID', 'IF', 'INCLUDE',
-                    'INCREASE', 'INJMOB', 'INJTGTP', 'INJTGTPHC', 'INTEGER', 'INT_1D', 'IPVT', 'ITIME', 'IW', 'IWAT',
-                    'K', 'LENGTH', 'LEVEL', 'LIMIT', 'LOGICAL', 'LOGICAL_1D', 'LOOP', 'LUMPED', 'MAX', 'MAXOPEN',
-                    'MDIN', 'MDOUT', 'METHOD', 'MIXED', 'MOBGRAD', 'MONTH', 'MULT', 'MULTIFIELD', 'N', 'N1', 'N2',
-                    'NAME', 'NETFILL', 'NETTEMP', 'NETVOID', 'NEWTON', 'NHC', 'NODECON', 'NODEIN', 'NODELIST',
-                    'NODEOUT', 'NODES', 'NONE', 'NOONTIME', 'NOSLIP', 'NOTDATA', 'NOW', 'NUMBER', 'OFF', 'OIL',
-                    'OILGRAD', 'ON', 'ONTIME', 'OUTPAVG', 'PARENT', 'PATTERN', 'PC', 'PD', 'PDCORR', 'PHASE', 'PIPE',
-                    'PIPEGRAD', 'PLUS', 'PMAX', 'PMIN', 'PRIORITY', 'PROC', 'PROCABORT', 'PROCS', 'PRODTGTP',
-                    'PRODTGTPHC', 'PRODWELLS', 'QALL', 'QALLMAX', 'QALLRMAX', 'QG', 'QGAS', 'QGLFT', 'QGNETPROD',
-                    'QGSMAX', 'QGSMIN', 'QGUIDE', 'QLIQ', 'QLIQLFT', 'QLIQSMAX', 'QLIQSMIN', 'QMIN', 'QMIN_NOSHUT',
-                    'QMULT', 'QMULTOPT', 'QO', 'QOIL', 'QOLFT', 'QOMAX', 'QOSMAX', 'QOSMIN', 'QW', 'QWAT', 'QWATER',
-                    'QWLFT', 'QWMAX', 'QWSMAX', 'QWSMIN', 'RANKDT', 'RATE', 'REAL', 'REAL_1D', 'REGAVG', 'REGHCAVG',
-                    'REGION', 'REMOVE', 'RESERVOIR', 'RFTWELLS', 'ROUGHNESS', 'SCALE', 'SEQUENTIAL', 'SETTING',
-                    'SHCGAS', 'SHCOIL', 'SHCWAT', 'SHUTINON', 'SHUTIN_UNSTABLE', 'SINK', 'SKIP', 'SS_CONS', 'SS_NODES',
-                    'SS_PERFS', 'SS_WELLS', 'START', 'STATIC', 'STATION', 'STD', 'STREAM', 'STREAMS', 'STREAM_TRACER',
-                    'SURFACE', 'TARG', 'TARGET', 'TARGETS', 'TEMP', 'TEMPGR', 'TEMPPR', 'TEST', 'TGTCON', 'THEN',
-                    'TIME', 'TRACER', 'TRACERS', 'TSTPRF', 'TVD', 'TYPE', 'VALUE', 'W', 'WATER', 'WATERINJWELLS',
-                    'WCUT', 'WCUTMAX', 'WCUTPERF', 'WCUTPLUG', 'WELL', 'WELLBORE', 'WELLCONTROL', 'WELLDATUM',
-                    'WELLGRAD', 'WELLHEAD', 'WELLLIST', 'WELLS', 'WI', 'WIMULT', 'X', 'YEAR']
-
-CONNECTION_KEYWORDS = ['NAME', 'NODEIN', 'NODEOUT', 'IPVT', 'IWAT', 'IBAT', 'TYPE', 'METHOD', 'LENGTH', 'NUMBER',
-                       'DDEPTH', 'DIAM', 'INNERDIAM', 'ROUGHNESS', 'ELEVPR', 'TEMPPR', 'MDIN', 'MDOUT', 'HTC', 'DPADD',
-                       'RATEMULT', 'TEMPIN', 'TEMPOUT', 'TRACERS', 'POLYMER', 'DTADD', 'SEAWPR', 'THICKNESS', 'INSTHN',
-                       'INSK', 'GRPGCR', 'FRPGCR', 'ACPGCR',
-                       ]
+# TODO: Not a complete list. Check manual for missing keywords.
+# TODO: Delete the keywords that are not tokens (i.e. that are only values in a table)
+
+SURFACE_KEYWORDS = ['A', 'ACPGCR', 'ACTIONS', 'ACTIVATE', 'ACTIVE', 'ADD', 'ADDVALUE', 'ALL', 'ALL1D', 'ALLOW_BHMOVE',
+                    'ANGLE', 'API', 'ARRAYBOUNDS', 'AVG', 'B', 'BACKFLOW', 'BEGGS', 'BHCON', 'BHDEPTH', 'BHP',
+                    'BLACKOIL', 'C', 'CALC', 'CALCCOND', 'CALCCONS', 'CALCMETHOD', 'CALCMULT', 'CELLAVG', 'CELLGRAD',
+                    'CLEAR', 'CLEARP', 'CLEARQ', 'COMPONENT', 'COMPONENTS', 'CON', 'CONCENTRATION', 'CONDEFAULTS',
+                    'CONLIST', 'CONNECTION', 'CONSTRAINT', 'CONSTRAINTS', 'CONTEST', 'CONTROL', 'CONTYPE',
+                    'CORRELATION', 'CROSSFLOW', 'CROSS_SHUT', 'CTRL', 'CTRLCOND', 'CTRLCONS', 'CTRLMETHOD', 'CWLIM',
+                    'CYCLE', 'D', 'DAMP', 'DATA', 'DATGRAD', 'DATUM', 'DAY', 'DAYS', 'DDEPTH', 'DEACTIVATE', 'DEN_TEMP',
+                    'DEPTH', 'DIAM', 'DO', 'DONTCLEAR', 'DP', 'DPADD', 'DPBHAVG', 'DPBHMX', 'DPERF', 'DT', 'DTMIN',
+                    'DUNROS', 'E', 'ELEVPR', 'ELSE', 'ELSEIF', 'END', 'ENDACTIVATE', 'ENDCONDEFAULTS', 'ENDCONLIST',
+                    'ENDCONSTRAINTS', 'ENDCONTEST', 'ENDDEACTIVATE', 'ENDDO', 'ENDELEVPR', 'ENDGASWELLS',
+                    'ENDGUIDERATE', 'ENDIF', 'ENDNODECON', 'ENDNODELIST', 'ENDNODES', 'ENDPDCORR', 'ENDPROCS', 'ENDPT',
+                    'ENDQMULT', 'ENDSKIP', 'ENDSTREAMS', 'ENDSTREAM_TRACER', 'ENDTARGET', 'ENDTEMPGR', 'ENDTEMPPR',
+                    'ENDTGTCON', 'ENDWELLBORE', 'ENDWELLHEAD', 'ENDWELLLIST', 'ENDWELLS', 'EOS', 'ESP', 'EXIT', 'F',
+                    'FLOW_UNSTABLE', 'FREQ', 'FRPGCR', 'GAS', 'GASLIFT', 'GASMOB', 'GASWATER', 'GASWELLS', 'GLIFT',
+                    'GOR', 'GORLIM', 'GORPERF', 'GORQMULT', 'GORWELL', 'GRADCALC', 'GROUP_PERFS', 'GRPGCR', 'GUIDERATE',
+                    'HAGEDORN', 'HAG_BEG', 'HEATTR', 'HTC', 'HYDRAULICS', 'HYDSTAB', 'IBAT', 'ID', 'IF', 'INCLUDE',
+                    'INCREASE', 'INJMOB', 'INJTGTP', 'INJTGTPHC', 'INTEGER', 'INT_1D', 'IPVT', 'ITIME', 'IW', 'IWAT',
+                    'K', 'LENGTH', 'LEVEL', 'LIMIT', 'LOGICAL', 'LOGICAL_1D', 'LOOP', 'LUMPED', 'MAX', 'MAXOPEN',
+                    'MDIN', 'MDOUT', 'METHOD', 'MIXED', 'MOBGRAD', 'MONTH', 'MULT', 'MULTIFIELD', 'N', 'N1', 'N2',
+                    'NAME', 'NETFILL', 'NETTEMP', 'NETVOID', 'NEWTON', 'NHC', 'NODECON', 'NODEIN', 'NODELIST',
+                    'NODEOUT', 'NODES', 'NONE', 'NOONTIME', 'NOSLIP', 'NOTDATA', 'NOW', 'NUMBER', 'OFF', 'OIL',
+                    'OILGRAD', 'ON', 'ONTIME', 'OUTPAVG', 'PARENT', 'PATTERN', 'PC', 'PD', 'PDCORR', 'PHASE', 'PIPE',
+                    'PIPEGRAD', 'PLUS', 'PMAX', 'PMIN', 'PRIORITY', 'PROC', 'PROCABORT', 'PROCS', 'PRODTGTP',
+                    'PRODTGTPHC', 'PRODWELLS', 'QALL', 'QALLMAX', 'QALLRMAX', 'QG', 'QGAS', 'QGLFT', 'QGNETPROD',
+                    'QGSMAX', 'QGSMIN', 'QGUIDE', 'QLIQ', 'QLIQLFT', 'QLIQSMAX', 'QLIQSMIN', 'QMIN', 'QMIN_NOSHUT',
+                    'QMULT', 'QMULTOPT', 'QO', 'QOIL', 'QOLFT', 'QOMAX', 'QOSMAX', 'QOSMIN', 'QW', 'QWAT', 'QWATER',
+                    'QWLFT', 'QWMAX', 'QWSMAX', 'QWSMIN', 'RANKDT', 'RATE', 'REAL', 'REAL_1D', 'REGAVG', 'REGHCAVG',
+                    'REGION', 'REMOVE', 'RESERVOIR', 'RFTWELLS', 'ROUGHNESS', 'SCALE', 'SEQUENTIAL', 'SETTING',
+                    'SHCGAS', 'SHCOIL', 'SHCWAT', 'SHUTINON', 'SHUTIN_UNSTABLE', 'SINK', 'SKIP', 'SS_CONS', 'SS_NODES',
+                    'SS_PERFS', 'SS_WELLS', 'START', 'STATIC', 'STATION', 'STD', 'STREAM', 'STREAMS', 'STREAM_TRACER',
+                    'SURFACE', 'TARG', 'TARGET', 'TARGETS', 'TEMP', 'TEMPGR', 'TEMPPR', 'TEST', 'TGTCON', 'THEN',
+                    'TIME', 'TRACER', 'TRACERS', 'TSTPRF', 'TVD', 'TYPE', 'VALUE', 'W', 'WATER', 'WATERINJWELLS',
+                    'WCUT', 'WCUTMAX', 'WCUTPERF', 'WCUTPLUG', 'WELL', 'WELLBORE', 'WELLCONTROL', 'WELLDATUM',
+                    'WELLGRAD', 'WELLHEAD', 'WELLLIST', 'WELLS', 'WI', 'WIMULT', 'X', 'YEAR']
+
+CONNECTION_KEYWORDS = ['NAME', 'NODEIN', 'NODEOUT', 'IPVT', 'IWAT', 'IBAT', 'TYPE', 'METHOD', 'LENGTH', 'NUMBER',
+                       'DDEPTH', 'DIAM', 'INNERDIAM', 'ROUGHNESS', 'ELEVPR', 'TEMPPR', 'MDIN', 'MDOUT', 'HTC', 'DPADD',
+                       'RATEMULT', 'TEMPIN', 'TEMPOUT', 'TRACERS', 'POLYMER', 'DTADD', 'SEAWPR', 'THICKNESS', 'INSTHN',
+                       'INSK', 'GRPGCR', 'FRPGCR', 'ACPGCR',
+                       ]
```

### Comparing `ressimpy-1.0.0/ResSimpy/Nexus/NexusNetwork.py` & `ressimpy-1.0.1/ResSimpy/Nexus/NexusNetwork.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,185 +1,185 @@
-from __future__ import annotations
-from dataclasses import dataclass
-from typing import TYPE_CHECKING, Optional, Any, Literal
-
-from ResSimpy.Network import Network
-from ResSimpy.Nexus.nexus_collect_tables import collect_all_tables_to_objects
-from ResSimpy.Nexus.DataModels.Network.NexusConstraint import NexusConstraint
-from ResSimpy.Nexus.DataModels.Network.NexusConstraints import NexusConstraints
-from ResSimpy.Nexus.DataModels.Network.NexusNode import NexusNode
-from ResSimpy.Nexus.DataModels.Network.NexusNodeConnection import NexusNodeConnection
-from ResSimpy.Nexus.DataModels.Network.NexusNodeConnections import NexusNodeConnections
-from ResSimpy.Nexus.DataModels.Network.NexusNodes import NexusNodes
-from ResSimpy.Nexus.DataModels.Network.NexusWellConnection import NexusWellConnection
-from ResSimpy.Nexus.DataModels.Network.NexusWellConnections import NexusWellConnections
-from ResSimpy.Nexus.DataModels.Network.NexusWellbore import NexusWellbore
-from ResSimpy.Nexus.DataModels.Network.NexusWellbores import NexusWellbores
-from ResSimpy.Nexus.DataModels.Network.NexusWellhead import NexusWellhead
-from ResSimpy.Nexus.DataModels.Network.NexusWellheads import NexusWellheads
-from ResSimpy.Nexus.DataModels.NexusFile import NexusFile
-
-if TYPE_CHECKING:
-    from ResSimpy.Nexus.NexusSimulator import NexusSimulator
-
-
-@dataclass(kw_only=True)
-class NexusNetwork(Network):
-    __model: NexusSimulator
-    nodes: NexusNodes
-    connections: NexusNodeConnections
-    well_connections: NexusWellConnections
-    wellheads: NexusWellheads
-    wellbores: NexusWellbores
-    constraints: NexusConstraints
-    __has_been_loaded: bool = False
-
-    def __init__(self, model: NexusSimulator) -> None:
-        self.__has_been_loaded: bool = False
-        self.__model: NexusSimulator = model
-        self.nodes: NexusNodes = NexusNodes(self)
-        self.connections: NexusNodeConnections = NexusNodeConnections(self)
-        self.well_connections: NexusWellConnections = NexusWellConnections(self)
-        self.wellheads: NexusWellheads = NexusWellheads(self)
-        self.wellbores: NexusWellbores = NexusWellbores(self)
-        self.constraints: NexusConstraints = NexusConstraints(self, model)
-
-    def get_load_status(self) -> bool:
-        """Checks load status and loads the network if it hasn't already been loaded."""
-        if not self.__has_been_loaded:
-            self.load()
-        return self.__has_been_loaded
-
-    @property
-    def model(self) -> NexusSimulator:
-        return self.__model
-
-    def get_network_file(self, method_number: int = 1) -> NexusFile:
-        """Gets a specific network file object from the method number.
-
-        Args:
-        ----
-            method_number (int): Method number for selection of a specific surface file.
-                If None then returns a dictionary of method, surface file object
-
-        Returns:
-        -------
-            NexusFile: returns a specific surface file object of surface files keyed by method number
-        """
-        if self.__model.model_files.surface_files is None:
-            raise ValueError('No files found for the surface network')
-        network_file = self.__model.model_files.surface_files.get(method_number, None)
-        if network_file is None:
-            raise ValueError(f'No file found for {method_number=}, instead found {network_file=}')
-        return network_file
-
-    def load(self) -> None:
-        """Loads all the objects from the surface files in the Simulator class.
-        Table headers with None next to their name are currently skipped awaiting development.
-        """
-
-        def type_check_lists(input: Optional[list[Any] | dict[str, list[NexusConstraint]]]) -> Optional[list[Any]]:
-            """Guards against dictionaries coming from the dictionary."""
-            if isinstance(input, dict):
-                raise TypeError(f"Expected a list, instead received a dict: {input}")
-            return input
-
-        def type_check_dicts(input: Optional[list[Any] | dict[str, list[NexusConstraint]]]) -> \
-                Optional[dict[str, list[NexusConstraint]]]:
-            """Guards against dictionaries coming from the dictionary."""
-            if isinstance(input, list):
-                raise TypeError(f"Expected a dict, instead received a list: {input}")
-            return input
-
-        # TODO implement all objects with Nones next to them in the dictionary below
-        if self.__model.model_files.surface_files is None:
-            raise FileNotFoundError('Could not find any surface files associated with the fcs file provided.')
-
-        for surface in self.__model.model_files.surface_files.values():
-            nexus_obj_dict = collect_all_tables_to_objects(
-                surface, {'NODECON': NexusNodeConnection,
-                          'NODES': NexusNode,
-                          'WELLS': NexusWellConnection,
-                          'WELLHEAD': NexusWellhead,
-                          'WELLBORE': NexusWellbore,
-                          'CONSTRAINTS': NexusConstraint,
-                          'CONSTRAINT': NexusConstraint,
-                          'QMULT': NexusConstraint,
-                          'CONDEFAULTS': None,
-                          'TARGET': None,
-                          },
-                start_date=self.__model.start_date,
-                default_units=self.__model.default_units,
-                )
-            self.nodes._add_to_memory(type_check_lists(nexus_obj_dict.get('NODES')))
-            self.connections._add_to_memory(type_check_lists(nexus_obj_dict.get('NODECON')))
-            self.well_connections._add_to_memory(type_check_lists(nexus_obj_dict.get('WELLS')))
-            self.wellheads._add_to_memory(type_check_lists(nexus_obj_dict.get('WELLHEAD')))
-            self.wellbores._add_to_memory(type_check_lists(nexus_obj_dict.get('WELLBORE')))
-            self.constraints._add_to_memory(type_check_dicts(nexus_obj_dict.get('CONSTRAINTS')))
-
-        self.__has_been_loaded = True
-
-    def get_unique_names_in_network(self) -> list[str]:
-        """Extracts all names from a network including all the nodes, wells and connections.
-
-        Returns:
-            list[str]: list of all the unique names from the network including nodes, wells and connections
-
-        """
-        constraint_names_to_add = []
-        constraint_names_to_add.extend([x.name for x in self.nodes.get_all() if x.name is not None])
-        constraint_names_to_add.extend([x.name for x in self.well_connections.get_all()
-                                        if x.name is not None])
-        constraint_names_to_add.extend([x.name for x in self.connections.get_all() if x.name is not None])
-        constraint_names_to_add.extend([x.name for x in self.wellbores.get_all() if x.name is not None])
-        constraint_names_to_add.extend([x.name for x in self.wellheads.get_all() if x.name is not None])
-        constraint_names_to_add = list(set(constraint_names_to_add))
-
-        return constraint_names_to_add
-
-    def find_network_element_with_dict(self, name: str, search_dict: dict[str, None | float | str | int],
-                                       network_element_type: Literal['nodes', 'connections', 'well_connections',
-                                                                     'wellheads', 'wellbores', 'constraints']) -> Any:
-        """Finds a uniquely matching constraint from a given set of properties in a dictionary of attributes.
-
-        Args:
-            name (str): name of the node/connection to find
-            search_dict (dict[str, float | str | int]): dictionary of attributes to match on. \
-            Allows for partial matches if it finds a unique object.
-            network_element_type (Literal[str]): one of nodes, connections, well_connections, wellheads, wellbores,
-                constraints
-
-        Returns:
-            NexusConstraint of an existing constraint in the model that uniquely matches the provided \
-            constraint_dict constraint
-        """
-        network_element_to_search: Any = None
-        self.get_load_status()
-        if network_element_type == 'constraints':
-            network_element_to_search = self.constraints.get_all().get(name, None)
-        else:
-            # retrieve the getter method on the network attribute
-            network_element = getattr(self, f'{network_element_type}', None)
-            if network_element is None:
-                raise ValueError(f'Network has no elements associated with the {network_element_type=} requested')
-
-            network_element_to_search = [x for x in network_element.get_all() if x.name == name]
-
-        if network_element_to_search is None or len(network_element_to_search) == 0:
-            raise ValueError(f'No {network_element_type} found with {name=}')
-
-        matching_elements = []
-        for elements in network_element_to_search:
-            for prop, value in search_dict.items():
-                if getattr(elements, prop) == value:
-                    continue
-                else:
-                    break
-            else:
-                matching_elements.append(elements)
-
-        if len(matching_elements) == 1:
-            return matching_elements[0]
-        else:
-            raise ValueError(f'No unique matching {network_element_type} with the properties provided.'
-                             f'Instead found: {len(matching_elements)} matching {network_element_type}.')
+from __future__ import annotations
+from dataclasses import dataclass
+from typing import TYPE_CHECKING, Optional, Any, Literal
+
+from ResSimpy.Network import Network
+from ResSimpy.Nexus.nexus_collect_tables import collect_all_tables_to_objects
+from ResSimpy.Nexus.DataModels.Network.NexusConstraint import NexusConstraint
+from ResSimpy.Nexus.DataModels.Network.NexusConstraints import NexusConstraints
+from ResSimpy.Nexus.DataModels.Network.NexusNode import NexusNode
+from ResSimpy.Nexus.DataModels.Network.NexusNodeConnection import NexusNodeConnection
+from ResSimpy.Nexus.DataModels.Network.NexusNodeConnections import NexusNodeConnections
+from ResSimpy.Nexus.DataModels.Network.NexusNodes import NexusNodes
+from ResSimpy.Nexus.DataModels.Network.NexusWellConnection import NexusWellConnection
+from ResSimpy.Nexus.DataModels.Network.NexusWellConnections import NexusWellConnections
+from ResSimpy.Nexus.DataModels.Network.NexusWellbore import NexusWellbore
+from ResSimpy.Nexus.DataModels.Network.NexusWellbores import NexusWellbores
+from ResSimpy.Nexus.DataModels.Network.NexusWellhead import NexusWellhead
+from ResSimpy.Nexus.DataModels.Network.NexusWellheads import NexusWellheads
+from ResSimpy.Nexus.DataModels.NexusFile import NexusFile
+
+if TYPE_CHECKING:
+    from ResSimpy.Nexus.NexusSimulator import NexusSimulator
+
+
+@dataclass(kw_only=True)
+class NexusNetwork(Network):
+    __model: NexusSimulator
+    nodes: NexusNodes
+    connections: NexusNodeConnections
+    well_connections: NexusWellConnections
+    wellheads: NexusWellheads
+    wellbores: NexusWellbores
+    constraints: NexusConstraints
+    __has_been_loaded: bool = False
+
+    def __init__(self, model: NexusSimulator) -> None:
+        self.__has_been_loaded: bool = False
+        self.__model: NexusSimulator = model
+        self.nodes: NexusNodes = NexusNodes(self)
+        self.connections: NexusNodeConnections = NexusNodeConnections(self)
+        self.well_connections: NexusWellConnections = NexusWellConnections(self)
+        self.wellheads: NexusWellheads = NexusWellheads(self)
+        self.wellbores: NexusWellbores = NexusWellbores(self)
+        self.constraints: NexusConstraints = NexusConstraints(self, model)
+
+    def get_load_status(self) -> bool:
+        """Checks load status and loads the network if it hasn't already been loaded."""
+        if not self.__has_been_loaded:
+            self.load()
+        return self.__has_been_loaded
+
+    @property
+    def model(self) -> NexusSimulator:
+        return self.__model
+
+    def get_network_file(self, method_number: int = 1) -> NexusFile:
+        """Gets a specific network file object from the method number.
+
+        Args:
+        ----
+            method_number (int): Method number for selection of a specific surface file.
+                If None then returns a dictionary of method, surface file object
+
+        Returns:
+        -------
+            NexusFile: returns a specific surface file object of surface files keyed by method number
+        """
+        if self.__model.model_files.surface_files is None:
+            raise ValueError('No files found for the surface network')
+        network_file = self.__model.model_files.surface_files.get(method_number, None)
+        if network_file is None:
+            raise ValueError(f'No file found for {method_number=}, instead found {network_file=}')
+        return network_file
+
+    def load(self) -> None:
+        """Loads all the objects from the surface files in the Simulator class.
+        Table headers with None next to their name are currently skipped awaiting development.
+        """
+
+        def type_check_lists(input: Optional[list[Any] | dict[str, list[NexusConstraint]]]) -> Optional[list[Any]]:
+            """Guards against dictionaries coming from the dictionary."""
+            if isinstance(input, dict):
+                raise TypeError(f"Expected a list, instead received a dict: {input}")
+            return input
+
+        def type_check_dicts(input: Optional[list[Any] | dict[str, list[NexusConstraint]]]) -> \
+                Optional[dict[str, list[NexusConstraint]]]:
+            """Guards against dictionaries coming from the dictionary."""
+            if isinstance(input, list):
+                raise TypeError(f"Expected a dict, instead received a list: {input}")
+            return input
+
+        # TODO implement all objects with Nones next to them in the dictionary below
+        if self.__model.model_files.surface_files is None:
+            raise FileNotFoundError('Could not find any surface files associated with the fcs file provided.')
+
+        for surface in self.__model.model_files.surface_files.values():
+            nexus_obj_dict = collect_all_tables_to_objects(
+                surface, {'NODECON': NexusNodeConnection,
+                          'NODES': NexusNode,
+                          'WELLS': NexusWellConnection,
+                          'WELLHEAD': NexusWellhead,
+                          'WELLBORE': NexusWellbore,
+                          'CONSTRAINTS': NexusConstraint,
+                          'CONSTRAINT': NexusConstraint,
+                          'QMULT': NexusConstraint,
+                          'CONDEFAULTS': None,
+                          'TARGET': None,
+                          },
+                start_date=self.__model.start_date,
+                default_units=self.__model.default_units,
+                )
+            self.nodes._add_to_memory(type_check_lists(nexus_obj_dict.get('NODES')))
+            self.connections._add_to_memory(type_check_lists(nexus_obj_dict.get('NODECON')))
+            self.well_connections._add_to_memory(type_check_lists(nexus_obj_dict.get('WELLS')))
+            self.wellheads._add_to_memory(type_check_lists(nexus_obj_dict.get('WELLHEAD')))
+            self.wellbores._add_to_memory(type_check_lists(nexus_obj_dict.get('WELLBORE')))
+            self.constraints._add_to_memory(type_check_dicts(nexus_obj_dict.get('CONSTRAINTS')))
+
+        self.__has_been_loaded = True
+
+    def get_unique_names_in_network(self) -> list[str]:
+        """Extracts all names from a network including all the nodes, wells and connections.
+
+        Returns:
+            list[str]: list of all the unique names from the network including nodes, wells and connections
+
+        """
+        constraint_names_to_add = []
+        constraint_names_to_add.extend([x.name for x in self.nodes.get_all() if x.name is not None])
+        constraint_names_to_add.extend([x.name for x in self.well_connections.get_all()
+                                        if x.name is not None])
+        constraint_names_to_add.extend([x.name for x in self.connections.get_all() if x.name is not None])
+        constraint_names_to_add.extend([x.name for x in self.wellbores.get_all() if x.name is not None])
+        constraint_names_to_add.extend([x.name for x in self.wellheads.get_all() if x.name is not None])
+        constraint_names_to_add = list(set(constraint_names_to_add))
+
+        return constraint_names_to_add
+
+    def find_network_element_with_dict(self, name: str, search_dict: dict[str, None | float | str | int],
+                                       network_element_type: Literal['nodes', 'connections', 'well_connections',
+                                                                     'wellheads', 'wellbores', 'constraints']) -> Any:
+        """Finds a uniquely matching constraint from a given set of properties in a dictionary of attributes.
+
+        Args:
+            name (str): name of the node/connection to find
+            search_dict (dict[str, float | str | int]): dictionary of attributes to match on. \
+            Allows for partial matches if it finds a unique object.
+            network_element_type (Literal[str]): one of nodes, connections, well_connections, wellheads, wellbores,
+                constraints
+
+        Returns:
+            NexusConstraint of an existing constraint in the model that uniquely matches the provided \
+            constraint_dict constraint
+        """
+        network_element_to_search: Any = None
+        self.get_load_status()
+        if network_element_type == 'constraints':
+            network_element_to_search = self.constraints.get_all().get(name, None)
+        else:
+            # retrieve the getter method on the network attribute
+            network_element = getattr(self, f'{network_element_type}', None)
+            if network_element is None:
+                raise ValueError(f'Network has no elements associated with the {network_element_type=} requested')
+
+            network_element_to_search = [x for x in network_element.get_all() if x.name == name]
+
+        if network_element_to_search is None or len(network_element_to_search) == 0:
+            raise ValueError(f'No {network_element_type} found with {name=}')
+
+        matching_elements = []
+        for elements in network_element_to_search:
+            for prop, value in search_dict.items():
+                if getattr(elements, prop) == value:
+                    continue
+                else:
+                    break
+            else:
+                matching_elements.append(elements)
+
+        if len(matching_elements) == 1:
+            return matching_elements[0]
+        else:
+            raise ValueError(f'No unique matching {network_element_type} with the properties provided.'
+                             f'Instead found: {len(matching_elements)} matching {network_element_type}.')
```

### Comparing `ressimpy-1.0.0/ResSimpy/Nexus/NexusPVTMethods.py` & `ressimpy-1.0.1/ResSimpy/Nexus/NexusPVTMethods.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,69 +1,69 @@
-from dataclasses import dataclass
-import os
-from typing import Optional, MutableMapping
-from ResSimpy.Nexus.DataModels.NexusFile import NexusFile
-from ResSimpy.Nexus.DataModels.NexusPVTMethod import NexusPVTMethod
-from ResSimpy.PVT import PVT
-
-
-@dataclass(kw_only=True)
-class NexusPVTMethods(PVT):
-    """Class for collection of Nexus PVT property methods.
-
-    Attributes:
-        inputs (dict[int, NexusPVTMethod]): Collection of Nexus PVT property methods, as a dictionary
-        files (dict[int, NexusFile]): Dictionary collection of PVT property files, as defined in Nexus fcs file.
-    """
-
-    __inputs: MutableMapping[int, NexusPVTMethod]
-    __files: dict[int, NexusFile]
-    __properties_loaded: bool = False  # Used in lazy loading
-
-    def __init__(self, inputs: Optional[MutableMapping[int, NexusPVTMethod]] = None,
-                 files: Optional[dict[int, NexusFile]] = None) -> None:
-        if inputs:
-            self.__inputs = inputs
-        else:
-            self.__inputs: MutableMapping[int, NexusPVTMethod] = {}
-        if files:
-            self.__files = files
-        else:
-            self.__files = {}
-        super().__init__()
-
-    def __repr__(self) -> str:
-        """Pretty printing pvt methods."""
-        if not self.__properties_loaded:
-            self.load_pvt_methods()
-        printable_str = ''
-        for table_num in self.__inputs.keys():
-            printable_str += '\n--------------------------------\n'
-            printable_str += f'PVT method {table_num}\n'
-            printable_str += '--------------------------------\n'
-            printable_str += self.__inputs[table_num].__repr__()
-            printable_str += '\n'
-
-        return printable_str
-
-    @property
-    def inputs(self) -> MutableMapping[int, NexusPVTMethod]:
-        if not self.__properties_loaded:
-            self.load_pvt_methods()
-        return self.__inputs
-
-    @property
-    def files(self) -> dict[int, NexusFile]:
-        return self.__files
-
-    def load_pvt_methods(self):
-        # Read in pvt properties from Nexus pvt method files
-        if self.__files is not None and len(self.__files) > 0:  # Check if pvt files exist
-            for table_num in self.__files.keys():  # For each pvt property method
-                pvt_file = self.__files[table_num]
-                if pvt_file.location is None:
-                    raise ValueError(f'Unable to find pvt file: {pvt_file}')
-                if os.path.isfile(pvt_file.location):
-                    # Create NexusPVTMethod object
-                    self.__inputs[table_num] = NexusPVTMethod(file=pvt_file, input_number=table_num)
-                    self.__inputs[table_num].read_properties()  # Populate object with pvt properties in file
-        self.__properties_loaded = True
+from dataclasses import dataclass
+import os
+from typing import Optional, MutableMapping
+from ResSimpy.Nexus.DataModels.NexusFile import NexusFile
+from ResSimpy.Nexus.DataModels.NexusPVTMethod import NexusPVTMethod
+from ResSimpy.PVT import PVT
+
+
+@dataclass(kw_only=True)
+class NexusPVTMethods(PVT):
+    """Class for collection of Nexus PVT property methods.
+
+    Attributes:
+        inputs (dict[int, NexusPVTMethod]): Collection of Nexus PVT property methods, as a dictionary
+        files (dict[int, NexusFile]): Dictionary collection of PVT property files, as defined in Nexus fcs file.
+    """
+
+    __inputs: MutableMapping[int, NexusPVTMethod]
+    __files: dict[int, NexusFile]
+    __properties_loaded: bool = False  # Used in lazy loading
+
+    def __init__(self, inputs: Optional[MutableMapping[int, NexusPVTMethod]] = None,
+                 files: Optional[dict[int, NexusFile]] = None) -> None:
+        if inputs:
+            self.__inputs = inputs
+        else:
+            self.__inputs: MutableMapping[int, NexusPVTMethod] = {}
+        if files:
+            self.__files = files
+        else:
+            self.__files = {}
+        super().__init__()
+
+    def __repr__(self) -> str:
+        """Pretty printing pvt methods."""
+        if not self.__properties_loaded:
+            self.load_pvt_methods()
+        printable_str = ''
+        for table_num in self.__inputs.keys():
+            printable_str += '\n--------------------------------\n'
+            printable_str += f'PVT method {table_num}\n'
+            printable_str += '--------------------------------\n'
+            printable_str += self.__inputs[table_num].__repr__()
+            printable_str += '\n'
+
+        return printable_str
+
+    @property
+    def inputs(self) -> MutableMapping[int, NexusPVTMethod]:
+        if not self.__properties_loaded:
+            self.load_pvt_methods()
+        return self.__inputs
+
+    @property
+    def files(self) -> dict[int, NexusFile]:
+        return self.__files
+
+    def load_pvt_methods(self):
+        # Read in pvt properties from Nexus pvt method files
+        if self.__files is not None and len(self.__files) > 0:  # Check if pvt files exist
+            for table_num in self.__files.keys():  # For each pvt property method
+                pvt_file = self.__files[table_num]
+                if pvt_file.location is None:
+                    raise ValueError(f'Unable to find pvt file: {pvt_file}')
+                if os.path.isfile(pvt_file.location):
+                    # Create NexusPVTMethod object
+                    self.__inputs[table_num] = NexusPVTMethod(file=pvt_file, input_number=table_num)
+                    self.__inputs[table_num].read_properties()  # Populate object with pvt properties in file
+        self.__properties_loaded = True
```

### Comparing `ressimpy-1.0.0/ResSimpy/Nexus/NexusRelPermMethods.py` & `ressimpy-1.0.1/ResSimpy/Nexus/NexusRelPermMethods.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,70 +1,70 @@
-from dataclasses import dataclass
-import os
-from typing import Optional, MutableMapping
-from ResSimpy.Nexus.DataModels.NexusFile import NexusFile
-from ResSimpy.Nexus.DataModels.NexusRelPermMethod import NexusRelPermMethod
-from ResSimpy.RelPerm import RelPerm
-
-
-@dataclass(kw_only=True)
-class NexusRelPermMethods(RelPerm):
-    """Class for collection of Nexus relative permeability and capillary pressure property inputs.
-
-    Attributes:
-        inputs (dict[int, NexusRelPermMethod]): Collection of Nexus relperm property inputs, as a dictionary
-        files (dict[int, NexusFile]): Dictionary collection of relperm property files, as defined in Nexus fcs.
-    """
-
-    __inputs: MutableMapping[int, NexusRelPermMethod]
-    __files: dict[int, NexusFile]
-    __properties_loaded: bool = False  # Used in lazy loading
-
-    def __init__(self, inputs: Optional[MutableMapping[int, NexusRelPermMethod]] = None,
-                 files: Optional[dict[int, NexusFile]] = None) -> None:
-        if inputs:
-            self.__inputs = inputs
-        else:
-            self.__inputs: MutableMapping[int, NexusRelPermMethod] = {}
-        if files:
-            self.__files = files
-        else:
-            self.__files = {}
-        super().__init__()
-
-    def __repr__(self) -> str:
-        """Pretty printing relative permeability and capillary pressure methods."""
-        if not self.__properties_loaded:
-            self.load_relperm_methods()
-        printable_str = ''
-        for table_num in self.__inputs.keys():
-            printable_str += '\n--------------------------------\n'
-            printable_str += f'RELPM method {table_num}\n'
-            printable_str += '--------------------------------\n'
-            printable_str += self.__inputs[table_num].__repr__()
-            printable_str += '\n'
-
-        return printable_str
-
-    @property
-    def inputs(self) -> MutableMapping[int, NexusRelPermMethod]:
-        if not self.__properties_loaded:
-            self.load_relperm_methods()
-        return self.__inputs
-
-    @property
-    def files(self) -> dict[int, NexusFile]:
-        return self.__files
-
-    def load_relperm_methods(self):
-        # Read in relperm properties from Nexus relperm method files
-        if self.__files is not None and len(self.__files) > 0:  # Check if relperm files exist
-            for table_num in self.__files.keys():  # For each relperm property method
-                relperm_file = self.__files[table_num]
-                if relperm_file.location is None:
-                    raise ValueError(f'Unable to find relperm file: {relperm_file}')
-                if os.path.isfile(relperm_file.location):
-                    # Create NexusRelPermMethod object
-                    self.__inputs[table_num] = NexusRelPermMethod(file=relperm_file, input_number=table_num)
-                    # Populate object with relperm properties in file
-                    self.__inputs[table_num].read_properties()
-        self.__properties_loaded = True
+from dataclasses import dataclass
+import os
+from typing import Optional, MutableMapping
+from ResSimpy.Nexus.DataModels.NexusFile import NexusFile
+from ResSimpy.Nexus.DataModels.NexusRelPermMethod import NexusRelPermMethod
+from ResSimpy.RelPerm import RelPerm
+
+
+@dataclass(kw_only=True)
+class NexusRelPermMethods(RelPerm):
+    """Class for collection of Nexus relative permeability and capillary pressure property inputs.
+
+    Attributes:
+        inputs (dict[int, NexusRelPermMethod]): Collection of Nexus relperm property inputs, as a dictionary
+        files (dict[int, NexusFile]): Dictionary collection of relperm property files, as defined in Nexus fcs.
+    """
+
+    __inputs: MutableMapping[int, NexusRelPermMethod]
+    __files: dict[int, NexusFile]
+    __properties_loaded: bool = False  # Used in lazy loading
+
+    def __init__(self, inputs: Optional[MutableMapping[int, NexusRelPermMethod]] = None,
+                 files: Optional[dict[int, NexusFile]] = None) -> None:
+        if inputs:
+            self.__inputs = inputs
+        else:
+            self.__inputs: MutableMapping[int, NexusRelPermMethod] = {}
+        if files:
+            self.__files = files
+        else:
+            self.__files = {}
+        super().__init__()
+
+    def __repr__(self) -> str:
+        """Pretty printing relative permeability and capillary pressure methods."""
+        if not self.__properties_loaded:
+            self.load_relperm_methods()
+        printable_str = ''
+        for table_num in self.__inputs.keys():
+            printable_str += '\n--------------------------------\n'
+            printable_str += f'RELPM method {table_num}\n'
+            printable_str += '--------------------------------\n'
+            printable_str += self.__inputs[table_num].__repr__()
+            printable_str += '\n'
+
+        return printable_str
+
+    @property
+    def inputs(self) -> MutableMapping[int, NexusRelPermMethod]:
+        if not self.__properties_loaded:
+            self.load_relperm_methods()
+        return self.__inputs
+
+    @property
+    def files(self) -> dict[int, NexusFile]:
+        return self.__files
+
+    def load_relperm_methods(self):
+        # Read in relperm properties from Nexus relperm method files
+        if self.__files is not None and len(self.__files) > 0:  # Check if relperm files exist
+            for table_num in self.__files.keys():  # For each relperm property method
+                relperm_file = self.__files[table_num]
+                if relperm_file.location is None:
+                    raise ValueError(f'Unable to find relperm file: {relperm_file}')
+                if os.path.isfile(relperm_file.location):
+                    # Create NexusRelPermMethod object
+                    self.__inputs[table_num] = NexusRelPermMethod(file=relperm_file, input_number=table_num)
+                    # Populate object with relperm properties in file
+                    self.__inputs[table_num].read_properties()
+        self.__properties_loaded = True
```

### Comparing `ressimpy-1.0.0/ResSimpy/Nexus/NexusReporting.py` & `ressimpy-1.0.1/ResSimpy/Nexus/NexusReporting.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,44 +1,44 @@
-import ResSimpy.Nexus.nexus_file_operations as nfo
-
-
-class Reporting:
-    def __init__(self, model) -> None:
-        self.__model = model
-
-    def add_map_properties_to_start_of_grid_file(self):
-        """Adds 'map' statements to the start of the grid file to ensure standalone outputs all the required \
-        properties. Writes out to the same structured grid file path provided.
-
-        Raises:
-            ValueError: if no structured grid file path is specified in the class instance
-        """
-        structured_grid_path = self.__model.structured_grid_path
-        if self.__model.structured_grid_path is None:
-            raise ValueError("No file path given or found for structured grid file path. \
-                Please update structured grid file path")
-        file = nfo.load_file_as_list(structured_grid_path)
-
-        if not nfo.value_in_file('MAPBINARY', file):
-            new_file = ['MAPBINARY\n']
-        else:
-            new_file = []
-
-        if not nfo.value_in_file('MAPVDB', file):
-            new_file.extend(['MAPVDB\n'])
-
-        if not nfo.value_in_file('MAPOUT', file):
-            new_file.extend(['MAPOUT ALL\n'])
-        else:
-            line_counter = 0
-            for line in file:
-                if nfo.check_token('MAPOUT', line):
-                    file[line_counter] = 'MAPOUT ALL\n'
-                    break
-                line_counter += 1
-
-        new_file.extend(file)
-
-        # Save the new file contents
-        new_file_str = "".join(new_file)
-        with open(structured_grid_path, "w") as text_file:
-            text_file.write(new_file_str)
+import ResSimpy.Nexus.nexus_file_operations as nfo
+
+
+class Reporting:
+    def __init__(self, model) -> None:
+        self.__model = model
+
+    def add_map_properties_to_start_of_grid_file(self):
+        """Adds 'map' statements to the start of the grid file to ensure standalone outputs all the required \
+        properties. Writes out to the same structured grid file path provided.
+
+        Raises:
+            ValueError: if no structured grid file path is specified in the class instance
+        """
+        structured_grid_path = self.__model.structured_grid_path
+        if self.__model.structured_grid_path is None:
+            raise ValueError("No file path given or found for structured grid file path. \
+                Please update structured grid file path")
+        file = nfo.load_file_as_list(structured_grid_path)
+
+        if not nfo.value_in_file('MAPBINARY', file):
+            new_file = ['MAPBINARY\n']
+        else:
+            new_file = []
+
+        if not nfo.value_in_file('MAPVDB', file):
+            new_file.extend(['MAPVDB\n'])
+
+        if not nfo.value_in_file('MAPOUT', file):
+            new_file.extend(['MAPOUT ALL\n'])
+        else:
+            line_counter = 0
+            for line in file:
+                if nfo.check_token('MAPOUT', line):
+                    file[line_counter] = 'MAPOUT ALL\n'
+                    break
+                line_counter += 1
+
+        new_file.extend(file)
+
+        # Save the new file contents
+        new_file_str = "".join(new_file)
+        with open(structured_grid_path, "w") as text_file:
+            text_file.write(new_file_str)
```

### Comparing `ressimpy-1.0.0/ResSimpy/Nexus/NexusSeparatorMethods.py` & `ressimpy-1.0.1/ResSimpy/Nexus/NexusGasliftMethods.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,71 +1,69 @@
-from dataclasses import dataclass
-import os
-from typing import Optional, MutableMapping
-from ResSimpy.Nexus.DataModels.NexusFile import NexusFile
-from ResSimpy.Nexus.DataModels.NexusSeparatorMethod import NexusSeparatorMethod
-from ResSimpy.Separator import Separator
-
-
-@dataclass(kw_only=True)
-class NexusSeparatorMethods(Separator):
-    """Class for collection of Nexus separator property methods.
-
-    Attributes:
-        inputs (dict[int, NexusSeparatorMethod]): Dictionary collection of Nexus separator property methods
-        files (dict[int, NexusFile]): Dictionary collection of separator property files, defined in Nexus fcs.
-    """
-
-    __inputs: MutableMapping[int, NexusSeparatorMethod]
-    __files: dict[int, NexusFile]
-    __properties_loaded: bool = False  # Used in lazy loading
-
-    def __init__(self, inputs: Optional[MutableMapping[int, NexusSeparatorMethod]] = None,
-                 files: Optional[dict[int, NexusFile]] = None) -> None:
-        if inputs:
-            self.__inputs = inputs
-        else:
-            self.__inputs: MutableMapping[int, NexusSeparatorMethod] = {}
-        if files:
-            self.__files = files
-        else:
-            self.__files = {}
-        super().__init__()
-
-    def __repr__(self) -> str:
-        """Pretty printing separator methods."""
-        if not self.__properties_loaded:
-            self.load_separator_methods()
-        printable_str = ''
-        for table_num in self.__inputs.keys():
-            printable_str += '\n--------------------------------\n'
-            printable_str += f'SEPARATOR method {table_num}\n'
-            printable_str += '--------------------------------\n'
-            printable_str += f'\nSEPARATOR_TYPE: {self.__inputs[table_num].separator_type}\n'
-            printable_str += self.__inputs[table_num].__repr__()
-            printable_str += '\n'
-
-        return printable_str
-
-    @property
-    def inputs(self) -> MutableMapping[int, NexusSeparatorMethod]:
-        if not self.__properties_loaded:
-            self.load_separator_methods()
-        return self.__inputs
-
-    @property
-    def files(self) -> dict[int, NexusFile]:
-        return self.__files
-
-    def load_separator_methods(self):
-        # Read in separator properties from Nexus separator method files
-        if self.__files is not None and len(self.__files) > 0:  # Check if separator files exist
-            for table_num in self.__files.keys():  # For each separator property method
-                separator_file = self.__files[table_num]
-                if separator_file.location is None:
-                    raise ValueError(f'Unable to find separator file: {separator_file}')
-                if os.path.isfile(separator_file.location):
-                    # Create NexusSeparatorMethod object
-                    self.__inputs[table_num] = NexusSeparatorMethod(file=separator_file, input_number=table_num)
-                    # Populate object with separator properties in input file
-                    self.__inputs[table_num].read_properties()
-        self.__properties_loaded = True
+from dataclasses import dataclass
+import os
+from typing import Optional, MutableMapping
+from ResSimpy.Nexus.DataModels.NexusFile import NexusFile
+from ResSimpy.Nexus.DataModels.NexusGasliftMethod import NexusGasliftMethod
+from ResSimpy.Gaslift import Gaslift
+
+
+@dataclass(kw_only=True)
+class NexusGasliftMethods(Gaslift):
+    """Class for collection of Nexus gaslift methods.
+
+    Attributes:
+        inputs (dict[int, NexusGasliftMethod]): Collection of Nexus gaslift methods, as a dictionary
+        files (dict[int, NexusFile]): Dictionary collection of gaslift files, as defined in Nexus fcs file.
+    """
+
+    __inputs: MutableMapping[int, NexusGasliftMethod]
+    __files: dict[int, NexusFile]
+    __properties_loaded: bool = False  # Used in lazy loading
+
+    def __init__(self, inputs: Optional[MutableMapping[int, NexusGasliftMethod]] = None,
+                 files: Optional[dict[int, NexusFile]] = None) -> None:
+        if inputs:
+            self.__inputs = inputs
+        else:
+            self.__inputs: MutableMapping[int, NexusGasliftMethod] = {}
+        if files:
+            self.__files = files
+        else:
+            self.__files = {}
+        super().__init__()
+
+    def __repr__(self) -> str:
+        """Pretty printing gaslift methods."""
+        if not self.__properties_loaded:
+            self.load_gaslift_methods()
+        printable_str = ''
+        for table_num in self.__inputs.keys():
+            printable_str += '\n--------------------------------\n'
+            printable_str += f'GASLIFT method {table_num}\n'
+            printable_str += '--------------------------------\n'
+            printable_str += self.__inputs[table_num].__repr__()
+            printable_str += '\n'
+
+        return printable_str
+
+    @property
+    def inputs(self) -> MutableMapping[int, NexusGasliftMethod]:
+        if not self.__properties_loaded:
+            self.load_gaslift_methods()
+        return self.__inputs
+
+    @property
+    def files(self) -> dict[int, NexusFile]:
+        return self.__files
+
+    def load_gaslift_methods(self):
+        # Read in gaslift properties from Nexus gaslift method files
+        if self.__files is not None and len(self.__files) > 0:  # Check if gaslift files exist
+            for table_num in self.__files.keys():  # For each gaslift property method
+                gaslift_file = self.__files[table_num]
+                if gaslift_file.location is None:
+                    raise ValueError(f'Unable to find gaslift file: {gaslift_file}')
+                if os.path.isfile(gaslift_file.location):
+                    # Create NexusGasliftMethod object
+                    self.__inputs[table_num] = NexusGasliftMethod(file=gaslift_file, input_number=table_num)
+                    self.__inputs[table_num].read_properties()  # Populate object with gaslift props in file
+        self.__properties_loaded = True
```

### Comparing `ressimpy-1.0.0/ResSimpy/Nexus/NexusSimulator.py` & `ressimpy-1.0.1/ResSimpy/Nexus/NexusSimulator.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,672 +1,672 @@
-from __future__ import annotations
-
-import os
-import warnings
-from typing import Any, Union, Optional
-
-import resqpy.model as rq
-from datetime import datetime
-import ResSimpy.Nexus.nexus_file_operations as nfo
-from ResSimpy.Nexus.DataModels.FcsFile import FcsNexusFile
-from ResSimpy.Nexus.DataModels.NexusFile import NexusFile
-from ResSimpy.Nexus.NexusPVTMethods import NexusPVTMethods
-from ResSimpy.Nexus.NexusSeparatorMethods import NexusSeparatorMethods
-from ResSimpy.Nexus.NexusWaterMethods import NexusWaterMethods
-from ResSimpy.Nexus.NexusEquilMethods import NexusEquilMethods
-from ResSimpy.Nexus.NexusRockMethods import NexusRockMethods
-from ResSimpy.Nexus.NexusRelPermMethods import NexusRelPermMethods
-from ResSimpy.Nexus.NexusValveMethods import NexusValveMethods
-from ResSimpy.Nexus.NexusAquiferMethods import NexusAquiferMethods
-from ResSimpy.Nexus.NexusHydraulicsMethods import NexusHydraulicsMethods
-from ResSimpy.Nexus.NexusGasliftMethods import NexusGasliftMethods
-from ResSimpy.Nexus.DataModels.StructuredGrid.NexusGrid import NexusGrid
-from ResSimpy.Nexus.NexusEnums.DateFormatEnum import DateFormat
-from ResSimpy.Enums.UnitsEnum import UnitSystem
-from ResSimpy.Nexus.NexusNetwork import NexusNetwork
-from ResSimpy.Nexus.NexusReporting import Reporting
-from ResSimpy.Nexus.NexusWells import NexusWells
-from ResSimpy.Nexus.runcontrol_operations import SimControls
-from ResSimpy.Nexus.logfile_operations import Logging
-from ResSimpy.Nexus.structured_grid_operations import StructuredGridOperations
-from ResSimpy.Simulator import Simulator
-
-
-class NexusSimulator(Simulator):
-
-    def __init__(self, origin: Optional[str] = None, destination: Optional[str] = None,
-                 root_name: Optional[str] = None, nexus_data_name: str = "data", write_times: bool = False,
-                 manual_fcs_tidy_call: bool = False, lazy_loading: bool = True) -> None:
-        """Nexus simulator class. Inherits from the Simulator super class.
-
-        Args:
-            origin (Optional[str], optional): file path to the fcs file. Defaults to None.
-            root_name (Optional[str], optional): Root file name of the fcs. Defaults to None.
-            nexus_data_name (str, optional): Folder name for the nexus data files to be stored in. Defaults to "data".
-            write_times (bool, optional): Sets whether the runcontrol file will expand the include files with time \
-                cards in. Defaults to True.
-            manual_fcs_tidy_call (bool, optional): Determines whether fcs_tidy should be called - Currently not used. \
-                Defaults to False.
-
-        Attributes:
-            run_control_file_path (Optional[str]): file path to the run control file - derived from the fcs file
-            __destination (Optional[str]): output path for the simulation. Currently not used.
-            date_format (DateFormat): Enum value representing the date format.
-            __original_fcs_file_path (str): Path to the original fcs file path supplied
-            __new_fcs_file_path (str): Where the new fcs will be saved to
-            __force_output (bool): private attribute of force_output
-            __origin (str): private attribute of origin. File path to the fcs file.
-            __root_name (str): private attribute of root_name. Root file name of the fcs.
-            __nexus_data_name (str): private attribute of nexus_data_name. Folder name for the nexus data files to be \
-                stored in.
-            __structured_grid_file_path (Optional[str]): file path to the structured grid.
-            __structured_grid_file (Optional[NexusGrid]): StructuredGridFile object representing the \
-                structured grid used in Nexus
-            __run_units (Optional[str]): Unit system used in the Nexus model
-            use_american_run_units (bool): True if an American unit system is used equivalent to 'ENGLISH'. \
-                False otherwise. For the RUN_UNITS keyword.
-            use_american_input_units (bool): True if an American unit system is used equivalent to 'ENGLISH'. \
-                False otherwise. For the DEFAULT_UNITS keyword.
-            __write_times (bool): private attribute for write_times. Sets whether the runcontrol file will expand \
-                the include files with time cards in.
-            __manual_fcs_tidy_call (bool): private attribute for manual_fcs_tidy_call. Determines whether fcs_tidy \
-                should be called
-
-        Raises:
-            ValueError: If the FCS file path is not given
-        """
-        if origin is None:
-            raise ValueError(f'Origin path to model fcs file is required. Instead got {origin}.')
-        self.origin: str = origin
-
-        self._start_date: str = ''
-        self.run_control_file_path: Optional[str] = ''
-        self.__destination: Optional[str] = None
-        self.date_format: DateFormat = DateFormat.MM_DD_YYYY  # Nexus default
-        self.__original_fcs_file_path: str = self.origin
-        self.__new_fcs_file_path: str = self.origin
-        self.__nexus_data_name: str = nexus_data_name
-        self.__run_units: UnitSystem = UnitSystem.ENGLISH  # The Nexus default
-        self.root_name: str = root_name
-        self.use_american_run_units: bool = False
-        self.use_american_input_units: bool = False
-        self.__write_times: bool = write_times
-        self.__manual_fcs_tidy_call: bool = manual_fcs_tidy_call
-
-        self.__default_units: UnitSystem = UnitSystem.ENGLISH  # The Nexus default
-        #
-        self._wells: NexusWells = NexusWells(self)
-        self._grid: Optional[NexusGrid] = None
-        self._network: NexusNetwork = NexusNetwork(model=self)
-        # Model dynamic properties
-        self._pvt: NexusPVTMethods = NexusPVTMethods()
-        self._separator: NexusSeparatorMethods = NexusSeparatorMethods()
-        self._water: NexusWaterMethods = NexusWaterMethods()
-        self._equil: NexusEquilMethods = NexusEquilMethods()
-        self._rock: NexusRockMethods = NexusRockMethods()
-        self._relperm: NexusRelPermMethods = NexusRelPermMethods()
-        self._valve: NexusValveMethods = NexusValveMethods()
-        self._aquifer: NexusAquiferMethods = NexusAquiferMethods()
-        self._hydraulics: NexusHydraulicsMethods = NexusHydraulicsMethods()
-        self._gaslift: NexusGasliftMethods = NexusGasliftMethods()
-        # Nexus operations modules
-        self._sim_controls: SimControls = SimControls(self)
-        self.reporting: Reporting = Reporting(self)
-        self._structured_grid_operations: StructuredGridOperations = StructuredGridOperations(self)
-        self.logging: Logging = Logging(self)
-        self.__lazy_loading: bool = lazy_loading
-
-        if destination is not None and destination != '':
-            self.set_output_path(path=destination.strip())
-
-        # Check the status of any existing or completed runs related to this model
-        self.get_simulation_status(from_startup=True)
-
-        self._model_files: FcsNexusFile
-        # Load in the model
-        self.__load_fcs_file()
-
-    def remove_temp_from_properties(self):
-        """Updates model values if the files are moved from a temp directory
-        Replaces the first instance of temp/ in the file paths in the nexus simulation file paths.
-
-        Raises:
-            ValueError: if any of [__structured_grid_file_path, __new_fcs_file_path, __surface_file_path] are None.
-        """
-        if self.model_files.structured_grid_file.location is None:
-            raise ValueError(
-                "No structured_grid_file_path found, can't remove temporary properties from file path")
-        if self.__new_fcs_file_path is None:
-            raise ValueError(
-                "No __new_fcs_file_path found, can't remove temporary properties from file path")
-        if self.model_files.surface_files[1] is None or self.model_files.surface_files[1].location is None:
-            raise ValueError(
-                "No __surface_file_path found, can't remove temporary properties from file path")
-
-        self._origin = self._origin.replace('temp/', '', 1)
-        self.__root_name = self.__root_name.replace('temp/', '', 1)
-        self.model_files.structured_grid_file.location = \
-            self.model_files.structured_grid_file.location.replace('temp/', '', 1)
-        self.__new_fcs_file_path = self.__new_fcs_file_path.replace('temp/', '', 1)
-        self.model_files.surface_files[1].location = self.model_files.surface_files[1].location.replace('temp/', '', 1)
-
-    def get_simulation_status(self, from_startup: bool = False) -> Optional[str]:
-        return self.logging.get_simulation_status(from_startup)
-
-    def get_simulation_progress(self) -> float:
-        return self.logging.get_simulation_progress()
-
-    def get_users_linked_with_files(self) -> Optional[list[tuple[Optional[str], Optional[str], Optional[datetime]]]]:
-        return self.model_files.files_info
-
-    @property
-    def model_files(self) -> FcsNexusFile:
-        return self._model_files
-
-    @property
-    def structured_grid_path(self):
-        """Returns the location of the structured grid file."""
-        return self.model_files.structured_grid_file.location
-
-    @property
-    def default_units(self):
-        """Returns the default units."""
-        return self.__default_units
-
-    @property
-    def run_units(self):
-        """Returns the run units."""
-        return self.__run_units
-
-    @property
-    def new_fcs_name(self):
-        """Returns the new name for the FCS file without the fcs extension."""
-        return self.__root_name
-
-    @property
-    def write_times(self) -> bool:
-        return self.__write_times
-
-    @property
-    def original_fcs_file_path(self):
-        return self.__original_fcs_file_path
-
-    @property
-    def root_name(self):
-        return self.__root_name
-
-    @root_name.setter
-    def root_name(self, value: str) -> None:
-        """Returns the name of the fcs file without the .fcs extension.
-
-        Returns:
-            str: string of the fcs file without the .fcs extension.
-        """
-        if value is not None:
-            rootname = value
-        else:
-            rootname = os.path.basename(self._origin)
-            rootname = rootname.split(".fcs")[0]
-        self.__root_name = rootname
-
-    @staticmethod
-    def get_check_run_input_units_for_models(models: list[str]) -> tuple[Optional[bool], Optional[bool]]:
-        # TODO: add LAB units
-        """Returns the run and input unit formats for all the supplied models.
-
-        Supported model formats:
-            RESQML type epc files ending in ".epc"
-            Nexus files containing a line identifying the "RUN_UNITS" or "DEFAULT_UNITS".
-
-        Supported units: ENGLISH, METRIC
-
-        Args:
-            models (list[str]): list of paths to supported reservoir models
-
-        Raises:
-            ValueError: if a model in the list is using inconcistent run/default units
-
-        Returns:
-            Tuple[Optional[Bool], Optional[Bool]]: If all units are consistent between models,
-                Returns (True, True) if 'ft' is the length unit in an epc or Nexus specifies "ENGLISH" as the
-                (RUN_UNITS,DEFAULT_UNITS) respectively and False, False otherwise.
-                Returns (None, None) if it can't find a (RUN_UNITS, DEFAULT_UNITS) in the supplied files.
-        """
-        oilfield_run_units: Optional[bool] = None
-        oilfield_default_units: Optional[bool] = None
-
-        for model in models:
-            # If we're checking the units of a RESQML model, read it in and get the units. Otherwise, read the units
-            # from the fcs file
-            if os.path.splitext(model)[1] == '.epc':
-                resqpy_model = rq.Model(epc_file=model)
-
-                # Load in the RESQML grid
-                grid = resqpy_model.grid()
-
-                # Check the grid units
-                grid_length_unit = grid.xy_units()
-                model_oilfield_default_units = grid_length_unit == 'ft'
-                model_oilfield_run_units = grid_length_unit == 'ft'
-            else:
-                simulator = NexusSimulator(origin=model)
-                model_oilfield_default_units = simulator.default_units == UnitSystem.ENGLISH
-                model_oilfield_run_units = simulator.run_units == UnitSystem.ENGLISH
-
-            # If not defined, assign it to model_oilfield_default_units
-            if oilfield_default_units is None:
-                oilfield_default_units = model_oilfield_default_units
-            # Raise ValueError if default units are inconsistent with the other models
-            elif model_oilfield_default_units != oilfield_default_units:
-                raise ValueError(f"Model at {model} using inconsistent default units")
-
-            # If not defined, assign it to model_oilfield_run_units
-            if oilfield_run_units is None:
-                oilfield_run_units = model_oilfield_run_units
-            # Raise ValueError if run units are inconsistent with the other models
-            elif model_oilfield_run_units != oilfield_run_units:
-                raise ValueError(f"Model at {model} using inconsistent run units")
-
-        return oilfield_run_units, oilfield_default_units
-
-    @staticmethod
-    def get_check_oil_gas_types_for_models(models: list[str]) -> Optional[str]:
-        """Checks for fluid types within a list of paths to models.
-        Currently limited to checking for the first SURFACE network in a file.
-
-        Args:
-            models (list[str]): a list of paths to models to check for fluid types.
-
-        Raises:
-            ValueError: If fluid types are inconsistent between models
-
-        Returns:
-            Optional[str]: The fluid type used for the model for the first surface network
-        """
-        fluid_type = None
-        for model in models:
-            model_fluid_type = None
-            fcs_file = NexusFile.generate_file_include_structure(model).get_flat_list_str_file
-            surface_filename = None
-            if fcs_file is None:
-                warnings.warn(UserWarning(f'No file found for {model}'))
-                continue
-            for line in fcs_file:
-                if nfo.check_token("SURFACE Network 1", line):
-                    surface_filename = nfo.get_expected_token_value(token="SURFACE Network 1", token_line=line,
-                                                                    file_list=fcs_file)
-                    break
-
-            if surface_filename is not None:
-                surface_filename = surface_filename if os.path.isabs(surface_filename) else \
-                    os.path.dirname(model) + "/" + surface_filename
-                model_fluid_type = NexusSimulator.get_fluid_type(
-                    surface_file_name=surface_filename)
-
-            if fluid_type is None:
-                fluid_type = model_fluid_type
-            elif fluid_type != model_fluid_type:
-                raise ValueError(
-                    f"Inconsistent Oil / Gas types: {model_fluid_type} found for {model}")
-
-        return fluid_type
-
-    @staticmethod
-    def get_eos_details(surface_file: list[str]) -> str:
-        """Gets all the information about an EOS from a Nexus model.
-
-        Args:
-            surface_file (list[str]): path to the surface file in a Nexus model
-
-        Returns:
-            str: a concatenated string of EOS components
-        """
-        eos_string: str = ''
-        eos_found: bool = False
-        for line in surface_file:
-            if nfo.check_token("EOS", line):
-                eos_string += line
-                eos_found = True
-            elif eos_found:
-                eos_string += line
-            if nfo.check_token("COMPONENTS", line):
-                break
-
-        return eos_string
-
-    @staticmethod
-    def get_fluid_type(surface_file_name: str) -> str:
-        """Gets the fluid type for a single model from a surface file.
-
-        Args:
-            surface_file_name (str): path to the surface file in a Nexus model
-
-        Raises:
-            ValueError: if no fluid type is found within the provided file path
-
-        Returns:
-            str: fluid type as one of [BLACKOIL, WATEROIL, GASWATER,] or the full details from an EOS model
-        """
-        surface_file = nfo.load_file_as_list(surface_file_name)
-        fluid_type = None
-
-        for line in surface_file:
-            if nfo.check_token("BLACKOIL", line):
-                fluid_type = "BLACKOIL"
-                break
-            elif nfo.check_token("WATEROIL", line):
-                fluid_type = "WATEROIL"
-                break
-            elif nfo.check_token("GASWATER", line):
-                fluid_type = "GASWATER"
-                break
-            elif nfo.check_token("EOS", line):
-                fluid_type = NexusSimulator.get_eos_details(surface_file)
-
-        if fluid_type is None:
-            raise ValueError("No Oil / Gas type detected")
-
-        return fluid_type
-
-    def get_model_oil_type(self) -> str:
-        """Returns the get_fluid_type method on the existing NexusSimulator instance.
-
-        Raises:
-            ValueError: If no file path is provided for the surface file path
-
-        Returns:
-            str: fluid type as one of [BLACKOIL, WATEROIL, GASWATER,] or the full details from an EOS model
-        """
-        if self.model_files.surface_files is None or self.model_files.surface_files[1].location is None:
-            raise ValueError("No value found for the path to the surface file")
-        return NexusSimulator.get_fluid_type(self.model_files.surface_files[1].location)
-
-    def check_output_path(self) -> None:
-        """Confirms that the output path has been set (used to stop accidental writing operations in the original
-        directory).
-
-        Raises:
-            ValueError: if the destination provided is set to None.
-        """
-        if self.__destination is None:
-            raise ValueError("Destination is required for this operation. Currently set to: ", self.__destination)
-
-    @property
-    def destination(self) -> Optional[str]:
-        return self.__destination
-
-    def set_output_path(self, path: str) -> None:
-        """Initialises the output to the declared output location.
-        If the file is a different directory to the origin path location the function will set the origin
-        to the new destination.
-        """
-        self.__destination = path
-        if self.__destination is not None and os.path.dirname(self._origin) != os.path.dirname(self.__destination):
-            self._origin = self.__destination + "/" + os.path.basename(self.__original_fcs_file_path)
-
-    def __load_fcs_file(self):
-        """Loads in the information from the supplied FCS file into the class instance.
-        Loads in the paths for runcontrol, structured grid and the first surface network.
-        Loads in the values for dateformat and run units.
-        Attempts to load the run_control_file.
-        Loads the wellspec and dynamic property files.
-        """
-        # fcs_content_with_includes is used to scan only the fcs file and files specifically called with the INCLUDE
-        # token in front of it to prevent it from reading through all the other files. We need this here to extract the
-        # fcs properties only. The FcsFile structure is then generated and stored in the object (with all the nesting of
-        # the NexusFiles as self.model_files (e.g. STRUCTURED_GRID, RUNCONTROL etc)
-        fcs_content_with_includes = NexusFile.generate_file_include_structure(
-            self.__new_fcs_file_path).get_flat_list_str_file
-        self._model_files = FcsNexusFile.generate_fcs_structure(self.__new_fcs_file_path)
-        if fcs_content_with_includes is None:
-            raise ValueError(f'FCS file not found, no content for {self.__new_fcs_file_path}')
-        for line in fcs_content_with_includes:
-            if nfo.check_token('DATEFORMAT', line) or nfo.check_token('DATE_FORMAT', line):
-                format_token = 'DATEFORMAT' if nfo.check_token('DATEFORMAT', line) else 'DATE_FORMAT'
-                value = nfo.get_token_value(format_token, line, fcs_content_with_includes)
-                if value is not None:
-                    self.date_format = DateFormat.DD_MM_YYYY if value == 'DD/MM/YYYY' else DateFormat.MM_DD_YYYY
-
-                self._sim_controls.date_format_string = "%m/%d/%Y" if self.date_format is DateFormat.MM_DD_YYYY \
-                    else "%d/%m/%Y"
-            elif nfo.check_token('RUN_UNITS', line):
-                value = nfo.get_token_value('RUN_UNITS', line, fcs_content_with_includes)
-                if value is not None:
-                    self.__run_units = UnitSystem(value.upper())
-            elif nfo.check_token('DEFAULT_UNITS', line):
-                value = nfo.get_token_value('DEFAULT_UNITS', line, fcs_content_with_includes)
-                if value is not None:
-                    self.__default_units = UnitSystem(value.upper())
-
-        # Load in the other files
-
-        # === Load in dynamic properties ===
-        # Read in PVT properties from Nexus PVT method files
-        if self.model_files.pvt_files is not None and \
-                len(self.model_files.pvt_files) > 0:
-            self._pvt = NexusPVTMethods(files=self.model_files.pvt_files)
-
-        # Read in separator properties from Nexus separator method files
-        if self.model_files.separator_files is not None and \
-                len(self.model_files.separator_files) > 0:
-            self._separator = NexusSeparatorMethods(files=self.model_files.separator_files)
-
-        # Read in water properties from Nexus water method files
-        if self.model_files.water_files is not None and \
-                len(self.model_files.water_files) > 0:
-            self._water = NexusWaterMethods(files=self.model_files.water_files)
-
-        # Read in equilibration properties from Nexus equil method files
-        if self.model_files.equil_files is not None and \
-                len(self.model_files.equil_files) > 0:
-            self._equil = NexusEquilMethods(files=self.model_files.equil_files)
-
-        # Read in rock properties from Nexus rock method files
-        if self.model_files.rock_files is not None and \
-                len(self.model_files.rock_files) > 0:
-            self._rock = NexusRockMethods(files=self.model_files.rock_files)
-
-        # Read in relative permeability and capillary pressure properties from Nexus relperm method files
-        if self.model_files.relperm_files is not None and \
-                len(self.model_files.relperm_files) > 0:
-            self._relperm = NexusRelPermMethods(files=self.model_files.relperm_files)
-
-        # Read in valve and choke properties from Nexus valve method files
-        if self.model_files.valve_files is not None and \
-                len(self.model_files.valve_files) > 0:
-            self._valve = NexusValveMethods(files=self.model_files.valve_files)
-
-        # Read in aquifer properties from Nexus aquifer method files
-        if self.model_files.aquifer_files is not None and \
-                len(self.model_files.aquifer_files) > 0:
-            self._aquifer = NexusAquiferMethods(files=self.model_files.aquifer_files)
-
-        # Read in hydraulics properties from Nexus hyd method files
-        if self.model_files.hyd_files is not None and \
-                len(self.model_files.hyd_files) > 0:
-            self._hydraulics = NexusHydraulicsMethods(files=self.model_files.hyd_files)
-
-        # Read in gaslift properties from Nexus gaslift method files
-        if self.model_files.gas_lift_files is not None and \
-                len(self.model_files.gas_lift_files) > 0:
-            self._gaslift = NexusGasliftMethods(files=self.model_files.gas_lift_files)
-
-        # === End of dynamic properties loading ===
-
-        # Load in Runcontrol
-        if self.model_files.runcontrol_file is not None:
-            self.run_control_file_path = self.model_files.runcontrol_file.location
-            self._sim_controls.load_run_control_file()
-
-        if self.model_files.structured_grid_file is not None:
-            self._grid = NexusGrid.load_structured_grid_file(self.model_files.structured_grid_file,
-                                                             lazy_loading=self.__lazy_loading)
-
-        # Load in wellspec files
-        if self.model_files.well_files is not None and \
-                len(self.model_files.well_files) > 0:
-            for well_file in self.model_files.well_files.values():
-                if well_file.location is None:
-                    warnings.warn(f'Well file location has not been found for {well_file}')
-                    continue
-
-    @staticmethod
-    def update_file_value(file_path: str, token: str, new_value: str, add_to_start: bool = False) -> None:
-        """Updates a value in a file if it is present and in the format {TOKEN} {VALUE}. If the token
-        isn't present, it will add the token + value to either the start or end of the file.
-
-        Args:
-            file_path (str): path to a file to update the token/value pair in
-            token (str): Keyword token to find in the given file (e.g. KX)
-            new_value (str): Value following the TOKEN to be replaced
-            add_to_start (bool, optional): Inserts the token/value pair to the start of the file. Defaults to False.
-
-        Raises:
-            ValueError: If no value is found after the token
-        """
-
-        file = nfo.load_file_as_list(file_path)
-
-        line_counter = 0
-        token_found = False
-        for line in file:
-            modified_line = line.lower().replace('/t', ' ')
-            modified_line = ' '.join(modified_line.split())
-            if token.lower() in modified_line:
-                # We've found the token, now replace the value
-                token_location = modified_line.find(token.lower())
-                line_before_token_value = line[0: token_location]
-                line_after_token = line[token_location:]
-                current_value = nfo.get_next_value(0, [line], line_after_token[len(token) + 1:])
-                if current_value is None:
-                    raise ValueError(f"No value found after the supplied {token=}, \
-                        please check the following line for that token: {line}")
-                new_line_after = line_after_token.replace(
-                    current_value, new_value, 1)
-                file[line_counter] = line_before_token_value + new_line_after
-                token_found = True
-                break
-            line_counter += 1
-
-        if token_found is False:
-            token_line = f"{token} {new_value}"
-            if add_to_start:
-                file.insert(0, token_line + '\n')
-            else:
-                file.append('\n' + token_line)
-
-        new_file_str = "".join(file)
-
-        with open(file_path, "w") as text_file:
-            text_file.write(new_file_str)
-
-    def update_fcs_file_value(self, token, new_value, add_to_start=False):
-        """Updates a value in the FCS file."""
-        self.update_file_value(self.__new_fcs_file_path, token=token, new_value=new_value, add_to_start=add_to_start)
-
-    @staticmethod
-    def comment_out_file_value(token: str, file_path: str) -> None:
-        """Comments out an uncommented line containing the specified token.
-
-        Args:
-            token (str): Keyword token to find in the given file (e.g. KX)
-            file_path (str): path to a file containing the token
-        """
-        file = nfo.load_file_as_list(file_path)
-
-        line_counter = 0
-        for line in file:
-            modified_line = line.lower().replace('/t', ' ')
-            modified_line = ' '.join(modified_line.split())
-            # If we've found the token, and it isn't already commented, comment it out
-            if token.lower() in modified_line and \
-                    (modified_line.find(token.lower()) < modified_line.find("!") or modified_line.find("!") == -1):
-                file[line_counter] = f"! {file[line_counter]}"
-                break
-            line_counter += 1
-
-        new_file_str = "".join(file)
-
-        with open(file_path, "w") as text_file:
-            text_file.write(new_file_str)
-
-    def get_date_format(self) -> str:
-        """Returns the date format being used by the model
-        formats used: ('MM/DD/YYYY', 'DD/MM/YYYY').
-        """
-        return self._sim_controls.get_date_format(self.date_format)
-
-    def modify(self, operation: str, section: str, keyword: str, content: list[str]):
-        """Generic modify method to modify part of the input deck. \
-        Operations are dependent on the section being modified.
-
-        Args:
-            operation (str): operation to perform on the section of the input deck (e.g. 'merge')
-            section (str): file type from the input deck provided (e.g. RUNCONTROL)
-            keyword (str): which keyword/token to find within the deck provided (e.g. TIME)
-            content (list[str]): The content to modify using the above operation, \
-            represented as a list of strings with a new entry per line of the file
-
-        Raises:
-            NotImplementedError: if the functionality is not yet implemented
-        """
-        section = section.upper()
-        keyword = keyword.upper()
-        operation = operation.lower()
-
-        if section == "RUNCONTROL":
-            if keyword == "TIME":
-                self._sim_controls.modify_times(content=content, operation=operation)
-            else:
-                raise NotImplementedError(keyword, "not yet implemented")
-        else:
-            raise NotImplementedError(section, "not yet implemented")
-
-    def get_content(self, section: str, keyword: str) -> Union[list[str], None]:
-        """Returns the requested input information.
-
-        Args:
-            section (str): Section to retreive information from
-            keyword (str): Keyword/token to retrieve the information for
-
-        Raises:
-            NotImplementedError: if the functionality is not yet implemented
-
-        Returns:
-            Union[list[str], None]: the requested information
-        """
-        section = section.upper()
-        keyword = keyword.upper()
-        if section == "RUNCONTROL":
-            if keyword == "TIME":
-                return self._sim_controls.times
-            else:
-                raise NotImplementedError(keyword, "not yet implemented")
-        else:
-            raise NotImplementedError(section, "not yet implemented")
-
-    def get_structured_grid_dict(self) -> dict[str, Any]:
-        """Convert the structured grid info to a dictionary and pass it to the front end."""
-        if self._grid is None:
-            return {}
-        return self._grid.to_dict()
-
-    def get_abs_structured_grid_path(self, filename: str):
-        """Returns the absolute path to the Structured Grid file."""
-        if self.model_files.structured_grid_file is None:
-            raise ValueError(
-                f"No structured grid file found within simulator class: {self.model_files.structured_grid_file}")
-        grid_path = self.model_files.structured_grid_file.location
-        if grid_path is None:
-            raise ValueError("No path found for structured grid file path. \
-                Please provide a path to the structured grid")
-        return os.path.dirname(grid_path) + '/' + filename
-
-    def get_surface_file_path(self):
-        """Get the surface file path."""
-        if self.model_files.surface_files is None or self.model_files.surface_files[1] is None:
-            raise ValueError('No path found for surface file.')
-        return self.model_files.surface_files[1].location
-
-    def load_network(self):
-        """Populates nodes and connections from a surface file."""
-        self._network.load()
+from __future__ import annotations
+
+import os
+import warnings
+from typing import Any, Union, Optional
+
+import resqpy.model as rq
+from datetime import datetime
+import ResSimpy.Nexus.nexus_file_operations as nfo
+from ResSimpy.Nexus.DataModels.FcsFile import FcsNexusFile
+from ResSimpy.Nexus.DataModels.NexusFile import NexusFile
+from ResSimpy.Nexus.NexusPVTMethods import NexusPVTMethods
+from ResSimpy.Nexus.NexusSeparatorMethods import NexusSeparatorMethods
+from ResSimpy.Nexus.NexusWaterMethods import NexusWaterMethods
+from ResSimpy.Nexus.NexusEquilMethods import NexusEquilMethods
+from ResSimpy.Nexus.NexusRockMethods import NexusRockMethods
+from ResSimpy.Nexus.NexusRelPermMethods import NexusRelPermMethods
+from ResSimpy.Nexus.NexusValveMethods import NexusValveMethods
+from ResSimpy.Nexus.NexusAquiferMethods import NexusAquiferMethods
+from ResSimpy.Nexus.NexusHydraulicsMethods import NexusHydraulicsMethods
+from ResSimpy.Nexus.NexusGasliftMethods import NexusGasliftMethods
+from ResSimpy.Nexus.DataModels.StructuredGrid.NexusGrid import NexusGrid
+from ResSimpy.Nexus.NexusEnums.DateFormatEnum import DateFormat
+from ResSimpy.Enums.UnitsEnum import UnitSystem
+from ResSimpy.Nexus.NexusNetwork import NexusNetwork
+from ResSimpy.Nexus.NexusReporting import Reporting
+from ResSimpy.Nexus.NexusWells import NexusWells
+from ResSimpy.Nexus.runcontrol_operations import SimControls
+from ResSimpy.Nexus.logfile_operations import Logging
+from ResSimpy.Nexus.structured_grid_operations import StructuredGridOperations
+from ResSimpy.Simulator import Simulator
+
+
+class NexusSimulator(Simulator):
+
+    def __init__(self, origin: Optional[str] = None, destination: Optional[str] = None,
+                 root_name: Optional[str] = None, nexus_data_name: str = "data", write_times: bool = False,
+                 manual_fcs_tidy_call: bool = False, lazy_loading: bool = True) -> None:
+        """Nexus simulator class. Inherits from the Simulator super class.
+
+        Args:
+            origin (Optional[str], optional): file path to the fcs file. Defaults to None.
+            root_name (Optional[str], optional): Root file name of the fcs. Defaults to None.
+            nexus_data_name (str, optional): Folder name for the nexus data files to be stored in. Defaults to "data".
+            write_times (bool, optional): Sets whether the runcontrol file will expand the include files with time \
+                cards in. Defaults to True.
+            manual_fcs_tidy_call (bool, optional): Determines whether fcs_tidy should be called - Currently not used. \
+                Defaults to False.
+
+        Attributes:
+            run_control_file_path (Optional[str]): file path to the run control file - derived from the fcs file
+            __destination (Optional[str]): output path for the simulation. Currently not used.
+            date_format (DateFormat): Enum value representing the date format.
+            __original_fcs_file_path (str): Path to the original fcs file path supplied
+            __new_fcs_file_path (str): Where the new fcs will be saved to
+            __force_output (bool): private attribute of force_output
+            __origin (str): private attribute of origin. File path to the fcs file.
+            __root_name (str): private attribute of root_name. Root file name of the fcs.
+            __nexus_data_name (str): private attribute of nexus_data_name. Folder name for the nexus data files to be \
+                stored in.
+            __structured_grid_file_path (Optional[str]): file path to the structured grid.
+            __structured_grid_file (Optional[NexusGrid]): StructuredGridFile object representing the \
+                structured grid used in Nexus
+            __run_units (Optional[str]): Unit system used in the Nexus model
+            use_american_run_units (bool): True if an American unit system is used equivalent to 'ENGLISH'. \
+                False otherwise. For the RUN_UNITS keyword.
+            use_american_input_units (bool): True if an American unit system is used equivalent to 'ENGLISH'. \
+                False otherwise. For the DEFAULT_UNITS keyword.
+            __write_times (bool): private attribute for write_times. Sets whether the runcontrol file will expand \
+                the include files with time cards in.
+            __manual_fcs_tidy_call (bool): private attribute for manual_fcs_tidy_call. Determines whether fcs_tidy \
+                should be called
+
+        Raises:
+            ValueError: If the FCS file path is not given
+        """
+        if origin is None:
+            raise ValueError(f'Origin path to model fcs file is required. Instead got {origin}.')
+        self.origin: str = origin
+
+        self._start_date: str = ''
+        self.run_control_file_path: Optional[str] = ''
+        self.__destination: Optional[str] = None
+        self.date_format: DateFormat = DateFormat.MM_DD_YYYY  # Nexus default
+        self.__original_fcs_file_path: str = self.origin
+        self.__new_fcs_file_path: str = self.origin
+        self.__nexus_data_name: str = nexus_data_name
+        self.__run_units: UnitSystem = UnitSystem.ENGLISH  # The Nexus default
+        self.root_name: str = root_name
+        self.use_american_run_units: bool = False
+        self.use_american_input_units: bool = False
+        self.__write_times: bool = write_times
+        self.__manual_fcs_tidy_call: bool = manual_fcs_tidy_call
+
+        self.__default_units: UnitSystem = UnitSystem.ENGLISH  # The Nexus default
+        #
+        self._wells: NexusWells = NexusWells(self)
+        self._grid: Optional[NexusGrid] = None
+        self._network: NexusNetwork = NexusNetwork(model=self)
+        # Model dynamic properties
+        self._pvt: NexusPVTMethods = NexusPVTMethods()
+        self._separator: NexusSeparatorMethods = NexusSeparatorMethods()
+        self._water: NexusWaterMethods = NexusWaterMethods()
+        self._equil: NexusEquilMethods = NexusEquilMethods()
+        self._rock: NexusRockMethods = NexusRockMethods()
+        self._relperm: NexusRelPermMethods = NexusRelPermMethods()
+        self._valve: NexusValveMethods = NexusValveMethods()
+        self._aquifer: NexusAquiferMethods = NexusAquiferMethods()
+        self._hydraulics: NexusHydraulicsMethods = NexusHydraulicsMethods()
+        self._gaslift: NexusGasliftMethods = NexusGasliftMethods()
+        # Nexus operations modules
+        self._sim_controls: SimControls = SimControls(self)
+        self.reporting: Reporting = Reporting(self)
+        self._structured_grid_operations: StructuredGridOperations = StructuredGridOperations(self)
+        self.logging: Logging = Logging(self)
+        self.__lazy_loading: bool = lazy_loading
+
+        if destination is not None and destination != '':
+            self.set_output_path(path=destination.strip())
+
+        # Check the status of any existing or completed runs related to this model
+        self.get_simulation_status(from_startup=True)
+
+        self._model_files: FcsNexusFile
+        # Load in the model
+        self.__load_fcs_file()
+
+    def remove_temp_from_properties(self):
+        """Updates model values if the files are moved from a temp directory
+        Replaces the first instance of temp/ in the file paths in the nexus simulation file paths.
+
+        Raises:
+            ValueError: if any of [__structured_grid_file_path, __new_fcs_file_path, __surface_file_path] are None.
+        """
+        if self.model_files.structured_grid_file.location is None:
+            raise ValueError(
+                "No structured_grid_file_path found, can't remove temporary properties from file path")
+        if self.__new_fcs_file_path is None:
+            raise ValueError(
+                "No __new_fcs_file_path found, can't remove temporary properties from file path")
+        if self.model_files.surface_files[1] is None or self.model_files.surface_files[1].location is None:
+            raise ValueError(
+                "No __surface_file_path found, can't remove temporary properties from file path")
+
+        self._origin = self._origin.replace('temp/', '', 1)
+        self.__root_name = self.__root_name.replace('temp/', '', 1)
+        self.model_files.structured_grid_file.location = \
+            self.model_files.structured_grid_file.location.replace('temp/', '', 1)
+        self.__new_fcs_file_path = self.__new_fcs_file_path.replace('temp/', '', 1)
+        self.model_files.surface_files[1].location = self.model_files.surface_files[1].location.replace('temp/', '', 1)
+
+    def get_simulation_status(self, from_startup: bool = False) -> Optional[str]:
+        return self.logging.get_simulation_status(from_startup)
+
+    def get_simulation_progress(self) -> float:
+        return self.logging.get_simulation_progress()
+
+    def get_users_linked_with_files(self) -> Optional[list[tuple[Optional[str], Optional[str], Optional[datetime]]]]:
+        return self.model_files.files_info
+
+    @property
+    def model_files(self) -> FcsNexusFile:
+        return self._model_files
+
+    @property
+    def structured_grid_path(self):
+        """Returns the location of the structured grid file."""
+        return self.model_files.structured_grid_file.location
+
+    @property
+    def default_units(self):
+        """Returns the default units."""
+        return self.__default_units
+
+    @property
+    def run_units(self):
+        """Returns the run units."""
+        return self.__run_units
+
+    @property
+    def new_fcs_name(self):
+        """Returns the new name for the FCS file without the fcs extension."""
+        return self.__root_name
+
+    @property
+    def write_times(self) -> bool:
+        return self.__write_times
+
+    @property
+    def original_fcs_file_path(self):
+        return self.__original_fcs_file_path
+
+    @property
+    def root_name(self):
+        return self.__root_name
+
+    @root_name.setter
+    def root_name(self, value: str) -> None:
+        """Returns the name of the fcs file without the .fcs extension.
+
+        Returns:
+            str: string of the fcs file without the .fcs extension.
+        """
+        if value is not None:
+            rootname = value
+        else:
+            rootname = os.path.basename(self._origin)
+            rootname = rootname.split(".fcs")[0]
+        self.__root_name = rootname
+
+    @staticmethod
+    def get_check_run_input_units_for_models(models: list[str]) -> tuple[Optional[bool], Optional[bool]]:
+        # TODO: add LAB units
+        """Returns the run and input unit formats for all the supplied models.
+
+        Supported model formats:
+            RESQML type epc files ending in ".epc"
+            Nexus files containing a line identifying the "RUN_UNITS" or "DEFAULT_UNITS".
+
+        Supported units: ENGLISH, METRIC
+
+        Args:
+            models (list[str]): list of paths to supported reservoir models
+
+        Raises:
+            ValueError: if a model in the list is using inconcistent run/default units
+
+        Returns:
+            Tuple[Optional[Bool], Optional[Bool]]: If all units are consistent between models,
+                Returns (True, True) if 'ft' is the length unit in an epc or Nexus specifies "ENGLISH" as the
+                (RUN_UNITS,DEFAULT_UNITS) respectively and False, False otherwise.
+                Returns (None, None) if it can't find a (RUN_UNITS, DEFAULT_UNITS) in the supplied files.
+        """
+        oilfield_run_units: Optional[bool] = None
+        oilfield_default_units: Optional[bool] = None
+
+        for model in models:
+            # If we're checking the units of a RESQML model, read it in and get the units. Otherwise, read the units
+            # from the fcs file
+            if os.path.splitext(model)[1] == '.epc':
+                resqpy_model = rq.Model(epc_file=model)
+
+                # Load in the RESQML grid
+                grid = resqpy_model.grid()
+
+                # Check the grid units
+                grid_length_unit = grid.xy_units()
+                model_oilfield_default_units = grid_length_unit == 'ft'
+                model_oilfield_run_units = grid_length_unit == 'ft'
+            else:
+                simulator = NexusSimulator(origin=model)
+                model_oilfield_default_units = simulator.default_units == UnitSystem.ENGLISH
+                model_oilfield_run_units = simulator.run_units == UnitSystem.ENGLISH
+
+            # If not defined, assign it to model_oilfield_default_units
+            if oilfield_default_units is None:
+                oilfield_default_units = model_oilfield_default_units
+            # Raise ValueError if default units are inconsistent with the other models
+            elif model_oilfield_default_units != oilfield_default_units:
+                raise ValueError(f"Model at {model} using inconsistent default units")
+
+            # If not defined, assign it to model_oilfield_run_units
+            if oilfield_run_units is None:
+                oilfield_run_units = model_oilfield_run_units
+            # Raise ValueError if run units are inconsistent with the other models
+            elif model_oilfield_run_units != oilfield_run_units:
+                raise ValueError(f"Model at {model} using inconsistent run units")
+
+        return oilfield_run_units, oilfield_default_units
+
+    @staticmethod
+    def get_check_oil_gas_types_for_models(models: list[str]) -> Optional[str]:
+        """Checks for fluid types within a list of paths to models.
+        Currently limited to checking for the first SURFACE network in a file.
+
+        Args:
+            models (list[str]): a list of paths to models to check for fluid types.
+
+        Raises:
+            ValueError: If fluid types are inconsistent between models
+
+        Returns:
+            Optional[str]: The fluid type used for the model for the first surface network
+        """
+        fluid_type = None
+        for model in models:
+            model_fluid_type = None
+            fcs_file = NexusFile.generate_file_include_structure(model).get_flat_list_str_file
+            surface_filename = None
+            if fcs_file is None:
+                warnings.warn(UserWarning(f'No file found for {model}'))
+                continue
+            for line in fcs_file:
+                if nfo.check_token("SURFACE Network 1", line):
+                    surface_filename = nfo.get_expected_token_value(token="SURFACE Network 1", token_line=line,
+                                                                    file_list=fcs_file)
+                    break
+
+            if surface_filename is not None:
+                surface_filename = surface_filename if os.path.isabs(surface_filename) else \
+                    os.path.dirname(model) + "/" + surface_filename
+                model_fluid_type = NexusSimulator.get_fluid_type(
+                    surface_file_name=surface_filename)
+
+            if fluid_type is None:
+                fluid_type = model_fluid_type
+            elif fluid_type != model_fluid_type:
+                raise ValueError(
+                    f"Inconsistent Oil / Gas types: {model_fluid_type} found for {model}")
+
+        return fluid_type
+
+    @staticmethod
+    def get_eos_details(surface_file: list[str]) -> str:
+        """Gets all the information about an EOS from a Nexus model.
+
+        Args:
+            surface_file (list[str]): path to the surface file in a Nexus model
+
+        Returns:
+            str: a concatenated string of EOS components
+        """
+        eos_string: str = ''
+        eos_found: bool = False
+        for line in surface_file:
+            if nfo.check_token("EOS", line):
+                eos_string += line
+                eos_found = True
+            elif eos_found:
+                eos_string += line
+            if nfo.check_token("COMPONENTS", line):
+                break
+
+        return eos_string
+
+    @staticmethod
+    def get_fluid_type(surface_file_name: str) -> str:
+        """Gets the fluid type for a single model from a surface file.
+
+        Args:
+            surface_file_name (str): path to the surface file in a Nexus model
+
+        Raises:
+            ValueError: if no fluid type is found within the provided file path
+
+        Returns:
+            str: fluid type as one of [BLACKOIL, WATEROIL, GASWATER,] or the full details from an EOS model
+        """
+        surface_file = nfo.load_file_as_list(surface_file_name)
+        fluid_type = None
+
+        for line in surface_file:
+            if nfo.check_token("BLACKOIL", line):
+                fluid_type = "BLACKOIL"
+                break
+            elif nfo.check_token("WATEROIL", line):
+                fluid_type = "WATEROIL"
+                break
+            elif nfo.check_token("GASWATER", line):
+                fluid_type = "GASWATER"
+                break
+            elif nfo.check_token("EOS", line):
+                fluid_type = NexusSimulator.get_eos_details(surface_file)
+
+        if fluid_type is None:
+            raise ValueError("No Oil / Gas type detected")
+
+        return fluid_type
+
+    def get_model_oil_type(self) -> str:
+        """Returns the get_fluid_type method on the existing NexusSimulator instance.
+
+        Raises:
+            ValueError: If no file path is provided for the surface file path
+
+        Returns:
+            str: fluid type as one of [BLACKOIL, WATEROIL, GASWATER,] or the full details from an EOS model
+        """
+        if self.model_files.surface_files is None or self.model_files.surface_files[1].location is None:
+            raise ValueError("No value found for the path to the surface file")
+        return NexusSimulator.get_fluid_type(self.model_files.surface_files[1].location)
+
+    def check_output_path(self) -> None:
+        """Confirms that the output path has been set (used to stop accidental writing operations in the original
+        directory).
+
+        Raises:
+            ValueError: if the destination provided is set to None.
+        """
+        if self.__destination is None:
+            raise ValueError("Destination is required for this operation. Currently set to: ", self.__destination)
+
+    @property
+    def destination(self) -> Optional[str]:
+        return self.__destination
+
+    def set_output_path(self, path: str) -> None:
+        """Initialises the output to the declared output location.
+        If the file is a different directory to the origin path location the function will set the origin
+        to the new destination.
+        """
+        self.__destination = path
+        if self.__destination is not None and os.path.dirname(self._origin) != os.path.dirname(self.__destination):
+            self._origin = self.__destination + "/" + os.path.basename(self.__original_fcs_file_path)
+
+    def __load_fcs_file(self):
+        """Loads in the information from the supplied FCS file into the class instance.
+        Loads in the paths for runcontrol, structured grid and the first surface network.
+        Loads in the values for dateformat and run units.
+        Attempts to load the run_control_file.
+        Loads the wellspec and dynamic property files.
+        """
+        # fcs_content_with_includes is used to scan only the fcs file and files specifically called with the INCLUDE
+        # token in front of it to prevent it from reading through all the other files. We need this here to extract the
+        # fcs properties only. The FcsFile structure is then generated and stored in the object (with all the nesting of
+        # the NexusFiles as self.model_files (e.g. STRUCTURED_GRID, RUNCONTROL etc)
+        fcs_content_with_includes = NexusFile.generate_file_include_structure(
+            self.__new_fcs_file_path).get_flat_list_str_file
+        self._model_files = FcsNexusFile.generate_fcs_structure(self.__new_fcs_file_path)
+        if fcs_content_with_includes is None:
+            raise ValueError(f'FCS file not found, no content for {self.__new_fcs_file_path}')
+        for line in fcs_content_with_includes:
+            if nfo.check_token('DATEFORMAT', line) or nfo.check_token('DATE_FORMAT', line):
+                format_token = 'DATEFORMAT' if nfo.check_token('DATEFORMAT', line) else 'DATE_FORMAT'
+                value = nfo.get_token_value(format_token, line, fcs_content_with_includes)
+                if value is not None:
+                    self.date_format = DateFormat.DD_MM_YYYY if value == 'DD/MM/YYYY' else DateFormat.MM_DD_YYYY
+
+                self._sim_controls.date_format_string = "%m/%d/%Y" if self.date_format is DateFormat.MM_DD_YYYY \
+                    else "%d/%m/%Y"
+            elif nfo.check_token('RUN_UNITS', line):
+                value = nfo.get_token_value('RUN_UNITS', line, fcs_content_with_includes)
+                if value is not None:
+                    self.__run_units = UnitSystem(value.upper())
+            elif nfo.check_token('DEFAULT_UNITS', line):
+                value = nfo.get_token_value('DEFAULT_UNITS', line, fcs_content_with_includes)
+                if value is not None:
+                    self.__default_units = UnitSystem(value.upper())
+
+        # Load in the other files
+
+        # === Load in dynamic properties ===
+        # Read in PVT properties from Nexus PVT method files
+        if self.model_files.pvt_files is not None and \
+                len(self.model_files.pvt_files) > 0:
+            self._pvt = NexusPVTMethods(files=self.model_files.pvt_files)
+
+        # Read in separator properties from Nexus separator method files
+        if self.model_files.separator_files is not None and \
+                len(self.model_files.separator_files) > 0:
+            self._separator = NexusSeparatorMethods(files=self.model_files.separator_files)
+
+        # Read in water properties from Nexus water method files
+        if self.model_files.water_files is not None and \
+                len(self.model_files.water_files) > 0:
+            self._water = NexusWaterMethods(files=self.model_files.water_files)
+
+        # Read in equilibration properties from Nexus equil method files
+        if self.model_files.equil_files is not None and \
+                len(self.model_files.equil_files) > 0:
+            self._equil = NexusEquilMethods(files=self.model_files.equil_files)
+
+        # Read in rock properties from Nexus rock method files
+        if self.model_files.rock_files is not None and \
+                len(self.model_files.rock_files) > 0:
+            self._rock = NexusRockMethods(files=self.model_files.rock_files)
+
+        # Read in relative permeability and capillary pressure properties from Nexus relperm method files
+        if self.model_files.relperm_files is not None and \
+                len(self.model_files.relperm_files) > 0:
+            self._relperm = NexusRelPermMethods(files=self.model_files.relperm_files)
+
+        # Read in valve and choke properties from Nexus valve method files
+        if self.model_files.valve_files is not None and \
+                len(self.model_files.valve_files) > 0:
+            self._valve = NexusValveMethods(files=self.model_files.valve_files)
+
+        # Read in aquifer properties from Nexus aquifer method files
+        if self.model_files.aquifer_files is not None and \
+                len(self.model_files.aquifer_files) > 0:
+            self._aquifer = NexusAquiferMethods(files=self.model_files.aquifer_files)
+
+        # Read in hydraulics properties from Nexus hyd method files
+        if self.model_files.hyd_files is not None and \
+                len(self.model_files.hyd_files) > 0:
+            self._hydraulics = NexusHydraulicsMethods(files=self.model_files.hyd_files)
+
+        # Read in gaslift properties from Nexus gaslift method files
+        if self.model_files.gas_lift_files is not None and \
+                len(self.model_files.gas_lift_files) > 0:
+            self._gaslift = NexusGasliftMethods(files=self.model_files.gas_lift_files)
+
+        # === End of dynamic properties loading ===
+
+        # Load in Runcontrol
+        if self.model_files.runcontrol_file is not None:
+            self.run_control_file_path = self.model_files.runcontrol_file.location
+            self._sim_controls.load_run_control_file()
+
+        if self.model_files.structured_grid_file is not None:
+            self._grid = NexusGrid.load_structured_grid_file(self.model_files.structured_grid_file,
+                                                             lazy_loading=self.__lazy_loading)
+
+        # Load in wellspec files
+        if self.model_files.well_files is not None and \
+                len(self.model_files.well_files) > 0:
+            for well_file in self.model_files.well_files.values():
+                if well_file.location is None:
+                    warnings.warn(f'Well file location has not been found for {well_file}')
+                    continue
+
+    @staticmethod
+    def update_file_value(file_path: str, token: str, new_value: str, add_to_start: bool = False) -> None:
+        """Updates a value in a file if it is present and in the format {TOKEN} {VALUE}. If the token
+        isn't present, it will add the token + value to either the start or end of the file.
+
+        Args:
+            file_path (str): path to a file to update the token/value pair in
+            token (str): Keyword token to find in the given file (e.g. KX)
+            new_value (str): Value following the TOKEN to be replaced
+            add_to_start (bool, optional): Inserts the token/value pair to the start of the file. Defaults to False.
+
+        Raises:
+            ValueError: If no value is found after the token
+        """
+
+        file = nfo.load_file_as_list(file_path)
+
+        line_counter = 0
+        token_found = False
+        for line in file:
+            modified_line = line.lower().replace('/t', ' ')
+            modified_line = ' '.join(modified_line.split())
+            if token.lower() in modified_line:
+                # We've found the token, now replace the value
+                token_location = modified_line.find(token.lower())
+                line_before_token_value = line[0: token_location]
+                line_after_token = line[token_location:]
+                current_value = nfo.get_next_value(0, [line], line_after_token[len(token) + 1:])
+                if current_value is None:
+                    raise ValueError(f"No value found after the supplied {token=}, \
+                        please check the following line for that token: {line}")
+                new_line_after = line_after_token.replace(
+                    current_value, new_value, 1)
+                file[line_counter] = line_before_token_value + new_line_after
+                token_found = True
+                break
+            line_counter += 1
+
+        if token_found is False:
+            token_line = f"{token} {new_value}"
+            if add_to_start:
+                file.insert(0, token_line + '\n')
+            else:
+                file.append('\n' + token_line)
+
+        new_file_str = "".join(file)
+
+        with open(file_path, "w") as text_file:
+            text_file.write(new_file_str)
+
+    def update_fcs_file_value(self, token, new_value, add_to_start=False):
+        """Updates a value in the FCS file."""
+        self.update_file_value(self.__new_fcs_file_path, token=token, new_value=new_value, add_to_start=add_to_start)
+
+    @staticmethod
+    def comment_out_file_value(token: str, file_path: str) -> None:
+        """Comments out an uncommented line containing the specified token.
+
+        Args:
+            token (str): Keyword token to find in the given file (e.g. KX)
+            file_path (str): path to a file containing the token
+        """
+        file = nfo.load_file_as_list(file_path)
+
+        line_counter = 0
+        for line in file:
+            modified_line = line.lower().replace('/t', ' ')
+            modified_line = ' '.join(modified_line.split())
+            # If we've found the token, and it isn't already commented, comment it out
+            if token.lower() in modified_line and \
+                    (modified_line.find(token.lower()) < modified_line.find("!") or modified_line.find("!") == -1):
+                file[line_counter] = f"! {file[line_counter]}"
+                break
+            line_counter += 1
+
+        new_file_str = "".join(file)
+
+        with open(file_path, "w") as text_file:
+            text_file.write(new_file_str)
+
+    def get_date_format(self) -> str:
+        """Returns the date format being used by the model
+        formats used: ('MM/DD/YYYY', 'DD/MM/YYYY').
+        """
+        return self._sim_controls.get_date_format(self.date_format)
+
+    def modify(self, operation: str, section: str, keyword: str, content: list[str]):
+        """Generic modify method to modify part of the input deck. \
+        Operations are dependent on the section being modified.
+
+        Args:
+            operation (str): operation to perform on the section of the input deck (e.g. 'merge')
+            section (str): file type from the input deck provided (e.g. RUNCONTROL)
+            keyword (str): which keyword/token to find within the deck provided (e.g. TIME)
+            content (list[str]): The content to modify using the above operation, \
+            represented as a list of strings with a new entry per line of the file
+
+        Raises:
+            NotImplementedError: if the functionality is not yet implemented
+        """
+        section = section.upper()
+        keyword = keyword.upper()
+        operation = operation.lower()
+
+        if section == "RUNCONTROL":
+            if keyword == "TIME":
+                self._sim_controls.modify_times(content=content, operation=operation)
+            else:
+                raise NotImplementedError(keyword, "not yet implemented")
+        else:
+            raise NotImplementedError(section, "not yet implemented")
+
+    def get_content(self, section: str, keyword: str) -> Union[list[str], None]:
+        """Returns the requested input information.
+
+        Args:
+            section (str): Section to retreive information from
+            keyword (str): Keyword/token to retrieve the information for
+
+        Raises:
+            NotImplementedError: if the functionality is not yet implemented
+
+        Returns:
+            Union[list[str], None]: the requested information
+        """
+        section = section.upper()
+        keyword = keyword.upper()
+        if section == "RUNCONTROL":
+            if keyword == "TIME":
+                return self._sim_controls.times
+            else:
+                raise NotImplementedError(keyword, "not yet implemented")
+        else:
+            raise NotImplementedError(section, "not yet implemented")
+
+    def get_structured_grid_dict(self) -> dict[str, Any]:
+        """Convert the structured grid info to a dictionary and pass it to the front end."""
+        if self._grid is None:
+            return {}
+        return self._grid.to_dict()
+
+    def get_abs_structured_grid_path(self, filename: str):
+        """Returns the absolute path to the Structured Grid file."""
+        if self.model_files.structured_grid_file is None:
+            raise ValueError(
+                f"No structured grid file found within simulator class: {self.model_files.structured_grid_file}")
+        grid_path = self.model_files.structured_grid_file.location
+        if grid_path is None:
+            raise ValueError("No path found for structured grid file path. \
+                Please provide a path to the structured grid")
+        return os.path.dirname(grid_path) + '/' + filename
+
+    def get_surface_file_path(self):
+        """Get the surface file path."""
+        if self.model_files.surface_files is None or self.model_files.surface_files[1] is None:
+            raise ValueError('No path found for surface file.')
+        return self.model_files.surface_files[1].location
+
+    def load_network(self):
+        """Populates nodes and connections from a surface file."""
+        self._network.load()
```

### Comparing `ressimpy-1.0.0/ResSimpy/Nexus/NexusValveMethods.py` & `ressimpy-1.0.1/ResSimpy/Nexus/NexusRockMethods.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,69 +1,69 @@
-from dataclasses import dataclass
-import os
-from typing import Optional, MutableMapping
-from ResSimpy.Nexus.DataModels.NexusFile import NexusFile
-from ResSimpy.Nexus.DataModels.NexusValveMethod import NexusValveMethod
-from ResSimpy.Valve import Valve
-
-
-@dataclass(kw_only=True)
-class NexusValveMethods(Valve):
-    """Class for collection of Nexus valve property inputs.
-
-    Attributes:
-        inputs (dict[int, NexusValveMethod]): Collection of Nexus valve property methods, as a dictionary
-        files (dict[int, NexusFile]): Dictionary collection of valve property files, as defined in Nexus fcs file.
-    """
-
-    __inputs: MutableMapping[int, NexusValveMethod]
-    __files: dict[int, NexusFile]
-    __properties_loaded: bool = False  # Used in lazy loading
-
-    def __init__(self, inputs: Optional[MutableMapping[int, NexusValveMethod]] = None,
-                 files: Optional[dict[int, NexusFile]] = None) -> None:
-        if inputs:
-            self.__inputs = inputs
-        else:
-            self.__inputs: MutableMapping[int, NexusValveMethod] = {}
-        if files:
-            self.__files = files
-        else:
-            self.__files = {}
-        super().__init__()
-
-    def __repr__(self) -> str:
-        """Pretty printing valve methods."""
-        if not self.__properties_loaded:
-            self.load_valve_methods()
-        printable_str = ''
-        for table_num in self.__inputs.keys():
-            printable_str += '\n--------------------------------\n'
-            printable_str += f'VALVE method {table_num}\n'
-            printable_str += '--------------------------------\n'
-            printable_str += self.__inputs[table_num].__repr__()
-            printable_str += '\n'
-
-        return printable_str
-
-    @property
-    def inputs(self) -> MutableMapping[int, NexusValveMethod]:
-        if not self.__properties_loaded:
-            self.load_valve_methods()
-        return self.__inputs
-
-    @property
-    def valve_files(self) -> dict[int, NexusFile]:
-        return self.__files
-
-    def load_valve_methods(self):
-        # Read in valve properties from Nexus valve method files
-        if self.__files is not None and len(self.__files) > 0:  # Check if valve files exist
-            for table_num in self.__files.keys():  # For each valve property method
-                valve_file = self.__files[table_num]
-                if valve_file.location is None:
-                    raise ValueError(f'Unable to find valve file: {valve_file}')
-                if os.path.isfile(valve_file.location):
-                    # Create NexusValveMethod object
-                    self.__inputs[table_num] = NexusValveMethod(file=valve_file, input_number=table_num)
-                    self.__inputs[table_num].read_properties()  # Populate object with valve properties in file
-        self.__properties_loaded = True
+from dataclasses import dataclass
+import os
+from typing import Optional, MutableMapping
+from ResSimpy.Nexus.DataModels.NexusFile import NexusFile
+from ResSimpy.Nexus.DataModels.NexusRockMethod import NexusRockMethod
+from ResSimpy.Rock import Rock
+
+
+@dataclass(kw_only=True)
+class NexusRockMethods(Rock):
+    """Class for collection of Nexus rock property methods.
+
+    Attributes:
+        inputs (dict[int, NexusRockMethod]): Collection of Nexus rock property methods, as a dictionary
+        files (dict[int, NexusFile]): Dictionary collection of rock property files, as defined in Nexus fcs file.
+    """
+
+    __inputs: MutableMapping[int, NexusRockMethod]
+    __files: dict[int, NexusFile]
+    __properties_loaded: bool = False  # Used in lazy loading
+
+    def __init__(self, inputs: Optional[MutableMapping[int, NexusRockMethod]] = None,
+                 files: Optional[dict[int, NexusFile]] = None) -> None:
+        if inputs:
+            self.__inputs = inputs
+        else:
+            self.__inputs: MutableMapping[int, NexusRockMethod] = {}
+        if files:
+            self.__files = files
+        else:
+            self.__files = {}
+        super().__init__()
+
+    def __repr__(self) -> str:
+        """Pretty printing rock methods."""
+        if not self.__properties_loaded:
+            self.load_rock_methods()
+        printable_str = ''
+        for table_num in self.__inputs.keys():
+            printable_str += '\n--------------------------------\n'
+            printable_str += f'ROCK method {table_num}\n'
+            printable_str += '--------------------------------\n'
+            printable_str += self.__inputs[table_num].__repr__()
+            printable_str += '\n'
+
+        return printable_str
+
+    @property
+    def inputs(self) -> MutableMapping[int, NexusRockMethod]:
+        if not self.__properties_loaded:
+            self.load_rock_methods()
+        return self.__inputs
+
+    @property
+    def files(self) -> dict[int, NexusFile]:
+        return self.__files
+
+    def load_rock_methods(self):
+        # Read in rock properties from Nexus rock method files
+        if self.__files is not None and len(self.__files) > 0:  # Check if rock files exist
+            for table_num in self.__files.keys():  # For each rock property method
+                rock_file = self.__files[table_num]
+                if rock_file.location is None:
+                    raise ValueError(f'Unable to find rock file: {rock_file}')
+                if os.path.isfile(rock_file.location):
+                    # Create NexusRockMethod object
+                    self.__inputs[table_num] = NexusRockMethod(file=rock_file, input_number=table_num)
+                    self.__inputs[table_num].read_properties()  # Populate object with rock properties in file
+        self.__properties_loaded = True
```

### Comparing `ressimpy-1.0.0/ResSimpy/Nexus/NexusWaterMethods.py` & `ressimpy-1.0.1/ResSimpy/Nexus/NexusWaterMethods.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,69 +1,69 @@
-from dataclasses import dataclass
-import os
-from typing import Optional, MutableMapping
-from ResSimpy.Nexus.DataModels.NexusFile import NexusFile
-from ResSimpy.Nexus.DataModels.NexusWaterMethod import NexusWaterMethod
-from ResSimpy.Water import Water
-
-
-@dataclass(kw_only=True)
-class NexusWaterMethods(Water):
-    """Class for collection of Nexus water property methods.
-
-    Attributes:
-        inputs (dict[int, NexusWaterMethod]): Collection of Nexus water property methods, as a dictionary
-        files (dict[int, NexusFile]): Dictionary collection of water property files, as defined in Nexus fcs file.
-    """
-
-    __inputs: MutableMapping[int, NexusWaterMethod]
-    __files: dict[int, NexusFile]
-    __properties_loaded: bool = False  # Used in lazy loading
-
-    def __init__(self, inputs: Optional[MutableMapping[int, NexusWaterMethod]] = None,
-                 files: Optional[dict[int, NexusFile]] = None) -> None:
-        if inputs:
-            self.__inputs = inputs
-        else:
-            self.__inputs: MutableMapping[int, NexusWaterMethod] = {}
-        if files:
-            self.__files = files
-        else:
-            self.__files = {}
-        super().__init__()
-
-    def __repr__(self) -> str:
-        """Pretty printing water methods."""
-        if not self.__properties_loaded:
-            self.load_water_methods()
-        printable_str = ''
-        for table_num in self.__inputs.keys():
-            printable_str += '\n--------------------------------\n'
-            printable_str += f'WATER method {table_num}\n'
-            printable_str += '--------------------------------\n'
-            printable_str += self.__inputs[table_num].__repr__()
-            printable_str += '\n'
-
-        return printable_str
-
-    @property
-    def inputs(self) -> MutableMapping[int, NexusWaterMethod]:
-        if not self.__properties_loaded:
-            self.load_water_methods()
-        return self.__inputs
-
-    @property
-    def files(self) -> dict[int, NexusFile]:
-        return self.__files
-
-    def load_water_methods(self):
-        # Read in water properties from Nexus water method files
-        if self.__files is not None and len(self.__files) > 0:  # Check if water files exist
-            for table_num in self.__files.keys():  # For each water property method
-                water_file = self.__files[table_num]
-                if water_file.location is None:
-                    raise ValueError(f'Unable to find water file: {water_file}')
-                if os.path.isfile(water_file.location):
-                    # Create NexusWaterMethod object
-                    self.__inputs[table_num] = NexusWaterMethod(file=water_file, input_number=table_num)
-                    self.__inputs[table_num].read_properties()  # Populate object with water properties in file
-        self.__properties_loaded = True
+from dataclasses import dataclass
+import os
+from typing import Optional, MutableMapping
+from ResSimpy.Nexus.DataModels.NexusFile import NexusFile
+from ResSimpy.Nexus.DataModels.NexusWaterMethod import NexusWaterMethod
+from ResSimpy.Water import Water
+
+
+@dataclass(kw_only=True)
+class NexusWaterMethods(Water):
+    """Class for collection of Nexus water property methods.
+
+    Attributes:
+        inputs (dict[int, NexusWaterMethod]): Collection of Nexus water property methods, as a dictionary
+        files (dict[int, NexusFile]): Dictionary collection of water property files, as defined in Nexus fcs file.
+    """
+
+    __inputs: MutableMapping[int, NexusWaterMethod]
+    __files: dict[int, NexusFile]
+    __properties_loaded: bool = False  # Used in lazy loading
+
+    def __init__(self, inputs: Optional[MutableMapping[int, NexusWaterMethod]] = None,
+                 files: Optional[dict[int, NexusFile]] = None) -> None:
+        if inputs:
+            self.__inputs = inputs
+        else:
+            self.__inputs: MutableMapping[int, NexusWaterMethod] = {}
+        if files:
+            self.__files = files
+        else:
+            self.__files = {}
+        super().__init__()
+
+    def __repr__(self) -> str:
+        """Pretty printing water methods."""
+        if not self.__properties_loaded:
+            self.load_water_methods()
+        printable_str = ''
+        for table_num in self.__inputs.keys():
+            printable_str += '\n--------------------------------\n'
+            printable_str += f'WATER method {table_num}\n'
+            printable_str += '--------------------------------\n'
+            printable_str += self.__inputs[table_num].__repr__()
+            printable_str += '\n'
+
+        return printable_str
+
+    @property
+    def inputs(self) -> MutableMapping[int, NexusWaterMethod]:
+        if not self.__properties_loaded:
+            self.load_water_methods()
+        return self.__inputs
+
+    @property
+    def files(self) -> dict[int, NexusFile]:
+        return self.__files
+
+    def load_water_methods(self):
+        # Read in water properties from Nexus water method files
+        if self.__files is not None and len(self.__files) > 0:  # Check if water files exist
+            for table_num in self.__files.keys():  # For each water property method
+                water_file = self.__files[table_num]
+                if water_file.location is None:
+                    raise ValueError(f'Unable to find water file: {water_file}')
+                if os.path.isfile(water_file.location):
+                    # Create NexusWaterMethod object
+                    self.__inputs[table_num] = NexusWaterMethod(file=water_file, input_number=table_num)
+                    self.__inputs[table_num].read_properties()  # Populate object with water properties in file
+        self.__properties_loaded = True
```

### Comparing `ressimpy-1.0.0/ResSimpy/Nexus/NexusWells.py` & `ressimpy-1.0.1/ResSimpy/Nexus/NexusWells.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,415 +1,415 @@
-from __future__ import annotations
-import warnings
-from dataclasses import dataclass, field
-from functools import cmp_to_key
-from typing import Sequence, Optional, TYPE_CHECKING
-from uuid import UUID
-
-import pandas as pd
-
-from ResSimpy.Enums.HowEnum import OperationEnum
-from ResSimpy.Nexus.DataModels.NexusCompletion import NexusCompletion
-from ResSimpy.Nexus.DataModels.NexusFile import NexusFile
-from ResSimpy.Nexus.DataModels.NexusWell import NexusWell
-from ResSimpy.Nexus.NexusKeywords.wells_keywords import WELLS_KEYWORDS
-from ResSimpy.Nexus.nexus_add_new_object_to_file import AddObjectOperations
-from ResSimpy.Wells import Wells
-from ResSimpy.Nexus.load_wells import load_wells
-import ResSimpy.Nexus.nexus_file_operations as nfo
-from ResSimpy.Utils.invert_nexus_map import attribute_name_to_nexus_keyword
-
-if TYPE_CHECKING:
-    from ResSimpy.Nexus.NexusSimulator import NexusSimulator
-
-
-@dataclass(kw_only=True)
-class NexusWells(Wells):
-    __model: NexusSimulator
-    __wells: list[NexusWell] = field(default_factory=list)
-    __wells_loaded: bool = False
-
-    def __init__(self, model: NexusSimulator) -> None:
-        self.__model = model
-        self.__wells = []
-        self.__add_object_operations = AddObjectOperations(model, self.table_header, self.table_footer)
-        super().__init__()
-
-    @property
-    def table_header(self) -> str:
-        return 'WELLSPEC'
-
-    @property
-    def table_footer(self) -> str:
-        return ''
-
-    def get_wells(self) -> Sequence[NexusWell]:
-        if not self.__wells_loaded:
-            self.load_wells()
-        return self.__wells
-
-    def get_well(self, well_name: str) -> Optional[NexusWell]:
-        """Returns a specific well requested, or None if that well cannot be found."""
-        if not self.__wells_loaded:
-            self.load_wells()
-
-        wells_to_return = filter(lambda x: x.well_name.upper() == well_name.upper(), self.__wells)
-
-        return next(wells_to_return, None)
-
-    def get_wells_df(self) -> pd.DataFrame:
-        # loop through wells and completions to output a table
-        if not self.__wells_loaded:
-            self.load_wells()
-
-        store_dictionaries = []
-        for well in self.__wells:
-            for completion in well.completions:
-                completion_props: dict[str, None | float | int | str] = {
-                    'well_name': well.well_name,
-                    'units': well.units.name,
-                    }
-                completion_props.update(completion.to_dict())
-                store_dictionaries.append(completion_props)
-        df_store = pd.DataFrame(store_dictionaries)
-        df_store = df_store.dropna(axis=1, how='all')
-        return df_store
-
-    def load_wells(self) -> None:
-        if self.__model.model_files.well_files is None:
-            raise FileNotFoundError('No wells files found for current model.')
-        for method_number, well_file in self.__model.model_files.well_files.items():
-            if well_file.location is None:
-                warnings.warn(f'Well file location has not been found for {well_file}')
-                continue
-            new_wells = load_wells(nexus_file=well_file, start_date=self.__model.start_date,
-                                   default_units=self.__model.default_units, date_format=self.__model.date_format)
-            self.__wells += new_wells
-        self.__wells_loaded = True
-
-    def get_wells_overview(self) -> str:
-        if not self.__wells_loaded:
-            self.load_wells()
-
-        overview: str = ''
-        for well in self.__wells:
-            overview += well.printable_well_info
-
-        return overview
-
-    def get_wells_dates(self) -> set[str]:
-        """Returns a set of the unique dates in the wellspec file over all wells."""
-        if not self.__wells_loaded:
-            self.load_wells()
-
-        set_dates: set[str] = set()
-        for well in self.__wells:
-            set_dates.update(set(well.dates_of_completions))
-
-        return set_dates
-
-    def modify_well(self, well_name: str, completion_properties_list: list[dict[str, None | float | int | str]],
-                    how: OperationEnum = OperationEnum.ADD) -> None:
-        """Modify the existing wells in memory using a dictionary of properties.
-
-        Args:
-        ----
-            well_name (str): name of the well to modify
-            completion_properties_list (list[InputDict]): a dictionary containing the properties to modify with the \
-                attribute as keys and the values as the updated property value. If remove will remove perforation that \
-                matches the values in the dictionary.
-            how (OperationEnum): operation enum taking the values OperationEnum.ADD, OperationEnum.REMOVE. \
-                Specifies how to modify the existing wells perforations.
-            remove_all_that_match (bool): If True will remove all wells that partially match the completion_properties\
-                provided. If False will remove perforation if only one matches, if several match throws a warning and \
-                does not remove them.
-            write_to_file (bool): If True writes directly to file. (Currently not in use)
-        """
-        well = self.get_well(well_name)
-        if well is None:
-            raise ValueError(f'No well named {well_name} found in simulator')
-        for perf in completion_properties_list:
-            if how == OperationEnum.ADD:
-                try:
-                    date = perf.get('date')
-                except AttributeError:
-                    raise AttributeError(
-                        f'No date provided in perf: {perf}, please provide a date to add the perforation at.')
-                if date is None:
-                    raise AttributeError(
-                        f'No date provided in perf: {perf}, please provide a date to add the perforation at.')
-                self.add_completion(well_name=well_name, completion_properties=perf)
-            elif how == OperationEnum.REMOVE:
-                completions_to_remove = well.find_completions(perf)
-                well._remove_completions_from_memory(completions_to_remove)
-            elif how == OperationEnum.MODIFY:
-                raise NotImplementedError('Modify in place not yet available. Please choose one of ADD/REMOVE')
-            else:
-                raise ValueError('Please select one of the valid OperationEnum values: e.g. OperationEnum.ADD')
-
-    def add_completion(self, well_name: str, completion_properties: dict[str, None | float | int | str],
-                       preserve_previous_completions: bool = True, comments: Optional[str] = None) -> None:
-        """Adds a completion to an existing wellspec file.
-
-        Args:
-        ----
-            well_name (str): well name to update
-            completion_properties (dict[str, float | int | str): properties of the completion you want to update.
-            Must contain date of the completion to be added.
-            preserve_previous_completions (bool): if true a new perforation added on a TIME card without a \
-            wellspec card for that well will preserve the previous completions from the closest TIME card in addition \
-            to the new completion
-        """
-        _, completion_date = self.__add_object_operations.check_name_date({'name': well_name} | completion_properties)
-        well = self.get_well(well_name)
-        if well is None:
-            # TODO could make this not raise an error and instead initialize a NexusWell and add it to NexusWells
-            raise ValueError(
-                f"No well found named: {well_name}. Cannot add completion to a well that doesn't exist")
-        well_id = well.completions[0].id
-
-        # add completion in memory
-        new_completion = well._add_completion_to_memory(completion_date, completion_properties)
-
-        if self.__model.model_files.well_files is None:
-            raise FileNotFoundError('No well file found, cannot modify ')
-
-        wellspec_file = self.__add_object_operations.find_which_file_from_id(id=well_id,
-                                                                             file_type_to_search='well_files')
-
-        # initialise some storage variables
-        nexus_mapping = NexusCompletion.get_nexus_mapping()
-        new_completion_time_index = -1
-        header_index = -1
-        headers: list[str] = []
-        headers_original: list[str] = []
-        additional_headers: list[str] = []
-        file_content = wellspec_file.get_flat_list_str_file
-        date_found = False
-        new_completion_index = len(file_content)
-        new_completion_string: list[str] = []
-        last_valid_line_index: int = -1
-        writing_new_wellspec_table = False
-        date_comp = 0
-        # if no time cards present in the file just find the name of the well instead
-        if not nfo.value_in_file('TIME', file_content):
-            new_completion_time_index = 0
-
-        for index, line in enumerate(file_content):
-            if header_index == -1 and nfo.check_token('TIME', line):
-                wellspec_date = nfo.get_expected_token_value('TIME', line, [line])
-                date_comp = self.__model._sim_controls.compare_dates(wellspec_date, completion_date)
-                if date_comp == 0:
-                    # if we've found the date we're looking for start looking for a wellspec and name card
-                    new_completion_time_index = index
-                    date_found = True
-                    continue
-                elif date_comp > 0 and header_index == -1:
-                    # if no date is found that is equal and we've found a date that is greater than the specified date
-                    # start to compile a wellspec table from scratch and add in the time cards
-                    new_completion_index = index
-                    header_index = index - 1
-                    headers, new_completion_index, new_completion_string, found_completion_at_previous_date = \
-                        self.__write_out_existing_wellspec(
-                            completion_date, completion_properties, date_found, index,
-                            new_completion_index, preserve_previous_completions, well, well_name)
-                    writing_new_wellspec_table = True
-                    if not found_completion_at_previous_date:
-                        break
-                else:
-                    continue
-
-            if nfo.check_token('WELLSPEC', line) and nfo.get_token_value('WELLSPEC', line, [line]) == well_name \
-                    and new_completion_time_index != -1:
-                # get the header of the wellspec table
-                header_index, headers, headers_original = self.__add_object_operations.get_and_write_new_header(
-                    additional_headers, completion_properties, file_content, index, nexus_mapping, wellspec_file
-                    )
-                continue
-
-            if header_index != -1 and nfo.nexus_token_found(line, WELLS_KEYWORDS) and index > header_index:
-                # if we hit the end of the wellspec table for the given well set the index for the new completion
-                if last_valid_line_index != -1:
-                    new_completion_index = last_valid_line_index + 1
-                break
-
-            elif header_index != -1 and index > header_index:
-                # check for valid rows + fill extra columns with NA
-                line_valid_index = self.__add_object_operations.fill_in_nas(additional_headers, headers_original, index,
-                                                                            line, wellspec_file, file_content)
-                # set the line to insert the new completion at to be the one after the last valid line
-                last_valid_line_index = line_valid_index if line_valid_index > 0 else last_valid_line_index
-        # If we haven't found a TIME card after the for loop then we haven't got a valid date so add it at the end
-        if date_comp < 0:
-            new_completion_index = len(file_content)
-            headers, new_completion_index, new_completion_string, found_completion_at_previous_date = \
-                self.__write_out_existing_wellspec(
-                    completion_date, completion_properties, date_found, new_completion_index,
-                    new_completion_index, preserve_previous_completions, well, well_name)
-            writing_new_wellspec_table = True
-
-        # construct the new completion and ensure the order of the values is in the same order as the headers
-        new_completion_string += new_completion.completion_to_wellspec_row(headers)
-        new_completion_additional_lines = len(new_completion_string)
-        if writing_new_wellspec_table:
-            new_completion_string += ['\n']
-        # write out to the file_content_as_list
-        new_completion_object_ids = {new_completion.id: [new_completion_index + new_completion_additional_lines - 1]}
-        wellspec_file.add_to_file_as_list(additional_content=new_completion_string, index=new_completion_index,
-                                          additional_objects=new_completion_object_ids, comments=comments)
-
-    def __write_out_existing_wellspec(self, completion_date: str,
-                                      completion_properties: dict[str, None | float | int | str],
-                                      date_found: bool, index: int, new_completion_index: int,
-                                      preserve_previous_completions: bool, well: NexusWell, well_name: str) -> \
-            tuple[list[str], int, list[str], bool]:
-        """Writes out the existing wellspec for a well at a new time stamp."""
-        nexus_mapping = NexusCompletion.get_nexus_mapping()
-        completion_table_as_list = ['\n']
-        if not date_found:
-            completion_table_as_list += ['TIME ' + completion_date + '\n']
-        completion_table_as_list += ['WELLSPEC ' + well_name + '\n']
-        headers = [k for k, v in nexus_mapping.items() if v[0] in completion_properties]
-        if preserve_previous_completions:
-            # get all the dates for that well
-            date_list = well.dates_of_completions
-            previous_dates = [x for x in date_list if
-                              self.__model._sim_controls.compare_dates(x, completion_date) < 0]
-            if len(previous_dates) == 0:
-                # if no dates that are smaller than the completion date then only add the perforation
-                # at the current index with a new wellspec card.
-                warnings.warn(f'No previous completions found for {well_name} at date: {completion_date}')
-                new_completion_index = index
-                write_out_headers = [' '.join(headers) + '\n']
-                completion_table_as_list += write_out_headers
-                return headers, new_completion_index, completion_table_as_list, False
-
-            # get the most recent date that is earlier than the new completion date
-            previous_dates = sorted(previous_dates, key=cmp_to_key(self.__model._sim_controls.compare_dates))
-            last_date = str(previous_dates[-1])
-            completion_to_find: dict[str, None | float | int | str] = {'date': last_date}
-            # find all completions at this date
-            previous_completion_list = well.find_completions(completion_to_find)
-            if len(previous_completion_list) > 0:
-                prev_completion_properties = {k: v for k, v in previous_completion_list[0].to_dict().items() if
-                                              v is not None}
-                for key in prev_completion_properties:
-                    if key == 'date':
-                        continue
-                    header_key = attribute_name_to_nexus_keyword(nexus_mapping, key)
-                    if header_key not in headers:
-                        headers.append(header_key)
-
-            write_out_headers = [' '.join(headers) + '\n']
-            completion_table_as_list += write_out_headers
-            # run through the existing completions to duplicate the completion at the new time
-            for completion in previous_completion_list:
-                completion_table_as_list += completion.completion_to_wellspec_row(headers)
-        else:
-            write_out_headers = [' '.join(headers) + '\n']
-            completion_table_as_list += write_out_headers
-        return headers, new_completion_index, completion_table_as_list, True
-
-    def remove_completion(self, well_name: str,
-                          completion_properties: Optional[dict[str, None | float | int | str]] = None,
-                          completion_id: Optional[UUID] = None) -> None:
-
-        well = self.get_well(well_name)
-        if well is None:
-            raise ValueError(f'No well found with name: {well_name}')
-
-        if completion_properties is None and completion_id is None:
-            raise ValueError('Must provide one of completion_properties dictionary or completion_id.')
-
-        # check for a date:
-        if completion_properties is not None:
-            completion_date = completion_properties.get('date', 'NO_DATE_PROVIDED')
-            if completion_date == 'NO_DATE_PROVIDED':
-                raise AttributeError('Completion requires a date. '
-                                     'Please provide a date in the completion_properties_list dictionary.')
-            if completion_id is None:
-                completion_id = well.find_completion(completion_properties).id
-        if completion_id is None:
-            raise ValueError('No completion found for completion_properties')
-        # find which wellspec file we should edit
-        wellspec_file = self.__add_object_operations.find_which_file_from_id(id=completion_id,
-                                                                             file_type_to_search='well_files')
-
-        # remove from the well object/wells class
-        completion_date = well.get_completion_by_id(completion_id).date
-        well._remove_completion_from_memory(completion_to_remove=completion_id)
-
-        # drop it from the wellspec file or include file if stored in include file
-        if wellspec_file.object_locations is None:
-            raise ValueError(f'No object locations specified, cannot find completion id: {completion_id}')
-        completion_indices = wellspec_file.object_locations[completion_id]
-        if len(completion_indices) > 0:
-            for comp_index in completion_indices:
-                wellspec_file.remove_from_file_as_list(comp_index, [completion_id])
-
-        # check that we have completions left:
-        find_completions_dict: dict[str, None | float | int | str] = {'date': completion_date}
-        remaining_completions = well.find_completions(find_completions_dict)
-        if len(remaining_completions) == 0:
-            # if there are no more completions remaining for that time stamp then remove the wellspec header!
-            self.__remove_wellspec_header(str(completion_date), well_name, wellspec_file)
-
-    def __remove_wellspec_header(self, completion_date: str, well_name: str, wellspec_file: NexusFile) -> None:
-        """Removes the wellspec and header if the wellspec table is empty\
-        must first check for whether the well has any remaining completions in the wellspec table.
-        """
-        nexus_mapping = NexusCompletion.get_nexus_mapping()
-        completion_date_found = False
-        file_content = wellspec_file.get_flat_list_str_file
-        wellspec_index = -1
-        header_index = -1
-        for index, line in enumerate(file_content):
-            if nfo.check_token('TIME', line) and nfo.get_expected_token_value('TIME', line, [line]) == \
-                    completion_date:
-                completion_date_found = True
-            if completion_date_found and nfo.check_token('WELLSPEC', line) and \
-                    nfo.get_token_value('WELLSPEC', line, [line]) == well_name:
-                # get the index in the list as string
-                wellspec_index = index
-                keyword_map = {x: y[0] for x, y in nexus_mapping.items()}
-                wellspec_table = file_content[wellspec_index::]
-                header_index, _ = nfo.get_table_header(file_as_list=wellspec_table, header_values=keyword_map)
-                header_index += wellspec_index
-                break
-        wellspec_file.remove_from_file_as_list(header_index)
-        wellspec_file.remove_from_file_as_list(wellspec_index)
-
-    def modify_completion(self, well_name: str, properties_to_modify: dict[str, None | float | int | str],
-                          completion_to_change: Optional[dict[str, None | float | int | str]] = None,
-                          completion_id: Optional[UUID] = None,
-                          comments: Optional[str] = None) -> None:
-        """Modify an existing matching completion, preserves attributes and modifies only additional properties
-        found within the provided properties to modify dictionary.
-
-        Args:
-            well_name (str): Name of the well with the completion to be modified.
-            properties_to_modify (dict[str, None | float | int | str]): attributes to change to.
-            completion_to_change (Optional[dict[str, None | float | int | str]]): properties of the existing completion.
-            User must provide enough to uniquely identify the completion.
-            completion_id (Optional[UUID]): If provided will match against a known UUID for the completion.
-        """
-        well = self.get_well(well_name)
-        if well is None:
-            raise ValueError(f'No well found with name: {well_name}')
-
-        if completion_to_change is not None:
-            completion = well.find_completion(completion_to_change)
-            completion_id = completion.id
-        elif completion_id is not None:
-            completion = well.get_completion_by_id(completion_id)
-        else:
-            raise ValueError('Must provide one of completion_to_change dictionary or completion_id')
-
-        # start with the existing properties
-        update_completion_properties: dict[str, None | float | int | str] = \
-            {k: v for k, v in completion.to_dict().items() if v is not None}
-
-        update_completion_properties.update(properties_to_modify)
-
-        self.remove_completion(well_name, completion_id=completion_id)
-        self.add_completion(well_name, update_completion_properties, preserve_previous_completions=True,
-                            comments=comments)
+from __future__ import annotations
+import warnings
+from dataclasses import dataclass, field
+from functools import cmp_to_key
+from typing import Sequence, Optional, TYPE_CHECKING
+from uuid import UUID
+
+import pandas as pd
+
+from ResSimpy.Enums.HowEnum import OperationEnum
+from ResSimpy.Nexus.DataModels.NexusCompletion import NexusCompletion
+from ResSimpy.Nexus.DataModels.NexusFile import NexusFile
+from ResSimpy.Nexus.DataModels.NexusWell import NexusWell
+from ResSimpy.Nexus.NexusKeywords.wells_keywords import WELLS_KEYWORDS
+from ResSimpy.Nexus.nexus_add_new_object_to_file import AddObjectOperations
+from ResSimpy.Wells import Wells
+from ResSimpy.Nexus.load_wells import load_wells
+import ResSimpy.Nexus.nexus_file_operations as nfo
+from ResSimpy.Utils.invert_nexus_map import attribute_name_to_nexus_keyword
+
+if TYPE_CHECKING:
+    from ResSimpy.Nexus.NexusSimulator import NexusSimulator
+
+
+@dataclass(kw_only=True)
+class NexusWells(Wells):
+    __model: NexusSimulator
+    __wells: list[NexusWell] = field(default_factory=list)
+    __wells_loaded: bool = False
+
+    def __init__(self, model: NexusSimulator) -> None:
+        self.__model = model
+        self.__wells = []
+        self.__add_object_operations = AddObjectOperations(model, self.table_header, self.table_footer)
+        super().__init__()
+
+    @property
+    def table_header(self) -> str:
+        return 'WELLSPEC'
+
+    @property
+    def table_footer(self) -> str:
+        return ''
+
+    def get_wells(self) -> Sequence[NexusWell]:
+        if not self.__wells_loaded:
+            self.load_wells()
+        return self.__wells
+
+    def get_well(self, well_name: str) -> Optional[NexusWell]:
+        """Returns a specific well requested, or None if that well cannot be found."""
+        if not self.__wells_loaded:
+            self.load_wells()
+
+        wells_to_return = filter(lambda x: x.well_name.upper() == well_name.upper(), self.__wells)
+
+        return next(wells_to_return, None)
+
+    def get_wells_df(self) -> pd.DataFrame:
+        # loop through wells and completions to output a table
+        if not self.__wells_loaded:
+            self.load_wells()
+
+        store_dictionaries = []
+        for well in self.__wells:
+            for completion in well.completions:
+                completion_props: dict[str, None | float | int | str] = {
+                    'well_name': well.well_name,
+                    'units': well.units.name,
+                    }
+                completion_props.update(completion.to_dict())
+                store_dictionaries.append(completion_props)
+        df_store = pd.DataFrame(store_dictionaries)
+        df_store = df_store.dropna(axis=1, how='all')
+        return df_store
+
+    def load_wells(self) -> None:
+        if self.__model.model_files.well_files is None:
+            raise FileNotFoundError('No wells files found for current model.')
+        for method_number, well_file in self.__model.model_files.well_files.items():
+            if well_file.location is None:
+                warnings.warn(f'Well file location has not been found for {well_file}')
+                continue
+            new_wells = load_wells(nexus_file=well_file, start_date=self.__model.start_date,
+                                   default_units=self.__model.default_units, date_format=self.__model.date_format)
+            self.__wells += new_wells
+        self.__wells_loaded = True
+
+    def get_wells_overview(self) -> str:
+        if not self.__wells_loaded:
+            self.load_wells()
+
+        overview: str = ''
+        for well in self.__wells:
+            overview += well.printable_well_info
+
+        return overview
+
+    def get_wells_dates(self) -> set[str]:
+        """Returns a set of the unique dates in the wellspec file over all wells."""
+        if not self.__wells_loaded:
+            self.load_wells()
+
+        set_dates: set[str] = set()
+        for well in self.__wells:
+            set_dates.update(set(well.dates_of_completions))
+
+        return set_dates
+
+    def modify_well(self, well_name: str, completion_properties_list: list[dict[str, None | float | int | str]],
+                    how: OperationEnum = OperationEnum.ADD) -> None:
+        """Modify the existing wells in memory using a dictionary of properties.
+
+        Args:
+        ----
+            well_name (str): name of the well to modify
+            completion_properties_list (list[InputDict]): a dictionary containing the properties to modify with the \
+                attribute as keys and the values as the updated property value. If remove will remove perforation that \
+                matches the values in the dictionary.
+            how (OperationEnum): operation enum taking the values OperationEnum.ADD, OperationEnum.REMOVE. \
+                Specifies how to modify the existing wells perforations.
+            remove_all_that_match (bool): If True will remove all wells that partially match the completion_properties\
+                provided. If False will remove perforation if only one matches, if several match throws a warning and \
+                does not remove them.
+            write_to_file (bool): If True writes directly to file. (Currently not in use)
+        """
+        well = self.get_well(well_name)
+        if well is None:
+            raise ValueError(f'No well named {well_name} found in simulator')
+        for perf in completion_properties_list:
+            if how == OperationEnum.ADD:
+                try:
+                    date = perf.get('date')
+                except AttributeError:
+                    raise AttributeError(
+                        f'No date provided in perf: {perf}, please provide a date to add the perforation at.')
+                if date is None:
+                    raise AttributeError(
+                        f'No date provided in perf: {perf}, please provide a date to add the perforation at.')
+                self.add_completion(well_name=well_name, completion_properties=perf)
+            elif how == OperationEnum.REMOVE:
+                completions_to_remove = well.find_completions(perf)
+                well._remove_completions_from_memory(completions_to_remove)
+            elif how == OperationEnum.MODIFY:
+                raise NotImplementedError('Modify in place not yet available. Please choose one of ADD/REMOVE')
+            else:
+                raise ValueError('Please select one of the valid OperationEnum values: e.g. OperationEnum.ADD')
+
+    def add_completion(self, well_name: str, completion_properties: dict[str, None | float | int | str],
+                       preserve_previous_completions: bool = True, comments: Optional[str] = None) -> None:
+        """Adds a completion to an existing wellspec file.
+
+        Args:
+        ----
+            well_name (str): well name to update
+            completion_properties (dict[str, float | int | str): properties of the completion you want to update.
+            Must contain date of the completion to be added.
+            preserve_previous_completions (bool): if true a new perforation added on a TIME card without a \
+            wellspec card for that well will preserve the previous completions from the closest TIME card in addition \
+            to the new completion
+        """
+        _, completion_date = self.__add_object_operations.check_name_date({'name': well_name} | completion_properties)
+        well = self.get_well(well_name)
+        if well is None:
+            # TODO could make this not raise an error and instead initialize a NexusWell and add it to NexusWells
+            raise ValueError(
+                f"No well found named: {well_name}. Cannot add completion to a well that doesn't exist")
+        well_id = well.completions[0].id
+
+        # add completion in memory
+        new_completion = well._add_completion_to_memory(completion_date, completion_properties)
+
+        if self.__model.model_files.well_files is None:
+            raise FileNotFoundError('No well file found, cannot modify ')
+
+        wellspec_file = self.__add_object_operations.find_which_file_from_id(id=well_id,
+                                                                             file_type_to_search='well_files')
+
+        # initialise some storage variables
+        nexus_mapping = NexusCompletion.get_nexus_mapping()
+        new_completion_time_index = -1
+        header_index = -1
+        headers: list[str] = []
+        headers_original: list[str] = []
+        additional_headers: list[str] = []
+        file_content = wellspec_file.get_flat_list_str_file
+        date_found = False
+        new_completion_index = len(file_content)
+        new_completion_string: list[str] = []
+        last_valid_line_index: int = -1
+        writing_new_wellspec_table = False
+        date_comp = 0
+        # if no time cards present in the file just find the name of the well instead
+        if not nfo.value_in_file('TIME', file_content):
+            new_completion_time_index = 0
+
+        for index, line in enumerate(file_content):
+            if header_index == -1 and nfo.check_token('TIME', line):
+                wellspec_date = nfo.get_expected_token_value('TIME', line, [line])
+                date_comp = self.__model._sim_controls.compare_dates(wellspec_date, completion_date)
+                if date_comp == 0:
+                    # if we've found the date we're looking for start looking for a wellspec and name card
+                    new_completion_time_index = index
+                    date_found = True
+                    continue
+                elif date_comp > 0 and header_index == -1:
+                    # if no date is found that is equal and we've found a date that is greater than the specified date
+                    # start to compile a wellspec table from scratch and add in the time cards
+                    new_completion_index = index
+                    header_index = index - 1
+                    headers, new_completion_index, new_completion_string, found_completion_at_previous_date = \
+                        self.__write_out_existing_wellspec(
+                            completion_date, completion_properties, date_found, index,
+                            new_completion_index, preserve_previous_completions, well, well_name)
+                    writing_new_wellspec_table = True
+                    if not found_completion_at_previous_date:
+                        break
+                else:
+                    continue
+
+            if nfo.check_token('WELLSPEC', line) and nfo.get_token_value('WELLSPEC', line, [line]) == well_name \
+                    and new_completion_time_index != -1:
+                # get the header of the wellspec table
+                header_index, headers, headers_original = self.__add_object_operations.get_and_write_new_header(
+                    additional_headers, completion_properties, file_content, index, nexus_mapping, wellspec_file
+                    )
+                continue
+
+            if header_index != -1 and nfo.nexus_token_found(line, WELLS_KEYWORDS) and index > header_index:
+                # if we hit the end of the wellspec table for the given well set the index for the new completion
+                if last_valid_line_index != -1:
+                    new_completion_index = last_valid_line_index + 1
+                break
+
+            elif header_index != -1 and index > header_index:
+                # check for valid rows + fill extra columns with NA
+                line_valid_index = self.__add_object_operations.fill_in_nas(additional_headers, headers_original, index,
+                                                                            line, wellspec_file, file_content)
+                # set the line to insert the new completion at to be the one after the last valid line
+                last_valid_line_index = line_valid_index if line_valid_index > 0 else last_valid_line_index
+        # If we haven't found a TIME card after the for loop then we haven't got a valid date so add it at the end
+        if date_comp < 0:
+            new_completion_index = len(file_content)
+            headers, new_completion_index, new_completion_string, found_completion_at_previous_date = \
+                self.__write_out_existing_wellspec(
+                    completion_date, completion_properties, date_found, new_completion_index,
+                    new_completion_index, preserve_previous_completions, well, well_name)
+            writing_new_wellspec_table = True
+
+        # construct the new completion and ensure the order of the values is in the same order as the headers
+        new_completion_string += new_completion.completion_to_wellspec_row(headers)
+        new_completion_additional_lines = len(new_completion_string)
+        if writing_new_wellspec_table:
+            new_completion_string += ['\n']
+        # write out to the file_content_as_list
+        new_completion_object_ids = {new_completion.id: [new_completion_index + new_completion_additional_lines - 1]}
+        wellspec_file.add_to_file_as_list(additional_content=new_completion_string, index=new_completion_index,
+                                          additional_objects=new_completion_object_ids, comments=comments)
+
+    def __write_out_existing_wellspec(self, completion_date: str,
+                                      completion_properties: dict[str, None | float | int | str],
+                                      date_found: bool, index: int, new_completion_index: int,
+                                      preserve_previous_completions: bool, well: NexusWell, well_name: str) -> \
+            tuple[list[str], int, list[str], bool]:
+        """Writes out the existing wellspec for a well at a new time stamp."""
+        nexus_mapping = NexusCompletion.get_nexus_mapping()
+        completion_table_as_list = ['\n']
+        if not date_found:
+            completion_table_as_list += ['TIME ' + completion_date + '\n']
+        completion_table_as_list += ['WELLSPEC ' + well_name + '\n']
+        headers = [k for k, v in nexus_mapping.items() if v[0] in completion_properties]
+        if preserve_previous_completions:
+            # get all the dates for that well
+            date_list = well.dates_of_completions
+            previous_dates = [x for x in date_list if
+                              self.__model._sim_controls.compare_dates(x, completion_date) < 0]
+            if len(previous_dates) == 0:
+                # if no dates that are smaller than the completion date then only add the perforation
+                # at the current index with a new wellspec card.
+                warnings.warn(f'No previous completions found for {well_name} at date: {completion_date}')
+                new_completion_index = index
+                write_out_headers = [' '.join(headers) + '\n']
+                completion_table_as_list += write_out_headers
+                return headers, new_completion_index, completion_table_as_list, False
+
+            # get the most recent date that is earlier than the new completion date
+            previous_dates = sorted(previous_dates, key=cmp_to_key(self.__model._sim_controls.compare_dates))
+            last_date = str(previous_dates[-1])
+            completion_to_find: dict[str, None | float | int | str] = {'date': last_date}
+            # find all completions at this date
+            previous_completion_list = well.find_completions(completion_to_find)
+            if len(previous_completion_list) > 0:
+                prev_completion_properties = {k: v for k, v in previous_completion_list[0].to_dict().items() if
+                                              v is not None}
+                for key in prev_completion_properties:
+                    if key == 'date':
+                        continue
+                    header_key = attribute_name_to_nexus_keyword(nexus_mapping, key)
+                    if header_key not in headers:
+                        headers.append(header_key)
+
+            write_out_headers = [' '.join(headers) + '\n']
+            completion_table_as_list += write_out_headers
+            # run through the existing completions to duplicate the completion at the new time
+            for completion in previous_completion_list:
+                completion_table_as_list += completion.completion_to_wellspec_row(headers)
+        else:
+            write_out_headers = [' '.join(headers) + '\n']
+            completion_table_as_list += write_out_headers
+        return headers, new_completion_index, completion_table_as_list, True
+
+    def remove_completion(self, well_name: str,
+                          completion_properties: Optional[dict[str, None | float | int | str]] = None,
+                          completion_id: Optional[UUID] = None) -> None:
+
+        well = self.get_well(well_name)
+        if well is None:
+            raise ValueError(f'No well found with name: {well_name}')
+
+        if completion_properties is None and completion_id is None:
+            raise ValueError('Must provide one of completion_properties dictionary or completion_id.')
+
+        # check for a date:
+        if completion_properties is not None:
+            completion_date = completion_properties.get('date', 'NO_DATE_PROVIDED')
+            if completion_date == 'NO_DATE_PROVIDED':
+                raise AttributeError('Completion requires a date. '
+                                     'Please provide a date in the completion_properties_list dictionary.')
+            if completion_id is None:
+                completion_id = well.find_completion(completion_properties).id
+        if completion_id is None:
+            raise ValueError('No completion found for completion_properties')
+        # find which wellspec file we should edit
+        wellspec_file = self.__add_object_operations.find_which_file_from_id(id=completion_id,
+                                                                             file_type_to_search='well_files')
+
+        # remove from the well object/wells class
+        completion_date = well.get_completion_by_id(completion_id).date
+        well._remove_completion_from_memory(completion_to_remove=completion_id)
+
+        # drop it from the wellspec file or include file if stored in include file
+        if wellspec_file.object_locations is None:
+            raise ValueError(f'No object locations specified, cannot find completion id: {completion_id}')
+        completion_indices = wellspec_file.object_locations[completion_id]
+        if len(completion_indices) > 0:
+            for comp_index in completion_indices:
+                wellspec_file.remove_from_file_as_list(comp_index, [completion_id])
+
+        # check that we have completions left:
+        find_completions_dict: dict[str, None | float | int | str] = {'date': completion_date}
+        remaining_completions = well.find_completions(find_completions_dict)
+        if len(remaining_completions) == 0:
+            # if there are no more completions remaining for that time stamp then remove the wellspec header!
+            self.__remove_wellspec_header(str(completion_date), well_name, wellspec_file)
+
+    def __remove_wellspec_header(self, completion_date: str, well_name: str, wellspec_file: NexusFile) -> None:
+        """Removes the wellspec and header if the wellspec table is empty\
+        must first check for whether the well has any remaining completions in the wellspec table.
+        """
+        nexus_mapping = NexusCompletion.get_nexus_mapping()
+        completion_date_found = False
+        file_content = wellspec_file.get_flat_list_str_file
+        wellspec_index = -1
+        header_index = -1
+        for index, line in enumerate(file_content):
+            if nfo.check_token('TIME', line) and nfo.get_expected_token_value('TIME', line, [line]) == \
+                    completion_date:
+                completion_date_found = True
+            if completion_date_found and nfo.check_token('WELLSPEC', line) and \
+                    nfo.get_token_value('WELLSPEC', line, [line]) == well_name:
+                # get the index in the list as string
+                wellspec_index = index
+                keyword_map = {x: y[0] for x, y in nexus_mapping.items()}
+                wellspec_table = file_content[wellspec_index::]
+                header_index, _ = nfo.get_table_header(file_as_list=wellspec_table, header_values=keyword_map)
+                header_index += wellspec_index
+                break
+        wellspec_file.remove_from_file_as_list(header_index)
+        wellspec_file.remove_from_file_as_list(wellspec_index)
+
+    def modify_completion(self, well_name: str, properties_to_modify: dict[str, None | float | int | str],
+                          completion_to_change: Optional[dict[str, None | float | int | str]] = None,
+                          completion_id: Optional[UUID] = None,
+                          comments: Optional[str] = None) -> None:
+        """Modify an existing matching completion, preserves attributes and modifies only additional properties
+        found within the provided properties to modify dictionary.
+
+        Args:
+            well_name (str): Name of the well with the completion to be modified.
+            properties_to_modify (dict[str, None | float | int | str]): attributes to change to.
+            completion_to_change (Optional[dict[str, None | float | int | str]]): properties of the existing completion.
+            User must provide enough to uniquely identify the completion.
+            completion_id (Optional[UUID]): If provided will match against a known UUID for the completion.
+        """
+        well = self.get_well(well_name)
+        if well is None:
+            raise ValueError(f'No well found with name: {well_name}')
+
+        if completion_to_change is not None:
+            completion = well.find_completion(completion_to_change)
+            completion_id = completion.id
+        elif completion_id is not None:
+            completion = well.get_completion_by_id(completion_id)
+        else:
+            raise ValueError('Must provide one of completion_to_change dictionary or completion_id')
+
+        # start with the existing properties
+        update_completion_properties: dict[str, None | float | int | str] = \
+            {k: v for k, v in completion.to_dict().items() if v is not None}
+
+        update_completion_properties.update(properties_to_modify)
+
+        self.remove_completion(well_name, completion_id=completion_id)
+        self.add_completion(well_name, update_completion_properties, preserve_previous_completions=True,
+                            comments=comments)
```

### Comparing `ressimpy-1.0.0/ResSimpy/Nexus/runcontrol_operations.py` & `ressimpy-1.0.1/ResSimpy/Nexus/runcontrol_operations.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,334 +1,334 @@
-from __future__ import annotations
-
-import warnings
-from datetime import datetime, timedelta
-from functools import cmp_to_key
-from typing import Union, Optional
-import ResSimpy.Nexus.nexus_file_operations as nfo
-from ResSimpy.Nexus.NexusEnums.DateFormatEnum import DateFormat
-from ResSimpy.Nexus.constants import DATE_WITH_TIME_LENGTH
-
-
-class SimControls:
-    def __init__(self, model) -> None:
-        """Class for controlling all runcontrol and time related functionality
-        Args:
-            model: NexusSimulator instance
-            __times (Optional[list[str]]): list of times to be included in the runcontrol file
-            __date_format_string (str): How the dates should formatted based on date_format.
-
-        """
-        self.__model = model
-        self.__times: Optional[list[str]] = None
-        self.__date_format_string: str = ''
-
-    @property
-    def date_format_string(self):
-        return self.__date_format_string
-
-    @date_format_string.setter
-    def date_format_string(self, value):
-        self.__date_format_string = value
-
-    @property
-    def times(self):
-        return self.__times if self.__times is not None else []
-
-    @staticmethod
-    def get_times(times_file: list[str]) -> list[str]:
-        """Retrieves a list of TIMES from the supplied Runcontrol / Include file.
-
-        Args:
-        ----
-            times_file (list[str]): list of strings with each line from the file a new entry in the list
-        Returns:
-            list[str]: list of all the values following the TIME keyword in supplied file, \
-                empty list if no values found
-        """
-        times = []
-        for line in times_file:
-            if nfo.check_token('TIME', line):
-                value = nfo.get_token_value('TIME', line, times_file)
-                if value is not None:
-                    times.append(value)
-
-        return times
-
-    @staticmethod
-    def delete_times(file_content: list[str]) -> list[str]:
-        """Deletes times from file contents.
-
-        Args:
-            file_content (list[str]):  list of strings with each line from the file a new entry in the list.
-
-        Returns:
-            list[str]: the modified file without any TIME cards in
-        """
-        new_file: list[str] = []
-        previous_line_is_time = False
-        for line in file_content:
-            if "TIME " not in line and (previous_line_is_time is False or line != '\n'):
-                new_file.append(line)
-                previous_line_is_time = False
-            elif "TIME " in line:
-                previous_line_is_time = True
-            else:
-                previous_line_is_time = False
-        return new_file
-
-    @staticmethod
-    def remove_times_from_file(file_content: list[str], output_file_path: str) -> None:
-        """Removes the times from a file - used for replacing with new times
-        Args:
-            file_content (list[str]): a list of strings containing each line of the file as a new entry
-            output_file_path (str): path to the file to output to.
-        """
-        new_file_content = SimControls.delete_times(file_content)
-
-        new_file_str = "".join(new_file_content)
-
-        with open(output_file_path, "w") as text_file:
-            text_file.write(new_file_str)
-
-    def convert_date_to_number(self, date: Union[str, int, float]) -> float:
-        """Converts a date to a number designating number of days from the start date.
-
-        Args:
-        ----
-            date (Union[str, int, float]): a date or time stamp from a Nexus simulation
-        Raises:
-            ValueError: if supplied incorrect type for 'date' parameter
-
-        Returns:
-        -------
-            float: the difference between the supplied date and the start date of the simulator
-        """
-        # If we can retrieve a number of days from date, use that, otherwise convert the string date to a number of days
-        try:
-            converted_date: Union[str, float] = float(date)
-        except ValueError:
-            if not isinstance(date, str):
-                raise ValueError("convert_date_to_number: Incorrect type for 'date' parameter")
-            converted_date = date
-
-        if isinstance(converted_date, float):
-            date_format = self.date_format_string
-            if len(self.__model.start_date) == DATE_WITH_TIME_LENGTH:
-                date_format += "(%H:%M:%S)"
-            start_date_as_datetime = datetime.strptime(self.__model.start_date, date_format)
-            date_as_datetime = start_date_as_datetime + timedelta(days=converted_date)
-        else:
-            start_date_format = self.date_format_string
-            if len(self.__model.start_date) == DATE_WITH_TIME_LENGTH:
-                start_date_format += "(%H:%M:%S)"
-            end_date_format = self.date_format_string
-            if len(converted_date) == DATE_WITH_TIME_LENGTH:
-                end_date_format += "(%H:%M:%S)"
-            date_as_datetime = datetime.strptime(converted_date, end_date_format)
-            start_date_as_datetime = datetime.strptime(self.__model.start_date, start_date_format)
-
-        difference = date_as_datetime - start_date_as_datetime
-        return difference.total_seconds() / timedelta(days=1).total_seconds()
-
-    def compare_dates(self, x: Union[str, float], y: Union[str, float]) -> int:
-        """Comparator for two supplied dates or numbers.
-
-        Args:
-        ----
-            x (Union[str, float]): first date to compare
-            y (Union[str, float]): second date to compare
-
-        Returns:
-        -------
-            int: -1 if y > x, 0 if y == x, 1 if y < x
-        """
-        date_comp = self.convert_date_to_number(x) - self.convert_date_to_number(y)
-        if date_comp < 0:
-            date_comp_int = -1
-        elif date_comp == 0:
-            date_comp_int = 0
-        else:
-            date_comp_int = 1
-
-        return date_comp_int
-
-    def sort_remove_duplicate_times(self, times: list[str]) -> list[str]:
-        """Removes duplicates and nans from the times list, then sorts them.
-
-        Args:
-        ----
-            times (list[str]): list of times to remove duplicates from
-
-        Returns:
-        -------
-            list[str]: list of times without duplicates
-        """
-        new_times = []
-        for i in times:
-            i_value = i.strip()
-            if i != i or i_value in new_times:
-                continue
-            new_times.append(i_value)
-        new_times = sorted(new_times, key=cmp_to_key(self.compare_dates))
-        return new_times
-
-    def check_date_format(self, date: Union[str, float]) -> None:
-        """Checks that a supplied date is in the correct format.
-
-        Args:
-        ----
-            date (Union[str, float]): date to check the format of
-        Raises:
-            ValueError: If a date provided isn't in a date format that the model expects
-        """
-        try:
-            float(date)
-        except ValueError:
-            # Value isn't a float - attempt to extract date from value
-            try:
-                date_format = self.date_format_string
-                if len(str(date)) == DATE_WITH_TIME_LENGTH:
-                    date_format += "(%H:%M:%S)"
-                datetime.strptime(str(date), date_format)
-            except ValueError:
-                current_date_format = self.get_date_format(self.__model.date_format)
-                raise ValueError(
-                    "Invalid date format " + str(date) + " the model is using " + current_date_format + " date format.")
-
-    @staticmethod
-    def get_date_format(date_format: DateFormat) -> str:
-        """Returns the date format being used by the model
-        formats used: ('MM/DD/YYYY', 'DD/MM/YYYY').
-        """
-
-        if date_format is DateFormat.MM_DD_YYYY:
-            return 'MM/DD/YYYY'
-        else:
-            return 'DD/MM/YYYY'
-
-    def __update_times_in_file(self) -> None:
-        """Updates the list of times in the Runcontrol file to the current stored values in __times.
-
-        Returns:
-            None: writes out a file at the same path as the existing runcontrol file
-        """
-        self.__model.check_output_path()
-        if self.__model.model_files.runcontrol_file is None or \
-                self.__model.model_files.runcontrol_file.location is None:
-            raise ValueError(f"No file path found for {self.__model.model_files}")
-        file_content = self.__model.model_files.runcontrol_file.get_flat_list_str_file
-        filename = self.__model.model_files.runcontrol_file.location
-
-        new_file_content = self.__model._sim_controls.delete_times(file_content)
-
-        time_list = self.times
-        stop_string = 'STOP\n'
-        if stop_string in new_file_content:
-            new_file_content.remove(stop_string)
-
-        def prepend_time(s: str) -> str:
-            return "TIME " + s
-
-        time_list = [prepend_time(x) for x in time_list]
-        num_times = len(time_list)
-
-        new_line_list = ["\n\n"] * num_times
-        zipped_list = list(zip(time_list, new_line_list))
-        flat_list = [item for sublist in zipped_list for item in sublist]
-        flat_list.append(stop_string)
-        new_file_content.extend(flat_list)
-        new_file_str = "".join(new_file_content)
-
-        with open(filename, "w") as text_file:
-            text_file.write(new_file_str)
-
-    def load_run_control_file(self):
-        """Loads the run control information into the class instance. \
-            If the write_times attribute is True then it expands out any INCLUDE files with the times found within
-        Raises:
-            ValueError: if the run_control_file attribute is None.
-        """
-        if self.__model.model_files.runcontrol_file is None:
-            warnings.warn(f"Run control file path not found for {self.__model.model_files.location}")
-            return
-        run_control_file_content = self.__model.model_files.runcontrol_file.get_flat_list_str_file
-
-        if (run_control_file_content is None) or (self.__model.model_files.runcontrol_file.location is None):
-            raise ValueError(f"No file path provided for {self.__model.model_files.runcontrol_file.location=}")
-
-        # set the start date
-        for line in run_control_file_content:
-            if nfo.check_token('START', line):
-                value = nfo.get_expected_token_value('START', line, run_control_file_content)
-                if value is not None:
-                    self.__model.start_date = value
-
-        times = []
-        run_control_times = self.get_times(run_control_file_content)
-        times.extend(run_control_times)
-        if self.__model.start_date is None or self.__model.start_date == '':
-            try:
-                self.__model.start_date = times[0]
-            except IndexError:
-                for line in run_control_file_content:
-                    if nfo.check_token('TIME', line):
-                        value = nfo.get_expected_token_value('TIME', line, run_control_file_content)
-                        self.__model.start_date = value
-                        warnings.warn(f'Setting start date to first time card found in the runcontrol file as: {value}')
-                        break
-                warnings.warn('No value found for start date explicitly with START or TIME card')
-
-        self.__times = self.sort_remove_duplicate_times(times)
-
-        # If we don't want to write the times, return here.
-        if not self.__model.write_times:
-            return
-        if self.__model.model_files.runcontrol_file.include_locations is None:
-            warnings.warn(f'No includes files found in {self.__model.model_files.runcontrol_file.location}')
-            return
-        for file in self.__model.model_files.runcontrol_file.include_locations:
-            if self.__model.destination is not None:
-                self.remove_times_from_file(run_control_file_content, file)
-
-        self.modify_times(content=times, operation='replace')
-
-    def modify_times(self, content: Optional[list[str]] = None, operation: str = 'merge'):
-        """Modifies the output times in the simulation.
-
-        Args:
-        ----
-            content (list[str]], optional): The content to modify using the above operation, \
-            represented as a list of strings with a new entry per line of the file. Defaults to None.
-            operation (str, optional): operation to perform on the content provided (e.g. 'merge'). Defaults to 'merge'.
-
-        Raises:
-        ------
-            ValueError: if the supplied dates are before the start date of the simulation
-        """
-        if content is None:
-            content = []
-        for time in content:
-            self.check_date_format(time)
-
-        new_times = self.sort_remove_duplicate_times(content)
-        if len(new_times) > 0 > self.compare_dates(new_times[0], self.__model.start_date):
-            raise ValueError(
-                f"The supplied date of {new_times[0]} precedes the start date of {self.__model.start_date}")
-        operation = operation.lower()
-        self.__times = self.__times if self.__times is not None else []
-
-        if operation == 'merge':
-            self.__times.extend(content)
-        elif operation == 'replace':
-            self.__times = content
-        elif operation == 'reset':
-            self.__times = []
-        elif operation == 'remove':
-            for time in content:
-                if time in self.__times:
-                    self.__times.remove(time)
-
-        self.__times = self.sort_remove_duplicate_times(self.__times)
-
-        if self.__model.destination is not None:
-            self.__update_times_in_file()
+from __future__ import annotations
+
+import warnings
+from datetime import datetime, timedelta
+from functools import cmp_to_key
+from typing import Union, Optional
+import ResSimpy.Nexus.nexus_file_operations as nfo
+from ResSimpy.Nexus.NexusEnums.DateFormatEnum import DateFormat
+from ResSimpy.Nexus.constants import DATE_WITH_TIME_LENGTH
+
+
+class SimControls:
+    def __init__(self, model) -> None:
+        """Class for controlling all runcontrol and time related functionality
+        Args:
+            model: NexusSimulator instance
+            __times (Optional[list[str]]): list of times to be included in the runcontrol file
+            __date_format_string (str): How the dates should formatted based on date_format.
+
+        """
+        self.__model = model
+        self.__times: Optional[list[str]] = None
+        self.__date_format_string: str = ''
+
+    @property
+    def date_format_string(self):
+        return self.__date_format_string
+
+    @date_format_string.setter
+    def date_format_string(self, value):
+        self.__date_format_string = value
+
+    @property
+    def times(self):
+        return self.__times if self.__times is not None else []
+
+    @staticmethod
+    def get_times(times_file: list[str]) -> list[str]:
+        """Retrieves a list of TIMES from the supplied Runcontrol / Include file.
+
+        Args:
+        ----
+            times_file (list[str]): list of strings with each line from the file a new entry in the list
+        Returns:
+            list[str]: list of all the values following the TIME keyword in supplied file, \
+                empty list if no values found
+        """
+        times = []
+        for line in times_file:
+            if nfo.check_token('TIME', line):
+                value = nfo.get_token_value('TIME', line, times_file)
+                if value is not None:
+                    times.append(value)
+
+        return times
+
+    @staticmethod
+    def delete_times(file_content: list[str]) -> list[str]:
+        """Deletes times from file contents.
+
+        Args:
+            file_content (list[str]):  list of strings with each line from the file a new entry in the list.
+
+        Returns:
+            list[str]: the modified file without any TIME cards in
+        """
+        new_file: list[str] = []
+        previous_line_is_time = False
+        for line in file_content:
+            if "TIME " not in line and (previous_line_is_time is False or line != '\n'):
+                new_file.append(line)
+                previous_line_is_time = False
+            elif "TIME " in line:
+                previous_line_is_time = True
+            else:
+                previous_line_is_time = False
+        return new_file
+
+    @staticmethod
+    def remove_times_from_file(file_content: list[str], output_file_path: str) -> None:
+        """Removes the times from a file - used for replacing with new times
+        Args:
+            file_content (list[str]): a list of strings containing each line of the file as a new entry
+            output_file_path (str): path to the file to output to.
+        """
+        new_file_content = SimControls.delete_times(file_content)
+
+        new_file_str = "".join(new_file_content)
+
+        with open(output_file_path, "w") as text_file:
+            text_file.write(new_file_str)
+
+    def convert_date_to_number(self, date: Union[str, int, float]) -> float:
+        """Converts a date to a number designating number of days from the start date.
+
+        Args:
+        ----
+            date (Union[str, int, float]): a date or time stamp from a Nexus simulation
+        Raises:
+            ValueError: if supplied incorrect type for 'date' parameter
+
+        Returns:
+        -------
+            float: the difference between the supplied date and the start date of the simulator
+        """
+        # If we can retrieve a number of days from date, use that, otherwise convert the string date to a number of days
+        try:
+            converted_date: Union[str, float] = float(date)
+        except ValueError:
+            if not isinstance(date, str):
+                raise ValueError("convert_date_to_number: Incorrect type for 'date' parameter")
+            converted_date = date
+
+        if isinstance(converted_date, float):
+            date_format = self.date_format_string
+            if len(self.__model.start_date) == DATE_WITH_TIME_LENGTH:
+                date_format += "(%H:%M:%S)"
+            start_date_as_datetime = datetime.strptime(self.__model.start_date, date_format)
+            date_as_datetime = start_date_as_datetime + timedelta(days=converted_date)
+        else:
+            start_date_format = self.date_format_string
+            if len(self.__model.start_date) == DATE_WITH_TIME_LENGTH:
+                start_date_format += "(%H:%M:%S)"
+            end_date_format = self.date_format_string
+            if len(converted_date) == DATE_WITH_TIME_LENGTH:
+                end_date_format += "(%H:%M:%S)"
+            date_as_datetime = datetime.strptime(converted_date, end_date_format)
+            start_date_as_datetime = datetime.strptime(self.__model.start_date, start_date_format)
+
+        difference = date_as_datetime - start_date_as_datetime
+        return difference.total_seconds() / timedelta(days=1).total_seconds()
+
+    def compare_dates(self, x: Union[str, float], y: Union[str, float]) -> int:
+        """Comparator for two supplied dates or numbers.
+
+        Args:
+        ----
+            x (Union[str, float]): first date to compare
+            y (Union[str, float]): second date to compare
+
+        Returns:
+        -------
+            int: -1 if y > x, 0 if y == x, 1 if y < x
+        """
+        date_comp = self.convert_date_to_number(x) - self.convert_date_to_number(y)
+        if date_comp < 0:
+            date_comp_int = -1
+        elif date_comp == 0:
+            date_comp_int = 0
+        else:
+            date_comp_int = 1
+
+        return date_comp_int
+
+    def sort_remove_duplicate_times(self, times: list[str]) -> list[str]:
+        """Removes duplicates and nans from the times list, then sorts them.
+
+        Args:
+        ----
+            times (list[str]): list of times to remove duplicates from
+
+        Returns:
+        -------
+            list[str]: list of times without duplicates
+        """
+        new_times = []
+        for i in times:
+            i_value = i.strip()
+            if i != i or i_value in new_times:
+                continue
+            new_times.append(i_value)
+        new_times = sorted(new_times, key=cmp_to_key(self.compare_dates))
+        return new_times
+
+    def check_date_format(self, date: Union[str, float]) -> None:
+        """Checks that a supplied date is in the correct format.
+
+        Args:
+        ----
+            date (Union[str, float]): date to check the format of
+        Raises:
+            ValueError: If a date provided isn't in a date format that the model expects
+        """
+        try:
+            float(date)
+        except ValueError:
+            # Value isn't a float - attempt to extract date from value
+            try:
+                date_format = self.date_format_string
+                if len(str(date)) == DATE_WITH_TIME_LENGTH:
+                    date_format += "(%H:%M:%S)"
+                datetime.strptime(str(date), date_format)
+            except ValueError:
+                current_date_format = self.get_date_format(self.__model.date_format)
+                raise ValueError(
+                    "Invalid date format " + str(date) + " the model is using " + current_date_format + " date format.")
+
+    @staticmethod
+    def get_date_format(date_format: DateFormat) -> str:
+        """Returns the date format being used by the model
+        formats used: ('MM/DD/YYYY', 'DD/MM/YYYY').
+        """
+
+        if date_format is DateFormat.MM_DD_YYYY:
+            return 'MM/DD/YYYY'
+        else:
+            return 'DD/MM/YYYY'
+
+    def __update_times_in_file(self) -> None:
+        """Updates the list of times in the Runcontrol file to the current stored values in __times.
+
+        Returns:
+            None: writes out a file at the same path as the existing runcontrol file
+        """
+        self.__model.check_output_path()
+        if self.__model.model_files.runcontrol_file is None or \
+                self.__model.model_files.runcontrol_file.location is None:
+            raise ValueError(f"No file path found for {self.__model.model_files}")
+        file_content = self.__model.model_files.runcontrol_file.get_flat_list_str_file
+        filename = self.__model.model_files.runcontrol_file.location
+
+        new_file_content = self.__model._sim_controls.delete_times(file_content)
+
+        time_list = self.times
+        stop_string = 'STOP\n'
+        if stop_string in new_file_content:
+            new_file_content.remove(stop_string)
+
+        def prepend_time(s: str) -> str:
+            return "TIME " + s
+
+        time_list = [prepend_time(x) for x in time_list]
+        num_times = len(time_list)
+
+        new_line_list = ["\n\n"] * num_times
+        zipped_list = list(zip(time_list, new_line_list))
+        flat_list = [item for sublist in zipped_list for item in sublist]
+        flat_list.append(stop_string)
+        new_file_content.extend(flat_list)
+        new_file_str = "".join(new_file_content)
+
+        with open(filename, "w") as text_file:
+            text_file.write(new_file_str)
+
+    def load_run_control_file(self):
+        """Loads the run control information into the class instance. \
+            If the write_times attribute is True then it expands out any INCLUDE files with the times found within
+        Raises:
+            ValueError: if the run_control_file attribute is None.
+        """
+        if self.__model.model_files.runcontrol_file is None:
+            warnings.warn(f"Run control file path not found for {self.__model.model_files.location}")
+            return
+        run_control_file_content = self.__model.model_files.runcontrol_file.get_flat_list_str_file
+
+        if (run_control_file_content is None) or (self.__model.model_files.runcontrol_file.location is None):
+            raise ValueError(f"No file path provided for {self.__model.model_files.runcontrol_file.location=}")
+
+        # set the start date
+        for line in run_control_file_content:
+            if nfo.check_token('START', line):
+                value = nfo.get_expected_token_value('START', line, run_control_file_content)
+                if value is not None:
+                    self.__model.start_date = value
+
+        times = []
+        run_control_times = self.get_times(run_control_file_content)
+        times.extend(run_control_times)
+        if self.__model.start_date is None or self.__model.start_date == '':
+            try:
+                self.__model.start_date = times[0]
+            except IndexError:
+                for line in run_control_file_content:
+                    if nfo.check_token('TIME', line):
+                        value = nfo.get_expected_token_value('TIME', line, run_control_file_content)
+                        self.__model.start_date = value
+                        warnings.warn(f'Setting start date to first time card found in the runcontrol file as: {value}')
+                        break
+                warnings.warn('No value found for start date explicitly with START or TIME card')
+
+        self.__times = self.sort_remove_duplicate_times(times)
+
+        # If we don't want to write the times, return here.
+        if not self.__model.write_times:
+            return
+        if self.__model.model_files.runcontrol_file.include_locations is None:
+            warnings.warn(f'No includes files found in {self.__model.model_files.runcontrol_file.location}')
+            return
+        for file in self.__model.model_files.runcontrol_file.include_locations:
+            if self.__model.destination is not None:
+                self.remove_times_from_file(run_control_file_content, file)
+
+        self.modify_times(content=times, operation='replace')
+
+    def modify_times(self, content: Optional[list[str]] = None, operation: str = 'merge'):
+        """Modifies the output times in the simulation.
+
+        Args:
+        ----
+            content (list[str]], optional): The content to modify using the above operation, \
+            represented as a list of strings with a new entry per line of the file. Defaults to None.
+            operation (str, optional): operation to perform on the content provided (e.g. 'merge'). Defaults to 'merge'.
+
+        Raises:
+        ------
+            ValueError: if the supplied dates are before the start date of the simulation
+        """
+        if content is None:
+            content = []
+        for time in content:
+            self.check_date_format(time)
+
+        new_times = self.sort_remove_duplicate_times(content)
+        if len(new_times) > 0 > self.compare_dates(new_times[0], self.__model.start_date):
+            raise ValueError(
+                f"The supplied date of {new_times[0]} precedes the start date of {self.__model.start_date}")
+        operation = operation.lower()
+        self.__times = self.__times if self.__times is not None else []
+
+        if operation == 'merge':
+            self.__times.extend(content)
+        elif operation == 'replace':
+            self.__times = content
+        elif operation == 'reset':
+            self.__times = []
+        elif operation == 'remove':
+            for time in content:
+                if time in self.__times:
+                    self.__times.remove(time)
+
+        self.__times = self.sort_remove_duplicate_times(self.__times)
+
+        if self.__model.destination is not None:
+            self.__update_times_in_file()
```

### Comparing `ressimpy-1.0.0/ResSimpy/Nexus/structured_grid_operations.py` & `ressimpy-1.0.1/ResSimpy/Nexus/structured_grid_operations.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,192 +1,192 @@
-from __future__ import annotations
-from typing import Optional, TYPE_CHECKING
-from ResSimpy.Grid import VariableEntry
-import ResSimpy.Nexus.nexus_file_operations as nfo
-
-if TYPE_CHECKING:
-    from ResSimpy.Nexus.NexusSimulator import NexusSimulator
-
-
-class StructuredGridOperations:
-    def __init__(self, model: NexusSimulator) -> None:
-        self.__model: NexusSimulator = model
-
-    @staticmethod
-    def load_token_value_if_present(token: str, modifier: str, token_property: VariableEntry,
-                                    line: str, file_as_list: list[str],
-                                    ignore_values: Optional[list[str]] = None) -> None:
-        """Gets a token's value if there is one and loads it into the token_property.
-
-        Args:
-        ----
-            token (str): the token being searched for. e.g. 'PERMX'
-            modifier (str): any modifiers applied to the token e.g. 'MULT'
-            token_property (VariableEntry): VariableEntry object to store the modifier and value pair into
-            line (str): line to search for the token in
-            ignore_values (Optional[list[str]], optional): values to be ignored. Defaults to None.
-
-        Raises:
-        ------
-            ValueError: raises an error if no numerical value can be found after the supplied token modifier pair
-        Returns:
-            None: stores the value into token_property supplied instead
-        """
-
-        if ignore_values is None:
-            ignore_values = []
-        token_modifier = f"{token} {modifier}"
-
-        if nfo.check_token(token, line) and nfo.get_token_value(token, line, file_as_list) == modifier:
-            # If we are loading a multiple, load the two relevant values, otherwise just the next value
-            if modifier == 'MULT':
-                numerical_value = nfo.get_expected_token_value(token_modifier, line, file_as_list, ignore_values=None)
-                if numerical_value is None:
-                    raise ValueError(
-                        f'No numerical value found after {token_modifier} keyword in line: {line}')
-                value_to_multiply = nfo.get_token_value(token_modifier, line, file_as_list,
-                                                        ignore_values=[numerical_value])
-                if numerical_value is not None and value_to_multiply is not None:
-                    token_property.modifier = 'MULT'
-                    token_property.value = f"{numerical_value} {value_to_multiply}"
-            else:
-                value = nfo.get_token_value(token_modifier, line, file_as_list, ignore_values=ignore_values)
-                if value is None:
-                    # Could be 'cut short' by us excluding the rest of a file
-                    token_property.value = None
-                    token_property.modifier = modifier
-                token_property.value = value
-                token_property.modifier = modifier
-
-    @staticmethod
-    def replace_value(file_as_list: list[str], old_property: VariableEntry, new_property: VariableEntry,
-                      token_name: str) -> None:
-        """Replace the value and token + modifier with the new values.
-
-        Args:
-        ----
-            file_as_list (list[str]): a list of strings containing each line of the file as a new entry
-            old_property (VariableEntry): property found in the original file to be replaced
-            new_property (VariableEntry): new property to replace the old property with
-            token_name (str): name of the token being replaced
-        Returns:
-            None: modifies the file_as_list with the new property
-        """
-
-        for line in file_as_list:
-            old_token_modifier = f"{token_name} {old_property.modifier}"
-            new_token_modifier = f"{token_name} {new_property.modifier}"
-            ignore_values = ['INCLUDE'] if old_property.modifier == 'VALUE' else []
-            if nfo.check_token(old_token_modifier, line):
-                # If we are replacing a mult, replace the first value with a blank
-                if old_property.modifier == 'MULT':
-                    dummy_value = VariableEntry('MULT', '')
-                    nfo.get_token_value(old_token_modifier, line, file_as_list, ignore_values=ignore_values,
-                                        replace_with=dummy_value)
-
-                nfo.get_token_value(old_token_modifier, line, file_as_list, ignore_values=ignore_values,
-                                    replace_with=new_property)
-
-                new_line = line.replace(old_token_modifier, new_token_modifier, 1)
-                line_index = file_as_list.index(line)
-                file_as_list[line_index] = new_line
-
-    @staticmethod
-    def append_include_to_grid_file(include_file_location: str, structured_grid_file_path: str) -> None:
-        # TODO: change append to be an optional parameter
-        """Appends an include file to the end of a grid for adding LGRs.
-
-        Args:
-        ----
-            include_file_location (str): path to a file to include in the grid
-            structured_grid_file_path (str): file path to the structured grid.
-
-        Raises:
-        ------
-            ValueError: if no structured grid file path is specified in the class instance
-        """
-        # Get the existing file as a list
-        if structured_grid_file_path is None:
-            raise ValueError("No file path given or found for structured grid file path. \
-                Please update structured grid file path")
-        file = nfo.load_file_as_list(structured_grid_file_path)
-
-        file.append(f"\nINCLUDE {include_file_location}\n")
-        file.append("TOLPV LGR1 0\n")
-
-        # Save the new file contents
-        new_file_str = "".join(file)
-        with open(structured_grid_file_path, "w") as text_file:
-            text_file.write(new_file_str)
-
-    @staticmethod
-    def get_grid_file_as_3d_list(path: str) -> Optional[list]:
-        """Converts a grid file to a 3D list.
-
-        Args:
-        ----
-            path (str): path to a grid file
-
-        Returns:
-        -------
-            Optional[list[str]]: Returns None if no file is found, returns the grid as a 3d array otherwise
-        """
-        try:
-            with open(path) as f:
-                grid_file_list = list(f)
-        except FileNotFoundError:
-            return None
-
-        sub_lists = []
-
-        new_list_str = ""
-        for sub_list in grid_file_list[4:]:
-            if sub_list == '\n':
-                new_list_split = [x.split("\t") for x in new_list_str.split("\n")]
-                new_list_split_cleaned = []
-                for x_list in new_list_split:
-                    float_list_split = [float(x) for x in x_list if x != ""]
-                    new_list_split_cleaned.append(float_list_split)
-                sub_lists.append(new_list_split_cleaned)
-                new_list_str = ""
-            else:
-                new_list_str = new_list_str + sub_list
-        return sub_lists
-
-    def view_command(self, field: str, previous_lines: int = 3, following_lines: int = 3) -> Optional[str]:
-        """Displays how the property is declared in the structured grid file.
-
-        Args:
-        ----
-            field (str): property as written in the structured grid (e.g. KX)
-            previous_lines (int, optional): how many lines to look back from the field searched for. Defaults to 3.
-            following_lines (int, optional): how many lines to look forward from the field searched for. Defaults to 3.
-
-        Raises:
-        ------
-            ValueError: if no structured grid file path is specified in the class instance
-
-        Returns:
-        -------
-            Optional[str]: the string associated with the supplied property from within the structured grid. \
-                If the field is not found in the structured grid returns None.
-        """
-        structured_grid_dict = self.__model.get_structured_grid_dict()
-        structured_grid_path = self.__model.structured_grid_path
-        command_token = f"{field.upper()} {structured_grid_dict[field.lower()].modifier}"
-        if structured_grid_path is None:
-            raise ValueError("No path found for structured grid file path. \
-                Please provide a path to the structured grid")
-        file_as_list = nfo.load_file_as_list(structured_grid_path)
-
-        for line in file_as_list:
-            if nfo.check_token(command_token, line):
-                start_index = file_as_list.index(line) - previous_lines \
-                    if file_as_list.index(line) - previous_lines > 0 else 0
-                end_index = file_as_list.index(line) + following_lines \
-                    if file_as_list.index(line) + following_lines < len(file_as_list) else len(file_as_list) - 1
-
-                new_array = file_as_list[start_index: end_index]
-                new_array = [x.strip("'") for x in new_array]
-                value = "".join(new_array)
-                return value
-        return None
+from __future__ import annotations
+from typing import Optional, TYPE_CHECKING
+from ResSimpy.Grid import VariableEntry
+import ResSimpy.Nexus.nexus_file_operations as nfo
+
+if TYPE_CHECKING:
+    from ResSimpy.Nexus.NexusSimulator import NexusSimulator
+
+
+class StructuredGridOperations:
+    def __init__(self, model: NexusSimulator) -> None:
+        self.__model: NexusSimulator = model
+
+    @staticmethod
+    def load_token_value_if_present(token: str, modifier: str, token_property: VariableEntry,
+                                    line: str, file_as_list: list[str],
+                                    ignore_values: Optional[list[str]] = None) -> None:
+        """Gets a token's value if there is one and loads it into the token_property.
+
+        Args:
+        ----
+            token (str): the token being searched for. e.g. 'PERMX'
+            modifier (str): any modifiers applied to the token e.g. 'MULT'
+            token_property (VariableEntry): VariableEntry object to store the modifier and value pair into
+            line (str): line to search for the token in
+            ignore_values (Optional[list[str]], optional): values to be ignored. Defaults to None.
+
+        Raises:
+        ------
+            ValueError: raises an error if no numerical value can be found after the supplied token modifier pair
+        Returns:
+            None: stores the value into token_property supplied instead
+        """
+
+        if ignore_values is None:
+            ignore_values = []
+        token_modifier = f"{token} {modifier}"
+
+        if nfo.check_token(token, line) and nfo.get_token_value(token, line, file_as_list) == modifier:
+            # If we are loading a multiple, load the two relevant values, otherwise just the next value
+            if modifier == 'MULT':
+                numerical_value = nfo.get_expected_token_value(token_modifier, line, file_as_list, ignore_values=None)
+                if numerical_value is None:
+                    raise ValueError(
+                        f'No numerical value found after {token_modifier} keyword in line: {line}')
+                value_to_multiply = nfo.get_token_value(token_modifier, line, file_as_list,
+                                                        ignore_values=[numerical_value])
+                if numerical_value is not None and value_to_multiply is not None:
+                    token_property.modifier = 'MULT'
+                    token_property.value = f"{numerical_value} {value_to_multiply}"
+            else:
+                value = nfo.get_token_value(token_modifier, line, file_as_list, ignore_values=ignore_values)
+                if value is None:
+                    # Could be 'cut short' by us excluding the rest of a file
+                    token_property.value = None
+                    token_property.modifier = modifier
+                token_property.value = value
+                token_property.modifier = modifier
+
+    @staticmethod
+    def replace_value(file_as_list: list[str], old_property: VariableEntry, new_property: VariableEntry,
+                      token_name: str) -> None:
+        """Replace the value and token + modifier with the new values.
+
+        Args:
+        ----
+            file_as_list (list[str]): a list of strings containing each line of the file as a new entry
+            old_property (VariableEntry): property found in the original file to be replaced
+            new_property (VariableEntry): new property to replace the old property with
+            token_name (str): name of the token being replaced
+        Returns:
+            None: modifies the file_as_list with the new property
+        """
+
+        for line in file_as_list:
+            old_token_modifier = f"{token_name} {old_property.modifier}"
+            new_token_modifier = f"{token_name} {new_property.modifier}"
+            ignore_values = ['INCLUDE'] if old_property.modifier == 'VALUE' else []
+            if nfo.check_token(old_token_modifier, line):
+                # If we are replacing a mult, replace the first value with a blank
+                if old_property.modifier == 'MULT':
+                    dummy_value = VariableEntry('MULT', '')
+                    nfo.get_token_value(old_token_modifier, line, file_as_list, ignore_values=ignore_values,
+                                        replace_with=dummy_value)
+
+                nfo.get_token_value(old_token_modifier, line, file_as_list, ignore_values=ignore_values,
+                                    replace_with=new_property)
+
+                new_line = line.replace(old_token_modifier, new_token_modifier, 1)
+                line_index = file_as_list.index(line)
+                file_as_list[line_index] = new_line
+
+    @staticmethod
+    def append_include_to_grid_file(include_file_location: str, structured_grid_file_path: str) -> None:
+        # TODO: change append to be an optional parameter
+        """Appends an include file to the end of a grid for adding LGRs.
+
+        Args:
+        ----
+            include_file_location (str): path to a file to include in the grid
+            structured_grid_file_path (str): file path to the structured grid.
+
+        Raises:
+        ------
+            ValueError: if no structured grid file path is specified in the class instance
+        """
+        # Get the existing file as a list
+        if structured_grid_file_path is None:
+            raise ValueError("No file path given or found for structured grid file path. \
+                Please update structured grid file path")
+        file = nfo.load_file_as_list(structured_grid_file_path)
+
+        file.append(f"\nINCLUDE {include_file_location}\n")
+        file.append("TOLPV LGR1 0\n")
+
+        # Save the new file contents
+        new_file_str = "".join(file)
+        with open(structured_grid_file_path, "w") as text_file:
+            text_file.write(new_file_str)
+
+    @staticmethod
+    def get_grid_file_as_3d_list(path: str) -> Optional[list]:
+        """Converts a grid file to a 3D list.
+
+        Args:
+        ----
+            path (str): path to a grid file
+
+        Returns:
+        -------
+            Optional[list[str]]: Returns None if no file is found, returns the grid as a 3d array otherwise
+        """
+        try:
+            with open(path) as f:
+                grid_file_list = list(f)
+        except FileNotFoundError:
+            return None
+
+        sub_lists = []
+
+        new_list_str = ""
+        for sub_list in grid_file_list[4:]:
+            if sub_list == '\n':
+                new_list_split = [x.split("\t") for x in new_list_str.split("\n")]
+                new_list_split_cleaned = []
+                for x_list in new_list_split:
+                    float_list_split = [float(x) for x in x_list if x != ""]
+                    new_list_split_cleaned.append(float_list_split)
+                sub_lists.append(new_list_split_cleaned)
+                new_list_str = ""
+            else:
+                new_list_str = new_list_str + sub_list
+        return sub_lists
+
+    def view_command(self, field: str, previous_lines: int = 3, following_lines: int = 3) -> Optional[str]:
+        """Displays how the property is declared in the structured grid file.
+
+        Args:
+        ----
+            field (str): property as written in the structured grid (e.g. KX)
+            previous_lines (int, optional): how many lines to look back from the field searched for. Defaults to 3.
+            following_lines (int, optional): how many lines to look forward from the field searched for. Defaults to 3.
+
+        Raises:
+        ------
+            ValueError: if no structured grid file path is specified in the class instance
+
+        Returns:
+        -------
+            Optional[str]: the string associated with the supplied property from within the structured grid. \
+                If the field is not found in the structured grid returns None.
+        """
+        structured_grid_dict = self.__model.get_structured_grid_dict()
+        structured_grid_path = self.__model.structured_grid_path
+        command_token = f"{field.upper()} {structured_grid_dict[field.lower()].modifier}"
+        if structured_grid_path is None:
+            raise ValueError("No path found for structured grid file path. \
+                Please provide a path to the structured grid")
+        file_as_list = nfo.load_file_as_list(structured_grid_path)
+
+        for line in file_as_list:
+            if nfo.check_token(command_token, line):
+                start_index = file_as_list.index(line) - previous_lines \
+                    if file_as_list.index(line) - previous_lines > 0 else 0
+                end_index = file_as_list.index(line) + following_lines \
+                    if file_as_list.index(line) + following_lines < len(file_as_list) else len(file_as_list) - 1
+
+                new_array = file_as_list[start_index: end_index]
+                new_array = [x.strip("'") for x in new_array]
+                value = "".join(new_array)
+                return value
+        return None
```

### Comparing `ressimpy-1.0.0/ResSimpy/Node.py` & `ressimpy-1.0.1/ResSimpy/Node.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-from __future__ import annotations
-
-import uuid
-from abc import ABC
-from dataclasses import dataclass, field
-from typing import Optional
-
-from ResSimpy.Enums.UnitsEnum import UnitSystem
-
-
-@dataclass
-class Node(ABC):
-    name: Optional[str] = None
-    type: Optional[str] = None
-    depth: Optional[float] = None
-    date: Optional[str] = None
-    unit_system: Optional[UnitSystem] = None
-    __id: uuid.UUID = field(default_factory=lambda: uuid.uuid4(), compare=False)
-
-    def to_dict(self) -> dict:
-        raise NotImplementedError("Implement this in the derived class")
-
-    def to_table_line(self, headers: list[str]) -> str:
-        raise NotImplementedError("Implement this in the derived class")
-
-    @property
-    def id(self) -> uuid.UUID:
-        """Unique identifier for each Node object."""
-        return self.__id
+from __future__ import annotations
+
+import uuid
+from abc import ABC
+from dataclasses import dataclass, field
+from typing import Optional
+
+from ResSimpy.Enums.UnitsEnum import UnitSystem
+
+
+@dataclass
+class Node(ABC):
+    name: Optional[str] = None
+    type: Optional[str] = None
+    depth: Optional[float] = None
+    date: Optional[str] = None
+    unit_system: Optional[UnitSystem] = None
+    __id: uuid.UUID = field(default_factory=lambda: uuid.uuid4(), compare=False)
+
+    def to_dict(self) -> dict:
+        raise NotImplementedError("Implement this in the derived class")
+
+    def to_table_line(self, headers: list[str]) -> str:
+        raise NotImplementedError("Implement this in the derived class")
+
+    @property
+    def id(self) -> uuid.UUID:
+        """Unique identifier for each Node object."""
+        return self.__id
```

### Comparing `ressimpy-1.0.0/ResSimpy/RelPermEndPoint.py` & `ressimpy-1.0.1/ResSimpy/RelPermEndPoint.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,87 +1,87 @@
-from dataclasses import dataclass
-from abc import ABC
-from typing import Optional
-
-
-@dataclass
-class RelPermEndPoint(ABC):
-    __swl: Optional[float] = None
-    __swr: Optional[float] = None
-    __swu: Optional[float] = None
-    __sgl: Optional[float] = None
-    __sgr: Optional[float] = None
-    __sgu: Optional[float] = None
-    __swro: Optional[float] = None
-    __sgro: Optional[float] = None
-    __sgrw: Optional[float] = None
-    __krw_swro: Optional[float] = None
-    __krw_swu: Optional[float] = None
-    __krg_sgro: Optional[float] = None
-    __krg_sgu: Optional[float] = None
-    __kro_swl: Optional[float] = None
-    __kro_swr: Optional[float] = None
-    __kro_sgl: Optional[float] = None
-    __kro_sgr: Optional[float] = None
-    __krw_sgl: Optional[float] = None
-    __krw_sgr: Optional[float] = None
-    __krg_sgrw: Optional[float] = None
-    __sgtr: Optional[float] = None
-    __sotr: Optional[float] = None
-
-    def __init__(self, swl: Optional[float] = None, swr: Optional[float] = None, swu: Optional[float] = None,
-                 sgl: Optional[float] = None, sgr: Optional[float] = None, sgu: Optional[float] = None,
-                 swro: Optional[float] = None, sgro: Optional[float] = None, sgrw: Optional[float] = None,
-                 krw_swro: Optional[float] = None, krw_swu: Optional[float] = None, krg_sgro: Optional[float] = None,
-                 krg_sgu: Optional[float] = None, kro_swl: Optional[float] = None, kro_swr: Optional[float] = None,
-                 kro_sgl: Optional[float] = None, kro_sgr: Optional[float] = None, krw_sgl: Optional[float] = None,
-                 krw_sgr: Optional[float] = None, krg_sgrw: Optional[float] = None, sgtr: Optional[float] = None,
-                 sotr: Optional[float] = None) -> None:
-        self.__swl = swl
-        self.__swr = swr
-        self.__swu = swu
-        self.__sgl = sgl
-        self.__sgr = sgr
-        self.__sgu = sgu
-        self.__swro = swro
-        self.__sgro = sgro
-        self.__sgrw = sgrw
-        self.__krw_swro = krw_swro
-        self.__krw_swu = krw_swu
-        self.__krg_sgro = krg_sgro
-        self.__krg_sgu = krg_sgu
-        self.__kro_swl = kro_swl
-        self.__kro_swr = kro_swr
-        self.__kro_sgl = kro_sgl
-        self.__kro_sgr = kro_sgr
-        self.__krw_sgl = krw_sgl
-        self.__krw_sgr = krw_sgr
-        self.__krg_sgrw = krg_sgrw
-        self.__sgtr = sgtr
-        self.__sotr = sotr
-
-    def to_dict(self) -> dict[str, Optional[float]]:
-        attribute_dict: dict[str, Optional[float]] = {
-            'swl': self.__swl,
-            'swr': self.__swr,
-            'swu': self.__swu,
-            'sgl': self.__sgl,
-            'sgr': self.__sgr,
-            'sgu': self.__sgu,
-            'swro': self.__swro,
-            'sgro': self.__sgro,
-            'sgrw': self.__sgrw,
-            'krw_swro': self.__krw_swro,
-            'krw_swu': self.__krw_swu,
-            'krg_sgro': self.__krg_sgro,
-            'krg_sgu': self.__krg_sgu,
-            'kro_swl': self.__kro_swl,
-            'kro_swr': self.__kro_swr,
-            'kro_sgl': self.__kro_sgl,
-            'kro_sgr': self.__kro_sgr,
-            'krw_sgl': self.__krw_sgl,
-            'krw_sgr': self.__krw_sgr,
-            'krg_sgrw': self.__krg_sgrw,
-            'sgtr': self.__sgtr,
-            'sotr': self.__sotr,
-        }
-        return attribute_dict
+from dataclasses import dataclass
+from abc import ABC
+from typing import Optional
+
+
+@dataclass
+class RelPermEndPoint(ABC):
+    __swl: Optional[float] = None
+    __swr: Optional[float] = None
+    __swu: Optional[float] = None
+    __sgl: Optional[float] = None
+    __sgr: Optional[float] = None
+    __sgu: Optional[float] = None
+    __swro: Optional[float] = None
+    __sgro: Optional[float] = None
+    __sgrw: Optional[float] = None
+    __krw_swro: Optional[float] = None
+    __krw_swu: Optional[float] = None
+    __krg_sgro: Optional[float] = None
+    __krg_sgu: Optional[float] = None
+    __kro_swl: Optional[float] = None
+    __kro_swr: Optional[float] = None
+    __kro_sgl: Optional[float] = None
+    __kro_sgr: Optional[float] = None
+    __krw_sgl: Optional[float] = None
+    __krw_sgr: Optional[float] = None
+    __krg_sgrw: Optional[float] = None
+    __sgtr: Optional[float] = None
+    __sotr: Optional[float] = None
+
+    def __init__(self, swl: Optional[float] = None, swr: Optional[float] = None, swu: Optional[float] = None,
+                 sgl: Optional[float] = None, sgr: Optional[float] = None, sgu: Optional[float] = None,
+                 swro: Optional[float] = None, sgro: Optional[float] = None, sgrw: Optional[float] = None,
+                 krw_swro: Optional[float] = None, krw_swu: Optional[float] = None, krg_sgro: Optional[float] = None,
+                 krg_sgu: Optional[float] = None, kro_swl: Optional[float] = None, kro_swr: Optional[float] = None,
+                 kro_sgl: Optional[float] = None, kro_sgr: Optional[float] = None, krw_sgl: Optional[float] = None,
+                 krw_sgr: Optional[float] = None, krg_sgrw: Optional[float] = None, sgtr: Optional[float] = None,
+                 sotr: Optional[float] = None) -> None:
+        self.__swl = swl
+        self.__swr = swr
+        self.__swu = swu
+        self.__sgl = sgl
+        self.__sgr = sgr
+        self.__sgu = sgu
+        self.__swro = swro
+        self.__sgro = sgro
+        self.__sgrw = sgrw
+        self.__krw_swro = krw_swro
+        self.__krw_swu = krw_swu
+        self.__krg_sgro = krg_sgro
+        self.__krg_sgu = krg_sgu
+        self.__kro_swl = kro_swl
+        self.__kro_swr = kro_swr
+        self.__kro_sgl = kro_sgl
+        self.__kro_sgr = kro_sgr
+        self.__krw_sgl = krw_sgl
+        self.__krw_sgr = krw_sgr
+        self.__krg_sgrw = krg_sgrw
+        self.__sgtr = sgtr
+        self.__sotr = sotr
+
+    def to_dict(self) -> dict[str, Optional[float]]:
+        attribute_dict: dict[str, Optional[float]] = {
+            'swl': self.__swl,
+            'swr': self.__swr,
+            'swu': self.__swu,
+            'sgl': self.__sgl,
+            'sgr': self.__sgr,
+            'sgu': self.__sgu,
+            'swro': self.__swro,
+            'sgro': self.__sgro,
+            'sgrw': self.__sgrw,
+            'krw_swro': self.__krw_swro,
+            'krw_swu': self.__krw_swu,
+            'krg_sgro': self.__krg_sgro,
+            'krg_sgu': self.__krg_sgu,
+            'kro_swl': self.__kro_swl,
+            'kro_swr': self.__kro_swr,
+            'kro_sgl': self.__kro_sgl,
+            'kro_sgr': self.__kro_sgr,
+            'krw_sgl': self.__krw_sgl,
+            'krw_sgr': self.__krw_sgr,
+            'krg_sgrw': self.__krg_sgrw,
+            'sgtr': self.__sgtr,
+            'sotr': self.__sotr,
+        }
+        return attribute_dict
```

### Comparing `ressimpy-1.0.0/ResSimpy/Utils/factory_methods.py` & `ressimpy-1.0.1/ResSimpy/Utils/factory_methods.py`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,65 +1,65 @@
-from __future__ import annotations
-from enum import Enum
-from typing import TYPE_CHECKING, Union
-from uuid import UUID
-
-import pandas as pd
-
-if TYPE_CHECKING:
-    from ResSimpy.Nexus.DataModels.NexusFile import NexusFile
-    from ResSimpy.Nexus.DataModels.NexusWaterMethod import NexusWaterParams
-
-
-# Factory methods for generating empty lists with typing
-def get_empty_list_str() -> list[str]:
-    value: list[str] = []
-    return value
-
-
-# Factory method for generating empty dictionary with typing
-def get_empty_dict_union() -> dict[str, Union[str, int, float, Enum, list[str], pd.DataFrame,
-                                   dict[str, Union[float, pd.DataFrame]]]]:
-    value: dict[str, Union[str, int, float, Enum, list[str], pd.DataFrame, dict[str, Union[float, pd.DataFrame]]]] = {}
-    return value
-
-
-# Factory method for generating empty dictionary for eos options
-def get_empty_eosopt_dict_union() -> \
-        dict[str, Union[str, int, float, pd.DataFrame, list[str], dict[str, float], tuple[str, dict[str, float]], dict[
-            str, pd.DataFrame]]]:
-    value: dict[str, Union[
-        str, int, float, pd.DataFrame, list[str], dict[str, float], tuple[str, dict[str, float]], dict[
-            str, pd.DataFrame]]] = {}
-    return value
-
-
-# Factory method for generating empty dictionary for hysteresis parameters
-def get_empty_hysteresis_dict() -> dict[str, Union[str, float, dict[str,
-                                        Union[str, float, dict[str, Union[str, float]]]]]]:
-    value: dict[str, Union[str, float, dict[str, Union[str, float, dict[str, Union[str, float]]]]]] = {}
-    return value
-
-
-def get_empty_list_str_nexus_file() -> list[Union[str, NexusFile]]:
-    value: list[Union[str, NexusFile]] = []
-    return value
-
-
-def get_empty_list_nexus_file() -> list[NexusFile]:
-    value: list[NexusFile] = []
-    return value
-
-
-def get_empty_dict_int_nexus_file() -> dict[int, NexusFile]:
-    value: dict[int, NexusFile] = {}
-    return value
-
-
-def get_empty_dict_uuid_list_int() -> dict[UUID, list[int]]:
-    value: dict[UUID, list[int]] = {}
-    return value
-
-
-def get_empty_list_nexus_water_params() -> list[NexusWaterParams]:
-    value: list[NexusWaterParams] = []
-    return value
+from __future__ import annotations
+from enum import Enum
+from typing import TYPE_CHECKING, Union
+from uuid import UUID
+
+import pandas as pd
+
+if TYPE_CHECKING:
+    from ResSimpy.Nexus.DataModels.NexusFile import NexusFile
+    from ResSimpy.Nexus.DataModels.NexusWaterMethod import NexusWaterParams
+
+
+# Factory methods for generating empty lists with typing
+def get_empty_list_str() -> list[str]:
+    value: list[str] = []
+    return value
+
+
+# Factory method for generating empty dictionary with typing
+def get_empty_dict_union() -> dict[str, Union[str, int, float, Enum, list[str], pd.DataFrame,
+                                   dict[str, Union[float, pd.DataFrame]]]]:
+    value: dict[str, Union[str, int, float, Enum, list[str], pd.DataFrame, dict[str, Union[float, pd.DataFrame]]]] = {}
+    return value
+
+
+# Factory method for generating empty dictionary for eos options
+def get_empty_eosopt_dict_union() -> \
+        dict[str, Union[str, int, float, pd.DataFrame, list[str], dict[str, float], tuple[str, dict[str, float]], dict[
+            str, pd.DataFrame]]]:
+    value: dict[str, Union[
+        str, int, float, pd.DataFrame, list[str], dict[str, float], tuple[str, dict[str, float]], dict[
+            str, pd.DataFrame]]] = {}
+    return value
+
+
+# Factory method for generating empty dictionary for hysteresis parameters
+def get_empty_hysteresis_dict() -> dict[str, Union[str, float, dict[str,
+                                        Union[str, float, dict[str, Union[str, float]]]]]]:
+    value: dict[str, Union[str, float, dict[str, Union[str, float, dict[str, Union[str, float]]]]]] = {}
+    return value
+
+
+def get_empty_list_str_nexus_file() -> list[Union[str, NexusFile]]:
+    value: list[Union[str, NexusFile]] = []
+    return value
+
+
+def get_empty_list_nexus_file() -> list[NexusFile]:
+    value: list[NexusFile] = []
+    return value
+
+
+def get_empty_dict_int_nexus_file() -> dict[int, NexusFile]:
+    value: dict[int, NexusFile] = {}
+    return value
+
+
+def get_empty_dict_uuid_list_int() -> dict[UUID, list[int]]:
+    value: dict[UUID, list[int]] = {}
+    return value
+
+
+def get_empty_list_nexus_water_params() -> list[NexusWaterParams]:
+    value: list[NexusWaterParams] = []
+    return value
```

### Comparing `ressimpy-1.0.0/ResSimpy/Utils/generic_repr.py` & `ressimpy-1.0.1/ResSimpy/Utils/generic_repr.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-from typing import Any
-
-
-def generic_repr(input_class: Any) -> str:
-    """Creates a prettier object representation while removing attributes that are None from that
-    representation.
-
-    Args:
-    ----
-        input_class (Any): a class with attributes to summarise
-
-    Returns:
-    -------
-        (str): Pretty representation of the string.
-    """
-    filtered_attrs = {k: v for k, v in vars(input_class).items() if v is not None}
-    attrs = ', '.join(f"{k}={v!r}" for k, v in filtered_attrs.items())
-    return f"{input_class.__class__.__name__}({attrs})"
+from typing import Any
+
+
+def generic_repr(input_class: Any) -> str:
+    """Creates a prettier object representation while removing attributes that are None from that
+    representation.
+
+    Args:
+    ----
+        input_class (Any): a class with attributes to summarise
+
+    Returns:
+    -------
+        (str): Pretty representation of the string.
+    """
+    filtered_attrs = {k: v for k, v in vars(input_class).items() if v is not None}
+    attrs = ', '.join(f"{k}={v!r}" for k, v in filtered_attrs.items())
+    return f"{input_class.__class__.__name__}({attrs})"
```

### Comparing `ressimpy-1.0.0/ResSimpy/Utils/invert_nexus_map.py` & `ressimpy-1.0.1/ResSimpy/Utils/invert_nexus_map.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-def invert_nexus_map(nexus_mapping: dict[str, tuple[str, type]]) -> dict[str, str]:
-    r"""Takes a nexus map of the form {NEXUS KEYWORD: ('attribute_name', type), ...} and reverses it to
-    give a map from attribute names to Nexus Keywords.
-
-    Args:
-    ----
-        nexus_mapping (dict[str, tuple[str, type]]): dictionary of the form \n
-        {NEXUS KEYWORD: ('attribute_name', type), ...}
-
-    Returns:
-    -------
-        dict[str, str] of the form {'attribute_name': 'NEXUS_KEYWORD'}
-
-    """
-    inverted_nexus_map = {v[0]: k for k, v in nexus_mapping.items()}
-    return inverted_nexus_map
-
-
-def nexus_keyword_to_attribute_name(nexus_mapping: dict[str, tuple[str, type]], nexus_keyword: str) -> str:
-    """Takes a Nexus Keyword and maps to the corresponding attribute name from a given nexus mapping."""
-    attribute_name_tuple = nexus_mapping.get(nexus_keyword.upper(), None)
-    if attribute_name_tuple is None:
-        raise AttributeError(f'No nexus keyword found named "{nexus_keyword.upper()}" in the provided nexus mapping')
-    return attribute_name_tuple[0]
-
-
-def attribute_name_to_nexus_keyword(nexus_mapping: dict[str, tuple[str, type]], attribute_name: str) -> str:
-    """Takes an attribute name and maps to the corresponding nexus keyword from a given nexus mapping."""
-
-    invert_map = invert_nexus_map(nexus_mapping)
-    nexus_keyword = invert_map.get(attribute_name.lower(), None)
-    if nexus_keyword is None:
-        raise AttributeError(f'No attribute found with name {attribute_name.lower()} in the provided nexus mapping')
-    return nexus_keyword
+def invert_nexus_map(nexus_mapping: dict[str, tuple[str, type]]) -> dict[str, str]:
+    r"""Takes a nexus map of the form {NEXUS KEYWORD: ('attribute_name', type), ...} and reverses it to
+    give a map from attribute names to Nexus Keywords.
+
+    Args:
+    ----
+        nexus_mapping (dict[str, tuple[str, type]]): dictionary of the form \n
+        {NEXUS KEYWORD: ('attribute_name', type), ...}
+
+    Returns:
+    -------
+        dict[str, str] of the form {'attribute_name': 'NEXUS_KEYWORD'}
+
+    """
+    inverted_nexus_map = {v[0]: k for k, v in nexus_mapping.items()}
+    return inverted_nexus_map
+
+
+def nexus_keyword_to_attribute_name(nexus_mapping: dict[str, tuple[str, type]], nexus_keyword: str) -> str:
+    """Takes a Nexus Keyword and maps to the corresponding attribute name from a given nexus mapping."""
+    attribute_name_tuple = nexus_mapping.get(nexus_keyword.upper(), None)
+    if attribute_name_tuple is None:
+        raise AttributeError(f'No nexus keyword found named "{nexus_keyword.upper()}" in the provided nexus mapping')
+    return attribute_name_tuple[0]
+
+
+def attribute_name_to_nexus_keyword(nexus_mapping: dict[str, tuple[str, type]], attribute_name: str) -> str:
+    """Takes an attribute name and maps to the corresponding nexus keyword from a given nexus mapping."""
+
+    invert_map = invert_nexus_map(nexus_mapping)
+    nexus_keyword = invert_map.get(attribute_name.lower(), None)
+    if nexus_keyword is None:
+        raise AttributeError(f'No attribute found with name {attribute_name.lower()} in the provided nexus mapping')
+    return nexus_keyword
```

### Comparing `ressimpy-1.0.0/ResSimpy/Utils/obj_to_table_string.py` & `ressimpy-1.0.1/ResSimpy/Utils/obj_to_table_string.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-from typing import Any
-
-from ResSimpy.Utils.invert_nexus_map import nexus_keyword_to_attribute_name
-
-
-def to_table_line(obj: Any, headers: list[str]) -> str:
-    """Takes a generic Nexus object and returns the attribute values as a string in the order of headers provided.
-    Requires an implemented to_dict method and get_nexus_mapping() method.
-
-    Args:
-        obj (Any): a NexusObject with a to_dict and get_nexus_mapping method.
-        headers (list[str]): list of header values in Nexus keyword format
-
-    Returns:
-        string of the values in the order of the headers provided.
-
-    """
-    nexus_mapping = obj.get_nexus_mapping()
-    properties = obj.to_dict()
-
-    constructed_values = []
-    for header in headers:
-        attribute_name = nexus_keyword_to_attribute_name(nexus_mapping, header)
-        attribute_value = properties[attribute_name]
-        if attribute_value is None:
-            attribute_value = 'NA'
-        constructed_values.append(attribute_value)
-    return ' '.join([str(x) for x in constructed_values]) + '\n'
+from typing import Any
+
+from ResSimpy.Utils.invert_nexus_map import nexus_keyword_to_attribute_name
+
+
+def to_table_line(obj: Any, headers: list[str]) -> str:
+    """Takes a generic Nexus object and returns the attribute values as a string in the order of headers provided.
+    Requires an implemented to_dict method and get_nexus_mapping() method.
+
+    Args:
+        obj (Any): a NexusObject with a to_dict and get_nexus_mapping method.
+        headers (list[str]): list of header values in Nexus keyword format
+
+    Returns:
+        string of the values in the order of the headers provided.
+
+    """
+    nexus_mapping = obj.get_nexus_mapping()
+    properties = obj.to_dict()
+
+    constructed_values = []
+    for header in headers:
+        attribute_name = nexus_keyword_to_attribute_name(nexus_mapping, header)
+        attribute_value = properties[attribute_name]
+        if attribute_value is None:
+            attribute_value = 'NA'
+        constructed_values.append(attribute_value)
+    return ' '.join([str(x) for x in constructed_values]) + '\n'
```

### Comparing `ressimpy-1.0.0/ResSimpy/Utils/to_dict_generic.py` & `ressimpy-1.0.1/ResSimpy/Utils/to_dict_generic.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,49 +1,49 @@
-from typing import Any
-
-from ResSimpy.Enums.UnitsEnum import UnitSystem
-
-
-def to_dict(nexus_object: Any, keys_in_nexus_style: bool = False, add_date: bool = True, add_units: bool = True,
-            include_nones: bool = True) -> dict[str, None | str | int | float]:
-    """Returns a dictionary of the attributes of a Nexus object. Requires a nexus mapping dictionary.
-        Useful for creating dataframes of objects.
-
-    Args:
-    ----
-        nexus_object (Any): Nexus object with a mapping dictionary defined
-        keys_in_nexus_style (bool): if True returns the key values in Nexus keywords, otherwise returns the
-            attribute name as stored by ressimpy
-        add_date (bool): adds a date attribute if it exists
-        add_units (bool): adds a units attribute if it exists.
-        include_nones (bool): If False filters the nones out of the dictionary. Defaults to True
-
-    Returns:
-    -------
-        a dictionary keyed by attributes and values as the value of the attribute
-    """
-    mapping_dict = nexus_object.get_nexus_mapping()
-    if keys_in_nexus_style:
-        result_dict = {x: nexus_object.__getattribute__(y[0]) for x, y in mapping_dict.items()}
-
-    else:
-        result_dict = {y[0]: nexus_object.__getattribute__(y[0]) for y in mapping_dict.values()}
-
-    if add_date:
-        try:
-            result_dict['date'] = getattr(nexus_object, 'date')
-        except AttributeError:
-            raise AttributeError('Date was requested from the object but does not have a date associated with it.'
-                                 f'Try setting add_date to False. Full contents of object: {nexus_object}')
-    if add_units:
-        try:
-            unit_sys = getattr(nexus_object, 'unit_system')
-        except AttributeError:
-            raise AttributeError(
-                'Unit system was requested from the object but does not have a unit system associated with it.'
-                f'Try setting add_units to False. Full contents of the object: {nexus_object}')
-        if isinstance(unit_sys, UnitSystem):
-            result_dict['unit_system'] = unit_sys.value
-
-    if not include_nones:
-        result_dict = {k: v for k, v in result_dict.items() if v is not None}
-    return result_dict
+from typing import Any
+
+from ResSimpy.Enums.UnitsEnum import UnitSystem
+
+
+def to_dict(nexus_object: Any, keys_in_nexus_style: bool = False, add_date: bool = True, add_units: bool = True,
+            include_nones: bool = True) -> dict[str, None | str | int | float]:
+    """Returns a dictionary of the attributes of a Nexus object. Requires a nexus mapping dictionary.
+        Useful for creating dataframes of objects.
+
+    Args:
+    ----
+        nexus_object (Any): Nexus object with a mapping dictionary defined
+        keys_in_nexus_style (bool): if True returns the key values in Nexus keywords, otherwise returns the
+            attribute name as stored by ressimpy
+        add_date (bool): adds a date attribute if it exists
+        add_units (bool): adds a units attribute if it exists.
+        include_nones (bool): If False filters the nones out of the dictionary. Defaults to True
+
+    Returns:
+    -------
+        a dictionary keyed by attributes and values as the value of the attribute
+    """
+    mapping_dict = nexus_object.get_nexus_mapping()
+    if keys_in_nexus_style:
+        result_dict = {x: nexus_object.__getattribute__(y[0]) for x, y in mapping_dict.items()}
+
+    else:
+        result_dict = {y[0]: nexus_object.__getattribute__(y[0]) for y in mapping_dict.values()}
+
+    if add_date:
+        try:
+            result_dict['date'] = getattr(nexus_object, 'date')
+        except AttributeError:
+            raise AttributeError('Date was requested from the object but does not have a date associated with it.'
+                                 f'Try setting add_date to False. Full contents of object: {nexus_object}')
+    if add_units:
+        try:
+            unit_sys = getattr(nexus_object, 'unit_system')
+        except AttributeError:
+            raise AttributeError(
+                'Unit system was requested from the object but does not have a unit system associated with it.'
+                f'Try setting add_units to False. Full contents of the object: {nexus_object}')
+        if isinstance(unit_sys, UnitSystem):
+            result_dict['unit_system'] = unit_sys.value
+
+    if not include_nones:
+        result_dict = {k: v for k, v in result_dict.items() if v is not None}
+    return result_dict
```

### Comparing `ressimpy-1.0.0/ResSimpy/Wellbore.py` & `ressimpy-1.0.1/ResSimpy/Wellbore.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-from __future__ import annotations
-from abc import ABC
-from dataclasses import dataclass, field
-from typing import Optional
-import uuid
-
-from ResSimpy.Enums.UnitsEnum import UnitSystem
-
-
-@dataclass
-class Wellbore(ABC):
-    date: Optional[str] = None
-    unit_system: Optional[UnitSystem] = None
-    name: Optional[str] = None
-    diameter: Optional[float] = None
-    inner_diameter: Optional[float] = None
-    roughness: Optional[float] = None
-
-    __id: uuid.UUID = field(default_factory=lambda: uuid.uuid4(), compare=False)
-
-    def to_dict(self):
-        raise NotImplementedError("Implement this in the derived class")
-
-    @property
-    def id(self) -> uuid.UUID:
-        """Unique identifier for each Node object."""
-        return self.__id
+from __future__ import annotations
+from abc import ABC
+from dataclasses import dataclass, field
+from typing import Optional
+import uuid
+
+from ResSimpy.Enums.UnitsEnum import UnitSystem
+
+
+@dataclass
+class Wellbore(ABC):
+    date: Optional[str] = None
+    unit_system: Optional[UnitSystem] = None
+    name: Optional[str] = None
+    diameter: Optional[float] = None
+    inner_diameter: Optional[float] = None
+    roughness: Optional[float] = None
+
+    __id: uuid.UUID = field(default_factory=lambda: uuid.uuid4(), compare=False)
+
+    def to_dict(self):
+        raise NotImplementedError("Implement this in the derived class")
+
+    @property
+    def id(self) -> uuid.UUID:
+        """Unique identifier for each Node object."""
+        return self.__id
```

### Comparing `ressimpy-1.0.0/ResSimpy/Wellhead.py` & `ressimpy-1.0.1/ResSimpy/NodeConnection.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,24 @@
-from __future__ import annotations
-from abc import ABC
-from dataclasses import dataclass, field
-from typing import Optional
-import uuid
-
-from ResSimpy.Enums.UnitsEnum import UnitSystem
-
-
-@dataclass
-class Wellhead(ABC):
-    well: Optional[str] = None
-    name: Optional[str] = None
-    date: Optional[str] = None
-    unit_system: Optional[UnitSystem] = None
-    wellhead_type: Optional[str] = None
-    depth: Optional[float] = None
-    x_pos: Optional[float] = None
-    y_pos: Optional[float] = None
-    __id: uuid.UUID = field(default_factory=lambda: uuid.uuid4(), compare=False)
-
-    @property
-    def id(self) -> uuid.UUID:
-        """Unique identifier for each Node object."""
-        return self.__id
-
-    def to_dict(self):
-        raise NotImplementedError("Implement this in the derived class")
+from __future__ import annotations
+from abc import ABC
+from dataclasses import dataclass, field
+from typing import Optional
+import uuid
+
+
+@dataclass
+class NodeConnection(ABC):
+    name: Optional[str] = None
+    date: Optional[str] = None
+    node_in: Optional[str] = None
+    node_out: Optional[str] = None
+    con_type: Optional[str] = None
+    depth: Optional[float] = None
+    __id: uuid.UUID = field(default_factory=lambda: uuid.uuid4(), compare=False)
+
+    def to_dict(self):
+        raise NotImplementedError("Implement this in the derived class")
+
+    @property
+    def id(self) -> uuid.UUID:
+        """Unique identifier for each Node object."""
+        return self.__id
```

