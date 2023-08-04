# Comparing `tmp/qoqo-1.6.0a1.tar.gz` & `tmp/qoqo-1.6.0a2.tar.gz`

## Comparing `qoqo-1.6.0a1.tar` & `qoqo-1.6.0a2.tar`

### file list

```diff
@@ -1,82 +1,82 @@
--rw-r--r--   0        0        0      610 1970-01-01 00:00:00.000000 qoqo-1.6.0a1/local_dependencies/roqoqo-derive/Cargo.toml
--rw-r--r--   0     1001      123    11363 2023-07-20 11:47:24.000000 qoqo-1.6.0a1/local_dependencies/roqoqo-derive/LICENSE
--rw-r--r--   0     1001      123     5566 2023-07-20 11:47:24.000000 qoqo-1.6.0a1/local_dependencies/roqoqo-derive/src/involve_modes.rs
--rw-r--r--   0     1001      123     9027 2023-07-20 11:47:24.000000 qoqo-1.6.0a1/local_dependencies/roqoqo-derive/src/involve_qubits.rs
--rw-r--r--   0     1001      123    13554 2023-07-20 11:47:24.000000 qoqo-1.6.0a1/local_dependencies/roqoqo-derive/src/lib.rs
--rw-r--r--   0     1001      123    10486 2023-07-20 11:47:24.000000 qoqo-1.6.0a1/local_dependencies/roqoqo-derive/src/operate.rs
--rw-r--r--   0     1001      123     7015 2023-07-20 11:47:24.000000 qoqo-1.6.0a1/local_dependencies/roqoqo-derive/src/operate_n_mode.rs
--rw-r--r--   0     1001      123    13664 2023-07-20 11:47:24.000000 qoqo-1.6.0a1/local_dependencies/roqoqo-derive/src/operate_n_qubit.rs
--rw-r--r--   0     1001      123    17807 2023-07-20 11:47:24.000000 qoqo-1.6.0a1/local_dependencies/roqoqo-derive/src/operate_unitary.rs
--rw-r--r--   0     1001      123     3126 2023-07-20 11:47:24.000000 qoqo-1.6.0a1/local_dependencies/roqoqo-derive/src/operate_unitary_modes.rs
--rw-r--r--   0     1001      123     5488 2023-07-20 11:47:24.000000 qoqo-1.6.0a1/local_dependencies/roqoqo-derive/src/substitute.rs
--rw-r--r--   0     1001      123     3286 2023-07-20 11:47:24.000000 qoqo-1.6.0a1/local_dependencies/roqoqo-derive/src/substitute_modes.rs
--rw-r--r--   0     1001      123     2452 2023-07-20 11:47:24.000000 qoqo-1.6.0a1/local_dependencies/roqoqo-derive/src/supported_version.rs
--rw-r--r--   0        0        0     1977 1970-01-01 00:00:00.000000 qoqo-1.6.0a1/local_dependencies/roqoqo/Cargo.toml
--rw-r--r--   0     1001      123    11363 2023-07-20 11:47:24.000000 qoqo-1.6.0a1/local_dependencies/roqoqo/LICENSE
--rw-r--r--   0     1001      123     3068 2023-07-20 11:47:24.000000 qoqo-1.6.0a1/local_dependencies/roqoqo/README.md
--rw-r--r--   0     1001      123    36500 2023-07-20 11:47:24.000000 qoqo-1.6.0a1/local_dependencies/roqoqo/build.rs
--rw-r--r--   0     1001      123    14193 2023-07-20 11:47:24.000000 qoqo-1.6.0a1/local_dependencies/roqoqo/src/backends.rs
--rw-r--r--   0     1001      123    29978 2023-07-20 11:47:24.000000 qoqo-1.6.0a1/local_dependencies/roqoqo/src/circuit.rs
--rw-r--r--   0     1001      123    47768 2023-07-20 11:47:24.000000 qoqo-1.6.0a1/local_dependencies/roqoqo/src/circuitdag.rs
--rw-r--r--   0     1001      123    17909 2023-07-20 11:47:24.000000 qoqo-1.6.0a1/local_dependencies/roqoqo/src/devices/all_to_all.rs
--rw-r--r--   0     1001      123    18928 2023-07-20 11:47:24.000000 qoqo-1.6.0a1/local_dependencies/roqoqo/src/devices/generic_device.rs
--rw-r--r--   0     1001      123    18755 2023-07-20 11:47:24.000000 qoqo-1.6.0a1/local_dependencies/roqoqo/src/devices/mod.rs
--rw-r--r--   0     1001      123    22692 2023-07-20 11:47:24.000000 qoqo-1.6.0a1/local_dependencies/roqoqo/src/devices/square_lattice.rs
--rw-r--r--   0     1001      123    12690 2023-07-20 11:47:24.000000 qoqo-1.6.0a1/local_dependencies/roqoqo/src/lib.rs
--rw-r--r--   0     1001      123    12893 2023-07-20 11:47:24.000000 qoqo-1.6.0a1/local_dependencies/roqoqo/src/measurements/basis_rotation_measurement.rs
--rw-r--r--   0     1001      123     6921 2023-07-20 11:47:24.000000 qoqo-1.6.0a1/local_dependencies/roqoqo/src/measurements/cheated_basis_rotation_measurement.rs
--rw-r--r--   0     1001      123    10116 2023-07-20 11:47:24.000000 qoqo-1.6.0a1/local_dependencies/roqoqo/src/measurements/cheated_measurement.rs
--rw-r--r--   0     1001      123     3994 2023-07-20 11:47:24.000000 qoqo-1.6.0a1/local_dependencies/roqoqo/src/measurements/classical_register_measurement.rs
--rw-r--r--   0     1001      123    16003 2023-07-20 11:47:24.000000 qoqo-1.6.0a1/local_dependencies/roqoqo/src/measurements/measurement_auxiliary_data_input.rs
--rw-r--r--   0     1001      123     9562 2023-07-20 11:47:24.000000 qoqo-1.6.0a1/local_dependencies/roqoqo/src/measurements/mod.rs
--rw-r--r--   0     1001      123     6432 2023-07-20 11:47:24.000000 qoqo-1.6.0a1/local_dependencies/roqoqo/src/operations/bosonic_operations.rs
--rw-r--r--   0     1001      123     9297 2023-07-20 11:47:24.000000 qoqo-1.6.0a1/local_dependencies/roqoqo/src/operations/define_operations.rs
--rw-r--r--   0     1001      123    15648 2023-07-20 11:47:24.000000 qoqo-1.6.0a1/local_dependencies/roqoqo/src/operations/measurement_operations.rs
--rw-r--r--   0     1001      123    37139 2023-07-20 11:47:24.000000 qoqo-1.6.0a1/local_dependencies/roqoqo/src/operations/mod.rs
--rw-r--r--   0     1001      123     5717 2023-07-20 11:47:24.000000 qoqo-1.6.0a1/local_dependencies/roqoqo/src/operations/multi_qubit_gate_operations.rs
--rw-r--r--   0     1001      123    43893 2023-07-20 11:47:24.000000 qoqo-1.6.0a1/local_dependencies/roqoqo/src/operations/pragma_operations.rs
--rw-r--r--   0     1001      123    58341 2023-07-20 11:47:24.000000 qoqo-1.6.0a1/local_dependencies/roqoqo/src/operations/single_qubit_gate_operations.rs
--rw-r--r--   0     1001      123    17860 2023-07-20 11:47:24.000000 qoqo-1.6.0a1/local_dependencies/roqoqo/src/operations/three_qubit_gate_operations.rs
--rw-r--r--   0     1001      123    85038 2023-07-20 11:47:24.000000 qoqo-1.6.0a1/local_dependencies/roqoqo/src/operations/two_qubit_gate_operations.rs
--rw-r--r--   0     1001      123     1497 2023-07-20 11:47:24.000000 qoqo-1.6.0a1/local_dependencies/roqoqo/src/prelude.rs
--rw-r--r--   0     1001      123    15180 2023-07-20 11:47:24.000000 qoqo-1.6.0a1/local_dependencies/roqoqo/src/quantum_program.rs
--rw-r--r--   0     1001      123     2268 2023-07-20 11:47:24.000000 qoqo-1.6.0a1/local_dependencies/roqoqo/src/registers.rs
--rw-r--r--   0        0        0      565 1970-01-01 00:00:00.000000 qoqo-1.6.0a1/local_dependencies/qoqo-macros/Cargo.toml
--rw-r--r--   0     1001      123    11363 2023-07-20 11:47:24.000000 qoqo-1.6.0a1/local_dependencies/qoqo-macros/LICENSE
--rw-r--r--   0     1001      123    45504 2023-07-20 11:47:24.000000 qoqo-1.6.0a1/local_dependencies/qoqo-macros/src/lib.rs
--rw-r--r--   0     1001      123    11147 2023-07-20 11:47:24.000000 qoqo-1.6.0a1/local_dependencies/qoqo-macros/src/operate.rs
--rw-r--r--   0        0        0     1609 1970-01-01 00:00:00.000000 qoqo-1.6.0a1/Cargo.toml
--rw-r--r--   0     1001      123    11363 2023-07-20 11:47:24.000000 qoqo-1.6.0a1/LICENSE
--rw-r--r--   0     1001      123     3420 2023-07-20 11:47:24.000000 qoqo-1.6.0a1/README.md
--rw-r--r--   0     1001      123    14143 2023-07-20 11:47:24.000000 qoqo-1.6.0a1/build.rs
--rw-r--r--   0     1001      123      752 2023-07-20 11:47:24.000000 qoqo-1.6.0a1/pyproject.toml
--rw-r--r--   0     1001      123       87 2023-07-20 11:47:24.000000 qoqo-1.6.0a1/python_tests/README.md
--rw-r--r--   0     1001      123   955534 2023-07-20 11:47:24.000000 qoqo-1.6.0a1/qoqo/DEPENDENCIES
--rw-r--r--   0     1001      123    11881 2023-07-20 11:47:24.000000 qoqo-1.6.0a1/qoqo/LICENSE_FOR_BINARY_DISTRIBUTION
--rw-r--r--   0     1001      123     2404 2023-07-20 11:47:24.000000 qoqo-1.6.0a1/qoqo/PYTHON_LICENSE
--rw-r--r--   0     1001      123     1043 2023-07-20 11:47:24.000000 qoqo-1.6.0a1/qoqo/__init__.py
--rw-r--r--   0     1001      123    25370 2023-07-20 11:47:24.000000 qoqo-1.6.0a1/src/circuit.rs
--rw-r--r--   0     1001      123    19244 2023-07-20 11:47:24.000000 qoqo-1.6.0a1/src/circuitdag.rs
--rw-r--r--   0     1001      123     6599 2023-07-20 11:47:24.000000 qoqo-1.6.0a1/src/devices/all_to_all.rs
--rw-r--r--   0     1001      123     2707 2023-07-20 11:47:24.000000 qoqo-1.6.0a1/src/devices/generic_device.rs
--rw-r--r--   0     1001      123     3091 2023-07-20 11:47:24.000000 qoqo-1.6.0a1/src/devices/mod.rs
--rw-r--r--   0     1001      123     7642 2023-07-20 11:47:24.000000 qoqo-1.6.0a1/src/devices/square_lattice.rs
--rw-r--r--   0     1001      123     4815 2023-07-20 11:47:24.000000 qoqo-1.6.0a1/src/lib.rs
--rw-r--r--   0     1001      123    14381 2023-07-20 11:47:24.000000 qoqo-1.6.0a1/src/measurements/basis_rotation_measurement.rs
--rw-r--r--   0     1001      123    14760 2023-07-20 11:47:24.000000 qoqo-1.6.0a1/src/measurements/cheated_basis_rotation_measurement.rs
--rw-r--r--   0     1001      123    13996 2023-07-20 11:47:24.000000 qoqo-1.6.0a1/src/measurements/cheated_measurement.rs
--rw-r--r--   0     1001      123    10940 2023-07-20 11:47:24.000000 qoqo-1.6.0a1/src/measurements/classical_register_measurement.rs
--rw-r--r--   0     1001      123    26681 2023-07-20 11:47:24.000000 qoqo-1.6.0a1/src/measurements/measurement_auxiliary_data_input.rs
--rw-r--r--   0     1001      123     1753 2023-07-20 11:47:24.000000 qoqo-1.6.0a1/src/measurements/mod.rs
--rw-r--r--   0     1001      123     3552 2023-07-20 11:47:24.000000 qoqo-1.6.0a1/src/operations/bosonic_operations.rs
--rw-r--r--   0     1001      123     3391 2023-07-20 11:47:24.000000 qoqo-1.6.0a1/src/operations/define_operations.rs
--rw-r--r--   0     1001      123     4435 2023-07-20 11:47:24.000000 qoqo-1.6.0a1/src/operations/measurement_operations.rs
--rw-r--r--   0     1001      123     6180 2023-07-20 11:47:24.000000 qoqo-1.6.0a1/src/operations/mod.rs
--rw-r--r--   0     1001      123     2164 2023-07-20 11:47:24.000000 qoqo-1.6.0a1/src/operations/multi_qubit_gate_operations.rs
--rw-r--r--   0     1001      123    62577 2023-07-20 11:47:24.000000 qoqo-1.6.0a1/src/operations/pragma_operations.rs
--rw-r--r--   0     1001      123    11320 2023-07-20 11:47:24.000000 qoqo-1.6.0a1/src/operations/single_qubit_gate_operations.rs
--rw-r--r--   0     1001      123     4595 2023-07-20 11:47:24.000000 qoqo-1.6.0a1/src/operations/three_qubit_gate_operations.rs
--rw-r--r--   0     1001      123    23032 2023-07-20 11:47:24.000000 qoqo-1.6.0a1/src/operations/two_qubit_gate_operations.rs
--rw-r--r--   0     1001      123    21543 2023-07-20 11:47:24.000000 qoqo-1.6.0a1/src/quantum_program.rs
--rw-r--r--   0     1001      123    24460 2023-07-20 11:47:24.000000 qoqo-1.6.0a1/Cargo.lock
--rw-r--r--   0        0        0     4503 1970-01-01 00:00:00.000000 qoqo-1.6.0a1/PKG-INFO
+-rw-r--r--   0        0        0     1995 1970-01-01 00:00:00.000000 qoqo-1.6.0a2/local_dependencies/roqoqo/Cargo.toml
+-rw-r--r--   0     1001      123    11363 2023-08-04 12:45:00.000000 qoqo-1.6.0a2/local_dependencies/roqoqo/LICENSE
+-rw-r--r--   0     1001      123     3068 2023-08-04 12:45:00.000000 qoqo-1.6.0a2/local_dependencies/roqoqo/README.md
+-rw-r--r--   0     1001      123    36437 2023-08-04 12:45:00.000000 qoqo-1.6.0a2/local_dependencies/roqoqo/build.rs
+-rw-r--r--   0     1001      123    14193 2023-08-04 12:45:00.000000 qoqo-1.6.0a2/local_dependencies/roqoqo/src/backends.rs
+-rw-r--r--   0     1001      123    29975 2023-08-04 12:45:00.000000 qoqo-1.6.0a2/local_dependencies/roqoqo/src/circuit.rs
+-rw-r--r--   0     1001      123    47768 2023-08-04 12:45:00.000000 qoqo-1.6.0a2/local_dependencies/roqoqo/src/circuitdag.rs
+-rw-r--r--   0     1001      123    17976 2023-08-04 12:45:00.000000 qoqo-1.6.0a2/local_dependencies/roqoqo/src/devices/all_to_all.rs
+-rw-r--r--   0     1001      123    20001 2023-08-04 12:45:00.000000 qoqo-1.6.0a2/local_dependencies/roqoqo/src/devices/generic_device.rs
+-rw-r--r--   0     1001      123    18755 2023-08-04 12:45:00.000000 qoqo-1.6.0a2/local_dependencies/roqoqo/src/devices/mod.rs
+-rw-r--r--   0     1001      123    22759 2023-08-04 12:45:00.000000 qoqo-1.6.0a2/local_dependencies/roqoqo/src/devices/square_lattice.rs
+-rw-r--r--   0     1001      123    16197 2023-08-04 12:45:00.000000 qoqo-1.6.0a2/local_dependencies/roqoqo/src/lib.rs
+-rw-r--r--   0     1001      123    12890 2023-08-04 12:45:00.000000 qoqo-1.6.0a2/local_dependencies/roqoqo/src/measurements/basis_rotation_measurement.rs
+-rw-r--r--   0     1001      123     6918 2023-08-04 12:45:00.000000 qoqo-1.6.0a2/local_dependencies/roqoqo/src/measurements/cheated_basis_rotation_measurement.rs
+-rw-r--r--   0     1001      123    10113 2023-08-04 12:45:00.000000 qoqo-1.6.0a2/local_dependencies/roqoqo/src/measurements/cheated_measurement.rs
+-rw-r--r--   0     1001      123     3991 2023-08-04 12:45:00.000000 qoqo-1.6.0a2/local_dependencies/roqoqo/src/measurements/classical_register_measurement.rs
+-rw-r--r--   0     1001      123    16709 2023-08-04 12:45:00.000000 qoqo-1.6.0a2/local_dependencies/roqoqo/src/measurements/measurement_auxiliary_data_input.rs
+-rw-r--r--   0     1001      123     9562 2023-08-04 12:45:00.000000 qoqo-1.6.0a2/local_dependencies/roqoqo/src/measurements/mod.rs
+-rw-r--r--   0     1001      123     6700 2023-08-04 12:45:00.000000 qoqo-1.6.0a2/local_dependencies/roqoqo/src/operations/bosonic_operations.rs
+-rw-r--r--   0     1001      123     9279 2023-08-04 12:45:00.000000 qoqo-1.6.0a2/local_dependencies/roqoqo/src/operations/define_operations.rs
+-rw-r--r--   0     1001      123    15630 2023-08-04 12:45:00.000000 qoqo-1.6.0a2/local_dependencies/roqoqo/src/operations/measurement_operations.rs
+-rw-r--r--   0     1001      123    37139 2023-08-04 12:45:00.000000 qoqo-1.6.0a2/local_dependencies/roqoqo/src/operations/mod.rs
+-rw-r--r--   0     1001      123     5653 2023-08-04 12:45:00.000000 qoqo-1.6.0a2/local_dependencies/roqoqo/src/operations/multi_qubit_gate_operations.rs
+-rw-r--r--   0     1001      123    45668 2023-08-04 12:45:00.000000 qoqo-1.6.0a2/local_dependencies/roqoqo/src/operations/pragma_operations.rs
+-rw-r--r--   0     1001      123    58357 2023-08-04 12:45:00.000000 qoqo-1.6.0a2/local_dependencies/roqoqo/src/operations/single_qubit_gate_operations.rs
+-rw-r--r--   0     1001      123    18060 2023-08-04 12:45:00.000000 qoqo-1.6.0a2/local_dependencies/roqoqo/src/operations/three_qubit_gate_operations.rs
+-rw-r--r--   0     1001      123    85106 2023-08-04 12:45:00.000000 qoqo-1.6.0a2/local_dependencies/roqoqo/src/operations/two_qubit_gate_operations.rs
+-rw-r--r--   0     1001      123     1497 2023-08-04 12:45:00.000000 qoqo-1.6.0a2/local_dependencies/roqoqo/src/prelude.rs
+-rw-r--r--   0     1001      123    15177 2023-08-04 12:45:00.000000 qoqo-1.6.0a2/local_dependencies/roqoqo/src/quantum_program.rs
+-rw-r--r--   0     1001      123     2268 2023-08-04 12:45:00.000000 qoqo-1.6.0a2/local_dependencies/roqoqo/src/registers.rs
+-rw-r--r--   0        0        0      565 1970-01-01 00:00:00.000000 qoqo-1.6.0a2/local_dependencies/qoqo-macros/Cargo.toml
+-rw-r--r--   0     1001      123    11363 2023-08-04 12:45:00.000000 qoqo-1.6.0a2/local_dependencies/qoqo-macros/LICENSE
+-rw-r--r--   0     1001      123    47026 2023-08-04 12:45:00.000000 qoqo-1.6.0a2/local_dependencies/qoqo-macros/src/lib.rs
+-rw-r--r--   0     1001      123    11147 2023-08-04 12:45:00.000000 qoqo-1.6.0a2/local_dependencies/qoqo-macros/src/operate.rs
+-rw-r--r--   0        0        0      610 1970-01-01 00:00:00.000000 qoqo-1.6.0a2/local_dependencies/roqoqo-derive/Cargo.toml
+-rw-r--r--   0     1001      123    11363 2023-08-04 12:45:00.000000 qoqo-1.6.0a2/local_dependencies/roqoqo-derive/LICENSE
+-rw-r--r--   0     1001      123     5566 2023-08-04 12:45:00.000000 qoqo-1.6.0a2/local_dependencies/roqoqo-derive/src/involve_modes.rs
+-rw-r--r--   0     1001      123     9027 2023-08-04 12:45:00.000000 qoqo-1.6.0a2/local_dependencies/roqoqo-derive/src/involve_qubits.rs
+-rw-r--r--   0     1001      123    13554 2023-08-04 12:45:00.000000 qoqo-1.6.0a2/local_dependencies/roqoqo-derive/src/lib.rs
+-rw-r--r--   0     1001      123    10486 2023-08-04 12:45:00.000000 qoqo-1.6.0a2/local_dependencies/roqoqo-derive/src/operate.rs
+-rw-r--r--   0     1001      123     7015 2023-08-04 12:45:00.000000 qoqo-1.6.0a2/local_dependencies/roqoqo-derive/src/operate_n_mode.rs
+-rw-r--r--   0     1001      123    13664 2023-08-04 12:45:00.000000 qoqo-1.6.0a2/local_dependencies/roqoqo-derive/src/operate_n_qubit.rs
+-rw-r--r--   0     1001      123    17807 2023-08-04 12:45:00.000000 qoqo-1.6.0a2/local_dependencies/roqoqo-derive/src/operate_unitary.rs
+-rw-r--r--   0     1001      123     3126 2023-08-04 12:45:00.000000 qoqo-1.6.0a2/local_dependencies/roqoqo-derive/src/operate_unitary_modes.rs
+-rw-r--r--   0     1001      123     5488 2023-08-04 12:45:00.000000 qoqo-1.6.0a2/local_dependencies/roqoqo-derive/src/substitute.rs
+-rw-r--r--   0     1001      123     3286 2023-08-04 12:45:00.000000 qoqo-1.6.0a2/local_dependencies/roqoqo-derive/src/substitute_modes.rs
+-rw-r--r--   0     1001      123     2452 2023-08-04 12:45:00.000000 qoqo-1.6.0a2/local_dependencies/roqoqo-derive/src/supported_version.rs
+-rw-r--r--   0        0        0     1678 1970-01-01 00:00:00.000000 qoqo-1.6.0a2/Cargo.toml
+-rw-r--r--   0     1001      123    11363 2023-08-04 12:45:00.000000 qoqo-1.6.0a2/LICENSE
+-rw-r--r--   0     1001      123     3420 2023-08-04 12:45:00.000000 qoqo-1.6.0a2/README.md
+-rw-r--r--   0     1001      123    14143 2023-08-04 12:45:00.000000 qoqo-1.6.0a2/build.rs
+-rw-r--r--   0     1001      123      752 2023-08-04 12:45:00.000000 qoqo-1.6.0a2/pyproject.toml
+-rw-r--r--   0     1001      123       87 2023-08-04 12:45:00.000000 qoqo-1.6.0a2/python_tests/README.md
+-rw-r--r--   0     1001      123   955534 2023-08-04 12:45:00.000000 qoqo-1.6.0a2/qoqo/DEPENDENCIES
+-rw-r--r--   0     1001      123    11881 2023-08-04 12:45:00.000000 qoqo-1.6.0a2/qoqo/LICENSE_FOR_BINARY_DISTRIBUTION
+-rw-r--r--   0     1001      123     2404 2023-08-04 12:45:00.000000 qoqo-1.6.0a2/qoqo/PYTHON_LICENSE
+-rw-r--r--   0     1001      123     1043 2023-08-04 12:45:00.000000 qoqo-1.6.0a2/qoqo/__init__.py
+-rw-r--r--   0     1001      123    26503 2023-08-04 12:45:00.000000 qoqo-1.6.0a2/src/circuit.rs
+-rw-r--r--   0     1001      123    19244 2023-08-04 12:45:00.000000 qoqo-1.6.0a2/src/circuitdag.rs
+-rw-r--r--   0     1001      123     7856 2023-08-04 12:45:00.000000 qoqo-1.6.0a2/src/devices/all_to_all.rs
+-rw-r--r--   0     1001      123     3945 2023-08-04 12:45:00.000000 qoqo-1.6.0a2/src/devices/generic_device.rs
+-rw-r--r--   0     1001      123     3091 2023-08-04 12:45:00.000000 qoqo-1.6.0a2/src/devices/mod.rs
+-rw-r--r--   0     1001      123     8909 2023-08-04 12:45:00.000000 qoqo-1.6.0a2/src/devices/square_lattice.rs
+-rw-r--r--   0     1001      123     4815 2023-08-04 12:45:00.000000 qoqo-1.6.0a2/src/lib.rs
+-rw-r--r--   0     1001      123    15587 2023-08-04 12:45:00.000000 qoqo-1.6.0a2/src/measurements/basis_rotation_measurement.rs
+-rw-r--r--   0     1001      123    15980 2023-08-04 12:45:00.000000 qoqo-1.6.0a2/src/measurements/cheated_basis_rotation_measurement.rs
+-rw-r--r--   0     1001      123    15190 2023-08-04 12:45:00.000000 qoqo-1.6.0a2/src/measurements/cheated_measurement.rs
+-rw-r--r--   0     1001      123    12154 2023-08-04 12:45:00.000000 qoqo-1.6.0a2/src/measurements/classical_register_measurement.rs
+-rw-r--r--   0     1001      123    30240 2023-08-04 12:45:00.000000 qoqo-1.6.0a2/src/measurements/measurement_auxiliary_data_input.rs
+-rw-r--r--   0     1001      123     1753 2023-08-04 12:45:00.000000 qoqo-1.6.0a2/src/measurements/mod.rs
+-rw-r--r--   0     1001      123     3698 2023-08-04 12:45:00.000000 qoqo-1.6.0a2/src/operations/bosonic_operations.rs
+-rw-r--r--   0     1001      123     3523 2023-08-04 12:45:00.000000 qoqo-1.6.0a2/src/operations/define_operations.rs
+-rw-r--r--   0     1001      123     4567 2023-08-04 12:45:00.000000 qoqo-1.6.0a2/src/operations/measurement_operations.rs
+-rw-r--r--   0     1001      123     6180 2023-08-04 12:45:00.000000 qoqo-1.6.0a2/src/operations/mod.rs
+-rw-r--r--   0     1001      123     2300 2023-08-04 12:45:00.000000 qoqo-1.6.0a2/src/operations/multi_qubit_gate_operations.rs
+-rw-r--r--   0     1001      123    67489 2023-08-04 12:45:00.000000 qoqo-1.6.0a2/src/operations/pragma_operations.rs
+-rw-r--r--   0     1001      123    11830 2023-08-04 12:45:00.000000 qoqo-1.6.0a2/src/operations/single_qubit_gate_operations.rs
+-rw-r--r--   0     1001      123     4761 2023-08-04 12:45:00.000000 qoqo-1.6.0a2/src/operations/three_qubit_gate_operations.rs
+-rw-r--r--   0     1001      123    23588 2023-08-04 12:45:00.000000 qoqo-1.6.0a2/src/operations/two_qubit_gate_operations.rs
+-rw-r--r--   0     1001      123    22764 2023-08-04 12:45:00.000000 qoqo-1.6.0a2/src/quantum_program.rs
+-rw-r--r--   0     1001      123    48888 2023-08-04 12:45:00.000000 qoqo-1.6.0a2/Cargo.lock
+-rw-r--r--   0        0        0     4503 1970-01-01 00:00:00.000000 qoqo-1.6.0a2/PKG-INFO
```

### Comparing `qoqo-1.6.0a1/local_dependencies/roqoqo-derive/Cargo.toml` & `qoqo-1.6.0a2/local_dependencies/roqoqo-derive/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "roqoqo-derive"
-version = "1.6.0-alpha.1"
+version = "1.6.0-alpha.2"
 authors = ["HQS Quantum Simulations <info@quantumsimulations.de>"]
 license = "Apache-2.0"
 edition = "2021"
 rust-version = "1.56"
 categories = ["science", "simulation"]
 readme = "../README.md"
 description = "Macros for the roqoqo crate"
```

### Comparing `qoqo-1.6.0a1/local_dependencies/roqoqo-derive/LICENSE` & `qoqo-1.6.0a2/local_dependencies/roqoqo/LICENSE`

 * *Files identical despite different names*

### Comparing `qoqo-1.6.0a1/local_dependencies/roqoqo-derive/src/involve_modes.rs` & `qoqo-1.6.0a2/local_dependencies/roqoqo-derive/src/involve_modes.rs`

 * *Files identical despite different names*

### Comparing `qoqo-1.6.0a1/local_dependencies/roqoqo-derive/src/involve_qubits.rs` & `qoqo-1.6.0a2/local_dependencies/roqoqo-derive/src/involve_qubits.rs`

 * *Files identical despite different names*

### Comparing `qoqo-1.6.0a1/local_dependencies/roqoqo-derive/src/lib.rs` & `qoqo-1.6.0a2/local_dependencies/roqoqo-derive/src/lib.rs`

 * *Files identical despite different names*

### Comparing `qoqo-1.6.0a1/local_dependencies/roqoqo-derive/src/operate.rs` & `qoqo-1.6.0a2/local_dependencies/roqoqo-derive/src/operate.rs`

 * *Files identical despite different names*

### Comparing `qoqo-1.6.0a1/local_dependencies/roqoqo-derive/src/operate_n_mode.rs` & `qoqo-1.6.0a2/local_dependencies/roqoqo-derive/src/operate_n_mode.rs`

 * *Files identical despite different names*

### Comparing `qoqo-1.6.0a1/local_dependencies/roqoqo-derive/src/operate_n_qubit.rs` & `qoqo-1.6.0a2/local_dependencies/roqoqo-derive/src/operate_n_qubit.rs`

 * *Files identical despite different names*

### Comparing `qoqo-1.6.0a1/local_dependencies/roqoqo-derive/src/operate_unitary.rs` & `qoqo-1.6.0a2/local_dependencies/roqoqo-derive/src/operate_unitary.rs`

 * *Files identical despite different names*

### Comparing `qoqo-1.6.0a1/local_dependencies/roqoqo-derive/src/operate_unitary_modes.rs` & `qoqo-1.6.0a2/local_dependencies/roqoqo-derive/src/operate_unitary_modes.rs`

 * *Files identical despite different names*

### Comparing `qoqo-1.6.0a1/local_dependencies/roqoqo-derive/src/substitute.rs` & `qoqo-1.6.0a2/local_dependencies/roqoqo-derive/src/substitute.rs`

 * *Files identical despite different names*

### Comparing `qoqo-1.6.0a1/local_dependencies/roqoqo-derive/src/substitute_modes.rs` & `qoqo-1.6.0a2/local_dependencies/roqoqo-derive/src/substitute_modes.rs`

 * *Files identical despite different names*

### Comparing `qoqo-1.6.0a1/local_dependencies/roqoqo-derive/src/supported_version.rs` & `qoqo-1.6.0a2/local_dependencies/roqoqo-derive/src/supported_version.rs`

 * *Files identical despite different names*

### Comparing `qoqo-1.6.0a1/local_dependencies/roqoqo/Cargo.toml` & `qoqo-1.6.0a2/local_dependencies/roqoqo/Cargo.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "roqoqo"
-version = "1.6.0-alpha.1"
+version = "1.6.0-alpha.2"
 authors = ["HQS Quantum Simulations <info@quantumsimulations.de>"]
 license = "Apache-2.0"
 edition = "2021"
 rust-version = "1.56"
 categories = ["science", "simulation"]
 homepage = "https://github.com/HQSquantumsimulations/qoqo"
 repository = "https://github.com/HQSquantumsimulations/qoqo"
@@ -24,18 +24,19 @@
 [dependencies]
 serde = { version = "1.0", features = ["derive"], optional=true}
 ndarray = { version = "0.15" }
 num-complex = { version = "0.4"}
 thiserror = "1.0"
 dyn-clone = {version="1.0", optional=true}
 qoqo_calculator = { version="1.1"}
-roqoqo-derive = {version="1.6.0-alpha.1", path= "../roqoqo-derive" }
+roqoqo-derive = {version="1.6.0-alpha.2", path= "../roqoqo-derive" }
 typetag = {version="0.2", optional=true}
 nalgebra = "0.32"
-# schemars = { version="0.8", features = ["num-complex", "ndarray"], optional=true }
+schemars = { version="0.8", optional=true }
+jsonschema = { version="0.17", optional=true }
 rand_distr = {version="0.4", optional=true}
 rand = { version = "0.8.4"}
 async-trait = {version = "0.1", optional = true}
 futures ={version = "0.3", optional=true}
 petgraph = {version = "0.6.2", optional=true}
 bincode = {version="1.3", optional=true}
 
@@ -51,9 +52,9 @@
 [features]
 default = ["serialize", "circuitdag"]
 dynamic = ["typetag", "dyn-clone"]
 unstable_qoqo_devices = []
 serialize = ["serde", "ndarray/serde", "num-complex/serde", "bincode", "petgraph/serde-1"]
 overrotate = [ "rand_distr", "roqoqo-derive/overrotate"]
 async = ["async-trait", "futures"]
-# json_schema=["schemars", "serialize", "qoqo_calculator/json_schema"]
+json_schema=["schemars", "serialize", "qoqo_calculator/json_schema", "jsonschema"]
 circuitdag = ["petgraph"]
```

### Comparing `qoqo-1.6.0a1/local_dependencies/roqoqo/LICENSE` & `qoqo-1.6.0a2/local_dependencies/qoqo-macros/LICENSE`

 * *Files identical despite different names*

### Comparing `qoqo-1.6.0a1/local_dependencies/roqoqo/README.md` & `qoqo-1.6.0a2/local_dependencies/roqoqo/README.md`

 * *Files identical despite different names*

### Comparing `qoqo-1.6.0a1/local_dependencies/roqoqo/build.rs` & `qoqo-1.6.0a2/local_dependencies/roqoqo/build.rs`

 * *Files 2% similar despite different names*

```diff
@@ -549,197 +549,197 @@
     let final_quote = quote! {
 
         //use crate::operations::*;
 
         /// Enum of all Operations implementing [Operate]
         #[derive(Debug, Clone, PartialEq, InvolveQubits, Operate, Substitute, SupportedVersion)]
         #[cfg_attr(feature = "serialize", derive(serde::Serialize, serde::Deserialize))]
-        // #[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
+        #[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
         #[non_exhaustive]
         pub enum Operation {
             #(#operations_quotes),* ,
 
         }
 
         /// Enum of all Operations implementing [OperateSingleQubit]
         #[derive(Debug, Clone, PartialEq, InvolveQubits, Operate, OperateTryFromEnum, Substitute, OperateSingleQubit, SupportedVersion)]
         #[cfg_attr(feature = "serialize", derive(serde::Serialize, serde::Deserialize))]
-        // #[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
+        #[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
         #[non_exhaustive]
         pub enum SingleQubitOperation {
             #(#single_qubit_operations_quotes),*
         }
 
         /// Enum of all Operations implementing [OperateTwoQubit]
         #[derive(Debug, Clone, PartialEq, InvolveQubits, Operate, OperateTryFromEnum, Substitute, OperateTwoQubit,  SupportedVersion)]
         #[cfg_attr(feature = "serialize", derive(serde::Serialize, serde::Deserialize))]
-        // #[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
+        #[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
         #[non_exhaustive]
         pub enum TwoQubitOperation {
             #(#two_qubit_operations_quotes),*
         }
 
         /// Enum of all Operations implementing [OperateThreeQubit]
         #[derive(Debug, Clone, PartialEq, InvolveQubits, Operate, OperateTryFromEnum, Substitute, OperateThreeQubit,  SupportedVersion)]
         #[cfg_attr(feature = "serialize", derive(serde::Serialize, serde::Deserialize))]
-        // #[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
+        #[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
         #[non_exhaustive]
         pub enum ThreeQubitOperation {
             #(#three_qubit_operations_quotes),*
         }
 
         /// Enum of all Operations implementing [OperateMultiQubit]
         #[derive(Debug, Clone, PartialEq, InvolveQubits, Operate, OperateTryFromEnum, Substitute, OperateMultiQubit,  SupportedVersion)]
         #[cfg_attr(feature = "serialize", derive(serde::Serialize, serde::Deserialize))]
-        // #[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
+        #[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
         #[non_exhaustive]
         pub enum MultiQubitOperation {
             #(#multi_qubit_operations_quotes),*
         }
 
         /// Enum of all Operations implementing [OperatePragma]
         #[derive(Debug, Clone, PartialEq, InvolveQubits, Operate, OperateTryFromEnum, Substitute, OperatePragma,  SupportedVersion)]
-        // #[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
         #[cfg_attr(feature = "serialize", derive(serde::Serialize, serde::Deserialize))]
+        #[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
         #[non_exhaustive]
         pub enum PragmaOperation {
             #(#pragma_operations_quotes),*
         }
 
         /// Enum of all Operations implementing [OperatePragmaNoise]
         #[derive(Debug, Clone, PartialEq, InvolveQubits, Operate, OperateTryFromEnum, Substitute, OperatePragma, OperatePragmaNoise,  SupportedVersion)]
-        // #[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
         #[cfg_attr(feature = "serialize", derive(serde::Serialize, serde::Deserialize))]
+        #[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
         #[non_exhaustive]
         pub enum PragmaNoiseOperation {
             #(#pragma_noise_operations_quotes),*
         }
 
         /// Enum of all Operations implementing [OperatePragmaNoiseProba]
         #[derive(Debug, Clone, PartialEq, InvolveQubits, Operate, OperateTryFromEnum, Substitute, OperatePragma, OperatePragmaNoise, OperatePragmaNoiseProba,  SupportedVersion)]
         #[cfg_attr(feature = "serialize", derive(serde::Serialize, serde::Deserialize))]
-        // #[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
+        #[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
         #[non_exhaustive]
         pub enum PragmaNoiseProbaOperation {
             #(#pragma_noise_proba_operations_quotes),*
         }
 
         /// Enum of all Operations implementing [OperateGate]
         #[derive(Debug, Clone, PartialEq, InvolveQubits, Operate, OperateTryFromEnum, Substitute, OperateGate,  SupportedVersion)]
         #[cfg_attr(feature = "serialize", derive(serde::Serialize, serde::Deserialize))]
-        // #[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
+        #[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
         #[non_exhaustive]
         pub enum GateOperation {
             #(#gate_operations_quotes),*
         }
 
         /// Enum of all Operations implementing [Rotate]
         #[allow(clippy::upper_case_acronyms)]
         #[derive(Debug, Clone, PartialEq, InvolveQubits, Operate, OperateTryFromEnum, Substitute, OperateGate, Rotate,  SupportedVersion)]
         #[cfg_attr(feature = "serialize", derive(serde::Serialize, serde::Deserialize))]
-        // #[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
+        #[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
         #[non_exhaustive]
         pub enum Rotation {
             #(#rotations_quotes),*
         }
 
         /// Enum of all Operations implementing [Define]
         #[derive(Debug, Clone, PartialEq,InvolveQubits, Operate, OperateTryFromEnum, Substitute, Define,  SupportedVersion)]
         #[cfg_attr(feature = "serialize", derive(serde::Serialize, serde::Deserialize))]
-        // #[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
+        #[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
         #[non_exhaustive]
         pub enum Definition {
             #(#definitions_quotes),* ,
         }
 
         /// Enum of all Operations implementing [OperateConstantGate]
         #[derive(Debug, Clone, PartialEq, Eq,InvolveQubits, Operate, OperateTryFromEnum, Substitute, OperateGate, OperateConstantGate,  SupportedVersion)]
         #[cfg_attr(feature = "serialize", derive(serde::Serialize, serde::Deserialize))]
-        // #[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
+        #[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
         #[non_exhaustive]
         pub enum ConstantGateOperation {
             #(#constant_gate_operations_quote),*
         }
 
         /// Enum of all Operations implementing [OperateSingleQubitGate]
         #[derive(Debug, Clone, PartialEq, InvolveQubits, Operate, OperateTryFromEnum, Substitute, OperateGate, OperateSingleQubit, OperateSingleQubitGate,  SupportedVersion)]
         #[cfg_attr(feature = "serialize", derive(serde::Serialize, serde::Deserialize))]
-        // #[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
+        #[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
         #[non_exhaustive]
         pub enum SingleQubitGateOperation {
             #(#single_qubit_gate_operations_quote),*
         }
 
         /// Enum of all Operations implementing [OperateTwoQubitGate]
         #[derive(Debug, Clone, PartialEq, InvolveQubits, Operate, OperateTryFromEnum, Substitute, OperateGate, OperateTwoQubit, OperateTwoQubitGate,  SupportedVersion)]
         #[cfg_attr(feature = "serialize", derive(serde::Serialize, serde::Deserialize))]
-        // #[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
+        #[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
         #[non_exhaustive]
         pub enum TwoQubitGateOperation {
             #(#two_qubit_gate_operations_quote),*
         }
 
         /// Enum of all Operations implementing [OperateThreeQubitGate]
         #[derive(Debug, Clone, PartialEq, InvolveQubits, Operate, OperateTryFromEnum, Substitute, OperateGate, OperateThreeQubit, OperateThreeQubitGate,  SupportedVersion)]
         #[cfg_attr(feature = "serialize", derive(serde::Serialize, serde::Deserialize))]
-        // #[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
+        #[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
         #[non_exhaustive]
         pub enum ThreeQubitGateOperation {
             #(#three_qubit_gate_operations_quote),*
         }
 
         /// Enum of all Operations implementing [OperateMultiQubitGate]
         #[derive(Debug, Clone, PartialEq, InvolveQubits, Operate, OperateTryFromEnum, Substitute, OperateGate, OperateMultiQubit, OperateMultiQubitGate, SupportedVersion)]
         #[cfg_attr(feature = "serialize", derive(serde::Serialize, serde::Deserialize))]
-        // #[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
+        #[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
         #[non_exhaustive]
         pub enum MultiQubitGateOperation {
             #(#multi_qubit_gate_operations_quote),*
         }
 
         /// Enum of all Operations implementing [OperateModeGate]
         #[derive(Debug, Clone, PartialEq, InvolveQubits, InvolveModes, Operate, OperateTryFromEnum, Substitute, SubstituteModes, OperateModeGate,SupportedVersion)]
         #[cfg_attr(feature = "serialize", derive(serde::Serialize, serde::Deserialize))]
-        // #[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
+        #[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
         #[non_exhaustive]
         pub enum ModeGateOperation {
             #(#mode_gate_operations_quotes),*
         }
 
         /// Enum of all Operations implementing [OperateSingleMode]
         #[derive(Debug, Clone, PartialEq, InvolveQubits, InvolveModes, Operate, OperateTryFromEnum, Substitute, SubstituteModes, OperateSingleMode,SupportedVersion)]
         #[cfg_attr(feature = "serialize", derive(serde::Serialize, serde::Deserialize))]
-        // #[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
+        #[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
         #[non_exhaustive]
         pub enum SingleModeOperation {
             #(#single_mode_operations_quotes),*
         }
 
         /// Enum of all Operations implementing [OperateTwoMode]
         #[derive(Debug, Clone, PartialEq, InvolveQubits, InvolveModes, Operate, OperateTryFromEnum, Substitute, SubstituteModes, OperateTwoMode, SupportedVersion)]
         #[cfg_attr(feature = "serialize", derive(serde::Serialize, serde::Deserialize))]
-        // #[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
+        #[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
         #[non_exhaustive]
         pub enum TwoModeOperation {
             #(#two_mode_operations_quotes),*
         }
 
         /// Enum of all Operations implementing [OperateSingleModeGate]
         #[derive(Debug, Clone, PartialEq, InvolveQubits, InvolveModes, Operate, OperateTryFromEnum, Substitute, SubstituteModes, OperateModeGate, OperateSingleMode, OperateSingleModeGate, SupportedVersion)]
         #[cfg_attr(feature = "serialize", derive(serde::Serialize, serde::Deserialize))]
-        // #[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
+        #[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
         #[non_exhaustive]
         pub enum SingleModeGateOperation {
             #(#single_mode_gate_operations_quote),*
         }
 
         /// Enum of all Operations implementing [OperateTwoModeGate]
         #[derive(Debug, Clone, PartialEq, InvolveQubits, InvolveModes, Operate, OperateTryFromEnum, Substitute, SubstituteModes, OperateModeGate, OperateTwoMode, OperateTwoModeGate, SupportedVersion)]
         #[cfg_attr(feature = "serialize", derive(serde::Serialize, serde::Deserialize))]
-        // #[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
+        #[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
         #[non_exhaustive]
         pub enum TwoModeGateOperation {
             #(#two_mode_gate_operations_quote),*
         }
 
     };
     let final_str = format!("{}", final_quote);
```

### Comparing `qoqo-1.6.0a1/local_dependencies/roqoqo/src/backends.rs` & `qoqo-1.6.0a2/local_dependencies/roqoqo/src/backends.rs`

 * *Files identical despite different names*

### Comparing `qoqo-1.6.0a1/local_dependencies/roqoqo/src/circuit.rs` & `qoqo-1.6.0a2/local_dependencies/roqoqo/src/circuit.rs`

 * *Files 0% similar despite different names*

```diff
@@ -82,15 +82,15 @@
 /// * `extend(iterator)`: adds the operations in the specified iterator to the Circuit
 /// * `default()`: creates an empty Circuit
 /// * `[...]`: gets a slice of the Circuit (returned as a vector)
 /// * `+` and `+=`: add two circuits or an operation to the Circuit
 ///
 #[derive(Debug, Clone, PartialEq)]
 #[cfg_attr(feature = "serialize", derive(serde::Serialize, serde::Deserialize))]
-// #[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
+#[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
 #[cfg_attr(feature = "serialize", serde(try_from = "CircuitSerializable"))]
 #[cfg_attr(feature = "serialize", serde(into = "CircuitSerializable"))]
 pub struct Circuit {
     /// Definitions in the quantum circuit, must be unique.
     definitions: Vec<Operation>,
     /// Operations of the quantum circuit, do not have to be unique.
     operations: Vec<Operation>,
```

### Comparing `qoqo-1.6.0a1/local_dependencies/roqoqo/src/circuitdag.rs` & `qoqo-1.6.0a2/local_dependencies/roqoqo/src/circuitdag.rs`

 * *Files identical despite different names*

### Comparing `qoqo-1.6.0a1/local_dependencies/roqoqo/src/devices/all_to_all.rs` & `qoqo-1.6.0a2/local_dependencies/roqoqo/src/devices/all_to_all.rs`

 * *Files 0% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 use super::GenericDevice;
 use crate::RoqoqoError;
 use ndarray::Array2;
 /// A device assuming all-to-all connectivity between all involved qubits.
 ///
 #[derive(Clone, Debug, PartialEq, Default)]
 #[cfg_attr(feature = "serialize", derive(serde::Serialize, serde::Deserialize))]
+#[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
 pub struct AllToAllDevice {
     number_qubits: usize,
     generic_device: GenericDevice,
 }
 
 impl AllToAllDevice {
     /// Creates a new AllToAllDevice.
```

### Comparing `qoqo-1.6.0a1/local_dependencies/roqoqo/src/devices/generic_device.rs` & `qoqo-1.6.0a2/local_dependencies/roqoqo/src/devices/generic_device.rs`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 // License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either
 // express or implied. See the License for the specific language governing permissions and
 // limitations under the License.
 
 use std::collections::HashMap;
 
 use super::Device;
+#[cfg(feature = "json_schema")]
+use crate::Array2f64Def;
 use crate::RoqoqoError;
 use crate::RoqoqoVersionSerializable;
 use ndarray::{array, Array2};
 /// A generic device assuming all-to-all connectivity between all involved qubits.
 ///
 /// # Note
 ///
@@ -35,33 +37,60 @@
     pub two_qubit_gates: HashMap<String, TwoQubitGates>,
     /// Gate times for all multi qubit gates
     pub multi_qubit_gates: HashMap<String, HashMap<Vec<usize>, f64>>,
     /// Decoherence rates for all qubits
     pub decoherence_rates: HashMap<usize, Array2<f64>>,
 }
 
+#[cfg(feature = "json_schema")]
+impl schemars::JsonSchema for GenericDevice {
+    fn schema_name() -> String {
+        "GenericDevice".to_string()
+    }
+
+    fn json_schema(gen: &mut schemars::gen::SchemaGenerator) -> schemars::schema::Schema {
+        <SchemaHelperGenericDeviceSerialize<Array2f64Def>>::json_schema(gen)
+    }
+}
+
 type TwoQubitGates = HashMap<(usize, usize), f64>;
 type TwoQubitGatesVec = Vec<((usize, usize), f64)>;
 
 #[derive(Clone)]
 #[cfg_attr(feature = "serialize", derive(serde::Serialize, serde::Deserialize))]
-
 struct GenericDeviceSerialize {
+    /// The number of qubits
     number_qubits: usize,
     /// Gate times for all single qubit gates
     single_qubit_gates: HashMap<String, Vec<(usize, f64)>>,
     /// Gate times for all two qubit gates
     two_qubit_gates: HashMap<String, TwoQubitGatesVec>,
     /// Gate times for all multi qubit gates
     multi_qubit_gates: HashMap<String, Vec<(Vec<usize>, f64)>>,
     /// Decoherence rates for all qubits
     decoherence_rates: Vec<(usize, Array2<f64>)>,
     _roqoqo_version: RoqoqoVersionSerializable,
 }
 
+#[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
+#[allow(dead_code)]
+struct SchemaHelperGenericDeviceSerialize<Array2f64Def> {
+    /// The number of qubits
+    number_qubits: usize,
+    /// Gate times for all single qubit gates
+    single_qubit_gates: HashMap<String, Vec<(usize, f64)>>,
+    /// Gate times for all two qubit gates
+    two_qubit_gates: HashMap<String, TwoQubitGatesVec>,
+    /// Gate times for all multi qubit gates
+    multi_qubit_gates: HashMap<String, Vec<(Vec<usize>, f64)>>,
+    /// Decoherence rates for all qubits
+    decoherence_rates: Vec<(usize, Array2f64Def)>,
+    _roqoqo_version: RoqoqoVersionSerializable,
+}
+
 impl From<GenericDeviceSerialize> for GenericDevice {
     fn from(value: GenericDeviceSerialize) -> Self {
         let mut two_qubit_gates: HashMap<String, TwoQubitGates> =
             HashMap::with_capacity(value.two_qubit_gates.len());
         let mut single_qubit_gates: HashMap<String, HashMap<usize, f64>> =
             HashMap::with_capacity(value.two_qubit_gates.len());
         let mut multi_qubit_gates: HashMap<String, HashMap<Vec<usize>, f64>> =
```

### Comparing `qoqo-1.6.0a1/local_dependencies/roqoqo/src/devices/mod.rs` & `qoqo-1.6.0a2/local_dependencies/roqoqo/src/devices/mod.rs`

 * *Files identical despite different names*

### Comparing `qoqo-1.6.0a1/local_dependencies/roqoqo/src/devices/square_lattice.rs` & `qoqo-1.6.0a2/local_dependencies/roqoqo/src/devices/square_lattice.rs`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 use super::GenericDevice;
 use crate::RoqoqoError;
 use ndarray::Array2;
 /// A device assuming all-to-all connectivity between all involved qubits.
 ///
 #[derive(Clone, Debug, PartialEq, Default)]
 #[cfg_attr(feature = "serialize", derive(serde::Serialize, serde::Deserialize))]
+#[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
 pub struct SquareLatticeDevice {
     number_rows: usize,
     number_columns: usize,
     generic_device: GenericDevice,
 }
 
 impl SquareLatticeDevice {
```

### Comparing `qoqo-1.6.0a1/local_dependencies/roqoqo/src/lib.rs` & `qoqo-1.6.0a2/local_dependencies/roqoqo/src/lib.rs`

 * *Files 22% similar despite different names*

```diff
@@ -19,41 +19,47 @@
 
 //! # roqoqo
 //!
 //! `Rust only Quantum Operation Quantum Operation` - the quantum computing toolkit by HQS Quantum Simulations.
 //!
 use qoqo_calculator::CalculatorError;
 use qoqo_calculator::CalculatorFloat;
-// #[cfg(feature = "json_schema")]
-// use schemars::{schema::Schema, JsonSchema};
+#[cfg(feature = "json_schema")]
+use schemars::{
+    gen::SchemaGenerator,
+    schema::SchemaObject,
+    schema::{InstanceType, Schema},
+    JsonSchema,
+};
 use std::str::FromStr;
 use thiserror::Error;
 
 /// roqoqo version information, used for roqoqo import/export checks
 pub const ROQOQO_VERSION: &str = env!("CARGO_PKG_VERSION");
 
 #[derive(Clone, Copy, PartialEq, Eq, PartialOrd, Ord, Debug, Default)]
 #[cfg_attr(feature = "serialize", derive(serde::Serialize, serde::Deserialize))]
 #[cfg_attr(feature = "serialize", serde(try_from = "RoqoqoVersionSerializable"))]
 #[cfg_attr(feature = "serialize", serde(into = "RoqoqoVersionSerializable"))]
 
 struct RoqoqoVersion;
 
-// #[cfg(feature = "json_schema")]
-// impl JsonSchema for RoqoqoVersion {
-//     fn schema_name() -> String {
-//         "RoqoqoVersion".to_string()
-//     }
-
-//     fn json_schema(gen: &mut schemars::gen::SchemaGenerator) -> Schema {
-//         RoqoqoVersionSerializable::json_schema(gen)
-//     }
-// }
+#[cfg(feature = "json_schema")]
+impl JsonSchema for RoqoqoVersion {
+    fn schema_name() -> String {
+        "RoqoqoVersion".to_string()
+    }
+
+    fn json_schema(gen: &mut schemars::gen::SchemaGenerator) -> Schema {
+        RoqoqoVersionSerializable::json_schema(gen)
+    }
+}
+
 #[derive(Clone, Copy, PartialEq, Eq, PartialOrd, Ord, Debug, Default)]
-// #[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
+#[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
 #[cfg_attr(feature = "serialize", derive(serde::Serialize, serde::Deserialize))]
 struct RoqoqoVersionSerializable {
     /// The semver major version of roqoqo
     major_version: u32,
     /// The semver minor version of roqoqo
     minor_version: u32,
 }
@@ -307,14 +313,119 @@
     #[error(transparent)]
     RoqoqoError(#[from] RoqoqoError),
     /// Transparent propagation of CalculatorError.
     #[error(transparent)]
     CalculatorError(#[from] CalculatorError),
 }
 
+#[cfg(feature = "json_schema")]
+pub(crate) struct Complex64Def;
+#[cfg(feature = "json_schema")]
+impl JsonSchema for Complex64Def {
+    fn schema_name() -> String {
+        "Complex64".to_string()
+    }
+    fn json_schema(gen: &mut SchemaGenerator) -> Schema {
+        let mut schema = SchemaObject {
+            instance_type: Some(InstanceType::Number.into()),
+            ..Default::default()
+        };
+        let obj = schema.object();
+        obj.required.insert("re".to_owned());
+        obj.required.insert("im".to_owned());
+        obj.properties
+            .insert("re".to_owned(), <f64>::json_schema(gen));
+        obj.properties
+            .insert("im".to_owned(), <f64>::json_schema(gen));
+        schema.into()
+    }
+}
+
+#[cfg(feature = "json_schema")]
+pub(crate) struct Array1C64Def;
+#[cfg(feature = "json_schema")]
+impl JsonSchema for Array1C64Def {
+    fn schema_name() -> String {
+        "Array1_Complex64".to_string()
+    }
+    fn json_schema(gen: &mut SchemaGenerator) -> Schema {
+        let mut schema = SchemaObject {
+            instance_type: Some(InstanceType::Object.into()),
+            ..Default::default()
+        };
+        let obj = schema.object();
+        obj.required.insert("v".to_owned());
+        obj.required.insert("dim".to_owned());
+        obj.required.insert("data".to_owned());
+        obj.properties
+            .insert("v".to_owned(), <u8>::json_schema(gen));
+        obj.properties
+            .insert("dim".to_owned(), <Vec<u8>>::json_schema(gen));
+        obj.properties.insert(
+            "data".to_owned(),
+            <Vec<Vec<Complex64Def>>>::json_schema(gen),
+        );
+        schema.into()
+    }
+}
+
+#[cfg(feature = "json_schema")]
+pub(crate) struct Array2C64Def;
+#[cfg(feature = "json_schema")]
+impl JsonSchema for Array2C64Def {
+    fn schema_name() -> String {
+        "Array2_Complex64".to_string()
+    }
+    fn json_schema(gen: &mut SchemaGenerator) -> Schema {
+        let mut schema = SchemaObject {
+            instance_type: Some(InstanceType::Object.into()),
+            ..Default::default()
+        };
+        let obj = schema.object();
+        obj.required.insert("v".to_owned());
+        obj.required.insert("dim".to_owned());
+        obj.required.insert("data".to_owned());
+        obj.properties
+            .insert("v".to_owned(), <u8>::json_schema(gen));
+        obj.properties
+            .insert("dim".to_owned(), <Vec<u8>>::json_schema(gen));
+        obj.properties.insert(
+            "data".to_owned(),
+            <Vec<Vec<Complex64Def>>>::json_schema(gen),
+        );
+        schema.into()
+    }
+}
+
+#[cfg(feature = "json_schema")]
+pub(crate) struct Array2f64Def;
+#[cfg(feature = "json_schema")]
+impl JsonSchema for Array2f64Def {
+    fn schema_name() -> String {
+        "Array2_f64".to_string()
+    }
+    fn json_schema(gen: &mut SchemaGenerator) -> Schema {
+        let mut schema = SchemaObject {
+            instance_type: Some(InstanceType::Object.into()),
+            ..Default::default()
+        };
+        let obj = schema.object();
+        obj.required.insert("v".to_owned());
+        obj.required.insert("dim".to_owned());
+        obj.required.insert("data".to_owned());
+        obj.properties
+            .insert("v".to_owned(), <u8>::json_schema(gen));
+        obj.properties
+            .insert("dim".to_owned(), <Vec<u8>>::json_schema(gen));
+        obj.properties
+            .insert("data".to_owned(), <Vec<f64>>::json_schema(gen));
+        schema.into()
+    }
+}
+
 #[doc(hidden)]
 mod circuit;
 pub use circuit::Circuit;
 #[doc(hidden)]
 pub use circuit::*;
 #[cfg(feature = "circuitdag")]
 mod circuitdag;
```

### Comparing `qoqo-1.6.0a1/local_dependencies/roqoqo/src/measurements/basis_rotation_measurement.rs` & `qoqo-1.6.0a2/local_dependencies/roqoqo/src/measurements/basis_rotation_measurement.rs`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 use super::*;
 use ndarray::{Array1, Array2};
 #[cfg(feature = "serialize")]
 use serde::{Deserialize, Serialize};
 
 /// Collected information for executing a measurement of PauliZ product.
 #[derive(Debug, PartialEq, Clone)]
-// #[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
+#[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
 #[cfg_attr(feature = "serialize", derive(Serialize, Deserialize))]
 pub struct PauliZProduct {
     /// Constant Circuit that is executed before each Circuit in circuits.
     pub constant_circuit: Option<Circuit>,
     /// Collection of quantum circuits for the separate basis rotations.
     pub circuits: Vec<Circuit>,
     /// Additional input information required for measurement.
```

### Comparing `qoqo-1.6.0a1/local_dependencies/roqoqo/src/measurements/cheated_basis_rotation_measurement.rs` & `qoqo-1.6.0a2/local_dependencies/roqoqo/src/measurements/cheated_basis_rotation_measurement.rs`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 use super::*;
 use ndarray::Array1;
 #[cfg(feature = "serialize")]
 use serde::{Deserialize, Serialize};
 
 /// Collected information for executing a cheated measurement of a PauliZ product.
 #[derive(Debug, PartialEq, Clone)]
-// #[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
+#[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
 #[cfg_attr(feature = "serialize", derive(Serialize, Deserialize))]
 pub struct CheatedPauliZProduct {
     /// Constant Circuit that is executed before each Circuit in circuits.
     pub constant_circuit: Option<Circuit>,
     /// Collection of quantum circuits for the separate basis rotations.
     pub circuits: Vec<Circuit>,
     /// Additional input information required for measurement.
```

### Comparing `qoqo-1.6.0a1/local_dependencies/roqoqo/src/measurements/cheated_measurement.rs` & `qoqo-1.6.0a2/local_dependencies/roqoqo/src/measurements/cheated_measurement.rs`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 /// Cheated measurement using state obtained from simulator backend.
 ///
 /// Cheated measurements are only possible witch simulator backends that can return the state vector or the density matrix of the quantum computer.
 /// The expectation values are defined by a matrix representation of the measured observables.
 #[derive(Debug, PartialEq, Clone)]
 #[cfg_attr(feature = "serialize", derive(serde::Serialize, serde::Deserialize))]
-// #[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
+#[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
 pub struct Cheated {
     /// Constant Circuit that is executed before each Circuit in circuits.
     pub constant_circuit: Option<Circuit>,
     /// Collection of quantum circuits for the separate basis rotations.
     pub circuits: Vec<Circuit>,
     /// Additional input information required for measurement.
     pub input: CheatedInput,
```

### Comparing `qoqo-1.6.0a1/local_dependencies/roqoqo/src/measurements/classical_register_measurement.rs` & `qoqo-1.6.0a2/local_dependencies/roqoqo/src/measurements/classical_register_measurement.rs`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 use crate::RoqoqoError;
 use std::collections::HashMap;
 
 /// Classical register measurement.
 ///
 /// Runs a sequence of circuits and returns the classical registers written during circuit execution.
 #[derive(Debug, PartialEq, Clone)]
-// #[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
+#[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
 #[cfg_attr(feature = "serialize", derive(serde::Serialize, serde::Deserialize))]
 pub struct ClassicalRegister {
     /// Constant Circuit that is executed before each Circuit in circuits.
     pub constant_circuit: Option<Circuit>,
     /// Collection of quantum circuits for the separate basis rotations.
     pub circuits: Vec<Circuit>,
 }
```

### Comparing `qoqo-1.6.0a1/local_dependencies/roqoqo/src/measurements/measurement_auxiliary_data_input.rs` & `qoqo-1.6.0a2/local_dependencies/roqoqo/src/measurements/measurement_auxiliary_data_input.rs`

 * *Files 4% similar despite different names*

```diff
@@ -7,27 +7,29 @@
 //
 // Unless required by applicable law or agreed to in writing, software distributed under the
 // License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either
 // express or implied. See the License for the specific language governing permissions and
 // limitations under the License.
 
 use crate::CalculatorFloat;
+#[cfg(feature = "json_schema")]
+use crate::Complex64Def;
 use crate::RoqoqoError;
 use num_complex::Complex64;
 use std::collections::HashMap;
 
 /// Provides PauliProductMasks for all Pauli Products measured from one readout register.
 pub type SingleReadoutPauliProductMasks = HashMap<usize, PauliProductMask>;
 
 /// Provides Mask for a single PauliProduct.
 pub type PauliProductMask = Vec<usize>;
 
 /// Defines how Pauli Products expectation values are post-processed into observable expectation value.
 #[derive(Debug, Clone, PartialEq)]
-// #[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
+#[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
 #[cfg_attr(feature = "serialize", derive(serde::Serialize, serde::Deserialize))]
 pub enum PauliProductsToExpVal {
     /// Expectation value of observable is a linear combination of Pauli Product expectation values.
     ///
     /// Only scalar real expectation values are supported.  
     /// For complex observables or vector/matrix observables
     /// components have to be postprocessed separately.
@@ -42,15 +44,15 @@
 
 /// Provides Necessary Information to run a [crate::measurements::PauliZProduct] measurement.
 ///
 /// PauliZProductInput is the input struct for a PauliZProduct measurement, dictating which expectation
 /// values are measured by PauliZProduct. These expecation values are defined as
 /// expectation values of pauli products.
 #[derive(Debug, Clone, PartialEq)]
-// #[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
+#[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
 #[cfg_attr(feature = "serialize", derive(serde::Serialize, serde::Deserialize))]
 pub struct PauliZProductInput {
     /// Collection of PauliProductMasks for each readout register in Measurement.
     pub pauli_product_qubit_masks: HashMap<String, SingleReadoutPauliProductMasks>,
     /// Number of qubits that are measured.
     pub number_qubits: usize,
     /// Number of Pauli Products that are measured.
@@ -199,15 +201,15 @@
 }
 
 /// Provides necessary information to run a [crate::measurements::CheatedPauliZProduct] measurement.
 ///
 /// Is used by the full measurement struct [crate::measurements::CheatedPauliZProduct].
 #[derive(Debug, Clone, PartialEq)]
 #[cfg_attr(feature = "serialize", derive(serde::Serialize, serde::Deserialize))]
-// #[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
+#[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
 pub struct CheatedPauliZProductInput {
     /// Collection of names and construction methods of  expectation values.
     ///
     /// The construction methods are given by [PauliProductsToExpVal] enums.
     pub measured_exp_vals: HashMap<String, PauliProductsToExpVal>,
     /// Mapping the pauli product indices to the readout keys.
     pub pauli_product_keys: HashMap<String, usize>,
@@ -319,22 +321,42 @@
 }
 
 /// Provides necessary information to run a [crate::measurements::Cheated] measurement.
 ///
 /// Is used by the full measurement struct [crate::measurements::Cheated].
 #[derive(Debug, Clone, PartialEq)]
 #[cfg_attr(feature = "serialize", derive(serde::Serialize, serde::Deserialize))]
-// #[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
 pub struct CheatedInput {
     /// Map of expectation values and corresponding operator Matrices on the Hilbert Space.
     pub measured_operators: HashMap<String, (OperatorSparseVec, String)>,
     /// Number of qubits that defines the dimension of the Hilbertspace.
     pub number_qubits: usize,
 }
 
+#[cfg(feature = "json_schema")]
+impl schemars::JsonSchema for CheatedInput {
+    fn schema_name() -> String {
+        "CheatedInput".to_string()
+    }
+
+    fn json_schema(gen: &mut schemars::gen::SchemaGenerator) -> schemars::schema::Schema {
+        <SchemaHelperCheatedInput>::json_schema(gen)
+    }
+}
+
+#[cfg(feature = "json_schema")]
+#[derive(schemars::JsonSchema)]
+#[allow(dead_code, clippy::type_complexity)]
+struct SchemaHelperCheatedInput {
+    /// Map of expectation values and corresponding operator Matrices on the Hilbert Space.
+    measured_operators: HashMap<String, (Vec<(usize, usize, Complex64Def)>, String)>,
+    /// Number of qubits that defines the dimension of the Hilbertspace.
+    number_qubits: usize,
+}
+
 /// Represents Operator acting on Hilbert space as a sparse list of two indices and a value.
 ///
 /// The vector contains the triplets of non-zero elements of the sparse matrix
 /// representing the operator on the Hilbert space.
 /// The first element is the row index, the second the column index and the last the
 /// complex value of the non-zero entry.
 pub type OperatorSparseVec = Vec<(usize, usize, Complex64)>;
```

### Comparing `qoqo-1.6.0a1/local_dependencies/roqoqo/src/measurements/mod.rs` & `qoqo-1.6.0a2/local_dependencies/roqoqo/src/measurements/mod.rs`

 * *Files identical despite different names*

### Comparing `qoqo-1.6.0a1/local_dependencies/roqoqo/src/operations/bosonic_operations.rs` & `qoqo-1.6.0a2/local_dependencies/roqoqo/src/operations/bosonic_operations.rs`

 * *Files 9% similar despite different names*

```diff
@@ -35,14 +35,15 @@
     roqoqo_derive::Operate,
     roqoqo_derive::Substitute,
     roqoqo_derive::InvolveModes,
     roqoqo_derive::SubstituteModes,
     roqoqo_derive::OperateSingleMode,
 )]
 #[cfg_attr(feature = "serialize", derive(serde::Serialize, serde::Deserialize))]
+#[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
 pub struct Squeezing {
     /// The mode the squeezing gate is applied to.
     mode: usize,
     /// The coefficient of the squeezing operation.
     squeezing: CalculatorFloat,
     /// The squeezing phase angle of the squeezing operation.
     phase: CalculatorFloat,
@@ -84,14 +85,15 @@
     roqoqo_derive::Operate,
     roqoqo_derive::Substitute,
     roqoqo_derive::InvolveModes,
     roqoqo_derive::SubstituteModes,
     roqoqo_derive::OperateSingleMode,
 )]
 #[cfg_attr(feature = "serialize", derive(serde::Serialize, serde::Deserialize))]
+#[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
 pub struct PhaseShift {
     /// The mode the phase-shift gate is applied to.
     mode: usize,
     /// The phase by which to shift the mode.
     phase: CalculatorFloat,
 }
 
@@ -129,14 +131,15 @@
     roqoqo_derive::Operate,
     roqoqo_derive::Substitute,
     roqoqo_derive::InvolveModes,
     roqoqo_derive::SubstituteModes,
     roqoqo_derive::OperateTwoMode,
 )]
 #[cfg_attr(feature = "serialize", derive(serde::Serialize, serde::Deserialize))]
+#[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
 pub struct BeamSplitter {
     /// The first mode the beam-splitter is applied to.
     mode_0: usize,
     /// The second mode the beam-splitter is applied to.
     mode_1: usize,
     /// The transmittivity angle of the beam-splitter.
     theta: CalculatorFloat,
@@ -179,14 +182,15 @@
     roqoqo_derive::Operate,
     roqoqo_derive::Substitute,
     roqoqo_derive::InvolveModes,
     roqoqo_derive::SubstituteModes,
     roqoqo_derive::OperateSingleMode,
 )]
 #[cfg_attr(feature = "serialize", derive(serde::Serialize, serde::Deserialize))]
+#[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
 pub struct PhotonDetection {
     /// The mode the detector (measurement) is applied to.
     mode: usize,
     /// The register for the readout.
     readout: String,
     /// The index in the readout the result is saved to.
     readout_index: usize,
```

### Comparing `qoqo-1.6.0a1/local_dependencies/roqoqo/src/operations/define_operations.rs` & `qoqo-1.6.0a2/local_dependencies/roqoqo/src/operations/define_operations.rs`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     Eq,
     roqoqo_derive::SupportedVersion,
     roqoqo_derive::Operate,
     roqoqo_derive::Substitute,
     roqoqo_derive::Define,
 )]
 #[cfg_attr(feature = "serialize", derive(serde::Serialize, serde::Deserialize))]
-// #[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
+#[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
 pub struct DefinitionFloat {
     /// The name of the register that is defined.
     name: String,
     /// The length of the register that is defined, usually the number of qubits to be measured.
     length: usize,
     /// True/False if the variable is an output to the program.
     is_output: bool,
@@ -82,15 +82,15 @@
     Eq,
     roqoqo_derive::SupportedVersion,
     roqoqo_derive::Operate,
     roqoqo_derive::Substitute,
     roqoqo_derive::Define,
 )]
 #[cfg_attr(feature = "serialize", derive(serde::Serialize, serde::Deserialize))]
-// #[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
+#[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
 
 pub struct DefinitionComplex {
     /// The name of the register that is defined.
     name: String,
     /// The length of the register that is defined, usually the number of qubits to be measured.
     length: usize,
     /// True/False if the variable is an output to the program.
@@ -122,15 +122,15 @@
     Eq,
     roqoqo_derive::SupportedVersion,
     roqoqo_derive::Operate,
     roqoqo_derive::Substitute,
     roqoqo_derive::Define,
 )]
 #[cfg_attr(feature = "serialize", derive(serde::Serialize, serde::Deserialize))]
-// #[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
+#[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
 pub struct DefinitionUsize {
     /// The name of the register that is defined.
     name: String,
     /// The length of the register that is defined, usually the number of qubits to be measured.
     length: usize,
     /// True/False if the variable is an output to the program.
     is_output: bool,
@@ -160,15 +160,15 @@
     Eq,
     roqoqo_derive::SupportedVersion,
     roqoqo_derive::Operate,
     roqoqo_derive::Substitute,
     roqoqo_derive::Define,
 )]
 #[cfg_attr(feature = "serialize", derive(serde::Serialize, serde::Deserialize))]
-// #[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
+#[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
 pub struct DefinitionBit {
     /// The name of the register that is defined.
     name: String,
     /// The length of the register that is defined, usually the number of qubits to be measured.
     length: usize,
     /// True/False if the variable is an output to the program.
     is_output: bool,
@@ -197,15 +197,15 @@
     PartialEq,
     roqoqo_derive::SupportedVersion,
     roqoqo_derive::Operate,
     roqoqo_derive::Substitute,
     roqoqo_derive::Define,
 )]
 #[cfg_attr(feature = "serialize", derive(serde::Serialize, serde::Deserialize))]
-// #[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
+#[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
 pub struct InputSymbolic {
     /// The name of the register that is defined.
     name: String,
     /// The floating point type value by which to replace the quantities marked as "name".
     input: f64,
 }
 
@@ -234,15 +234,15 @@
     PartialEq,
     Eq,
     roqoqo_derive::Operate,
     roqoqo_derive::Substitute,
     roqoqo_derive::Define,
 )]
 #[cfg_attr(feature = "serialize", derive(serde::Serialize, serde::Deserialize))]
-// #[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
+#[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
 pub struct InputBit {
     /// The name of the register that where the bit is set.
     name: String,
     /// The index in the register that is set.
     index: usize,
     /// The value the bit is set to
     value: bool,
```

### Comparing `qoqo-1.6.0a1/local_dependencies/roqoqo/src/operations/measurement_operations.rs` & `qoqo-1.6.0a2/local_dependencies/roqoqo/src/operations/measurement_operations.rs`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     Eq,
     roqoqo_derive::SupportedVersion,
     roqoqo_derive::Operate,
     roqoqo_derive::Substitute,
     roqoqo_derive::OperateSingleQubit,
 )]
 #[cfg_attr(feature = "serialize", derive(serde::Serialize, serde::Deserialize))]
-// #[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
+#[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
 pub struct MeasureQubit {
     /// The measured qubit.
     qubit: usize,
     /// The register for the readout.
     readout: String,
     /// The index in the readout the result is saved to.
     readout_index: usize,
@@ -78,15 +78,15 @@
     Clone,
     PartialEq,
     roqoqo_derive::SupportedVersion,
     roqoqo_derive::Operate,
     roqoqo_derive::OperatePragma,
 )]
 #[cfg_attr(feature = "serialize", derive(serde::Serialize, serde::Deserialize))]
-// #[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
+#[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
 pub struct PragmaGetStateVector {
     /// The name of the classical readout register.
     readout: String,
     /// The measurement preparation Circuit, applied on a copy of the register before measurement (None if not defined, Some(Circuit) otherwise).
     circuit: Option<Circuit>,
 }
 
@@ -138,15 +138,15 @@
     Clone,
     PartialEq,
     roqoqo_derive::SupportedVersion,
     roqoqo_derive::Operate,
     roqoqo_derive::OperatePragma,
 )]
 #[cfg_attr(feature = "serialize", derive(serde::Serialize, serde::Deserialize))]
-// #[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
+#[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
 pub struct PragmaGetDensityMatrix {
     /// The name of the classical readout register.
     readout: String,
     /// The measurement preparation Circuit, applied on a copy of the register before measurement (None if not defined, Some(Circuit) otherwise).
     circuit: Option<Circuit>,
 }
 
@@ -207,15 +207,15 @@
     Clone,
     PartialEq,
     roqoqo_derive::SupportedVersion,
     roqoqo_derive::Operate,
     roqoqo_derive::OperatePragma,
 )]
 #[cfg_attr(feature = "serialize", derive(serde::Serialize, serde::Deserialize))]
-// #[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
+#[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
 pub struct PragmaGetOccupationProbability {
     /// The name of the classical readout register.
     readout: String,
     /// The measurement preparation Circuit, applied on a copy of the register before measurement (None if not defined, Some(Circuit) otherwise).
     circuit: Option<Circuit>,
 }
 
@@ -277,15 +277,15 @@
     Clone,
     PartialEq,
     roqoqo_derive::SupportedVersion,
     roqoqo_derive::Operate,
     roqoqo_derive::OperatePragma,
 )]
 #[cfg_attr(feature = "serialize", derive(serde::Serialize, serde::Deserialize))]
-// #[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
+#[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
 pub struct PragmaGetPauliProduct {
     /// The HashMap of the pauli matrix to apply to each qubit in the form {qubit: pauli}. Allowed values to be provided for 'pauli' are: `0` = identity, `1` = PauliX, `2` = PauliY, `3` = PauliZ.
     qubit_paulis: HashMap<usize, usize>,
     /// The name of the classical readout register.
     readout: String,
     /// The measurement preparation Circuit, applied on a copy of the register before measurement.
     circuit: Circuit,
@@ -360,15 +360,15 @@
     PartialEq,
     Eq,
     roqoqo_derive::SupportedVersion,
     roqoqo_derive::Operate,
     roqoqo_derive::OperatePragma,
 )]
 #[cfg_attr(feature = "serialize", derive(serde::Serialize, serde::Deserialize))]
-// #[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
+#[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
 pub struct PragmaRepeatedMeasurement {
     /// The name of the classical readout register.
     readout: String,
     /// The number of times N to repeat the measurement.
     number_measurements: usize,
     /// The mapping of qubits to indices in the readout register.
     qubit_mapping: Option<HashMap<usize, usize>>,
```

### Comparing `qoqo-1.6.0a1/local_dependencies/roqoqo/src/operations/mod.rs` & `qoqo-1.6.0a2/local_dependencies/roqoqo/src/operations/mod.rs`

 * *Files identical despite different names*

### Comparing `qoqo-1.6.0a1/local_dependencies/roqoqo/src/operations/multi_qubit_gate_operations.rs` & `qoqo-1.6.0a2/local_dependencies/roqoqo/src/operations/multi_qubit_gate_operations.rs`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     roqoqo_derive::SupportedVersion,
     roqoqo_derive::Operate,
     roqoqo_derive::Substitute,
     roqoqo_derive::OperateMultiQubit,
     roqoqo_derive::Rotate,
 )]
 #[cfg_attr(feature = "serialize", derive(Serialize, Deserialize))]
-// #[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
+#[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
 pub struct MultiQubitMS {
     /// The qubits involved in the multi qubit Molmer-Sorensen gate.
     qubits: Vec<usize>,
     /// The angle of the multi qubit Molmer-Sorensen gate.
     theta: CalculatorFloat,
 }
 
@@ -68,15 +68,14 @@
             array[(i, dim - i - 1)] = sin;
         }
         Ok(array)
     }
 }
 
 impl OperateMultiQubitGate for MultiQubitMS {
-    // Todo fill out circuit
     fn circuit(&self) -> Circuit {
         let dim = self.qubits.len();
         let mut circuit = Circuit::new();
         for q in self.qubits.iter() {
             circuit += operations::Hadamard::new(*q);
         }
         for q in self.qubits[1..].iter() {
@@ -106,15 +105,15 @@
     roqoqo_derive::SupportedVersion,
     roqoqo_derive::Operate,
     roqoqo_derive::Substitute,
     roqoqo_derive::OperateMultiQubit,
     roqoqo_derive::Rotate,
 )]
 #[cfg_attr(feature = "serialize", derive(Serialize, Deserialize))]
-// #[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
+#[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
 pub struct MultiQubitZZ {
     /// The qubits involved in the multi qubit Molmer-Sorensen gate.
     qubits: Vec<usize>,
     /// The angle of the multi qubit Molmer-Sorensen gate.
     theta: CalculatorFloat,
 }
 
@@ -144,15 +143,14 @@
             array[(i, i)] = cos + prefactor * sin;
         }
         Ok(array)
     }
 }
 
 impl OperateMultiQubitGate for MultiQubitZZ {
-    // Todo fill out circuit
     fn circuit(&self) -> Circuit {
         let dim = self.qubits.len();
         let mut circuit = Circuit::new();
         for q in self.qubits[1..].iter() {
             circuit += operations::CNOT::new(*q - 1, *q);
         }
         circuit += operations::RotateZ::new(dim - 1, self.theta.clone());
```

### Comparing `qoqo-1.6.0a1/local_dependencies/roqoqo/src/operations/pragma_operations.rs` & `qoqo-1.6.0a2/local_dependencies/roqoqo/src/operations/pragma_operations.rs`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 //!
 
 use crate::operations::{
     InvolveQubits, InvolvedQubits, Operate, OperateMultiQubit, OperatePragma, OperatePragmaNoise,
     OperatePragmaNoiseProba, OperateSingleQubit, RoqoqoError, Substitute, SupportedVersion,
 };
 use crate::Circuit;
+#[cfg(feature = "json_schema")]
+use crate::{Array1C64Def, Array2C64Def, Array2f64Def};
 #[cfg(feature = "serialize")]
 use bincode::serialize;
 use nalgebra::{matrix, Matrix4};
 use ndarray::{array, Array, Array1, Array2};
 use num_complex::Complex64;
 use qoqo_calculator::{Calculator, CalculatorFloat};
 #[cfg(feature = "serialize")]
@@ -43,15 +45,15 @@
     Eq,
     roqoqo_derive::SupportedVersion,
     roqoqo_derive::Operate,
     roqoqo_derive::Substitute,
     roqoqo_derive::OperatePragma,
 )]
 #[cfg_attr(feature = "serialize", derive(Serialize, Deserialize))]
-// #[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
+#[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
 pub struct PragmaSetNumberOfMeasurements {
     /// The number of measurements.
     number_measurements: usize,
     /// The register for the readout.
     readout: String,
 }
 
@@ -101,20 +103,39 @@
     PartialEq,
     roqoqo_derive::SupportedVersion,
     roqoqo_derive::Operate,
     roqoqo_derive::Substitute,
     roqoqo_derive::OperatePragma,
 )]
 #[cfg_attr(feature = "serialize", derive(serde::Serialize, serde::Deserialize))]
-// #[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
 pub struct PragmaSetStateVector {
     /// The statevector that is initialized.
     statevector: Array1<Complex64>,
 }
 
+#[cfg(feature = "json_schema")]
+impl schemars::JsonSchema for PragmaSetStateVector {
+    fn schema_name() -> String {
+        "PragmaSetStateVector".to_string()
+    }
+
+    fn json_schema(gen: &mut schemars::gen::SchemaGenerator) -> schemars::schema::Schema {
+        <SchemaHelperPragmaSetStateVector>::json_schema(gen)
+    }
+}
+
+#[cfg(feature = "json_schema")]
+#[derive(schemars::JsonSchema)]
+#[allow(dead_code)]
+struct SchemaHelperPragmaSetStateVector {
+    /// The statevector that is initialized.
+    #[serde(with = "Array1C64Def")]
+    statevector: Array1<Complex64>,
+}
+
 #[allow(non_upper_case_globals)]
 const TAGS_PragmaSetStateVector: &[&str; 3] =
     &["Operation", "PragmaOperation", "PragmaSetStateVector"];
 
 // Implementing the InvolveQubits trait for PragmaSetStateVector.
 impl InvolveQubits for PragmaSetStateVector {
     /// Lists all involved qubits (here, all).
@@ -149,20 +170,39 @@
     PartialEq,
     roqoqo_derive::SupportedVersion,
     roqoqo_derive::Operate,
     roqoqo_derive::Substitute,
     roqoqo_derive::OperatePragma,
 )]
 #[cfg_attr(feature = "serialize", derive(serde::Serialize, serde::Deserialize))]
-// #[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
 pub struct PragmaSetDensityMatrix {
     /// The density matrix that is initialized.
     density_matrix: Array2<Complex64>,
 }
 
+#[cfg(feature = "json_schema")]
+impl schemars::JsonSchema for PragmaSetDensityMatrix {
+    fn schema_name() -> String {
+        "PragmaSetDensityMatrix".to_string()
+    }
+
+    fn json_schema(gen: &mut schemars::gen::SchemaGenerator) -> schemars::schema::Schema {
+        <SchemaHelperPragmaSetDensityMatrix>::json_schema(gen)
+    }
+}
+
+#[cfg(feature = "json_schema")]
+#[derive(schemars::JsonSchema)]
+#[allow(dead_code)]
+struct SchemaHelperPragmaSetDensityMatrix {
+    /// The density matrix that is initialized.
+    #[serde(with = "Array2C64Def")]
+    density_matrix: Array2<Complex64>,
+}
+
 #[allow(non_upper_case_globals)]
 const TAGS_PragmaSetDensityMatrix: &[&str; 3] =
     &["Operation", "PragmaOperation", "PragmaSetDensityMatrix"];
 
 // Implementing the InvolveQubits trait for PragmaSetDensityMatrix.
 impl InvolveQubits for PragmaSetDensityMatrix {
     /// Lists all involved qubits (here, all).
@@ -182,15 +222,15 @@
     Eq,
     roqoqo_derive::SupportedVersion,
     roqoqo_derive::Operate,
     roqoqo_derive::Substitute,
     roqoqo_derive::OperatePragma,
 )]
 #[cfg_attr(feature = "serialize", derive(serde::Serialize, serde::Deserialize))]
-// #[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
+#[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
 pub struct PragmaRepeatGate {
     /// The number of times the following gate is repeated.
     repetition_coefficient: usize,
 }
 
 #[allow(non_upper_case_globals)]
 const TAGS_PragmaRepeatGate: &[&str; 3] = &["Operation", "PragmaOperation", "PragmaRepeatGate"];
@@ -220,15 +260,15 @@
     roqoqo_derive::Operate,
     roqoqo_derive::Substitute,
     roqoqo_derive::InvolveQubits,
     roqoqo_derive::OperatePragma,
     roqoqo_derive::OperateMultiQubit,
 )]
 #[cfg_attr(feature = "serialize", derive(serde::Serialize, serde::Deserialize))]
-// #[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
+#[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
 // #[cfg_attr(feature = "overrotate")]
 pub struct PragmaOverrotation {
     /// The unique hqslang name of the gate to overrotate.
     gate_hqslang: String,
     /// The qubits of the gate to overrotate.
     qubits: Vec<usize>,
     /// The amplitude the random number is multiplied by.
@@ -253,15 +293,15 @@
     PartialEq,
     roqoqo_derive::SupportedVersion,
     roqoqo_derive::Operate,
     roqoqo_derive::Substitute,
     roqoqo_derive::OperatePragma,
 )]
 #[cfg_attr(feature = "serialize", derive(serde::Serialize, serde::Deserialize))]
-// #[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
+#[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
 pub struct PragmaBoostNoise {
     /// The coefficient by which the noise is boosted, i.e. the number by which the gate time is multiplied.
     noise_coefficient: CalculatorFloat,
 }
 
 #[allow(non_upper_case_globals)]
 const TAGS_PragmaBoostNoise: &[&str; 3] = &["Operation", "PragmaOperation", "PragmaBoostNoise"];
@@ -284,15 +324,15 @@
     roqoqo_derive::SupportedVersion,
     roqoqo_derive::Operate,
     roqoqo_derive::Substitute,
     roqoqo_derive::OperateMultiQubit,
     roqoqo_derive::OperatePragma,
 )]
 #[cfg_attr(feature = "serialize", derive(serde::Serialize, serde::Deserialize))]
-// #[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
+#[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
 pub struct PragmaStopParallelBlock {
     /// The qubits involved in parallel execution block.
     qubits: Vec<usize>,
     /// The time for the execution of the block in seconds.
     execution_time: CalculatorFloat,
 }
 
@@ -315,15 +355,15 @@
     PartialEq,
     roqoqo_derive::SupportedVersion,
     roqoqo_derive::Operate,
     roqoqo_derive::Substitute,
     roqoqo_derive::OperatePragma,
 )]
 #[cfg_attr(feature = "serialize", derive(serde::Serialize, serde::Deserialize))]
-// #[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
+#[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
 pub struct PragmaGlobalPhase {
     /// The picked up global phase.
     phase: CalculatorFloat,
 }
 
 #[allow(non_upper_case_globals)]
 const TAGS_PragmaGlobalPhase: &[&str; 3] = &["Operation", "PragmaOperation", "PragmaGlobalPhase"];
@@ -349,15 +389,15 @@
     roqoqo_derive::SupportedVersion,
     roqoqo_derive::Operate,
     roqoqo_derive::Substitute,
     roqoqo_derive::OperateMultiQubit,
     roqoqo_derive::OperatePragma,
 )]
 #[cfg_attr(feature = "serialize", derive(serde::Serialize, serde::Deserialize))]
-// #[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
+#[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
 pub struct PragmaSleep {
     /// The qubits involved in the sleep block.
     qubits: Vec<usize>,
     /// Time for the execution of the operation in seconds.
     sleep_time: CalculatorFloat,
 }
 
@@ -380,15 +420,15 @@
     roqoqo_derive::SupportedVersion,
     roqoqo_derive::Operate,
     roqoqo_derive::Substitute,
     roqoqo_derive::OperateSingleQubit,
     roqoqo_derive::OperatePragma,
 )]
 #[cfg_attr(feature = "serialize", derive(serde::Serialize, serde::Deserialize))]
-// #[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
+#[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
 pub struct PragmaActiveReset {
     /// The qubit to be reset.
     qubit: usize,
 }
 
 #[allow(non_upper_case_globals)]
 const TAGS_PragmaActiveReset: &[&str; 4] = &[
@@ -408,15 +448,15 @@
     roqoqo_derive::InvolveQubits,
     roqoqo_derive::SupportedVersion,
     roqoqo_derive::Operate,
     roqoqo_derive::OperateMultiQubit,
     roqoqo_derive::OperatePragma,
 )]
 #[cfg_attr(feature = "serialize", derive(serde::Serialize, serde::Deserialize))]
-// #[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
+#[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
 pub struct PragmaStartDecompositionBlock {
     /// The qubits involved in the decomposition block.
     qubits: Vec<usize>,
     /// The reordering dictionary of the block.
     reordering_dictionary: HashMap<usize, usize>,
 }
 
@@ -472,15 +512,15 @@
     roqoqo_derive::SupportedVersion,
     roqoqo_derive::Operate,
     roqoqo_derive::Substitute,
     roqoqo_derive::OperateMultiQubit,
     roqoqo_derive::OperatePragma,
 )]
 #[cfg_attr(feature = "serialize", derive(serde::Serialize, serde::Deserialize))]
-// #[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
+#[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
 pub struct PragmaStopDecompositionBlock {
     /// The qubits involved in the decomposition block.
     qubits: Vec<usize>,
 }
 
 #[allow(non_upper_case_globals)]
 const TAGS_PragmaStopDecompositionBlock: &[&str; 4] = &[
@@ -508,15 +548,15 @@
     roqoqo_derive::SupportedVersion,
     roqoqo_derive::Operate,
     roqoqo_derive::Substitute,
     roqoqo_derive::OperateSingleQubit,
     roqoqo_derive::OperatePragma,
 )]
 #[cfg_attr(feature = "serialize", derive(serde::Serialize, serde::Deserialize))]
-// #[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
+#[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
 pub struct PragmaDamping {
     /// The qubit on which to apply the damping.
     qubit: usize,
     /// The time (in seconds) the gate takes to be applied to the qubit on the (simulated) hardware
     gate_time: CalculatorFloat,
     /// The error rate of the damping (in 1/second).
     rate: CalculatorFloat,
@@ -579,15 +619,15 @@
     roqoqo_derive::SupportedVersion,
     roqoqo_derive::Operate,
     roqoqo_derive::Substitute,
     roqoqo_derive::OperateSingleQubit,
     roqoqo_derive::OperatePragma,
 )]
 #[cfg_attr(feature = "serialize", derive(serde::Serialize, serde::Deserialize))]
-// #[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
+#[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
 pub struct PragmaDepolarising {
     /// The qubit on which to apply the depolarising.
     qubit: usize,
     /// The time (in seconds) the gate takes to be applied to the qubit on the (simulated) hardware
     gate_time: CalculatorFloat,
     /// The error rate of the depolarisation (in 1/second).
     rate: CalculatorFloat,
@@ -647,15 +687,15 @@
     roqoqo_derive::SupportedVersion,
     roqoqo_derive::Operate,
     roqoqo_derive::Substitute,
     roqoqo_derive::OperateSingleQubit,
     roqoqo_derive::OperatePragma,
 )]
 #[cfg_attr(feature = "serialize", derive(serde::Serialize, serde::Deserialize))]
-// #[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
+#[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
 pub struct PragmaDephasing {
     /// The qubit on which to apply the dephasing.
     qubit: usize,
     /// The time (in seconds) the gate takes to be applied to the qubit on the (simulated) hardware
     gate_time: CalculatorFloat,
     /// The error rate of the dephasing (in 1/second).
     rate: CalculatorFloat,
@@ -719,15 +759,15 @@
     roqoqo_derive::SupportedVersion,
     roqoqo_derive::Operate,
     roqoqo_derive::Substitute,
     roqoqo_derive::OperateSingleQubit,
     roqoqo_derive::OperatePragma,
 )]
 #[cfg_attr(feature = "serialize", derive(serde::Serialize, serde::Deserialize))]
-// #[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
+#[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
 pub struct PragmaRandomNoise {
     /// The qubit the PRAGMA Operation is applied to.
     qubit: usize,
     /// The time (in seconds) the gate takes to be applied to the qubit on the (simulated) hardware
     gate_time: CalculatorFloat,
     /// The error rate of the depolarisation (in 1/second).
     depolarising_rate: CalculatorFloat,
@@ -841,24 +881,47 @@
     roqoqo_derive::SupportedVersion,
     roqoqo_derive::Operate,
     roqoqo_derive::Substitute,
     roqoqo_derive::OperateSingleQubit,
     roqoqo_derive::OperatePragma,
 )]
 #[cfg_attr(feature = "serialize", derive(serde::Serialize, serde::Deserialize))]
-// #[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
 pub struct PragmaGeneralNoise {
     /// The qubit the PRAGMA Operation is applied to.
     qubit: usize,
     /// The time (in seconds) the gate takes to be applied to the qubit on the (simulated) hardware
     gate_time: CalculatorFloat,
     /// The rates representing the general noise matrix M (a 3x3 matrix).
     rates: Array2<f64>,
 }
 
+#[cfg(feature = "json_schema")]
+impl schemars::JsonSchema for PragmaGeneralNoise {
+    fn schema_name() -> String {
+        "PragmaGeneralNoise".to_string()
+    }
+
+    fn json_schema(gen: &mut schemars::gen::SchemaGenerator) -> schemars::schema::Schema {
+        <SchemaHelperPragmaGeneralNoise>::json_schema(gen)
+    }
+}
+
+#[cfg(feature = "json_schema")]
+#[derive(schemars::JsonSchema)]
+#[allow(dead_code)]
+struct SchemaHelperPragmaGeneralNoise {
+    /// The qubit the PRAGMA Operation is applied to.
+    qubit: usize,
+    /// The time (in seconds) the gate takes to be applied to the qubit on the (simulated) hardware
+    gate_time: CalculatorFloat,
+    /// The rates representing the general noise matrix M (a 3x3 matrix).
+    #[serde(with = "Array2f64Def")]
+    rates: Array2<f64>,
+}
+
 #[allow(non_upper_case_globals)]
 const TAGS_PragmaGeneralNoise: &[&str; 5] = &[
     "Operation",
     "SingleQubitOperation",
     "PragmaOperation",
     "PragmaNoiseOperation",
     "PragmaGeneralNoise",
@@ -979,15 +1042,15 @@
     Clone,
     PartialEq,
     roqoqo_derive::SupportedVersion,
     roqoqo_derive::Operate,
     roqoqo_derive::OperatePragma,
 )]
 #[cfg_attr(feature = "serialize", derive(serde::Serialize, serde::Deserialize))]
-// #[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
+#[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
 pub struct PragmaConditional {
     /// The name of the [crate::registers::BitRegister] containting the condition bool value.
     condition_register: String,
     /// The index in the [crate::registers::BitRegister] containting the condition bool value.
     condition_index: usize,
     /// The circuit executed if the condition is met.
     circuit: Circuit,
@@ -1038,15 +1101,15 @@
 /// The circuit is applied when the qubit is in state 1.
 /// Note that this is a unitary operation (for example a CNOT(0,1)
 /// is equvalent to a PragmaControlledCircuit(0, [PauliX(1)]) but it cannot be represented
 /// by a unitary operation in qoqo for arbitraty circuits.
 ///
 #[derive(Debug, Clone, PartialEq, roqoqo_derive::Operate, roqoqo_derive::OperatePragma)]
 #[cfg_attr(feature = "serialize", derive(serde::Serialize, serde::Deserialize))]
-// #[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
+#[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
 pub struct PragmaControlledCircuit {
     /// The qubit controlling if the circuit is applied. Circuit is applied for qubit in state 1.
     controlling_qubit: usize,
     /// The circuit executed if the condition is met.
     circuit: Circuit,
 }
 
@@ -1122,15 +1185,15 @@
 ///
 /// Since this PRAGMA uses serde and bincode to store a representation of the wrapped
 /// operation internally it is only available when roqoqo is built with the `serialize` feature
 #[derive(
     Debug, Clone, PartialEq, Eq, roqoqo_derive::SupportedVersion, roqoqo_derive::OperatePragma,
 )]
 #[cfg_attr(feature = "serialize", derive(serde::Serialize, serde::Deserialize))]
-// #[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
+#[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
 pub struct PragmaChangeDevice {
     /// The tags of the wrapped operation.
     pub wrapped_tags: Vec<String>,
     /// The hqslang name of the wrapped operation.
     pub wrapped_hqslang: String,
     /// Binary representation of the wrapped operation using serde and bincode.
     pub wrapped_operation: Vec<u8>,
@@ -1200,15 +1263,15 @@
     }
 }
 
 /// This PRAGMA repeats a circuit .
 ///
 #[derive(Debug, Clone, PartialEq, roqoqo_derive::Operate, roqoqo_derive::OperatePragma)]
 #[cfg_attr(feature = "serialize", derive(serde::Serialize, serde::Deserialize))]
-// #[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
+#[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
 pub struct PragmaLoop {
     /// The name of the classical readout register.
     repetitions: CalculatorFloat,
     /// The Circuit that is looped.
     circuit: Circuit,
 }
 impl super::ImplementedIn1point1 for PragmaLoop {}
```

### Comparing `qoqo-1.6.0a1/local_dependencies/roqoqo/src/operations/single_qubit_gate_operations.rs` & `qoqo-1.6.0a2/local_dependencies/roqoqo/src/operations/single_qubit_gate_operations.rs`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     roqoqo_derive::InvolveQubits,
     roqoqo_derive::SupportedVersion,
     roqoqo_derive::Operate,
     roqoqo_derive::Substitute,
     roqoqo_derive::OperateSingleQubit,
 )]
 #[cfg_attr(feature = "serialize", derive(serde::Serialize, serde::Deserialize))]
-// #[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
+#[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
 pub struct SingleQubitGate {
     /// The qubit the unitary gate is applied to.
     qubit: usize,
     /// The real part Re(α) of the on-diagonal elements of the single-qubit unitary.
     alpha_r: CalculatorFloat,
     /// The imaginary part Im(α) of the on-diagonal elements of the single-qubit unitary.
     alpha_i: CalculatorFloat,
@@ -165,15 +165,15 @@
     roqoqo_derive::SupportedVersion,
     roqoqo_derive::Operate,
     roqoqo_derive::Substitute,
     roqoqo_derive::OperateSingleQubit,
     roqoqo_derive::Rotate,
 )]
 #[cfg_attr(feature = "serialize", derive(serde::Serialize, serde::Deserialize))]
-// #[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
+#[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
 pub struct RotateZ {
     /// The qubit the unitary gate is applied to.
     qubit: usize,
     /// The angle θ of the rotation, in the interval from 0 to 2 * 2π.
     theta: CalculatorFloat,
 }
 
@@ -262,15 +262,15 @@
     roqoqo_derive::SupportedVersion,
     roqoqo_derive::Operate,
     roqoqo_derive::Substitute,
     roqoqo_derive::OperateSingleQubit,
     roqoqo_derive::Rotate,
 )]
 #[cfg_attr(feature = "serialize", derive(serde::Serialize, serde::Deserialize))]
-// #[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
+#[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
 pub struct RotateX {
     /// The qubit the unitary gate is applied to.
     qubit: usize,
     /// The angle θ of the rotation, in the interval from 0 to 2 * 2π.
     theta: CalculatorFloat,
 }
 #[allow(non_upper_case_globals)]
@@ -354,15 +354,15 @@
     roqoqo_derive::SupportedVersion,
     roqoqo_derive::Operate,
     roqoqo_derive::Substitute,
     roqoqo_derive::OperateSingleQubit,
     roqoqo_derive::Rotate,
 )]
 #[cfg_attr(feature = "serialize", derive(serde::Serialize, serde::Deserialize))]
-// #[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
+#[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
 pub struct RotateY {
     /// The qubit the unitary gate is applied to.
     qubit: usize,
     /// The angle θ of the rotation, in the interval from 0 to 2 * 2π.
     theta: CalculatorFloat,
 }
 #[allow(non_upper_case_globals)]
@@ -446,15 +446,15 @@
     roqoqo_derive::InvolveQubits,
     roqoqo_derive::SupportedVersion,
     roqoqo_derive::Operate,
     roqoqo_derive::Substitute,
     roqoqo_derive::OperateSingleQubit,
 )]
 #[cfg_attr(feature = "serialize", derive(serde::Serialize, serde::Deserialize))]
-// #[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
+#[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
 pub struct PauliX {
     /// The qubit the unitary gate is applied to.
     qubit: usize,
 }
 
 #[allow(non_upper_case_globals)]
 const TAGS_PauliX: &[&str; 4] = &[
@@ -534,15 +534,15 @@
     roqoqo_derive::InvolveQubits,
     roqoqo_derive::SupportedVersion,
     roqoqo_derive::Operate,
     roqoqo_derive::Substitute,
     roqoqo_derive::OperateSingleQubit,
 )]
 #[cfg_attr(feature = "serialize", derive(serde::Serialize, serde::Deserialize))]
-// #[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
+#[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
 pub struct PauliY {
     /// The qubit the unitary gate is applied to.
     qubit: usize,
 }
 
 #[allow(non_upper_case_globals)]
 const TAGS_PauliY: &[&str; 4] = &[
@@ -622,15 +622,15 @@
     roqoqo_derive::InvolveQubits,
     roqoqo_derive::SupportedVersion,
     roqoqo_derive::Operate,
     roqoqo_derive::Substitute,
     roqoqo_derive::OperateSingleQubit,
 )]
 #[cfg_attr(feature = "serialize", derive(serde::Serialize, serde::Deserialize))]
-// #[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
+#[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
 pub struct PauliZ {
     /// The qubit the unitary gate is applied to.
     qubit: usize,
 }
 
 #[allow(non_upper_case_globals)]
 const TAGS_PauliZ: &[&str; 4] = &[
@@ -710,15 +710,15 @@
     roqoqo_derive::InvolveQubits,
     roqoqo_derive::SupportedVersion,
     roqoqo_derive::Operate,
     roqoqo_derive::Substitute,
     roqoqo_derive::OperateSingleQubit,
 )]
 #[cfg_attr(feature = "serialize", derive(serde::Serialize, serde::Deserialize))]
-// #[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
+#[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
 pub struct SqrtPauliX {
     /// The qubit the unitary gate is applied to.
     qubit: usize,
 }
 
 #[allow(non_upper_case_globals)]
 const TAGS_SqrtPauliX: &[&str; 4] = &[
@@ -801,15 +801,15 @@
     roqoqo_derive::InvolveQubits,
     roqoqo_derive::SupportedVersion,
     roqoqo_derive::Operate,
     roqoqo_derive::Substitute,
     roqoqo_derive::OperateSingleQubit,
 )]
 #[cfg_attr(feature = "serialize", derive(serde::Serialize, serde::Deserialize))]
-// #[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
+#[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
 pub struct InvSqrtPauliX {
     /// The qubit the unitary gate is applied to.
     qubit: usize,
 }
 
 #[allow(non_upper_case_globals)]
 const TAGS_InvSqrtPauliX: &[&str; 4] = &[
@@ -892,15 +892,15 @@
     roqoqo_derive::InvolveQubits,
     roqoqo_derive::SupportedVersion,
     roqoqo_derive::Operate,
     roqoqo_derive::Substitute,
     roqoqo_derive::OperateSingleQubit,
 )]
 #[cfg_attr(feature = "serialize", derive(serde::Serialize, serde::Deserialize))]
-// #[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
+#[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
 pub struct Hadamard {
     /// The qubit the unitary gate is applied to.
     qubit: usize,
 }
 
 #[allow(non_upper_case_globals)]
 const TAGS_Hadamard: &[&str; 4] = &[
@@ -981,15 +981,15 @@
     roqoqo_derive::InvolveQubits,
     roqoqo_derive::SupportedVersion,
     roqoqo_derive::Operate,
     roqoqo_derive::Substitute,
     roqoqo_derive::OperateSingleQubit,
 )]
 #[cfg_attr(feature = "serialize", derive(serde::Serialize, serde::Deserialize))]
-// #[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
+#[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
 pub struct SGate {
     /// The qubit the unitary gate is applied to.
     qubit: usize,
 }
 
 #[allow(non_upper_case_globals)]
 const TAGS_SGate: &[&str; 4] = &[
@@ -1069,15 +1069,15 @@
     roqoqo_derive::InvolveQubits,
     roqoqo_derive::SupportedVersion,
     roqoqo_derive::Operate,
     roqoqo_derive::Substitute,
     roqoqo_derive::OperateSingleQubit,
 )]
 #[cfg_attr(feature = "serialize", derive(serde::Serialize, serde::Deserialize))]
-// #[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
+#[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
 pub struct TGate {
     /// The qubit the unitary gate is applied to.
     qubit: usize,
 }
 
 #[allow(non_upper_case_globals)]
 const TAGS_TGate: &[&str; 4] = &[
@@ -1162,15 +1162,15 @@
     roqoqo_derive::SupportedVersion,
     roqoqo_derive::Operate,
     roqoqo_derive::Substitute,
     roqoqo_derive::OperateSingleQubit,
     roqoqo_derive::Rotate,
 )]
 #[cfg_attr(feature = "serialize", derive(serde::Serialize, serde::Deserialize))]
-// #[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
+#[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
 pub struct PhaseShiftState1 {
     /// The qubit the unitary gate is applied to.
     qubit: usize,
     /// The angle θ of the rotation, in the interval from 0 to 2π.
     theta: CalculatorFloat,
 }
 
@@ -1259,15 +1259,15 @@
     roqoqo_derive::SupportedVersion,
     roqoqo_derive::Operate,
     roqoqo_derive::Substitute,
     roqoqo_derive::OperateSingleQubit,
     roqoqo_derive::Rotate,
 )]
 #[cfg_attr(feature = "serialize", derive(serde::Serialize, serde::Deserialize))]
-// #[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
+#[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
 pub struct PhaseShiftState0 {
     /// The qubit the unitary gate is applied to.
     qubit: usize,
     /// The angle θ of the rotation, in the interval from 0 to 2π.
     theta: CalculatorFloat,
 }
 
@@ -1354,15 +1354,15 @@
     roqoqo_derive::SupportedVersion,
     roqoqo_derive::Operate,
     roqoqo_derive::Substitute,
     roqoqo_derive::OperateSingleQubit,
     roqoqo_derive::Rotate,
 )]
 #[cfg_attr(feature = "serialize", derive(serde::Serialize, serde::Deserialize))]
-// #[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
+#[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
 pub struct RotateAroundSphericalAxis {
     /// The qubit the unitary gate is applied to.
     qubit: usize,
     /// The angle θ of the rotation, in the interval from 0 to 2 * 2π.
     theta: CalculatorFloat,
     /// The rotation axis, unit-vector spherical coordinates θ_{sph}.
     spherical_theta: CalculatorFloat,
@@ -1470,15 +1470,15 @@
     roqoqo_derive::SupportedVersion,
     roqoqo_derive::Operate,
     roqoqo_derive::Substitute,
     roqoqo_derive::OperateSingleQubit,
     roqoqo_derive::Rotate,
 )]
 #[cfg_attr(feature = "serialize", derive(serde::Serialize, serde::Deserialize))]
-// #[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
+#[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
 pub struct RotateXY {
     /// The qubit the unitary gate is applied to.
     qubit: usize,
     /// The angle θ of the rotation, in the interval from 0 to 2 * 2π.
     theta: CalculatorFloat,
     /// The rotation axis, in spherical coordinates φ gives the angle in the x-y plane.
     phi: CalculatorFloat,
@@ -1576,14 +1576,15 @@
     roqoqo_derive::InvolveQubits,
     roqoqo_derive::Operate,
     roqoqo_derive::Substitute,
     roqoqo_derive::OperateSingleQubit,
     roqoqo_derive::Rotate,
 )]
 #[cfg_attr(feature = "serialize", derive(serde::Serialize, serde::Deserialize))]
+#[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
 pub struct GPi {
     /// The qubit the unitary gate is applied to.
     qubit: usize,
     /// The rotation axis, in spherical coordinates φ gives the angle in the x-y plane.
     theta: CalculatorFloat,
 }
 
@@ -1675,15 +1676,15 @@
     roqoqo_derive::InvolveQubits,
     roqoqo_derive::Operate,
     roqoqo_derive::Substitute,
     roqoqo_derive::OperateSingleQubit,
     roqoqo_derive::Rotate,
 )]
 #[cfg_attr(feature = "serialize", derive(serde::Serialize, serde::Deserialize))]
-// #[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
+#[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
 pub struct GPi2 {
     /// The qubit the unitary gate is applied to.
     qubit: usize,
     /// The rotation axis, in spherical coordinates φ gives the angle in the x-y plane.
     theta: CalculatorFloat,
 }
 impl super::ImplementedIn1point4 for GPi2 {}
```

### Comparing `qoqo-1.6.0a1/local_dependencies/roqoqo/src/operations/three_qubit_gate_operations.rs` & `qoqo-1.6.0a2/local_dependencies/roqoqo/src/operations/three_qubit_gate_operations.rs`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     Eq,
     roqoqo_derive::InvolveQubits,
     roqoqo_derive::Operate,
     roqoqo_derive::Substitute,
     roqoqo_derive::OperateThreeQubit,
 )]
 #[cfg_attr(feature = "serialize", derive(serde::Serialize, serde::Deserialize))]
-
+#[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
 pub struct ControlledControlledPauliZ {
     /// The index of the most significant qubit in the unitary representation. Here, the first controlling qubit of the operation.
     control_0: usize,
     /// The index of the second most significant qubit in the unitary representation. Here, the second controlling qubit of the operation.
     control_1: usize,
     /// The index of the least significant qubit in the unitary representation. Here, the qubit PauliZ is applied to.
     target: usize,
@@ -185,14 +185,15 @@
     roqoqo_derive::InvolveQubits,
     roqoqo_derive::Operate,
     roqoqo_derive::Substitute,
     roqoqo_derive::OperateThreeQubit,
     roqoqo_derive::Rotate,
 )]
 #[cfg_attr(feature = "serialize", derive(serde::Serialize, serde::Deserialize))]
+#[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
 pub struct ControlledControlledPhaseShift {
     /// The index of the most significant qubit in the unitary representation. Here, the first controlling qubit of the operation.
     control_0: usize,
     /// The index of the second most significant qubit in the unitary representation. Here, the second controlling qubit of the operation.
     control_1: usize,
     /// The index of the least significant qubit in the unitary representation. Here, the qubit the phase-shift is applied to.
     target: usize,
@@ -337,14 +338,15 @@
     PartialEq,
     roqoqo_derive::InvolveQubits,
     roqoqo_derive::Operate,
     roqoqo_derive::Substitute,
     roqoqo_derive::OperateThreeQubit,
 )]
 #[cfg_attr(feature = "serialize", derive(serde::Serialize, serde::Deserialize))]
+#[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
 pub struct Toffoli {
     /// The index of the most significant qubit in the unitary representation. Here, the first controlling qubit of the operation.
     control_0: usize,
     /// The index of the second most significant qubit in the unitary representation. Here, the second controlling qubit of the operation.
     control_1: usize,
     /// The index of the least significant qubit in the unitary representation. Here, the qubit the phase-shift is applied to.
     target: usize,
```

### Comparing `qoqo-1.6.0a1/local_dependencies/roqoqo/src/operations/two_qubit_gate_operations.rs` & `qoqo-1.6.0a2/local_dependencies/roqoqo/src/operations/two_qubit_gate_operations.rs`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
     roqoqo_derive::InvolveQubits,
     roqoqo_derive::SupportedVersion,
     roqoqo_derive::Operate,
     roqoqo_derive::Substitute,
     roqoqo_derive::OperateTwoQubit,
 )]
 #[cfg_attr(feature = "serialize", derive(serde::Serialize, serde::Deserialize))]
-// #[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
+#[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
 pub struct CNOT {
     /// The index of the most significant qubit in the unitary representation. Here, the qubit that controls the application of NOT on the target qubit.
     control: usize,
     /// The index of the least significant qubit in the unitary representation. Here, the qubit NOT is applied to.
     target: usize,
 }
 
@@ -157,15 +157,15 @@
     roqoqo_derive::InvolveQubits,
     roqoqo_derive::SupportedVersion,
     roqoqo_derive::Operate,
     roqoqo_derive::Substitute,
     roqoqo_derive::OperateTwoQubit,
 )]
 #[cfg_attr(feature = "serialize", derive(serde::Serialize, serde::Deserialize))]
-// #[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
+#[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
 pub struct SWAP {
     /// The index of the most significant qubit in the unitary representation.
     control: usize,
     /// The index of the least significant qubit in the unitary representation.
     target: usize,
 }
 
@@ -249,15 +249,15 @@
     roqoqo_derive::InvolveQubits,
     roqoqo_derive::SupportedVersion,
     roqoqo_derive::Operate,
     roqoqo_derive::Substitute,
     roqoqo_derive::OperateTwoQubit,
 )]
 #[cfg_attr(feature = "serialize", derive(serde::Serialize, serde::Deserialize))]
-// #[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
+#[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
 pub struct ISwap {
     /// The index of the most significant qubit in the unitary representation.
     control: usize,
     /// The index of the least significant qubit in the unitary representation.
     target: usize,
 }
 
@@ -342,15 +342,15 @@
     roqoqo_derive::InvolveQubits,
     roqoqo_derive::SupportedVersion,
     roqoqo_derive::Operate,
     roqoqo_derive::Substitute,
     roqoqo_derive::OperateTwoQubit,
 )]
 #[cfg_attr(feature = "serialize", derive(serde::Serialize, serde::Deserialize))]
-// #[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
+#[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
 pub struct FSwap {
     /// The index of the most significant qubit in the unitary representation.
     control: usize,
     /// The index of the least significant qubit in the unitary representation.
     target: usize,
 }
 
@@ -438,15 +438,15 @@
     roqoqo_derive::InvolveQubits,
     roqoqo_derive::SupportedVersion,
     roqoqo_derive::Operate,
     roqoqo_derive::Substitute,
     roqoqo_derive::OperateTwoQubit,
 )]
 #[cfg_attr(feature = "serialize", derive(serde::Serialize, serde::Deserialize))]
-// #[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
+#[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
 pub struct SqrtISwap {
     /// The index of the most significant qubit in the unitary representation.
     control: usize,
     /// The index of the least significant qubit in the unitary representation.
     target: usize,
 }
 
@@ -530,15 +530,15 @@
     roqoqo_derive::InvolveQubits,
     roqoqo_derive::SupportedVersion,
     roqoqo_derive::Operate,
     roqoqo_derive::Substitute,
     roqoqo_derive::OperateTwoQubit,
 )]
 #[cfg_attr(feature = "serialize", derive(serde::Serialize, serde::Deserialize))]
-// #[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
+#[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
 pub struct InvSqrtISwap {
     /// The index of the most significant qubit in the unitary representation.
     control: usize,
     /// The index of the least significant qubit in the unitary representation.
     target: usize,
 }
 
@@ -624,15 +624,15 @@
     roqoqo_derive::SupportedVersion,
     roqoqo_derive::Operate,
     roqoqo_derive::Substitute,
     roqoqo_derive::OperateTwoQubit,
     roqoqo_derive::Rotate,
 )]
 #[cfg_attr(feature = "serialize", derive(serde::Serialize, serde::Deserialize))]
-// #[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
+#[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
 pub struct XY {
     /// The index of the most significant qubit in the unitary representation.
     control: usize,
     /// The index of the least significant qubit in the unitary representation.
     target: usize,
     /// The rotation angle θ.
     theta: CalculatorFloat,
@@ -722,15 +722,15 @@
     roqoqo_derive::SupportedVersion,
     roqoqo_derive::Operate,
     roqoqo_derive::Substitute,
     roqoqo_derive::OperateTwoQubit,
     roqoqo_derive::Rotate,
 )]
 #[cfg_attr(feature = "serialize", derive(serde::Serialize, serde::Deserialize))]
-// #[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
+#[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
 pub struct ControlledPhaseShift {
     /// The index of the most significant qubit in the unitary representation. Here, the qubit that controls the application of the phase-shift on the target qubit.
     control: usize,
     /// The index of the least significant qubit in the unitary representation. Here, the qubit phase-shift is applied to.
     target: usize,
     /// The rotation angle θ.
     theta: CalculatorFloat,
@@ -823,15 +823,15 @@
     roqoqo_derive::InvolveQubits,
     roqoqo_derive::SupportedVersion,
     roqoqo_derive::Operate,
     roqoqo_derive::Substitute,
     roqoqo_derive::OperateTwoQubit,
 )]
 #[cfg_attr(feature = "serialize", derive(serde::Serialize, serde::Deserialize))]
-// #[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
+#[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
 pub struct ControlledPauliY {
     /// The index of the most significant qubit in the unitary representation. Here, the qubit that controls the application of PauliY gate on the target qubit.
     control: usize,
     /// The index of the least significant qubit in the unitary representation. Here, the qubit PauliY is applied to.
     target: usize,
 }
 
@@ -922,15 +922,15 @@
     roqoqo_derive::InvolveQubits,
     roqoqo_derive::SupportedVersion,
     roqoqo_derive::Operate,
     roqoqo_derive::Substitute,
     roqoqo_derive::OperateTwoQubit,
 )]
 #[cfg_attr(feature = "serialize", derive(serde::Serialize, serde::Deserialize))]
-// #[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
+#[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
 pub struct ControlledPauliZ {
     /// The index of the most significant qubit in the unitary representation. Here, the qubit that controls the application of PauliZ gate on the target qubit.
     control: usize,
     /// The index of the least significant qubit in the unitary representation. Here, the qubit PauliZ is applied to.
     target: usize,
 }
 
@@ -1017,15 +1017,15 @@
     roqoqo_derive::InvolveQubits,
     roqoqo_derive::SupportedVersion,
     roqoqo_derive::Operate,
     roqoqo_derive::Substitute,
     roqoqo_derive::OperateTwoQubit,
 )]
 #[cfg_attr(feature = "serialize", derive(serde::Serialize, serde::Deserialize))]
-// #[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
+#[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
 pub struct MolmerSorensenXX {
     /// The index of the most significant qubit in the unitary representation. The gate is symmetric under the exchange of qubits.
     control: usize,
     /// The index of the least significant qubit in the unitary representation. The gate is symmetric under the exchange of qubits.
     target: usize,
 }
 
@@ -1109,15 +1109,15 @@
     roqoqo_derive::SupportedVersion,
     roqoqo_derive::Operate,
     roqoqo_derive::Substitute,
     roqoqo_derive::OperateTwoQubit,
     roqoqo_derive::Rotate,
 )]
 #[cfg_attr(feature = "serialize", derive(serde::Serialize, serde::Deserialize))]
-// #[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
+#[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
 pub struct VariableMSXX {
     /// The index of the most significant qubit in the unitary representation. The gate is symmetric under the exchange of qubits.
     control: usize,
     /// The index of the least significant qubit in the unitary representation. The gate is symmetric under the exchange of qubits.
     target: usize,
     /// The rotation angle θ.
     theta: CalculatorFloat,
@@ -1207,15 +1207,15 @@
     roqoqo_derive::SupportedVersion,
     roqoqo_derive::Operate,
     roqoqo_derive::Substitute,
     roqoqo_derive::OperateTwoQubit,
     roqoqo_derive::Rotate,
 )]
 #[cfg_attr(feature = "serialize", derive(serde::Serialize, serde::Deserialize))]
-// #[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
+#[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
 pub struct GivensRotation {
     /// The index of the most significant qubit in the unitary representation.
     control: usize,
     /// The index of the least significant qubit in the unitary representation.
     target: usize,
     /// The rotation angle θ.
     theta: CalculatorFloat,
@@ -1316,15 +1316,15 @@
     roqoqo_derive::SupportedVersion,
     roqoqo_derive::Operate,
     roqoqo_derive::Substitute,
     roqoqo_derive::OperateTwoQubit,
     roqoqo_derive::Rotate,
 )]
 #[cfg_attr(feature = "serialize", derive(serde::Serialize, serde::Deserialize))]
-// #[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
+#[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
 pub struct GivensRotationLittleEndian {
     /// The index of the most significant qubit in the unitary representation.
     control: usize,
     /// The index of the least significant qubit in the unitary representation.
     target: usize,
     /// The rotation angle θ.
     theta: CalculatorFloat,
@@ -1425,15 +1425,15 @@
     roqoqo_derive::InvolveQubits,
     roqoqo_derive::SupportedVersion,
     roqoqo_derive::Operate,
     roqoqo_derive::Substitute,
     roqoqo_derive::OperateTwoQubit,
 )]
 #[cfg_attr(feature = "serialize", derive(serde::Serialize, serde::Deserialize))]
-// #[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
+#[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
 pub struct Qsim {
     /// The index of the most significant qubit in the unitary representation.
     control: usize,
     /// The index of the least significant qubit in the unitary representation.
     target: usize,
     /// The prefactor of the XX interaction.
     x: CalculatorFloat,
@@ -1542,15 +1542,15 @@
     roqoqo_derive::InvolveQubits,
     roqoqo_derive::SupportedVersion,
     roqoqo_derive::Operate,
     roqoqo_derive::Substitute,
     roqoqo_derive::OperateTwoQubit,
 )]
 #[cfg_attr(feature = "serialize", derive(serde::Serialize, serde::Deserialize))]
-// #[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
+#[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
 pub struct Fsim {
     /// The index of the most significant qubit in the unitary representation.
     control: usize,
     /// The index of the least significant qubit in the unitary representation.
     target: usize,
     /// The hopping strength.
     t: CalculatorFloat,
@@ -1648,15 +1648,15 @@
     roqoqo_derive::InvolveQubits,
     roqoqo_derive::SupportedVersion,
     roqoqo_derive::Operate,
     roqoqo_derive::Substitute,
     roqoqo_derive::OperateTwoQubit,
 )]
 #[cfg_attr(feature = "serialize", derive(serde::Serialize, serde::Deserialize))]
-// #[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
+#[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
 pub struct SpinInteraction {
     /// The index of the most significant qubit in the unitary representation.
     control: usize,
     /// The index of the least significant qubit in the unitary representation.
     target: usize,
     /// The prefactor of the XX interaction.
     x: CalculatorFloat,
@@ -1761,15 +1761,15 @@
     roqoqo_derive::InvolveQubits,
     roqoqo_derive::SupportedVersion,
     roqoqo_derive::Operate,
     roqoqo_derive::Substitute,
     roqoqo_derive::OperateTwoQubit,
 )]
 #[cfg_attr(feature = "serialize", derive(serde::Serialize, serde::Deserialize))]
-// #[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
+#[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
 pub struct Bogoliubov {
     /// The index of the most significant qubit in the unitary representation.
     control: usize,
     /// The index of the least significant qubit in the unitary representation.
     target: usize,
     /// The real part of the complex Bogoliubov interaction strength Re(Δ).
     delta_real: CalculatorFloat,
@@ -1873,15 +1873,15 @@
     roqoqo_derive::InvolveQubits,
     roqoqo_derive::SupportedVersion,
     roqoqo_derive::Operate,
     roqoqo_derive::Substitute,
     roqoqo_derive::OperateTwoQubit,
 )]
 #[cfg_attr(feature = "serialize", derive(serde::Serialize, serde::Deserialize))]
-// #[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
+#[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
 pub struct PMInteraction {
     /// The index of the most significant qubit in the unitary representation.
     control: usize,
     /// The index of the least significant qubit in the unitary representation.
     target: usize,
     /// The strength of the rotation θ.
     t: CalculatorFloat,
@@ -1970,15 +1970,15 @@
     roqoqo_derive::InvolveQubits,
     roqoqo_derive::SupportedVersion,
     roqoqo_derive::Operate,
     roqoqo_derive::Substitute,
     roqoqo_derive::OperateTwoQubit,
 )]
 #[cfg_attr(feature = "serialize", derive(serde::Serialize, serde::Deserialize))]
-// #[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
+#[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
 pub struct ComplexPMInteraction {
     /// The index of the most significant qubit in the unitary representation.
     control: usize,
     /// The index of the least significant qubit in the unitary representation.
     target: usize,
     /// The real part of the strength of the rotation Re(θ).
     t_real: CalculatorFloat,
@@ -2076,15 +2076,15 @@
     roqoqo_derive::InvolveQubits,
     roqoqo_derive::SupportedVersion,
     roqoqo_derive::Operate,
     roqoqo_derive::Substitute,
     roqoqo_derive::OperateTwoQubit,
 )]
 #[cfg_attr(feature = "serialize", derive(serde::Serialize, serde::Deserialize))]
-// #[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
+#[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
 pub struct PhaseShiftedControlledZ {
     /// The index of the most significant qubit in the unitary representation. Here, the qubit that controls the application of the phase-shift on the target qubit.
     control: usize,
     /// The index of the least significant qubit in the unitary representation. Here, the qubit phase-shift is applied to.
     target: usize,
     /// The single qubit phase φ.
     phi: CalculatorFloat,
@@ -2182,15 +2182,15 @@
     roqoqo_derive::InvolveQubits,
     roqoqo_derive::Operate,
     roqoqo_derive::Substitute,
     roqoqo_derive::OperateTwoQubit,
     roqoqo_derive::Rotate,
 )]
 #[cfg_attr(feature = "serialize", derive(serde::Serialize, serde::Deserialize))]
-// #[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
+#[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
 pub struct PhaseShiftedControlledPhase {
     /// The index of the most significant qubit in the unitary representation. Here, the qubit that controls the application of the phase-shift on the target qubit.
     control: usize,
     /// The index of the least significant qubit in the unitary representation. Here, the qubit phase-shift is applied to.
     target: usize,
     /// The phase rotation θ.
     theta: CalculatorFloat,
@@ -2298,14 +2298,15 @@
     roqoqo_derive::InvolveQubits,
     roqoqo_derive::Operate,
     roqoqo_derive::Substitute,
     roqoqo_derive::OperateTwoQubit,
     roqoqo_derive::Rotate,
 )]
 #[cfg_attr(feature = "serialize", derive(serde::Serialize, serde::Deserialize))]
+#[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
 pub struct ControlledRotateX {
     /// The index of the most significant qubit in the unitary representation. Here, the qubit that controls the application of the phase-shift on the target qubit.
     control: usize,
     /// The index of the least significant qubit in the unitary representation. Here, the qubit phase-shift is applied to.
     target: usize,
     /// The angle θ of the rotation, in the interval from 0 to 2 * 2π.
     theta: CalculatorFloat,
@@ -2405,14 +2406,15 @@
     roqoqo_derive::InvolveQubits,
     roqoqo_derive::Operate,
     roqoqo_derive::Substitute,
     roqoqo_derive::OperateTwoQubit,
     roqoqo_derive::Rotate,
 )]
 #[cfg_attr(feature = "serialize", derive(serde::Serialize, serde::Deserialize))]
+#[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
 pub struct ControlledRotateXY {
     /// The index of the most significant qubit in the unitary representation. Here, the qubit that controls the application of the phase-shift on the target qubit.
     control: usize,
     /// The index of the least significant qubit in the unitary representation. Here, the qubit phase-shift is applied to.
     target: usize,
     /// The angle θ of the rotation, in the interval from 0 to 2 * 2π.
     theta: CalculatorFloat,
```

### Comparing `qoqo-1.6.0a1/local_dependencies/roqoqo/src/prelude.rs` & `qoqo-1.6.0a2/local_dependencies/roqoqo/src/prelude.rs`

 * *Files identical despite different names*

### Comparing `qoqo-1.6.0a1/local_dependencies/roqoqo/src/quantum_program.rs` & `qoqo-1.6.0a2/local_dependencies/roqoqo/src/quantum_program.rs`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 /// replace the parameters with its `run` methods and return the result.
 ///
 /// The QuantumProgram should correspond as closely as possible to a normal multi-parameter function
 /// in classical computing that can be called with a set of parameters and returns a result.
 /// It is the intended way to interface between normal program code and roqoqo based quantum programs.
 ///
 #[derive(Debug, PartialEq, Clone)]
-// #[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
+#[cfg_attr(feature = "json_schema", derive(schemars::JsonSchema))]
 #[cfg_attr(feature = "serialize", derive(serde::Serialize, serde::Deserialize))]
 #[non_exhaustive]
 pub enum QuantumProgram {
     /// Variant for basis rotation measurement based quantum programs
     PauliZProduct {
         /// The measurement that is performed
         measurement: measurements::PauliZProduct,
```

### Comparing `qoqo-1.6.0a1/local_dependencies/roqoqo/src/registers.rs` & `qoqo-1.6.0a2/local_dependencies/roqoqo/src/registers.rs`

 * *Files identical despite different names*

### Comparing `qoqo-1.6.0a1/local_dependencies/qoqo-macros/Cargo.toml` & `qoqo-1.6.0a2/local_dependencies/qoqo-macros/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "qoqo-macros"
-version = "1.6.0-alpha.1"
+version = "1.6.0-alpha.2"
 authors = ["HQS Quantum Simulations <info@quantumsimulations.de>"]
 license = "Apache-2.0"
 readme = "../README.md"
 edition = "2021"
 rust-version = "1.56"
 categories = ["science", "simulation"]
 description = "Macros for the qoqo crate"
```

### Comparing `qoqo-1.6.0a1/local_dependencies/qoqo-macros/LICENSE` & `qoqo-1.6.0a2/local_dependencies/roqoqo-derive/LICENSE`

 * *Files identical despite different names*

### Comparing `qoqo-1.6.0a1/local_dependencies/qoqo-macros/src/lib.rs` & `qoqo-1.6.0a2/local_dependencies/qoqo-macros/src/lib.rs`

 * *Files 2% similar despite different names*

```diff
@@ -522,14 +522,50 @@
         TokenStream::new()
     };
     let operate_two_mode_gate_quote = if attribute_arguments.contains("OperateTwoModeGate") {
         quote! {}
     } else {
         TokenStream::new()
     };
+    let json_schema_quote = if attribute_arguments.contains("JsonSchema") {
+        quote! {
+            #[cfg(feature = "json_schema")]
+            /// Returns the current version of the qoqo library .
+            ///
+            /// Returns:
+            ///     str: The current version of the library.
+            #[staticmethod]
+            pub fn current_version() -> String {
+                ROQOQO_VERSION.to_string()
+            }
+
+            #[cfg(feature = "json_schema")]
+            /// Return the minimum version of qoqo that supports this object.
+            ///
+            /// Returns:
+            ///     str: The minimum version of the qoqo library to deserialize this object.
+            pub fn min_supported_version(&self) -> String {
+                let min_version: (u32, u32, u32) = #ident::minimum_supported_roqoqo_version(&self.internal);
+                format!("{}.{}.{}", min_version.0, min_version.1, min_version.2)
+            }
+
+            #[cfg(feature = "json_schema")]
+            /// Return the JsonSchema for the json serialisation of the class.
+            ///
+            /// Returns:
+            ///     str: The json schema serialized to json
+            #[staticmethod]
+            pub fn json_schema() -> String {
+                let schema = schemars::schema_for!(#ident);
+                serde_json::to_string_pretty(&schema).expect("Unexpected failure to serialize schema")
+            }
+        }
+    } else {
+        TokenStream::new()
+    };
 
     let msg = format!("Internal storage of {} object", ident);
     let q = quote! {
         #[automatically_derived]
         #[pyclass(name=#str_ident)]
         #(#struct_attributes)*
         #[derive(Debug, Clone, PartialEq)]
@@ -559,23 +595,23 @@
             #involve_modes_quote
             #substitute_modes_quote
             #operate_mode_gate_quote
             #operate_single_mode_quote
             #operate_two_mode_quote
             #operate_single_mode_gate_quote
             #operate_two_mode_gate_quote
+            #json_schema_quote
             fn __format__(&self, _format_spec: &str) -> PyResult<String> {
                 Ok(format!("{:?}", self.internal))
             }
 
             fn __repr__(&self) -> PyResult<String> {
                 Ok(format!("{:?}", self.internal))
             }
 
-
             /// Returns the __richcmp__ magic method to perform rich comparison
             /// operations on Operation.
             ///
             /// Args:
             ///
             /// * `&self` - the OperationWrapper object
             /// * `other` - the object to compare self to
```

### Comparing `qoqo-1.6.0a1/local_dependencies/qoqo-macros/src/operate.rs` & `qoqo-1.6.0a2/local_dependencies/qoqo-macros/src/operate.rs`

 * *Files identical despite different names*

### Comparing `qoqo-1.6.0a1/Cargo.toml` & `qoqo-1.6.0a2/Cargo.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "qoqo"
-version = "1.6.0-alpha.1"
+version = "1.6.0-alpha.2"
 authors = ["HQS Quantum Simulations <info@quantumsimulations.de>"]
 license = "Apache-2.0"
 homepage = "https://github.com/HQSquantumsimulations/qoqo"
 repository = "https://github.com/HQSquantumsimulations/qoqo"
 documentation = "https://docs.rs/qoqo/"
 readme = "README.md"
 edition = "2021"
@@ -28,27 +28,29 @@
 [dependencies]
 serde = { version = "1.0", features = ["derive"] }
 ndarray = "0.15"
 num-complex = "0.4"
 thiserror = "1.0"
 qoqo_calculator = { version="1.1" }
 qoqo_calculator_pyo3 = {version="1.1", default-features=false}
-qoqo-macros = {version="1.6.0-alpha.1", path= "local_dependencies/qoqo-macros" }
-roqoqo = {version="1.6.0-alpha.1", path= "local_dependencies/roqoqo", features=["serialize", "overrotate"]}
+qoqo-macros = {version="1.6.0-alpha.2", path= "local_dependencies/qoqo-macros" }
+roqoqo = {version="1.6.0-alpha.2", path= "local_dependencies/roqoqo", features=["serialize", "overrotate"]}
 numpy = "0.19"
 bincode = "1.3"
 serde_json = "1.0"
+schemars = "0.8"
 
 [build-dependencies]
 quote = "1.0"
 syn = { version = "2.0", features = ["full", "visit"] }
 proc-macro2 = "1.0"
 pyo3-build-config = "0.19"
 
 [package.metadata.docs.rs]
 no-default-features = true
 
 [features]
 extension-module = ["pyo3/extension-module", "circuitdag"]
-default = ["extension-module"]
+default = ["extension-module", "json_schema"]
 circuitdag = ["roqoqo/circuitdag"]
+json_schema = ["roqoqo/json_schema"]
```

### Comparing `qoqo-1.6.0a1/LICENSE` & `qoqo-1.6.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `qoqo-1.6.0a1/README.md` & `qoqo-1.6.0a2/README.md`

 * *Files identical despite different names*

### Comparing `qoqo-1.6.0a1/build.rs` & `qoqo-1.6.0a2/build.rs`

 * *Files identical despite different names*

### Comparing `qoqo-1.6.0a1/pyproject.toml` & `qoqo-1.6.0a2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "qoqo"
-version = "1.6.0-alpha.1"
+version = "1.6.0-alpha.2"
 dependencies = [
   'numpy',
   'qoqo_calculator_pyo3>=1.1',
 ]
 license = {text="Apache-2.0 AND Apache-2.0 with LLVM-exception AND MIT AND Unicode-DFS-2016 AND BSD-2-Clause AND BSD-3-CLause"}
 maintainers = [{name = "HQS Quantum Simulations GmbH", email = "info@quantumsimulations.de"}]
 requires-python = ">=3.7"
```

### Comparing `qoqo-1.6.0a1/qoqo/DEPENDENCIES` & `qoqo-1.6.0a2/qoqo/DEPENDENCIES`

 * *Files identical despite different names*

### Comparing `qoqo-1.6.0a1/qoqo/LICENSE_FOR_BINARY_DISTRIBUTION` & `qoqo-1.6.0a2/qoqo/LICENSE_FOR_BINARY_DISTRIBUTION`

 * *Files identical despite different names*

### Comparing `qoqo-1.6.0a1/qoqo/PYTHON_LICENSE` & `qoqo-1.6.0a2/qoqo/PYTHON_LICENSE`

 * *Files identical despite different names*

### Comparing `qoqo-1.6.0a1/qoqo/__init__.py` & `qoqo-1.6.0a2/qoqo/__init__.py`

 * *Files identical despite different names*

### Comparing `qoqo-1.6.0a1/src/circuit.rs` & `qoqo-1.6.0a2/src/circuit.rs`

 * *Files 6% similar despite different names*

```diff
@@ -259,26 +259,26 @@
             .map_err(|_| PyValueError::new_err("Cannot serialize Circuit to bytes"))?;
         let b: Py<PyByteArray> = Python::with_gil(|py| -> Py<PyByteArray> {
             PyByteArray::new(py, &serialized[..]).into()
         });
         Ok(b)
     }
 
-    #[staticmethod]
     /// Convert the bincode representation of the Circuit to a Circuit using the [bincode] crate.
     ///
     /// Args:
     ///     input (ByteArray): The serialized Circuit (in [bincode] form).
     ///
     /// Returns:
     ///     Circuit: The deserialized Circuit.
     ///
     /// Raises:
     ///     TypeError: Input cannot be converted to byte array.
     ///     ValueError: Input cannot be deserialized to Circuit.
+    #[staticmethod]
     pub fn from_bincode(input: &PyAny) -> PyResult<Self> {
         let bytes = input
             .extract::<Vec<u8>>()
             .map_err(|_| PyTypeError::new_err("Input cannot be converted to byte array"))?;
 
         Ok(Self {
             internal: deserialize(&bytes[..])
@@ -295,25 +295,57 @@
     ///     ValueError: Cannot serialize Circuit to json.
     fn to_json(&self) -> PyResult<String> {
         let serialized = serde_json::to_string(&self.internal)
             .map_err(|_| PyValueError::new_err("Cannot serialize Circuit to json"))?;
         Ok(serialized)
     }
 
+    #[cfg(feature = "json_schema")]
+    /// Return the JsonSchema for the json serialisation of the class.
+    ///
+    /// Returns:
+    ///     str: The json schema serialized to json
+    #[staticmethod]
+    pub fn json_schema() -> String {
+        let schema = schemars::schema_for!(Circuit);
+        serde_json::to_string_pretty(&schema).expect("Unexpected failure to serialize schema")
+    }
+
+    #[cfg(feature = "json_schema")]
+    /// Returns the current version of the qoqo library .
+    ///
+    /// Returns:
+    ///     str: The current version of the library.
     #[staticmethod]
+    pub fn current_version() -> String {
+        ROQOQO_VERSION.to_string()
+    }
+
+    #[cfg(feature = "json_schema")]
+    /// Return the minimum version of qoqo that supports this object.
+    ///
+    /// Returns:
+    ///     str: The minimum version of the qoqo library to deserialize this object.
+    pub fn min_supported_version(&self) -> String {
+        let min_version: (u32, u32, u32) =
+            Circuit::minimum_supported_roqoqo_version(&self.internal);
+        format!("{}.{}.{}", min_version.0, min_version.1, min_version.2)
+    }
+
     /// Convert the json representation of a Circuit to a Circuit.
     ///
     /// Args:
     ///     input (str): The serialized Circuit in json form.
     ///
     /// Returns:
     ///     Circuit: The deserialized Circuit.
     ///
     /// Raises:
     ///     ValueError: Input cannot be deserialized to Circuit.
+    #[staticmethod]
     pub fn from_json(json_string: &str) -> PyResult<Self> {
         Ok(Self {
             internal: serde_json::from_str(json_string)
                 .map_err(|_| PyValueError::new_err("Input cannot be deserialized to Circuit"))?,
         })
     }
```

### Comparing `qoqo-1.6.0a1/src/circuitdag.rs` & `qoqo-1.6.0a2/src/circuitdag.rs`

 * *Files identical despite different names*

### Comparing `qoqo-1.6.0a1/src/devices/all_to_all.rs` & `qoqo-1.6.0a2/src/devices/all_to_all.rs`

 * *Files 11% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 use ndarray::Array2;
 use numpy::{PyArray2, PyReadonlyArray2, ToPyArray};
 use pyo3::exceptions::{PyTypeError, PyValueError};
 use pyo3::prelude::*;
 use pyo3::types::PyByteArray;
 use qoqo_macros::devicewrapper;
 use roqoqo::devices::{AllToAllDevice, Device};
+#[cfg(feature = "json_schema")]
+use roqoqo::{operations::SupportedVersion, ROQOQO_VERSION};
 
 /// A generic device with all-to-all connectivity.
 ///
 /// Args:
 ///     number_qubits (int): Fixed number of qubits.
 ///     single_qubit_gates (List[str]): A list of 'hqslang' names of single-qubit-gates supported by the device.
 ///     two_qubit_gate (str): The 'hqslang' name of the basic two-qubit-gate supported by the device.
@@ -72,15 +74,15 @@
     /// Args:
     ///     gate (str): The hqslang name of the two-qubit-gate.
     ///     gate_time (float): New gate time.
     ///
     /// Returns:
     ///     AllToAllDevice.
     ///
-    #[pyo3(text_signature = "(gate, gate_time)")]
+    #[pyo3(text_signature = "(gate, gate_time, /)")]
     pub fn set_all_two_qubit_gate_times(&mut self, gate: &str, gate_time: f64) -> Self {
         Self {
             internal: self
                 .internal
                 .clone()
                 .set_all_two_qubit_gate_times(gate, gate_time),
         }
@@ -91,15 +93,15 @@
     /// Args:
     ///     gate (str): The hqslang name of the single-qubit-gate.
     ///     gate_time (float): New gate time.
     ///
     /// Returns:
     ///     AllToAllDevice
     ///
-    #[pyo3(text_signature = "(gate, gate_time)")]
+    #[pyo3(text_signature = "(gate, gate_time, /)")]
     pub fn set_all_single_qubit_gate_times(&self, gate: &str, gate_time: f64) -> Self {
         Self {
             internal: self
                 .internal
                 .clone()
                 .set_all_single_qubit_gate_times(gate, gate_time),
         }
@@ -111,15 +113,15 @@
     ///     rates[2d array]: Decoherence rates provided as (3x3)-matrix for all qubits in the device.
     ///
     /// Returns:
     ///     AllToAllDevice
     ///
     /// Raises:
     ///     PyValueError: The input parameter `rates` needs to be a (3x3)-matrix.
-    #[pyo3(text_signature = "(rates)")]
+    #[pyo3(text_signature = "(rates, /)")]
     pub fn set_all_qubit_decoherence_rates(&self, rates: PyReadonlyArray2<f64>) -> PyResult<Self> {
         let rates_matrix = rates.as_array().to_owned();
         Ok(Self {
             internal: self
                 .internal
                 .clone()
                 .set_all_qubit_decoherence_rates(rates_matrix)
@@ -132,48 +134,80 @@
     /// Adds qubit damping to noise rates.
     ///
     /// Args:
     ///     daming[f64]: The damping rates.
     ///
     /// Returns:
     ///     AllToAllDevice
-    #[pyo3(text_signature = "(damping)")]
+    #[pyo3(text_signature = "(damping, /)")]
     pub fn add_damping_all(&mut self, damping: f64) -> Self {
         Self {
             internal: self.internal.clone().add_damping_all(damping),
         }
     }
 
     /// Adds qubit dephasing to noise rates.
     ///
     /// Args:
     ///     dephasing[f64]: The dephasing rates.
     ///
     /// Returns:
     ///     AllToAllDevice
-    #[pyo3(text_signature = "(dephasing)")]
+    #[pyo3(text_signature = "(dephasing, /)")]
     pub fn add_dephasing_all(&mut self, dephasing: f64) -> Self {
         Self {
             internal: self.internal.clone().add_dephasing_all(dephasing),
         }
     }
 
     /// Adds qubit depolarising to noise rates.
     ///
     /// Args:
     ///     depolarising (float): The depolarising rates.
     ///
     /// Returns:
     ///     AllToAllDevice
-    #[pyo3(text_signature = "(depolarising)")]
+    #[pyo3(text_signature = "(depolarising, /)")]
     pub fn add_depolarising_all(&mut self, depolarising: f64) -> Self {
         Self {
             internal: self.internal.clone().add_depolarising_all(depolarising),
         }
     }
+
+    #[cfg(feature = "json_schema")]
+    /// Return the JsonSchema for the json serialisation of the class.
+    ///
+    /// Returns:
+    ///     str: The json schema serialized to json
+    #[staticmethod]
+    pub fn json_schema() -> String {
+        let schema = schemars::schema_for!(AllToAllDevice);
+        serde_json::to_string_pretty(&schema).expect("Unexpected failure to serialize schema")
+    }
+
+    #[cfg(feature = "json_schema")]
+    /// Returns the current version of the qoqo library .
+    ///
+    /// Returns:
+    ///     str: The current version of the library.
+    #[staticmethod]
+    pub fn current_version() -> String {
+        ROQOQO_VERSION.to_string()
+    }
+
+    #[cfg(feature = "json_schema")]
+    /// Return the minimum version of qoqo that supports this object.
+    ///
+    /// Returns:
+    ///     str: The minimum version of the qoqo library to deserialize this object.
+    pub fn min_supported_version(&self) -> String {
+        let min_version: (u32, u32, u32) =
+            AllToAllDevice::minimum_supported_roqoqo_version(&self.internal);
+        format!("{}.{}.{}", min_version.0, min_version.1, min_version.2)
+    }
 }
 
 impl AllToAllDeviceWrapper {
     /// Fallible conversion of generic python object.
     pub fn from_pyany(input: Py<PyAny>) -> PyResult<AllToAllDevice> {
         Python::with_gil(|py| -> PyResult<AllToAllDevice> {
             let input = input.as_ref(py);
```

### Comparing `qoqo-1.6.0a1/src/devices/generic_device.rs` & `qoqo-1.6.0a2/src/devices/generic_device.rs`

 * *Files 24% similar despite different names*

```diff
@@ -15,14 +15,17 @@
 use ndarray::Array2;
 use numpy::{PyArray2, PyReadonlyArray2, ToPyArray};
 use pyo3::exceptions::{PyTypeError, PyValueError};
 use pyo3::prelude::*;
 use pyo3::types::PyByteArray;
 use qoqo_macros::devicewrapper;
 use roqoqo::devices::{Device, GenericDevice};
+#[cfg(feature = "json_schema")]
+use roqoqo::{operations::SupportedVersion, ROQOQO_VERSION};
+
 /// A generic device assuming all-to-all connectivity between all involved qubits.
 ///
 /// Args:
 ///     number_qubits (int): The number of qubits in the device
 ///
 /// Note:
 ///     GenericDevice uses nested HashMaps to represent the most general device connectivity.
@@ -40,14 +43,46 @@
     #[new]
     #[pyo3(text_signature = "(number_qubits)")]
     pub fn new(number_qubits: usize) -> PyResult<Self> {
         Ok(Self {
             internal: GenericDevice::new(number_qubits),
         })
     }
+
+    #[cfg(feature = "json_schema")]
+    /// Return the JsonSchema for the json serialisation of the class.
+    ///
+    /// Returns:
+    ///     str: The json schema serialized to json
+    #[staticmethod]
+    pub fn json_schema() -> String {
+        let schema = schemars::schema_for!(GenericDevice);
+        serde_json::to_string_pretty(&schema).expect("Unexpected failure to serialize schema")
+    }
+
+    #[cfg(feature = "json_schema")]
+    /// Returns the current version of the qoqo library .
+    ///
+    /// Returns:
+    ///     str: The current version of the library.
+    #[staticmethod]
+    pub fn current_version() -> String {
+        ROQOQO_VERSION.to_string()
+    }
+
+    #[cfg(feature = "json_schema")]
+    /// Return the minimum version of qoqo that supports this object.
+    ///
+    /// Returns:
+    ///     str: The minimum version of the qoqo library to deserialize this object.
+    pub fn min_supported_version(&self) -> String {
+        let min_version: (u32, u32, u32) =
+            GenericDevice::minimum_supported_roqoqo_version(&self.internal);
+        format!("{}.{}.{}", min_version.0, min_version.1, min_version.2)
+    }
 }
 
 impl GenericDeviceWrapper {
     /// Fallible conversion of generic python object..
     pub fn from_pyany(input: Py<PyAny>) -> PyResult<GenericDevice> {
         Python::with_gil(|py| -> PyResult<GenericDevice> {
             let input = input.as_ref(py);
```

### Comparing `qoqo-1.6.0a1/src/devices/mod.rs` & `qoqo-1.6.0a2/src/devices/mod.rs`

 * *Files identical despite different names*

### Comparing `qoqo-1.6.0a1/src/devices/square_lattice.rs` & `qoqo-1.6.0a2/src/devices/square_lattice.rs`

 * *Files 5% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 use ndarray::Array2;
 use numpy::{PyArray2, PyReadonlyArray2, ToPyArray};
 use pyo3::exceptions::{PyTypeError, PyValueError};
 use pyo3::prelude::*;
 use pyo3::types::PyByteArray;
 use qoqo_macros::devicewrapper;
 use roqoqo::devices::{Device, SquareLatticeDevice};
+#[cfg(feature = "json_schema")]
+use roqoqo::{operations::SupportedVersion, ROQOQO_VERSION};
 
 /// A generic square lattice device with only next-neighbours-connectivity.
 ///
 /// Args:
 ///     number_rows (int): The fixed number of rows in device..
 ///     number_columns (int): Fixed number of columns in device.
 ///     single_qubit_gates (List[str]): A list of 'hqslang' names of single-qubit-gates supported by the device.
@@ -94,15 +96,15 @@
     /// Args:
     ///     gate[str]: The hqslang name of the two-qubit-gate.
     ///     gate_time[f64]: Gate time for the given gate, valid for all qubits in the device.
     ///
     /// Returns:
     ///     A qoqo Device with updated gate times.
     ///
-    #[pyo3(text_signature = "(gate, gate_time)")]
+    #[pyo3(text_signature = "(gate, gate_time, /)")]
     pub fn set_all_two_qubit_gate_times(&self, gate: &str, gate_time: f64) -> Self {
         Self {
             internal: self
                 .internal
                 .clone()
                 .set_all_two_qubit_gate_times(gate, gate_time),
         }
@@ -113,15 +115,15 @@
     /// Args:
     ///     gate[str]: The hqslang name of the single-qubit-gate.
     ///     gate_time[f64]: New gate time.
     ///
     /// Returns:
     ///     A qoqo Device with updated gate times.
     ///
-    #[pyo3(text_signature = "(gate, gate_time)")]
+    #[pyo3(text_signature = "(gate, gate_time, /)")]
     pub fn set_all_single_qubit_gate_times(&self, gate: &str, gate_time: f64) -> Self {
         Self {
             internal: self
                 .internal
                 .clone()
                 .set_all_single_qubit_gate_times(gate, gate_time),
         }
@@ -133,15 +135,15 @@
     ///     rates[2d array]: Decoherence rates provided as (3x3)-matrix for all qubits in the device.
     ///
     /// Returns:
     ///     SquareLatticeDevice
     ///
     /// Raises:
     ///     PyValueError: The input parameter `rates` needs to be a (3x3)-matrix.
-    #[pyo3(text_signature = "(rates)")]
+    #[pyo3(text_signature = "(rates, /)")]
     pub fn set_all_qubit_decoherence_rates(&self, rates: PyReadonlyArray2<f64>) -> PyResult<Self> {
         let rates_matrix = rates.as_array().to_owned();
         Ok(Self {
             internal: self
                 .internal
                 .clone()
                 .set_all_qubit_decoherence_rates(rates_matrix)
@@ -154,48 +156,80 @@
     /// Adds qubit damping to noise rates.
     ///
     /// Args:
     ///     daming (float): The damping rates.
     ///
     /// Returns:
     ///     SquareLatticeDevice
-    #[pyo3(text_signature = "(damping)")]
+    #[pyo3(text_signature = "(damping, /)")]
     pub fn add_damping_all(&mut self, damping: f64) -> Self {
         Self {
             internal: self.internal.clone().add_damping_all(damping),
         }
     }
 
     /// Adds qubit dephasing to noise rates.
     ///
     /// Args:
     ///     dephasing (float): The dephasing rates.
     ///
     /// Returns:
     ///     SquareLatticeDevice
-    #[pyo3(text_signature = "(dephasing)")]
+    #[pyo3(text_signature = "(dephasing, /)")]
     pub fn add_dephasing_all(&mut self, dephasing: f64) -> Self {
         Self {
             internal: self.internal.clone().add_dephasing_all(dephasing),
         }
     }
 
     /// Adds qubit depolarising to noise rates.
     ///
     /// Args:
     ///     depolarising (float): The depolarising rates.
     ///
     /// Returns:
     ///     SquareLatticeDevice
-    #[pyo3(text_signature = "(depolarising)")]
+    #[pyo3(text_signature = "(depolarising, /)")]
     pub fn add_depolarising_all(&mut self, depolarising: f64) -> Self {
         Self {
             internal: self.internal.clone().add_depolarising_all(depolarising),
         }
     }
+
+    #[cfg(feature = "json_schema")]
+    /// Return the JsonSchema for the json serialisation of the class.
+    ///
+    /// Returns:
+    ///     str: The json schema serialized to json
+    #[staticmethod]
+    pub fn json_schema() -> String {
+        let schema = schemars::schema_for!(SquareLatticeDevice);
+        serde_json::to_string_pretty(&schema).expect("Unexpected failure to serialize schema")
+    }
+
+    #[cfg(feature = "json_schema")]
+    /// Returns the current version of the qoqo library .
+    ///
+    /// Returns:
+    ///     str: The current version of the library.
+    #[staticmethod]
+    pub fn current_version() -> String {
+        ROQOQO_VERSION.to_string()
+    }
+
+    #[cfg(feature = "json_schema")]
+    /// Return the minimum version of qoqo that supports this object.
+    ///
+    /// Returns:
+    ///     str: The minimum version of the qoqo library to deserialize this object.
+    pub fn min_supported_version(&self) -> String {
+        let min_version: (u32, u32, u32) =
+            SquareLatticeDevice::minimum_supported_roqoqo_version(&self.internal);
+        format!("{}.{}.{}", min_version.0, min_version.1, min_version.2)
+    }
 }
 
 impl SquareLatticeDeviceWrapper {
     /// Fallible conversion of generic python object..
     pub fn from_pyany(input: Py<PyAny>) -> PyResult<SquareLatticeDevice> {
         Python::with_gil(|py| -> PyResult<SquareLatticeDevice> {
             let input = input.as_ref(py);
```

### Comparing `qoqo-1.6.0a1/src/lib.rs` & `qoqo-1.6.0a2/src/lib.rs`

 * *Files identical despite different names*

### Comparing `qoqo-1.6.0a1/src/measurements/basis_rotation_measurement.rs` & `qoqo-1.6.0a2/src/measurements/basis_rotation_measurement.rs`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,18 @@
 use pyo3::exceptions::{PyRuntimeError, PyTypeError, PyValueError};
 use pyo3::prelude::*;
 use pyo3::types::PyByteArray;
 use roqoqo::measurements::PauliZProduct;
 use roqoqo::prelude::*;
 use roqoqo::registers::{BitOutputRegister, ComplexOutputRegister, FloatOutputRegister};
 use roqoqo::Circuit;
+#[cfg(feature = "json_schema")]
+use roqoqo::ROQOQO_VERSION;
 use std::collections::HashMap;
+
 #[pyclass(name = "PauliZProduct", module = "qoqo.measurements")]
 #[derive(Clone, Debug)]
 /// Collected information for executing a measurement of PauliZ product.
 pub struct PauliZProductWrapper {
     /// Internal storage of [roqoqo::PauliZProduct].
     pub internal: PauliZProduct,
 }
@@ -235,26 +238,26 @@
             .map_err(|_| PyValueError::new_err("Cannot serialize PauliZProduct to bytes"))?;
         let b: Py<PyByteArray> = Python::with_gil(|py| -> Py<PyByteArray> {
             PyByteArray::new(py, &serialized[..]).into()
         });
         Ok(b)
     }
 
-    #[staticmethod]
     /// Convert the bincode representation of the PauliZProduct to a PauliZProduct using the [bincode] crate.
     ///
     /// Args:
     ///     input (ByteArray): The serialized PauliZProduct (in [bincode] form).
     ///
     /// Returns:
     ///     PauliZProduct: The deserialized PauliZProduct.
     ///
     /// Raises:
     ///     TypeError: Input cannot be converted to byte array.
     ///     ValueError: Input cannot be deserialized to PauliZProduct.
+    #[staticmethod]
     pub fn from_bincode(input: &PyAny) -> PyResult<Self> {
         let bytes = input
             .extract::<Vec<u8>>()
             .map_err(|_| PyTypeError::new_err("Input cannot be converted to byte array"))?;
 
         Ok(Self {
             internal: deserialize(&bytes[..]).map_err(|_| {
@@ -325,14 +328,46 @@
             pyo3::class::basic::CompareOp::Eq => Ok(self.internal == other.internal),
             pyo3::class::basic::CompareOp::Ne => Ok(self.internal != other.internal),
             _ => Err(pyo3::exceptions::PyNotImplementedError::new_err(
                 "Other comparison not implemented",
             )),
         }
     }
+
+    #[cfg(feature = "json_schema")]
+    /// Return the JsonSchema for the json serialisation of the class.
+    ///
+    /// Returns:
+    ///     str: The json schema serialized to json
+    #[staticmethod]
+    pub fn json_schema() -> String {
+        let schema = schemars::schema_for!(PauliZProduct);
+        serde_json::to_string_pretty(&schema).expect("Unexpected failure to serialize schema")
+    }
+
+    #[cfg(feature = "json_schema")]
+    /// Returns the current version of the qoqo library .
+    ///
+    /// Returns:
+    ///     str: The current version of the library.
+    #[staticmethod]
+    pub fn current_version() -> String {
+        ROQOQO_VERSION.to_string()
+    }
+
+    #[cfg(feature = "json_schema")]
+    /// Return the minimum version of qoqo that supports this object.
+    ///
+    /// Returns:
+    ///     str: The minimum version of the qoqo library to deserialize this object.
+    pub fn min_supported_version(&self) -> String {
+        let min_version: (u32, u32, u32) =
+            PauliZProduct::minimum_supported_roqoqo_version(&self.internal);
+        format!("{}.{}.{}", min_version.0, min_version.1, min_version.2)
+    }
 }
 
 impl PauliZProductWrapper {
     /// Extracts a PauliZProduct from a PauliZProductWrapper python object.
     ///
     /// When working with qoqo and other rust based python packages compiled separately
     /// a downcast will not detect that two PauliZProductWrapper objects are compatible.
```

### Comparing `qoqo-1.6.0a1/src/measurements/cheated_basis_rotation_measurement.rs` & `qoqo-1.6.0a2/src/measurements/cheated_basis_rotation_measurement.rs`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,18 @@
 use pyo3::exceptions::{PyRuntimeError, PyTypeError, PyValueError};
 use pyo3::prelude::*;
 use pyo3::types::PyByteArray;
 use roqoqo::measurements::CheatedPauliZProduct;
 use roqoqo::prelude::*;
 use roqoqo::registers::{BitOutputRegister, ComplexOutputRegister, FloatOutputRegister};
 use roqoqo::Circuit;
+#[cfg(feature = "json_schema")]
+use roqoqo::ROQOQO_VERSION;
 use std::collections::HashMap;
+
 #[pyclass(name = "CheatedPauliZProduct", module = "qoqo.measurements")]
 #[derive(Clone, Debug)]
 /// Collected information for executing a cheated measurement of PauliZ product.
 pub struct CheatedPauliZProductWrapper {
     /// Internal storage of [roqoqo::PauliZProduct].
     pub internal: CheatedPauliZProduct,
 }
@@ -234,26 +237,26 @@
             .map_err(|_| PyValueError::new_err("Cannot serialize CheatedPauliZProduct to bytes"))?;
         let b: Py<PyByteArray> = Python::with_gil(|py| -> Py<PyByteArray> {
             PyByteArray::new(py, &serialized[..]).into()
         });
         Ok(b)
     }
 
-    #[staticmethod]
     /// Convert the bincode representation of the CheatedPauliZProduct to a CheatedPauliZProduct using the [bincode] crate.
     ///
     /// Args:
     ///     input (ByteArray): The serialized CheatedPauliZProduct (in [bincode] form).
     ///
     /// Returns:
     ///     CheatedPauliZProduct: The deserialized CheatedPauliZProduct.
     ///
     /// Raises:
     ///     TypeError: Input cannot be converted to byte array.
     ///     ValueError: Input cannot be deserialized to CheatedPauliZProduct.
+    #[staticmethod]
     pub fn from_bincode(input: &PyAny) -> PyResult<Self> {
         let bytes = input
             .extract::<Vec<u8>>()
             .map_err(|_| PyTypeError::new_err("Input cannot be converted to byte array"))?;
 
         Ok(Self {
             internal: deserialize(&bytes[..]).map_err(|_| {
@@ -324,14 +327,46 @@
             pyo3::class::basic::CompareOp::Eq => Ok(self.internal == other.internal),
             pyo3::class::basic::CompareOp::Ne => Ok(self.internal != other.internal),
             _ => Err(pyo3::exceptions::PyNotImplementedError::new_err(
                 "Other comparison not implemented",
             )),
         }
     }
+
+    #[cfg(feature = "json_schema")]
+    /// Return the JsonSchema for the json serialisation of the class.
+    ///
+    /// Returns:
+    ///     str: The json schema serialized to json
+    #[staticmethod]
+    pub fn json_schema() -> String {
+        let schema = schemars::schema_for!(CheatedPauliZProduct);
+        serde_json::to_string_pretty(&schema).expect("Unexpected failure to serialize schema")
+    }
+
+    #[cfg(feature = "json_schema")]
+    /// Returns the current version of the qoqo library .
+    ///
+    /// Returns:
+    ///     str: The current version of the library.
+    #[staticmethod]
+    pub fn current_version() -> String {
+        ROQOQO_VERSION.to_string()
+    }
+
+    #[cfg(feature = "json_schema")]
+    /// Return the minimum version of qoqo that supports this object.
+    ///
+    /// Returns:
+    ///     str: The minimum version of the qoqo library to deserialize this object.
+    pub fn min_supported_version(&self) -> String {
+        let min_version: (u32, u32, u32) =
+            CheatedPauliZProduct::minimum_supported_roqoqo_version(&self.internal);
+        format!("{}.{}.{}", min_version.0, min_version.1, min_version.2)
+    }
 }
 
 impl CheatedPauliZProductWrapper {
     /// Extracts a CheatedPauliZProduct from a CheatedPauliZProductWrapper python object.
     ///
     /// When working with qoqo and other rust based python packages compiled separately
     /// a downcast will not detect that two CheatedPauliZProductWrapper objects are compatible.
```

### Comparing `qoqo-1.6.0a1/src/measurements/cheated_measurement.rs` & `qoqo-1.6.0a2/src/measurements/cheated_measurement.rs`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,18 @@
 use pyo3::exceptions::{PyRuntimeError, PyTypeError, PyValueError};
 use pyo3::prelude::*;
 use pyo3::types::PyByteArray;
 use roqoqo::measurements::Cheated;
 use roqoqo::prelude::*;
 use roqoqo::registers::{BitOutputRegister, ComplexOutputRegister, FloatOutputRegister};
 use roqoqo::Circuit;
+#[cfg(feature = "json_schema")]
+use roqoqo::ROQOQO_VERSION;
 use std::collections::HashMap;
+
 #[pyclass(name = "Cheated", module = "qoqo.measurements")]
 #[derive(Clone, Debug)]
 /// Collected information for executing a cheated measurement.
 pub struct CheatedWrapper {
     /// Internal storage of [roqoqo::Cheated]
     pub internal: Cheated,
 }
@@ -234,26 +237,26 @@
             .map_err(|_| PyValueError::new_err("Cannot serialize Cheated to bytes"))?;
         let b: Py<PyByteArray> = Python::with_gil(|py| -> Py<PyByteArray> {
             PyByteArray::new(py, &serialized[..]).into()
         });
         Ok(b)
     }
 
-    #[staticmethod]
     /// Convert the bincode representation of the Cheated to a Cheated using the [bincode] crate.
     ///
     /// Args:
     ///     input (ByteArray): The serialized Cheated (in [bincode] form).
     ///
     /// Returns:
     ///     Cheated: The deserialized Cheated.
     ///
     /// Raises:
     ///     TypeError: Input cannot be converted to byte array.
     ///     ValueError: Input cannot be deserialized to Cheated.
+    #[staticmethod]
     pub fn from_bincode(input: &PyAny) -> PyResult<Self> {
         let bytes = input
             .extract::<Vec<u8>>()
             .map_err(|_| PyTypeError::new_err("Input cannot be converted to byte array"))?;
 
         Ok(Self {
             internal: deserialize(&bytes[..])
@@ -323,14 +326,46 @@
             pyo3::class::basic::CompareOp::Eq => Ok(self.internal == other.internal),
             pyo3::class::basic::CompareOp::Ne => Ok(self.internal != other.internal),
             _ => Err(pyo3::exceptions::PyNotImplementedError::new_err(
                 "Other comparison not implemented",
             )),
         }
     }
+
+    #[cfg(feature = "json_schema")]
+    /// Return the JsonSchema for the json serialisation of the class.
+    ///
+    /// Returns:
+    ///     str: The json schema serialized to json
+    #[staticmethod]
+    pub fn json_schema() -> String {
+        let schema = schemars::schema_for!(Cheated);
+        serde_json::to_string_pretty(&schema).expect("Unexpected failure to serialize schema")
+    }
+
+    #[cfg(feature = "json_schema")]
+    /// Returns the current version of the qoqo library .
+    ///
+    /// Returns:
+    ///     str: The current version of the library.
+    #[staticmethod]
+    pub fn current_version() -> String {
+        ROQOQO_VERSION.to_string()
+    }
+
+    #[cfg(feature = "json_schema")]
+    /// Return the minimum version of qoqo that supports this object.
+    ///
+    /// Returns:
+    ///     str: The minimum version of the qoqo library to deserialize this object.
+    pub fn min_supported_version(&self) -> String {
+        let min_version: (u32, u32, u32) =
+            Cheated::minimum_supported_roqoqo_version(&self.internal);
+        format!("{}.{}.{}", min_version.0, min_version.1, min_version.2)
+    }
 }
 
 impl CheatedWrapper {
     /// Extracts a Cheated from a CheatedWrapper python object.
     ///
     /// When working with qoqo and other rust based python packages compiled separately
     /// a downcast will not detect that two CheatedWrapper objects are compatible.
```

### Comparing `qoqo-1.6.0a1/src/measurements/classical_register_measurement.rs` & `qoqo-1.6.0a2/src/measurements/classical_register_measurement.rs`

 * *Files 6% similar despite different names*

```diff
@@ -16,15 +16,18 @@
 use bincode::{deserialize, serialize};
 use pyo3::exceptions::{PyRuntimeError, PyTypeError, PyValueError};
 use pyo3::prelude::*;
 use pyo3::types::PyByteArray;
 use roqoqo::measurements::ClassicalRegister;
 use roqoqo::prelude::*;
 use roqoqo::Circuit;
+#[cfg(feature = "json_schema")]
+use roqoqo::ROQOQO_VERSION;
 use std::collections::HashMap;
+
 #[pyclass(name = "ClassicalRegister", module = "qoqo.measurements")]
 #[derive(Clone, Debug)]
 /// Collected information for executing a classical register.
 pub struct ClassicalRegisterWrapper {
     /// Internal storage of [roqoqo::ClassicalRegister].
     pub internal: ClassicalRegister,
 }
@@ -156,26 +159,26 @@
             .map_err(|_| PyValueError::new_err("Cannot serialize ClassicalRegister to bytes"))?;
         let b: Py<PyByteArray> = Python::with_gil(|py| -> Py<PyByteArray> {
             PyByteArray::new(py, &serialized[..]).into()
         });
         Ok(b)
     }
 
-    #[staticmethod]
     /// Convert the bincode representation of the ClassicalRegister to a ClassicalRegister using the [bincode] crate.
     ///
     /// Args:
     ///     input (ByteArray): The serialized ClassicalRegister (in [bincode] form).
     ///
     /// Returns:
     ///     ClassicalRegister: The deserialized ClassicalRegister.
     ///
     /// Raises:
     ///     TypeError: Input cannot be converted to byte array.
     ///     ValueError: Input cannot be deserialized to ClassicalRegister.
+    #[staticmethod]
     pub fn from_bincode(input: &PyAny) -> PyResult<Self> {
         let bytes = input
             .extract::<Vec<u8>>()
             .map_err(|_| PyTypeError::new_err("Input cannot be converted to byte array"))?;
 
         Ok(Self {
             internal: deserialize(&bytes[..]).map_err(|_| {
@@ -246,14 +249,46 @@
             pyo3::class::basic::CompareOp::Eq => Ok(self.internal == other.internal),
             pyo3::class::basic::CompareOp::Ne => Ok(self.internal != other.internal),
             _ => Err(pyo3::exceptions::PyNotImplementedError::new_err(
                 "Other comparison not implemented",
             )),
         }
     }
+
+    #[cfg(feature = "json_schema")]
+    /// Return the JsonSchema for the json serialisation of the class.
+    ///
+    /// Returns:
+    ///     str: The json schema serialized to json
+    #[staticmethod]
+    pub fn json_schema() -> String {
+        let schema = schemars::schema_for!(ClassicalRegister);
+        serde_json::to_string_pretty(&schema).expect("Unexpected failure to serialize schema")
+    }
+
+    #[cfg(feature = "json_schema")]
+    /// Returns the current version of the qoqo library .
+    ///
+    /// Returns:
+    ///     str: The current version of the library.
+    #[staticmethod]
+    pub fn current_version() -> String {
+        ROQOQO_VERSION.to_string()
+    }
+
+    #[cfg(feature = "json_schema")]
+    /// Return the minimum version of qoqo that supports this object.
+    ///
+    /// Returns:
+    ///     str: The minimum version of the qoqo library to deserialize this object.
+    pub fn min_supported_version(&self) -> String {
+        let min_version: (u32, u32, u32) =
+            ClassicalRegister::minimum_supported_roqoqo_version(&self.internal);
+        format!("{}.{}.{}", min_version.0, min_version.1, min_version.2)
+    }
 }
 
 impl ClassicalRegisterWrapper {
     /// Extracts a ClassicalRegister from a ClassicalRegisterWrapper python object.
     ///
     /// When working with qoqo and other rust based python packages compiled separately
     /// a downcast will not detect that two ClassicalRegisterWrapper objects are compatible.
```

### Comparing `qoqo-1.6.0a1/src/measurements/measurement_auxiliary_data_input.rs` & `qoqo-1.6.0a2/src/measurements/measurement_auxiliary_data_input.rs`

 * *Files 6% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 use num_complex::Complex64;
 use pyo3::exceptions::{PyRuntimeError, PyTypeError, PyValueError};
 use pyo3::prelude::*;
 use pyo3::types::PyByteArray;
 use roqoqo::measurements::{
     CheatedInput, CheatedPauliZProductInput, PauliProductMask, PauliZProductInput,
 };
+#[cfg(feature = "json_schema")]
+use roqoqo::{operations::SupportedVersion, ROQOQO_VERSION};
 use std::collections::HashMap;
 
 #[pyclass(name = "PauliZProductInput", module = "qoqo.measurements")]
 #[derive(Clone, Debug)]
 /// Provides Necessary Information to run a [roqoqo::measurements::PauliZProduct] measurement.
 pub struct PauliZProductInputWrapper {
     /// Internal storage of [roqoqo::PauliZProductInput].
@@ -162,26 +164,26 @@
             .map_err(|_| PyValueError::new_err("Cannot serialize PauliZProductInput to bytes"))?;
         let b: Py<PyByteArray> = Python::with_gil(|py| -> Py<PyByteArray> {
             PyByteArray::new(py, &serialized[..]).into()
         });
         Ok(b)
     }
 
-    #[staticmethod]
     /// Convert the bincode representation of the PauliZProductInput to a PauliZProductInput using the [bincode] crate.
     ///
     /// Args:
     ///     input (ByteArray): The serialized PauliZProductInput (in [bincode] form).
     ///
     /// Returns:
     ///     PauliZProductInput: The deserialized PauliZProductInput.
     ///
     /// Raises:
     ///     TypeError: Input cannot be converted to byte array.
     ///     ValueError: Input cannot be deserialized to PauliZProductInput.
+    #[staticmethod]
     pub fn from_bincode(input: &PyAny) -> PyResult<Self> {
         let bytes = input
             .extract::<Vec<u8>>()
             .map_err(|_| PyTypeError::new_err("Input cannot be converted to byte array"))?;
 
         Ok(Self {
             internal: deserialize(&bytes[..]).map_err(|_| {
@@ -214,14 +216,46 @@
         }
     }
 
     /// Return a deep copy of the Object.
     pub fn __deepcopy__(&self, _memodict: Py<PyAny>) -> Self {
         self.clone()
     }
+
+    #[cfg(feature = "json_schema")]
+    /// Return the JsonSchema for the json serialisation of the class.
+    ///
+    /// Returns:
+    ///     str: The json schema serialized to json
+    #[staticmethod]
+    pub fn json_schema() -> String {
+        let schema = schemars::schema_for!(PauliZProductInput);
+        serde_json::to_string_pretty(&schema).expect("Unexpected failure to serialize schema")
+    }
+
+    #[cfg(feature = "json_schema")]
+    /// Returns the current version of the qoqo library .
+    ///
+    /// Returns:
+    ///     str: The current version of the library.
+    #[staticmethod]
+    pub fn current_version() -> String {
+        ROQOQO_VERSION.to_string()
+    }
+
+    #[cfg(feature = "json_schema")]
+    /// Return the minimum version of qoqo that supports this object.
+    ///
+    /// Returns:
+    ///     str: The minimum version of the qoqo library to deserialize this object.
+    pub fn min_supported_version(&self) -> String {
+        let min_version: (u32, u32, u32) =
+            PauliZProductInput::minimum_supported_roqoqo_version(&self.internal);
+        format!("{}.{}.{}", min_version.0, min_version.1, min_version.2)
+    }
 }
 
 #[pyclass(name = "CheatedPauliZProductInput", module = "qoqo.measurements")]
 #[derive(Clone, Debug)]
 /// Collected information for executing a cheated basis rotation measurement.
 pub struct CheatedPauliZProductInputWrapper {
     /// Internal storage of [roqoqo::CheatedPauliZProductInput].
@@ -354,26 +388,26 @@
         })?;
         let b: Py<PyByteArray> = Python::with_gil(|py| -> Py<PyByteArray> {
             PyByteArray::new(py, &serialized[..]).into()
         });
         Ok(b)
     }
 
-    #[staticmethod]
     /// Convert the bincode representation of the CheatedPauliZProductInput to a CheatedPauliZProductInput using the [bincode] crate.
     ///
     /// Args:
     ///     input (ByteArray): The serialized CheatedPauliZProductInput (in [bincode] form).
     ///
     /// Returns:
     ///     CheatedPauliZProductInput: The deserialized CheatedPauliZProductInput.
     ///
     /// Raises:
     ///     TypeError: Input cannot be converted to byte array.
     ///     ValueError: Input cannot be deserialized to CheatedPauliZProductInput.
+    #[staticmethod]
     pub fn from_bincode(input: &PyAny) -> PyResult<Self> {
         let bytes = input
             .extract::<Vec<u8>>()
             .map_err(|_| PyTypeError::new_err("Input cannot be converted to byte array"))?;
 
         Ok(Self {
             internal: deserialize(&bytes[..]).map_err(|_| {
@@ -406,14 +440,46 @@
             pyo3::class::basic::CompareOp::Eq => Ok(self.internal == other.internal),
             pyo3::class::basic::CompareOp::Ne => Ok(self.internal != other.internal),
             _ => Err(pyo3::exceptions::PyNotImplementedError::new_err(
                 "Other comparison not implemented",
             )),
         }
     }
+
+    #[cfg(feature = "json_schema")]
+    /// Return the JsonSchema for the json serialisation of the class.
+    ///
+    /// Returns:
+    ///     str: The json schema serialized to json
+    #[staticmethod]
+    pub fn json_schema() -> String {
+        let schema = schemars::schema_for!(CheatedPauliZProductInput);
+        serde_json::to_string_pretty(&schema).expect("Unexpected failure to serialize schema")
+    }
+
+    #[cfg(feature = "json_schema")]
+    /// Returns the current version of the qoqo library .
+    ///
+    /// Returns:
+    ///     str: The current version of the library.
+    #[staticmethod]
+    pub fn current_version() -> String {
+        ROQOQO_VERSION.to_string()
+    }
+
+    #[cfg(feature = "json_schema")]
+    /// Return the minimum version of qoqo that supports this object.
+    ///
+    /// Returns:
+    ///     str: The minimum version of the qoqo library to deserialize this object.
+    pub fn min_supported_version(&self) -> String {
+        let min_version: (u32, u32, u32) =
+            CheatedPauliZProductInput::minimum_supported_roqoqo_version(&self.internal);
+        format!("{}.{}.{}", min_version.0, min_version.1, min_version.2)
+    }
 }
 
 #[pyclass(name = "CheatedInput", module = "qoqo.measurements")]
 #[derive(Clone, Debug)]
 /// Provides Necessary Information to run a cheated measurement.
 pub struct CheatedInputWrapper {
     /// Internal storage of [roqoqo::CheatedInput].
@@ -510,26 +576,26 @@
             .map_err(|_| PyValueError::new_err("Cannot serialize CheatedInput to bytes"))?;
         let b: Py<PyByteArray> = Python::with_gil(|py| -> Py<PyByteArray> {
             PyByteArray::new(py, &serialized[..]).into()
         });
         Ok(b)
     }
 
-    #[staticmethod]
     /// Convert the bincode representation of the CheatedInput to a CheatedInput using the [bincode] crate.
     ///
     /// Args:
     ///     input (ByteArray): The serialized CheatedInput (in [bincode] form).
     ///
     /// Returns:
     ///     CheatedInput: The deserialized CheatedInput.
     ///
     /// Raises:
     ///     TypeError: Input cannot be converted to byte array.
     ///     ValueError: Input cannot be deserialized to CheatedInput.
+    #[staticmethod]
     pub fn from_bincode(input: &PyAny) -> PyResult<Self> {
         let bytes = input
             .extract::<Vec<u8>>()
             .map_err(|_| PyTypeError::new_err("Input cannot be converted to byte array"))?;
 
         Ok(Self {
             internal: deserialize(&bytes[..]).map_err(|_| {
@@ -561,14 +627,46 @@
             pyo3::class::basic::CompareOp::Eq => Ok(self.internal == other.internal),
             pyo3::class::basic::CompareOp::Ne => Ok(self.internal != other.internal),
             _ => Err(pyo3::exceptions::PyNotImplementedError::new_err(
                 "Other comparison not implemented",
             )),
         }
     }
+
+    #[cfg(feature = "json_schema")]
+    /// Return the JsonSchema for the json serialisation of the class.
+    ///
+    /// Returns:
+    ///     str: The json schema serialized to json
+    #[staticmethod]
+    pub fn json_schema() -> String {
+        let schema = schemars::schema_for!(CheatedInput);
+        serde_json::to_string_pretty(&schema).expect("Unexpected failure to serialize schema")
+    }
+
+    #[cfg(feature = "json_schema")]
+    /// Returns the current version of the qoqo library .
+    ///
+    /// Returns:
+    ///     str: The current version of the library.
+    #[staticmethod]
+    pub fn current_version() -> String {
+        ROQOQO_VERSION.to_string()
+    }
+
+    #[cfg(feature = "json_schema")]
+    /// Return the minimum version of qoqo that supports this object.
+    ///
+    /// Returns:
+    ///     str: The minimum version of the qoqo library to deserialize this object.
+    pub fn min_supported_version(&self) -> String {
+        let min_version: (u32, u32, u32) =
+            CheatedInput::minimum_supported_roqoqo_version(&self.internal);
+        format!("{}.{}.{}", min_version.0, min_version.1, min_version.2)
+    }
 }
 
 impl CheatedPauliZProductInputWrapper {
     /// Extracts a CheatedPauliZProductInput from a CheatedPauliZProductInputWrapper python object.
     ///
     /// When working with qoqo and other rust based python packages compiled separately
     /// a downcast will not detect that two CheatedPauliZProductInputWrapper objects are compatible.
```

### Comparing `qoqo-1.6.0a1/src/measurements/mod.rs` & `qoqo-1.6.0a2/src/measurements/mod.rs`

 * *Files identical despite different names*

### Comparing `qoqo-1.6.0a1/src/operations/bosonic_operations.rs` & `qoqo-1.6.0a2/src/operations/bosonic_operations.rs`

 * *Files 4% similar despite different names*

```diff
@@ -13,25 +13,28 @@
 use pyo3::exceptions::PyRuntimeError;
 use pyo3::prelude::*;
 use pyo3::types::PySet;
 use qoqo_calculator::CalculatorFloat;
 use qoqo_calculator_pyo3::{convert_into_calculator_float, CalculatorFloatWrapper};
 use qoqo_macros::*;
 use roqoqo::operations::*;
+#[cfg(feature = "json_schema")]
+use roqoqo::ROQOQO_VERSION;
 use std::collections::HashMap;
 
 #[wrap(
     Operate,
     OperateModeGate,
     Substitute,
     SubstituteModes,
     InvolveModes,
     OperateSingleMode,
     InvolveQubits,
-    OperateSingleModeGate
+    OperateSingleModeGate,
+    JsonSchema
 )]
 /// The single-mode squeezing gate with tunable squeezing.
 ///
 /// The squeezing gate is a quantum operation that allows for precise manipulation of quantum states,
 /// by reducing the uncertainty in one variable and therefore increasing the uncertainty of another.
 /// https://arxiv.org/pdf/quant-ph/0106157.pdf
 ///
@@ -49,15 +52,16 @@
     Operate,
     OperateModeGate,
     Substitute,
     SubstituteModes,
     InvolveModes,
     OperateSingleMode,
     InvolveQubits,
-    OperateSingleModeGate
+    OperateSingleModeGate,
+    JsonSchema
 )]
 /// The single-mode phase-shift gate with variable phase, given by R(θ) = eexp(i * θ * 𝑁̂).
 ///
 /// https://arxiv.org/pdf/2104.03241.pdf
 ///
 /// Args:
 ///     mode (int): The mode the phase-shift gate is applied to.
@@ -70,15 +74,16 @@
 #[wrap(
     OperateModeGate,
     OperateTwoModeGate,
     Operate,
     Substitute,
     InvolveModes,
     SubstituteModes,
-    OperateTwoMode
+    OperateTwoMode,
+    JsonSchema
 )]
 /// The 2-mode beam splitter which splits a beam with a transmission amplitude cos(θ) and a reflection amplitude exp(i * φ) * sin(θ).
 ///
 /// Args:
 ///     mode_0 (int): The first mode the beam-splitter is applied to.
 ///     mode_1 (int): The second mode the beam-splitter is applied to.
 ///     theta (CalculatorFloat): The transmittivity angle of the beam-splitter.
@@ -86,15 +91,22 @@
 pub struct BeamSplitter {
     mode_0: usize,
     mode_1: usize,
     theta: CalculatorFloat,
     phi: CalculatorFloat,
 }
 
-#[wrap(Operate, Substitute, InvolveModes, SubstituteModes, OperateSingleMode)]
+#[wrap(
+    Operate,
+    Substitute,
+    InvolveModes,
+    SubstituteModes,
+    OperateSingleMode,
+    JsonSchema
+)]
 /// The photon number-resolving detector measurement for bosons.
 ///
 /// This can be used as a single-shot measurement of the photon number.
 /// https://arxiv.org/pdf/0902.4824.pdf
 ///
 /// Args:
 ///     mode (int): The mode the detector (measurement) is applied to.
```

### Comparing `qoqo-1.6.0a1/src/operations/define_operations.rs` & `qoqo-1.6.0a2/src/operations/define_operations.rs`

 * *Files 16% similar despite different names*

```diff
@@ -11,84 +11,86 @@
 // limitations under the License.
 
 use pyo3::exceptions::PyRuntimeError;
 use pyo3::prelude::*;
 use pyo3::types::PySet;
 use qoqo_macros::*;
 use roqoqo::operations::*;
+#[cfg(feature = "json_schema")]
+use roqoqo::ROQOQO_VERSION;
 use std::collections::HashMap;
 
-#[wrap(Operate, Define)]
+#[wrap(Operate, Define, JsonSchema)]
 #[derive(Eq)]
 /// DefinitionFloat is the Definition for a Float type register.
 ///
 /// Args:
 ///     name (string): The name of the register that is defined.
 ///     length (int): The length of the register that is defined, usually the number of qubits to be measured.
 ///     is_output (bool): True/False if the variable is an output to the program.
 pub struct DefinitionFloat {
     name: String,
     length: usize,
     is_output: bool,
 }
 
-#[wrap(Operate, Define)]
+#[wrap(Operate, Define, JsonSchema)]
 #[derive(Eq)]
 /// DefinitionComplex is the Definition for a Complex type register.
 ///
 /// Args:
 ///     name (string): The name of the register that is defined.
 ///     length (int): The length of the register that is defined, usually the number of qubits to be measured.
 ///     is_output (bool): True/False if the variable is an output to the program.
 pub struct DefinitionComplex {
     name: String,
     length: usize,
     is_output: bool,
 }
 
-#[wrap(Operate, Define)]
+#[wrap(Operate, Define, JsonSchema)]
 #[derive(Eq)]
 /// DefinitionUsize is the Definition for an Integer type register.
 ///
 /// Args:
 ///     name (string): The name of the register that is defined.
 ///     length (int): The length of the register that is defined, usually the number of qubits to be measured.
 ///     is_output (bool): True/False if the variable is an output to the program.
 pub struct DefinitionUsize {
     name: String,
     length: usize,
     is_output: bool,
 }
 
-#[wrap(Operate, Define)]
+#[wrap(Operate, Define, JsonSchema)]
 #[derive(Eq)]
 /// DefinitionBit is the Definition for a Bit type register.
 ///
 /// Args:
 ///     name (string): The name of the register that is defined.
 ///     length (int): The length of the register that is defined, usually the number of qubits to be measured.
 ///     is_output (bool): True/False if the variable is an output to the program.
 pub struct DefinitionBit {
     name: String,
     length: usize,
     is_output: bool,
 }
 
-#[wrap(Operate, Define)]
+#[wrap(Operate, Define, JsonSchema)]
 /// InputSymbolic is the Definition for a Float which will replace a certain symbolic parameter.
 ///
 /// Args:
 ///     name (string): The name of the register that is defined.
 ///     input (float): The float by which to replace the quantities marked as "name".
 pub struct InputSymbolic {
     name: String,
     input: f64,
 }
 
-#[wrap(Operate, Define)]
+#[wrap(Operate, Define, JsonSchema)]
 #[derive(Eq)]
 /// InputBit sets a certain bit in an existing BitRegister of the circuit.
 ///
 /// Args:
 ///     name (string): The name of the register that is defined.
 ///     index (int): The index in the register that is set.
 ///     value (int): The value the bit is set to.
```

### Comparing `qoqo-1.6.0a1/src/operations/measurement_operations.rs` & `qoqo-1.6.0a2/src/operations/measurement_operations.rs`

 * *Files 2% similar despite different names*

```diff
@@ -12,17 +12,19 @@
 use crate::{convert_into_circuit, CircuitWrapper};
 use pyo3::exceptions::PyRuntimeError;
 use pyo3::prelude::*;
 use pyo3::types::PySet;
 use qoqo_macros::*;
 use roqoqo::operations::*;
 use roqoqo::Circuit;
+#[cfg(feature = "json_schema")]
+use roqoqo::ROQOQO_VERSION;
 use std::collections::HashMap;
 
-#[wrap(Operate, OperateSingleQubit)]
+#[wrap(Operate, OperateSingleQubit, JsonSchema)]
 #[derive(Eq)]
 /// Measurement gate operation.
 ///
 /// This Operation acts on one qubit writing the result of the measurement into a readout.
 /// The classical register for the readout needs to be defined in advance by using a Definition operation.
 ///
 /// Args:
@@ -32,54 +34,54 @@
 ///
 pub struct MeasureQubit {
     qubit: usize,
     readout: String,
     readout_index: usize,
 }
 
-#[wrap(Operate, OperatePragma)]
+#[wrap(Operate, OperatePragma, JsonSchema)]
 /// This PRAGMA measurement operation returns the statevector of a quantum register.
 ///
 /// Args:
 ///     readout (string): The name of the classical readout register.
 ///     circuit (Optional[Circuit]): The measurement preparation Circuit, applied on a copy of the register before measurement.
 ///
 pub struct PragmaGetStateVector {
     readout: String,
     circuit: Option<Circuit>,
 }
 
-#[wrap(Operate, OperatePragma)]
+#[wrap(Operate, OperatePragma, JsonSchema)]
 /// This PRAGMA measurement operation returns the density matrix of a quantum register.
 ///
 /// Args:
 ///     readout (string): The name of the classical readout register.
 ///     circuit (Optional[Circuit]): The measurement preparation Circuit, applied on a copy of the register before measurement.
 ///
 struct PragmaGetDensityMatrix {
     readout: String,
     circuit: Option<Circuit>,
 }
 
-#[wrap(Operate, OperatePragma)]
+#[wrap(Operate, OperatePragma, JsonSchema)]
 /// This PRAGMA measurement operation returns the vector of the occupation probabilities.
 ///
 /// Occupation probabilities in the context of this PRAGMA operation are probabilities of finding the quantum
 /// register in each :math:`\sigma_z` basis state. The quantum register remains unchanged by this PRAGMA measurement operation.
 ///
 /// Args:
 ///     readout (string): The name of the classical readout register.
 ///     circuit (Optional[Circuit]): The Circuit used to rotate the qureg.
 ///
 struct PragmaGetOccupationProbability {
     readout: String,
     circuit: Option<Circuit>,
 }
 
-#[wrap(Operate, OperatePragma)]
+#[wrap(Operate, OperatePragma, JsonSchema)]
 /// This PRAGMA measurement operation returns a Pauli product expectation value.
 ///
 /// This PRAGMA operation returns a Pauli product expectation value after applying
 /// a Rotate to another basis. It performs all of the operation on a clone of the quantum register,
 /// sothat the actual quantum register remains unchanged.
 ///
 /// Args:
@@ -90,15 +92,15 @@
 ///
 struct PragmaGetPauliProduct {
     qubit_paulis: std::collections::HashMap<usize, usize>,
     readout: String,
     circuit: Circuit,
 }
 
-#[wrap(Operate, OperatePragma)]
+#[wrap(Operate, OperatePragma, JsonSchema)]
 #[derive(Eq)]
 /// This PRAGMA measurement operation returns a measurement record for N repeated measurements.
 ///
 /// Args:
 ///     readout (string): The name of the classical readout register.
 ///     qubit_mapping (dict[int, int]): The mapping of qubits to indices in readout register.
 ///     number_measurements (int): The number of times to repeat the measurement.
```

### Comparing `qoqo-1.6.0a1/src/operations/mod.rs` & `qoqo-1.6.0a2/src/operations/mod.rs`

 * *Files identical despite different names*

### Comparing `qoqo-1.6.0a1/src/operations/multi_qubit_gate_operations.rs` & `qoqo-1.6.0a2/src/operations/multi_qubit_gate_operations.rs`

 * *Files 24% similar despite different names*

```diff
@@ -17,31 +17,47 @@
 use pyo3::prelude::*;
 use pyo3::types::PySet;
 use qoqo_calculator::CalculatorFloat;
 use qoqo_calculator_pyo3::convert_into_calculator_float;
 use qoqo_calculator_pyo3::CalculatorFloatWrapper;
 use qoqo_macros::*;
 use roqoqo::operations::*;
+#[cfg(feature = "json_schema")]
+use roqoqo::ROQOQO_VERSION;
 use std::collections::HashMap;
 
 #[allow(clippy::upper_case_acronyms)]
-#[wrap(Operate, Rotate, OperateMultiQubit, OperateGate, OperateMultiQubitGate)]
+#[wrap(
+    Operate,
+    Rotate,
+    OperateMultiQubit,
+    OperateGate,
+    OperateMultiQubitGate,
+    JsonSchema
+)]
 /// The Molmer-Sorensen gate between multiple qubits.
 ///
 /// The gate applies the rotation under the product of Pauli X operators on multiple qubits.
 /// In mathematical terms the gate applies exp(-i * theta/2 * X_i0 * X_i1 * ... * X_in).
 pub struct MultiQubitMS {
     /// The qubits involved in the multi qubit Molmer-Sorensen gate.
     qubits: Vec<usize>,
     /// The angle of the multi qubit Molmer-Sorensen gate.
     theta: CalculatorFloat,
 }
 
 #[allow(clippy::upper_case_acronyms)]
-#[wrap(Operate, Rotate, OperateMultiQubit, OperateGate, OperateMultiQubitGate)]
+#[wrap(
+    Operate,
+    Rotate,
+    OperateMultiQubit,
+    OperateGate,
+    OperateMultiQubitGate,
+    JsonSchema
+)]
 /// The multi qubit Pauli-Z-Product gate.
 ///
 /// The gate applies the rotation under the product of Pauli Z operators on multiple qubits.
 /// In mathematical terms the gate applies exp(-i * theta/2 * Z_i0 * Z_i1 * ... * Z_in).
 pub struct MultiQubitZZ {
     /// The qubits involved in the multi qubit Molmer-Sorensen gate.
     qubits: Vec<usize>,
```

### Comparing `qoqo-1.6.0a1/src/operations/pragma_operations.rs` & `qoqo-1.6.0a2/src/operations/pragma_operations.rs`

 * *Files 7% similar despite different names*

```diff
@@ -19,33 +19,35 @@
 use pyo3::types::PyByteArray;
 use pyo3::types::PySet;
 use qoqo_calculator::CalculatorFloat;
 use qoqo_calculator_pyo3::{convert_into_calculator_float, CalculatorFloatWrapper};
 use qoqo_macros::*;
 use roqoqo::operations::*;
 use roqoqo::Circuit;
+#[cfg(feature = "json_schema")]
+use roqoqo::ROQOQO_VERSION;
 use std::collections::HashMap;
 
 /// Wrap function automatically generates functions in these traits.
-#[wrap(Operate, OperatePragma)]
+#[wrap(Operate, OperatePragma, JsonSchema)]
 #[derive(Eq)]
 /// This PRAGMA operation sets the number of measurements of the circuit.
 ///
 /// This is used for backends that allow setting the number of tries. However, setting the number of
 /// measurements does not allow access to the underlying wavefunction or density matrix.
 ///
 /// Args:
 ///     number_measurements (uint): The number of measurements.
 ///     readout (string): The register for the readout.
 struct PragmaSetNumberOfMeasurements {
     number_measurements: usize,
     readout: String,
 }
 
-#[wrap(Operate, OperatePragma)]
+#[wrap(Operate, OperatePragma, JsonSchema)]
 /// This PRAGMA measurement operation returns the statevector of a quantum register.
 ///
 /// Args:
 ///     repetitions (CalculatorFloat): The number of repetitions as a symbolic float. At evaluation the floor of any float value is taken
 ///     circuit (Circuit): The Circuit that is looped.
 ///
 pub struct PragmaLoop {
@@ -309,14 +311,46 @@
                 Ok(Operation::from(self.internal.clone()) != other)
             }
             _ => Err(pyo3::exceptions::PyNotImplementedError::new_err(
                 "Other comparison not implemented.",
             )),
         }
     }
+
+    #[cfg(feature = "json_schema")]
+    /// Return the JsonSchema for the json serialisation of the class.
+    ///
+    /// Returns:
+    ///     str: The json schema serialized to json
+    #[staticmethod]
+    pub fn json_schema() -> String {
+        let schema = schemars::schema_for!(PragmaSetStateVector);
+        serde_json::to_string_pretty(&schema).expect("Unexpected failure to serialize schema")
+    }
+
+    #[cfg(feature = "json_schema")]
+    /// Returns the current version of the qoqo library .
+    ///
+    /// Returns:
+    ///     str: The current version of the library.
+    #[staticmethod]
+    pub fn current_version() -> String {
+        ROQOQO_VERSION.to_string()
+    }
+
+    #[cfg(feature = "json_schema")]
+    /// Return the minimum version of qoqo that supports this object.
+    ///
+    /// Returns:
+    ///     str: The minimum version of the qoqo library to deserialize this object.
+    pub fn min_supported_version(&self) -> String {
+        let min_version: (u32, u32, u32) =
+            PragmaSetStateVector::minimum_supported_roqoqo_version(&self.internal);
+        format!("{}.{}.{}", min_version.0, min_version.1, min_version.2)
+    }
 }
 
 /// Module containing the PragmaSetDensityMatrix class.
 #[pymodule]
 fn pragma_set_density_matrix(_py: Python, module: &PyModule) -> PyResult<()> {
     module.add_class::<PragmaSetDensityMatrixWrapper>()?;
     Ok(())
@@ -531,30 +565,62 @@
                 Ok(Operation::from(self.internal.clone()) != other)
             }
             _ => Err(pyo3::exceptions::PyNotImplementedError::new_err(
                 "Other comparison not implemented.",
             )),
         }
     }
+
+    #[cfg(feature = "json_schema")]
+    /// Return the JsonSchema for the json serialisation of the class.
+    ///
+    /// Returns:
+    ///     str: The json schema serialized to json
+    #[staticmethod]
+    pub fn json_schema() -> String {
+        let schema = schemars::schema_for!(PragmaSetDensityMatrix);
+        serde_json::to_string_pretty(&schema).expect("Unexpected failure to serialize schema")
+    }
+
+    #[cfg(feature = "json_schema")]
+    /// Returns the current version of the qoqo library .
+    ///
+    /// Returns:
+    ///     str: The current version of the library.
+    #[staticmethod]
+    pub fn current_version() -> String {
+        ROQOQO_VERSION.to_string()
+    }
+
+    #[cfg(feature = "json_schema")]
+    /// Return the minimum version of qoqo that supports this object.
+    ///
+    /// Returns:
+    ///     str: The minimum version of the qoqo library to deserialize this object.
+    pub fn min_supported_version(&self) -> String {
+        let min_version: (u32, u32, u32) =
+            PragmaSetDensityMatrix::minimum_supported_roqoqo_version(&self.internal);
+        format!("{}.{}.{}", min_version.0, min_version.1, min_version.2)
+    }
 }
 
-#[wrap(Operate, OperatePragma)]
+#[wrap(Operate, OperatePragma, JsonSchema)]
 #[derive(Eq)]
 /// The repeated gate PRAGMA operation.
 ///
 /// This PRAGMA operation repeats the next gate in the circuit the given number of times
 /// to increase the rate for error mitigation.
 ///
 /// Args:
 ///     repetition_coefficient (int): The number of times the following gate is repeated.
 struct PragmaRepeatGate {
     repetition_coefficient: usize,
 }
 
-#[wrap(Operate, OperatePragma, OperateMultiQubit)]
+#[wrap(Operate, OperatePragma, OperateMultiQubit, JsonSchema)]
 /// The statistical overrotation PRAGMA operation.
 ///
 /// This PRAGMA applies a statistical overrotation to the next rotation gate in the circuit, which
 /// matches the hqslang name in the `gate` parameter of PragmaOverrotation and the involved qubits in `qubits`.
 ///
 /// The applied overrotation corresponds to adding a random number to the rotation angle.
 /// The random number is drawn from a normal distribution with mean `0`
@@ -570,98 +636,99 @@
 struct PragmaOverrotation {
     gate_hqslang: String,
     qubits: Vec<usize>,
     amplitude: f64,
     variance: f64,
 }
 
-#[wrap(Operate, OperatePragma)]
+#[wrap(Operate, OperatePragma, JsonSchema)]
 /// This PRAGMA operation boosts noise and overrotations in the circuit.
 ///
 /// Args:
 ///     noise_coefficient (CalculatorFloat): The coefficient by which the noise is boosted.
 struct PragmaBoostNoise {
     noise_coefficient: CalculatorFloat,
 }
 
-#[wrap(Operate, OperateMultiQubit, OperatePragma)]
+#[wrap(Operate, OperateMultiQubit, OperatePragma, JsonSchema)]
 /// This PRAGMA operation signals the STOP of a parallel execution block.
 ///
 /// Args:
 ///     qubits (list[int]): The qubits involved in parallel execution block.
 ///     execution_time (CalculatorFloat): The time for the execution of the block in seconds.
 struct PragmaStopParallelBlock {
     qubits: Vec<usize>,
     execution_time: CalculatorFloat,
 }
 
-#[wrap(Operate)]
+#[wrap(Operate, JsonSchema)]
 /// The global phase PRAGMA operation.
 ///
 /// This PRAGMA operation signals that the quantum register picks up a global phase,
 /// i.e. it provides information that there is a global phase to be considered.
 ///
 /// Args:
 ///     phase (CalculatorFloat): The picked up global phase.
 struct PragmaGlobalPhase {
     phase: CalculatorFloat,
 }
 
-#[wrap(Operate, OperateMultiQubit, OperatePragma)]
+#[wrap(Operate, OperateMultiQubit, OperatePragma, JsonSchema)]
 /// This PRAGMA operation makes the quantum hardware wait a given amount of time.
 ///
 /// This PRAGMA operation is used for error mitigation reasons, for instance.
 /// It can be used to boost the noise on the qubits since it gets worse with time.
 ///
 /// Args:
 ///     qubits (list[int]): The qubits involved in the sleep block.
 ///     sleep_time (CalculatorFloat): The time for the execution of the block in seconds.
 pub struct PragmaSleep {
     qubits: Vec<usize>,
     sleep_time: CalculatorFloat,
 }
 
-#[wrap(Operate, OperateSingleQubit, OperatePragma)]
+#[wrap(Operate, OperateSingleQubit, OperatePragma, JsonSchema)]
 #[derive(Eq)]
 /// This PRAGMA operation resets the chosen qubit to the zero state.
 ///
 /// Args:
 ///     qubit (int): The qubit to be reset.
 pub struct PragmaActiveReset {
     qubit: usize,
 }
 
-#[wrap(Operate, OperateMultiQubit, OperatePragma)]
+#[wrap(Operate, OperateMultiQubit, OperatePragma, JsonSchema)]
 #[derive(Eq)]
 /// This PRAGMA operation signals the START of a decomposition block.
 ///
 /// Args:
 ///     qubits (list[int]): The qubits involved in the decomposition block.
 ///     reordering_dictionary dict[int, int]): The reordering dictionary of the block.
 pub struct PragmaStartDecompositionBlock {
     qubits: Vec<usize>,
     reordering_dictionary: HashMap<usize, usize>,
 }
 
-#[wrap(Operate, OperateMultiQubit, OperatePragma)]
+#[wrap(Operate, OperateMultiQubit, OperatePragma, JsonSchema)]
 #[derive(Eq)]
 /// This PRAGMA operation signals the STOP of a decomposition block.
 ///
 /// Args:
 ///     qubits (list[int]): The qubits involved in the decomposition block.
 pub struct PragmaStopDecompositionBlock {
     qubits: Vec<usize>,
 }
 
 #[wrap(
     Operate,
     OperateSingleQubit,
     OperatePragma,
     OperatePragmaNoise,
-    OperatePragmaNoiseProba
+    OperatePragmaNoiseProba,
+    JsonSchema
 )]
 /// The damping PRAGMA noise operation.
 ///
 /// This PRAGMA operation applies a pure damping error corresponding to zero temperature environments.
 ///
 /// Note
 ///
@@ -719,15 +786,16 @@
 // }
 
 #[wrap(
     Operate,
     OperateSingleQubit,
     OperatePragma,
     OperatePragmaNoise,
-    OperatePragmaNoiseProba
+    OperatePragmaNoiseProba,
+    JsonSchema
 )]
 /// The depolarising PRAGMA noise operation.
 ///
 /// This PRAGMA operation applies a depolarising error corresponding to infinite temperature environments.
 ///
 /// Args:
 ///     qubit (int): The qubit on which to apply the depolarising.
@@ -778,15 +846,16 @@
 // }
 
 #[wrap(
     Operate,
     OperateSingleQubit,
     OperatePragma,
     OperatePragmaNoise,
-    OperatePragmaNoiseProba
+    OperatePragmaNoiseProba,
+    JsonSchema
 )]
 /// The dephasing PRAGMA noise operation.
 ///
 /// This PRAGMA operation applies a pure dephasing error.
 ///
 /// Args:
 ///     qubit (int): The qubit on which to apply the dephasing.
@@ -837,15 +906,16 @@
 // }
 
 #[wrap(
     Operate,
     OperateSingleQubit,
     OperatePragma,
     OperatePragmaNoise,
-    OperatePragmaNoiseProba
+    OperatePragmaNoiseProba,
+    JsonSchema
 )]
 /// The random noise PRAGMA operation.
 ///
 /// This PRAGMA operation applies a pure damping error corresponding to zero temperature environments.
 ///
 /// Args:
 ///     qubit (int): The qubit on which to apply the damping.
@@ -1189,32 +1259,64 @@
                 Ok(Operation::from(self.internal.clone()) != other)
             }
             _ => Err(pyo3::exceptions::PyNotImplementedError::new_err(
                 "Other comparison not implemented.",
             )),
         }
     }
+
+    #[cfg(feature = "json_schema")]
+    /// Return the JsonSchema for the json serialisation of the class.
+    ///
+    /// Returns:
+    ///     str: The json schema serialized to json
+    #[staticmethod]
+    pub fn json_schema() -> String {
+        let schema = schemars::schema_for!(PragmaGeneralNoise);
+        serde_json::to_string_pretty(&schema).expect("Unexpected failure to serialize schema")
+    }
+
+    #[cfg(feature = "json_schema")]
+    /// Returns the current version of the qoqo library .
+    ///
+    /// Returns:
+    ///     str: The current version of the library.
+    #[staticmethod]
+    pub fn current_version() -> String {
+        ROQOQO_VERSION.to_string()
+    }
+
+    #[cfg(feature = "json_schema")]
+    /// Return the minimum version of qoqo that supports this object.
+    ///
+    /// Returns:
+    ///     str: The minimum version of the qoqo library to deserialize this object.
+    pub fn min_supported_version(&self) -> String {
+        let min_version: (u32, u32, u32) =
+            PragmaGeneralNoise::minimum_supported_roqoqo_version(&self.internal);
+        format!("{}.{}.{}", min_version.0, min_version.1, min_version.2)
+    }
 }
 
-#[wrap(Operate, OperatePragma)]
+#[wrap(Operate, OperatePragma, JsonSchema)]
 /// The conditional PRAGMA operation.
 ///
 /// This PRAGMA executes a circuit when the condition bit/bool stored in a classical bit register is true.
 ///
 /// Args:
 ///     condition_register (str): The name of the bit register containting the condition bool value.
 ///     condition_index (int): - The index in the bit register containting the condition bool value.
 ///     circuit (Circuit): - The circuit executed if the condition is met.
 pub struct PragmaConditional {
     condition_register: String,
     condition_index: usize,
     circuit: Circuit,
 }
 
-#[wrap(Operate, OperatePragma)]
+#[wrap(Operate, OperatePragma, JsonSchema)]
 /// A circuit controlled by a qubit.
 ///
 /// The circuit is applied when the qubit is in state 1.
 /// Note that this is a unitary operation (for example a CNOT(0,1)
 /// is equvalent to a PragmaControlledCircuit(0, [PauliX(1)]) but it cannot be represented
 /// by a unitary operation in qoqo for arbitraty circuits.
 ///
@@ -1450,14 +1552,46 @@
                 Ok(Operation::from(self.internal.clone()) != other)
             }
             _ => Err(pyo3::exceptions::PyNotImplementedError::new_err(
                 "Other comparison not implemented.",
             )),
         }
     }
+
+    #[cfg(feature = "json_schema")]
+    /// Return the JsonSchema for the json serialisation of the class.
+    ///
+    /// Returns:
+    ///     str: The json schema serialized to json
+    #[staticmethod]
+    pub fn json_schema() -> String {
+        let schema = schemars::schema_for!(PragmaChangeDevice);
+        serde_json::to_string_pretty(&schema).expect("Unexpected failure to serialize schema")
+    }
+
+    #[cfg(feature = "json_schema")]
+    /// Returns the current version of the qoqo library .
+    ///
+    /// Returns:
+    ///     str: The current version of the library.
+    #[staticmethod]
+    pub fn current_version() -> String {
+        ROQOQO_VERSION.to_string()
+    }
+
+    #[cfg(feature = "json_schema")]
+    /// Return the minimum version of qoqo that supports this object.
+    ///
+    /// Returns:
+    ///     str: The minimum version of the qoqo library to deserialize this object.
+    pub fn min_supported_version(&self) -> String {
+        let min_version: (u32, u32, u32) =
+            PragmaChangeDevice::minimum_supported_roqoqo_version(&self.internal);
+        format!("{}.{}.{}", min_version.0, min_version.1, min_version.2)
+    }
 }
 
 #[cfg(test)]
 mod tests {
     use crate::operations::*;
     use bincode::serialize;
     use roqoqo::operations::*;
```

### Comparing `qoqo-1.6.0a1/src/operations/single_qubit_gate_operations.rs` & `qoqo-1.6.0a2/src/operations/single_qubit_gate_operations.rs`

 * *Files 11% similar despite different names*

```diff
@@ -15,17 +15,25 @@
 use pyo3::exceptions::{PyRuntimeError, PyValueError};
 use pyo3::prelude::*;
 use pyo3::types::PySet;
 use qoqo_calculator::CalculatorFloat;
 use qoqo_calculator_pyo3::{convert_into_calculator_float, CalculatorFloatWrapper};
 use qoqo_macros::*;
 use roqoqo::operations::*;
+#[cfg(feature = "json_schema")]
+use roqoqo::ROQOQO_VERSION;
 use std::collections::HashMap;
 
-#[wrap(Operate, OperateSingleQubit, OperateSingleQubitGate, OperateGate)]
+#[wrap(
+    Operate,
+    OperateSingleQubit,
+    OperateSingleQubitGate,
+    OperateGate,
+    JsonSchema
+)]
 /// The general single qubit unitary gate.
 ///
 /// .. math::
 ///     U =\begin{pmatrix}
 ///         \alpha_r+i \alpha_i & -\beta_r+i \beta_i \\\\
 ///         \beta_r+i \beta_i & \alpha_r-i\alpha_i
 ///         \end{pmatrix}
@@ -48,15 +56,16 @@
 }
 
 #[wrap(
     Operate,
     OperateSingleQubit,
     Rotate,
     OperateGate,
-    OperateSingleQubitGate
+    OperateSingleQubitGate,
+    JsonSchema
 )]
 /// The XPower gate :math:`e^{-i \frac{\theta}{2} \sigma^x}`.
 ///
 /// .. math::
 ///     U = \begin{pmatrix}
 ///         \cos(\frac{\theta}{2}) & 0 \\\\
 ///         0 & \cos(\frac{\theta}{2})
@@ -76,15 +85,16 @@
 }
 
 #[wrap(
     Operate,
     OperateSingleQubit,
     Rotate,
     OperateGate,
-    OperateSingleQubitGate
+    OperateSingleQubitGate,
+    JsonSchema
 )]
 /// The YPower gate :math:`e^{-i \frac{\theta}{2} \sigma^y}`.
 ///
 /// .. math::
 ///     U = \begin{pmatrix}
 ///         \cos(\frac{\theta}{2}) & 0 \\\\
 ///         0 & \cos(\frac{\theta}{2})
@@ -104,15 +114,16 @@
 }
 
 #[wrap(
     Operate,
     OperateSingleQubit,
     Rotate,
     OperateGate,
-    OperateSingleQubitGate
+    OperateSingleQubitGate,
+    JsonSchema
 )]
 /// The ZPower gate :math:`e^{-i \frac{\theta}{2} \sigma^z}`.
 ///
 /// .. math::
 ///     U = \begin{pmatrix}
 ///         \cos(\frac{\theta}{2}) & 0 \\\\
 ///         0 & \cos(\frac{\theta}{2})
@@ -132,15 +143,16 @@
 }
 
 #[wrap(
     Operate,
     OperateSingleQubit,
     Rotate,
     OperateGate,
-    OperateSingleQubitGate
+    OperateSingleQubitGate,
+    JsonSchema
 )]
 /// The phase shift gate applied on state |1>.
 ///
 /// Rotation around Z-axis by an arbitrary angle $\theta$ (AC Stark shift of the state |1>).
 ///
 /// .. math::
 ///     U = \begin{pmatrix}
@@ -158,15 +170,16 @@
 }
 
 #[wrap(
     Operate,
     OperateSingleQubit,
     Rotate,
     OperateGate,
-    OperateSingleQubitGate
+    OperateSingleQubitGate,
+    JsonSchema
 )]
 /// The phase shift gate applied on state |0>.
 ///
 /// Rotation around Z-axis by an arbitrary angle $\theta$ (AC Stark shift of the state |0>).
 ///
 /// .. math::
 ///     U = \begin{pmatrix}
@@ -179,15 +192,21 @@
 ///     theta (CalculatorFloat): The angle :math:`\theta` of the rotation.
 ///
 struct PhaseShiftState0 {
     qubit: usize,
     theta: CalculatorFloat,
 }
 
-#[wrap(Operate, OperateSingleQubit, OperateGate, OperateSingleQubitGate)]
+#[wrap(
+    Operate,
+    OperateSingleQubit,
+    OperateGate,
+    OperateSingleQubitGate,
+    JsonSchema
+)]
 #[derive(Eq)]
 /// The Pauli X gate.
 ///
 /// .. math::
 ///     U = \begin{pmatrix}
 ///         0 & 1 \\\\
 ///         1 & 0
@@ -196,15 +215,21 @@
 /// Args:
 ///     qubit (int): The qubit the unitary gate is applied to.
 ///
 struct PauliX {
     qubit: usize,
 }
 
-#[wrap(Operate, OperateSingleQubit, OperateGate, OperateSingleQubitGate)]
+#[wrap(
+    Operate,
+    OperateSingleQubit,
+    OperateGate,
+    OperateSingleQubitGate,
+    JsonSchema
+)]
 #[derive(Eq)]
 /// The Pauli Y gate.
 ///
 /// .. math::
 ///     U = \begin{pmatrix}
 ///         0 & -i \\\\
 ///         i & 0
@@ -213,15 +238,21 @@
 /// Args:
 ///     qubit (int): The qubit the unitary gate is applied to.
 ///
 struct PauliY {
     qubit: usize,
 }
 
-#[wrap(Operate, OperateSingleQubit, OperateGate, OperateSingleQubitGate)]
+#[wrap(
+    Operate,
+    OperateSingleQubit,
+    OperateGate,
+    OperateSingleQubitGate,
+    JsonSchema
+)]
 #[derive(Eq)]
 /// The Pauli Z gate.
 ///
 /// .. math::
 ///     U = \begin{pmatrix}
 ///         1 & 0 \\\\
 ///         0 & -1
@@ -230,15 +261,21 @@
 /// Args:
 ///     qubit (int): The qubit the unitary gate is applied to.
 ///
 struct PauliZ {
     qubit: usize,
 }
 
-#[wrap(Operate, OperateSingleQubit, OperateGate, OperateSingleQubitGate)]
+#[wrap(
+    Operate,
+    OperateSingleQubit,
+    OperateGate,
+    OperateSingleQubitGate,
+    JsonSchema
+)]
 #[derive(Eq)]
 /// The square root of the XPower gate :math:`e^{-i \frac{\pi}{4} \sigma^x}`.
 ///
 /// .. math::
 ///     U = \frac{1}{\sqrt(2)}\begin{pmatrix}
 ///         1 & -i \\\\
 ///         -i & 1
@@ -247,15 +284,21 @@
 /// Args:
 ///     qubit (int): The qubit the unitary gate is applied to.
 ///
 struct SqrtPauliX {
     qubit: usize,
 }
 
-#[wrap(Operate, OperateSingleQubit, OperateGate, OperateSingleQubitGate)]
+#[wrap(
+    Operate,
+    OperateSingleQubit,
+    OperateGate,
+    OperateSingleQubitGate,
+    JsonSchema
+)]
 #[derive(Eq)]
 /// The inverse square root XPower gate :math:`e^{i \frac{\pi}{2} \sigma^x}`.
 ///
 /// .. math::
 ///     U = \frac{1}{\sqrt{2}} \begin{pmatrix}
 ///         1 & i \\\\
 ///         i & 1
@@ -264,15 +307,21 @@
 /// Args:
 ///     qubit (int): The qubit the unitary gate is applied to.
 ///
 struct InvSqrtPauliX {
     qubit: usize,
 }
 
-#[wrap(Operate, OperateSingleQubit, OperateGate, OperateSingleQubitGate)]
+#[wrap(
+    Operate,
+    OperateSingleQubit,
+    OperateGate,
+    OperateSingleQubitGate,
+    JsonSchema
+)]
 #[derive(Eq)]
 /// The Hadamard gate.
 ///
 /// .. math::
 ///     U = \frac{1}{\sqrt{2}} \begin{pmatrix}
 ///         1 & 1\\\\
 ///         1 & -1
@@ -281,15 +330,21 @@
 /// Args:
 ///     qubit (int): The qubit the unitary gate is applied to.
 ///
 struct Hadamard {
     qubit: usize,
 }
 
-#[wrap(Operate, OperateSingleQubit, OperateGate, OperateSingleQubitGate)]
+#[wrap(
+    Operate,
+    OperateSingleQubit,
+    OperateGate,
+    OperateSingleQubitGate,
+    JsonSchema
+)]
 #[derive(Eq)]
 /// The S gate.
 ///
 /// .. math::
 ///     U = \frac{1}{\sqrt{2}} \begin{pmatrix}
 ///         1 & 0 \\\\
 ///         0 & i
@@ -297,15 +352,21 @@
 ///
 /// Args:
 ///     qubit (int): The qubit the unitary gate is applied to.
 ///
 struct SGate {
     qubit: usize,
 }
-#[wrap(Operate, OperateSingleQubit, OperateGate, OperateSingleQubitGate)]
+#[wrap(
+    Operate,
+    OperateSingleQubit,
+    OperateGate,
+    OperateSingleQubitGate,
+    JsonSchema
+)]
 #[derive(Eq)]
 /// The T gate.
 ///
 /// .. math::
 ///     U = \frac{1}{\sqrt{2}} \begin{pmatrix}
 ///         1 & 0 \\\\
 ///         0 & e^{i \frac{\pi}{4}}
@@ -319,15 +380,16 @@
 }
 
 #[wrap(
     Operate,
     OperateSingleQubit,
     Rotate,
     OperateGate,
-    OperateSingleQubitGate
+    OperateSingleQubitGate,
+    JsonSchema
 )]
 /// Implements a rotation around an axis in the x-y plane in spherical coordinates.
 ///
 /// .. math::
 ///     U = \begin{pmatrix}
 ///         \cos(\frac{\theta}{2}) & 0 \\\\
 ///         0 & \cos(\frac{\theta}{2})
@@ -358,15 +420,16 @@
 }
 
 #[wrap(
     Operate,
     OperateSingleQubit,
     Rotate,
     OperateGate,
-    OperateSingleQubitGate
+    OperateSingleQubitGate,
+    JsonSchema
 )]
 /// Implements a rotation around an axis in the x-y plane in spherical coordinates.
 ///
 /// .. math::
 /// U = \begin{pmatrix}
 /// \cos(\frac{\theta}{2}) & -i e^{-i \phi} \sin(\frac{\theta}{2})\\\\
 /// -i e^{i \phi} \sin(\frac{\theta}{2}) & \cos(\frac{\theta}{2})
@@ -384,15 +447,16 @@
 }
 
 #[wrap(
     Operate,
     OperateSingleQubit,
     Rotate,
     OperateGate,
-    OperateSingleQubitGate
+    OperateSingleQubitGate,
+    JsonSchema
 )]
 /// Implements a pi-rotation with an embedded phase.
 ///
 /// .. math::
 /// U = \begin{pmatrix}
 /// 0 & e^{-i \theta}\\\\
 /// e^{i \theta} & 0
@@ -408,15 +472,16 @@
 }
 
 #[wrap(
     Operate,
     OperateSingleQubit,
     Rotate,
     OperateGate,
-    OperateSingleQubitGate
+    OperateSingleQubitGate,
+    JsonSchema
 )]
 /// Implements a pi/2-rotation with an embedded phase.
 ///
 /// .. math::
 /// U = \frac{1}{\sqrt{2}} \begin{pmatrix}
 /// 1 & -i e^{-i \theta}\\\\
 /// -i e^{i \theta} & 1
```

### Comparing `qoqo-1.6.0a1/src/operations/three_qubit_gate_operations.rs` & `qoqo-1.6.0a2/src/operations/three_qubit_gate_operations.rs`

 * *Files 5% similar despite different names*

```diff
@@ -17,23 +17,31 @@
 use pyo3::prelude::*;
 use pyo3::types::PySet;
 
 use qoqo_calculator::CalculatorFloat;
 use qoqo_calculator_pyo3::{convert_into_calculator_float, CalculatorFloatWrapper};
 
 use roqoqo::operations::*;
+#[cfg(feature = "json_schema")]
+use roqoqo::ROQOQO_VERSION;
 
 use std::collections::HashMap;
 
 use crate::CircuitWrapper;
 
 use qoqo_macros::*;
 
 #[allow(clippy::upper_case_acronyms)]
-#[wrap(Operate, OperateThreeQubit, OperateGate, OperateThreeQubitGate)]
+#[wrap(
+    Operate,
+    OperateThreeQubit,
+    OperateGate,
+    OperateThreeQubitGate,
+    JsonSchema
+)]
 #[derive(Eq)]
 /// Implements the double-controlled PauliZ gate.
 ///
 /// .. math::
 ///     U = \begin{pmatrix}
 ///         1 & 0 & 0 & 0 & 0 & 0 & 0 & 0 \\\\
 ///         0 & 1 & 0 & 0 & 0 & 0 & 0 & 0 \\\\
@@ -52,15 +60,22 @@
 pub struct ControlledControlledPauliZ {
     control_0: usize,
     control_1: usize,
     target: usize,
 }
 
 #[allow(clippy::upper_case_acronyms)]
-#[wrap(Operate, OperateThreeQubit, Rotate, OperateGate, OperateThreeQubitGate)]
+#[wrap(
+    Operate,
+    OperateThreeQubit,
+    Rotate,
+    OperateGate,
+    OperateThreeQubitGate,
+    JsonSchema
+)]
 /// Implements the double-controlled PhaseShift gate.
 ///
 /// .. math::
 ///     U = \begin{pmatrix}
 ///         1 & 0 & 0 & 0 & 0 & 0 & 0 & 0 \\\\
 ///         0 & 1 & 0 & 0 & 0 & 0 & 0 & 0 \\\\
 ///         0 & 0 & 1 & 0 & 0 & 0 & 0 & 0 \\\\
@@ -80,15 +95,21 @@
     control_0: usize,
     control_1: usize,
     target: usize,
     theta: CalculatorFloat,
 }
 
 #[allow(clippy::upper_case_acronyms)]
-#[wrap(Operate, OperateThreeQubit, OperateGate, OperateThreeQubitGate)]
+#[wrap(
+    Operate,
+    OperateThreeQubit,
+    OperateGate,
+    OperateThreeQubitGate,
+    JsonSchema
+)]
 /// Implements Toffoli gate.
 ///
 /// .. math::
 ///     U = \begin{pmatrix}
 ///         1 & 0 & 0 & 0 & 0 & 0 & 0 & 0 \\\\
 ///         0 & 1 & 0 & 0 & 0 & 0 & 0 & 0 \\\\
 ///         0 & 0 & 1 & 0 & 0 & 0 & 0 & 0 \\\\
```

### Comparing `qoqo-1.6.0a1/src/operations/two_qubit_gate_operations.rs` & `qoqo-1.6.0a2/src/operations/two_qubit_gate_operations.rs`

 * *Files 8% similar despite different names*

```diff
@@ -15,18 +15,20 @@
 use pyo3::exceptions::{PyRuntimeError, PyValueError};
 use pyo3::prelude::*;
 use pyo3::types::PySet;
 use qoqo_calculator::CalculatorFloat;
 use qoqo_calculator_pyo3::{convert_into_calculator_float, CalculatorFloatWrapper};
 use qoqo_macros::*;
 use roqoqo::operations::*;
+#[cfg(feature = "json_schema")]
+use roqoqo::ROQOQO_VERSION;
 use std::collections::HashMap;
 
 #[allow(clippy::upper_case_acronyms)]
-#[wrap(Operate, OperateTwoQubit, OperateGate, OperateTwoQubitGate)]
+#[wrap(Operate, OperateTwoQubit, OperateGate, OperateTwoQubitGate, JsonSchema)]
 #[derive(Eq)]
 /// The controlled NOT quantum operation.
 ///
 /// .. math::
 ///     U = \begin{pmatrix}
 ///         1 & 0 & 0 & 0 \\\\
 ///         0 & 1 & 0 & 0 \\\\
@@ -40,15 +42,15 @@
 ///
 pub struct CNOT {
     control: usize,
     target: usize,
 }
 
 #[allow(clippy::upper_case_acronyms)]
-#[wrap(Operate, OperateTwoQubit, OperateGate, OperateTwoQubitGate)]
+#[wrap(Operate, OperateTwoQubit, OperateGate, OperateTwoQubitGate, JsonSchema)]
 #[derive(Eq)]
 /// The controlled SWAP quantum operation.
 ///
 /// .. math::
 ///     U = \begin{pmatrix}
 ///         1 & 0 & 0 & 0 \\\\
 ///         0 & 0 & 1 & 0 \\\\
@@ -62,15 +64,15 @@
 ///
 pub struct SWAP {
     control: usize,
     target: usize,
 }
 
 #[allow(clippy::upper_case_acronyms)]
-#[wrap(Operate, OperateTwoQubit, OperateGate, OperateTwoQubitGate)]
+#[wrap(Operate, OperateTwoQubit, OperateGate, OperateTwoQubitGate, JsonSchema)]
 #[derive(Eq)]
 /// The controlled ISwap quantum operation.
 ///
 /// .. math::
 ///     U = \begin{pmatrix}
 ///         1 & 0 & 0 & 0 \\\\
 ///         0 & 0 & i & 0 \\\\
@@ -84,15 +86,15 @@
 ///
 pub struct ISwap {
     control: usize,
     target: usize,
 }
 
 #[allow(clippy::upper_case_acronyms)]
-#[wrap(Operate, OperateTwoQubit, OperateGate, OperateTwoQubitGate)]
+#[wrap(Operate, OperateTwoQubit, OperateGate, OperateTwoQubitGate, JsonSchema)]
 #[derive(Eq)]
 /// The controlled square root ISwap quantum operation.
 ///
 /// .. math::
 ///     U = \begin{pmatrix}
 ///         1 & 0 & 0 & 0 \\\\
 ///         0 & \frac{1}{\sqrt{2}} & \frac{i}{\sqrt{2}} & 0 \\\\
@@ -106,15 +108,15 @@
 ///
 pub struct SqrtISwap {
     control: usize,
     target: usize,
 }
 
 #[allow(clippy::upper_case_acronyms)]
-#[wrap(Operate, OperateTwoQubit, OperateGate, OperateTwoQubitGate)]
+#[wrap(Operate, OperateTwoQubit, OperateGate, OperateTwoQubitGate, JsonSchema)]
 #[derive(Eq)]
 /// The controlled inverse square root ISwap quantum operation.
 ///
 /// .. math::
 ///     U = \begin{pmatrix}
 ///         1 & 0 & 0 & 0 \\\\
 ///         0 & \frac{1}{\sqrt{2}} & \frac{-i}{\sqrt{2}} & 0 \\\\
@@ -128,15 +130,15 @@
 ///
 pub struct InvSqrtISwap {
     control: usize,
     target: usize,
 }
 
 #[allow(clippy::upper_case_acronyms)]
-#[wrap(Operate, OperateTwoQubit, OperateGate, OperateTwoQubitGate)]
+#[wrap(Operate, OperateTwoQubit, OperateGate, OperateTwoQubitGate, JsonSchema)]
 #[derive(Eq)]
 /// The controlled fermionic SWAP gate.
 ///
 /// .. math::
 ///     U = \begin{pmatrix}
 ///         1 & 0 & 0 & 0 \\\\
 ///         0 & 0 & 1 & 0 \\\\
@@ -150,15 +152,15 @@
 ///
 pub struct FSwap {
     control: usize,
     target: usize,
 }
 
 #[allow(clippy::upper_case_acronyms)]
-#[wrap(Operate, OperateTwoQubit, OperateGate, OperateTwoQubitGate)]
+#[wrap(Operate, OperateTwoQubit, OperateGate, OperateTwoQubitGate, JsonSchema)]
 #[derive(Eq)]
 /// The fixed phase MolmerSorensen XX gate. <http://arxiv.org/abs/1705.02771>
 ///
 /// .. math::
 ///     U = \frac{1}{\sqrt{2}} \begin{pmatrix}
 ///         1 & 0 & 0 & -i \\\\
 ///         0 & 1 & -i & 0 \\\\
@@ -172,15 +174,22 @@
 ///
 pub struct MolmerSorensenXX {
     control: usize,
     target: usize,
 }
 
 #[allow(clippy::upper_case_acronyms)]
-#[wrap(Operate, OperateTwoQubit, Rotate, OperateGate, OperateTwoQubitGate)]
+#[wrap(
+    Operate,
+    OperateTwoQubit,
+    Rotate,
+    OperateGate,
+    OperateTwoQubitGate,
+    JsonSchema
+)]
 /// The variable-angle MolmerSorensen XX gate.
 ///
 /// .. math::
 ///     U = \begin{pmatrix}
 ///         \cos(\theta/2) & 0 & 0 & -i \sin(\theta/2) \\\\
 ///         0 & \cos(\theta/2) & -i \sin(\theta/2) & 0 \\\\
 ///         0 & -i \sin(\theta/2) & \cos(\theta/2) & 0 \\\\
@@ -195,15 +204,22 @@
 pub struct VariableMSXX {
     control: usize,
     target: usize,
     theta: CalculatorFloat,
 }
 
 #[allow(clippy::upper_case_acronyms)]
-#[wrap(Operate, OperateTwoQubit, Rotate, OperateGate, OperateTwoQubitGate)]
+#[wrap(
+    Operate,
+    OperateTwoQubit,
+    Rotate,
+    OperateGate,
+    OperateTwoQubitGate,
+    JsonSchema
+)]
 /// The Givens rotation interaction gate in big endian notation: :math:`e^{-\mathrm{i} \theta (X_c Y_t - Y_c X_t)}`.
 ///
 /// Where :math:`X_c` is the Pauli matrix :math:`\sigma^x` acting on the control qubit
 /// and :math:`Y_t` is the Pauli matrix :math:`\sigma^y` acting on the target qubit.
 ///
 /// .. math::
 ///     U = \begin{pmatrix}
@@ -223,15 +239,22 @@
     control: usize,
     target: usize,
     theta: CalculatorFloat,
     phi: CalculatorFloat,
 }
 
 #[allow(clippy::upper_case_acronyms)]
-#[wrap(Operate, OperateTwoQubit, Rotate, OperateGate, OperateTwoQubitGate)]
+#[wrap(
+    Operate,
+    OperateTwoQubit,
+    Rotate,
+    OperateGate,
+    OperateTwoQubitGate,
+    JsonSchema
+)]
 /// The Givens rotation interaction gate in little endian notation: :math:`e^{-\mathrm{i} \theta (X_c Y_t - Y_c X_t)}`.
 ///
 /// Where :math:`X_c` is the Pauli matrix :math:`\sigma^x` acting on the control qubit
 /// and :math:`Y_t` is the Pauli matrix :math:`\sigma^y` acting on the target qubit.
 ///
 /// .. math::
 ///     U = \begin{pmatrix}
@@ -251,15 +274,22 @@
     control: usize,
     target: usize,
     theta: CalculatorFloat,
     phi: CalculatorFloat,
 }
 
 #[allow(clippy::upper_case_acronyms)]
-#[wrap(Operate, OperateTwoQubit, Rotate, OperateGate, OperateTwoQubitGate)]
+#[wrap(
+    Operate,
+    OperateTwoQubit,
+    Rotate,
+    OperateGate,
+    OperateTwoQubitGate,
+    JsonSchema
+)]
 /// The controlled XY quantum operation
 ///
 /// .. math::
 ///     U = \begin{pmatrix}
 ///         1 & 0 & 0 & 0 \\\
 ///         0 & cos(\theta/2) & i sin(\theta/2) & 0 \\\
 ///         0 & i sin(\theta/2) & cos(\theta/2) & 0 \\\
@@ -274,15 +304,22 @@
 pub struct XY {
     control: usize,
     target: usize,
     theta: CalculatorFloat,
 }
 
 #[allow(clippy::upper_case_acronyms)]
-#[wrap(Operate, OperateTwoQubit, Rotate, OperateGate, OperateTwoQubitGate)]
+#[wrap(
+    Operate,
+    OperateTwoQubit,
+    Rotate,
+    OperateGate,
+    OperateTwoQubitGate,
+    JsonSchema
+)]
 /// The controlled-PhaseShift quantum operation.
 ///
 /// .. math::
 ///     U = \begin{pmatrix}
 ///         1 & 0 & 0 & 0 \\\\
 ///         0 & 1 & 0 & 0 \\\\
 ///         0 & 0 & 1 & 0 \\\\
@@ -297,15 +334,15 @@
 pub struct ControlledPhaseShift {
     control: usize,
     target: usize,
     theta: CalculatorFloat,
 }
 
 #[allow(clippy::upper_case_acronyms)]
-#[wrap(Operate, OperateTwoQubit, OperateGate, OperateTwoQubitGate)]
+#[wrap(Operate, OperateTwoQubit, OperateGate, OperateTwoQubitGate, JsonSchema)]
 #[derive(Eq)]
 /// The controlled PauliY quantum operation
 ///
 /// .. math::
 ///     U = \begin{pmatrix}
 ///         1 & 0 & 0 & 0 \\\\
 ///         0 & 1 & 0 & 0 \\\\
@@ -319,15 +356,15 @@
 ///
 pub struct ControlledPauliY {
     control: usize,
     target: usize,
 }
 
 #[allow(clippy::upper_case_acronyms)]
-#[wrap(Operate, OperateTwoQubit, OperateGate, OperateTwoQubitGate)]
+#[wrap(Operate, OperateTwoQubit, OperateGate, OperateTwoQubitGate, JsonSchema)]
 #[derive(Eq)]
 /// The controlled PauliZ quantum operation
 ///
 /// .. math::
 ///     U = \begin{pmatrix}
 ///         1 & 0 & 0 & 0 \\\\
 ///         0 & 1 & 0 & 0 \\\\
@@ -341,15 +378,15 @@
 ///
 pub struct ControlledPauliZ {
     control: usize,
     target: usize,
 }
 
 #[allow(clippy::upper_case_acronyms)]
-#[wrap(Operate, OperateTwoQubit, OperateGate, OperateTwoQubitGate)]
+#[wrap(Operate, OperateTwoQubit, OperateGate, OperateTwoQubitGate, JsonSchema)]
 /// The qubit simulation (Qsim) gate.
 ///
 /// .. math::
 ///     U = \begin{pmatrix}
 ///         \cos(x-y) \cdot e^{-i z} & 0 & 0 & -i\sin(x-y)\cdot e^{-i z}\\\\
 ///         0 & -i \sin(x+y)\cdot e^{i z} & \cos(x+y)\cdot e^{i z} & 0 \\\\
 ///         0 & \cos(x+y)\cdot e^{i z}& -i \sin(x+y)\cdot e^{i z} & 0 \\\\
@@ -368,15 +405,15 @@
     target: usize,
     x: CalculatorFloat,
     y: CalculatorFloat,
     z: CalculatorFloat,
 }
 
 #[allow(clippy::upper_case_acronyms)]
-#[wrap(Operate, OperateTwoQubit, OperateGate, OperateTwoQubitGate)]
+#[wrap(Operate, OperateTwoQubit, OperateGate, OperateTwoQubitGate, JsonSchema)]
 /// The fermionic qubit simulation (Fsim) gate.
 ///
 /// .. math::
 ///     U = \begin{pmatrix}
 ///         \cos(\Delta) & 0 & 0 & i \sin(\Delta) \\\\
 ///         0 & -i \sin(t) & \cos(t) & 0 \\\\
 ///         0 & \cos(t) & -i \sin(t) & 0 \\\\
@@ -399,15 +436,15 @@
     target: usize,
     t: CalculatorFloat,
     u: CalculatorFloat,
     delta: CalculatorFloat,
 }
 
 #[allow(clippy::upper_case_acronyms)]
-#[wrap(Operate, OperateTwoQubit, OperateGate, OperateTwoQubitGate)]
+#[wrap(Operate, OperateTwoQubit, OperateGate, OperateTwoQubitGate, JsonSchema)]
 /// The generalized, anisotropic XYZ Heisenberg interaction between spins.
 ///
 /// :math:`e^{-\mathrm{i} (x \cdot X_c X_t + y \cdot Y_c Y_t + z \cdot Z_c Z_t)}`
 ///
 /// Where x, y, z are prefactors of the :math:`X_c X_t`, :math:`Y_c Y_t`, :math:`Z_c Z_t` Pauliproducts acting on control and target qubit,
 /// with :math:`XX \equiv \sigma_x \sigma_x`, :math:`YY \equiv \sigma_y \sigma_y` and :math:`ZZ \equiv \sigma_z \sigma_z`.
 ///
@@ -423,15 +460,15 @@
     target: usize,
     x: CalculatorFloat,
     y: CalculatorFloat,
     z: CalculatorFloat,
 }
 
 #[allow(clippy::upper_case_acronyms)]
-#[wrap(Operate, OperateTwoQubit, OperateGate, OperateTwoQubitGate)]
+#[wrap(Operate, OperateTwoQubit, OperateGate, OperateTwoQubitGate, JsonSchema)]
 /// The Bogoliubov DeGennes interaction gate.
 ///
 /// :math:`e^{-\mathrm{i} Re(\Delta) (X_c X_t - Y_c Y_t)/2 + Im(\Delta) (X_c Y_t+Y_c X_t)/2}`
 ///
 /// Where :math:`X_c` is the Pauli matrix :math:`\sigma^x` acting on the control qubit
 /// and :math:`Y_t` is the Pauli matrix :math:`\sigma^y` acting on the target qubit.
 ///
@@ -455,15 +492,15 @@
     control: usize,
     target: usize,
     delta_real: CalculatorFloat,
     delta_imag: CalculatorFloat,
 }
 
 #[allow(clippy::upper_case_acronyms)]
-#[wrap(Operate, OperateTwoQubit, OperateGate, OperateTwoQubitGate)]
+#[wrap(Operate, OperateTwoQubit, OperateGate, OperateTwoQubitGate, JsonSchema)]
 /// The transversal interaction gate.
 ///
 /// :math:`e^{-\mathrm{i} \theta (X_c X_t + Y_c Y_t)} = e^{-\mathrm{i} \theta (\sigma^+_c \sigma^-_t + \sigma^-_c \sigma^+_t)}`
 ///
 /// Where :math:`X_c` is the Pauli matrix :math:`\sigma^x` acting on the control qubit
 /// and :math:`Y_t` is the Pauli matrix :math:`\sigma^y` acting on the target qubit.
 ///
@@ -475,15 +512,15 @@
 pub struct PMInteraction {
     control: usize,
     target: usize,
     t: CalculatorFloat,
 }
 
 #[allow(clippy::upper_case_acronyms)]
-#[wrap(Operate, OperateTwoQubit, OperateGate, OperateTwoQubitGate)]
+#[wrap(Operate, OperateTwoQubit, OperateGate, OperateTwoQubitGate, JsonSchema)]
 /// The complex hopping gate.
 ///
 /// :math:`e^{-\mathrm{i} \left[ Re(\theta) \cdot (X_c X_t + Y_c Y_t) - Im(\theta) \cdot (X_c Y_t - Y_c X_t) \right] }`
 ///
 /// Where :math:`X_c` is the Pauli matrix :math:`\sigma^x` acting on the control qubit
 /// and :math:`Y_t` is the Pauli matrix :math:`\sigma^y` acting on the target qubit.
 ///
@@ -497,15 +534,15 @@
     control: usize,
     target: usize,
     t_real: CalculatorFloat,
     t_imag: CalculatorFloat,
 }
 
 #[allow(clippy::upper_case_acronyms)]
-#[wrap(Operate, OperateTwoQubit, OperateGate, OperateTwoQubitGate)]
+#[wrap(Operate, OperateTwoQubit, OperateGate, OperateTwoQubitGate, JsonSchema)]
 /// The phased-shifted controlled-Z gate.
 ///
 /// Modified, i.e. phase-shifted ControlledPauliZ two-qubit gate (`<https://arxiv.org/pdf/1908.06101.pdf eq.(1)>`).
 ///
 /// The unitary matrix representation is:
 ///
 /// .. math::
@@ -524,15 +561,22 @@
 pub struct PhaseShiftedControlledZ {
     control: usize,
     target: usize,
     phi: CalculatorFloat,
 }
 
 #[allow(clippy::upper_case_acronyms)]
-#[wrap(Operate, OperateTwoQubit, Rotate, OperateGate, OperateTwoQubitGate)]
+#[wrap(
+    Operate,
+    OperateTwoQubit,
+    Rotate,
+    OperateGate,
+    OperateTwoQubitGate,
+    JsonSchema
+)]
 /// Implements the phase-shifted controlled PhaseShift gate.
 ///
 /// The unitary matrix representation is:
 ///
 /// .. math::
 ///     U = \begin{pmatrix}
 ///         1 & 0 & 0 & 0 \\\\
@@ -551,15 +595,22 @@
     control: usize,
     target: usize,
     theta: CalculatorFloat,
     phi: CalculatorFloat,
 }
 
 #[allow(clippy::upper_case_acronyms)]
-#[wrap(Operate, OperateTwoQubit, Rotate, OperateGate, OperateTwoQubitGate)]
+#[wrap(
+    Operate,
+    OperateTwoQubit,
+    Rotate,
+    OperateGate,
+    OperateTwoQubitGate,
+    JsonSchema
+)]
 /// Implements the controlled RotateX operation.
 ///
 /// The unitary matrix representation is:
 ///
 /// .. math::
 ///     U = /begin{pmatrix}
 ///         1 & 0 & 0 & 0 \\\\
@@ -575,15 +626,22 @@
 pub struct ControlledRotateX {
     control: usize,
     target: usize,
     theta: CalculatorFloat,
 }
 
 #[allow(clippy::upper_case_acronyms)]
-#[wrap(Operate, OperateTwoQubit, Rotate, OperateGate, OperateTwoQubitGate)]
+#[wrap(
+    Operate,
+    OperateTwoQubit,
+    Rotate,
+    OperateGate,
+    OperateTwoQubitGate,
+    JsonSchema
+)]
 /// Implements the controlled RotateXY operation.
 ///
 /// The unitary matrix representation is:
 ///
 /// .. math::
 ///     U = /begin{pmatrix}
 ///         1 & 0 & 0 & 0 \\\\
```

### Comparing `qoqo-1.6.0a1/src/quantum_program.rs` & `qoqo-1.6.0a2/src/quantum_program.rs`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,16 @@
 };
 use crate::{QoqoError, QOQO_VERSION};
 use bincode::{deserialize, serialize};
 use pyo3::exceptions::{PyRuntimeError, PyTypeError, PyValueError};
 use pyo3::prelude::*;
 use pyo3::types::PyByteArray;
 use roqoqo::measurements::Measure;
+#[cfg(feature = "json_schema")]
+use roqoqo::operations::SupportedVersion;
 use roqoqo::QuantumProgram;
 use roqoqo::ROQOQO_VERSION;
 
 /// Represents a quantum program evaluating measurements based on a one or more free float parameters.
 ///
 /// The main use of QuantumProgram is to contain a Measurements implementing [crate::measurements::Measure]
 /// that measures expectation values or output registers of [crate::Circuit] quantum circuits that contain
@@ -338,26 +340,26 @@
             .map_err(|_| PyValueError::new_err("Cannot serialize QuantumProgram to bytes"))?;
         let b: Py<PyByteArray> = Python::with_gil(|py| -> Py<PyByteArray> {
             PyByteArray::new(py, &serialized[..]).into()
         });
         Ok(b)
     }
 
-    #[staticmethod]
     /// Convert the bincode representation of the QuantumProgram to a QuantumProgram using the [bincode] crate.
     ///
     /// Args:
     ///     input (ByteArray): The serialized QuantumProgram (in [bincode] form).
     ///
     /// Returns:
     ///     QuantumProgram: The deserialized QuantumProgram.
     ///
     /// Raises:
     ///     TypeError: Input cannot be converted to byte array.
     ///     ValueError: Input cannot be deserialized to QuantumProgram.
+    #[staticmethod]
     pub fn from_bincode(input: &PyAny) -> PyResult<Self> {
         let bytes = input
             .extract::<Vec<u8>>()
             .map_err(|_| PyTypeError::new_err("Input cannot be converted to byte array"))?;
 
         Ok(Self {
             internal: deserialize(&bytes[..]).map_err(|_| {
@@ -394,14 +396,46 @@
         Ok(Self {
             internal: serde_json::from_str(input).map_err(|_| {
                 PyValueError::new_err("Input cannot be deserialized to QuantumProgram")
             })?,
         })
     }
 
+    #[cfg(feature = "json_schema")]
+    /// Return the JsonSchema for the json serialisation of the class.
+    ///
+    /// Returns:
+    ///     str: The json schema serialized to json
+    #[staticmethod]
+    pub fn json_schema() -> String {
+        let schema = schemars::schema_for!(QuantumProgram);
+        serde_json::to_string_pretty(&schema).expect("Unexpected failure to serialize schema")
+    }
+
+    #[cfg(feature = "json_schema")]
+    /// Returns the current version of the qoqo library .
+    ///
+    /// Returns:
+    ///     str: The current version of the library.
+    #[staticmethod]
+    pub fn current_version() -> String {
+        ROQOQO_VERSION.to_string()
+    }
+
+    #[cfg(feature = "json_schema")]
+    /// Return the minimum version of qoqo that supports this object.
+    ///
+    /// Returns:
+    ///     str: The minimum version of the qoqo library to deserialize this object.
+    pub fn min_supported_version(&self) -> String {
+        let min_version: (u32, u32, u32) =
+            QuantumProgram::minimum_supported_roqoqo_version(&self.internal);
+        format!("{}.{}.{}", min_version.0, min_version.1, min_version.2)
+    }
+
     /// Return the __richcmp__ magic method to perform rich comparison operations on QuantumProgram.
     ///
     /// Args:
     ///     other: The object to compare self to.
     ///     op: Type of comparison.
     ///
     /// Returns:
```

### Comparing `qoqo-1.6.0a1/Cargo.lock` & `qoqo-1.6.0a2/Cargo.lock`

 * *Files 25% similar despite different names*

```diff
@@ -1,86 +1,356 @@
 # This file is automatically @generated by Cargo.
 # It is not intended for manual editing.
 version = 3
 
 [[package]]
+name = "addr2line"
+version = "0.20.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f4fa78e18c64fce05e902adecd7a5eed15a5e0a3439f7b0e169f0252214865e3"
+dependencies = [
+ "gimli",
+]
+
+[[package]]
+name = "adler"
+version = "1.0.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f26201604c87b1e01bd3d98f8d5d9a8fcbb815e8cedb41ffccbeb4bf593a35fe"
+
+[[package]]
+name = "ahash"
+version = "0.8.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2c99f64d1e06488f620f932677e24bc6e2897582980441ae90a671415bd7ec2f"
+dependencies = [
+ "cfg-if",
+ "getrandom",
+ "once_cell",
+ "serde",
+ "version_check",
+]
+
+[[package]]
+name = "aho-corasick"
+version = "1.0.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "43f6cb1bf222025340178f382c426f13757b2960e89779dfcb319c32542a5a41"
+dependencies = [
+ "memchr",
+]
+
+[[package]]
+name = "anstream"
+version = "0.3.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0ca84f3628370c59db74ee214b3263d58f9aadd9b4fe7e711fd87dc452b7f163"
+dependencies = [
+ "anstyle",
+ "anstyle-parse",
+ "anstyle-query",
+ "anstyle-wincon",
+ "colorchoice",
+ "is-terminal",
+ "utf8parse",
+]
+
+[[package]]
+name = "anstyle"
+version = "1.0.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3a30da5c5f2d5e72842e00bcb57657162cdabef0931f40e2deb9b4140440cecd"
+
+[[package]]
+name = "anstyle-parse"
+version = "0.2.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "938874ff5980b03a87c5524b3ae5b59cf99b1d6bc836848df7bc5ada9643c333"
+dependencies = [
+ "utf8parse",
+]
+
+[[package]]
+name = "anstyle-query"
+version = "1.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5ca11d4be1bab0c8bc8734a9aa7bf4ee8316d462a08c6ac5052f888fef5b494b"
+dependencies = [
+ "windows-sys",
+]
+
+[[package]]
+name = "anstyle-wincon"
+version = "1.0.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "180abfa45703aebe0093f79badacc01b8fd4ea2e35118747e5811127f926e188"
+dependencies = [
+ "anstyle",
+ "windows-sys",
+]
+
+[[package]]
+name = "anyhow"
+version = "1.0.72"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3b13c32d80ecc7ab747b80c3784bce54ee8a7a0cc4fbda9bf4cda2cf6fe90854"
+
+[[package]]
 name = "approx"
 version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "cab112f0a86d568ea0e627cc1d6be74a1e9cd55214684db5561995f6dad897c6"
 dependencies = [
  "num-traits",
 ]
 
 [[package]]
 name = "async-trait"
-version = "0.1.71"
+version = "0.1.72"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a564d521dd56509c4c47480d00b80ee55f7e385ae48db5744c67ad50c92d2ebf"
+checksum = "cc6dde6e4ed435a4c1ee4e73592f5ba9da2151af10076cc04858746af9352d09"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.26",
+ "syn 2.0.27",
 ]
 
 [[package]]
 name = "autocfg"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
 
 [[package]]
+name = "backtrace"
+version = "0.3.68"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4319208da049c43661739c5fade2ba182f09d1dc2299b32298d3a31692b17e12"
+dependencies = [
+ "addr2line",
+ "cc",
+ "cfg-if",
+ "libc",
+ "miniz_oxide",
+ "object",
+ "rustc-demangle",
+]
+
+[[package]]
+name = "base64"
+version = "0.21.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "604178f6c5c21f02dc555784810edfb88d34ac2c73b2eae109655649ee73ce3d"
+
+[[package]]
 name = "bincode"
 version = "1.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b1f45e9417d87227c7a56d22e471c6206462cba514c7590c09aff4cf6d1ddcad"
 dependencies = [
  "serde",
 ]
 
 [[package]]
+name = "bit-set"
+version = "0.5.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0700ddab506f33b20a03b13996eccd309a48e5ff77d0d95926aa0210fb4e95f1"
+dependencies = [
+ "bit-vec",
+]
+
+[[package]]
+name = "bit-vec"
+version = "0.6.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "349f9b6a179ed607305526ca489b34ad0a41aed5f7980fa90eb03160b69598fb"
+
+[[package]]
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
+name = "bitflags"
+version = "2.3.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "630be753d4e58660abd17930c71b647fe46c27ea6b63cc59e1e3851406972e42"
+
+[[package]]
+name = "bumpalo"
+version = "3.13.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a3e2c3daef883ecc1b5d58c15adae93470a91d425f3532ba1695849656af3fc1"
+
+[[package]]
+name = "bytecount"
+version = "0.6.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2c676a478f63e9fa2dd5368a42f28bba0d6c560b775f38583c8bbaa7fcd67c9c"
+
+[[package]]
 name = "bytemuck"
 version = "1.13.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "17febce684fd15d89027105661fec94afb475cb995fbc59d2865198446ba2eea"
 
 [[package]]
+name = "bytes"
+version = "1.4.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "89b2fd2a0dcf38d7971e2194b6b6eebab45ae01067456a7fd93d5547a61b70be"
+
+[[package]]
+name = "cc"
+version = "1.0.79"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "50d30906286121d95be3d479533b458f87493b30a4b5f79a607db8f5d11aa91f"
+
+[[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
+name = "clap"
+version = "4.3.19"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5fd304a20bff958a57f04c4e96a2e7594cc4490a0e809cbd48bb6437edaa452d"
+dependencies = [
+ "clap_builder",
+ "clap_derive",
+ "once_cell",
+]
+
+[[package]]
+name = "clap_builder"
+version = "4.3.19"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "01c6a3f08f1fe5662a35cfe393aec09c4df95f60ee93b7556505260f75eee9e1"
+dependencies = [
+ "anstream",
+ "anstyle",
+ "clap_lex",
+ "strsim",
+]
+
+[[package]]
+name = "clap_derive"
+version = "4.3.12"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "54a9bb5758fc5dfe728d1019941681eccaf0cf8a4189b692a0ee2f2ecf90a050"
+dependencies = [
+ "heck",
+ "proc-macro2",
+ "quote",
+ "syn 2.0.27",
+]
+
+[[package]]
+name = "clap_lex"
+version = "0.5.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2da6da31387c7e4ef160ffab6d5e7f00c42626fe39aea70a7b0f1773f7dd6c1b"
+
+[[package]]
+name = "colorchoice"
+version = "1.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "acbf1af155f9b9ef647e42cdc158db4b64a1b61f743629225fde6f3e0be2a7c7"
+
+[[package]]
 name = "dyn-clone"
 version = "1.0.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "304e6508efa593091e97a9abbc10f90aa7ca635b6d2784feff3c89d41dd12272"
 
 [[package]]
+name = "encoding_rs"
+version = "0.8.32"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "071a31f4ee85403370b58aca746f01041ede6f0da2730960ad001edc2b71b394"
+dependencies = [
+ "cfg-if",
+]
+
+[[package]]
 name = "erased-serde"
 version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "da96524cc884f6558f1769b6c46686af2fe8e8b4cd253bd5a3cdba8181b8e070"
 dependencies = [
  "serde",
 ]
 
 [[package]]
+name = "errno"
+version = "0.3.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4bcfec3a70f97c962c307b2d2c56e358cf1d00b558d74262b5f929ee8cc7e73a"
+dependencies = [
+ "errno-dragonfly",
+ "libc",
+ "windows-sys",
+]
+
+[[package]]
+name = "errno-dragonfly"
+version = "0.1.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "aa68f1b12764fab894d2755d2518754e71b4fd80ecfb822714a1206c2aab39bf"
+dependencies = [
+ "cc",
+ "libc",
+]
+
+[[package]]
+name = "fancy-regex"
+version = "0.11.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b95f7c0680e4142284cf8b22c14a476e87d61b004a3a0861872b32ef7ead40a2"
+dependencies = [
+ "bit-set",
+ "regex",
+]
+
+[[package]]
 name = "fixedbitset"
 version = "0.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0ce7134b9999ecaf8bcd65542e436736ef32ddca1b3e06094cb6ec5755203b80"
 
 [[package]]
+name = "fnv"
+version = "1.0.7"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3f9eec918d3f24069decb9af1554cad7c880e2da24a9afd88aca000531ab82c1"
+
+[[package]]
+name = "form_urlencoded"
+version = "1.2.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a62bc1cf6f830c2ec14a513a9fb124d0a213a629668a4186f329db21fe045652"
+dependencies = [
+ "percent-encoding",
+]
+
+[[package]]
+name = "fraction"
+version = "0.13.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3027ae1df8d41b4bed2241c8fdad4acc1e7af60c8e17743534b545e77182d678"
+dependencies = [
+ "lazy_static",
+ "num",
+]
+
+[[package]]
 name = "futures"
 version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "23342abe12aba583913b2e62f22225ff9c950774065e4bfb61a19cd9770fec40"
 dependencies = [
  "futures-channel",
  "futures-core",
@@ -128,15 +398,15 @@
 name = "futures-macro"
 version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "89ca545a94061b6365f2c7355b4b32bd20df3ff95f02da9329b34ccc3bd6ee72"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.26",
+ "syn 2.0.27",
 ]
 
 [[package]]
 name = "futures-sink"
 version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f43be4fe21a13b9781a69afa4985b0f6ee0e1afab2c6f454a8cf30e2b2237b6e"
@@ -168,25 +438,132 @@
 [[package]]
 name = "getrandom"
 version = "0.2.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "be4136b2a15dd319360be1c07d9933517ccf0be8f16bf62a3bee4f0d618df427"
 dependencies = [
  "cfg-if",
+ "js-sys",
  "libc",
  "wasi",
+ "wasm-bindgen",
+]
+
+[[package]]
+name = "gimli"
+version = "0.27.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b6c80984affa11d98d1b88b66ac8853f143217b399d3c74116778ff8fdb4ed2e"
+
+[[package]]
+name = "h2"
+version = "0.3.20"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "97ec8491ebaf99c8eaa73058b045fe58073cd6be7f596ac993ced0b0a0c01049"
+dependencies = [
+ "bytes",
+ "fnv",
+ "futures-core",
+ "futures-sink",
+ "futures-util",
+ "http",
+ "indexmap",
+ "slab",
+ "tokio",
+ "tokio-util",
+ "tracing",
 ]
 
 [[package]]
 name = "hashbrown"
 version = "0.12.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8a9ee70c43aaf417c914396645a0fa852624801b24ebb7ae78fe8272889ac888"
 
 [[package]]
+name = "heck"
+version = "0.4.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "95505c38b4572b2d910cecb0281560f54b440a19336cbbcb27bf6ce6adc6f5a8"
+
+[[package]]
+name = "hermit-abi"
+version = "0.3.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "443144c8cdadd93ebf52ddb4056d257f5b52c04d3c804e657d19eb73fc33668b"
+
+[[package]]
+name = "http"
+version = "0.2.9"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "bd6effc99afb63425aff9b05836f029929e345a6148a14b7ecd5ab67af944482"
+dependencies = [
+ "bytes",
+ "fnv",
+ "itoa",
+]
+
+[[package]]
+name = "http-body"
+version = "0.4.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d5f38f16d184e36f2408a55281cd658ecbd3ca05cce6d6510a176eca393e26d1"
+dependencies = [
+ "bytes",
+ "http",
+ "pin-project-lite",
+]
+
+[[package]]
+name = "httparse"
+version = "1.8.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d897f394bad6a705d5f4104762e116a75639e470d80901eed05a860a95cb1904"
+
+[[package]]
+name = "httpdate"
+version = "1.0.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c4a1e36c821dbe04574f602848a19f742f4fb3c98d40449f11bcad18d6b17421"
+
+[[package]]
+name = "hyper"
+version = "0.14.27"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ffb1cfd654a8219eaef89881fdb3bb3b1cdc5fa75ded05d6933b2b382e395468"
+dependencies = [
+ "bytes",
+ "futures-channel",
+ "futures-core",
+ "futures-util",
+ "h2",
+ "http",
+ "http-body",
+ "httparse",
+ "httpdate",
+ "itoa",
+ "pin-project-lite",
+ "socket2",
+ "tokio",
+ "tower-service",
+ "tracing",
+ "want",
+]
+
+[[package]]
+name = "idna"
+version = "0.4.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7d20d6b07bfbc108882d88ed8e37d39636dcc260e15e30c45e6ba089610b917c"
+dependencies = [
+ "unicode-bidi",
+ "unicode-normalization",
+]
+
+[[package]]
 name = "indexmap"
 version = "1.9.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bd070e393353796e801d209ad339e89596eb4c8d430d18ede6a1cced8fafbd99"
 dependencies = [
  "autocfg",
  "hashbrown",
@@ -196,47 +573,130 @@
 name = "indoc"
 version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
 
 [[package]]
 name = "inventory"
-version = "0.3.9"
+version = "0.3.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "25b1d6b4b9fb75fc419bdef998b689df5080a32931cb3395b86202046b56a9ea"
+checksum = "a53088c87cf71c9d4f3372a2cb9eea1e7b8a0b1bf8b7f7d23fe5b76dbb07e63b"
+
+[[package]]
+name = "ipnet"
+version = "2.8.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "28b29a3cd74f0f4598934efe3aeba42bae0eb4680554128851ebbecb02af14e6"
+
+[[package]]
+name = "is-terminal"
+version = "0.4.9"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "cb0889898416213fab133e1d33a0e5858a48177452750691bde3666d0fdbaf8b"
+dependencies = [
+ "hermit-abi",
+ "rustix",
+ "windows-sys",
+]
+
+[[package]]
+name = "iso8601"
+version = "0.6.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "924e5d73ea28f59011fec52a0d12185d496a9b075d360657aed2a5707f701153"
+dependencies = [
+ "nom",
+]
 
 [[package]]
 name = "itoa"
 version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "af150ab688ff2122fcef229be89cb50dd66af9e01a4ff320cc137eecc9bacc38"
 
 [[package]]
+name = "js-sys"
+version = "0.3.64"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c5f195fe497f702db0f318b07fdd68edb16955aed830df8363d837542f8f935a"
+dependencies = [
+ "wasm-bindgen",
+]
+
+[[package]]
+name = "jsonschema"
+version = "0.17.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2a071f4f7efc9a9118dfb627a0a94ef247986e1ab8606a4c806ae2b3aa3b6978"
+dependencies = [
+ "ahash",
+ "anyhow",
+ "base64",
+ "bytecount",
+ "clap",
+ "fancy-regex",
+ "fraction",
+ "getrandom",
+ "iso8601",
+ "itoa",
+ "memchr",
+ "num-cmp",
+ "once_cell",
+ "parking_lot",
+ "percent-encoding",
+ "regex",
+ "reqwest",
+ "serde",
+ "serde_json",
+ "time",
+ "url",
+ "uuid",
+]
+
+[[package]]
+name = "lazy_static"
+version = "1.4.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
+
+[[package]]
 name = "libc"
 version = "0.2.147"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b4668fb0ea861c1df094127ac5f1da3409a82116a4ba74fca2e58ef927159bb3"
 
 [[package]]
 name = "libm"
 version = "0.2.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f7012b1bbb0719e1097c47611d3898568c546d597c2e74d66f6087edd5233ff4"
 
 [[package]]
+name = "linux-raw-sys"
+version = "0.4.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "09fc20d2ca12cb9f044c93e3bd6d32d523e6e2ec3db4f7b2939cd99026ecd3f0"
+
+[[package]]
 name = "lock_api"
 version = "0.4.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c1cc9717a20b1bb222f333e6a92fd32f7d8a18ddc5a3191a11af45dcbf4dcd16"
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
+name = "log"
+version = "0.4.19"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b06a4cde4c0f271a446782e3eff8de789548ce57dbc8eca9292c27f4a42004b4"
+
+[[package]]
 name = "matrixmultiply"
 version = "0.3.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "090126dc04f95dc0d1c1c91f61bdd474b3930ca064c1edc8a849da2c6cbe1e77"
 dependencies = [
  "autocfg",
  "rawpointer",
@@ -254,14 +714,46 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5a634b1c61a95585bd15607c6ab0c4e5b226e695ff2800ba0cdccddf208c406c"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
+name = "mime"
+version = "0.3.17"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6877bb514081ee2a7ff5ef9de3281f14a4dd4bceac4c09388074a6b5df8a139a"
+
+[[package]]
+name = "minimal-lexical"
+version = "0.2.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "68354c5c6bd36d73ff3feceb05efa59b6acb7626617f4962be322a825e61f79a"
+
+[[package]]
+name = "miniz_oxide"
+version = "0.7.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e7810e0be55b428ada41041c41f32c9f1a42817901b4ccf45fa3d4b6561e74c7"
+dependencies = [
+ "adler",
+]
+
+[[package]]
+name = "mio"
+version = "0.8.8"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "927a765cd3fc26206e66b296465fa9d3e5ab003e651c1b3c060e7956d96b19d2"
+dependencies = [
+ "libc",
+ "wasi",
+ "windows-sys",
+]
+
+[[package]]
 name = "nalgebra"
 version = "0.32.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "307ed9b18cc2423f29e83f84fd23a8e73628727990181f18641a8b5dc2ab1caa"
 dependencies = [
  "approx",
  "matrixmultiply",
@@ -295,14 +787,55 @@
  "num-integer",
  "num-traits",
  "rawpointer",
  "serde",
 ]
 
 [[package]]
+name = "nom"
+version = "7.1.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d273983c5a657a70a3e8f2a01329822f3b8c8172b73826411a55751e404a0a4a"
+dependencies = [
+ "memchr",
+ "minimal-lexical",
+]
+
+[[package]]
+name = "num"
+version = "0.4.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b05180d69e3da0e530ba2a1dae5110317e49e3b7f3d41be227dc5f92e49ee7af"
+dependencies = [
+ "num-bigint",
+ "num-complex",
+ "num-integer",
+ "num-iter",
+ "num-rational",
+ "num-traits",
+]
+
+[[package]]
+name = "num-bigint"
+version = "0.4.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f93ab6289c7b344a8a9f60f88d80aa20032336fe78da341afc91c8a2341fc75f"
+dependencies = [
+ "autocfg",
+ "num-integer",
+ "num-traits",
+]
+
+[[package]]
+name = "num-cmp"
+version = "0.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "63335b2e2c34fae2fb0aa2cecfd9f0832a1e24b3b32ecec612c3426d46dc8aaa"
+
+[[package]]
 name = "num-complex"
 version = "0.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "02e0d21255c828d6f128a1e41534206671e8c3ea0c62f32291e808dc82cff17d"
 dependencies = [
  "num-traits",
  "serde",
@@ -315,35 +848,57 @@
 checksum = "225d3389fb3509a24c93f5c29eb6bde2586b98d9f016636dff58d7c6f7569cd9"
 dependencies = [
  "autocfg",
  "num-traits",
 ]
 
 [[package]]
+name = "num-iter"
+version = "0.1.43"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7d03e6c028c5dc5cac6e2dec0efda81fc887605bb3d884578bb6d6bf7514e252"
+dependencies = [
+ "autocfg",
+ "num-integer",
+ "num-traits",
+]
+
+[[package]]
 name = "num-rational"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0638a1c9d0a3c0914158145bc76cff373a75a627e6ecbfb71cbe6f453a5a19b0"
 dependencies = [
  "autocfg",
+ "num-bigint",
  "num-integer",
  "num-traits",
 ]
 
 [[package]]
 name = "num-traits"
-version = "0.2.15"
+version = "0.2.16"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "578ede34cf02f8924ab9447f50c28075b4d3e5b269972345e7e0372b38c6cdcd"
+checksum = "f30b0abd723be7e2ffca1272140fac1a2f084c77ec3e123c192b66af1ee9e6c2"
 dependencies = [
  "autocfg",
  "libm",
 ]
 
 [[package]]
+name = "num_cpus"
+version = "1.16.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4161fcb6d602d4d2081af7c3a45852d875a03dd337a6bfdd6e06407b61342a43"
+dependencies = [
+ "hermit-abi",
+ "libc",
+]
+
+[[package]]
 name = "numpy"
 version = "0.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "437213adf41bbccf4aeae535fbfcdad0f6fed241e1ae182ebe97fa1f3ce19389"
 dependencies = [
  "libc",
  "ndarray",
@@ -351,14 +906,23 @@
  "num-integer",
  "num-traits",
  "pyo3",
  "rustc-hash",
 ]
 
 [[package]]
+name = "object"
+version = "0.31.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8bda667d9f2b5051b8833f59f3bf748b28ef54f850f4fcb389a252aa383866d1"
+dependencies = [
+ "memchr",
+]
+
+[[package]]
 name = "once_cell"
 version = "1.18.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dd8b5dd2ae5ed71462c540258bedcb51965123ad7e7ccf4b9a8cafaa4a63576d"
 
 [[package]]
 name = "parking_lot"
@@ -386,14 +950,20 @@
 [[package]]
 name = "paste"
 version = "1.0.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "de3145af08024dea9fa9914f381a17b8fc6034dfb00f3a84013f7ff43f29ed4c"
 
 [[package]]
+name = "percent-encoding"
+version = "2.3.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9b2a4787296e9989611394c33f193f676704af1686e70b8f8033ab5ba9a35a94"
+
+[[package]]
 name = "petgraph"
 version = "0.6.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4dd7d28ee937e54fe3080c91faa1c3a46c06de6252988a7f4592ba2310ef22a4"
 dependencies = [
  "fixedbitset",
  "indexmap",
@@ -511,52 +1081,54 @@
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "qoqo"
-version = "1.6.0-alpha.1"
+version = "1.6.0-alpha.2"
 dependencies = [
  "bincode",
  "nalgebra",
  "ndarray",
  "num-complex",
  "numpy",
  "proc-macro2",
  "pyo3",
  "pyo3-build-config",
  "qoqo-macros",
  "qoqo_calculator",
  "qoqo_calculator_pyo3",
  "quote",
  "roqoqo",
+ "schemars",
  "serde",
  "serde_json",
- "syn 2.0.26",
+ "syn 2.0.27",
  "test-case",
  "thiserror",
 ]
 
 [[package]]
 name = "qoqo-macros"
-version = "1.6.0-alpha.1"
+version = "1.6.0-alpha.2"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.26",
+ "syn 2.0.27",
 ]
 
 [[package]]
 name = "qoqo_calculator"
 version = "1.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1ecdd0eebe8a6d299cc47d3430b32fc874b2868e9508b0cc5939af5eedf926d"
 dependencies = [
  "num-complex",
+ "schemars",
  "serde",
  "thiserror",
 ]
 
 [[package]]
 name = "qoqo_calculator_pyo3"
 version = "1.1.2"
@@ -569,17 +1141,17 @@
  "qoqo_calculator",
  "serde",
  "thiserror",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.31"
+version = "1.0.32"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5fe8a65d69dd0808184ebb5f836ab526bb259db23c657efa38711b1072ee47f0"
+checksum = "50f3b39ccfb720540debaa0164757101c08ecb8d326b15358ce76a62c7e85965"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "rand"
 version = "0.8.5"
@@ -628,74 +1200,158 @@
 
 [[package]]
 name = "redox_syscall"
 version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "567664f262709473930a4bf9e51bf2ebf3348f2e748ccc50dea20646858f8f29"
 dependencies = [
- "bitflags",
+ "bitflags 1.3.2",
+]
+
+[[package]]
+name = "regex"
+version = "1.9.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b2eae68fc220f7cf2532e4494aded17545fce192d59cd996e0fe7887f4ceb575"
+dependencies = [
+ "aho-corasick",
+ "memchr",
+ "regex-automata",
+ "regex-syntax",
+]
+
+[[package]]
+name = "regex-automata"
+version = "0.3.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "39354c10dd07468c2e73926b23bb9c2caca74c5501e38a35da70406f1d923310"
+dependencies = [
+ "aho-corasick",
+ "memchr",
+ "regex-syntax",
+]
+
+[[package]]
+name = "regex-syntax"
+version = "0.7.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e5ea92a5b6195c6ef2a0295ea818b312502c6fc94dde986c5553242e18fd4ce2"
+
+[[package]]
+name = "reqwest"
+version = "0.11.18"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "cde824a14b7c14f85caff81225f411faacc04a2013f41670f41443742b1c1c55"
+dependencies = [
+ "base64",
+ "bytes",
+ "encoding_rs",
+ "futures-core",
+ "futures-util",
+ "h2",
+ "http",
+ "http-body",
+ "hyper",
+ "ipnet",
+ "js-sys",
+ "log",
+ "mime",
+ "once_cell",
+ "percent-encoding",
+ "pin-project-lite",
+ "serde",
+ "serde_json",
+ "serde_urlencoded",
+ "tokio",
+ "tower-service",
+ "url",
+ "wasm-bindgen",
+ "wasm-bindgen-futures",
+ "web-sys",
+ "winreg",
 ]
 
 [[package]]
 name = "roqoqo"
-version = "1.6.0-alpha.1"
+version = "1.6.0-alpha.2"
 dependencies = [
  "async-trait",
  "bincode",
  "dyn-clone",
  "futures",
+ "jsonschema",
  "nalgebra",
  "ndarray",
  "num-complex",
  "petgraph",
  "proc-macro2",
  "qoqo_calculator",
  "quote",
  "rand",
  "rand_distr",
  "roqoqo-derive",
+ "schemars",
  "serde",
  "serde_json",
  "serde_test",
- "syn 2.0.26",
+ "syn 2.0.27",
  "test-case",
  "thiserror",
  "typetag",
 ]
 
 [[package]]
 name = "roqoqo-derive"
-version = "1.6.0-alpha.1"
+version = "1.6.0-alpha.2"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.26",
+ "syn 2.0.27",
 ]
 
 [[package]]
 name = "roqoqo-test"
-version = "1.6.0-alpha.1"
+version = "1.6.0-alpha.2"
 dependencies = [
  "nalgebra",
  "ndarray",
  "proc-macro2",
  "qoqo_calculator",
  "quote",
  "rand",
  "roqoqo",
- "syn 2.0.26",
+ "syn 2.0.27",
 ]
 
 [[package]]
+name = "rustc-demangle"
+version = "0.1.23"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d626bb9dae77e28219937af045c257c28bfd3f69333c512553507f5f9798cb76"
+
+[[package]]
 name = "rustc-hash"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "08d43f7aa6b08d49f382cde6a7982047c3426db949b1424bc4b7ec9ae12c6ce2"
 
 [[package]]
+name = "rustix"
+version = "0.38.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0a962918ea88d644592894bc6dc55acc6c0956488adcebbfb6e273506b7fd6e5"
+dependencies = [
+ "bitflags 2.3.3",
+ "errno",
+ "libc",
+ "linux-raw-sys",
+ "windows-sys",
+]
+
+[[package]]
 name = "ryu"
 version = "1.0.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1ad4cc8da4ef723ed60bced201181d83791ad433213d8c24efffda1eec85d741"
 
 [[package]]
 name = "safe_arch"
@@ -703,37 +1359,72 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f398075ce1e6a179b46f51bd88d0598b92b00d3551f1a2d4ac49e771b56ac354"
 dependencies = [
  "bytemuck",
 ]
 
 [[package]]
+name = "schemars"
+version = "0.8.12"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "02c613288622e5f0c3fdc5dbd4db1c5fbe752746b1d1a56a0630b78fd00de44f"
+dependencies = [
+ "dyn-clone",
+ "schemars_derive",
+ "serde",
+ "serde_json",
+]
+
+[[package]]
+name = "schemars_derive"
+version = "0.8.12"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "109da1e6b197438deb6db99952990c7f959572794b80ff93707d55a232545e7c"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "serde_derive_internals",
+ "syn 1.0.109",
+]
+
+[[package]]
 name = "scopeguard"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "94143f37725109f92c262ed2cf5e59bce7498c01bcc1502d7b9afe439a4e9f49"
 
 [[package]]
 name = "serde"
-version = "1.0.171"
+version = "1.0.175"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "30e27d1e4fd7659406c492fd6cfaf2066ba8773de45ca75e855590f856dc34a9"
+checksum = "5d25439cd7397d044e2748a6fe2432b5e85db703d6d097bd014b3c0ad1ebff0b"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.171"
+version = "1.0.175"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b23f7ade6f110613c0d63858ddb8b94c1041f550eab58a16b371bdf2c9c80ab4"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn 2.0.27",
+]
+
+[[package]]
+name = "serde_derive_internals"
+version = "0.26.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "389894603bd18c46fa56231694f8d827779c0951a667087194cf9de94ed24682"
+checksum = "85bf8229e7920a9f636479437026331ce11aa132b4dde37d121944a44d6e5f3c"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.26",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "serde_json"
 version = "1.0.103"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d03b412469450d4404fe8499a268edd7f8b79fecb074b0d812ad64ca21f4031b"
@@ -741,22 +1432,34 @@
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
 name = "serde_test"
-version = "1.0.171"
+version = "1.0.175"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b6480a2f4e1449ec9757ea143362ad5cea79bc7f1cb7711c06e1c5d03b6b5a3a"
+checksum = "29baf0f77ca9ad9c6ed46e1b408b5e0f30b5184bcd66884e7f6d36bd7a65a8a4"
 dependencies = [
  "serde",
 ]
 
 [[package]]
+name = "serde_urlencoded"
+version = "0.7.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d3491c14715ca2294c4d6a88f15e84739788c1d030eed8c110436aafdaa2f3fd"
+dependencies = [
+ "form_urlencoded",
+ "itoa",
+ "ryu",
+ "serde",
+]
+
+[[package]]
 name = "simba"
 version = "0.8.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "061507c94fc6ab4ba1c9a0305018408e312e17c041eb63bef8aa726fa33aceae"
 dependencies = [
  "approx",
  "num-complex",
@@ -777,29 +1480,45 @@
 [[package]]
 name = "smallvec"
 version = "1.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "62bb4feee49fdd9f707ef802e22365a35de4b7b299de4763d44bfea899442ff9"
 
 [[package]]
+name = "socket2"
+version = "0.4.9"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "64a4a911eed85daf18834cfaa86a79b7d266ff93ff5ba14005426219480ed662"
+dependencies = [
+ "libc",
+ "winapi",
+]
+
+[[package]]
+name = "strsim"
+version = "0.10.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "73473c0e59e6d5812c5dfe2a064a6444949f089e20eec9a2e5506596494e4623"
+
+[[package]]
 name = "syn"
 version = "1.0.109"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "72b64191b275b66ffe2469e8af2c1cfe3bafa67b529ead792a6d0160888b4237"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.26"
+version = "2.0.27"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "45c3457aacde3c65315de5031ec191ce46604304d2446e803d71ade03308d970"
+checksum = "b60f673f44a8255b9c8c657daf66a596d435f2da81a555b06dc644d080ba45e0"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
@@ -841,97 +1560,355 @@
  "quote",
  "syn 1.0.109",
  "test-case-core",
 ]
 
 [[package]]
 name = "thiserror"
-version = "1.0.43"
+version = "1.0.44"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a35fc5b8971143ca348fa6df4f024d4d55264f3468c71ad1c2f365b0a4d58c42"
+checksum = "611040a08a0439f8248d1990b111c95baa9c704c805fa1f62104b39655fd7f90"
 dependencies = [
  "thiserror-impl",
 ]
 
 [[package]]
 name = "thiserror-impl"
-version = "1.0.43"
+version = "1.0.44"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "463fe12d7993d3b327787537ce8dd4dfa058de32fc2b195ef3cde03dc4771e8f"
+checksum = "090198534930841fab3a5d1bb637cde49e339654e606195f8d9c76eeb081dc96"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.26",
+ "syn 2.0.27",
+]
+
+[[package]]
+name = "time"
+version = "0.3.23"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "59e399c068f43a5d116fedaf73b203fa4f9c519f17e2b34f63221d3792f81446"
+dependencies = [
+ "serde",
+ "time-core",
+ "time-macros",
+]
+
+[[package]]
+name = "time-core"
+version = "0.1.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7300fbefb4dadc1af235a9cef3737cea692a9d97e1b9cbcd4ebdae6f8868e6fb"
+
+[[package]]
+name = "time-macros"
+version = "0.2.10"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "96ba15a897f3c86766b757e5ac7221554c6750054d74d5b28844fce5fb36a6c4"
+dependencies = [
+ "time-core",
 ]
 
 [[package]]
+name = "tinyvec"
+version = "1.6.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "87cc5ceb3875bb20c2890005a4e226a4651264a5c75edb2421b52861a0a0cb50"
+dependencies = [
+ "tinyvec_macros",
+]
+
+[[package]]
+name = "tinyvec_macros"
+version = "0.1.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1f3ccbac311fea05f86f61904b462b55fb3df8837a366dfc601a0161d0532f20"
+
+[[package]]
+name = "tokio"
+version = "1.29.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "532826ff75199d5833b9d2c5fe410f29235e25704ee5f0ef599fb51c21f4a4da"
+dependencies = [
+ "autocfg",
+ "backtrace",
+ "bytes",
+ "libc",
+ "mio",
+ "num_cpus",
+ "pin-project-lite",
+ "socket2",
+ "windows-sys",
+]
+
+[[package]]
+name = "tokio-util"
+version = "0.7.8"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "806fe8c2c87eccc8b3267cbae29ed3ab2d0bd37fca70ab622e46aaa9375ddb7d"
+dependencies = [
+ "bytes",
+ "futures-core",
+ "futures-sink",
+ "pin-project-lite",
+ "tokio",
+ "tracing",
+]
+
+[[package]]
+name = "tower-service"
+version = "0.3.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b6bc1c9ce2b5135ac7f93c72918fc37feb872bdc6a5533a8b85eb4b86bfdae52"
+
+[[package]]
+name = "tracing"
+version = "0.1.37"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8ce8c33a8d48bd45d624a6e523445fd21ec13d3653cd51f681abf67418f54eb8"
+dependencies = [
+ "cfg-if",
+ "pin-project-lite",
+ "tracing-core",
+]
+
+[[package]]
+name = "tracing-core"
+version = "0.1.31"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0955b8137a1df6f1a2e9a37d8a6656291ff0297c1a97c24e0d8425fe2312f79a"
+dependencies = [
+ "once_cell",
+]
+
+[[package]]
+name = "try-lock"
+version = "0.2.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3528ecfd12c466c6f163363caf2d02a71161dd5e1cc6ae7b34207ea2d42d81ed"
+
+[[package]]
 name = "typenum"
 version = "1.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "497961ef93d974e23eb6f433eb5fe1b7930b659f06d12dec6fc44a8f554c0bba"
 
 [[package]]
 name = "typetag"
-version = "0.2.10"
+version = "0.2.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7a66aafcfb982bf1f9a28755ac6bcbdcd4631ff516cb038fa61299201ebb4364"
+checksum = "aec6850cc671cd0cfb3ab285465e48a3b927d9de155051c35797446b32f9169f"
 dependencies = [
  "erased-serde",
  "inventory",
  "once_cell",
  "serde",
  "typetag-impl",
 ]
 
 [[package]]
 name = "typetag-impl"
-version = "0.2.10"
+version = "0.2.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d836cd032f71d90cbaa3c1f85ce84266af23659766d8c0b1c4c6524a0fb4c36f"
+checksum = "30c49a6815b4f8379c36f06618bc1b80ca77aaf8a3fd4d8549dca6fdb016000f"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.26",
+ "syn 2.0.27",
 ]
 
 [[package]]
+name = "unicode-bidi"
+version = "0.3.13"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "92888ba5573ff080736b3648696b70cafad7d250551175acbaa4e0385b3e1460"
+
+[[package]]
 name = "unicode-ident"
 version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "301abaae475aa91687eb82514b328ab47a211a533026cb25fc3e519b86adfc3c"
 
 [[package]]
+name = "unicode-normalization"
+version = "0.1.22"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5c5713f0fc4b5db668a2ac63cdb7bb4469d8c9fed047b1d0292cc7b0ce2ba921"
+dependencies = [
+ "tinyvec",
+]
+
+[[package]]
 name = "unindent"
 version = "0.1.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1766d682d402817b5ac4490b3c3002d91dfa0d22812f341609f97b08757359c"
 
 [[package]]
+name = "url"
+version = "2.4.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "50bff7831e19200a85b17131d085c25d7811bc4e186efdaf54bbd132994a88cb"
+dependencies = [
+ "form_urlencoded",
+ "idna",
+ "percent-encoding",
+]
+
+[[package]]
+name = "utf8parse"
+version = "0.2.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "711b9620af191e0cdc7468a8d14e709c3dcdb115b36f838e601583af800a370a"
+
+[[package]]
+name = "uuid"
+version = "1.4.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "79daa5ed5740825c40b389c5e50312b9c86df53fccd33f281df655642b43869d"
+
+[[package]]
 name = "version_check"
 version = "0.9.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "49874b5167b65d7193b8aba1567f5c7d93d001cafc34600cee003eda787e483f"
 
 [[package]]
+name = "want"
+version = "0.3.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "bfa7760aed19e106de2c7c0b581b509f2f25d3dacaf737cb82ac61bc6d760b0e"
+dependencies = [
+ "try-lock",
+]
+
+[[package]]
 name = "wasi"
 version = "0.11.0+wasi-snapshot-preview1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c8d87e72b64a3b4db28d11ce29237c246188f4f51057d65a7eab63b7987e423"
 
 [[package]]
+name = "wasm-bindgen"
+version = "0.2.87"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7706a72ab36d8cb1f80ffbf0e071533974a60d0a308d01a5d0375bf60499a342"
+dependencies = [
+ "cfg-if",
+ "wasm-bindgen-macro",
+]
+
+[[package]]
+name = "wasm-bindgen-backend"
+version = "0.2.87"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5ef2b6d3c510e9625e5fe6f509ab07d66a760f0885d858736483c32ed7809abd"
+dependencies = [
+ "bumpalo",
+ "log",
+ "once_cell",
+ "proc-macro2",
+ "quote",
+ "syn 2.0.27",
+ "wasm-bindgen-shared",
+]
+
+[[package]]
+name = "wasm-bindgen-futures"
+version = "0.4.37"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c02dbc21516f9f1f04f187958890d7e6026df8d16540b7ad9492bc34a67cea03"
+dependencies = [
+ "cfg-if",
+ "js-sys",
+ "wasm-bindgen",
+ "web-sys",
+]
+
+[[package]]
+name = "wasm-bindgen-macro"
+version = "0.2.87"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "dee495e55982a3bd48105a7b947fd2a9b4a8ae3010041b9e0faab3f9cd028f1d"
+dependencies = [
+ "quote",
+ "wasm-bindgen-macro-support",
+]
+
+[[package]]
+name = "wasm-bindgen-macro-support"
+version = "0.2.87"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "54681b18a46765f095758388f2d0cf16eb8d4169b639ab575a8f5693af210c7b"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn 2.0.27",
+ "wasm-bindgen-backend",
+ "wasm-bindgen-shared",
+]
+
+[[package]]
+name = "wasm-bindgen-shared"
+version = "0.2.87"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ca6ad05a4870b2bf5fe995117d3728437bd27d7cd5f06f13c17443ef369775a1"
+
+[[package]]
+name = "web-sys"
+version = "0.3.64"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9b85cbef8c220a6abc02aefd892dfc0fc23afb1c6a426316ec33253a3877249b"
+dependencies = [
+ "js-sys",
+ "wasm-bindgen",
+]
+
+[[package]]
 name = "wide"
 version = "0.7.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "aa469ffa65ef7e0ba0f164183697b89b854253fd31aeb92358b7b6155177d62f"
 dependencies = [
  "bytemuck",
  "safe_arch",
 ]
 
 [[package]]
+name = "winapi"
+version = "0.3.9"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5c839a674fcd7a98952e593242ea400abe93992746761e38641405d28b00f419"
+dependencies = [
+ "winapi-i686-pc-windows-gnu",
+ "winapi-x86_64-pc-windows-gnu",
+]
+
+[[package]]
+name = "winapi-i686-pc-windows-gnu"
+version = "0.4.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ac3b87c63620426dd9b991e5ce0329eff545bccbbb34f3be09ff6fb6ab51b7b6"
+
+[[package]]
+name = "winapi-x86_64-pc-windows-gnu"
+version = "0.4.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "712e227841d057c1ee1cd2fb22fa7e5a5461ae8e48fa2ca79ec42cfc1931183f"
+
+[[package]]
+name = "windows-sys"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "677d2418bec65e3338edb076e806bc1ec15693c5d0104683f2efe857f61056a9"
+dependencies = [
+ "windows-targets",
+]
+
+[[package]]
 name = "windows-targets"
 version = "0.48.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "05d4b17490f70499f20b9e791dcf6a299785ce8af4d709018206dc5b4953e95f"
 dependencies = [
  "windows_aarch64_gnullvm",
  "windows_aarch64_msvc",
@@ -979,7 +1956,16 @@
 checksum = "7896dbc1f41e08872e9d5e8f8baa8fdd2677f29468c4e156210174edc7f7b953"
 
 [[package]]
 name = "windows_x86_64_msvc"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1a515f5799fe4961cb532f983ce2b23082366b898e52ffbce459c86f67c8378a"
+
+[[package]]
+name = "winreg"
+version = "0.10.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "80d0f4e272c85def139476380b12f9ac60926689dd2e01d4923222f40580869d"
+dependencies = [
+ "winapi",
+]
```

### Comparing `qoqo-1.6.0a1/PKG-INFO` & `qoqo-1.6.0a2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qoqo
-Version: 1.6.0a1
+Version: 1.6.0a2
 Requires-Dist: numpy
 Requires-Dist: qoqo_calculator_pyo3 >=1.1
 Requires-Dist: sphinx >=2.1 ; extra == 'docs'
 Requires-Dist: nbsphinx ; extra == 'docs'
 Requires-Dist: pygments ; extra == 'docs'
 Requires-Dist: recommonmark ; extra == 'docs'
 Requires-Dist: myst_parser ; extra == 'docs'
```

