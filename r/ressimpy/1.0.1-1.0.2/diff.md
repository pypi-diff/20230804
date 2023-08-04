# Comparing `tmp/ressimpy-1.0.1.tar.gz` & `tmp/ressimpy-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ressimpy-1.0.1.tar", max compression
+gzip compressed data, was "ressimpy-1.0.2.tar", max compression
```

## Comparing `ressimpy-1.0.1.tar` & `ressimpy-1.0.2.tar`

### file list

```diff
@@ -1,142 +1,143 @@
--rw-r--r--   0        0        0     1521 2023-08-04 13:28:48.983296 ressimpy-1.0.1/README.md
--rw-r--r--   0        0        0      395 2023-08-04 13:28:48.983296 ressimpy-1.0.1/ResSimpy/Aquifer.py
--rw-r--r--   0        0        0     7082 2023-08-04 13:28:48.983296 ressimpy-1.0.1/ResSimpy/Completion.py
--rw-r--r--   0        0        0     1263 2023-08-04 13:28:48.983296 ressimpy-1.0.1/ResSimpy/Constraint.py
--rw-r--r--   0        0        0     1595 2023-08-04 13:28:48.983296 ressimpy-1.0.1/ResSimpy/Constraints.py
--rw-r--r--   0        0        0     1945 2023-08-04 13:28:48.983296 ressimpy-1.0.1/ResSimpy/DynamicProperty.py
--rw-r--r--   0        0        0      168 2023-08-04 13:28:48.983296 ressimpy-1.0.1/ResSimpy/Enums/HowEnum.py
--rw-r--r--   0        0        0      722 2023-08-04 13:28:48.983296 ressimpy-1.0.1/ResSimpy/Enums/UnitsEnum.py
--rw-r--r--   0        0        0       62 2023-08-04 13:28:48.983296 ressimpy-1.0.1/ResSimpy/Enums/__init__.py
--rw-r--r--   0        0        0      413 2023-08-04 13:28:48.983296 ressimpy-1.0.1/ResSimpy/Equilibration.py
--rw-r--r--   0        0        0     2880 2023-08-04 13:28:48.983296 ressimpy-1.0.1/ResSimpy/File.py
--rw-r--r--   0        0        0     2068 2023-08-04 13:28:48.983296 ressimpy-1.0.1/ResSimpy/FileBase.py
--rw-r--r--   0        0        0      413 2023-08-04 13:28:48.983296 ressimpy-1.0.1/ResSimpy/Gaslift.py
--rw-r--r--   0        0        0     2631 2023-08-04 13:28:48.983296 ressimpy-1.0.1/ResSimpy/Grid.py
--rw-r--r--   0        0        0      393 2023-08-04 13:28:48.983296 ressimpy-1.0.1/ResSimpy/Grids.py
--rw-r--r--   0        0        0      404 2023-08-04 13:28:48.983296 ressimpy-1.0.1/ResSimpy/Hydraulics.py
--rw-r--r--   0        0        0     2163 2023-08-04 13:28:48.983296 ressimpy-1.0.1/ResSimpy/ISODateTime.py
--rw-r--r--   0        0        0      462 2023-08-04 13:28:48.983296 ressimpy-1.0.1/ResSimpy/Network.py
--rw-r--r--   0        0        0      545 2023-08-04 13:28:48.983296 ressimpy-1.0.1/ResSimpy/Nexus/DataModels/FcsConfig.py
--rw-r--r--   0        0        0    14289 2023-08-04 13:28:48.983296 ressimpy-1.0.1/ResSimpy/Nexus/DataModels/FcsFile.py
--rw-r--r--   0        0        0    21922 2023-08-04 13:28:48.983296 ressimpy-1.0.1/ResSimpy/Nexus/DataModels/Network/NexusConstraint.py
--rw-r--r--   0        0        0    17042 2023-08-04 13:28:48.983296 ressimpy-1.0.1/ResSimpy/Nexus/DataModels/Network/NexusConstraints.py
--rw-r--r--   0        0        0     2736 2023-08-04 13:28:48.983296 ressimpy-1.0.1/ResSimpy/Nexus/DataModels/Network/NexusNode.py
--rw-r--r--   0        0        0     5011 2023-08-04 13:28:48.983296 ressimpy-1.0.1/ResSimpy/Nexus/DataModels/Network/NexusNodeConnection.py
--rw-r--r--   0        0        0     7241 2023-08-04 13:28:48.983296 ressimpy-1.0.1/ResSimpy/Nexus/DataModels/Network/NexusNodeConnections.py
--rw-r--r--   0        0        0     7327 2023-08-04 13:28:48.983296 ressimpy-1.0.1/ResSimpy/Nexus/DataModels/Network/NexusNodes.py
--rw-r--r--   0        0        0     6821 2023-08-04 13:28:48.983296 ressimpy-1.0.1/ResSimpy/Nexus/DataModels/Network/NexusWellConnection.py
--rw-r--r--   0        0        0     4447 2023-08-04 13:28:48.983296 ressimpy-1.0.1/ResSimpy/Nexus/DataModels/Network/NexusWellConnections.py
--rw-r--r--   0        0        0     3172 2023-08-04 13:28:48.983296 ressimpy-1.0.1/ResSimpy/Nexus/DataModels/Network/NexusWellbore.py
--rw-r--r--   0        0        0     3340 2023-08-04 13:28:48.983296 ressimpy-1.0.1/ResSimpy/Nexus/DataModels/Network/NexusWellbores.py
--rw-r--r--   0        0        0     5008 2023-08-04 13:28:48.983296 ressimpy-1.0.1/ResSimpy/Nexus/DataModels/Network/NexusWellhead.py
--rw-r--r--   0        0        0     3445 2023-08-04 13:28:48.983296 ressimpy-1.0.1/ResSimpy/Nexus/DataModels/Network/NexusWellheads.py
--rw-r--r--   0        0        0      263 2023-08-04 13:28:48.983296 ressimpy-1.0.1/ResSimpy/Nexus/DataModels/Network/__init__.py
--rw-r--r--   0        0        0     6322 2023-08-04 13:28:48.983296 ressimpy-1.0.1/ResSimpy/Nexus/DataModels/NexusAquiferMethod.py
--rw-r--r--   0        0        0    13983 2023-08-04 13:28:48.983296 ressimpy-1.0.1/ResSimpy/Nexus/DataModels/NexusCompletion.py
--rw-r--r--   0        0        0     8514 2023-08-04 13:28:48.983296 ressimpy-1.0.1/ResSimpy/Nexus/DataModels/NexusEquilMethod.py
--rw-r--r--   0        0        0    29623 2023-08-04 13:28:48.983296 ressimpy-1.0.1/ResSimpy/Nexus/DataModels/NexusFile.py
--rw-r--r--   0        0        0     4843 2023-08-04 13:28:48.983296 ressimpy-1.0.1/ResSimpy/Nexus/DataModels/NexusGasliftMethod.py
--rw-r--r--   0        0        0    10498 2023-08-04 13:28:48.983296 ressimpy-1.0.1/ResSimpy/Nexus/DataModels/NexusHydraulicsMethod.py
--rw-r--r--   0        0        0    27650 2023-08-04 13:28:48.983296 ressimpy-1.0.1/ResSimpy/Nexus/DataModels/NexusPVTMethod.py
--rw-r--r--   0        0        0     2543 2023-08-04 13:28:48.983296 ressimpy-1.0.1/ResSimpy/Nexus/DataModels/NexusRelPermEndPoint.py
--rw-r--r--   0        0        0    18026 2023-08-04 13:28:48.983296 ressimpy-1.0.1/ResSimpy/Nexus/DataModels/NexusRelPermMethod.py
--rw-r--r--   0        0        0     8056 2023-08-04 13:28:48.983296 ressimpy-1.0.1/ResSimpy/Nexus/DataModels/NexusRockMethod.py
--rw-r--r--   0        0        0     7487 2023-08-04 13:28:48.983296 ressimpy-1.0.1/ResSimpy/Nexus/DataModels/NexusSeparatorMethod.py
--rw-r--r--   0        0        0     5159 2023-08-04 13:28:48.983296 ressimpy-1.0.1/ResSimpy/Nexus/DataModels/NexusValveMethod.py
--rw-r--r--   0        0        0     9929 2023-08-04 13:28:48.983296 ressimpy-1.0.1/ResSimpy/Nexus/DataModels/NexusWaterMethod.py
--rw-r--r--   0        0        0     9125 2023-08-04 13:28:48.983296 ressimpy-1.0.1/ResSimpy/Nexus/DataModels/NexusWell.py
--rw-r--r--   0        0        0    14736 2023-08-04 13:28:48.983296 ressimpy-1.0.1/ResSimpy/Nexus/DataModels/StructuredGrid/NexusGrid.py
--rw-r--r--   0        0        0        0 2023-08-04 13:28:48.983296 ressimpy-1.0.1/ResSimpy/Nexus/DataModels/StructuredGrid/__init__.py
--rw-r--r--   0        0        0       77 2023-08-04 13:28:48.983296 ressimpy-1.0.1/ResSimpy/Nexus/DataModels/__init__.py
--rw-r--r--   0        0        0     2879 2023-08-04 13:28:48.983296 ressimpy-1.0.1/ResSimpy/Nexus/NexusAquiferMethods.py
--rw-r--r--   0        0        0      142 2023-08-04 13:28:48.983296 ressimpy-1.0.1/ResSimpy/Nexus/NexusEnums/DateFormatEnum.py
--rw-r--r--   0        0        0      106 2023-08-04 13:28:48.983296 ressimpy-1.0.1/ResSimpy/Nexus/NexusEnums/__init__.py
--rw-r--r--   0        0        0     2858 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Nexus/NexusEquilMethods.py
--rw-r--r--   0        0        0     2869 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Nexus/NexusGasliftMethods.py
--rw-r--r--   0        0        0        0 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Nexus/NexusGrids.py
--rw-r--r--   0        0        0     2939 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Nexus/NexusHydraulicsMethods.py
--rw-r--r--   0        0        0        0 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Nexus/NexusKeywords/__init__.py
--rw-r--r--   0        0        0        0 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Nexus/NexusKeywords/adsorption_keywords.py
--rw-r--r--   0        0        0        0 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Nexus/NexusKeywords/alphaf_keywords.py
--rw-r--r--   0        0        0      757 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Nexus/NexusKeywords/aquifer_keywords.py
--rw-r--r--   0        0        0        0 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Nexus/NexusKeywords/choke_keywords.py
--rw-r--r--   0        0        0        0 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Nexus/NexusKeywords/compressor_keywords.py
--rw-r--r--   0        0        0        0 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Nexus/NexusKeywords/eos_defaults_keywords.py
--rw-r--r--   0        0        0     1210 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Nexus/NexusKeywords/equil_keywords.py
--rw-r--r--   0        0        0        0 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Nexus/NexusKeywords/esp_keywords.py
--rw-r--r--   0        0        0     1368 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Nexus/NexusKeywords/fcs_keywords.py
--rw-r--r--   0        0        0        0 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Nexus/NexusKeywords/fluxin_keywords.py
--rw-r--r--   0        0        0      170 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Nexus/NexusKeywords/gaslift_keywords.py
--rw-r--r--   0        0        0     1159 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Nexus/NexusKeywords/hyd_keywords.py
--rw-r--r--   0        0        0        0 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Nexus/NexusKeywords/icd_keywords.py
--rw-r--r--   0        0        0        0 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Nexus/NexusKeywords/ipr_keywords.py
--rw-r--r--   0        0        0     2658 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Nexus/NexusKeywords/nexus_keywords.py
--rw-r--r--   0        0        0      795 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Nexus/NexusKeywords/options_keywords.py
--rw-r--r--   0        0        0        0 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Nexus/NexusKeywords/polymer_keywords.py
--rw-r--r--   0        0        0        0 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Nexus/NexusKeywords/pump_keywords.py
--rw-r--r--   0        0        0     2547 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Nexus/NexusKeywords/pvt_keywords.py
--rw-r--r--   0        0        0     1579 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Nexus/NexusKeywords/relpm_keywords.py
--rw-r--r--   0        0        0      896 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Nexus/NexusKeywords/rock_keywords.py
--rw-r--r--   0        0        0     2864 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Nexus/NexusKeywords/runcontrol_keywords.py
--rw-r--r--   0        0        0      880 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Nexus/NexusKeywords/separator_keywords.py
--rw-r--r--   0        0        0     3082 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Nexus/NexusKeywords/structured_grid_keywords.py
--rw-r--r--   0        0        0     4492 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Nexus/NexusKeywords/surface_keywords.py
--rw-r--r--   0        0        0        0 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Nexus/NexusKeywords/tracer_init_keywords.py
--rw-r--r--   0        0        0      306 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Nexus/NexusKeywords/valve_keywords.py
--rw-r--r--   0        0        0      243 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Nexus/NexusKeywords/water_keywords.py
--rw-r--r--   0        0        0      902 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Nexus/NexusKeywords/wells_keywords.py
--rw-r--r--   0        0        0     9401 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Nexus/NexusNetwork.py
--rw-r--r--   0        0        0     2773 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Nexus/NexusPVTMethods.py
--rw-r--r--   0        0        0     2985 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Nexus/NexusRelPermMethods.py
--rw-r--r--   0        0        0     1607 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Nexus/NexusReporting.py
--rw-r--r--   0        0        0     2805 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Nexus/NexusRockMethods.py
--rw-r--r--   0        0        0     3070 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Nexus/NexusSeparatorMethods.py
--rw-r--r--   0        0        0    31715 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Nexus/NexusSimulator.py
--rw-r--r--   0        0        0     2842 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Nexus/NexusValveMethods.py
--rw-r--r--   0        0        0     2837 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Nexus/NexusWaterMethods.py
--rw-r--r--   0        0        0    22484 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Nexus/NexusWells.py
--rw-r--r--   0        0        0      404 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Nexus/__init__.py
--rw-r--r--   0        0        0    12346 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Nexus/array_function_operations.py
--rw-r--r--   0        0        0       77 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Nexus/constants.py
--rw-r--r--   0        0        0    15687 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Nexus/load_wells.py
--rw-r--r--   0        0        0    14023 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Nexus/logfile_operations.py
--rw-r--r--   0        0        0    14562 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Nexus/nexus_add_new_object_to_file.py
--rw-r--r--   0        0        0     7954 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Nexus/nexus_collect_tables.py
--rw-r--r--   0        0        0     6838 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Nexus/nexus_constraint_operations.py
--rw-r--r--   0        0        0    39152 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Nexus/nexus_file_operations.py
--rw-r--r--   0        0        0     1963 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Nexus/nexus_modify_object_in_file.py
--rw-r--r--   0        0        0     5297 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Nexus/nexus_remove_object_from_file.py
--rw-r--r--   0        0        0     5387 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Nexus/rel_perm_operations.py
--rw-r--r--   0        0        0    13632 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Nexus/runcontrol_operations.py
--rw-r--r--   0        0        0     8982 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Nexus/structured_grid_operations.py
--rw-r--r--   0        0        0      829 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Node.py
--rw-r--r--   0        0        0      679 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/NodeConnection.py
--rw-r--r--   0        0        0      456 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/NodeConnections.py
--rw-r--r--   0        0        0      398 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Nodes.py
--rw-r--r--   0        0        0     2158 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/OperationsMixin.py
--rw-r--r--   0        0        0      383 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/PVT.py
--rw-r--r--   0        0        0      467 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/RelPerm.py
--rw-r--r--   0        0        0     3354 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/RelPermEndPoint.py
--rw-r--r--   0        0        0      404 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Rock.py
--rw-r--r--   0        0        0      419 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Separator.py
--rw-r--r--   0        0        0     3402 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Simulator.py
--rw-r--r--   0        0        0       95 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Utils/__init__.py
--rw-r--r--   0        0        0     2213 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Utils/factory_methods.py
--rw-r--r--   0        0        0      566 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Utils/generic_repr.py
--rw-r--r--   0        0        0     1585 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Utils/invert_nexus_map.py
--rw-r--r--   0        0        0      453 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Utils/obj_to_dataframe.py
--rw-r--r--   0        0        0     1053 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Utils/obj_to_table_string.py
--rw-r--r--   0        0        0     2234 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Utils/to_dict_generic.py
--rw-r--r--   0        0        0      407 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Valve.py
--rw-r--r--   0        0        0      408 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Water.py
--rw-r--r--   0        0        0     2256 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Well.py
--rw-r--r--   0        0        0      618 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/WellConnection.py
--rw-r--r--   0        0        0      435 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/WellConnections.py
--rw-r--r--   0        0        0      748 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Wellbore.py
--rw-r--r--   0        0        0      427 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Wellbores.py
--rw-r--r--   0        0        0      802 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Wellhead.py
--rw-r--r--   0        0        0      426 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Wellheads.py
--rw-r--r--   0        0        0     1119 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/Wells.py
--rw-r--r--   0        0        0      245 2023-08-04 13:28:48.987296 ressimpy-1.0.1/ResSimpy/__init__.py
--rw-r--r--   0        0        0     1859 2023-08-04 13:28:48.991296 ressimpy-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     2315 1970-01-01 00:00:00.000000 ressimpy-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     9156 2023-08-04 15:14:27.440214 ressimpy-1.0.2/LICENSE.MD
+-rw-r--r--   0        0        0     1521 2023-08-04 15:14:27.440214 ressimpy-1.0.2/README.md
+-rw-r--r--   0        0        0      395 2023-08-04 15:14:27.440214 ressimpy-1.0.2/ResSimpy/Aquifer.py
+-rw-r--r--   0        0        0     7082 2023-08-04 15:14:27.440214 ressimpy-1.0.2/ResSimpy/Completion.py
+-rw-r--r--   0        0        0     1263 2023-08-04 15:14:27.440214 ressimpy-1.0.2/ResSimpy/Constraint.py
+-rw-r--r--   0        0        0     1595 2023-08-04 15:14:27.440214 ressimpy-1.0.2/ResSimpy/Constraints.py
+-rw-r--r--   0        0        0     1945 2023-08-04 15:14:27.440214 ressimpy-1.0.2/ResSimpy/DynamicProperty.py
+-rw-r--r--   0        0        0      168 2023-08-04 15:14:27.440214 ressimpy-1.0.2/ResSimpy/Enums/HowEnum.py
+-rw-r--r--   0        0        0      722 2023-08-04 15:14:27.440214 ressimpy-1.0.2/ResSimpy/Enums/UnitsEnum.py
+-rw-r--r--   0        0        0       62 2023-08-04 15:14:27.440214 ressimpy-1.0.2/ResSimpy/Enums/__init__.py
+-rw-r--r--   0        0        0      413 2023-08-04 15:14:27.440214 ressimpy-1.0.2/ResSimpy/Equilibration.py
+-rw-r--r--   0        0        0     2880 2023-08-04 15:14:27.440214 ressimpy-1.0.2/ResSimpy/File.py
+-rw-r--r--   0        0        0     2068 2023-08-04 15:14:27.440214 ressimpy-1.0.2/ResSimpy/FileBase.py
+-rw-r--r--   0        0        0      413 2023-08-04 15:14:27.440214 ressimpy-1.0.2/ResSimpy/Gaslift.py
+-rw-r--r--   0        0        0     2631 2023-08-04 15:14:27.440214 ressimpy-1.0.2/ResSimpy/Grid.py
+-rw-r--r--   0        0        0      393 2023-08-04 15:14:27.440214 ressimpy-1.0.2/ResSimpy/Grids.py
+-rw-r--r--   0        0        0      404 2023-08-04 15:14:27.440214 ressimpy-1.0.2/ResSimpy/Hydraulics.py
+-rw-r--r--   0        0        0     2163 2023-08-04 15:14:27.440214 ressimpy-1.0.2/ResSimpy/ISODateTime.py
+-rw-r--r--   0        0        0      462 2023-08-04 15:14:27.440214 ressimpy-1.0.2/ResSimpy/Network.py
+-rw-r--r--   0        0        0      545 2023-08-04 15:14:27.440214 ressimpy-1.0.2/ResSimpy/Nexus/DataModels/FcsConfig.py
+-rw-r--r--   0        0        0    14289 2023-08-04 15:14:27.440214 ressimpy-1.0.2/ResSimpy/Nexus/DataModels/FcsFile.py
+-rw-r--r--   0        0        0    21922 2023-08-04 15:14:27.440214 ressimpy-1.0.2/ResSimpy/Nexus/DataModels/Network/NexusConstraint.py
+-rw-r--r--   0        0        0    17042 2023-08-04 15:14:27.440214 ressimpy-1.0.2/ResSimpy/Nexus/DataModels/Network/NexusConstraints.py
+-rw-r--r--   0        0        0     2736 2023-08-04 15:14:27.440214 ressimpy-1.0.2/ResSimpy/Nexus/DataModels/Network/NexusNode.py
+-rw-r--r--   0        0        0     5011 2023-08-04 15:14:27.440214 ressimpy-1.0.2/ResSimpy/Nexus/DataModels/Network/NexusNodeConnection.py
+-rw-r--r--   0        0        0     7241 2023-08-04 15:14:27.440214 ressimpy-1.0.2/ResSimpy/Nexus/DataModels/Network/NexusNodeConnections.py
+-rw-r--r--   0        0        0     7327 2023-08-04 15:14:27.440214 ressimpy-1.0.2/ResSimpy/Nexus/DataModels/Network/NexusNodes.py
+-rw-r--r--   0        0        0     6821 2023-08-04 15:14:27.440214 ressimpy-1.0.2/ResSimpy/Nexus/DataModels/Network/NexusWellConnection.py
+-rw-r--r--   0        0        0     4447 2023-08-04 15:14:27.440214 ressimpy-1.0.2/ResSimpy/Nexus/DataModels/Network/NexusWellConnections.py
+-rw-r--r--   0        0        0     3172 2023-08-04 15:14:27.440214 ressimpy-1.0.2/ResSimpy/Nexus/DataModels/Network/NexusWellbore.py
+-rw-r--r--   0        0        0     3340 2023-08-04 15:14:27.440214 ressimpy-1.0.2/ResSimpy/Nexus/DataModels/Network/NexusWellbores.py
+-rw-r--r--   0        0        0     5008 2023-08-04 15:14:27.440214 ressimpy-1.0.2/ResSimpy/Nexus/DataModels/Network/NexusWellhead.py
+-rw-r--r--   0        0        0     3445 2023-08-04 15:14:27.440214 ressimpy-1.0.2/ResSimpy/Nexus/DataModels/Network/NexusWellheads.py
+-rw-r--r--   0        0        0      263 2023-08-04 15:14:27.440214 ressimpy-1.0.2/ResSimpy/Nexus/DataModels/Network/__init__.py
+-rw-r--r--   0        0        0     6322 2023-08-04 15:14:27.440214 ressimpy-1.0.2/ResSimpy/Nexus/DataModels/NexusAquiferMethod.py
+-rw-r--r--   0        0        0    13983 2023-08-04 15:14:27.440214 ressimpy-1.0.2/ResSimpy/Nexus/DataModels/NexusCompletion.py
+-rw-r--r--   0        0        0     8514 2023-08-04 15:14:27.440214 ressimpy-1.0.2/ResSimpy/Nexus/DataModels/NexusEquilMethod.py
+-rw-r--r--   0        0        0    29623 2023-08-04 15:14:27.440214 ressimpy-1.0.2/ResSimpy/Nexus/DataModels/NexusFile.py
+-rw-r--r--   0        0        0     4843 2023-08-04 15:14:27.440214 ressimpy-1.0.2/ResSimpy/Nexus/DataModels/NexusGasliftMethod.py
+-rw-r--r--   0        0        0    10498 2023-08-04 15:14:27.444214 ressimpy-1.0.2/ResSimpy/Nexus/DataModels/NexusHydraulicsMethod.py
+-rw-r--r--   0        0        0    27650 2023-08-04 15:14:27.444214 ressimpy-1.0.2/ResSimpy/Nexus/DataModels/NexusPVTMethod.py
+-rw-r--r--   0        0        0     2543 2023-08-04 15:14:27.444214 ressimpy-1.0.2/ResSimpy/Nexus/DataModels/NexusRelPermEndPoint.py
+-rw-r--r--   0        0        0    18026 2023-08-04 15:14:27.444214 ressimpy-1.0.2/ResSimpy/Nexus/DataModels/NexusRelPermMethod.py
+-rw-r--r--   0        0        0     8056 2023-08-04 15:14:27.444214 ressimpy-1.0.2/ResSimpy/Nexus/DataModels/NexusRockMethod.py
+-rw-r--r--   0        0        0     7487 2023-08-04 15:14:27.444214 ressimpy-1.0.2/ResSimpy/Nexus/DataModels/NexusSeparatorMethod.py
+-rw-r--r--   0        0        0     5159 2023-08-04 15:14:27.444214 ressimpy-1.0.2/ResSimpy/Nexus/DataModels/NexusValveMethod.py
+-rw-r--r--   0        0        0     9929 2023-08-04 15:14:27.444214 ressimpy-1.0.2/ResSimpy/Nexus/DataModels/NexusWaterMethod.py
+-rw-r--r--   0        0        0     9125 2023-08-04 15:14:27.444214 ressimpy-1.0.2/ResSimpy/Nexus/DataModels/NexusWell.py
+-rw-r--r--   0        0        0    14736 2023-08-04 15:14:27.444214 ressimpy-1.0.2/ResSimpy/Nexus/DataModels/StructuredGrid/NexusGrid.py
+-rw-r--r--   0        0        0        0 2023-08-04 15:14:27.444214 ressimpy-1.0.2/ResSimpy/Nexus/DataModels/StructuredGrid/__init__.py
+-rw-r--r--   0        0        0       77 2023-08-04 15:14:27.444214 ressimpy-1.0.2/ResSimpy/Nexus/DataModels/__init__.py
+-rw-r--r--   0        0        0     2879 2023-08-04 15:14:27.444214 ressimpy-1.0.2/ResSimpy/Nexus/NexusAquiferMethods.py
+-rw-r--r--   0        0        0      142 2023-08-04 15:14:27.444214 ressimpy-1.0.2/ResSimpy/Nexus/NexusEnums/DateFormatEnum.py
+-rw-r--r--   0        0        0      106 2023-08-04 15:14:27.444214 ressimpy-1.0.2/ResSimpy/Nexus/NexusEnums/__init__.py
+-rw-r--r--   0        0        0     2858 2023-08-04 15:14:27.444214 ressimpy-1.0.2/ResSimpy/Nexus/NexusEquilMethods.py
+-rw-r--r--   0        0        0     2869 2023-08-04 15:14:27.444214 ressimpy-1.0.2/ResSimpy/Nexus/NexusGasliftMethods.py
+-rw-r--r--   0        0        0        0 2023-08-04 15:14:27.444214 ressimpy-1.0.2/ResSimpy/Nexus/NexusGrids.py
+-rw-r--r--   0        0        0     2939 2023-08-04 15:14:27.444214 ressimpy-1.0.2/ResSimpy/Nexus/NexusHydraulicsMethods.py
+-rw-r--r--   0        0        0        0 2023-08-04 15:14:27.444214 ressimpy-1.0.2/ResSimpy/Nexus/NexusKeywords/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-04 15:14:27.444214 ressimpy-1.0.2/ResSimpy/Nexus/NexusKeywords/adsorption_keywords.py
+-rw-r--r--   0        0        0        0 2023-08-04 15:14:27.444214 ressimpy-1.0.2/ResSimpy/Nexus/NexusKeywords/alphaf_keywords.py
+-rw-r--r--   0        0        0      757 2023-08-04 15:14:27.444214 ressimpy-1.0.2/ResSimpy/Nexus/NexusKeywords/aquifer_keywords.py
+-rw-r--r--   0        0        0        0 2023-08-04 15:14:27.444214 ressimpy-1.0.2/ResSimpy/Nexus/NexusKeywords/choke_keywords.py
+-rw-r--r--   0        0        0        0 2023-08-04 15:14:27.444214 ressimpy-1.0.2/ResSimpy/Nexus/NexusKeywords/compressor_keywords.py
+-rw-r--r--   0        0        0        0 2023-08-04 15:14:27.444214 ressimpy-1.0.2/ResSimpy/Nexus/NexusKeywords/eos_defaults_keywords.py
+-rw-r--r--   0        0        0     1210 2023-08-04 15:14:27.444214 ressimpy-1.0.2/ResSimpy/Nexus/NexusKeywords/equil_keywords.py
+-rw-r--r--   0        0        0        0 2023-08-04 15:14:27.444214 ressimpy-1.0.2/ResSimpy/Nexus/NexusKeywords/esp_keywords.py
+-rw-r--r--   0        0        0     1368 2023-08-04 15:14:27.444214 ressimpy-1.0.2/ResSimpy/Nexus/NexusKeywords/fcs_keywords.py
+-rw-r--r--   0        0        0        0 2023-08-04 15:14:27.444214 ressimpy-1.0.2/ResSimpy/Nexus/NexusKeywords/fluxin_keywords.py
+-rw-r--r--   0        0        0      170 2023-08-04 15:14:27.444214 ressimpy-1.0.2/ResSimpy/Nexus/NexusKeywords/gaslift_keywords.py
+-rw-r--r--   0        0        0     1159 2023-08-04 15:14:27.444214 ressimpy-1.0.2/ResSimpy/Nexus/NexusKeywords/hyd_keywords.py
+-rw-r--r--   0        0        0        0 2023-08-04 15:14:27.444214 ressimpy-1.0.2/ResSimpy/Nexus/NexusKeywords/icd_keywords.py
+-rw-r--r--   0        0        0        0 2023-08-04 15:14:27.444214 ressimpy-1.0.2/ResSimpy/Nexus/NexusKeywords/ipr_keywords.py
+-rw-r--r--   0        0        0     2658 2023-08-04 15:14:27.444214 ressimpy-1.0.2/ResSimpy/Nexus/NexusKeywords/nexus_keywords.py
+-rw-r--r--   0        0        0      795 2023-08-04 15:14:27.444214 ressimpy-1.0.2/ResSimpy/Nexus/NexusKeywords/options_keywords.py
+-rw-r--r--   0        0        0        0 2023-08-04 15:14:27.444214 ressimpy-1.0.2/ResSimpy/Nexus/NexusKeywords/polymer_keywords.py
+-rw-r--r--   0        0        0        0 2023-08-04 15:14:27.444214 ressimpy-1.0.2/ResSimpy/Nexus/NexusKeywords/pump_keywords.py
+-rw-r--r--   0        0        0     2547 2023-08-04 15:14:27.444214 ressimpy-1.0.2/ResSimpy/Nexus/NexusKeywords/pvt_keywords.py
+-rw-r--r--   0        0        0     1579 2023-08-04 15:14:27.444214 ressimpy-1.0.2/ResSimpy/Nexus/NexusKeywords/relpm_keywords.py
+-rw-r--r--   0        0        0      896 2023-08-04 15:14:27.444214 ressimpy-1.0.2/ResSimpy/Nexus/NexusKeywords/rock_keywords.py
+-rw-r--r--   0        0        0     2864 2023-08-04 15:14:27.444214 ressimpy-1.0.2/ResSimpy/Nexus/NexusKeywords/runcontrol_keywords.py
+-rw-r--r--   0        0        0      880 2023-08-04 15:14:27.444214 ressimpy-1.0.2/ResSimpy/Nexus/NexusKeywords/separator_keywords.py
+-rw-r--r--   0        0        0     3082 2023-08-04 15:14:27.444214 ressimpy-1.0.2/ResSimpy/Nexus/NexusKeywords/structured_grid_keywords.py
+-rw-r--r--   0        0        0     4492 2023-08-04 15:14:27.444214 ressimpy-1.0.2/ResSimpy/Nexus/NexusKeywords/surface_keywords.py
+-rw-r--r--   0        0        0        0 2023-08-04 15:14:27.444214 ressimpy-1.0.2/ResSimpy/Nexus/NexusKeywords/tracer_init_keywords.py
+-rw-r--r--   0        0        0      306 2023-08-04 15:14:27.444214 ressimpy-1.0.2/ResSimpy/Nexus/NexusKeywords/valve_keywords.py
+-rw-r--r--   0        0        0      243 2023-08-04 15:14:27.444214 ressimpy-1.0.2/ResSimpy/Nexus/NexusKeywords/water_keywords.py
+-rw-r--r--   0        0        0      902 2023-08-04 15:14:27.444214 ressimpy-1.0.2/ResSimpy/Nexus/NexusKeywords/wells_keywords.py
+-rw-r--r--   0        0        0     9401 2023-08-04 15:14:27.444214 ressimpy-1.0.2/ResSimpy/Nexus/NexusNetwork.py
+-rw-r--r--   0        0        0     2773 2023-08-04 15:14:27.444214 ressimpy-1.0.2/ResSimpy/Nexus/NexusPVTMethods.py
+-rw-r--r--   0        0        0     2985 2023-08-04 15:14:27.444214 ressimpy-1.0.2/ResSimpy/Nexus/NexusRelPermMethods.py
+-rw-r--r--   0        0        0     1607 2023-08-04 15:14:27.444214 ressimpy-1.0.2/ResSimpy/Nexus/NexusReporting.py
+-rw-r--r--   0        0        0     2805 2023-08-04 15:14:27.444214 ressimpy-1.0.2/ResSimpy/Nexus/NexusRockMethods.py
+-rw-r--r--   0        0        0     3070 2023-08-04 15:14:27.444214 ressimpy-1.0.2/ResSimpy/Nexus/NexusSeparatorMethods.py
+-rw-r--r--   0        0        0    31715 2023-08-04 15:14:27.444214 ressimpy-1.0.2/ResSimpy/Nexus/NexusSimulator.py
+-rw-r--r--   0        0        0     2842 2023-08-04 15:14:27.444214 ressimpy-1.0.2/ResSimpy/Nexus/NexusValveMethods.py
+-rw-r--r--   0        0        0     2837 2023-08-04 15:14:27.444214 ressimpy-1.0.2/ResSimpy/Nexus/NexusWaterMethods.py
+-rw-r--r--   0        0        0    22484 2023-08-04 15:14:27.444214 ressimpy-1.0.2/ResSimpy/Nexus/NexusWells.py
+-rw-r--r--   0        0        0      404 2023-08-04 15:14:27.444214 ressimpy-1.0.2/ResSimpy/Nexus/__init__.py
+-rw-r--r--   0        0        0    12346 2023-08-04 15:14:27.444214 ressimpy-1.0.2/ResSimpy/Nexus/array_function_operations.py
+-rw-r--r--   0        0        0       77 2023-08-04 15:14:27.444214 ressimpy-1.0.2/ResSimpy/Nexus/constants.py
+-rw-r--r--   0        0        0    15687 2023-08-04 15:14:27.444214 ressimpy-1.0.2/ResSimpy/Nexus/load_wells.py
+-rw-r--r--   0        0        0    14023 2023-08-04 15:14:27.444214 ressimpy-1.0.2/ResSimpy/Nexus/logfile_operations.py
+-rw-r--r--   0        0        0    14562 2023-08-04 15:14:27.444214 ressimpy-1.0.2/ResSimpy/Nexus/nexus_add_new_object_to_file.py
+-rw-r--r--   0        0        0     7954 2023-08-04 15:14:27.448214 ressimpy-1.0.2/ResSimpy/Nexus/nexus_collect_tables.py
+-rw-r--r--   0        0        0     6838 2023-08-04 15:14:27.448214 ressimpy-1.0.2/ResSimpy/Nexus/nexus_constraint_operations.py
+-rw-r--r--   0        0        0    39152 2023-08-04 15:14:27.448214 ressimpy-1.0.2/ResSimpy/Nexus/nexus_file_operations.py
+-rw-r--r--   0        0        0     1963 2023-08-04 15:14:27.448214 ressimpy-1.0.2/ResSimpy/Nexus/nexus_modify_object_in_file.py
+-rw-r--r--   0        0        0     5297 2023-08-04 15:14:27.448214 ressimpy-1.0.2/ResSimpy/Nexus/nexus_remove_object_from_file.py
+-rw-r--r--   0        0        0     5387 2023-08-04 15:14:27.448214 ressimpy-1.0.2/ResSimpy/Nexus/rel_perm_operations.py
+-rw-r--r--   0        0        0    13632 2023-08-04 15:14:27.448214 ressimpy-1.0.2/ResSimpy/Nexus/runcontrol_operations.py
+-rw-r--r--   0        0        0     8982 2023-08-04 15:14:27.448214 ressimpy-1.0.2/ResSimpy/Nexus/structured_grid_operations.py
+-rw-r--r--   0        0        0      829 2023-08-04 15:14:27.448214 ressimpy-1.0.2/ResSimpy/Node.py
+-rw-r--r--   0        0        0      679 2023-08-04 15:14:27.448214 ressimpy-1.0.2/ResSimpy/NodeConnection.py
+-rw-r--r--   0        0        0      456 2023-08-04 15:14:27.448214 ressimpy-1.0.2/ResSimpy/NodeConnections.py
+-rw-r--r--   0        0        0      398 2023-08-04 15:14:27.448214 ressimpy-1.0.2/ResSimpy/Nodes.py
+-rw-r--r--   0        0        0     2158 2023-08-04 15:14:27.448214 ressimpy-1.0.2/ResSimpy/OperationsMixin.py
+-rw-r--r--   0        0        0      383 2023-08-04 15:14:27.448214 ressimpy-1.0.2/ResSimpy/PVT.py
+-rw-r--r--   0        0        0      467 2023-08-04 15:14:27.448214 ressimpy-1.0.2/ResSimpy/RelPerm.py
+-rw-r--r--   0        0        0     3354 2023-08-04 15:14:27.448214 ressimpy-1.0.2/ResSimpy/RelPermEndPoint.py
+-rw-r--r--   0        0        0      404 2023-08-04 15:14:27.448214 ressimpy-1.0.2/ResSimpy/Rock.py
+-rw-r--r--   0        0        0      419 2023-08-04 15:14:27.448214 ressimpy-1.0.2/ResSimpy/Separator.py
+-rw-r--r--   0        0        0     3402 2023-08-04 15:14:27.448214 ressimpy-1.0.2/ResSimpy/Simulator.py
+-rw-r--r--   0        0        0       95 2023-08-04 15:14:27.448214 ressimpy-1.0.2/ResSimpy/Utils/__init__.py
+-rw-r--r--   0        0        0     2213 2023-08-04 15:14:27.448214 ressimpy-1.0.2/ResSimpy/Utils/factory_methods.py
+-rw-r--r--   0        0        0      566 2023-08-04 15:14:27.448214 ressimpy-1.0.2/ResSimpy/Utils/generic_repr.py
+-rw-r--r--   0        0        0     1585 2023-08-04 15:14:27.448214 ressimpy-1.0.2/ResSimpy/Utils/invert_nexus_map.py
+-rw-r--r--   0        0        0      453 2023-08-04 15:14:27.448214 ressimpy-1.0.2/ResSimpy/Utils/obj_to_dataframe.py
+-rw-r--r--   0        0        0     1053 2023-08-04 15:14:27.448214 ressimpy-1.0.2/ResSimpy/Utils/obj_to_table_string.py
+-rw-r--r--   0        0        0     2234 2023-08-04 15:14:27.448214 ressimpy-1.0.2/ResSimpy/Utils/to_dict_generic.py
+-rw-r--r--   0        0        0      407 2023-08-04 15:14:27.448214 ressimpy-1.0.2/ResSimpy/Valve.py
+-rw-r--r--   0        0        0      408 2023-08-04 15:14:27.448214 ressimpy-1.0.2/ResSimpy/Water.py
+-rw-r--r--   0        0        0     2256 2023-08-04 15:14:27.448214 ressimpy-1.0.2/ResSimpy/Well.py
+-rw-r--r--   0        0        0      618 2023-08-04 15:14:27.448214 ressimpy-1.0.2/ResSimpy/WellConnection.py
+-rw-r--r--   0        0        0      435 2023-08-04 15:14:27.448214 ressimpy-1.0.2/ResSimpy/WellConnections.py
+-rw-r--r--   0        0        0      748 2023-08-04 15:14:27.448214 ressimpy-1.0.2/ResSimpy/Wellbore.py
+-rw-r--r--   0        0        0      427 2023-08-04 15:14:27.448214 ressimpy-1.0.2/ResSimpy/Wellbores.py
+-rw-r--r--   0        0        0      802 2023-08-04 15:14:27.448214 ressimpy-1.0.2/ResSimpy/Wellhead.py
+-rw-r--r--   0        0        0      426 2023-08-04 15:14:27.448214 ressimpy-1.0.2/ResSimpy/Wellheads.py
+-rw-r--r--   0        0        0     1119 2023-08-04 15:14:27.448214 ressimpy-1.0.2/ResSimpy/Wells.py
+-rw-r--r--   0        0        0      289 2023-08-04 15:14:27.448214 ressimpy-1.0.2/ResSimpy/__init__.py
+-rw-r--r--   0        0        0     2436 2023-08-04 15:14:45.521409 ressimpy-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2397 1970-01-01 00:00:00.000000 ressimpy-1.0.2/PKG-INFO
```

### Comparing `ressimpy-1.0.1/README.md` & `ressimpy-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `ressimpy-1.0.1/ResSimpy/Completion.py` & `ressimpy-1.0.2/ResSimpy/Completion.py`

 * *Files identical despite different names*

### Comparing `ressimpy-1.0.1/ResSimpy/Constraint.py` & `ressimpy-1.0.2/ResSimpy/Constraint.py`

 * *Files identical despite different names*

### Comparing `ressimpy-1.0.1/ResSimpy/Constraints.py` & `ressimpy-1.0.2/ResSimpy/Constraints.py`

 * *Files identical despite different names*

### Comparing `ressimpy-1.0.1/ResSimpy/DynamicProperty.py` & `ressimpy-1.0.2/ResSimpy/DynamicProperty.py`

 * *Files identical despite different names*

### Comparing `ressimpy-1.0.1/ResSimpy/Enums/UnitsEnum.py` & `ressimpy-1.0.2/ResSimpy/Enums/UnitsEnum.py`

 * *Files identical despite different names*

### Comparing `ressimpy-1.0.1/ResSimpy/File.py` & `ressimpy-1.0.2/ResSimpy/File.py`

 * *Files identical despite different names*

### Comparing `ressimpy-1.0.1/ResSimpy/FileBase.py` & `ressimpy-1.0.2/ResSimpy/FileBase.py`

 * *Files identical despite different names*

### Comparing `ressimpy-1.0.1/ResSimpy/Grid.py` & `ressimpy-1.0.2/ResSimpy/Grid.py`

 * *Files identical despite different names*

### Comparing `ressimpy-1.0.1/ResSimpy/ISODateTime.py` & `ressimpy-1.0.2/ResSimpy/ISODateTime.py`

 * *Files identical despite different names*

### Comparing `ressimpy-1.0.1/ResSimpy/Nexus/DataModels/FcsConfig.py` & `ressimpy-1.0.2/ResSimpy/Nexus/DataModels/FcsConfig.py`

 * *Files identical despite different names*

### Comparing `ressimpy-1.0.1/ResSimpy/Nexus/DataModels/FcsFile.py` & `ressimpy-1.0.2/ResSimpy/Nexus/DataModels/FcsFile.py`

 * *Files identical despite different names*

### Comparing `ressimpy-1.0.1/ResSimpy/Nexus/DataModels/Network/NexusConstraint.py` & `ressimpy-1.0.2/ResSimpy/Nexus/DataModels/Network/NexusConstraint.py`

 * *Files identical despite different names*

### Comparing `ressimpy-1.0.1/ResSimpy/Nexus/DataModels/Network/NexusConstraints.py` & `ressimpy-1.0.2/ResSimpy/Nexus/DataModels/Network/NexusConstraints.py`

 * *Files identical despite different names*

### Comparing `ressimpy-1.0.1/ResSimpy/Nexus/DataModels/Network/NexusNode.py` & `ressimpy-1.0.2/ResSimpy/Nexus/DataModels/Network/NexusNode.py`

 * *Files identical despite different names*

### Comparing `ressimpy-1.0.1/ResSimpy/Nexus/DataModels/Network/NexusNodeConnection.py` & `ressimpy-1.0.2/ResSimpy/Nexus/DataModels/Network/NexusNodeConnection.py`

 * *Files identical despite different names*

### Comparing `ressimpy-1.0.1/ResSimpy/Nexus/DataModels/Network/NexusNodeConnections.py` & `ressimpy-1.0.2/ResSimpy/Nexus/DataModels/Network/NexusNodeConnections.py`

 * *Files identical despite different names*

### Comparing `ressimpy-1.0.1/ResSimpy/Nexus/DataModels/Network/NexusNodes.py` & `ressimpy-1.0.2/ResSimpy/Nexus/DataModels/Network/NexusNodes.py`

 * *Files identical despite different names*

### Comparing `ressimpy-1.0.1/ResSimpy/Nexus/DataModels/Network/NexusWellConnection.py` & `ressimpy-1.0.2/ResSimpy/Nexus/DataModels/Network/NexusWellConnection.py`

 * *Files identical despite different names*

### Comparing `ressimpy-1.0.1/ResSimpy/Nexus/DataModels/Network/NexusWellConnections.py` & `ressimpy-1.0.2/ResSimpy/Nexus/DataModels/Network/NexusWellConnections.py`

 * *Files identical despite different names*

### Comparing `ressimpy-1.0.1/ResSimpy/Nexus/DataModels/Network/NexusWellbore.py` & `ressimpy-1.0.2/ResSimpy/Nexus/DataModels/Network/NexusWellbore.py`

 * *Files identical despite different names*

### Comparing `ressimpy-1.0.1/ResSimpy/Nexus/DataModels/Network/NexusWellbores.py` & `ressimpy-1.0.2/ResSimpy/Nexus/DataModels/Network/NexusWellbores.py`

 * *Files identical despite different names*

### Comparing `ressimpy-1.0.1/ResSimpy/Nexus/DataModels/Network/NexusWellhead.py` & `ressimpy-1.0.2/ResSimpy/Nexus/DataModels/Network/NexusWellhead.py`

 * *Files identical despite different names*

### Comparing `ressimpy-1.0.1/ResSimpy/Nexus/DataModels/Network/NexusWellheads.py` & `ressimpy-1.0.2/ResSimpy/Nexus/DataModels/Network/NexusWellheads.py`

 * *Files identical despite different names*

### Comparing `ressimpy-1.0.1/ResSimpy/Nexus/DataModels/NexusAquiferMethod.py` & `ressimpy-1.0.2/ResSimpy/Nexus/DataModels/NexusAquiferMethod.py`

 * *Files identical despite different names*

### Comparing `ressimpy-1.0.1/ResSimpy/Nexus/DataModels/NexusCompletion.py` & `ressimpy-1.0.2/ResSimpy/Nexus/DataModels/NexusCompletion.py`

 * *Files identical despite different names*

### Comparing `ressimpy-1.0.1/ResSimpy/Nexus/DataModels/NexusEquilMethod.py` & `ressimpy-1.0.2/ResSimpy/Nexus/DataModels/NexusEquilMethod.py`

 * *Files identical despite different names*

### Comparing `ressimpy-1.0.1/ResSimpy/Nexus/DataModels/NexusFile.py` & `ressimpy-1.0.2/ResSimpy/Nexus/DataModels/NexusFile.py`

 * *Files identical despite different names*

### Comparing `ressimpy-1.0.1/ResSimpy/Nexus/DataModels/NexusGasliftMethod.py` & `ressimpy-1.0.2/ResSimpy/Nexus/DataModels/NexusGasliftMethod.py`

 * *Files identical despite different names*

### Comparing `ressimpy-1.0.1/ResSimpy/Nexus/DataModels/NexusHydraulicsMethod.py` & `ressimpy-1.0.2/ResSimpy/Nexus/DataModels/NexusHydraulicsMethod.py`

 * *Files identical despite different names*

### Comparing `ressimpy-1.0.1/ResSimpy/Nexus/DataModels/NexusPVTMethod.py` & `ressimpy-1.0.2/ResSimpy/Nexus/DataModels/NexusPVTMethod.py`

 * *Files identical despite different names*

### Comparing `ressimpy-1.0.1/ResSimpy/Nexus/DataModels/NexusRelPermEndPoint.py` & `ressimpy-1.0.2/ResSimpy/Nexus/DataModels/NexusRelPermEndPoint.py`

 * *Files identical despite different names*

### Comparing `ressimpy-1.0.1/ResSimpy/Nexus/DataModels/NexusRelPermMethod.py` & `ressimpy-1.0.2/ResSimpy/Nexus/DataModels/NexusRelPermMethod.py`

 * *Files identical despite different names*

### Comparing `ressimpy-1.0.1/ResSimpy/Nexus/DataModels/NexusRockMethod.py` & `ressimpy-1.0.2/ResSimpy/Nexus/DataModels/NexusRockMethod.py`

 * *Files identical despite different names*

### Comparing `ressimpy-1.0.1/ResSimpy/Nexus/DataModels/NexusSeparatorMethod.py` & `ressimpy-1.0.2/ResSimpy/Nexus/DataModels/NexusSeparatorMethod.py`

 * *Files identical despite different names*

### Comparing `ressimpy-1.0.1/ResSimpy/Nexus/DataModels/NexusValveMethod.py` & `ressimpy-1.0.2/ResSimpy/Nexus/DataModels/NexusValveMethod.py`

 * *Files identical despite different names*

### Comparing `ressimpy-1.0.1/ResSimpy/Nexus/DataModels/NexusWaterMethod.py` & `ressimpy-1.0.2/ResSimpy/Nexus/DataModels/NexusWaterMethod.py`

 * *Files identical despite different names*

### Comparing `ressimpy-1.0.1/ResSimpy/Nexus/DataModels/NexusWell.py` & `ressimpy-1.0.2/ResSimpy/Nexus/DataModels/NexusWell.py`

 * *Files identical despite different names*

### Comparing `ressimpy-1.0.1/ResSimpy/Nexus/DataModels/StructuredGrid/NexusGrid.py` & `ressimpy-1.0.2/ResSimpy/Nexus/DataModels/StructuredGrid/NexusGrid.py`

 * *Files identical despite different names*

### Comparing `ressimpy-1.0.1/ResSimpy/Nexus/NexusAquiferMethods.py` & `ressimpy-1.0.2/ResSimpy/Nexus/NexusAquiferMethods.py`

 * *Files identical despite different names*

### Comparing `ressimpy-1.0.1/ResSimpy/Nexus/NexusEquilMethods.py` & `ressimpy-1.0.2/ResSimpy/Nexus/NexusEquilMethods.py`

 * *Files identical despite different names*

### Comparing `ressimpy-1.0.1/ResSimpy/Nexus/NexusGasliftMethods.py` & `ressimpy-1.0.2/ResSimpy/Nexus/NexusGasliftMethods.py`

 * *Files identical despite different names*

### Comparing `ressimpy-1.0.1/ResSimpy/Nexus/NexusHydraulicsMethods.py` & `ressimpy-1.0.2/ResSimpy/Nexus/NexusHydraulicsMethods.py`

 * *Files identical despite different names*

### Comparing `ressimpy-1.0.1/ResSimpy/Nexus/NexusKeywords/aquifer_keywords.py` & `ressimpy-1.0.2/ResSimpy/Nexus/NexusKeywords/aquifer_keywords.py`

 * *Files identical despite different names*

### Comparing `ressimpy-1.0.1/ResSimpy/Nexus/NexusKeywords/equil_keywords.py` & `ressimpy-1.0.2/ResSimpy/Nexus/NexusKeywords/equil_keywords.py`

 * *Files identical despite different names*

### Comparing `ressimpy-1.0.1/ResSimpy/Nexus/NexusKeywords/fcs_keywords.py` & `ressimpy-1.0.2/ResSimpy/Nexus/NexusKeywords/fcs_keywords.py`

 * *Files identical despite different names*

### Comparing `ressimpy-1.0.1/ResSimpy/Nexus/NexusKeywords/hyd_keywords.py` & `ressimpy-1.0.2/ResSimpy/Nexus/NexusKeywords/hyd_keywords.py`

 * *Files identical despite different names*

### Comparing `ressimpy-1.0.1/ResSimpy/Nexus/NexusKeywords/nexus_keywords.py` & `ressimpy-1.0.2/ResSimpy/Nexus/NexusKeywords/nexus_keywords.py`

 * *Files identical despite different names*

### Comparing `ressimpy-1.0.1/ResSimpy/Nexus/NexusKeywords/options_keywords.py` & `ressimpy-1.0.2/ResSimpy/Nexus/NexusKeywords/options_keywords.py`

 * *Files identical despite different names*

### Comparing `ressimpy-1.0.1/ResSimpy/Nexus/NexusKeywords/pvt_keywords.py` & `ressimpy-1.0.2/ResSimpy/Nexus/NexusKeywords/pvt_keywords.py`

 * *Files identical despite different names*

### Comparing `ressimpy-1.0.1/ResSimpy/Nexus/NexusKeywords/relpm_keywords.py` & `ressimpy-1.0.2/ResSimpy/Nexus/NexusKeywords/relpm_keywords.py`

 * *Files identical despite different names*

### Comparing `ressimpy-1.0.1/ResSimpy/Nexus/NexusKeywords/rock_keywords.py` & `ressimpy-1.0.2/ResSimpy/Nexus/NexusKeywords/rock_keywords.py`

 * *Files identical despite different names*

### Comparing `ressimpy-1.0.1/ResSimpy/Nexus/NexusKeywords/runcontrol_keywords.py` & `ressimpy-1.0.2/ResSimpy/Nexus/NexusKeywords/runcontrol_keywords.py`

 * *Files identical despite different names*

### Comparing `ressimpy-1.0.1/ResSimpy/Nexus/NexusKeywords/separator_keywords.py` & `ressimpy-1.0.2/ResSimpy/Nexus/NexusKeywords/separator_keywords.py`

 * *Files identical despite different names*

### Comparing `ressimpy-1.0.1/ResSimpy/Nexus/NexusKeywords/structured_grid_keywords.py` & `ressimpy-1.0.2/ResSimpy/Nexus/NexusKeywords/structured_grid_keywords.py`

 * *Files identical despite different names*

### Comparing `ressimpy-1.0.1/ResSimpy/Nexus/NexusKeywords/surface_keywords.py` & `ressimpy-1.0.2/ResSimpy/Nexus/NexusKeywords/surface_keywords.py`

 * *Files identical despite different names*

### Comparing `ressimpy-1.0.1/ResSimpy/Nexus/NexusKeywords/wells_keywords.py` & `ressimpy-1.0.2/ResSimpy/Nexus/NexusKeywords/wells_keywords.py`

 * *Files identical despite different names*

### Comparing `ressimpy-1.0.1/ResSimpy/Nexus/NexusNetwork.py` & `ressimpy-1.0.2/ResSimpy/Nexus/NexusNetwork.py`

 * *Files identical despite different names*

### Comparing `ressimpy-1.0.1/ResSimpy/Nexus/NexusPVTMethods.py` & `ressimpy-1.0.2/ResSimpy/Nexus/NexusPVTMethods.py`

 * *Files identical despite different names*

### Comparing `ressimpy-1.0.1/ResSimpy/Nexus/NexusRelPermMethods.py` & `ressimpy-1.0.2/ResSimpy/Nexus/NexusRelPermMethods.py`

 * *Files identical despite different names*

### Comparing `ressimpy-1.0.1/ResSimpy/Nexus/NexusReporting.py` & `ressimpy-1.0.2/ResSimpy/Nexus/NexusReporting.py`

 * *Files identical despite different names*

### Comparing `ressimpy-1.0.1/ResSimpy/Nexus/NexusRockMethods.py` & `ressimpy-1.0.2/ResSimpy/Nexus/NexusRockMethods.py`

 * *Files identical despite different names*

### Comparing `ressimpy-1.0.1/ResSimpy/Nexus/NexusSeparatorMethods.py` & `ressimpy-1.0.2/ResSimpy/Nexus/NexusSeparatorMethods.py`

 * *Files identical despite different names*

### Comparing `ressimpy-1.0.1/ResSimpy/Nexus/NexusSimulator.py` & `ressimpy-1.0.2/ResSimpy/Nexus/NexusSimulator.py`

 * *Files identical despite different names*

### Comparing `ressimpy-1.0.1/ResSimpy/Nexus/NexusValveMethods.py` & `ressimpy-1.0.2/ResSimpy/Nexus/NexusValveMethods.py`

 * *Files identical despite different names*

### Comparing `ressimpy-1.0.1/ResSimpy/Nexus/NexusWaterMethods.py` & `ressimpy-1.0.2/ResSimpy/Nexus/NexusWaterMethods.py`

 * *Files identical despite different names*

### Comparing `ressimpy-1.0.1/ResSimpy/Nexus/NexusWells.py` & `ressimpy-1.0.2/ResSimpy/Nexus/NexusWells.py`

 * *Files identical despite different names*

### Comparing `ressimpy-1.0.1/ResSimpy/Nexus/array_function_operations.py` & `ressimpy-1.0.2/ResSimpy/Nexus/array_function_operations.py`

 * *Files identical despite different names*

### Comparing `ressimpy-1.0.1/ResSimpy/Nexus/load_wells.py` & `ressimpy-1.0.2/ResSimpy/Nexus/load_wells.py`

 * *Files identical despite different names*

### Comparing `ressimpy-1.0.1/ResSimpy/Nexus/logfile_operations.py` & `ressimpy-1.0.2/ResSimpy/Nexus/logfile_operations.py`

 * *Files identical despite different names*

### Comparing `ressimpy-1.0.1/ResSimpy/Nexus/nexus_add_new_object_to_file.py` & `ressimpy-1.0.2/ResSimpy/Nexus/nexus_add_new_object_to_file.py`

 * *Files identical despite different names*

### Comparing `ressimpy-1.0.1/ResSimpy/Nexus/nexus_collect_tables.py` & `ressimpy-1.0.2/ResSimpy/Nexus/nexus_collect_tables.py`

 * *Files identical despite different names*

### Comparing `ressimpy-1.0.1/ResSimpy/Nexus/nexus_constraint_operations.py` & `ressimpy-1.0.2/ResSimpy/Nexus/nexus_constraint_operations.py`

 * *Files identical despite different names*

### Comparing `ressimpy-1.0.1/ResSimpy/Nexus/nexus_file_operations.py` & `ressimpy-1.0.2/ResSimpy/Nexus/nexus_file_operations.py`

 * *Files identical despite different names*

### Comparing `ressimpy-1.0.1/ResSimpy/Nexus/nexus_modify_object_in_file.py` & `ressimpy-1.0.2/ResSimpy/Nexus/nexus_modify_object_in_file.py`

 * *Files identical despite different names*

### Comparing `ressimpy-1.0.1/ResSimpy/Nexus/nexus_remove_object_from_file.py` & `ressimpy-1.0.2/ResSimpy/Nexus/nexus_remove_object_from_file.py`

 * *Files identical despite different names*

### Comparing `ressimpy-1.0.1/ResSimpy/Nexus/rel_perm_operations.py` & `ressimpy-1.0.2/ResSimpy/Nexus/rel_perm_operations.py`

 * *Files identical despite different names*

### Comparing `ressimpy-1.0.1/ResSimpy/Nexus/runcontrol_operations.py` & `ressimpy-1.0.2/ResSimpy/Nexus/runcontrol_operations.py`

 * *Files identical despite different names*

### Comparing `ressimpy-1.0.1/ResSimpy/Nexus/structured_grid_operations.py` & `ressimpy-1.0.2/ResSimpy/Nexus/structured_grid_operations.py`

 * *Files identical despite different names*

### Comparing `ressimpy-1.0.1/ResSimpy/Node.py` & `ressimpy-1.0.2/ResSimpy/Node.py`

 * *Files identical despite different names*

### Comparing `ressimpy-1.0.1/ResSimpy/NodeConnection.py` & `ressimpy-1.0.2/ResSimpy/NodeConnection.py`

 * *Files identical despite different names*

### Comparing `ressimpy-1.0.1/ResSimpy/OperationsMixin.py` & `ressimpy-1.0.2/ResSimpy/OperationsMixin.py`

 * *Files identical despite different names*

### Comparing `ressimpy-1.0.1/ResSimpy/RelPermEndPoint.py` & `ressimpy-1.0.2/ResSimpy/RelPermEndPoint.py`

 * *Files identical despite different names*

### Comparing `ressimpy-1.0.1/ResSimpy/Simulator.py` & `ressimpy-1.0.2/ResSimpy/Simulator.py`

 * *Files identical despite different names*

### Comparing `ressimpy-1.0.1/ResSimpy/Utils/factory_methods.py` & `ressimpy-1.0.2/ResSimpy/Utils/factory_methods.py`

 * *Files identical despite different names*

### Comparing `ressimpy-1.0.1/ResSimpy/Utils/generic_repr.py` & `ressimpy-1.0.2/ResSimpy/Utils/generic_repr.py`

 * *Files identical despite different names*

### Comparing `ressimpy-1.0.1/ResSimpy/Utils/invert_nexus_map.py` & `ressimpy-1.0.2/ResSimpy/Utils/invert_nexus_map.py`

 * *Files identical despite different names*

### Comparing `ressimpy-1.0.1/ResSimpy/Utils/obj_to_table_string.py` & `ressimpy-1.0.2/ResSimpy/Utils/obj_to_table_string.py`

 * *Files identical despite different names*

### Comparing `ressimpy-1.0.1/ResSimpy/Utils/to_dict_generic.py` & `ressimpy-1.0.2/ResSimpy/Utils/to_dict_generic.py`

 * *Files identical despite different names*

### Comparing `ressimpy-1.0.1/ResSimpy/Well.py` & `ressimpy-1.0.2/ResSimpy/Well.py`

 * *Files identical despite different names*

### Comparing `ressimpy-1.0.1/ResSimpy/WellConnection.py` & `ressimpy-1.0.2/ResSimpy/WellConnection.py`

 * *Files identical despite different names*

### Comparing `ressimpy-1.0.1/ResSimpy/Wellbore.py` & `ressimpy-1.0.2/ResSimpy/Wellbore.py`

 * *Files identical despite different names*

### Comparing `ressimpy-1.0.1/ResSimpy/Wellhead.py` & `ressimpy-1.0.2/ResSimpy/Wellhead.py`

 * *Files identical despite different names*

### Comparing `ressimpy-1.0.1/ResSimpy/Wells.py` & `ressimpy-1.0.2/ResSimpy/Wells.py`

 * *Files identical despite different names*

### Comparing `ressimpy-1.0.1/PKG-INFO` & `ressimpy-1.0.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: ressimpy
-Version: 1.0.1
+Version: 1.0.2
 Summary: A Python library for working with Reservoir Simulator Models.
+License: Apache-2.0
 Keywords: ResSimpy,Reservoir Engineering
 Author: BP
 Requires-Python: >=3.10,<3.12
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: System :: Filesystems
```

