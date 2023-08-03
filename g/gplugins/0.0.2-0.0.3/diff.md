# Comparing `tmp/gplugins-0.0.2.tar.gz` & `tmp/gplugins-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gplugins-0.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "gplugins-0.0.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `gplugins-0.0.2.tar` & `gplugins-0.0.3.tar`

### file list

```diff
@@ -1,200 +1,205 @@
--rw-r--r--   0        0        0     1077 2023-08-01 17:41:12.316807 gplugins-0.0.2/LICENSE
--rw-r--r--   0        0        0     3177 2023-08-01 17:41:12.316807 gplugins-0.0.2/README.md
--rw-r--r--   0        0        0       59 2023-08-01 17:41:12.320807 gplugins-0.0.2/gplugins/__init__.py
--rw-r--r--   0        0        0     4262 2023-08-01 17:41:12.320807 gplugins-0.0.2/gplugins/add_simulation_markers.py
--rw-r--r--   0        0        0      603 2023-08-01 17:41:12.320807 gplugins-0.0.2/gplugins/config.py
--rw-r--r--   0        0        0     3057 2023-08-01 17:41:12.320807 gplugins-0.0.2/gplugins/convert_sparameters.py
--rw-r--r--   0        0        0       28 2023-08-01 17:41:12.320807 gplugins-0.0.2/gplugins/dagster/Makefile
--rw-r--r--   0        0        0        0 2023-08-01 17:41:12.320807 gplugins-0.0.2/gplugins/dagster/__init__.py
--rw-r--r--   0        0        0      933 2023-08-01 17:41:12.320807 gplugins-0.0.2/gplugins/dagster/workflow.py
--rw-r--r--   0        0        0      566 2023-08-01 17:41:12.320807 gplugins-0.0.2/gplugins/database/README.md
--rw-r--r--   0        0        0        0 2023-08-01 17:41:12.320807 gplugins-0.0.2/gplugins/database/__init__.py
--rw-r--r--   0        0        0     6182 2023-08-01 17:41:12.320807 gplugins-0.0.2/gplugins/database/db_upload.py
--rw-r--r--   0        0        0    16141 2023-08-01 17:41:12.320807 gplugins-0.0.2/gplugins/database/models.py
--rw-r--r--   0        0        0      571 2023-08-01 17:41:12.320807 gplugins-0.0.2/gplugins/devsim/__init__.py
--rw-r--r--   0        0        0     2569 2023-08-01 17:41:12.320807 gplugins-0.0.2/gplugins/devsim/doping.py
--rw-r--r--   0        0        0    11898 2023-08-01 17:41:12.320807 gplugins-0.0.2/gplugins/devsim/get_simulation.py
--rw-r--r--   0        0        0    28839 2023-08-01 17:41:12.320807 gplugins-0.0.2/gplugins/devsim/get_simulation_xsection.py
--rw-r--r--   0        0        0    19679 2023-08-01 17:41:12.320807 gplugins-0.0.2/gplugins/devsim/get_solver.py
--rw-r--r--   0        0        0     1598 2023-08-01 17:41:12.320807 gplugins-0.0.2/gplugins/devsim/test_devsim.py
--rw-r--r--   0        0        0      251 2023-08-01 17:41:12.320807 gplugins-0.0.2/gplugins/disable_print.py
--rw-r--r--   0        0        0       66 2023-08-01 17:41:12.320807 gplugins-0.0.2/gplugins/eme/__init__.py
--rw-r--r--   0        0        0    16034 2023-08-01 17:41:12.320807 gplugins-0.0.2/gplugins/eme/meow_eme.py
--rw-r--r--   0        0        0     1801 2023-08-01 17:41:12.320807 gplugins-0.0.2/gplugins/eme/test_meow_simulation.py
--rw-r--r--   0        0        0      107 2023-08-01 17:41:12.320807 gplugins-0.0.2/gplugins/fem/__init__.py
--rw-r--r--   0        0        0   567372 2023-08-01 17:41:12.324807 gplugins-0.0.2/gplugins/fem/mesh.msh
--rw-r--r--   0        0        0     8557 2023-08-01 17:41:12.324807 gplugins-0.0.2/gplugins/fem/mode_solver.py
--rw-r--r--   0        0        0     7772 2023-08-01 17:41:12.324807 gplugins-0.0.2/gplugins/fem/solve_thermal.py
--rw-r--r--   0        0        0     1410 2023-08-01 17:41:12.324807 gplugins-0.0.2/gplugins/fem/test_mode_solver.py
--rw-r--r--   0        0        0     3407 2023-08-01 17:41:12.324807 gplugins-0.0.2/gplugins/get_effective_indices.py
--rw-r--r--   0        0        0     2879 2023-08-01 17:41:12.324807 gplugins-0.0.2/gplugins/get_sparameters_path.py
--rw-r--r--   0        0        0     1900 2023-08-01 17:41:12.324807 gplugins-0.0.2/gplugins/gmeep/__init__.py
--rw-r--r--   0        0        0     1311 2023-08-01 17:41:12.324807 gplugins-0.0.2/gplugins/gmeep/async_utils.py
--rw-r--r--   0        0        0     3152 2023-08-01 17:41:12.324807 gplugins-0.0.2/gplugins/gmeep/get_material.py
--rw-r--r--   0        0        0     6037 2023-08-01 17:41:12.324807 gplugins-0.0.2/gplugins/gmeep/get_meep_geometry.py
--rw-r--r--   0        0        0     6028 2023-08-01 17:41:12.324807 gplugins-0.0.2/gplugins/gmeep/get_port_eigenmode.py
--rw-r--r--   0        0        0    10937 2023-08-01 17:41:12.324807 gplugins-0.0.2/gplugins/gmeep/get_simulation.py
--rw-r--r--   0        0        0    15892 2023-08-01 17:41:12.324807 gplugins-0.0.2/gplugins/gmeep/get_simulation_grating_farfield.py
--rw-r--r--   0        0        0    18153 2023-08-01 17:41:12.324807 gplugins-0.0.2/gplugins/gmeep/get_simulation_grating_fiber.py
--rw-r--r--   0        0        0    12263 2023-08-01 17:41:12.324807 gplugins-0.0.2/gplugins/gmeep/meep_adjoint_optimization.py
--rw-r--r--   0        0        0    11862 2023-08-01 17:41:12.324807 gplugins-0.0.2/gplugins/gmeep/test_eigenmode.py
--rw-r--r--   0        0        0      820 2023-08-01 17:41:12.324807 gplugins-0.0.2/gplugins/gmeep/test_materials.py
--rw-r--r--   0        0        0    10128 2023-08-01 17:41:12.324807 gplugins-0.0.2/gplugins/gmeep/test_sparameterNxN/test_sparameterNxN_crossing.csv
--rw-r--r--   0        0        0    10128 2023-08-01 17:41:12.324807 gplugins-0.0.2/gplugins/gmeep/test_sparameterNxN/test_sparameterNxN_straight.csv
--rw-r--r--   0        0        0     6189 2023-08-01 17:41:12.324807 gplugins-0.0.2/gplugins/gmeep/test_write_sparameters_meep.py
--rw-r--r--   0        0        0    10128 2023-08-01 17:41:12.324807 gplugins-0.0.2/gplugins/gmeep/test_write_sparameters_meep/test_sparameterNxN_crossing.csv
--rw-r--r--   0        0        0    10128 2023-08-01 17:41:12.324807 gplugins-0.0.2/gplugins/gmeep/test_write_sparameters_meep/test_sparameterNxN_straight.csv
--rw-r--r--   0        0        0    10093 2023-08-01 17:41:12.328807 gplugins-0.0.2/gplugins/gmeep/test_write_sparameters_meep/test_sparameterNxN_symmetries_straight.csv
--rw-r--r--   0        0        0    10085 2023-08-01 17:41:12.328807 gplugins-0.0.2/gplugins/gmeep/test_write_sparameters_meep/test_sparameter_straight_mpi.csv
--rw-r--r--   0        0        0    10085 2023-08-01 17:41:12.328807 gplugins-0.0.2/gplugins/gmeep/test_write_sparameters_meep/test_sparameter_straight_mpi_pool.csv
--rw-r--r--   0        0        0    34701 2023-08-01 17:41:12.328807 gplugins-0.0.2/gplugins/gmeep/test_write_sparameters_meep/test_sparameters_crossing_symmetric.csv
--rw-r--r--   0        0        0    10123 2023-08-01 17:41:12.328807 gplugins-0.0.2/gplugins/gmeep/test_write_sparameters_meep/test_sparameters_straight.csv
--rw-r--r--   0        0        0     9966 2023-08-01 17:41:12.328807 gplugins-0.0.2/gplugins/gmeep/test_write_sparameters_meep/test_sparameters_straight_batch.csv
--rw-r--r--   0        0        0     9966 2023-08-01 17:41:12.328807 gplugins-0.0.2/gplugins/gmeep/test_write_sparameters_meep/test_sparameters_straight_mpi.csv
--rw-r--r--   0        0        0    10085 2023-08-01 17:41:12.328807 gplugins-0.0.2/gplugins/gmeep/test_write_sparameters_meep/test_sparameters_straight_mpi_pool.csv
--rw-r--r--   0        0        0    10129 2023-08-01 17:41:12.328807 gplugins-0.0.2/gplugins/gmeep/test_write_sparameters_meep/test_sparameters_straight_symmetric.csv
--rw-r--r--   0        0        0    13928 2023-08-01 17:41:12.328807 gplugins-0.0.2/gplugins/gmeep/write_sparameters_grating.py
--rw-r--r--   0        0        0    21187 2023-08-01 17:41:12.328807 gplugins-0.0.2/gplugins/gmeep/write_sparameters_meep.py
--rw-r--r--   0        0        0     8069 2023-08-01 17:41:12.328807 gplugins-0.0.2/gplugins/gmeep/write_sparameters_meep_batch.py
--rw-r--r--   0        0        0     9516 2023-08-01 17:41:12.328807 gplugins-0.0.2/gplugins/gmeep/write_sparameters_meep_mpi.py
--rw-r--r--   0        0        0     1168 2023-08-01 17:41:12.328807 gplugins-0.0.2/gplugins/gmsh/__init__.py
--rw-r--r--   0        0        0     6640 2023-08-01 17:41:12.328807 gplugins-0.0.2/gplugins/gmsh/break_geometry.py
--rw-r--r--   0        0        0    11103 2023-08-01 17:41:12.328807 gplugins-0.0.2/gplugins/gmsh/mesh.py
--rw-r--r--   0        0        0    11769 2023-08-01 17:41:12.328807 gplugins-0.0.2/gplugins/gmsh/meshtracker.py
--rw-r--r--   0        0        0     7714 2023-08-01 17:41:12.328807 gplugins-0.0.2/gplugins/gmsh/parse_component.py
--rw-r--r--   0        0        0     3644 2023-08-01 17:41:12.328807 gplugins-0.0.2/gplugins/gmsh/parse_gds.py
--rw-r--r--   0        0        0     3604 2023-08-01 17:41:12.328807 gplugins-0.0.2/gplugins/gmsh/parse_layerstack.py
--rw-r--r--   0        0        0     2990 2023-08-01 17:41:12.328807 gplugins-0.0.2/gplugins/gmsh/refine.py
--rw-r--r--   0        0        0    10756 2023-08-01 17:41:12.328807 gplugins-0.0.2/gplugins/gmsh/scratch/mesh3D.py
--rw-r--r--   0        0        0     1997 2023-08-01 17:41:12.328807 gplugins-0.0.2/gplugins/gmsh/tests/test_meshing.py
--rw-r--r--   0        0        0    14029 2023-08-01 17:41:12.328807 gplugins-0.0.2/gplugins/gmsh/uz_xsection_mesh.py
--rw-r--r--   0        0        0     7281 2023-08-01 17:41:12.328807 gplugins-0.0.2/gplugins/gmsh/xy_xsection_mesh.py
--rw-r--r--   0        0        0     7928 2023-08-01 17:41:12.328807 gplugins-0.0.2/gplugins/gmsh/xyz_mesh.py
--rw-r--r--   0        0        0     1547 2023-08-01 17:41:12.328807 gplugins-0.0.2/gplugins/gtidy3d/__init__.py
--rw-r--r--   0        0        0     4449 2023-08-01 17:41:12.328807 gplugins-0.0.2/gplugins/gtidy3d/get_results.py
--rw-r--r--   0        0        0    19928 2023-08-01 17:41:12.328807 gplugins-0.0.2/gplugins/gtidy3d/get_simulation.py
--rw-r--r--   0        0        0    21022 2023-08-01 17:41:12.328807 gplugins-0.0.2/gplugins/gtidy3d/get_simulation_grating_coupler.py
--rw-r--r--   0        0        0     3431 2023-08-01 17:41:12.328807 gplugins-0.0.2/gplugins/gtidy3d/materials.py
--rw-r--r--   0        0        0    37242 2023-08-01 17:41:12.328807 gplugins-0.0.2/gplugins/gtidy3d/modes.py
--rw-r--r--   0        0        0     8941 2023-08-01 17:41:12.328807 gplugins-0.0.2/gplugins/gtidy3d/sim_run.yaml
--rw-r--r--   0        0        0     8114 2023-08-01 17:41:12.328807 gplugins-0.0.2/gplugins/gtidy3d/tests/sim_ref.yaml
--rw-r--r--   0        0        0     8114 2023-08-01 17:41:12.328807 gplugins-0.0.2/gplugins/gtidy3d/tests/sim_run.yaml
--rw-r--r--   0        0        0      731 2023-08-01 17:41:12.328807 gplugins-0.0.2/gplugins/gtidy3d/tests/test_modes.py
--rw-r--r--   0        0        0      262 2023-08-01 17:41:12.328807 gplugins-0.0.2/gplugins/gtidy3d/tests/test_modes/test_sweep_width.csv
--rw-r--r--   0        0        0      260 2023-08-01 17:41:12.328807 gplugins-0.0.2/gplugins/gtidy3d/tests/test_modes/test_sweep_width.obtained.csv
--rw-r--r--   0        0        0      854 2023-08-01 17:41:12.328807 gplugins-0.0.2/gplugins/gtidy3d/tests/test_results.py
--rw-r--r--   0        0        0     1503 2023-08-01 17:41:12.328807 gplugins-0.0.2/gplugins/gtidy3d/tests/test_simulation.py
--rw-r--r--   0        0        0     1642 2023-08-01 17:41:12.328807 gplugins-0.0.2/gplugins/gtidy3d/tests/test_write_sparameters.py
--rw-r--r--   0        0        0     9297 2023-08-01 17:41:12.328807 gplugins-0.0.2/gplugins/gtidy3d/tests/test_write_sparameters/test_sparameters_straight.csv
--rw-r--r--   0        0        0     1719 2023-08-01 17:41:12.328807 gplugins-0.0.2/gplugins/gtidy3d/tests/test_write_sparameters_grating_coupler.py
--rw-r--r--   0        0        0     1192 2023-08-01 17:41:12.328807 gplugins-0.0.2/gplugins/gtidy3d/utils.py
--rw-r--r--   0        0        0    11040 2023-08-01 17:41:12.328807 gplugins-0.0.2/gplugins/gtidy3d/write_sparameters.py
--rw-r--r--   0        0        0     8436 2023-08-01 17:41:12.328807 gplugins-0.0.2/gplugins/gtidy3d/write_sparameters_grating_coupler.py
--rw-r--r--   0        0        0      536 2023-08-01 17:41:12.328807 gplugins-0.0.2/gplugins/lumerical/__init__.py
--rw-r--r--   0        0        0    16025 2023-08-01 17:41:12.328807 gplugins-0.0.2/gplugins/lumerical/interconnect.py
--rw-r--r--   0        0        0     4223 2023-08-01 17:41:12.328807 gplugins-0.0.2/gplugins/lumerical/read.py
--rw-r--r--   0        0        0     3569 2023-08-01 17:41:12.328807 gplugins-0.0.2/gplugins/lumerical/settings.py
--rw-r--r--   0        0        0    19822 2023-08-01 17:41:12.328807 gplugins-0.0.2/gplugins/lumerical/write_sparameters_lumerical.py
--rw-r--r--   0        0        0     1459 2023-08-01 17:41:12.328807 gplugins-0.0.2/gplugins/lumerical/write_sparameters_lumerical_components.py
--rw-r--r--   0        0        0      854 2023-08-01 17:41:12.328807 gplugins-0.0.2/gplugins/modes/__init__.py
--rw-r--r--   0        0        0     1580 2023-08-01 17:41:12.328807 gplugins-0.0.2/gplugins/modes/coupler.py
--rw-r--r--   0        0        0     4153 2023-08-01 17:41:12.328807 gplugins-0.0.2/gplugins/modes/find_coupling_vs_gap.py
--rw-r--r--   0        0        0     2734 2023-08-01 17:41:12.328807 gplugins-0.0.2/gplugins/modes/find_mode_dispersion.py
--rw-r--r--   0        0        0     8835 2023-08-01 17:41:12.328807 gplugins-0.0.2/gplugins/modes/find_modes.py
--rwxr-xr-x   0        0        0     6956 2023-08-01 17:41:12.328807 gplugins-0.0.2/gplugins/modes/find_modes_cross_section.py
--rw-r--r--   0        0        0     4445 2023-08-01 17:41:12.328807 gplugins-0.0.2/gplugins/modes/find_neff_ng_dw_dh.py
--rw-r--r--   0        0        0     2715 2023-08-01 17:41:12.328807 gplugins-0.0.2/gplugins/modes/find_neff_vs_width.py
--rw-r--r--   0        0        0     7088 2023-08-01 17:41:12.328807 gplugins-0.0.2/gplugins/modes/get_mode_solver_coupler.py
--rwxr-xr-x   0        0        0     4410 2023-08-01 17:41:12.328807 gplugins-0.0.2/gplugins/modes/get_mode_solver_cross_section.py
--rw-r--r--   0        0        0     5377 2023-08-01 17:41:12.328807 gplugins-0.0.2/gplugins/modes/get_mode_solver_rib.py
--rw-r--r--   0        0        0     1110 2023-08-01 17:41:12.332807 gplugins-0.0.2/gplugins/modes/modes/neff_vs_width_nitride.csv
--rw-r--r--   0        0        0     1102 2023-08-01 17:41:12.332807 gplugins-0.0.2/gplugins/modes/modes/neff_vs_width_rib.csv
--rw-r--r--   0        0        0     1110 2023-08-01 17:41:12.332807 gplugins-0.0.2/gplugins/modes/modes/neff_vs_width_strip.csv
--rw-r--r--   0        0        0     7965 2023-08-01 17:41:12.332807 gplugins-0.0.2/gplugins/modes/neff_convergence_test.py
--rw-r--r--   0        0        0      267 2023-08-01 17:41:12.332807 gplugins-0.0.2/gplugins/modes/neff_vs_width.csv
--rw-r--r--   0        0        0     2443 2023-08-01 17:41:12.332807 gplugins-0.0.2/gplugins/modes/overlap.py
--rw-r--r--   0        0        0      405 2023-08-01 17:41:12.332807 gplugins-0.0.2/gplugins/modes/tests/test_dw_dh.py
--rw-r--r--   0        0        0       83 2023-08-01 17:41:12.332807 gplugins-0.0.2/gplugins/modes/tests/test_dw_dh/test_dw_dh.csv
--rw-r--r--   0        0        0       83 2023-08-01 17:41:12.332807 gplugins-0.0.2/gplugins/modes/tests/test_dw_dh/test_dw_dh.obtained.csv
--rw-r--r--   0        0        0      548 2023-08-01 17:41:12.332807 gplugins-0.0.2/gplugins/modes/tests/test_dw_dh/test_dw_dh_dispersion.csv
--rw-r--r--   0        0        0     1124 2023-08-01 17:41:12.332807 gplugins-0.0.2/gplugins/modes/tests/test_find_modes.py
--rw-r--r--   0        0        0      636 2023-08-01 17:41:12.332807 gplugins-0.0.2/gplugins/modes/tests/test_find_modes_dispersion.py
--rw-r--r--   0        0        0      341 2023-08-01 17:41:12.332807 gplugins-0.0.2/gplugins/modes/tests/test_neff_vs_width.py
--rw-r--r--   0        0        0      113 2023-08-01 17:41:12.332807 gplugins-0.0.2/gplugins/modes/tests/test_neff_vs_width/test_neff_vs_width.csv
--rw-r--r--   0        0        0      112 2023-08-01 17:41:12.332807 gplugins-0.0.2/gplugins/modes/tests/test_neff_vs_width/test_neff_vs_width.obtained.csv
--rw-r--r--   0        0        0    15453 2023-08-01 17:41:12.332807 gplugins-0.0.2/gplugins/modes/types.py
--rw-r--r--   0        0        0     1140 2023-08-01 17:41:12.332807 gplugins-0.0.2/gplugins/modes/waveguide.py
--rw-r--r--   0        0        0     2013 2023-08-01 17:41:12.332807 gplugins-0.0.2/gplugins/photonic_circuit_models/__init__.py
--rw-r--r--   0        0        0      597 2023-08-01 17:41:12.332807 gplugins-0.0.2/gplugins/photonic_circuit_models/coupler.py
--rw-r--r--   0        0        0      377 2023-08-01 17:41:12.332807 gplugins-0.0.2/gplugins/photonic_circuit_models/fsr.py
--rw-r--r--   0        0        0      418 2023-08-01 17:41:12.332807 gplugins-0.0.2/gplugins/photonic_circuit_models/heater.py
--rw-r--r--   0        0        0     3010 2023-08-01 17:41:12.332807 gplugins-0.0.2/gplugins/photonic_circuit_models/mzi.py
--rw-r--r--   0        0        0     2616 2023-08-01 17:41:12.332807 gplugins-0.0.2/gplugins/photonic_circuit_models/ring.py
--rw-r--r--   0        0        0     5951 2023-08-01 17:41:12.332807 gplugins-0.0.2/gplugins/plot.py
--rw-r--r--   0        0        0     2439 2023-08-01 17:41:12.332807 gplugins-0.0.2/gplugins/plot_csv.py
--rw-r--r--   0        0        0      613 2023-08-01 17:41:12.332807 gplugins-0.0.2/gplugins/port_symmetries.py
--rw-r--r--   0        0        0        0 2023-08-01 17:41:12.332807 gplugins-0.0.2/gplugins/process/__init__.py
--rw-r--r--   0        0        0     4623 2023-08-01 17:41:12.332807 gplugins-0.0.2/gplugins/process/diffusion.py
--rw-r--r--   0        0        0     5318 2023-08-01 17:41:12.332807 gplugins-0.0.2/gplugins/process/implant_tables.py
--rw-r--r--   0        0        0     6901 2023-08-01 17:41:12.332807 gplugins-0.0.2/gplugins/process/pysrim.py
--rw-r--r--   0        0        0     2182 2023-08-01 17:41:12.332807 gplugins-0.0.2/gplugins/process/silicon.py
--rw-r--r--   0        0        0     1861 2023-08-01 17:41:12.332807 gplugins-0.0.2/gplugins/process/skew/antimony_si_skew.csv
--rw-r--r--   0        0        0     1050 2023-08-01 17:41:12.332807 gplugins-0.0.2/gplugins/process/skew/arsenic_si_skew.csv
--rw-r--r--   0        0        0     1468 2023-08-01 17:41:12.332807 gplugins-0.0.2/gplugins/process/skew/boron_si_skew.csv
--rw-r--r--   0        0        0     1118 2023-08-01 17:41:12.332807 gplugins-0.0.2/gplugins/process/skew/phosphorus_si_skew.csv
--rw-r--r--   0        0        0      165 2023-08-01 17:41:12.332807 gplugins-0.0.2/gplugins/sax/__init__.py
--rw-r--r--   0        0        0    14710 2023-08-01 17:41:12.332807 gplugins-0.0.2/gplugins/sax/build_model.py
--rw-r--r--   0        0        0     7411 2023-08-01 17:41:12.332807 gplugins-0.0.2/gplugins/sax/femwell_waveguide_model.py
--rw-r--r--   0        0        0     1546 2023-08-01 17:41:12.332807 gplugins-0.0.2/gplugins/sax/interpolators.py
--rw-r--r--   0        0        0     6725 2023-08-01 17:41:12.332807 gplugins-0.0.2/gplugins/sax/meep_FDTD_model.py
--rw-r--r--   0        0        0     4491 2023-08-01 17:41:12.332807 gplugins-0.0.2/gplugins/sax/meow_eme_model.py
--rw-r--r--   0        0        0     5613 2023-08-01 17:41:12.332807 gplugins-0.0.2/gplugins/sax/mlp.py
--rw-r--r--   0        0        0     7345 2023-08-01 17:41:12.332807 gplugins-0.0.2/gplugins/sax/models.py
--rw-r--r--   0        0        0    13837 2023-08-01 17:41:12.332807 gplugins-0.0.2/gplugins/sax/parameter.py
--rwxr-xr-x   0        0        0     2173 2023-08-01 17:41:12.332807 gplugins-0.0.2/gplugins/sax/plot_model.py
--rw-r--r--   0        0        0     6769 2023-08-01 17:41:12.332807 gplugins-0.0.2/gplugins/sax/read.py
--rw-r--r--   0        0        0     1349 2023-08-01 17:41:12.332807 gplugins-0.0.2/gplugins/sax/tests/test_mzi.py
--rw-r--r--   0        0        0     2255 2023-08-01 17:41:12.332807 gplugins-0.0.2/gplugins/sax/tests/test_mzi_lattice.py
--rw-r--r--   0        0        0       76 2023-08-01 17:41:12.332807 gplugins-0.0.2/gplugins/sax/tests/test_mzi_lattice/test_mzi_lattice.obtained.yml
--rw-r--r--   0        0        0       76 2023-08-01 17:41:12.332807 gplugins-0.0.2/gplugins/sax/tests/test_mzi_lattice/test_mzi_lattice.yml
--rw-r--r--   0        0        0     1393 2023-08-01 17:41:12.332807 gplugins-0.0.2/gplugins/sax/tests/test_parameters.py
--rw-r--r--   0        0        0      102 2023-08-01 17:41:12.332807 gplugins-0.0.2/gplugins/schematic_editor/__init__.py
--rw-r--r--   0        0        0    16198 2023-08-01 17:41:12.332807 gplugins-0.0.2/gplugins/schematic_editor/circuitviz.py
--rw-r--r--   0        0        0    17770 2023-08-01 17:41:12.332807 gplugins-0.0.2/gplugins/schematic_editor/schematic_editor.py
--rw-r--r--   0        0        0       32 2023-08-01 17:41:12.332807 gplugins-0.0.2/gplugins/web/Makefile
--rw-r--r--   0        0        0       23 2023-08-01 17:41:12.332807 gplugins-0.0.2/gplugins/web/__init__.py
--rw-r--r--   0        0        0      212 2023-08-01 17:41:12.332807 gplugins-0.0.2/gplugins/web/gds_files/C.gds
--rw-r--r--   0        0        0      220 2023-08-01 17:41:12.332807 gplugins-0.0.2/gplugins/web/gds_files/C_width20.gds
--rw-r--r--   0        0        0      218 2023-08-01 17:41:12.332807 gplugins-0.0.2/gplugins/web/gds_files/C_width5.gds
--rw-r--r--   0        0        0    14536 2023-08-01 17:41:12.332807 gplugins-0.0.2/gplugins/web/gds_files/coh_rx_dual_pol.gds
--rw-r--r--   0        0        0    13550 2023-08-01 17:41:12.332807 gplugins-0.0.2/gplugins/web/gds_files/coh_rx_single_pol.gds
--rw-r--r--   0        0        0    13564 2023-08-01 17:41:12.332807 gplugins-0.0.2/gplugins/web/gds_files/coh_rx_single_pol_pad_d_19b6c499.gds
--rw-r--r--   0        0        0    13564 2023-08-01 17:41:12.332807 gplugins-0.0.2/gplugins/web/gds_files/coh_rx_single_pol_pad_d_d4526895.gds
--rw-r--r--   0        0        0    10292 2023-08-01 17:41:12.332807 gplugins-0.0.2/gplugins/web/gds_files/coh_tx_dual_pol.gds
--rw-r--r--   0        0        0     1498 2023-08-01 17:41:12.332807 gplugins-0.0.2/gplugins/web/gds_files/crossing_arm.gds
--rw-r--r--   0        0        0     7406 2023-08-01 17:41:12.332807 gplugins-0.0.2/gplugins/web/gds_files/dbr_cavity.gds
--rw-r--r--   0        0        0      440 2023-08-01 17:41:12.332807 gplugins-0.0.2/gplugins/web/gds_files/die_bbox_frame.gds
--rw-r--r--   0        0        0    27548 2023-08-01 17:41:12.332807 gplugins-0.0.2/gplugins/web/gds_files/loss_deembedding_ch14_23.gds
--rw-r--r--   0        0        0      872 2023-08-01 17:41:12.332807 gplugins-0.0.2/gplugins/web/gds_files/pad_array_add_fiducials.gds
--rw-r--r--   0        0        0    39252 2023-08-01 17:41:12.332807 gplugins-0.0.2/gplugins/web/gds_files/spiral_inner_io_add_gra_f2760628.gds
--rw-r--r--   0        0        0      182 2023-08-01 17:41:12.332807 gplugins-0.0.2/gplugins/web/gds_files/wg.gds
--rw-r--r--   0        0        0     8606 2023-08-01 17:41:12.332807 gplugins-0.0.2/gplugins/web/main.py
--rw-r--r--   0        0        0     1998 2023-08-01 17:41:12.332807 gplugins-0.0.2/gplugins/web/middleware.py
--rwxr-xr-x   0        0        0     7546 2023-08-01 17:41:12.332807 gplugins-0.0.2/gplugins/web/server.py
--rwxr-xr-x   0        0        0      636 2023-08-01 17:41:12.332807 gplugins-0.0.2/gplugins/web/server_jupyter.py
--rw-r--r--   0        0        0     1299 2023-08-01 17:41:12.332807 gplugins-0.0.2/gplugins/web/static/client.css
--rw-r--r--   0        0        0     9598 2023-08-01 17:41:12.332807 gplugins-0.0.2/gplugins/web/static/client.js
--rw-r--r--   0        0        0      840 2023-08-01 17:41:12.332807 gplugins-0.0.2/gplugins/web/templates/client.html.j2
--rw-r--r--   0        0        0      481 2023-08-01 17:41:12.332807 gplugins-0.0.2/gplugins/web/templates/file_browser.html.j2
--rw-r--r--   0        0        0     1999 2023-08-01 17:41:12.336807 gplugins-0.0.2/gplugins/web/templates/filewatcher.html.j2
--rw-r--r--   0        0        0      236 2023-08-01 17:41:12.336807 gplugins-0.0.2/gplugins/web/templates/footer.html.j2
--rw-r--r--   0        0        0      242 2023-08-01 17:41:12.336807 gplugins-0.0.2/gplugins/web/templates/gds_history.html.j2
--rw-r--r--   0        0        0      578 2023-08-01 17:41:12.336807 gplugins-0.0.2/gplugins/web/templates/header.html.j2
--rw-r--r--   0        0        0      376 2023-08-01 17:41:12.336807 gplugins-0.0.2/gplugins/web/templates/index.html.j2
--rw-r--r--   0        0        0      995 2023-08-01 17:41:12.336807 gplugins-0.0.2/gplugins/web/templates/navbar.html.j2
--rw-r--r--   0        0        0      272 2023-08-01 17:41:12.336807 gplugins-0.0.2/gplugins/web/templates/pdk.html.j2
--rw-r--r--   0        0        0     1871 2023-08-01 17:41:12.336807 gplugins-0.0.2/gplugins/web/templates/viewer.html.j2
--rw-r--r--   0        0        0       87 2023-08-01 17:41:12.336807 gplugins-0.0.2/gplugins/widget/__init__.py
--rw-r--r--   0        0        0    14938 2023-08-01 17:41:12.336807 gplugins-0.0.2/gplugins/widget/interactive.py
--rw-r--r--   0        0        0     3928 2023-08-01 17:41:12.336807 gplugins-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     5632 1970-01-01 00:00:00.000000 gplugins-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-08-03 23:24:20.872192 gplugins-0.0.3/LICENSE
+-rw-r--r--   0        0        0     2217 2023-08-03 23:24:20.872192 gplugins-0.0.3/README.md
+-rw-r--r--   0        0        0      244 2023-08-03 23:24:20.876192 gplugins-0.0.3/gplugins/__init__.py
+-rw-r--r--   0        0        0      603 2023-08-03 23:24:20.876192 gplugins-0.0.3/gplugins/config.py
+-rw-r--r--   0        0        0       28 2023-08-03 23:24:20.876192 gplugins-0.0.3/gplugins/dagster/Makefile
+-rw-r--r--   0        0        0        0 2023-08-03 23:24:20.876192 gplugins-0.0.3/gplugins/dagster/__init__.py
+-rw-r--r--   0        0        0      933 2023-08-03 23:24:20.876192 gplugins-0.0.3/gplugins/dagster/workflow.py
+-rw-r--r--   0        0        0      566 2023-08-03 23:24:20.876192 gplugins-0.0.3/gplugins/database/README.md
+-rw-r--r--   0        0        0        0 2023-08-03 23:24:20.876192 gplugins-0.0.3/gplugins/database/__init__.py
+-rw-r--r--   0        0        0     6142 2023-08-03 23:24:20.876192 gplugins-0.0.3/gplugins/database/db_upload.py
+-rw-r--r--   0        0        0    16141 2023-08-03 23:24:20.876192 gplugins-0.0.3/gplugins/database/models.py
+-rw-r--r--   0        0        0      571 2023-08-03 23:24:20.876192 gplugins-0.0.3/gplugins/devsim/__init__.py
+-rw-r--r--   0        0        0     2569 2023-08-03 23:24:20.876192 gplugins-0.0.3/gplugins/devsim/doping.py
+-rw-r--r--   0        0        0    11898 2023-08-03 23:24:20.876192 gplugins-0.0.3/gplugins/devsim/get_simulation.py
+-rw-r--r--   0        0        0    28843 2023-08-03 23:24:20.876192 gplugins-0.0.3/gplugins/devsim/get_simulation_xsection.py
+-rw-r--r--   0        0        0    19679 2023-08-03 23:24:20.876192 gplugins-0.0.3/gplugins/devsim/get_solver.py
+-rw-r--r--   0        0        0     1598 2023-08-03 23:24:20.876192 gplugins-0.0.3/gplugins/devsim/test_devsim.py
+-rw-r--r--   0        0        0      198 2023-08-03 23:24:20.876192 gplugins-0.0.3/gplugins/eme/__init__.py
+-rw-r--r--   0        0        0      207 2023-08-03 23:24:20.876192 gplugins-0.0.3/gplugins/fem/__init__.py
+-rw-r--r--   0        0        0      107 2023-08-03 23:24:20.876192 gplugins-0.0.3/gplugins/femwell/__init__.py
+-rw-r--r--   0        0        0     8557 2023-08-03 23:24:20.876192 gplugins-0.0.3/gplugins/femwell/mode_solver.py
+-rw-r--r--   0        0        0     7772 2023-08-03 23:24:20.876192 gplugins-0.0.3/gplugins/femwell/solve_thermal.py
+-rw-r--r--   0        0        0     1414 2023-08-03 23:24:20.876192 gplugins-0.0.3/gplugins/femwell/test_mode_solver.py
+-rw-r--r--   0        0        0     1906 2023-08-03 23:24:20.876192 gplugins-0.0.3/gplugins/gmeep/__init__.py
+-rw-r--r--   0        0        0     1311 2023-08-03 23:24:20.876192 gplugins-0.0.3/gplugins/gmeep/async_utils.py
+-rw-r--r--   0        0        0     3151 2023-08-03 23:24:20.876192 gplugins-0.0.3/gplugins/gmeep/get_material.py
+-rw-r--r--   0        0        0     6037 2023-08-03 23:24:20.876192 gplugins-0.0.3/gplugins/gmeep/get_meep_geometry.py
+-rw-r--r--   0        0        0     6028 2023-08-03 23:24:20.876192 gplugins-0.0.3/gplugins/gmeep/get_port_eigenmode.py
+-rw-r--r--   0        0        0    10937 2023-08-03 23:24:20.876192 gplugins-0.0.3/gplugins/gmeep/get_simulation.py
+-rw-r--r--   0        0        0    15892 2023-08-03 23:24:20.876192 gplugins-0.0.3/gplugins/gmeep/get_simulation_grating_farfield.py
+-rw-r--r--   0        0        0    18153 2023-08-03 23:24:20.876192 gplugins-0.0.3/gplugins/gmeep/get_simulation_grating_fiber.py
+-rw-r--r--   0        0        0    12263 2023-08-03 23:24:20.876192 gplugins-0.0.3/gplugins/gmeep/meep_adjoint_optimization.py
+-rw-r--r--   0        0        0    11862 2023-08-03 23:24:20.876192 gplugins-0.0.3/gplugins/gmeep/test_eigenmode.py
+-rw-r--r--   0        0        0      820 2023-08-03 23:24:20.876192 gplugins-0.0.3/gplugins/gmeep/test_materials.py
+-rw-r--r--   0        0        0    10128 2023-08-03 23:24:20.876192 gplugins-0.0.3/gplugins/gmeep/test_sparameterNxN/test_sparameterNxN_crossing.csv
+-rw-r--r--   0        0        0    10128 2023-08-03 23:24:20.876192 gplugins-0.0.3/gplugins/gmeep/test_sparameterNxN/test_sparameterNxN_straight.csv
+-rw-r--r--   0        0        0     6189 2023-08-03 23:24:20.876192 gplugins-0.0.3/gplugins/gmeep/test_write_sparameters_meep.py
+-rw-r--r--   0        0        0    10128 2023-08-03 23:24:20.876192 gplugins-0.0.3/gplugins/gmeep/test_write_sparameters_meep/test_sparameterNxN_crossing.csv
+-rw-r--r--   0        0        0    10128 2023-08-03 23:24:20.876192 gplugins-0.0.3/gplugins/gmeep/test_write_sparameters_meep/test_sparameterNxN_straight.csv
+-rw-r--r--   0        0        0    10093 2023-08-03 23:24:20.876192 gplugins-0.0.3/gplugins/gmeep/test_write_sparameters_meep/test_sparameterNxN_symmetries_straight.csv
+-rw-r--r--   0        0        0    10085 2023-08-03 23:24:20.876192 gplugins-0.0.3/gplugins/gmeep/test_write_sparameters_meep/test_sparameter_straight_mpi.csv
+-rw-r--r--   0        0        0    10085 2023-08-03 23:24:20.876192 gplugins-0.0.3/gplugins/gmeep/test_write_sparameters_meep/test_sparameter_straight_mpi_pool.csv
+-rw-r--r--   0        0        0    34701 2023-08-03 23:24:20.876192 gplugins-0.0.3/gplugins/gmeep/test_write_sparameters_meep/test_sparameters_crossing_symmetric.csv
+-rw-r--r--   0        0        0    10123 2023-08-03 23:24:20.876192 gplugins-0.0.3/gplugins/gmeep/test_write_sparameters_meep/test_sparameters_straight.csv
+-rw-r--r--   0        0        0     9966 2023-08-03 23:24:20.876192 gplugins-0.0.3/gplugins/gmeep/test_write_sparameters_meep/test_sparameters_straight_batch.csv
+-rw-r--r--   0        0        0     9966 2023-08-03 23:24:20.876192 gplugins-0.0.3/gplugins/gmeep/test_write_sparameters_meep/test_sparameters_straight_mpi.csv
+-rw-r--r--   0        0        0    10085 2023-08-03 23:24:20.876192 gplugins-0.0.3/gplugins/gmeep/test_write_sparameters_meep/test_sparameters_straight_mpi_pool.csv
+-rw-r--r--   0        0        0    10129 2023-08-03 23:24:20.876192 gplugins-0.0.3/gplugins/gmeep/test_write_sparameters_meep/test_sparameters_straight_symmetric.csv
+-rw-r--r--   0        0        0    13928 2023-08-03 23:24:20.876192 gplugins-0.0.3/gplugins/gmeep/write_sparameters_grating.py
+-rw-r--r--   0        0        0    21199 2023-08-03 23:24:20.876192 gplugins-0.0.3/gplugins/gmeep/write_sparameters_meep.py
+-rw-r--r--   0        0        0     8081 2023-08-03 23:24:20.876192 gplugins-0.0.3/gplugins/gmeep/write_sparameters_meep_batch.py
+-rw-r--r--   0        0        0     9528 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/gmeep/write_sparameters_meep_mpi.py
+-rw-r--r--   0        0        0     1168 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/gmsh/__init__.py
+-rw-r--r--   0        0        0     6640 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/gmsh/break_geometry.py
+-rw-r--r--   0        0        0    11103 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/gmsh/mesh.py
+-rw-r--r--   0        0        0    11769 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/gmsh/meshtracker.py
+-rw-r--r--   0        0        0     7714 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/gmsh/parse_component.py
+-rw-r--r--   0        0        0     3644 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/gmsh/parse_gds.py
+-rw-r--r--   0        0        0     3619 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/gmsh/parse_layerstack.py
+-rw-r--r--   0        0        0     2990 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/gmsh/refine.py
+-rw-r--r--   0        0        0    10756 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/gmsh/scratch/mesh3D.py
+-rw-r--r--   0        0        0     1997 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/gmsh/tests/test_meshing.py
+-rw-r--r--   0        0        0    14029 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/gmsh/uz_xsection_mesh.py
+-rw-r--r--   0        0        0     7281 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/gmsh/xy_xsection_mesh.py
+-rw-r--r--   0        0        0     9145 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/gmsh/xyz_mesh.py
+-rw-r--r--   0        0        0      220 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/gtidy3d/__init__.py
+-rw-r--r--   0        0        0      536 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/lumerical/__init__.py
+-rw-r--r--   0        0        0    16025 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/lumerical/interconnect.py
+-rw-r--r--   0        0        0     4229 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/lumerical/read.py
+-rw-r--r--   0        0        0     3569 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/lumerical/settings.py
+-rw-r--r--   0        0        0     2353 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/lumerical/tests/test_lumerical_read_sparameters.py
+-rw-r--r--   0        0        0    19826 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/lumerical/write_sparameters_lumerical.py
+-rw-r--r--   0        0        0     1459 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/lumerical/write_sparameters_lumerical_components.py
+-rw-r--r--   0        0        0       67 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/meow/__init__.py
+-rw-r--r--   0        0        0    16461 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/meow/meow_eme.py
+-rw-r--r--   0        0        0     1802 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/meow/test_meow_simulation.py
+-rw-r--r--   0        0        0      854 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/modes/__init__.py
+-rw-r--r--   0        0        0     1580 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/modes/coupler.py
+-rw-r--r--   0        0        0     4153 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/modes/find_coupling_vs_gap.py
+-rw-r--r--   0        0        0     2734 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/modes/find_mode_dispersion.py
+-rw-r--r--   0        0        0     8811 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/modes/find_modes.py
+-rwxr-xr-x   0        0        0     6968 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/modes/find_modes_cross_section.py
+-rw-r--r--   0        0        0     4445 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/modes/find_neff_ng_dw_dh.py
+-rw-r--r--   0        0        0     2715 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/modes/find_neff_vs_width.py
+-rw-r--r--   0        0        0     7088 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/modes/get_mode_solver_coupler.py
+-rwxr-xr-x   0        0        0     4410 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/modes/get_mode_solver_cross_section.py
+-rw-r--r--   0        0        0     5377 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/modes/get_mode_solver_rib.py
+-rw-r--r--   0        0        0     1110 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/modes/modes/neff_vs_width_nitride.csv
+-rw-r--r--   0        0        0     1102 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/modes/modes/neff_vs_width_rib.csv
+-rw-r--r--   0        0        0     1110 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/modes/modes/neff_vs_width_strip.csv
+-rw-r--r--   0        0        0     7965 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/modes/neff_convergence_test.py
+-rw-r--r--   0        0        0      267 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/modes/neff_vs_width.csv
+-rw-r--r--   0        0        0     2443 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/modes/overlap.py
+-rw-r--r--   0        0        0      405 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/modes/tests/test_dw_dh.py
+-rw-r--r--   0        0        0       83 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/modes/tests/test_dw_dh/test_dw_dh.csv
+-rw-r--r--   0        0        0       83 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/modes/tests/test_dw_dh/test_dw_dh.obtained.csv
+-rw-r--r--   0        0        0      548 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/modes/tests/test_dw_dh/test_dw_dh_dispersion.csv
+-rw-r--r--   0        0        0     1124 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/modes/tests/test_find_modes.py
+-rw-r--r--   0        0        0      636 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/modes/tests/test_find_modes_dispersion.py
+-rw-r--r--   0        0        0      341 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/modes/tests/test_neff_vs_width.py
+-rw-r--r--   0        0        0      113 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/modes/tests/test_neff_vs_width/test_neff_vs_width.csv
+-rw-r--r--   0        0        0      112 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/modes/tests/test_neff_vs_width/test_neff_vs_width.obtained.csv
+-rw-r--r--   0        0        0    15453 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/modes/types.py
+-rw-r--r--   0        0        0     1140 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/modes/waveguide.py
+-rw-r--r--   0        0        0      132 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/path_length_analysis/__init__.py
+-rw-r--r--   0        0        0    19360 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/path_length_analysis/path_length_analysis.py
+-rw-r--r--   0        0        0     5948 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/path_length_analysis/test_pathlength_extraction.py
+-rw-r--r--   0        0        0     2013 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/photonic_circuit_models/__init__.py
+-rw-r--r--   0        0        0      597 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/photonic_circuit_models/coupler.py
+-rw-r--r--   0        0        0      377 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/photonic_circuit_models/fsr.py
+-rw-r--r--   0        0        0      418 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/photonic_circuit_models/heater.py
+-rw-r--r--   0        0        0     3009 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/photonic_circuit_models/mzi.py
+-rw-r--r--   0        0        0     2616 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/photonic_circuit_models/ring.py
+-rw-r--r--   0        0        0        0 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/process/__init__.py
+-rw-r--r--   0        0        0     4623 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/process/diffusion.py
+-rw-r--r--   0        0        0     5318 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/process/implant_tables.py
+-rw-r--r--   0        0        0     6901 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/process/pysrim.py
+-rw-r--r--   0        0        0     2182 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/process/silicon.py
+-rw-r--r--   0        0        0     1861 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/process/skew/antimony_si_skew.csv
+-rw-r--r--   0        0        0     1050 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/process/skew/arsenic_si_skew.csv
+-rw-r--r--   0        0        0     1468 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/process/skew/boron_si_skew.csv
+-rw-r--r--   0        0        0     1118 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/process/skew/phosphorus_si_skew.csv
+-rw-r--r--   0        0        0      165 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/sax/__init__.py
+-rw-r--r--   0        0        0    14710 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/sax/build_model.py
+-rw-r--r--   0        0        0        0 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/sax/integrations/__init__.py
+-rw-r--r--   0        0        0     7415 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/sax/integrations/femwell_waveguide_model.py
+-rw-r--r--   0        0        0     6725 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/sax/integrations/meep_FDTD_model.py
+-rw-r--r--   0        0        0     4492 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/sax/integrations/meow_eme_model.py
+-rw-r--r--   0        0        0     1546 2023-08-03 23:24:20.880192 gplugins-0.0.3/gplugins/sax/interpolators.py
+-rw-r--r--   0        0        0     5613 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/sax/mlp.py
+-rw-r--r--   0        0        0     7345 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/sax/models.py
+-rw-r--r--   0        0        0    13837 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/sax/parameter.py
+-rwxr-xr-x   0        0        0     2173 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/sax/plot_model.py
+-rw-r--r--   0        0        0     6672 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/sax/read.py
+-rw-r--r--   0        0        0     1349 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/sax/tests/test_mzi.py
+-rw-r--r--   0        0        0     2255 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/sax/tests/test_mzi_lattice.py
+-rw-r--r--   0        0        0       76 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/sax/tests/test_mzi_lattice/test_mzi_lattice.obtained.yml
+-rw-r--r--   0        0        0       76 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/sax/tests/test_mzi_lattice/test_mzi_lattice.yml
+-rw-r--r--   0        0        0     1393 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/sax/tests/test_parameters.py
+-rw-r--r--   0        0        0      102 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/schematic_editor/__init__.py
+-rw-r--r--   0        0        0    16197 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/schematic_editor/circuitviz.py
+-rw-r--r--   0        0        0    17770 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/schematic_editor/schematic_editor.py
+-rw-r--r--   0        0        0     1541 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/tidy3d/__init__.py
+-rw-r--r--   0        0        0     4448 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/tidy3d/get_results.py
+-rw-r--r--   0        0        0    20040 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/tidy3d/get_simulation.py
+-rw-r--r--   0        0        0    21258 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/tidy3d/get_simulation_grating_coupler.py
+-rw-r--r--   0        0        0     3462 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/tidy3d/materials.py
+-rw-r--r--   0        0        0    37241 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/tidy3d/modes.py
+-rw-r--r--   0        0        0     9326 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/tidy3d/tests/sim_ref.yaml
+-rw-r--r--   0        0        0      730 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/tidy3d/tests/test_modes.py
+-rw-r--r--   0        0        0      262 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/tidy3d/tests/test_modes/test_sweep_width.csv
+-rw-r--r--   0        0        0      260 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/tidy3d/tests/test_modes/test_sweep_width.obtained.csv
+-rw-r--r--   0        0        0      852 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/tidy3d/tests/test_results.py
+-rw-r--r--   0        0        0     1562 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/tidy3d/tests/test_simulation.py
+-rw-r--r--   0        0        0     1709 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/tidy3d/tests/tests_sparameters/test_write_sparameters.py
+-rw-r--r--   0        0        0     1891 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/tidy3d/tests/tests_sparameters/test_write_sparameters_grating_coupler.py
+-rw-r--r--   0        0        0     1192 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/tidy3d/utils.py
+-rw-r--r--   0        0        0    11050 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/tidy3d/write_sparameters.py
+-rw-r--r--   0        0        0     8567 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/tidy3d/write_sparameters_grating_coupler.py
+-rw-r--r--   0        0        0        0 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/utils/__init__.py
+-rw-r--r--   0        0        0     4262 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/utils/add_simulation_markers.py
+-rw-r--r--   0        0        0     3276 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/utils/convert_sparameters.py
+-rw-r--r--   0        0        0      251 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/utils/disable_print.py
+-rw-r--r--   0        0        0     3407 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/utils/get_effective_indices.py
+-rw-r--r--   0        0        0     2893 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/utils/get_sparameters_path.py
+-rw-r--r--   0        0        0     5951 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/utils/plot.py
+-rw-r--r--   0        0        0     2439 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/utils/plot_csv.py
+-rw-r--r--   0        0        0      613 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/utils/port_symmetries.py
+-rw-r--r--   0        0        0       32 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/web/Makefile
+-rw-r--r--   0        0        0       23 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/web/__init__.py
+-rw-r--r--   0        0        0      212 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/web/gds_files/C.gds
+-rw-r--r--   0        0        0      220 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/web/gds_files/C_width20.gds
+-rw-r--r--   0        0        0      218 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/web/gds_files/C_width5.gds
+-rw-r--r--   0        0        0    14536 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/web/gds_files/coh_rx_dual_pol.gds
+-rw-r--r--   0        0        0    13550 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/web/gds_files/coh_rx_single_pol.gds
+-rw-r--r--   0        0        0    13564 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/web/gds_files/coh_rx_single_pol_pad_d_19b6c499.gds
+-rw-r--r--   0        0        0    13564 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/web/gds_files/coh_rx_single_pol_pad_d_d4526895.gds
+-rw-r--r--   0        0        0    10292 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/web/gds_files/coh_tx_dual_pol.gds
+-rw-r--r--   0        0        0     1498 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/web/gds_files/crossing_arm.gds
+-rw-r--r--   0        0        0     7406 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/web/gds_files/dbr_cavity.gds
+-rw-r--r--   0        0        0      440 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/web/gds_files/die_bbox_frame.gds
+-rw-r--r--   0        0        0    27548 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/web/gds_files/loss_deembedding_ch14_23.gds
+-rw-r--r--   0        0        0      872 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/web/gds_files/pad_array_add_fiducials.gds
+-rw-r--r--   0        0        0    39252 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/web/gds_files/spiral_inner_io_add_gra_f2760628.gds
+-rw-r--r--   0        0        0      182 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/web/gds_files/wg.gds
+-rw-r--r--   0        0        0     8606 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/web/main.py
+-rw-r--r--   0        0        0     1998 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/web/middleware.py
+-rwxr-xr-x   0        0        0     7546 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/web/server.py
+-rwxr-xr-x   0        0        0      636 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/web/server_jupyter.py
+-rw-r--r--   0        0        0     1299 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/web/static/client.css
+-rw-r--r--   0        0        0     9598 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/web/static/client.js
+-rw-r--r--   0        0        0      840 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/web/templates/client.html.j2
+-rw-r--r--   0        0        0      481 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/web/templates/file_browser.html.j2
+-rw-r--r--   0        0        0     1999 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/web/templates/filewatcher.html.j2
+-rw-r--r--   0        0        0      236 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/web/templates/footer.html.j2
+-rw-r--r--   0        0        0      242 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/web/templates/gds_history.html.j2
+-rw-r--r--   0        0        0      578 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/web/templates/header.html.j2
+-rw-r--r--   0        0        0      376 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/web/templates/index.html.j2
+-rw-r--r--   0        0        0      995 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/web/templates/navbar.html.j2
+-rw-r--r--   0        0        0      272 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/web/templates/pdk.html.j2
+-rw-r--r--   0        0        0     1871 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/web/templates/viewer.html.j2
+-rw-r--r--   0        0        0       87 2023-08-03 23:24:20.884192 gplugins-0.0.3/gplugins/widget/__init__.py
+-rw-r--r--   0        0        0    14936 2023-08-03 23:24:20.888192 gplugins-0.0.3/gplugins/widget/interactive.py
+-rw-r--r--   0        0        0     3132 2023-08-03 23:24:20.888192 gplugins-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     4927 1970-01-01 00:00:00.000000 gplugins-0.0.3/PKG-INFO
```

### Comparing `gplugins-0.0.2/LICENSE` & `gplugins-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.2/gplugins/add_simulation_markers.py` & `gplugins-0.0.3/gplugins/utils/add_simulation_markers.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.2/gplugins/config.py` & `gplugins-0.0.3/gplugins/config.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.2/gplugins/convert_sparameters.py` & `gplugins-0.0.3/gplugins/utils/convert_sparameters.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,14 +13,19 @@
     df: pd.DataFrame,
     magnitude_suffix: str = "m",
     phase_suffix: str = "a",
 ) -> pd.DataFrame:
     """Converts a pandas CSV sparameters from complex128 format to 2x float64 format.
 
     Adds magnitude_suffix (default m) and phase_suffix (default a) to original keys.
+
+    Args:
+        df: pandas DataFrame.
+        magnitude_suffix: m for module.
+        phase_suffix: a for angle.
     """
     new_df = pd.DataFrame()
 
     for key in df.keys():
         if key != "wavelengths":
             new_df[f"{key}{magnitude_suffix}"] = df[key].real
             new_df[f"{key}{phase_suffix}"] = df[key].imag
@@ -63,22 +68,24 @@
         name = f"{p1}@{m1},{p2}@{m2}"
         S[name] = df["magnitude"].values * np.exp(1j * df["phase"].values)
 
     return S
 
 
 def csv_to_npz(filepath: PathType) -> pathlib.Path:
+    """Convert CSV files into numpy."""
     df = pd.read_csv(filepath)
     sp = pandas_to_numpy(df)
     filepath_npz = pathlib.Path(filepath).with_suffix(".npz")
     np.savez_compressed(filepath_npz, **sp)
     return filepath_npz
 
 
 def convert_directory_csv_to_npz(dirpath: PathType) -> None:
+    """Convert CSV files from directory dirpath into numpy."""
     dirpath = pathlib.Path(dirpath)
     for filepath in tqdm(dirpath.glob("**/*.csv")):
         try:
             csv_to_npz(filepath)
         except Exception as e:
             print(filepath)
             print(e)
```

### Comparing `gplugins-0.0.2/gplugins/dagster/workflow.py` & `gplugins-0.0.3/gplugins/dagster/workflow.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.2/gplugins/database/README.md` & `gplugins-0.0.3/gplugins/database/README.md`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.2/gplugins/database/db_upload.py` & `gplugins-0.0.3/gplugins/database/db_upload.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """ Upload a component / simulation result to the database """
 
 import hashlib
 import os
 import tempfile
-from functools import lru_cache
+from functools import cache
 
 import boto3
 import boto3.session
 import gdsfactory as gf
 import numpy as np
 import pandas as pd
 from sqlmodel import Field, SQLModel, create_engine
@@ -42,28 +42,28 @@
     wavelength: float
     port_in: str = Field(min_length=1, max_length=10)
     port_out: str = Field(min_length=1, max_length=10)
     abs: float
     angle: float
 
 
-@lru_cache(maxsize=None)
+@cache
 def get_database_engine():
     host = os.getenv("PS_HOST", "")
     database = os.getenv("PS_DATABASE", "")
     username = os.getenv("PS_USERNAME", "")
     password = os.getenv("PS_PASSWORD", "")
     ssl_ca = os.getenv("PS_SSL_CERT", "")
     connection_string = f"mysql+pymysql://{username}:{password}@{host}/{database}"
     return create_engine(
         connection_string, echo=True, connect_args={"ssl": {"ca": ssl_ca}}
     )
 
 
-@lru_cache(maxsize=None)
+@cache
 def s3_client():
     return boto3.client("s3")
 
 
 def get_component_hash(component: gf.Component) -> str:
     with tempfile.NamedTemporaryFile() as file:
         path = os.path.abspath(file.name)
```

### Comparing `gplugins-0.0.2/gplugins/database/models.py` & `gplugins-0.0.3/gplugins/database/models.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.2/gplugins/devsim/__init__.py` & `gplugins-0.0.3/gplugins/devsim/__init__.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.2/gplugins/devsim/doping.py` & `gplugins-0.0.3/gplugins/devsim/doping.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.2/gplugins/devsim/get_simulation.py` & `gplugins-0.0.3/gplugins/devsim/get_simulation.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.2/gplugins/devsim/get_simulation_xsection.py` & `gplugins-0.0.3/gplugins/devsim/get_simulation_xsection.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,17 +19,17 @@
 import numpy as np
 import pyvista as pv
 import tidy3d as td
 from devsim.python_packages import model_create, simple_physics
 from pydantic import BaseModel, Extra
 from scipy.interpolate import griddata
 
-from gplugins.disable_print import disable_print, enable_print
-from gplugins.gtidy3d.materials import get_nk
-from gplugins.gtidy3d.modes import Precision, Waveguide
+from gplugins.tidy3d.materials import get_nk
+from gplugins.tidy3d.modes import Precision, Waveguide
+from gplugins.utils.disable_print import disable_print, enable_print
 
 if TYPE_CHECKING:
     from gdsfactory.typings import MaterialSpec
 
 nm = 1e-9
 um = 1e-6
 cm = 1e-2
```

### Comparing `gplugins-0.0.2/gplugins/devsim/get_solver.py` & `gplugins-0.0.3/gplugins/devsim/get_solver.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.2/gplugins/devsim/test_devsim.py` & `gplugins-0.0.3/gplugins/devsim/test_devsim.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.2/gplugins/eme/meow_eme.py` & `gplugins-0.0.3/gplugins/meow/meow_eme.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,18 +13,35 @@
 from gdsfactory.generic_tech import LAYER
 from gdsfactory.pdk import get_active_pdk, get_layer_stack
 from gdsfactory.technology import LayerStack
 from gdsfactory.typings import PathType
 from meow.base_model import _array as mw_array
 from tqdm.auto import tqdm
 
-from gplugins.get_sparameters_path import (
+from gplugins.utils.get_sparameters_path import (
     get_sparameters_path_meow as get_sparameters_path,
 )
-from gplugins.gmsh.parse_layerstack import list_unique_layerstack_z
+
+
+def list_unique_layerstack_z(
+    layerstack: LayerStack,
+) -> list[float]:
+    """List all unique LayerStack z coordinates.
+
+    Args:
+        layerstack: LayerStack
+    Returns:
+        Sorted set of z-coordinates for this layerstack
+    """
+    thicknesses = [layer.thickness for layer in layerstack.layers.values()]
+    zmins = [layer.zmin for layer in layerstack.layers.values()]
+    zmaxs = [sum(value) for value in zip(zmins, thicknesses)]
+
+    return sorted(set(zmins + zmaxs))
+
 
 ColorRGB = tuple[float, float, float]
 
 material_to_color_default = {
     "si": (0.9, 0, 0, 0.9),
     "sio2": (0.9, 0.9, 0.9, 0.9),
     "sin": (0.0, 0.9, 0.0, 0.9),
```

### Comparing `gplugins-0.0.2/gplugins/eme/test_meow_simulation.py` & `gplugins-0.0.3/gplugins/meow/test_meow_simulation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import gdsfactory as gf
 import numpy as np
 from gdsfactory.pdk import get_layer_stack
 from gdsfactory.technology import LayerStack
 
-from gplugins.eme import MEOW
+from gplugins.meow import MEOW
 
 PDK = gf.get_generic_pdk()
 PDK.activate()
 
 
 def test_meow_defaults() -> None:
     c = gf.components.taper_cross_section_linear()
```

### Comparing `gplugins-0.0.2/gplugins/fem/mode_solver.py` & `gplugins-0.0.3/gplugins/femwell/mode_solver.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.2/gplugins/fem/solve_thermal.py` & `gplugins-0.0.3/gplugins/femwell/solve_thermal.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.2/gplugins/fem/test_mode_solver.py` & `gplugins-0.0.3/gplugins/femwell/test_mode_solver.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import gdsfactory as gf
 import numpy as np
 from gdsfactory.generic_tech import LAYER_STACK
 from gdsfactory.technology import LayerStack
 
-from gplugins.fem.mode_solver import Modes, compute_cross_section_modes
+from gplugins.femwell.mode_solver import Modes, compute_cross_section_modes
 
 NUM_MODES = 1
 
 PDK = gf.get_generic_pdk()
 PDK.activate()
```

### Comparing `gplugins-0.0.2/gplugins/get_effective_indices.py` & `gplugins-0.0.3/gplugins/utils/get_effective_indices.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.2/gplugins/get_sparameters_path.py` & `gplugins-0.0.3/gplugins/utils/get_sparameters_path.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from functools import partial
 from pathlib import Path
 
 import gdsfactory as gf
 import numpy as np
 from gdsfactory.name import clean_value
 from gdsfactory.pdk import get_sparameters_path
-from gdsfactory.typings import ComponentSpec
+from gdsfactory.typings import ComponentSpec, PathType
 
 
 def get_kwargs_hash(**kwargs) -> str:
     """Returns kwargs parameters hash."""
     kwargs_list = [f"{key}={clean_value(kwargs[key])}" for key in sorted(kwargs.keys())]
     kwargs_string = "_".join(kwargs_list)
     return hashlib.md5(kwargs_string.encode()).hexdigest()
@@ -24,15 +24,15 @@
     h = hashlib.md5(gdspath.read_bytes()).hexdigest()
     gdspath.unlink()
     return h
 
 
 def _get_sparameters_path(
     component: ComponentSpec,
-    dirpath: Path | None = None,
+    dirpath: PathType | None = None,
     **kwargs,
 ) -> Path:
     """Return Sparameters npz filepath hashing simulation settings for \
             a consistent unique name.
 
     Args:
         component: component or component factory.
```

### Comparing `gplugins-0.0.2/gplugins/gmeep/__init__.py` & `gplugins-0.0.3/gplugins/gmeep/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 except ModuleNotFoundError as e:
     print("You need to 'conda install -c conda-forge pymeep=*=mpi_mpich_* nlopt -y'")
     raise e
 
 from gdsfactory.config import logger
 
 from gplugins import plot, port_symmetries
-from gplugins.get_sparameters_path import get_sparameters_data_meep
 from gplugins.gmeep.get_simulation import get_simulation
 from gplugins.gmeep.meep_adjoint_optimization import (
     get_meep_adjoint_optimizer,
     run_meep_adjoint_optimizer,
 )
 from gplugins.gmeep.write_sparameters_grating import (
     write_sparameters_grating,
@@ -31,14 +30,15 @@
     write_sparameters_meep_batch_1x1_bend90,
 )
 from gplugins.gmeep.write_sparameters_meep_mpi import (
     write_sparameters_meep_mpi,
     write_sparameters_meep_mpi_1x1,
     write_sparameters_meep_mpi_1x1_bend90,
 )
+from gplugins.utils.get_sparameters_path import get_sparameters_data_meep
 
 logger.info(f"Meep {mp.__version__!r} installed at {mp.__path__!r}")
 
 __all__ = [
     "get_meep_adjoint_optimizer",
     "get_simulation",
     "get_sparameters_data_meep",
```

### Comparing `gplugins-0.0.2/gplugins/gmeep/async_utils.py` & `gplugins-0.0.3/gplugins/gmeep/async_utils.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.2/gplugins/gmeep/get_material.py` & `gplugins-0.0.3/gplugins/gmeep/get_material.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     name = name.lower()
 
     if name not in material_name_to_meep and name not in materials:
         raise KeyError(f"material {name!r} not found in available materials")
 
     meep_name = material_name_to_meep[name]
 
-    if isinstance(meep_name, (int, float)):
+    if isinstance(meep_name, int | float):
         # if material is only a number, we can return early regardless of dispersion
         return mp.Medium(index=meep_name)
 
     material = getattr(mat, meep_name)
 
     if dispersive:
         return material
```

### Comparing `gplugins-0.0.2/gplugins/gmeep/get_meep_geometry.py` & `gplugins-0.0.3/gplugins/gmeep/get_meep_geometry.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.2/gplugins/gmeep/get_port_eigenmode.py` & `gplugins-0.0.3/gplugins/gmeep/get_port_eigenmode.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.2/gplugins/gmeep/get_simulation.py` & `gplugins-0.0.3/gplugins/gmeep/get_simulation.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.2/gplugins/gmeep/get_simulation_grating_farfield.py` & `gplugins-0.0.3/gplugins/gmeep/get_simulation_grating_farfield.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.2/gplugins/gmeep/get_simulation_grating_fiber.py` & `gplugins-0.0.3/gplugins/gmeep/get_simulation_grating_fiber.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.2/gplugins/gmeep/meep_adjoint_optimization.py` & `gplugins-0.0.3/gplugins/gmeep/meep_adjoint_optimization.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.2/gplugins/gmeep/test_eigenmode.py` & `gplugins-0.0.3/gplugins/gmeep/test_eigenmode.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.2/gplugins/gmeep/test_materials.py` & `gplugins-0.0.3/gplugins/gmeep/test_materials.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.2/gplugins/gmeep/test_sparameterNxN/test_sparameterNxN_crossing.csv` & `gplugins-0.0.3/gplugins/gmeep/test_sparameterNxN/test_sparameterNxN_crossing.csv`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.2/gplugins/gmeep/test_sparameterNxN/test_sparameterNxN_straight.csv` & `gplugins-0.0.3/gplugins/gmeep/test_sparameterNxN/test_sparameterNxN_straight.csv`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.2/gplugins/gmeep/test_write_sparameters_meep.py` & `gplugins-0.0.3/gplugins/gmeep/test_write_sparameters_meep.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.2/gplugins/gmeep/test_write_sparameters_meep/test_sparameterNxN_crossing.csv` & `gplugins-0.0.3/gplugins/gmeep/test_write_sparameters_meep/test_sparameterNxN_crossing.csv`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.2/gplugins/gmeep/test_write_sparameters_meep/test_sparameterNxN_straight.csv` & `gplugins-0.0.3/gplugins/gmeep/test_write_sparameters_meep/test_sparameterNxN_straight.csv`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.2/gplugins/gmeep/test_write_sparameters_meep/test_sparameterNxN_symmetries_straight.csv` & `gplugins-0.0.3/gplugins/gmeep/test_write_sparameters_meep/test_sparameterNxN_symmetries_straight.csv`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.2/gplugins/gmeep/test_write_sparameters_meep/test_sparameter_straight_mpi.csv` & `gplugins-0.0.3/gplugins/gmeep/test_write_sparameters_meep/test_sparameter_straight_mpi.csv`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.2/gplugins/gmeep/test_write_sparameters_meep/test_sparameter_straight_mpi_pool.csv` & `gplugins-0.0.3/gplugins/gmeep/test_write_sparameters_meep/test_sparameter_straight_mpi_pool.csv`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.2/gplugins/gmeep/test_write_sparameters_meep/test_sparameters_crossing_symmetric.csv` & `gplugins-0.0.3/gplugins/gmeep/test_write_sparameters_meep/test_sparameters_crossing_symmetric.csv`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.2/gplugins/gmeep/test_write_sparameters_meep/test_sparameters_straight.csv` & `gplugins-0.0.3/gplugins/gmeep/test_write_sparameters_meep/test_sparameters_straight.csv`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.2/gplugins/gmeep/test_write_sparameters_meep/test_sparameters_straight_batch.csv` & `gplugins-0.0.3/gplugins/gmeep/test_write_sparameters_meep/test_sparameters_straight_batch.csv`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.2/gplugins/gmeep/test_write_sparameters_meep/test_sparameters_straight_mpi.csv` & `gplugins-0.0.3/gplugins/gmeep/test_write_sparameters_meep/test_sparameters_straight_mpi.csv`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.2/gplugins/gmeep/test_write_sparameters_meep/test_sparameters_straight_mpi_pool.csv` & `gplugins-0.0.3/gplugins/gmeep/test_write_sparameters_meep/test_sparameters_straight_mpi_pool.csv`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.2/gplugins/gmeep/test_write_sparameters_meep/test_sparameters_straight_symmetric.csv` & `gplugins-0.0.3/gplugins/gmeep/test_write_sparameters_meep/test_sparameters_straight_symmetric.csv`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.2/gplugins/gmeep/write_sparameters_grating.py` & `gplugins-0.0.3/gplugins/gmeep/write_sparameters_grating.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.2/gplugins/gmeep/write_sparameters_meep.py` & `gplugins-0.0.3/gplugins/gmeep/write_sparameters_meep.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,22 +19,22 @@
 from gdsfactory.config import logger
 from gdsfactory.pdk import get_layer_stack
 from gdsfactory.serialization import clean_value_json
 from gdsfactory.technology import LayerStack
 from gdsfactory.typings import ComponentSpec, PathType, Port, PortSymmetries
 from tqdm.auto import tqdm
 
-from gplugins import port_symmetries
-from gplugins.get_sparameters_path import (
-    get_sparameters_path_meep as get_sparameters_path,
-)
 from gplugins.gmeep.get_simulation import (
     get_simulation,
     settings_get_simulation,
 )
+from gplugins.utils import port_symmetries
+from gplugins.utils.get_sparameters_path import (
+    get_sparameters_path_meep as get_sparameters_path,
+)
 
 core_materials = multiprocessing.cpu_count()
 
 
 def remove_simulation_kwargs(d: dict[str, Any]) -> dict[str, Any]:
     """Returns a copy of dict with only simulation settings.
```

### Comparing `gplugins-0.0.2/gplugins/gmeep/write_sparameters_meep_batch.py` & `gplugins-0.0.3/gplugins/gmeep/write_sparameters_meep_batch.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,22 +15,22 @@
 import pydantic
 from gdsfactory.component import Component
 from gdsfactory.config import logger, sparameters_path
 from gdsfactory.pdk import get_layer_stack
 from gdsfactory.technology import LayerStack
 from tqdm.auto import tqdm
 
-from gplugins import port_symmetries
-from gplugins.get_sparameters_path import (
-    get_sparameters_path_meep as get_sparameters_path,
-)
 from gplugins.gmeep.write_sparameters_meep import remove_simulation_kwargs
 from gplugins.gmeep.write_sparameters_meep_mpi import (
     write_sparameters_meep_mpi,
 )
+from gplugins.utils import port_symmetries
+from gplugins.utils.get_sparameters_path import (
+    get_sparameters_path_meep as get_sparameters_path,
+)
 
 core_materials = multiprocessing.cpu_count()
 
 temp_dir_default = Path(sparameters_path) / "temp"
 
 
 @pydantic.validate_arguments
```

### Comparing `gplugins-0.0.2/gplugins/gmeep/write_sparameters_meep_mpi.py` & `gplugins-0.0.3/gplugins/gmeep/write_sparameters_meep_mpi.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,22 +16,22 @@
 import pydantic
 from gdsfactory.component import Component
 from gdsfactory.config import logger, sparameters_path
 from gdsfactory.pdk import get_layer_stack
 from gdsfactory.technology import LayerStack
 from gdsfactory.typings import ComponentSpec, PathType
 
-from gplugins import port_symmetries
-from gplugins.get_sparameters_path import (
-    get_sparameters_path_meep as get_sparameters_path,
-)
 from gplugins.gmeep.write_sparameters_meep import (
     remove_simulation_kwargs,
     settings_write_sparameters_meep,
 )
+from gplugins.utils import port_symmetries
+from gplugins.utils.get_sparameters_path import (
+    get_sparameters_path_meep as get_sparameters_path,
+)
 
 core_materials = multiprocessing.cpu_count()
 
 temp_dir_default = Path(sparameters_path) / "temp"
 
 
 def _python() -> str:
```

### Comparing `gplugins-0.0.2/gplugins/gmsh/__init__.py` & `gplugins-0.0.3/gplugins/gmsh/__init__.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.2/gplugins/gmsh/break_geometry.py` & `gplugins-0.0.3/gplugins/gmsh/break_geometry.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.2/gplugins/gmsh/mesh.py` & `gplugins-0.0.3/gplugins/gmsh/mesh.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.2/gplugins/gmsh/meshtracker.py` & `gplugins-0.0.3/gplugins/gmsh/meshtracker.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.2/gplugins/gmsh/parse_component.py` & `gplugins-0.0.3/gplugins/gmsh/parse_component.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.2/gplugins/gmsh/parse_gds.py` & `gplugins-0.0.3/gplugins/gmsh/parse_gds.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.2/gplugins/gmsh/parse_layerstack.py` & `gplugins-0.0.3/gplugins/gmsh/parse_layerstack.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import numpy as np
 from gdsfactory.technology import LayerStack
 
 
 def list_unique_layerstack_z(
     layerstack: LayerStack,
-):
+) -> list[float]:
     """List all unique LayerStack z coordinates.
 
     Args:
         layerstack: LayerStack
     Returns:
         Sorted set of z-coordinates for this layerstack
     """
```

### Comparing `gplugins-0.0.2/gplugins/gmsh/refine.py` & `gplugins-0.0.3/gplugins/gmsh/refine.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.2/gplugins/gmsh/scratch/mesh3D.py` & `gplugins-0.0.3/gplugins/gmsh/scratch/mesh3D.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.2/gplugins/gmsh/tests/test_meshing.py` & `gplugins-0.0.3/gplugins/gmsh/tests/test_meshing.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.2/gplugins/gmsh/uz_xsection_mesh.py` & `gplugins-0.0.3/gplugins/gmsh/uz_xsection_mesh.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.2/gplugins/gmsh/xy_xsection_mesh.py` & `gplugins-0.0.3/gplugins/gmsh/xy_xsection_mesh.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.2/gplugins/gtidy3d/__init__.py` & `gplugins-0.0.3/gplugins/tidy3d/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,33 +11,33 @@
     import tidy3d as td
 except ModuleNotFoundError as e:
     print("You need to 'pip install tidy3d'")
     raise e
 
 from gdsfactory.config import logger
 
-from gplugins.gtidy3d import materials, modes, utils
-from gplugins.gtidy3d.get_results import get_results
-from gplugins.gtidy3d.get_simulation import (
+from gplugins.tidy3d import materials, modes, utils
+from gplugins.tidy3d.get_results import get_results
+from gplugins.tidy3d.get_simulation import (
     get_simulation,
     plot_simulation,
     plot_simulation_xz,
     plot_simulation_yz,
 )
-from gplugins.gtidy3d.get_simulation_grating_coupler import (
+from gplugins.tidy3d.get_simulation_grating_coupler import (
     get_simulation_grating_coupler,
 )
-from gplugins.gtidy3d.write_sparameters import (
+from gplugins.tidy3d.write_sparameters import (
     write_sparameters,
     write_sparameters_1x1,
     write_sparameters_batch,
     write_sparameters_batch_1x1,
     write_sparameters_crossing,
 )
-from gplugins.gtidy3d.write_sparameters_grating_coupler import (
+from gplugins.tidy3d.write_sparameters_grating_coupler import (
     write_sparameters_grating_coupler,
     write_sparameters_grating_coupler_batch,
 )
 
 __version__ = "0.0.3"
 __all__ = [
     "plot_simulation",
```

### Comparing `gplugins-0.0.2/gplugins/gtidy3d/get_results.py` & `gplugins-0.0.3/gplugins/tidy3d/get_results.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,15 +128,15 @@
     """
     task_names = [get_sim_hash(sim) for sim in sims]
     batch = web.Batch(simulations=dict(zip(task_names, sims)), verbose=verbose)
     return batch.run(path_dir=dirpath)
 
 
 if __name__ == "__main__":
-    import gplugins.gtidy3d as gt
+    import gplugins.tidy3d as gt
 
     component = gf.components.straight(length=3)
     sim = gt.get_simulation(component=component)
     sim_hash = get_sim_hash(sim)
     # hash_to_id = {d["taskName"]: d["task_id"] for d in web.get_tasks()}
 
     r = sim_data = get_results(sim=sim).result()
```

### Comparing `gplugins-0.0.2/gplugins/gtidy3d/get_simulation.py` & `gplugins-0.0.3/gplugins/tidy3d/get_simulation.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,21 +8,24 @@
 import matplotlib.pyplot as plt
 import numpy as np
 import pydantic
 import tidy3d as td
 from gdsfactory.component import Component
 from gdsfactory.components.extension import move_polar_rad_copy
 from gdsfactory.config import logger
-from gdsfactory.pdk import get_layer_stack, get_material_index
+from gdsfactory.pdk import get_layer_stack
 from gdsfactory.routing.sort_ports import sort_ports_x, sort_ports_y
 from gdsfactory.technology import LayerStack
 from gdsfactory.typings import ComponentSpec, Float2
 from tidy3d.plugins.mode import ModeSolver
 
-from gplugins.gtidy3d.materials import get_index, get_medium
+from gplugins.tidy3d.materials import (
+    get_index,
+    get_medium,
+)
 
 
 @pydantic.validate_arguments
 def get_simulation(
     component: ComponentSpec,
     port_extension: float | None = 4.0,
     layer_stack: LayerStack | None = None,
@@ -41,15 +44,15 @@
     distance_source_to_monitors: float = 0.2,
     wavelength_start: float = 1.50,
     wavelength_stop: float = 1.60,
     wavelength_points: int = 50,
     plot_modes: bool = False,
     num_modes: int = 2,
     run_time_ps: float = 10.0,
-    material_name_to_tidy3d: dict[str, str] | None = None,
+    material_name_to_tidy3d: None | dict[str, str] = None,
     is_3d: bool = True,
     with_all_monitors: bool = False,
     boundary_spec: td.BoundarySpec | None = None,
     grid_spec: td.GridSpec | None = None,
     sidewall_angle_deg: float = 0,
     dilation: float = 0.0,
     **kwargs,
@@ -176,15 +179,16 @@
 
         c = gf.components.bend_circular()
         sim = gt.get_simulation(c)
         gt.plot_simulation(sim)
 
     """
     component = gf.get_component(component)
-    assert isinstance(component, Component)
+    if not isinstance(component, Component):
+        raise ValueError(f"component should be a gdsfactory.Component not {component}")
 
     layer_stack = layer_stack or get_layer_stack()
     if is_3d:
         boundary_spec = boundary_spec or td.BoundarySpec.all_sides(boundary=td.PML())
 
     else:
         boundary_spec = boundary_spec or td.BoundarySpec(
@@ -197,17 +201,14 @@
     grid_spec = grid_spec or td.GridSpec.auto(wavelength=wavelength)
 
     layer_to_thickness = layer_stack.get_layer_to_thickness()
     layer_to_material = layer_stack.get_layer_to_material()
     layer_to_zmin = layer_stack.get_layer_to_zmin()
     # layer_to_sidewall_angle = layer_stack.get_layer_to_sidewall_angle()
 
-    assert isinstance(
-        component, Component
-    ), f"component needs to be a gf.Component, got Type {type(component)}"
     if port_source_name not in component.ports:
         warnings.warn(
             f"port_source_name={port_source_name!r} not in {list(component.ports.keys())}"
         )
         port_source = component.get_ports_list(port_type="optical")[0]
         port_source_name = port_source.name
         warnings.warn(f"Selecting port_source_name={port_source_name!r} instead.")
@@ -239,15 +240,17 @@
     component_ref.y = 0
 
     material_name_to_tidy3d = material_name_to_tidy3d or {}
 
     if material_name_to_tidy3d:
         clad_material_name_or_index = material_name_to_tidy3d[clad_material]
     else:
-        clad_material_name_or_index = get_material_index(clad_material, wavelength)
+        clad_material_name_or_index = (
+            clad_material(wavelength) if callable(clad_material) else clad_material
+        )
 
     clad = td.Structure(
         geometry=td.Box(
             size=(td.inf, td.inf, td.inf),
             center=(0, 0, 0),
         ),
         medium=get_medium(name_or_index=clad_material_name_or_index),
@@ -282,15 +285,19 @@
                 medium = get_medium(name_or_index=name_or_index)
                 index = get_index(name_or_index=name_or_index)
                 logger.debug(
                     f"Add {layer}, {name_or_index!r}, index = {index:.3f}, "
                     f"thickness = {thickness}, zmin = {zmin}, zmax = {zmax}"
                 )
             else:
-                material_index = get_material_index(material_name, wavelength)
+                material_index = (
+                    material_name(wavelength)
+                    if callable(material_name)
+                    else material_name
+                )
                 medium = get_medium(material_index)
 
             polygons = td.PolySlab.from_gds(
                 gds_cell=component_extended._cell,
                 gds_layer=layer[0],
                 gds_dtype=layer[1],
                 axis=2,
@@ -523,15 +530,15 @@
     # sim = get_simulation(c, is_3d=True)
     # plot_simulation(sim)
 
     # filepath = pathlib.Path(__file__).parent / "extra" / "wg2d.json"
     # filepath.write_text(sim.json())
 
     # sim.plotly(z=0)
-    plot_simulation_yz(s, wavelength=1.55, y=1)
+    # plot_simulation_yz(s, wavelength=1.55, y=1)
     # fig = plt.figure(figsize=(11, 4))
     # gs = mpl.gridspec.GridSpec(1, 2, figure=fig, width_ratios=[1, 1.4])
     # ax1 = fig.add_subplot(gs[0, 0])
     # ax2 = fig.add_subplot(gs[0, 1])
     # sim.plot(z=0.0, ax=ax1)
     # sim.plot(x=0.0, ax=ax2)
     # plt.show()
```

### Comparing `gplugins-0.0.2/gplugins/gtidy3d/get_simulation_grating_coupler.py` & `gplugins-0.0.3/gplugins/tidy3d/get_simulation_grating_coupler.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,54 +6,57 @@
 import gdsfactory as gf
 import matplotlib.pyplot as plt
 import numpy as np
 import tidy3d as td
 from gdsfactory.component import Component
 from gdsfactory.components.extension import move_polar_rad_copy
 from gdsfactory.config import logger
-from gdsfactory.pdk import get_layer_stack, get_material_index
+from gdsfactory.pdk import get_layer_stack
 from gdsfactory.technology import LayerStack
 from gdsfactory.typings import CrossSectionSpec
 from tidy3d.plugins.mode import ModeSolver
 
-from gplugins.gtidy3d.materials import get_index, get_medium
+from gplugins.tidy3d.materials import (
+    get_index,
+    get_medium,
+)
 
 
 def get_simulation_grating_coupler(
     component: Component,
-    port_extension: float | None = 10.0,
+    port_extension: float = 10.0,
     layer_stack: LayerStack | None = None,
     thickness_pml: float = 1.0,
     xmargin: float = 0,
     ymargin: float = 0,
     xmargin_left: float = 0,
     xmargin_right: float = 0,
     ymargin_top: float = 0,
     ymargin_bot: float = 0,
     zmargin: float = 1.0,
     clad_material: str = "sio2",
     box_material: str = "sio2",
-    box_thickness: float = 2.0,
+    box_thickness: float = 3.0,
     substrate_material: str = "si",
     port_waveguide_name: str = "o1",
     port_margin: float = 0.5,
     port_waveguide_offset: float = 0.1,
-    wavelength: float | None = 1.55,
+    wavelength: float = 1.55,
     wavelength_start: float = 1.20,
     wavelength_stop: float = 1.80,
     wavelength_points: int = 256,
     plot_modes: bool = False,
     num_modes: int = 2,
     run_time_ps: float = 10.0,
     fiber_port_prefix: str = "opt",
     fiber_xoffset: float = -7,
     fiber_z: float = 2,
     fiber_mfd: float = 10.4,
     fiber_angle_deg: float = 20.0,
-    material_name_to_tidy3d: dict[str, str] | None = None,
+    material_name_to_tidy3d: None | dict[str, str] = None,
     is_3d: bool = True,
     with_all_monitors: bool = False,
     boundary_spec: td.BoundarySpec | None = None,
     grid_spec: td.GridSpec | None = None,
     sidewall_angle_deg: float = 0,
     dilation: float = 0.0,
     cross_section: CrossSectionSpec | None = None,
@@ -201,15 +204,15 @@
             but result in longer simulation times.
         version: String specifying the front end version number.
 
     .. code::
 
         import matplotlib.pyplot as plt
         import gdsfactory as gf
-        import gplugins.gtidy3d as gt
+        import gplugins.tidy3d as gt
 
         c = gf.components.grating_coupler_elliptical_arbitrary(
             widths=[0.343] * 25, gaps=[0.345] * 25
         )
         sim = gt.get_simulation(c)
         gt.plot_simulation(sim)
 
@@ -229,17 +232,16 @@
             y=td.Boundary.periodic(),
             z=td.Boundary.pml(),
         )
     )
 
     grid_spec = grid_spec or td.GridSpec.auto(wavelength=wavelength)
 
-    assert isinstance(
-        component, Component
-    ), f"component needs to be a gf.Component, got Type {type(component)}"
+    if not isinstance(component, Component):
+        raise ValueError(f"component should be a gdsfactory.Component not {component}")
 
     if port_waveguide_name not in component.ports:
         warnings.warn(
             f"port_waveguide_name={port_waveguide_name!r} not in {component.ports.keys()}"
         )
         port_waveguide = component.get_ports_list()[0]
         port_waveguide_name = port_waveguide.name
@@ -300,18 +302,24 @@
     material_name_to_tidy3d = material_name_to_tidy3d or {}
 
     if material_name_to_tidy3d:
         clad_material_name_or_index = material_name_to_tidy3d[clad_material]
         box_material_name_or_index = material_name_to_tidy3d[box_material]
         substrate_material_name_or_index = material_name_to_tidy3d[substrate_material]
     else:
-        clad_material_name_or_index = get_material_index(clad_material, wavelength)
-        box_material_name_or_index = get_material_index(box_material, wavelength)
-        substrate_material_name_or_index = get_material_index(
-            substrate_material, wavelength
+        clad_material_name_or_index = (
+            clad_material(wavelength) if callable(clad_material) else clad_material
+        )
+        box_material_name_or_index = (
+            box_material(wavelength) if callable(box_material) else box_material
+        )
+        substrate_material_name_or_index = (
+            substrate_material(wavelength)
+            if callable(substrate_material)
+            else substrate_material
         )
 
     clad = td.Structure(
         geometry=td.Box(
             size=(td.inf, td.inf, sim_zsize),
             center=(0, 0, sim_zsize / 2),
         ),
@@ -350,15 +358,19 @@
                 index = get_index(name_or_index=name_or_index)
                 logger.debug(
                     f"Add {layer}, {name_or_index!r}, index = {index:.3f}, "
                     f"thickness = {thickness}, zmin = {zmin}, zmax = {zmax}"
                 )
 
             else:
-                material_index = get_material_index(material_name, wavelength)
+                material_index = (
+                    material_name(wavelength)
+                    if callable(material_name)
+                    else material_name
+                )
                 medium = get_medium(material_index)
 
             polygons = td.PolySlab.from_gds(
                 gds_cell=component_extended._cell,
                 gds_layer=layer[0],
                 gds_dtype=layer[1],
                 axis=2,
@@ -397,15 +409,15 @@
         (core_thickness + zmargin - box_thickness) / 2
     ]  # (x, y, z)
 
     waveguide_monitor = td.ModeMonitor(
         center=waveguide_port_center,
         size=waveguide_port_size,
         freqs=freqs,
-        mode_spec=td.ModeSpec(num_modes=1),
+        mode_spec=td.ModeSpec(num_modes=1, precision="double"),
         name="waveguide",
     )
 
     # Add fiber monitor
     fiber_port = component_ref.ports[fiber_port_name]
     fiber_port_x = fiber_port.x + fiber_xoffset
 
@@ -507,28 +519,26 @@
             axs[mode_ind, 0].set_aspect("equal")
             axs[mode_ind, 1].set_aspect("equal")
         plt.show()
     return sim
 
 
 if __name__ == "__main__":
-    import gplugins.gtidy3d as gt
-
     c = gf.components.grating_coupler_elliptical_trenches()
 
     # c = gf.components.grating_coupler_elliptical_arbitrary(
     #     widths=[0.343] * 25, gaps=[0.345] * 25
     # )
     sim = get_simulation_grating_coupler(
         c,
         plot_modes=False,
         is_3d=False,
         fiber_angle_deg=20,
     )
-    gt.plot_simulation(sim)  # make sure simulations looks good
+    # gt.plot_simulation(sim)  # make sure simulations looks good
 
     # c = gf.components.grating_coupler_elliptical_lumerical()  # inverse design grating
     # sim = get_simulation_grating_coupler(c, plot_modes=False, fiber_angle_deg=-5)
     # sim_data = gt.get_results(sim).result()
     # freq0 = td.constants.C_0 / 1.55
     # fig, (ax1, ax2, ax3) = plt.subplots(3, 1, tight_layout=True, figsize=(14, 16))
     # sim_data.plot_field("full_domain_fields", "Ey", freq=freq0, z=0, ax=ax1)
```

### Comparing `gplugins-0.0.2/gplugins/gtidy3d/materials.py` & `gplugins-0.0.3/gplugins/tidy3d/materials.py`

 * *Files 5% similar despite different names*

```diff
@@ -89,15 +89,15 @@
         material_name_to_medium: map name to medium.
 
     """
     name_or_index = (
         name_or_index.lower() if isinstance(name_or_index, str) else name_or_index
     )
 
-    if isinstance(name_or_index, (int, float)):
+    if isinstance(name_or_index, int | float):
         m = td.Medium(permittivity=name_or_index**2)
     elif name_or_index in material_name_to_medium:
         m = material_name_to_medium[name_or_index]
     else:
         materials = list(material_name_to_medium.keys())
 
         raise ValueError(f"Material {name_or_index!r} not in {materials}")
@@ -105,17 +105,17 @@
     return m
 
 
 si = partial(get_index, "si")
 sio2 = partial(get_index, "sio2")
 sin = partial(get_index, "sin")
 
-materials = dict(si=si, sio2=sio2, sin=sin)
+material_name_to_function_non_dispersive = dict(si=si, sio2=sio2, sin=sin)
 
 
 if __name__ == "__main__":
     print(si(1.55))
-    print(si(1.31))
-    # print(get_index(name_or_index="cSi"))
+    # print(si(1.31))
+    # print(get_index(name_or_index="si"))
     # print(get_index(name_or_index=3.4))
     # m = get_medium(name_or_index="SiO2")
     # m = td.Medium(permittivity=1.45 ** 2)
```

### Comparing `gplugins-0.0.2/gplugins/gtidy3d/modes.py` & `gplugins-0.0.3/gplugins/tidy3d/modes.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from gdsfactory.config import logger
 from gdsfactory.pdk import MaterialSpec, get_modes_path
 from gdsfactory.serialization import clean_value_name
 from gdsfactory.typings import PathType
 from tidy3d.plugins import waveguide
 from tqdm.auto import tqdm
 
-from gplugins.gtidy3d.materials import get_medium
+from gplugins.tidy3d.materials import get_medium
 
 Precision = Literal["single", "double"]
 nm = 1e-3
 
 
 class Waveguide(pydantic.BaseModel):
     """Waveguide Model.
```

### Comparing `gplugins-0.0.2/gplugins/gtidy3d/sim_run.yaml` & `gplugins-0.0.3/gplugins/tidy3d/tests/sim_ref.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -96,227 +96,249 @@
                 type: PMLParams
             type: PML
         type: Boundary
 center:
 - 0.0
 - 0.0
 - 0.0
-courant: 0.9
-grid_size: null
+courant: 0.99
 grid_spec:
     grid_x:
+        dl_min: 0.0
         max_scale: 1.4
         mesher:
             type: GradedMesher
         min_steps_per_wvl: 10.0
         type: AutoGrid
     grid_y:
+        dl_min: 0.0
         max_scale: 1.4
         mesher:
             type: GradedMesher
         min_steps_per_wvl: 10.0
         type: AutoGrid
     grid_z:
+        dl_min: 0.0
         max_scale: 1.4
         mesher:
             type: GradedMesher
         min_steps_per_wvl: 10.0
         type: AutoGrid
     override_structures: []
     type: GridSpec
-    wavelength: null
+    wavelength: 1.55
 medium:
+    allow_gain: false
     conductivity: 0.0
     frequency_range: null
     name: null
     permittivity: 1.0
     type: Medium
 monitors:
--   center:
+-   apodization:
+        end: null
+        start: null
+        type: ApodizationSpec
+        width: null
+    center:
     - -1.3
     - -2.4492935982947065e-17
     - 0.0
     freqs:
-        data_list:
-        - 199861639053964.53
-        - 199590087913945.56
-        - 199319273683397.47
-        - 199049193366753.28
-        - 198779843984660.25
-        - 198511222573870.2
-        - 198243326187130.84
-        - 197976151893078.1
-        - 197709696776129.12
-        - 197443957936376.25
-        - 197178932489481.78
-        - 196914617566573.62
-        - 196651010314141.8
-        - 196388107893935.72
-        - 196125907482862.38
-        - 195864406272885.25
-        - 195603601470924.03
-        - 195343490298755.25
-        - 195084069992913.6
-        - 194825337804594.1
-        - 194567290999554.88
-        - 194309926858021.06
-        - 194053242674589.06
-        - 193797235758131.84
-        - 193541903431704.78
-        - 193287243032452.56
-        - 193033251911516.34
-        - 192779927433942.2
-        - 192527266978589.7
-        - 192275267938041.8
-        - 192023927718514.94
-        - 191773243739770.16
-        - 191523213435024.7
-        - 191273834250864.5
-        - 191025103647157.25
-        - 190777019096966.16
-        - 190529578086464.25
-        - 190282778114849.66
-        - 190036616694261.25
-        - 189791091349695.0
-        - 189546199618921.2
-        - 189301939052401.97
-        - 189058307213209.7
-        - 188815301676945.9
-        - 188572920031661.0
-        - 188331159877774.28
-        - 188090018827994.8
-        - 187849494507242.88
-        - 187609584552572.06
-        - 187370286613091.75
+    - 199861638666666.66
+    - 199590087527173.9
+    - 199319273297150.6
+    - 199049192981029.8
+    - 198779843599458.72
+    - 198511222189189.2
+    - 198243325802968.97
+    - 197976151509433.97
+    - 197709696393001.34
+    - 197443957553763.44
+    - 197178932107382.56
+    - 196914617184986.6
+    - 196651009933065.6
+    - 196388107513368.97
+    - 196125907102803.72
+    - 195864405893333.34
+    - 195603601091877.5
+    - 195343489920212.78
+    - 195084069614873.84
+    - 194825337427055.7
+    - 194567290622516.56
+    - 194309926481481.47
+    - 194053242298546.88
+    - 193797235382585.75
+    - 193541903056653.47
+    - 193287242657894.75
+    - 193033251537450.72
+    - 192779927060367.47
+    - 192527266605504.6
+    - 192275267565445.03
+    - 192023927346405.22
+    - 191773243368146.2
+    - 191523213063885.25
+    - 191273833880208.3
+    - 191025103276983.06
+    - 190777018727272.72
+    - 190529577717250.3
+    - 190282777746114.0
+    - 190036616326002.6
+    - 189791090981912.12
+    - 189546199251612.9
+    - 189301938685567.0
+    - 189058306846846.84
+    - 188815301311053.97
+    - 188572919666238.75
+    - 188331159512820.5
+    - 188090018463508.3
+    - 187849494143222.5
+    - 187609584189016.6
+    - 187370286250000.0
     mode_spec:
         angle_phi: 0.0
         angle_theta: 0.0
         bend_axis: null
         bend_radius: null
+        filter_pol: null
+        group_index_step: false
         num_modes: 1
         num_pml:
         - 0
         - 0
-        sort_by: largest_neff
+        precision: single
         target_neff: null
+        track_freq: central
         type: ModeSpec
     name: o1
     size:
     - 0.0
     - 1.5
-    - 2.2199999999999998
+    - 5.0
     type: ModeMonitor
--   center:
+-   apodization:
+        end: null
+        start: null
+        type: ApodizationSpec
+        width: null
+    center:
     - 1.5
     - 0.0
     - 0.0
     freqs:
-        data_list:
-        - 199861639053964.53
-        - 199590087913945.56
-        - 199319273683397.47
-        - 199049193366753.28
-        - 198779843984660.25
-        - 198511222573870.2
-        - 198243326187130.84
-        - 197976151893078.1
-        - 197709696776129.12
-        - 197443957936376.25
-        - 197178932489481.78
-        - 196914617566573.62
-        - 196651010314141.8
-        - 196388107893935.72
-        - 196125907482862.38
-        - 195864406272885.25
-        - 195603601470924.03
-        - 195343490298755.25
-        - 195084069992913.6
-        - 194825337804594.1
-        - 194567290999554.88
-        - 194309926858021.06
-        - 194053242674589.06
-        - 193797235758131.84
-        - 193541903431704.78
-        - 193287243032452.56
-        - 193033251911516.34
-        - 192779927433942.2
-        - 192527266978589.7
-        - 192275267938041.8
-        - 192023927718514.94
-        - 191773243739770.16
-        - 191523213435024.7
-        - 191273834250864.5
-        - 191025103647157.25
-        - 190777019096966.16
-        - 190529578086464.25
-        - 190282778114849.66
-        - 190036616694261.25
-        - 189791091349695.0
-        - 189546199618921.2
-        - 189301939052401.97
-        - 189058307213209.7
-        - 188815301676945.9
-        - 188572920031661.0
-        - 188331159877774.28
-        - 188090018827994.8
-        - 187849494507242.88
-        - 187609584552572.06
-        - 187370286613091.75
+    - 199861638666666.66
+    - 199590087527173.9
+    - 199319273297150.6
+    - 199049192981029.8
+    - 198779843599458.72
+    - 198511222189189.2
+    - 198243325802968.97
+    - 197976151509433.97
+    - 197709696393001.34
+    - 197443957553763.44
+    - 197178932107382.56
+    - 196914617184986.6
+    - 196651009933065.6
+    - 196388107513368.97
+    - 196125907102803.72
+    - 195864405893333.34
+    - 195603601091877.5
+    - 195343489920212.78
+    - 195084069614873.84
+    - 194825337427055.7
+    - 194567290622516.56
+    - 194309926481481.47
+    - 194053242298546.88
+    - 193797235382585.75
+    - 193541903056653.47
+    - 193287242657894.75
+    - 193033251537450.72
+    - 192779927060367.47
+    - 192527266605504.6
+    - 192275267565445.03
+    - 192023927346405.22
+    - 191773243368146.2
+    - 191523213063885.25
+    - 191273833880208.3
+    - 191025103276983.06
+    - 190777018727272.72
+    - 190529577717250.3
+    - 190282777746114.0
+    - 190036616326002.6
+    - 189791090981912.12
+    - 189546199251612.9
+    - 189301938685567.0
+    - 189058306846846.84
+    - 188815301311053.97
+    - 188572919666238.75
+    - 188331159512820.5
+    - 188090018463508.3
+    - 187849494143222.5
+    - 187609584189016.6
+    - 187370286250000.0
     mode_spec:
         angle_phi: 0.0
         angle_theta: 0.0
         bend_axis: null
         bend_radius: null
+        filter_pol: null
+        group_index_step: false
         num_modes: 1
         num_pml:
         - 0
         - 0
-        sort_by: largest_neff
+        precision: single
         target_neff: null
+        track_freq: central
         type: ModeSpec
     name: o2
     size:
     - 0.0
     - 1.5
-    - 2.2199999999999998
+    - 5.0
     type: ModeMonitor
+normalize_index: 0
 run_time: 1.0e-11
 shutoff: 1.0e-05
 size:
-- 5.002
+- 5.0
 - 2.5
-- 4.22
+- 7.0
 sources:
 -   center:
     - -1.5
     - 0.0
     - 0.0
     direction: +
     mode_index: 0
     mode_spec:
         angle_phi: 0.0
         angle_theta: 0.0
         bend_axis: null
         bend_radius: null
+        filter_pol: null
+        group_index_step: false
         num_modes: 1
         num_pml:
         - 0
         - 0
-        sort_by: largest_neff
+        precision: single
         target_neff: null
+        track_freq: central
         type: ModeSpec
     name: null
+    num_freqs: 1
     size:
     - 0.0
     - 1.5
-    - 2.2199999999999998
+    - 5.0
     source_time:
         amplitude: 1.0
-        freq0: 193414489407062.47
-        fwidth: 19341448940706.246
+        freq0: 193414489032258.1
+        fwidth: 19341448903225.81
         offset: 5.0
         phase: 0.0
         type: GaussianPulse
     type: ModeSource
 structures:
 -   geometry:
         center:
@@ -325,61 +347,71 @@
         - 0.0
         size:
         - Infinity
         - Infinity
         - Infinity
         type: Box
     medium:
-        conductivity: 0.0
-        frequency_range: null
+        allow_gain: false
+        eps_inf: 1.0
+        frequency_range:
+        - 169259246959034.88
+        - 1208994621135963.5
         name: null
-        permittivity: 2.0736
-        type: Medium
+        poles:
+        -   -   imag: -1.823105111824081e+16
+                real: -75963372399806.36
+            -   imag: 1.0209565875622414e+16
+                real: 0.0
+        type: PoleResidue
     name: null
     type: Structure
 -   geometry:
         axis: 2
-        center:
-        - -0.0
-        - 9.420074148334662e-17
-        - 0.11
         dilation: 0.0
-        length: 0.22
+        reference_plane: middle
         sidewall_angle: 0.0
         slab_bounds:
         - 0.0
         - 0.22
         type: PolySlab
         vertices:
         -   - -1.5
             - -0.25
         -   - -5.5
-            - -0.2499999999999995
+            - -0.25
         -   - -5.5
-            - 0.2500000000000005
+            - 0.25
         -   - -1.5
             - 0.25
         -   - 1.5
             - 0.25
         -   - 5.5
             - 0.25
         -   - 5.5
             - -0.25
         -   - 1.5
             - -0.25
         -   - -1.5
             - -0.25
     medium:
-        conductivity: 0.0
-        frequency_range: null
+        allow_gain: false
+        eps_inf: 1.0
+        frequency_range:
+        - 21413747041496.2
+        - 249827048817455.7
         name: null
-        permittivity: 12.0409
-        type: Medium
+        poles:
+        -   -   imag: 6241549589084091.0
+                real: 0.0
+            -   imag: -3.3254308736142404e+16
+                real: 0.0
+        type: PoleResidue
     name: null
     type: Structure
 subpixel: true
 symmetry:
 - 0
 - 0
 - 0
 type: Simulation
-version: 1.4.0
+version: 2.3.3
```

### Comparing `gplugins-0.0.2/gplugins/gtidy3d/tests/test_modes.py` & `gplugins-0.0.3/gplugins/tidy3d/tests/test_modes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 import numpy as np
 
-import gplugins.gtidy3d as gt
+import gplugins.tidy3d as gt
 
 
 def test_neff() -> None:
     wg = gt.modes.Waveguide(
         wavelength=1.55,
         core_width=0.5,
         core_thickness=0.22,
```

### Comparing `gplugins-0.0.2/gplugins/gtidy3d/tests/test_results.py` & `gplugins-0.0.3/gplugins/tidy3d/tests/test_results.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 import gdsfactory as gf
 from gdsfactory.config import PATH
 
-import gplugins.gtidy3d as gt
-from gplugins.gtidy3d.get_results import get_results
+import gplugins.tidy3d as gt
+from gplugins.tidy3d.get_results import get_results
 
 # def test_results_run(data_regression) -> None:
 #     """Run simulations and checks local results."""
 
 #     component = gf.components.straight(length=3)
 #     sim = gt.get_simulation(component=component, is_3d=False)
```

### Comparing `gplugins-0.0.2/gplugins/gtidy3d/tests/test_write_sparameters.py` & `gplugins-0.0.3/gplugins/tidy3d/tests/tests_sparameters/test_write_sparameters.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,44 +1,46 @@
 from __future__ import annotations
 
 import gdsfactory as gf
 import numpy as np
 
-import gplugins.gtidy3d as gt
+import gplugins.tidy3d as gt
+from gplugins.config import PATH
 
 
-def test_sparameters_straight_3d(overwrite=True) -> None:
+def test_sparameters_straight_3d(overwrite=False) -> None:
     """Checks Sparameters for a straight waveguide in 2D."""
     c = gf.components.straight(length=2)
-    sp = gt.write_sparameters_1x1(c, overwrite=overwrite, is_3d=True)
+    sp = gt.write_sparameters_1x1(
+        c, overwrite=overwrite, is_3d=True, dirpath=PATH.sparameters_repo
+    )
 
     assert 1 > np.abs(sp["o1@0,o2@0"]).min() > 0.8, np.abs(sp["o1@0,o2@0"]).min()
     assert 0 < np.abs(sp["o1@0,o1@0"]).max() < 0.1, np.abs(sp["o1@0,o1@0"]).max()
 
 
-def test_sparameters_straight_2d(overwrite=True) -> None:
+def test_sparameters_straight_2d(overwrite=False) -> None:
     """Checks Sparameters for a straight waveguide in 2D."""
     c = gf.components.straight(length=2)
-    sp = gt.write_sparameters_1x1(c, overwrite=overwrite, is_3d=False)
+    sp = gt.write_sparameters_1x1(
+        c, overwrite=overwrite, is_3d=False, dirpath=PATH.sparameters_repo
+    )
 
-    assert 1 > np.abs(sp["o1@0,o2@0"]).min() > 0.7, np.abs(sp["o1@0,o2@0"]).min()
+    assert 1 > np.abs(sp["o1@0,o2@0"]).min() > 0.6, np.abs(sp["o1@0,o2@0"]).min()
     assert 0 < np.abs(sp["o1@0,o1@0"]).max() < 0.1, np.abs(sp["o1@0,o1@0"]).max()
 
     # assert np.allclose(sp["o2@0,o1@0"], 1, atol=1e-02), sp["o2@0,o1@0"]
     # assert np.allclose(sp["o1@0,o1@0"], 0, atol=5e-02), sp["o1@0,o1@0"]
     # assert np.allclose(sp["o2@0,o2@0"], 0, atol=5e-02), sp["o2@0,o2@0"]
 
     # if dataframe_regression:
     #     dataframe_regression.check(sp)
 
 
 if __name__ == "__main__":
-    # test_sparameters_straight()
-
     overwrite = False
-    overwrite = True
     c = gf.components.straight(length=3)
-    sp = gt.write_sparameters_1x1(c, overwrite=overwrite, is_3d=False, run=True)
+    sp = gt.write_sparameters_1x1(c, overwrite=overwrite, is_3d=True, run=True)
 
     # Check reasonable reflection/transmission
-    assert 1 > np.abs(sp["o1@0,o2@0"]).min() > 0.8, np.abs(sp["o1@0,o2@0"]).min()
+    assert 1 > np.abs(sp["o1@0,o2@0"]).min() > 0.6, np.abs(sp["o1@0,o2@0"]).min()
     assert 0 < np.abs(sp["o1@0,o1@0"]).max() < 0.1, np.abs(sp["o1@0,o1@0"]).max()
```

### Comparing `gplugins-0.0.2/gplugins/gtidy3d/tests/test_write_sparameters_grating_coupler.py` & `gplugins-0.0.3/gplugins/tidy3d/tests/tests_sparameters/test_write_sparameters_grating_coupler.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,62 +1,65 @@
 from __future__ import annotations
 
 import gdsfactory as gf
 import numpy as np
 
-import gplugins.gtidy3d as gt
+import gplugins.tidy3d as gt
+from gplugins.config import PATH
 
 fiber_port_name = "o2"
 
 
-def test_sparameters_grating_coupler(overwrite=True) -> None:
+def test_sparameters_grating_coupler(overwrite=False) -> None:
     """Checks Sparameters for a grating_coupler_elliptical_arbitrary in 2D."""
     c = gf.components.grating_coupler_elliptical_arbitrary(
         widths=[0.343] * 25, gaps=[0.345] * 25
     )
 
     fiber_angle_deg = 20
     offsets = [0]
     dfs = [
         gt.write_sparameters_grating_coupler(
             component=c,
             is_3d=False,
             fiber_angle_deg=fiber_angle_deg,
             fiber_xoffset=fiber_xoffset,
             overwrite=overwrite,
+            dirpath=PATH.sparameters_repo,
         )
         for fiber_xoffset in offsets
     ]
     sp = dfs[0]
 
     # Check reasonable reflection/transmission
     transmission = np.abs(sp[f"{fiber_port_name}@0,o1@0"])
     reflection = np.abs(sp["o1@0,o1@0"])
 
     assert 1 > transmission.max() > 0.2, transmission.max()
     assert 0.3 > reflection.max() > 0, reflection.max()
 
 
 if __name__ == "__main__":
-    overwrite = False
-    c = gf.components.grating_coupler_elliptical_arbitrary(
-        widths=[0.343] * 25, gaps=[0.345] * 25
-    )
-
-    fiber_angle_deg = 20
-    offsets = [0, 1]
-    dfs = [
-        gt.write_sparameters_grating_coupler(
-            component=c,
-            is_3d=False,
-            fiber_angle_deg=fiber_angle_deg,
-            fiber_xoffset=fiber_xoffset,
-            overwrite=overwrite,
-        )
-        for fiber_xoffset in offsets
-    ]
-    sp = dfs[0]
-    transmission = np.abs(sp[f"{fiber_port_name}@0,o1@0"])
-    reflection = np.abs(sp["o1@0,o1@0"])
+    test_sparameters_grating_coupler(overwrite=False)
+    # overwrite = False
+    # c = gf.components.grating_coupler_elliptical_arbitrary(
+    #     widths=[0.343] * 25, gaps=[0.345] * 25
+    # )
+
+    # fiber_angle_deg = 20
+    # offsets = [0, 1]
+    # dfs = [
+    #     gt.write_sparameters_grating_coupler(
+    #         component=c,
+    #         is_3d=False,
+    #         fiber_angle_deg=fiber_angle_deg,
+    #         fiber_xoffset=fiber_xoffset,
+    #         overwrite=overwrite,
+    #     )
+    #     for fiber_xoffset in offsets
+    # ]
+    # sp = dfs[0]
+    # transmission = np.abs(sp[f"{fiber_port_name}@0,o1@0"])
+    # reflection = np.abs(sp["o1@0,o1@0"])
 
-    assert 1 > transmission.max() > 0.2, transmission.max()
-    assert 0.3 > reflection.max() > 0, reflection.max()
+    # assert 1 > transmission.max() > 0.2, transmission.max()
+    # assert 0.3 > reflection.max() > 0, reflection.max()
```

### Comparing `gplugins-0.0.2/gplugins/gtidy3d/utils.py` & `gplugins-0.0.3/gplugins/tidy3d/utils.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.2/gplugins/gtidy3d/write_sparameters.py` & `gplugins-0.0.3/gplugins/tidy3d/write_sparameters.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,20 +20,20 @@
     PathType,
     Port,
     PortSymmetries,
     Sparameters,
     Tuple,
 )
 
-from gplugins import port_symmetries
-from gplugins.get_sparameters_path import (
+from gplugins.tidy3d.get_results import _executor, get_results_batch
+from gplugins.tidy3d.get_simulation import get_simulation, plot_simulation
+from gplugins.utils import port_symmetries
+from gplugins.utils.get_sparameters_path import (
     get_sparameters_path_tidy3d as get_sparameters_path,
 )
-from gplugins.gtidy3d.get_results import _executor, get_results_batch
-from gplugins.gtidy3d.get_simulation import get_simulation, plot_simulation
 
 
 def parse_port_eigenmode_coeff(
     port_name: str, ports: Dict[str, Port], sim_data: td.SimulationData
 ) -> Tuple[np.ndarray]:
     """Given a port and eigenmode coefficient result, returns the coefficients \
     relative to whether the wavevector is entering or exiting simulation.
```

### Comparing `gplugins-0.0.2/gplugins/gtidy3d/write_sparameters_grating_coupler.py` & `gplugins-0.0.3/gplugins/tidy3d/write_sparameters_grating_coupler.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,22 +16,22 @@
     ComponentSpec,
     Dict,
     List,
     PathType,
     Sparameters,
 )
 
-from gplugins.get_sparameters_path import (
-    get_sparameters_path_tidy3d as get_sparameters_path,
-)
-from gplugins.gtidy3d.get_results import _executor, get_results
-from gplugins.gtidy3d.get_simulation import plot_simulation
-from gplugins.gtidy3d.get_simulation_grating_coupler import (
+from gplugins.tidy3d.get_results import _executor, get_results
+from gplugins.tidy3d.get_simulation import plot_simulation
+from gplugins.tidy3d.get_simulation_grating_coupler import (
     get_simulation_grating_coupler,
 )
+from gplugins.utils.get_sparameters_path import (
+    get_sparameters_path_tidy3d as get_sparameters_path,
+)
 
 
 def write_sparameters_grating_coupler(
     component: ComponentSpec,
     dirpath: PathType | None = None,
     filepath: PathType | None = None,
     overwrite: bool = False,
@@ -96,15 +96,16 @@
         material_name_to_tidy3d: dispersive materials have a wavelength dependent index.
             Maps layer_stack names with tidy3d material database names.
         is_3d: True by default runs in 3D.
         with_all_monitors: stores all monitor fields.
 
     """
     component = gf.get_component(component)
-    assert isinstance(component, Component)
+    if not isinstance(component, Component):
+        raise ValueError(f"component should be a gdsfactory.Component not {component}")
 
     filepath = filepath or get_sparameters_path(
         component=component,
         dirpath=dirpath,
         **kwargs,
     )
     filepath = pathlib.Path(filepath).with_suffix(".npz")
@@ -195,31 +196,30 @@
     return [
         _executor.submit(write_sparameters_grating_coupler, **job, **kwargs)
         for job in jobs
     ]
 
 
 if __name__ == "__main__":
-    from gdsfactory.config import PATH
-
     c = gf.components.grating_coupler_elliptical_lumerical()  # inverse design grating
     offsets = [0, 5]
     offsets = [0]
     fiber_angle_deg = 8
+    sp = write_sparameters_grating_coupler(c, is_3d=False)
 
-    dfs = [
-        write_sparameters_grating_coupler(
-            component=c,
-            is_3d=False,
-            fiber_angle_deg=fiber_angle_deg,
-            fiber_xoffset=fiber_xoffset,
-            filepath=PATH.sparameters_repo / f"gc_offset{fiber_xoffset}.npz",
-        )
-        for fiber_xoffset in offsets
-    ]
+    # dfs = [
+    #     write_sparameters_grating_coupler(
+    #         component=c,
+    #         is_3d=False,
+    #         fiber_angle_deg=fiber_angle_deg,
+    #         fiber_xoffset=fiber_xoffset,
+    #         filepath=PATH.sparameters_repo / f"gc_offset{fiber_xoffset}.npz",
+    #     )
+    #     for fiber_xoffset in offsets
+    # ]
 
     # jobs = [
     #     dict(
     #         component=c,
     #         is_3d=False,
     #         fiber_angle_deg=fiber_angle_deg,
     #         fiber_xoffset=fiber_xoffset,
```

### Comparing `gplugins-0.0.2/gplugins/lumerical/__init__.py` & `gplugins-0.0.3/gplugins/lumerical/__init__.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.2/gplugins/lumerical/interconnect.py` & `gplugins-0.0.3/gplugins/lumerical/interconnect.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.2/gplugins/lumerical/read.py` & `gplugins-0.0.3/gplugins/lumerical/read.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import gdsfactory as gf
 import numpy as np
 from gdsfactory.component import Component
 from gdsfactory.config import logger
 from gdsfactory.generic_tech import LAYER_STACK
 from gdsfactory.technology import LayerStack
 
-from gplugins.get_sparameters_path import (
+from gplugins.utils.get_sparameters_path import (
     get_sparameters_path_lumerical as get_sparameters_path,
 )
 
 
 def get_ports(line: str) -> tuple[str, str]:
     """Returns 2 port labels strings from interconnect file."""
     line = line.replace('"', "")
```

### Comparing `gplugins-0.0.2/gplugins/lumerical/settings.py` & `gplugins-0.0.3/gplugins/lumerical/settings.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.2/gplugins/lumerical/write_sparameters_lumerical.py` & `gplugins-0.0.3/gplugins/lumerical/write_sparameters_lumerical.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from gdsfactory.generic_tech.simulation_settings import (
     SIMULATION_SETTINGS_LUMERICAL_FDTD,
     SimulationSettingsLumericalFdtd,
 )
 from gdsfactory.pdk import get_layer_stack
 from gdsfactory.technology import LayerStack
 
-from gplugins.get_sparameters_path import (
+from gplugins.utils.get_sparameters_path import (
     get_sparameters_path_lumerical as get_sparameters_path,
 )
 
 if TYPE_CHECKING:
     from gdsfactory.typings import ComponentSpec, MaterialSpec, PathType
 
 run_false_warning = """
@@ -42,22 +42,22 @@
             a string from lumerical database materials.
             a float or int, representing refractive index.
             a complex for n, k materials.
 
     """
     if isinstance(material, str):
         session.setnamed(structure, "material", material)
-    elif isinstance(material, (int, float)):
+    elif isinstance(material, int | float):
         session.setnamed(structure, "index", material)
     elif isinstance(material, complex):
         mat = session.addmaterial("(n,k) Material")
         session.setmaterial(mat, "Refractive Index", material.real)
         session.setmaterial(mat, "Imaginary Refractive Index", material.imag)
         session.setnamed(structure, "material", mat)
-    elif isinstance(material, (tuple, list)):
+    elif isinstance(material, tuple | list):
         if len(material) != 2:
             raise ValueError(
                 "Complex material requires a tuple or list of two numbers "
                 f"(real, imag). Got {material} "
             )
         real, imag = material
         mat = session.addmaterial("(n,k) Material")
```

### Comparing `gplugins-0.0.2/gplugins/lumerical/write_sparameters_lumerical_components.py` & `gplugins-0.0.3/gplugins/lumerical/write_sparameters_lumerical_components.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.2/gplugins/modes/__init__.py` & `gplugins-0.0.3/gplugins/modes/__init__.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.2/gplugins/modes/coupler.py` & `gplugins-0.0.3/gplugins/modes/coupler.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.2/gplugins/modes/find_coupling_vs_gap.py` & `gplugins-0.0.3/gplugins/modes/find_coupling_vs_gap.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.2/gplugins/modes/find_mode_dispersion.py` & `gplugins-0.0.3/gplugins/modes/find_mode_dispersion.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.2/gplugins/modes/find_modes.py` & `gplugins-0.0.3/gplugins/modes/find_modes.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,29 +6,27 @@
 Since there's no special lengthscale here, you can just
 use microns. In general, if you use units of x, the frequencies
 output are equivalent to x/lambda# so here, the frequencies will be
 output as um/lambda, e.g. 1.5um would correspond to the frequency
 1/1.5 = 0.6667.
 
 """
-from __future__ import annotations
-
 import pickle
 from functools import partial
 
 import meep as mp
 import numpy as np
 from gdsfactory.pdk import get_modes_path
 from meep import mpb
 
-from gplugins.disable_print import disable_print, enable_print
-from gplugins.get_sparameters_path import get_kwargs_hash
 from gplugins.modes.get_mode_solver_coupler import get_mode_solver_coupler
 from gplugins.modes.get_mode_solver_rib import get_mode_solver_rib
 from gplugins.modes.types import Mode
+from gplugins.utils.disable_print import disable_print, enable_print
+from gplugins.utils.get_sparameters_path import get_kwargs_hash
 
 mpb.Verbosity(0)
 
 
 def find_modes_waveguide(
     tol: float = 1e-6,
     wavelength: float = 1.55,
```

### Comparing `gplugins-0.0.2/gplugins/modes/find_modes_cross_section.py` & `gplugins-0.0.3/gplugins/modes/find_modes_cross_section.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,20 +16,20 @@
 
 import meep as mp
 import numpy as np
 from gdsfactory.pdk import get_modes_path
 from gdsfactory.typings import CrossSectionSpec
 from meep import mpb
 
-from gplugins.disable_print import disable_print, enable_print
-from gplugins.get_sparameters_path import get_kwargs_hash
 from gplugins.modes.get_mode_solver_cross_section import (
     get_mode_solver_cross_section,
 )
 from gplugins.modes.types import Mode
+from gplugins.utils.disable_print import disable_print, enable_print
+from gplugins.utils.get_sparameters_path import get_kwargs_hash
 
 mpb.Verbosity(0)
 
 
 def find_modes_cross_section(
     cross_section: CrossSectionSpec,
     tol: float = 1e-6,
```

### Comparing `gplugins-0.0.2/gplugins/modes/find_neff_ng_dw_dh.py` & `gplugins-0.0.3/gplugins/modes/find_neff_ng_dw_dh.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.2/gplugins/modes/find_neff_vs_width.py` & `gplugins-0.0.3/gplugins/modes/find_neff_vs_width.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.2/gplugins/modes/get_mode_solver_coupler.py` & `gplugins-0.0.3/gplugins/modes/get_mode_solver_coupler.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.2/gplugins/modes/get_mode_solver_cross_section.py` & `gplugins-0.0.3/gplugins/modes/get_mode_solver_cross_section.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.2/gplugins/modes/get_mode_solver_rib.py` & `gplugins-0.0.3/gplugins/modes/get_mode_solver_rib.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.2/gplugins/modes/modes/neff_vs_width_nitride.csv` & `gplugins-0.0.3/gplugins/modes/modes/neff_vs_width_nitride.csv`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.2/gplugins/modes/modes/neff_vs_width_rib.csv` & `gplugins-0.0.3/gplugins/modes/modes/neff_vs_width_rib.csv`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.2/gplugins/modes/modes/neff_vs_width_strip.csv` & `gplugins-0.0.3/gplugins/modes/modes/neff_vs_width_strip.csv`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.2/gplugins/modes/neff_convergence_test.py` & `gplugins-0.0.3/gplugins/modes/neff_convergence_test.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.2/gplugins/modes/overlap.py` & `gplugins-0.0.3/gplugins/modes/overlap.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.2/gplugins/modes/tests/test_dw_dh/test_dw_dh_dispersion.csv` & `gplugins-0.0.3/gplugins/modes/tests/test_dw_dh/test_dw_dh_dispersion.csv`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.2/gplugins/modes/tests/test_find_modes.py` & `gplugins-0.0.3/gplugins/modes/tests/test_find_modes.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.2/gplugins/modes/tests/test_find_modes_dispersion.py` & `gplugins-0.0.3/gplugins/modes/tests/test_find_modes_dispersion.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.2/gplugins/modes/types.py` & `gplugins-0.0.3/gplugins/modes/types.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.2/gplugins/modes/waveguide.py` & `gplugins-0.0.3/gplugins/modes/waveguide.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.2/gplugins/photonic_circuit_models/__init__.py` & `gplugins-0.0.3/gplugins/photonic_circuit_models/__init__.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.2/gplugins/photonic_circuit_models/coupler.py` & `gplugins-0.0.3/gplugins/photonic_circuit_models/coupler.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.2/gplugins/photonic_circuit_models/mzi.py` & `gplugins-0.0.3/gplugins/photonic_circuit_models/mzi.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     )
     return np.abs(E_out) ** 2
 
 
 if __name__ == "__main__":
     import matplotlib.pyplot as plt
 
-    import gplugins.gtidy3d as gt
+    import gplugins.tidy3d as gt
 
     nm = 1e-3
     strip = gt.modes.Waveguide(
         wavelength=1.55,
         core_width=500 * nm,
         core_thickness=220 * nm,
         slab_thickness=0.0,
```

### Comparing `gplugins-0.0.2/gplugins/photonic_circuit_models/ring.py` & `gplugins-0.0.3/gplugins/photonic_circuit_models/ring.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.2/gplugins/plot.py` & `gplugins-0.0.3/gplugins/utils/plot.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.2/gplugins/plot_csv.py` & `gplugins-0.0.3/gplugins/utils/plot_csv.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.2/gplugins/port_symmetries.py` & `gplugins-0.0.3/gplugins/utils/port_symmetries.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.2/gplugins/process/diffusion.py` & `gplugins-0.0.3/gplugins/process/diffusion.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.2/gplugins/process/implant_tables.py` & `gplugins-0.0.3/gplugins/process/implant_tables.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.2/gplugins/process/pysrim.py` & `gplugins-0.0.3/gplugins/process/pysrim.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.2/gplugins/process/silicon.py` & `gplugins-0.0.3/gplugins/process/silicon.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.2/gplugins/process/skew/antimony_si_skew.csv` & `gplugins-0.0.3/gplugins/process/skew/antimony_si_skew.csv`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.2/gplugins/process/skew/arsenic_si_skew.csv` & `gplugins-0.0.3/gplugins/process/skew/arsenic_si_skew.csv`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.2/gplugins/process/skew/boron_si_skew.csv` & `gplugins-0.0.3/gplugins/process/skew/boron_si_skew.csv`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.2/gplugins/process/skew/phosphorus_si_skew.csv` & `gplugins-0.0.3/gplugins/process/skew/phosphorus_si_skew.csv`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.2/gplugins/sax/build_model.py` & `gplugins-0.0.3/gplugins/sax/build_model.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.2/gplugins/sax/femwell_waveguide_model.py` & `gplugins-0.0.3/gplugins/sax/integrations/femwell_waveguide_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import jax.numpy as jnp
 import numpy as np
 import ray
 from gdsfactory.pdk import get_layer_stack
 from sax.utils import reciprocal
 
-from gplugins.fem.mode_solver import compute_cross_section_modes
+from gplugins.femwell.mode_solver import compute_cross_section_modes
 from gplugins.sax.build_model import Model
 
 
 @ray.remote(num_cpus=1)
 def remote_output_from_inputs(
     cross_section,
     layerstack,
```

### Comparing `gplugins-0.0.2/gplugins/sax/interpolators.py` & `gplugins-0.0.3/gplugins/sax/interpolators.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.2/gplugins/sax/meep_FDTD_model.py` & `gplugins-0.0.3/gplugins/sax/integrations/meep_FDTD_model.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.2/gplugins/sax/meow_eme_model.py` & `gplugins-0.0.3/gplugins/sax/integrations/meow_eme_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from gdsfactory.pdk import get_layer_stack
 
-from gplugins.eme.meow_eme import MEOW
+from gplugins.meow.meow_eme import MEOW
 from gplugins.sax.build_model import Model
 
 
 class MeowEMEModel(Model):
     def __init__(self, **kwargs) -> None:
         """Generic model inferred from MEOW EME calculations."""
         super().__init__(**kwargs)
```

### Comparing `gplugins-0.0.2/gplugins/sax/mlp.py` & `gplugins-0.0.3/gplugins/sax/mlp.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.2/gplugins/sax/models.py` & `gplugins-0.0.3/gplugins/sax/models.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.2/gplugins/sax/parameter.py` & `gplugins-0.0.3/gplugins/sax/parameter.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.2/gplugins/sax/plot_model.py` & `gplugins-0.0.3/gplugins/sax/plot_model.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.2/gplugins/sax/read.py` & `gplugins-0.0.3/gplugins/sax/read.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,53 +1,51 @@
 """read Sparameters from CSV file and returns sax model."""
 from __future__ import annotations
 
 import pathlib
 from functools import partial
-from typing import Literal, Union
+from typing import Literal
 
 import gdsfactory as gf
 import jax
 import jax.numpy as jnp
 import numpy as np
 import pandas as pd
 from sax.typing_ import Float, Model
 
-from gplugins.get_sparameters_path import (
+from gplugins.utils.get_sparameters_path import (
     get_sparameters_path_lumerical,
     get_sparameters_path_meep,
     get_sparameters_path_tidy3d,
 )
 
 wl_cband = np.linspace(1.500, 1.600, 128)
 
-PathType = Union[str, pathlib.Path]
+PathType = str | pathlib.Path
 
 Simulator = Literal["lumerical", "meep", "tidy3d"]
 
 
 def model_from_npz(
     filepath: PathType | np.ndarray,
     xkey: str = "wavelengths",
     xunits: float = 1,
-    prefix: str = "s",
 ) -> Model:
     """Returns a SAX Sparameters Model from a npz file.
 
     The SAX Model is a function that returns a SAX SDict interpolated over wavelength.
 
     Args:
         filepath: CSV Sparameters path or pandas DataFrame.
         wl: wavelength to interpolate (um).
         xkey: key for wavelengths in file.
         xunits: x units in um from the loaded file (um). 1 means 1um.
-        prefix: for the sparameters column names in file.
 
     """
-    sp = np.load(filepath) if isinstance(filepath, (pathlib.Path, str)) else filepath
+    sp = np.load(filepath) if isinstance(filepath, pathlib.Path | str) else filepath
     keys = list(sp.keys())
 
     if xkey not in keys:
         raise ValueError(f"{xkey!r} not in {keys}")
 
     x = jnp.asarray(sp[xkey] * xunits)
     wl = jnp.asarray(wl_cband)
@@ -61,16 +59,16 @@
     def model(wl: Float = wl):
         S = {}
         zero = jnp.zeros_like(x)
 
         for key in sp:
             if not key.startswith("wav"):
                 port_mode0, port_mode1 = key.split(",")
-                port0, mode0 = port_mode0.split("@")
-                port1, mode1 = port_mode1.split("@")
+                port0, _ = port_mode0.split("@")
+                port1, _ = port_mode1.split("@")
                 S[(port0, port1)] = jnp.interp(wl, x, sp.get(key, zero))
 
         return S
 
     return model
```

### Comparing `gplugins-0.0.2/gplugins/sax/tests/test_mzi.py` & `gplugins-0.0.3/gplugins/sax/tests/test_mzi.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.2/gplugins/sax/tests/test_mzi_lattice.py` & `gplugins-0.0.3/gplugins/sax/tests/test_mzi_lattice.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.2/gplugins/sax/tests/test_parameters.py` & `gplugins-0.0.3/gplugins/sax/tests/test_parameters.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.2/gplugins/schematic_editor/circuitviz.py` & `gplugins-0.0.3/gplugins/schematic_editor/circuitviz.py`

 * *Files 0% similar despite different names*

```diff
@@ -151,15 +151,15 @@
     fig=None,
     **kwargs,
 ):
     global data
     if fig is None:
         fig = bp.figure()
 
-    if isinstance(netlist, (PicYamlConfiguration, SchematicConfiguration)):
+    if isinstance(netlist, PicYamlConfiguration | SchematicConfiguration):
         objs = viz_netlist(netlist, instances, **kwargs)
     else:
         objs = netlist
         netlist = None
 
     if not isinstance(objs, list):
         raise ValueError("viz_bk can only visualize a list of objects.")
```

### Comparing `gplugins-0.0.2/gplugins/schematic_editor/schematic_editor.py` & `gplugins-0.0.3/gplugins/schematic_editor/schematic_editor.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.2/gplugins/web/gds_files/coh_rx_dual_pol.gds` & `gplugins-0.0.3/gplugins/web/gds_files/coh_rx_dual_pol.gds`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.2/gplugins/web/gds_files/coh_rx_single_pol.gds` & `gplugins-0.0.3/gplugins/web/gds_files/coh_rx_single_pol.gds`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.2/gplugins/web/gds_files/coh_rx_single_pol_pad_d_19b6c499.gds` & `gplugins-0.0.3/gplugins/web/gds_files/coh_rx_single_pol_pad_d_19b6c499.gds`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.2/gplugins/web/gds_files/coh_rx_single_pol_pad_d_d4526895.gds` & `gplugins-0.0.3/gplugins/web/gds_files/coh_rx_single_pol_pad_d_d4526895.gds`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.2/gplugins/web/gds_files/coh_tx_dual_pol.gds` & `gplugins-0.0.3/gplugins/web/gds_files/coh_tx_dual_pol.gds`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.2/gplugins/web/gds_files/crossing_arm.gds` & `gplugins-0.0.3/gplugins/web/gds_files/crossing_arm.gds`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.2/gplugins/web/gds_files/dbr_cavity.gds` & `gplugins-0.0.3/gplugins/web/gds_files/dbr_cavity.gds`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.2/gplugins/web/gds_files/loss_deembedding_ch14_23.gds` & `gplugins-0.0.3/gplugins/web/gds_files/loss_deembedding_ch14_23.gds`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.2/gplugins/web/gds_files/pad_array_add_fiducials.gds` & `gplugins-0.0.3/gplugins/web/gds_files/pad_array_add_fiducials.gds`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.2/gplugins/web/gds_files/spiral_inner_io_add_gra_f2760628.gds` & `gplugins-0.0.3/gplugins/web/gds_files/spiral_inner_io_add_gra_f2760628.gds`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.2/gplugins/web/main.py` & `gplugins-0.0.3/gplugins/web/main.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.2/gplugins/web/middleware.py` & `gplugins-0.0.3/gplugins/web/middleware.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.2/gplugins/web/server.py` & `gplugins-0.0.3/gplugins/web/server.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.2/gplugins/web/server_jupyter.py` & `gplugins-0.0.3/gplugins/web/server_jupyter.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.2/gplugins/web/static/client.css` & `gplugins-0.0.3/gplugins/web/static/client.css`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.2/gplugins/web/static/client.js` & `gplugins-0.0.3/gplugins/web/static/client.js`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.2/gplugins/web/templates/client.html.j2` & `gplugins-0.0.3/gplugins/web/templates/client.html.j2`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.2/gplugins/web/templates/filewatcher.html.j2` & `gplugins-0.0.3/gplugins/web/templates/filewatcher.html.j2`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.2/gplugins/web/templates/header.html.j2` & `gplugins-0.0.3/gplugins/web/templates/header.html.j2`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.2/gplugins/web/templates/navbar.html.j2` & `gplugins-0.0.3/gplugins/web/templates/navbar.html.j2`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.2/gplugins/web/templates/viewer.html.j2` & `gplugins-0.0.3/gplugins/web/templates/viewer.html.j2`

 * *Files identical despite different names*

### Comparing `gplugins-0.0.2/gplugins/widget/interactive.py` & `gplugins-0.0.3/gplugins/widget/interactive.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     )
     from kfactory import kdb, lay
     from kfactory.kcell import KCell
 
 
 except ImportError as e:
     print(
-        "You need install jupyter notebook plugin with `pip install gdsfactory[kfactory]`"
+        "You need install jupyter notebook plugin with `pip install gplugins[kfactory]`"
     )
     raise e
 
 
 def display_kcell(kc: KCell) -> None:
     cell_dup = kc.kcl.dup()[kc.name]
     cell_dup.draw_ports()
```

### Comparing `gplugins-0.0.2/pyproject.toml` & `gplugins-0.0.3/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,108 +1,105 @@
 # https://setuptools.pypa.io/en/latest/userguide/pyproject_config.html
+
 [build-system]
-requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
+requires = ["flit_core >=3.2,<4"]
 
 [project]
-name="gplugins"
-description="gdsfactory plugins"
+authors = [
+  {name = "gdsfactory", email = "contact@gdsfactory.com"}
+]
 classifiers = [
-	"Programming Language :: Python :: 3.10",
-	"Programming Language :: Python :: 3.11",
-	"Operating System :: OS Independent",
+  "Programming Language :: Python :: 3.10",
+  "Programming Language :: Python :: 3.11",
+  "Operating System :: OS Independent"
 ]
-version="0.0.2"
-authors = [
-    {name = "gdsfactory", email = "contact@gdsfactory.com"},
+dependencies = [
+  "gdsfactory[cad]>=7.0.2"
 ]
+description = "gdsfactory plugins"
 keywords = ["python"]
 license = {file = "LICENSE"}
-dependencies = [
-    "gdsfactory[cad]",
-]
+name = "gplugins"
 readme = "README.md"
 requires-python = ">=3.10"
+version = "0.0.3"
 
 [project.optional-dependencies]
-dev = [
-    "pre-commit",
-    "pytest",
-    "pytest-cov",
-    "pytest_regressions",
-    "jsondiff",
-    "mypy",
-    ]
-docs = [
-    "jupytext",
-    "autodoc_pydantic",
-    "matplotlib",
-    "jupyter-book==0.15.1",
-    "sphinx-autodoc-typehints",
-    "sphinx-click",
-    ]
 database = [
   "sqlalchemy",
   "sqlalchemy-utils",
   "dagster",
   "dagit",
   "sqlmodel",
   "boto3",
   "pymysql"
 ]
+dev = [
+  "pre-commit",
+  "pytest",
+  "pytest-cov",
+  "pytest_regressions",
+  "jsondiff",
+  "mypy",
+  "pyswarms",
+  "autograd",
+  "ray[tune,air]",
+  "hyperopt"
+]
 devsim = [
   "devsim",
   "pyvista",
   "tidy3d"
 ]
+docs = [
+  "jupytext",
+  "autodoc_pydantic",
+  "matplotlib",
+  "jupyter-book==0.15.1"
+]
 femwell = [
-  "femwell==0.1.5"
+  "femwell==0.1.6"
 ]
 gmsh = [
   "gmsh",
   "h5py",
   "mapbox_earcut",
   "meshio",
   "pygmsh",
   "pyvista",
   "trimesh",
-  "shapely"
-]
-kfactory = [
-  "kfactory[git,ipy]==0.7.5"
-]
-meow = [
-  "meow-sim==0.7.1"
-]
-meshwell = [
+  "shapely",
   "meshwell==0.0.9"
 ]
-ray = [
-  "ray[tune,air]",
-  "hyperopt"
+meow = [
+  "meow-sim==0.7.1",
+  "tidy3d==2.3.3"
 ]
 sax = [
   "sax==0.8.8",
   "jaxlib",
-  "jax"
+  "jax",
+  "scikit-learn"
+]
+schematic = [
+  'bokeh',
+  "natsort"
 ]
 tidy3d = [
   "tidy3d==2.3.3"
 ]
-
-[tool.setuptools.packages]
-find = {}
-
-# [project.scripts]
-# gplugins = "gplugins.cli:cli"
+web = [
+  "jinja2",
+  "python-multipart",
+  "fastapi",
+  "uvicorn[standard]"
+]
 
 [tool.black]
-line-length = 88
-target-version = ['py310']
-include = '\.pyi?$'
 exclude = '''  # Specify the files/dirs that should be ignored by the black formatter
 /(
     \.eggs
   | \.git
   | \.hg
   | \.mypy_cache
   | \.tox
@@ -110,97 +107,65 @@
   | env
   | _build
   | buck-out
   | build
   | dist
 )/
 '''
+include = '\.pyi?$'
+line-length = 88
+target-version = ['py310']
 
-[tool.pytest.ini_options]
-testpaths = ["gplugins/", "tests"]
-addopts = '--tb=short'
-python_files = ["gplugins/*.py", "notebooks/*.ipynb", "tests/*.py"]
-norecursedirs = [
-    "extra/*.py",
-    'gplugins/devsim',
-    ]
-
-[tool.flake8]
-max-line-length = 88
-max-complexity = 57
-select = ["B","C","E","F","W","T4","B9"]
-ignore = [ "E501", "E503", "E722", "W503", "W503", "E203", "B950", "B305", "B018", "B902", "B020", "B905"]
-extend-ignore = "RST303"
-
-exclude = [
-    ".git",
-    "__pycache__",
-    "lib",
-    "docs/source/conf.py",
-    "build",
-    "dist",
-    ".ipynb_checkpoints",
-    ".tox",
-    "extra",
-    "deprecated",
-    ".mypy_cache",
-    "venv",
-    "devsim"
-    ]
-
-[tool.commitizen]
-name = "cz_conventional_commits"
-version = "0.1.0"
-version_files = [
-    "pyproject.toml:version",
-]
+[tool.codespell]
+ignore-words-list = "te, te/tm, te, ba, fpr, fpr_spacing, ro, nd, donot, schem"
 
 [tool.mypy]
 python_version = "3.10"
 strict = true
 
 [tool.pylsp-mypy]
 enabled = true
 live_mode = true
 strict = true
 
-[tool.isort]
-multi_line_output = 3
-line_length = 88
-include_trailing_comma = true
-# skip = "gplugins/__init__.py"
-
-[tool.setuptools.package-data]
-mypkg = ["*.csv", "*.yaml"]
-
-[tool.codespell]
-ignore-words-list = "te, te/tm, te, ba, fpr, fpr_spacing, ro, nd, donot, schem"
-
-[tool.pydocstyle]
-inherit = false
-match = "(?!test).*\\.py"
-add-ignore = ["D100","D101","D102","D103","D104","D203","D405","D417"]
-convention = "google"
+[tool.pytest.ini_options]
+addopts = '--tb=short'
+norecursedirs = [
+  "extra/*.py",
+  'gplugins/devsim',
+  'gplugins/sax/integrations',
+  'gplugins/tidy3d/tests/tests_sparameters'
+]
+python_files = ["gplugins/*.py", "notebooks/*.ipynb", "tests/*.py"]
+testpaths = ["gplugins/", "tests"]
 
 [tool.ruff]
-select = [
-    "E",  # pycodestyle errors
-    "W",  # pycodestyle warnings
-    "F",  # pyflakes
-    "I",  # isort
-    "C",  # flake8-comprehensions
-    "B",  # flake8-bugbear
-]
+fix = true
 ignore = [
-    "E501",  # line too long, handled by black
-    "B008",  # do not perform function calls in argument defaults
-    "C901",  # too complex
-    "B905",  # `zip()` without an explicit `strict=` parameter
-    "C408",  # C408 Unnecessary `dict` call (rewrite as a literal)
-    "E402",  # module level import not at top of file
-    "B018",  # found useless expression
-    "B028"   # no explicit stacklevel
+  "E501",  # line too long, handled by black
+  "B008",  # do not perform function calls in argument defaults
+  "C901",  # too complex
+  "B905",  # `zip()` without an explicit `strict=` parameter
+  "C408",  # C408 Unnecessary `dict` call (rewrite as a literal)
+  "E402",  # module level import not at top of file
+  "B018",  # found useless expression
+  "B028"  # no explicit stacklevel
+]
+select = [
+  "E",  # pycodestyle errors
+  "W",  # pycodestyle warnings
+  "F",  # pyflakes
+  "I",  # isort
+  "C",  # flake8-comprehensions
+  "B",  # flake8-bugbear
+  "UP"
 ]
 
 [tool.ruff.per-file-ignores]
 "docs/notebooks/meep_01_sparameters.py" = ["F821", 'E402']
-"docs/notebooks/tcad_02_analytical_process.py" = ["F821", 'E402', 'F405','F403']
+"docs/notebooks/tcad_02_analytical_process.py" = ["F821", 'E402', 'F405', 'F403']
+
+[tool.setuptools.package-data]
+mypkg = ["*.csv", "*.yaml"]
+
+[tool.setuptools.packages]
+find = {}
```

### Comparing `gplugins-0.0.2/PKG-INFO` & `gplugins-0.0.3/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,122 +1,116 @@
 Metadata-Version: 2.1
 Name: gplugins
-Version: 0.0.2
+Version: 0.0.3
 Summary: gdsfactory plugins
 Keywords: python
 Author-email: gdsfactory <contact@gdsfactory.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
-Requires-Dist: gdsfactory[cad]
+Requires-Dist: gdsfactory[cad]>=7.0.2
 Requires-Dist: sqlalchemy ; extra == "database"
 Requires-Dist: sqlalchemy-utils ; extra == "database"
 Requires-Dist: dagster ; extra == "database"
 Requires-Dist: dagit ; extra == "database"
 Requires-Dist: sqlmodel ; extra == "database"
 Requires-Dist: boto3 ; extra == "database"
 Requires-Dist: pymysql ; extra == "database"
 Requires-Dist: pre-commit ; extra == "dev"
 Requires-Dist: pytest ; extra == "dev"
 Requires-Dist: pytest-cov ; extra == "dev"
 Requires-Dist: pytest_regressions ; extra == "dev"
 Requires-Dist: jsondiff ; extra == "dev"
 Requires-Dist: mypy ; extra == "dev"
+Requires-Dist: pyswarms ; extra == "dev"
+Requires-Dist: autograd ; extra == "dev"
+Requires-Dist: ray[tune,air] ; extra == "dev"
+Requires-Dist: hyperopt ; extra == "dev"
 Requires-Dist: devsim ; extra == "devsim"
 Requires-Dist: pyvista ; extra == "devsim"
 Requires-Dist: tidy3d ; extra == "devsim"
 Requires-Dist: jupytext ; extra == "docs"
 Requires-Dist: autodoc_pydantic ; extra == "docs"
 Requires-Dist: matplotlib ; extra == "docs"
 Requires-Dist: jupyter-book==0.15.1 ; extra == "docs"
-Requires-Dist: sphinx-autodoc-typehints ; extra == "docs"
-Requires-Dist: sphinx-click ; extra == "docs"
-Requires-Dist: femwell==0.1.5 ; extra == "femwell"
+Requires-Dist: femwell==0.1.6 ; extra == "femwell"
 Requires-Dist: gmsh ; extra == "gmsh"
 Requires-Dist: h5py ; extra == "gmsh"
 Requires-Dist: mapbox_earcut ; extra == "gmsh"
 Requires-Dist: meshio ; extra == "gmsh"
 Requires-Dist: pygmsh ; extra == "gmsh"
 Requires-Dist: pyvista ; extra == "gmsh"
 Requires-Dist: trimesh ; extra == "gmsh"
 Requires-Dist: shapely ; extra == "gmsh"
-Requires-Dist: kfactory[git,ipy]==0.7.5 ; extra == "kfactory"
+Requires-Dist: meshwell==0.0.9 ; extra == "gmsh"
 Requires-Dist: meow-sim==0.7.1 ; extra == "meow"
-Requires-Dist: meshwell==0.0.9 ; extra == "meshwell"
-Requires-Dist: ray[tune,air] ; extra == "ray"
-Requires-Dist: hyperopt ; extra == "ray"
+Requires-Dist: tidy3d==2.3.3 ; extra == "meow"
 Requires-Dist: sax==0.8.8 ; extra == "sax"
 Requires-Dist: jaxlib ; extra == "sax"
 Requires-Dist: jax ; extra == "sax"
+Requires-Dist: scikit-learn ; extra == "sax"
+Requires-Dist: bokeh ; extra == "schematic"
+Requires-Dist: natsort ; extra == "schematic"
 Requires-Dist: tidy3d==2.3.3 ; extra == "tidy3d"
+Requires-Dist: jinja2 ; extra == "web"
+Requires-Dist: python-multipart ; extra == "web"
+Requires-Dist: fastapi ; extra == "web"
+Requires-Dist: uvicorn[standard] ; extra == "web"
 Provides-Extra: database
 Provides-Extra: dev
 Provides-Extra: devsim
 Provides-Extra: docs
 Provides-Extra: femwell
 Provides-Extra: gmsh
-Provides-Extra: kfactory
 Provides-Extra: meow
-Provides-Extra: meshwell
-Provides-Extra: ray
 Provides-Extra: sax
+Provides-Extra: schematic
 Provides-Extra: tidy3d
+Provides-Extra: web
 
-# gplugins 0.0.2 gdsfactory plugins
+# gplugins 0.0.3
 
-* [Optimization](https://gdsfactory.github.io/gplugins/plugins_optimization.html)
-  - [Ray Tune Generic Black-Box Optimiser](https://gdsfactory.github.io/gplugins/notebooks/ray/optimiser.html)
+[![docs](https://github.com/gdsfactory/gplugins/actions/workflows/pages.yml/badge.svg)](https://gdsfactory.github.io/gplugins/)
+[![PyPI](https://img.shields.io/pypi/v/gplugins)](https://pypi.org/project/gplugins/)
+[![PyPI Python](https://img.shields.io/pypi/pyversions/gplugins.svg)](https://pypi.python.org/pypi/gplugins)
+[![MIT](https://img.shields.io/github/license/gdsfactory/gplugins)](https://choosealicense.com/licenses/mit/)
+[![codecov](https://img.shields.io/codecov/c/github/gdsfactory/gplugins)](https://codecov.io/gh/gdsfactory/gdsfactory/tree/main/gplugins)
 
-* [Meshing](https://gdsfactory.github.io/gplugins/notebooks/devsim/01_pin_waveguide.html#Meshing)
-
-* [Device Simulators](https://gdsfactory.github.io/gplugins/plugins_process.html)
-  - [Thermal Simulation](https://gdsfactory.github.io/gplugins/notebooks/thermal/thermal.html)
-  - [DEVSIM TCAD Simulation](https://gdsfactory.github.io/gplugins/notebooks/devsim/01_pin_waveguide.html)
-  - [Analytical Process Simulation](https://gdsfactory.github.io/gplugins/notebooks/tcad/02_analytical_process.html)
-  - [Montecarlo Implant Simulation](https://gdsfactory.github.io/gplugins/notebooks/tcad/03_numerical_implantation.html)
-
-* [Mode Solvers & Eigenmode Expansion (EME)](https://gdsfactory.github.io/gplugins/plugins_mode_solver.html)
-  - Finite Element Mode Solvers
-    - [Femwell](https://gdsfactory.github.io/gplugins/notebooks/fem/01_mode_solving.html)
-  - Finite Difference Mode Solvers
-    - [tidy3d](https://gdsfactory.github.io/gplugins/notebooks/tidy3d/01_tidy3d_modes.html)
-    - [MPB](https://gdsfactory.github.io/gplugins/notebooks/mpb/001_mpb_waveguide.html)
-  - Eigenmode Expansion (EME)
-    - [MEOW](https://gdsfactory.github.io/gplugins/notebooks/eme/01_meow.html)
-
-* [Electromagnetic Wave Solvers using Finite Difference Time Domain (FDTD)](https://gdsfactory.github.io/gplugins/plugins_fdtd.html)
-  - [tidy3d](https://gdsfactory.github.io/gplugins/notebooks/tidy3d/00_tidy3d.html)
-  - [MEEP](https://gdsfactory.github.io/gplugins/notebooks/meep/001_meep_sparameters.html)
-  - [Ansys Lumerical FDTD](https://gdsfactory.github.io/gplugins/notebooks/lumerical/1_fdtd_sparameters.html)
-
-* [S-Parameter Circuit Solvers](https://gdsfactory.github.io/gplugins/plugins_circuits.html)
-  - [SAX](https://gdsfactory.github.io/gplugins/notebooks/sax/sax.html)
-  - [Ansys Lumerical INTERCONNECT](https://gdsfactory.github.io/gplugins/notebooks/lumerical/2_interconnect.html)
-
-* [Database](https://gdsfactory.github.io/gplugins/notebooks/12_database.html)
+gdsfactory plugins:
 
+- `database` for simulation and measurement database and dagster for data pipelines.
+- `devsim` TCAD device simulator.
+- `meow` Eigen Mode Expansion (EME).
+- `femwell` Finite Element Method Solver (heaters, modes, TCAD, RF waveguides).
+- `gmsh` mesh structures.
+- `tidy3d` Finite Difference Time Domain (FDTD) simulations on the cloud using GPU.
+- `lumerical` For Ansys FDTD and Circuit interconnect.
+- `kfactory` for fill, dataprep and testing.
+- `ray` for distributed computing and optimization.
+- `sax` S-parameter circuit solver.
+- `schematic`: for bokeh schematic editor and `path_length_analysis`
+- `meep` for FDTD.
+- `mpb` for MPB mode solver.
+- `web`: for gdsfactory webapp
 
 ## Installation
 
 You can install all plugins with:
 
 ```
-pip install "gplugins[database,devsim,femwell,gmsh,kfactory,meow,meshwell,ray,sax,tidy3d]" --upgrade
+pip install "gplugins[database,devsim,femwell,gmsh,schematic,meow,meshwell,ray,sax,tidy3d]" --upgrade
 ```
 
-Or Install only the plugins you need `pip install gplugins[plugin1,plugin2]` from the available plugins:
+Or Install only the plugins you need `pip install gplugins[database,devsim]` from the available plugins:
 
-- `database` for simulation and measurement database.
-- `devsim` TCAD device simulator.
-- `femwell` Finite Element Method Solver (heaters, modes, TCAD, RF waveguides).
-- `gmsh` mesh structures.
-- `kfactory` for fill, dataprep and testing.
-- `meow` Eigen Mode Expansion (EME).
-- `ray` for distributed computing and optimization.
-- `sax` S-parameter circuit solver.
-- `tidy3d` Finite Difference Time Domain (FDTD) simulations on the cloud using GPU.
+Separate installation (not using pip):
+
+- For Meep and MPB you need to use `conda` or `mamba` on MacOS, Linux or [Windows WSL (Windows Subsystem for Linux)](https://learn.microsoft.com/en-us/windows/wsl/install) with `conda install pymeep=*=mpi_mpich_* -c conda-forge -y`
+
+## Getting started
 
-To install open source FDTD Meep you need to use `conda` or `mamba` on MacOS or Linux, so for Windows you need to use the [WSL (Windows Subsystem for Linux)](https://learn.microsoft.com/en-us/windows/wsl/install).
-- `conda install pymeep=*=mpi_mpich_* -c conda-forge -y`
+- [Read docs](https://gdsfactory.github.io/gplugins/)
+- [Read gdsfactory docs](https://gdsfactory.github.io/gdsfactory/)
+- [![Join the chat at https://gitter.im/gdsfactory-dev/community](https://badges.gitter.im/gdsfactory-dev/community.svg)](https://gitter.im/gdsfactory-dev/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)
```

