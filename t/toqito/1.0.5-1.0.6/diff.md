# Comparing `tmp/toqito-1.0.5.tar.gz` & `tmp/toqito-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toqito-1.0.5.tar", last modified: Tue Mar 14 01:20:12 2023, max compression
+gzip compressed data, was "toqito-1.0.6.tar", last modified: Sat Jul  8 08:38:24 2023, max compression
```

## Comparing `toqito-1.0.5.tar` & `toqito-1.0.6.tar`

### file list

```diff
@@ -1,357 +1,375 @@
-drwxr-xr-x   0 vincent.russo   (502) staff       (20)        0 2023-03-14 01:20:12.669375 toqito-1.0.5/
--rw-r--r--   0 vincent.russo   (502) staff       (20)     1070 2022-05-09 18:55:39.000000 toqito-1.0.5/LICENSE
--rw-r--r--   0 vincent.russo   (502) staff       (20)     3818 2023-03-14 01:20:12.669512 toqito-1.0.5/PKG-INFO
--rw-r--r--   0 vincent.russo   (502) staff       (20)     3215 2022-05-09 18:55:39.000000 toqito-1.0.5/README.md
--rw-r--r--   0 vincent.russo   (502) staff       (20)     1305 2023-03-14 01:18:53.000000 toqito-1.0.5/pyproject.toml
--rw-r--r--   0 vincent.russo   (502) staff       (20)      108 2023-03-14 01:20:12.670013 toqito-1.0.5/setup.cfg
--rw-r--r--   0 vincent.russo   (502) staff       (20)      951 2023-03-14 01:19:00.000000 toqito-1.0.5/setup.py
-drwxr-xr-x   0 vincent.russo   (502) staff       (20)        0 2023-03-14 01:20:12.516893 toqito-1.0.5/tests/
--rw-r--r--   0 vincent.russo   (502) staff       (20)       37 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/__init__.py
-drwxr-xr-x   0 vincent.russo   (502) staff       (20)        0 2023-03-14 01:20:12.518551 toqito-1.0.5/tests/test_channel_metrics/
--rw-r--r--   0 vincent.russo   (502) staff       (20)       33 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_channel_metrics/__init__.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     1295 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_channel_metrics/test_channel_fidelity.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     1227 2022-05-10 23:57:37.000000 toqito-1.0.5/tests/test_channel_metrics/test_diamond_norm.py
-drwxr-xr-x   0 vincent.russo   (502) staff       (20)        0 2023-03-14 01:20:12.521284 toqito-1.0.5/tests/test_channel_ops/
--rw-r--r--   0 vincent.russo   (502) staff       (20)       29 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_channel_ops/__init__.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     1690 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_channel_ops/test_apply_channel.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     1025 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_channel_ops/test_choi_to_kraus.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     3059 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_channel_ops/test_dual_channel.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     3481 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_channel_ops/test_kraus_to_choi.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     4619 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_channel_ops/test_partial_channel.py
-drwxr-xr-x   0 vincent.russo   (502) staff       (20)        0 2023-03-14 01:20:12.524951 toqito-1.0.5/tests/test_channel_props/
--rw-r--r--   0 vincent.russo   (502) staff       (20)       31 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_channel_props/__init__.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     1351 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_channel_props/test_choi_rank.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)      750 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_channel_props/test_is_completely_positive.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     1290 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_channel_props/test_is_herm_preserving.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)      683 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_channel_props/test_is_positive.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)      732 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_channel_props/test_is_quantum_channel.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)      726 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_channel_props/test_is_trace_preserving.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     1234 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_channel_props/test_is_unital.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)      618 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_channel_props/test_is_unitary.py
-drwxr-xr-x   0 vincent.russo   (502) staff       (20)        0 2023-03-14 01:20:12.529487 toqito-1.0.5/tests/test_channels/
--rw-r--r--   0 vincent.russo   (502) staff       (20)       26 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_channels/__init__.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     1478 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_channels/test_choi.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     1093 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_channels/test_dephasing.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     1288 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_channels/test_depolarizing.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)    35181 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_channels/test_partial_trace.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)    33377 2023-01-09 11:17:36.000000 toqito-1.0.5/tests/test_channels/test_partial_transpose.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)    11294 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_channels/test_realignment.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     1418 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_channels/test_reduction.py
-drwxr-xr-x   0 vincent.russo   (502) staff       (20)        0 2023-03-14 01:20:12.531837 toqito-1.0.5/tests/test_helper/
--rw-r--r--   0 vincent.russo   (502) staff       (20)       24 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_helper/__init__.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)      385 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_helper/test_cvx_kron.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)      836 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_helper/test_expr_as_np_array.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)      445 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_helper/test_np_array_as_expr.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     2644 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_helper/test_npa_constraints.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     2086 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_helper/test_update_odometer.py
-drwxr-xr-x   0 vincent.russo   (502) staff       (20)        0 2023-03-14 01:20:12.536369 toqito-1.0.5/tests/test_matrices/
--rw-r--r--   0 vincent.russo   (502) staff       (20)       21 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_matrices/__init__.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)      387 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_matrices/test_cnot.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)      427 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_matrices/test_fourier.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     2847 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_matrices/test_gell_mann.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     2637 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_matrices/test_gen_gell_mann.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     1171 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_matrices/test_gen_pauli.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     1791 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_matrices/test_hadamard.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)      624 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_matrices/test_iden.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     2666 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_matrices/test_pauli.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)      709 2023-01-09 11:17:36.000000 toqito-1.0.5/tests/test_matrices/test_standard_basis.py
-drwxr-xr-x   0 vincent.russo   (502) staff       (20)        0 2023-03-14 01:20:12.539441 toqito-1.0.5/tests/test_matrix_ops/
--rw-r--r--   0 vincent.russo   (502) staff       (20)       30 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_matrix_ops/__init__.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     1330 2023-03-01 20:54:25.000000 toqito-1.0.5/tests/test_matrix_ops/test_inner_product.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     1164 2023-03-01 20:54:25.000000 toqito-1.0.5/tests/test_matrix_ops/test_outer_product.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     4247 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_matrix_ops/test_tensor.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)      772 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_matrix_ops/test_unvec.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)      430 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_matrix_ops/test_vec.py
-drwxr-xr-x   0 vincent.russo   (502) staff       (20)        0 2023-03-14 01:20:12.547529 toqito-1.0.5/tests/test_matrix_props/
--rw-r--r--   0 vincent.russo   (502) staff       (20)       30 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_matrix_props/__init__.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     1545 2023-01-09 11:17:36.000000 toqito-1.0.5/tests/test_matrix_props/test_is_block_positive.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)      637 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_matrix_props/test_is_commuting.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)      604 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_matrix_props/test_is_density.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)      666 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_matrix_props/test_is_diagonal.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)      692 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_matrix_props/test_is_hermitian.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     1236 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_matrix_props/test_is_idempotent.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)      645 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_matrix_props/test_is_identity.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)      963 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_matrix_props/test_is_normal.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)      777 2023-01-09 11:17:36.000000 toqito-1.0.5/tests/test_matrix_props/test_is_orthonormal.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     1939 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_matrix_props/test_is_permutation.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     1452 2023-01-09 11:17:36.000000 toqito-1.0.5/tests/test_matrix_props/test_is_positive_definite.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)      601 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_matrix_props/test_is_positive_semidefinite.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)      889 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_matrix_props/test_is_projection.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)      648 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_matrix_props/test_is_square.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)      695 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_matrix_props/test_is_symmetric.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     1063 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_matrix_props/test_is_unitary.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)      881 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_matrix_props/test_majorizes.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     2539 2023-01-09 11:17:36.000000 toqito-1.0.5/tests/test_matrix_props/test_sk_norm.py
-drwxr-xr-x   0 vincent.russo   (502) staff       (20)        0 2023-03-14 01:20:12.548310 toqito-1.0.5/tests/test_measurement_ops/
--rw-r--r--   0 vincent.russo   (502) staff       (20)       33 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_measurement_ops/__init__.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)      585 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_measurement_ops/test_measure.py
-drwxr-xr-x   0 vincent.russo   (502) staff       (20)        0 2023-03-14 01:20:12.549192 toqito-1.0.5/tests/test_measurement_props/
--rw-r--r--   0 vincent.russo   (502) staff       (20)       35 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_measurement_props/__init__.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     1009 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_measurement_props/test_is_povm.py
-drwxr-xr-x   0 vincent.russo   (502) staff       (20)        0 2023-03-14 01:20:12.551288 toqito-1.0.5/tests/test_nonlocal_games/
--rw-r--r--   0 vincent.russo   (502) staff       (20)       47 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_nonlocal_games/__init__.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     7615 2023-01-09 11:17:36.000000 toqito-1.0.5/tests/test_nonlocal_games/test_extended_nonlocal_game.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     9362 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_nonlocal_games/test_nonlocal_game.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     4076 2022-06-15 14:44:03.000000 toqito-1.0.5/tests/test_nonlocal_games/test_quantum_hedging.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     5954 2023-03-11 11:52:07.000000 toqito-1.0.5/tests/test_nonlocal_games/test_xor_game.py
-drwxr-xr-x   0 vincent.russo   (502) staff       (20)        0 2023-03-14 01:20:12.556007 toqito-1.0.5/tests/test_perms/
--rw-r--r--   0 vincent.russo   (502) staff       (20)       23 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_perms/__init__.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     1312 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_perms/test_antisymmetric_projection.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     1768 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_perms/test_perfect_matchings.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)      468 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_perms/test_perm_sign.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     3164 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_perms/test_permutation_operator.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     8070 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_perms/test_permute_systems.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)    16464 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_perms/test_swap.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)      764 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_perms/test_swap_operator.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     4830 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_perms/test_symmetric_projection.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)      327 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_perms/test_unique_perms.py
-drwxr-xr-x   0 vincent.russo   (502) staff       (20)        0 2023-03-14 01:20:12.558587 toqito-1.0.5/tests/test_random/
--rw-r--r--   0 vincent.russo   (502) staff       (20)       24 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_random/__init__.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     1213 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_random/test_random_density_matrix.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)      388 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_random/test_random_ginibre.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     1138 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_random/test_random_povm.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     1560 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_random/test_random_state_vector.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)      706 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_random/test_random_unitary.py
-drwxr-xr-x   0 vincent.russo   (502) staff       (20)        0 2023-03-14 01:20:12.563101 toqito-1.0.5/tests/test_state_metrics/
--rw-r--r--   0 vincent.russo   (502) staff       (20)       41 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_state_metrics/__init__.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     2216 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_state_metrics/test_bures_distance.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     2065 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_state_metrics/test_fidelity.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)      870 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_state_metrics/test_helstrom_holevo.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)      736 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_state_metrics/test_hilbert_schmidt.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     1863 2023-01-09 11:17:36.000000 toqito-1.0.5/tests/test_state_metrics/test_hilbert_schmidt_inner_product.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     1937 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_state_metrics/test_matsumoto_fidelity.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     1900 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_state_metrics/test_sub_fidelity.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)      851 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_state_metrics/test_trace_distance.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)      600 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_state_metrics/test_trace_norm.py
-drwxr-xr-x   0 vincent.russo   (502) staff       (20)        0 2023-03-14 01:20:12.564323 toqito-1.0.5/tests/test_state_ops/
--rw-r--r--   0 vincent.russo   (502) staff       (20)       44 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_state_ops/__init__.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     1178 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_state_ops/test_pure_to_mixed.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)    10445 2022-05-09 21:26:26.000000 toqito-1.0.5/tests/test_state_ops/test_schmidt_decomposition.py
-drwxr-xr-x   0 vincent.russo   (502) staff       (20)        0 2023-03-14 01:20:12.567657 toqito-1.0.5/tests/test_state_opt/
--rw-r--r--   0 vincent.russo   (502) staff       (20)       47 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_state_opt/__init__.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     1682 2023-01-09 11:17:36.000000 toqito-1.0.5/tests/test_state_opt/test_optimal_clone.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     9162 2022-06-15 14:44:03.000000 toqito-1.0.5/tests/test_state_opt/test_ppt_distinguishability.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     2964 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_state_opt/test_state_distinguishability.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     5679 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_state_opt/test_state_exclusion.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     5483 2023-01-09 11:17:36.000000 toqito-1.0.5/tests/test_state_opt/test_symmetric_extension_hierarchy.py
-drwxr-xr-x   0 vincent.russo   (502) staff       (20)        0 2023-03-14 01:20:12.576432 toqito-1.0.5/tests/test_state_props/
--rw-r--r--   0 vincent.russo   (502) staff       (20)       44 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_state_props/__init__.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)      996 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_state_props/test_concurrence.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     1611 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_state_props/test_entanglement_of_formation.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     2250 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_state_props/test_has_symmetric_extension.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     1306 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_state_props/test_in_separable_ball.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)      651 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_state_props/test_is_ensemble.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)      401 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_state_props/test_is_mixed.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)      854 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_state_props/test_is_mutually_orthogonal.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     1201 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_state_props/test_is_mutually_unbiased_basis.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     1226 2022-05-13 00:48:31.000000 toqito-1.0.5/tests/test_state_props/test_is_npt.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     1222 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_state_props/test_is_ppt.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     2047 2022-05-09 20:41:17.000000 toqito-1.0.5/tests/test_state_props/test_is_product.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     1128 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_state_props/test_is_pure.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     3473 2023-01-09 11:17:36.000000 toqito-1.0.5/tests/test_state_props/test_is_separable.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)      410 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_state_props/test_l1_norm_coherence.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     1324 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_state_props/test_log_negativity.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     1284 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_state_props/test_negativity.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)      716 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_state_props/test_purity.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     2970 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_state_props/test_schmidt_rank.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)      511 2023-01-09 11:17:36.000000 toqito-1.0.5/tests/test_state_props/test_sk_vec_norm.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)      933 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_state_props/test_von_neumann_entropy.py
-drwxr-xr-x   0 vincent.russo   (502) staff       (20)        0 2023-03-14 01:20:12.583609 toqito-1.0.5/tests/test_states/
--rw-r--r--   0 vincent.russo   (502) staff       (20)       24 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_states/__init__.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)      930 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_states/test_basis.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     1588 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_states/test_bell.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)      760 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_states/test_brauer.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)      612 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_states/test_breuer.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)      761 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_states/test_chessboard.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     2821 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_states/test_domino.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     1415 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_states/test_gen_bell.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     1847 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_states/test_ghz.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)      656 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_states/test_gisin.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     2659 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_states/test_horodecki.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)      459 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_states/test_isotropic.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)      852 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_states/test_max_entangled.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)      730 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_states/test_max_mixed.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)      427 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_states/test_singlet.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     2455 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_states/test_tile.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     1461 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_states/test_w_state.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)      729 2022-05-09 18:55:39.000000 toqito-1.0.5/tests/test_states/test_werner.py
-drwxr-xr-x   0 vincent.russo   (502) staff       (20)        0 2023-03-14 01:20:12.583978 toqito-1.0.5/toqito/
--rw-r--r--   0 vincent.russo   (502) staff       (20)       59 2022-05-09 18:55:39.000000 toqito-1.0.5/toqito/__init__.py
-drwxr-xr-x   0 vincent.russo   (502) staff       (20)        0 2023-03-14 01:20:12.587589 toqito-1.0.5/toqito/channel_metrics/
--rw-r--r--   0 vincent.russo   (502) staff       (20)      175 2022-05-10 23:57:37.000000 toqito-1.0.5/toqito/channel_metrics/__init__.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     3648 2023-01-09 11:17:36.000000 toqito-1.0.5/toqito/channel_metrics/channel_fidelity.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     2224 2023-01-09 11:17:36.000000 toqito-1.0.5/toqito/channel_metrics/diamond_norm.py
-drwxr-xr-x   0 vincent.russo   (502) staff       (20)        0 2023-03-14 01:20:12.590294 toqito-1.0.5/toqito/channel_ops/
--rw-r--r--   0 vincent.russo   (502) staff       (20)      347 2022-05-09 18:55:39.000000 toqito-1.0.5/toqito/channel_ops/__init__.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     4875 2023-01-09 11:17:36.000000 toqito-1.0.5/toqito/channel_ops/apply_channel.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     2622 2022-05-09 18:55:39.000000 toqito-1.0.5/toqito/channel_ops/choi_to_kraus.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     3046 2023-01-09 11:17:36.000000 toqito-1.0.5/toqito/channel_ops/dual_channel.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     2345 2022-05-09 18:55:39.000000 toqito-1.0.5/toqito/channel_ops/kraus_to_choi.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     6431 2023-01-09 11:17:36.000000 toqito-1.0.5/toqito/channel_ops/partial_channel.py
-drwxr-xr-x   0 vincent.russo   (502) staff       (20)        0 2023-03-14 01:20:12.594380 toqito-1.0.5/toqito/channel_props/
--rw-r--r--   0 vincent.russo   (502) staff       (20)      562 2022-05-09 18:55:39.000000 toqito-1.0.5/toqito/channel_props/__init__.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     2792 2023-01-09 11:17:36.000000 toqito-1.0.5/toqito/channel_props/choi_rank.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     3050 2023-01-09 11:17:36.000000 toqito-1.0.5/toqito/channel_props/is_completely_positive.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     2598 2023-01-09 11:17:36.000000 toqito-1.0.5/toqito/channel_props/is_herm_preserving.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     2540 2023-01-09 11:17:36.000000 toqito-1.0.5/toqito/channel_props/is_positive.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     1988 2023-01-09 11:17:36.000000 toqito-1.0.5/toqito/channel_props/is_quantum_channel.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     3416 2023-01-09 11:17:36.000000 toqito-1.0.5/toqito/channel_props/is_trace_preserving.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     2084 2023-01-09 11:17:36.000000 toqito-1.0.5/toqito/channel_props/is_unital.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     2183 2023-01-09 11:17:36.000000 toqito-1.0.5/toqito/channel_props/is_unitary.py
-drwxr-xr-x   0 vincent.russo   (502) staff       (20)        0 2023-03-14 01:20:12.598264 toqito-1.0.5/toqito/channels/
--rw-r--r--   0 vincent.russo   (502) staff       (20)      412 2022-05-09 18:55:39.000000 toqito-1.0.5/toqito/channels/__init__.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     4015 2022-05-09 18:55:39.000000 toqito-1.0.5/toqito/channels/choi.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     2916 2022-05-09 18:55:39.000000 toqito-1.0.5/toqito/channels/dephasing.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     3370 2022-06-15 14:44:03.000000 toqito-1.0.5/toqito/channels/depolarizing.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     7313 2023-01-09 11:17:36.000000 toqito-1.0.5/toqito/channels/partial_trace.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     7108 2023-01-09 11:17:36.000000 toqito-1.0.5/toqito/channels/partial_transpose.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     3096 2023-01-09 11:17:36.000000 toqito-1.0.5/toqito/channels/realignment.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     1678 2022-06-15 14:44:03.000000 toqito-1.0.5/toqito/channels/reduction.py
-drwxr-xr-x   0 vincent.russo   (502) staff       (20)        0 2023-03-14 01:20:12.601153 toqito-1.0.5/toqito/helper/
--rw-r--r--   0 vincent.russo   (502) staff       (20)      375 2023-01-09 11:17:36.000000 toqito-1.0.5/toqito/helper/__init__.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     1096 2023-01-09 11:17:36.000000 toqito-1.0.5/toqito/helper/cvx_kron.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)      701 2022-05-09 18:55:39.000000 toqito-1.0.5/toqito/helper/expr_as_np_array.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)      748 2023-01-09 11:17:36.000000 toqito-1.0.5/toqito/helper/kp_norm.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)      447 2022-05-09 18:55:39.000000 toqito-1.0.5/toqito/helper/np_array_as_expr.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)    10195 2023-01-09 11:17:36.000000 toqito-1.0.5/toqito/helper/npa_hierarchy.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     2556 2023-01-09 11:17:36.000000 toqito-1.0.5/toqito/helper/update_odometer.py
-drwxr-xr-x   0 vincent.russo   (502) staff       (20)        0 2023-03-14 01:20:12.606223 toqito-1.0.5/toqito/matrices/
--rw-r--r--   0 vincent.russo   (502) staff       (20)      512 2023-01-09 11:17:36.000000 toqito-1.0.5/toqito/matrices/__init__.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     1733 2022-05-09 18:55:39.000000 toqito-1.0.5/toqito/matrices/clock.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)      748 2022-05-09 18:55:39.000000 toqito-1.0.5/toqito/matrices/cnot.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     1816 2022-05-09 18:55:39.000000 toqito-1.0.5/toqito/matrices/fourier.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     4486 2023-01-09 11:17:36.000000 toqito-1.0.5/toqito/matrices/gell_mann.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     3064 2023-01-09 11:17:36.000000 toqito-1.0.5/toqito/matrices/gen_gell_mann.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     2688 2022-05-09 18:55:39.000000 toqito-1.0.5/toqito/matrices/gen_pauli.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     1793 2022-06-15 14:44:03.000000 toqito-1.0.5/toqito/matrices/hadamard.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     2119 2022-05-09 18:55:39.000000 toqito-1.0.5/toqito/matrices/iden.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     3004 2023-01-09 11:17:36.000000 toqito-1.0.5/toqito/matrices/pauli.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     1665 2022-05-09 18:55:39.000000 toqito-1.0.5/toqito/matrices/shift.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)      961 2023-01-09 11:17:36.000000 toqito-1.0.5/toqito/matrices/standard_basis.py
-drwxr-xr-x   0 vincent.russo   (502) staff       (20)        0 2023-03-14 01:20:12.608781 toqito-1.0.5/toqito/matrix_ops/
--rw-r--r--   0 vincent.russo   (502) staff       (20)      281 2023-03-01 20:54:25.000000 toqito-1.0.5/toqito/matrix_ops/__init__.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     1791 2023-03-01 20:54:25.000000 toqito-1.0.5/toqito/matrix_ops/inner_product.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     2066 2023-03-01 20:54:25.000000 toqito-1.0.5/toqito/matrix_ops/outer_product.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     5043 2023-03-01 20:54:25.000000 toqito-1.0.5/toqito/matrix_ops/tensor.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     2336 2023-01-09 11:17:36.000000 toqito-1.0.5/toqito/matrix_ops/unvec.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     2158 2022-05-09 18:55:39.000000 toqito-1.0.5/toqito/matrix_ops/vec.py
-drwxr-xr-x   0 vincent.russo   (502) staff       (20)        0 2023-03-14 01:20:12.617704 toqito-1.0.5/toqito/matrix_props/
--rw-r--r--   0 vincent.russo   (502) staff       (20)     1116 2023-01-09 11:17:36.000000 toqito-1.0.5/toqito/matrix_props/__init__.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     4184 2023-01-09 11:17:36.000000 toqito-1.0.5/toqito/matrix_props/is_block_positive.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     2341 2022-05-09 18:55:39.000000 toqito-1.0.5/toqito/matrix_props/is_commuting.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     2218 2022-05-09 18:55:39.000000 toqito-1.0.5/toqito/matrix_props/is_density.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     1994 2022-05-09 18:55:39.000000 toqito-1.0.5/toqito/matrix_props/is_diagonal.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     1780 2022-05-09 18:55:39.000000 toqito-1.0.5/toqito/matrix_props/is_hermitian.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     1716 2022-05-09 18:55:39.000000 toqito-1.0.5/toqito/matrix_props/is_idempotent.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     2042 2022-05-09 18:55:39.000000 toqito-1.0.5/toqito/matrix_props/is_identity.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     1896 2022-05-09 18:55:39.000000 toqito-1.0.5/toqito/matrix_props/is_normal.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)      464 2023-01-09 11:17:36.000000 toqito-1.0.5/toqito/matrix_props/is_orthonormal.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     1776 2022-05-09 18:55:39.000000 toqito-1.0.5/toqito/matrix_props/is_permutation.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     2014 2023-03-11 11:51:59.000000 toqito-1.0.5/toqito/matrix_props/is_positive_definite.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     1679 2022-05-09 18:55:39.000000 toqito-1.0.5/toqito/matrix_props/is_positive_semidefinite.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     1873 2022-05-09 18:55:39.000000 toqito-1.0.5/toqito/matrix_props/is_projection.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     1489 2023-01-09 11:17:36.000000 toqito-1.0.5/toqito/matrix_props/is_square.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     1773 2022-05-09 18:55:39.000000 toqito-1.0.5/toqito/matrix_props/is_symmetric.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     2371 2022-05-09 18:55:39.000000 toqito-1.0.5/toqito/matrix_props/is_unitary.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     2877 2023-01-09 11:17:36.000000 toqito-1.0.5/toqito/matrix_props/majorizes.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)    16191 2023-01-09 11:17:36.000000 toqito-1.0.5/toqito/matrix_props/sk_norm.py
-drwxr-xr-x   0 vincent.russo   (502) staff       (20)        0 2023-03-14 01:20:12.618644 toqito-1.0.5/toqito/measurement_ops/
--rw-r--r--   0 vincent.russo   (502) staff       (20)       95 2022-05-09 18:55:39.000000 toqito-1.0.5/toqito/measurement_ops/__init__.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     2131 2022-05-09 18:55:39.000000 toqito-1.0.5/toqito/measurement_ops/measure.py
-drwxr-xr-x   0 vincent.russo   (502) staff       (20)        0 2023-03-14 01:20:12.619409 toqito-1.0.5/toqito/measurement_props/
--rw-r--r--   0 vincent.russo   (502) staff       (20)       96 2022-05-09 18:55:39.000000 toqito-1.0.5/toqito/measurement_props/__init__.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     3028 2022-05-09 18:55:39.000000 toqito-1.0.5/toqito/measurement_props/is_povm.py
-drwxr-xr-x   0 vincent.russo   (502) staff       (20)        0 2023-03-14 01:20:12.622024 toqito-1.0.5/toqito/nonlocal_games/
--rw-r--r--   0 vincent.russo   (502) staff       (20)      317 2022-05-09 18:55:39.000000 toqito-1.0.5/toqito/nonlocal_games/__init__.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)    20186 2023-01-09 11:17:36.000000 toqito-1.0.5/toqito/nonlocal_games/extended_nonlocal_game.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)    26713 2023-01-09 11:17:36.000000 toqito-1.0.5/toqito/nonlocal_games/nonlocal_game.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     9655 2022-06-15 14:44:03.000000 toqito-1.0.5/toqito/nonlocal_games/quantum_hedging.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     9544 2023-03-11 11:52:07.000000 toqito-1.0.5/toqito/nonlocal_games/xor_game.py
-drwxr-xr-x   0 vincent.russo   (502) staff       (20)        0 2023-03-14 01:20:12.627097 toqito-1.0.5/toqito/perms/
--rw-r--r--   0 vincent.russo   (502) staff       (20)      558 2022-05-09 18:55:39.000000 toqito-1.0.5/toqito/perms/__init__.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     3507 2022-06-15 14:44:03.000000 toqito-1.0.5/toqito/perms/antisymmetric_projection.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     2398 2023-01-09 11:17:36.000000 toqito-1.0.5/toqito/perms/perfect_matchings.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     1439 2023-01-09 11:17:36.000000 toqito-1.0.5/toqito/perms/perm_sign.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     2052 2023-01-09 11:17:36.000000 toqito-1.0.5/toqito/perms/permutation_operator.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     8634 2023-01-09 11:17:36.000000 toqito-1.0.5/toqito/perms/permute_systems.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     5127 2023-01-09 11:17:36.000000 toqito-1.0.5/toqito/perms/swap.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     2038 2023-01-09 11:17:36.000000 toqito-1.0.5/toqito/perms/swap_operator.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     3030 2022-06-15 14:44:03.000000 toqito-1.0.5/toqito/perms/symmetric_projection.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     1691 2022-05-09 18:55:39.000000 toqito-1.0.5/toqito/perms/unique_perms.py
-drwxr-xr-x   0 vincent.russo   (502) staff       (20)        0 2023-03-14 01:20:12.639001 toqito-1.0.5/toqito/random/
--rw-r--r--   0 vincent.russo   (502) staff       (20)      353 2022-05-09 18:55:39.000000 toqito-1.0.5/toqito/random/__init__.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     3689 2023-03-01 20:54:25.000000 toqito-1.0.5/toqito/random/random_density_matrix.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     1396 2022-05-09 18:55:39.000000 toqito-1.0.5/toqito/random/random_ginibre.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     2595 2022-05-09 18:55:39.000000 toqito-1.0.5/toqito/random/random_povm.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     2505 2023-01-09 11:17:36.000000 toqito-1.0.5/toqito/random/random_state_vector.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     3197 2023-01-09 11:17:36.000000 toqito-1.0.5/toqito/random/random_unitary.py
-drwxr-xr-x   0 vincent.russo   (502) staff       (20)        0 2023-03-14 01:20:12.646367 toqito-1.0.5/toqito/state_metrics/
--rw-r--r--   0 vincent.russo   (502) staff       (20)      628 2023-01-09 11:17:36.000000 toqito-1.0.5/toqito/state_metrics/__init__.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     2533 2023-01-09 11:17:36.000000 toqito-1.0.5/toqito/state_metrics/bures_distance.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     3263 2023-01-09 11:17:36.000000 toqito-1.0.5/toqito/state_metrics/fidelity.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     2186 2023-01-09 11:17:36.000000 toqito-1.0.5/toqito/state_metrics/helstrom_holevo.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     1433 2023-01-09 11:17:36.000000 toqito-1.0.5/toqito/state_metrics/hilbert_schmidt.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     1361 2023-01-09 11:17:36.000000 toqito-1.0.5/toqito/state_metrics/hilbert_schmidt_inner_product.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     4153 2023-01-09 11:17:36.000000 toqito-1.0.5/toqito/state_metrics/matsumoto_fidelity.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     2938 2023-01-09 11:17:36.000000 toqito-1.0.5/toqito/state_metrics/sub_fidelity.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     1996 2023-01-09 11:17:36.000000 toqito-1.0.5/toqito/state_metrics/trace_distance.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     1393 2022-05-09 18:55:39.000000 toqito-1.0.5/toqito/state_metrics/trace_norm.py
-drwxr-xr-x   0 vincent.russo   (502) staff       (20)        0 2023-03-14 01:20:12.648059 toqito-1.0.5/toqito/state_ops/
--rw-r--r--   0 vincent.russo   (502) staff       (20)      166 2022-05-09 21:26:26.000000 toqito-1.0.5/toqito/state_ops/__init__.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     2268 2023-01-09 11:17:36.000000 toqito-1.0.5/toqito/state_ops/pure_to_mixed.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     6454 2023-01-09 11:17:36.000000 toqito-1.0.5/toqito/state_ops/schmidt_decomposition.py
-drwxr-xr-x   0 vincent.russo   (502) staff       (20)        0 2023-03-14 01:20:12.651937 toqito-1.0.5/toqito/state_opt/
--rw-r--r--   0 vincent.russo   (502) staff       (20)      402 2022-05-09 18:55:39.000000 toqito-1.0.5/toqito/state_opt/__init__.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     7266 2023-01-09 11:17:36.000000 toqito-1.0.5/toqito/state_opt/optimal_clone.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)    11336 2023-03-11 11:51:59.000000 toqito-1.0.5/toqito/state_opt/ppt_distinguishability.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     5153 2023-01-09 11:17:36.000000 toqito-1.0.5/toqito/state_opt/state_distinguishability.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     7196 2022-07-01 12:50:38.000000 toqito-1.0.5/toqito/state_opt/state_exclusion.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)      633 2022-05-09 18:55:39.000000 toqito-1.0.5/toqito/state_opt/state_helper.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     8835 2023-01-09 11:17:36.000000 toqito-1.0.5/toqito/state_opt/symmetric_extension_hierarchy.py
-drwxr-xr-x   0 vincent.russo   (502) staff       (20)        0 2023-03-14 01:20:12.661308 toqito-1.0.5/toqito/state_props/
--rw-r--r--   0 vincent.russo   (502) staff       (20)     1188 2023-01-09 11:17:36.000000 toqito-1.0.5/toqito/state_props/__init__.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     2628 2023-01-09 11:17:36.000000 toqito-1.0.5/toqito/state_props/concurrence.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     4038 2023-01-09 11:17:36.000000 toqito-1.0.5/toqito/state_props/entanglement_of_formation.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     5540 2023-01-09 11:17:36.000000 toqito-1.0.5/toqito/state_props/has_symmetric_extension.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     3277 2022-05-09 18:55:39.000000 toqito-1.0.5/toqito/state_props/in_separable_ball.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     1802 2022-05-09 18:55:39.000000 toqito-1.0.5/toqito/state_props/is_ensemble.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     1226 2022-05-09 18:55:39.000000 toqito-1.0.5/toqito/state_props/is_mixed.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     2445 2023-01-09 11:17:36.000000 toqito-1.0.5/toqito/state_props/is_mutually_orthogonal.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     3639 2023-01-09 11:17:36.000000 toqito-1.0.5/toqito/state_props/is_mutually_unbiased_basis.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     1332 2023-01-09 11:17:36.000000 toqito-1.0.5/toqito/state_props/is_npt.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     3210 2023-01-09 11:17:36.000000 toqito-1.0.5/toqito/state_props/is_ppt.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     4805 2023-01-09 11:17:36.000000 toqito-1.0.5/toqito/state_props/is_product.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     2705 2023-01-09 11:17:36.000000 toqito-1.0.5/toqito/state_props/is_pure.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     7456 2023-01-09 11:17:36.000000 toqito-1.0.5/toqito/state_props/is_separable.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     1724 2022-05-09 18:55:39.000000 toqito-1.0.5/toqito/state_props/l1_norm_coherence.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     2750 2023-01-09 11:17:36.000000 toqito-1.0.5/toqito/state_props/log_negativity.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     2811 2023-01-09 11:17:36.000000 toqito-1.0.5/toqito/state_props/negativity.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     1835 2023-01-09 11:17:36.000000 toqito-1.0.5/toqito/state_props/purity.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     4285 2023-01-09 11:17:36.000000 toqito-1.0.5/toqito/state_props/schmidt_rank.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     2342 2023-01-09 11:17:36.000000 toqito-1.0.5/toqito/state_props/sk_vec_norm.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     3088 2023-01-09 11:17:36.000000 toqito-1.0.5/toqito/state_props/von_neumann_entropy.py
-drwxr-xr-x   0 vincent.russo   (502) staff       (20)        0 2023-03-14 01:20:12.668923 toqito-1.0.5/toqito/states/
--rw-r--r--   0 vincent.russo   (502) staff       (20)      732 2022-05-09 18:55:39.000000 toqito-1.0.5/toqito/states/__init__.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     1471 2023-01-09 11:17:36.000000 toqito-1.0.5/toqito/states/basis.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     1902 2023-01-09 11:17:36.000000 toqito-1.0.5/toqito/states/bell.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     2384 2022-05-09 18:55:39.000000 toqito-1.0.5/toqito/states/brauer.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     1734 2023-01-09 11:17:36.000000 toqito-1.0.5/toqito/states/breuer.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     3157 2022-05-09 18:55:39.000000 toqito-1.0.5/toqito/states/chessboard.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     3547 2023-01-09 11:17:36.000000 toqito-1.0.5/toqito/states/domino.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     3631 2022-05-09 18:55:39.000000 toqito-1.0.5/toqito/states/gen_bell.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     3119 2023-01-09 11:17:36.000000 toqito-1.0.5/toqito/states/ghz.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     2507 2023-01-09 11:17:36.000000 toqito-1.0.5/toqito/states/gisin.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     6942 2023-01-09 11:17:36.000000 toqito-1.0.5/toqito/states/horodecki.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     2568 2022-06-15 14:44:03.000000 toqito-1.0.5/toqito/states/isotropic.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     1958 2023-01-09 11:17:36.000000 toqito-1.0.5/toqito/states/max_entangled.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     2114 2023-03-11 11:51:59.000000 toqito-1.0.5/toqito/states/max_mixed.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     2918 2022-06-15 14:44:03.000000 toqito-1.0.5/toqito/states/singlet.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     2479 2023-01-09 11:17:36.000000 toqito-1.0.5/toqito/states/tile.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     2599 2023-01-09 11:17:36.000000 toqito-1.0.5/toqito/states/w_state.py
--rw-r--r--   0 vincent.russo   (502) staff       (20)     5740 2023-01-09 11:17:36.000000 toqito-1.0.5/toqito/states/werner.py
-drwxr-xr-x   0 vincent.russo   (502) staff       (20)        0 2023-03-14 01:20:12.586117 toqito-1.0.5/toqito.egg-info/
--rw-r--r--   0 vincent.russo   (502) staff       (20)     3818 2023-03-14 01:20:12.000000 toqito-1.0.5/toqito.egg-info/PKG-INFO
--rw-r--r--   0 vincent.russo   (502) staff       (20)    11707 2023-03-14 01:20:12.000000 toqito-1.0.5/toqito.egg-info/SOURCES.txt
--rw-r--r--   0 vincent.russo   (502) staff       (20)        1 2023-03-14 01:20:12.000000 toqito-1.0.5/toqito.egg-info/dependency_links.txt
--rw-r--r--   0 vincent.russo   (502) staff       (20)       41 2023-03-14 01:20:12.000000 toqito-1.0.5/toqito.egg-info/requires.txt
--rw-r--r--   0 vincent.russo   (502) staff       (20)       13 2023-03-14 01:20:12.000000 toqito-1.0.5/toqito.egg-info/top_level.txt
+drwxr-xr-x   0 vrusso     (502) staff       (20)        0 2023-07-08 08:38:24.046903 toqito-1.0.6/
+-rw-r--r--   0 vrusso     (502) staff       (20)     1070 2023-06-02 18:20:51.000000 toqito-1.0.6/LICENSE
+-rw-r--r--   0 vrusso     (502) staff       (20)     4817 2023-07-08 08:38:24.047024 toqito-1.0.6/PKG-INFO
+-rw-r--r--   0 vrusso     (502) staff       (20)     4214 2023-06-24 22:22:46.000000 toqito-1.0.6/README.md
+-rw-r--r--   0 vrusso     (502) staff       (20)     1315 2023-07-08 08:38:12.000000 toqito-1.0.6/pyproject.toml
+-rw-r--r--   0 vrusso     (502) staff       (20)      108 2023-07-08 08:38:24.047596 toqito-1.0.6/setup.cfg
+-rw-r--r--   0 vrusso     (502) staff       (20)      951 2023-07-08 08:38:15.000000 toqito-1.0.6/setup.py
+drwxr-xr-x   0 vrusso     (502) staff       (20)        0 2023-07-08 08:38:23.897711 toqito-1.0.6/tests/
+-rw-r--r--   0 vrusso     (502) staff       (20)       37 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/__init__.py
+drwxr-xr-x   0 vrusso     (502) staff       (20)        0 2023-07-08 08:38:23.901334 toqito-1.0.6/tests/test_channel_metrics/
+-rw-r--r--   0 vrusso     (502) staff       (20)       33 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_channel_metrics/__init__.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     1295 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_channel_metrics/test_channel_fidelity.py
+-rw-r--r--   0 vrusso     (502) staff       (20)      517 2023-06-24 22:22:46.000000 toqito-1.0.6/tests/test_channel_metrics/test_completely_bounded_spectral_norm.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     1245 2023-06-24 22:22:46.000000 toqito-1.0.6/tests/test_channel_metrics/test_completely_bounded_trace_norm.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     1227 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_channel_metrics/test_diamond_norm.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     1355 2023-06-24 22:22:46.000000 toqito-1.0.6/tests/test_channel_metrics/test_fidelity_of_separability.py
+drwxr-xr-x   0 vrusso     (502) staff       (20)        0 2023-07-08 08:38:23.903979 toqito-1.0.6/tests/test_channel_ops/
+-rw-r--r--   0 vrusso     (502) staff       (20)       29 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_channel_ops/__init__.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     2818 2023-06-24 22:22:46.000000 toqito-1.0.6/tests/test_channel_ops/test_apply_channel.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     4683 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_channel_ops/test_choi_to_kraus.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     3411 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_channel_ops/test_dual_channel.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     4801 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_channel_ops/test_kraus_to_choi.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     5442 2023-06-24 22:22:46.000000 toqito-1.0.6/tests/test_channel_ops/test_partial_channel.py
+drwxr-xr-x   0 vrusso     (502) staff       (20)        0 2023-07-08 08:38:23.908368 toqito-1.0.6/tests/test_channel_props/
+-rw-r--r--   0 vrusso     (502) staff       (20)       31 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_channel_props/__init__.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     1351 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_channel_props/test_choi_rank.py
+-rw-r--r--   0 vrusso     (502) staff       (20)      750 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_channel_props/test_is_completely_positive.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     1290 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_channel_props/test_is_herm_preserving.py
+-rw-r--r--   0 vrusso     (502) staff       (20)      683 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_channel_props/test_is_positive.py
+-rw-r--r--   0 vrusso     (502) staff       (20)      732 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_channel_props/test_is_quantum_channel.py
+-rw-r--r--   0 vrusso     (502) staff       (20)      726 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_channel_props/test_is_trace_preserving.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     1999 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_channel_props/test_is_unital.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     1540 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_channel_props/test_is_unitary.py
+drwxr-xr-x   0 vrusso     (502) staff       (20)        0 2023-07-08 08:38:23.914044 toqito-1.0.6/tests/test_channels/
+-rw-r--r--   0 vrusso     (502) staff       (20)       26 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_channels/__init__.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     1478 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_channels/test_choi.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     1115 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_channels/test_dephasing.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     1136 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_channels/test_depolarizing.py
+-rw-r--r--   0 vrusso     (502) staff       (20)    35512 2023-06-24 22:22:46.000000 toqito-1.0.6/tests/test_channels/test_partial_trace.py
+-rw-r--r--   0 vrusso     (502) staff       (20)    33772 2023-06-24 22:22:46.000000 toqito-1.0.6/tests/test_channels/test_partial_transpose.py
+-rw-r--r--   0 vrusso     (502) staff       (20)    11294 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_channels/test_realignment.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     1418 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_channels/test_reduction.py
+drwxr-xr-x   0 vrusso     (502) staff       (20)        0 2023-07-08 08:38:23.918491 toqito-1.0.6/tests/test_helper/
+-rw-r--r--   0 vrusso     (502) staff       (20)       24 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_helper/__init__.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     4265 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_helper/test_channel_dim.py
+-rw-r--r--   0 vrusso     (502) staff       (20)      385 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_helper/test_cvx_kron.py
+-rw-r--r--   0 vrusso     (502) staff       (20)      836 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_helper/test_expr_as_np_array.py
+-rw-r--r--   0 vrusso     (502) staff       (20)      445 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_helper/test_np_array_as_expr.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     2644 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_helper/test_npa_constraints.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     2086 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_helper/test_update_odometer.py
+drwxr-xr-x   0 vrusso     (502) staff       (20)        0 2023-07-08 08:38:23.923362 toqito-1.0.6/tests/test_matrices/
+-rw-r--r--   0 vrusso     (502) staff       (20)       21 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_matrices/__init__.py
+-rw-r--r--   0 vrusso     (502) staff       (20)      387 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_matrices/test_cnot.py
+-rw-r--r--   0 vrusso     (502) staff       (20)      427 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_matrices/test_fourier.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     2847 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_matrices/test_gell_mann.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     2637 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_matrices/test_gen_gell_mann.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     1171 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_matrices/test_gen_pauli.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     1791 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_matrices/test_hadamard.py
+-rw-r--r--   0 vrusso     (502) staff       (20)      624 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_matrices/test_iden.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     2666 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_matrices/test_pauli.py
+-rw-r--r--   0 vrusso     (502) staff       (20)      709 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_matrices/test_standard_basis.py
+drwxr-xr-x   0 vrusso     (502) staff       (20)        0 2023-07-08 08:38:23.926159 toqito-1.0.6/tests/test_matrix_ops/
+-rw-r--r--   0 vrusso     (502) staff       (20)       30 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_matrix_ops/__init__.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     1353 2023-06-24 22:22:46.000000 toqito-1.0.6/tests/test_matrix_ops/test_inner_product.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     1199 2023-06-24 22:22:46.000000 toqito-1.0.6/tests/test_matrix_ops/test_outer_product.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     4247 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_matrix_ops/test_tensor.py
+-rw-r--r--   0 vrusso     (502) staff       (20)      772 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_matrix_ops/test_unvec.py
+-rw-r--r--   0 vrusso     (502) staff       (20)      430 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_matrix_ops/test_vec.py
+-rw-r--r--   0 vrusso     (502) staff       (20)      972 2023-07-08 07:42:22.000000 toqito-1.0.6/tests/test_matrix_ops/test_vectors_from_gram_matrix.py
+-rw-r--r--   0 vrusso     (502) staff       (20)      655 2023-07-08 07:42:22.000000 toqito-1.0.6/tests/test_matrix_ops/test_vectors_to_gram_matrix.py
+drwxr-xr-x   0 vrusso     (502) staff       (20)        0 2023-07-08 08:38:23.937520 toqito-1.0.6/tests/test_matrix_props/
+-rw-r--r--   0 vrusso     (502) staff       (20)       30 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_matrix_props/__init__.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     1564 2023-06-05 15:52:22.000000 toqito-1.0.6/tests/test_matrix_props/test_is_block_positive.py
+-rw-r--r--   0 vrusso     (502) staff       (20)      637 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_matrix_props/test_is_commuting.py
+-rw-r--r--   0 vrusso     (502) staff       (20)      604 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_matrix_props/test_is_density.py
+-rw-r--r--   0 vrusso     (502) staff       (20)      666 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_matrix_props/test_is_diagonal.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     1458 2023-06-24 22:22:46.000000 toqito-1.0.6/tests/test_matrix_props/test_is_diagonally_dominant.py
+-rw-r--r--   0 vrusso     (502) staff       (20)      692 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_matrix_props/test_is_hermitian.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     1236 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_matrix_props/test_is_idempotent.py
+-rw-r--r--   0 vrusso     (502) staff       (20)      645 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_matrix_props/test_is_identity.py
+-rw-r--r--   0 vrusso     (502) staff       (20)      963 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_matrix_props/test_is_normal.py
+-rw-r--r--   0 vrusso     (502) staff       (20)      777 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_matrix_props/test_is_orthonormal.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     1939 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_matrix_props/test_is_permutation.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     1607 2023-06-24 22:22:46.000000 toqito-1.0.6/tests/test_matrix_props/test_is_positive_definite.py
+-rw-r--r--   0 vrusso     (502) staff       (20)      601 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_matrix_props/test_is_positive_semidefinite.py
+-rw-r--r--   0 vrusso     (502) staff       (20)      889 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_matrix_props/test_is_projection.py
+-rw-r--r--   0 vrusso     (502) staff       (20)      648 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_matrix_props/test_is_square.py
+-rw-r--r--   0 vrusso     (502) staff       (20)      695 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_matrix_props/test_is_symmetric.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     1063 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_matrix_props/test_is_unitary.py
+-rw-r--r--   0 vrusso     (502) staff       (20)      907 2023-06-05 15:52:22.000000 toqito-1.0.6/tests/test_matrix_props/test_majorizes.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     2561 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_matrix_props/test_sk_norm.py
+-rw-r--r--   0 vrusso     (502) staff       (20)      599 2023-06-24 22:22:46.000000 toqito-1.0.6/tests/test_matrix_props/test_trace_norm.py
+drwxr-xr-x   0 vrusso     (502) staff       (20)        0 2023-07-08 08:38:23.938370 toqito-1.0.6/tests/test_measurement_ops/
+-rw-r--r--   0 vrusso     (502) staff       (20)       33 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_measurement_ops/__init__.py
+-rw-r--r--   0 vrusso     (502) staff       (20)      585 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_measurement_ops/test_measure.py
+drwxr-xr-x   0 vrusso     (502) staff       (20)        0 2023-07-08 08:38:23.939122 toqito-1.0.6/tests/test_measurement_props/
+-rw-r--r--   0 vrusso     (502) staff       (20)       35 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_measurement_props/__init__.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     1009 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_measurement_props/test_is_povm.py
+drwxr-xr-x   0 vrusso     (502) staff       (20)        0 2023-07-08 08:38:23.940987 toqito-1.0.6/tests/test_nonlocal_games/
+-rw-r--r--   0 vrusso     (502) staff       (20)       47 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_nonlocal_games/__init__.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     7615 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_nonlocal_games/test_extended_nonlocal_game.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     9362 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_nonlocal_games/test_nonlocal_game.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     4076 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_nonlocal_games/test_quantum_hedging.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     7023 2023-06-24 22:22:46.000000 toqito-1.0.6/tests/test_nonlocal_games/test_xor_game.py
+drwxr-xr-x   0 vrusso     (502) staff       (20)        0 2023-07-08 08:38:23.945458 toqito-1.0.6/tests/test_perms/
+-rw-r--r--   0 vrusso     (502) staff       (20)       23 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_perms/__init__.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     1312 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_perms/test_antisymmetric_projection.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     1768 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_perms/test_perfect_matchings.py
+-rw-r--r--   0 vrusso     (502) staff       (20)      468 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_perms/test_perm_sign.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     3164 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_perms/test_permutation_operator.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     8070 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_perms/test_permute_systems.py
+-rw-r--r--   0 vrusso     (502) staff       (20)    16464 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_perms/test_swap.py
+-rw-r--r--   0 vrusso     (502) staff       (20)      764 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_perms/test_swap_operator.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     4830 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_perms/test_symmetric_projection.py
+-rw-r--r--   0 vrusso     (502) staff       (20)      327 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_perms/test_unique_perms.py
+drwxr-xr-x   0 vrusso     (502) staff       (20)        0 2023-07-08 08:38:23.948993 toqito-1.0.6/tests/test_random/
+-rw-r--r--   0 vrusso     (502) staff       (20)       24 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_random/__init__.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     1213 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_random/test_random_density_matrix.py
+-rw-r--r--   0 vrusso     (502) staff       (20)      388 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_random/test_random_ginibre.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     1138 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_random/test_random_povm.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     1560 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_random/test_random_state_vector.py
+-rw-r--r--   0 vrusso     (502) staff       (20)      706 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_random/test_random_unitary.py
+drwxr-xr-x   0 vrusso     (502) staff       (20)        0 2023-07-08 08:38:23.954630 toqito-1.0.6/tests/test_state_metrics/
+-rw-r--r--   0 vrusso     (502) staff       (20)       41 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_state_metrics/__init__.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     2209 2023-07-07 07:19:23.000000 toqito-1.0.6/tests/test_state_metrics/test_bures_angle.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     2216 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_state_metrics/test_bures_distance.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     2065 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_state_metrics/test_fidelity.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     1580 2023-06-24 22:22:46.000000 toqito-1.0.6/tests/test_state_metrics/test_fidelity_of_separability.py
+-rw-r--r--   0 vrusso     (502) staff       (20)      870 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_state_metrics/test_helstrom_holevo.py
+-rw-r--r--   0 vrusso     (502) staff       (20)      736 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_state_metrics/test_hilbert_schmidt.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     1795 2023-06-24 22:22:46.000000 toqito-1.0.6/tests/test_state_metrics/test_hilbert_schmidt_inner_product.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     1937 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_state_metrics/test_matsumoto_fidelity.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     1900 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_state_metrics/test_sub_fidelity.py
+-rw-r--r--   0 vrusso     (502) staff       (20)      851 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_state_metrics/test_trace_distance.py
+drwxr-xr-x   0 vrusso     (502) staff       (20)        0 2023-07-08 08:38:23.956103 toqito-1.0.6/tests/test_state_ops/
+-rw-r--r--   0 vrusso     (502) staff       (20)       44 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_state_ops/__init__.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     1178 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_state_ops/test_pure_to_mixed.py
+-rw-r--r--   0 vrusso     (502) staff       (20)    10445 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_state_ops/test_schmidt_decomposition.py
+drwxr-xr-x   0 vrusso     (502) staff       (20)        0 2023-07-08 08:38:23.958621 toqito-1.0.6/tests/test_state_opt/
+-rw-r--r--   0 vrusso     (502) staff       (20)       47 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_state_opt/__init__.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     1682 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_state_opt/test_optimal_clone.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     9162 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_state_opt/test_ppt_distinguishability.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     2964 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_state_opt/test_state_distinguishability.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     1171 2023-07-08 07:42:22.000000 toqito-1.0.6/tests/test_state_opt/test_state_exclusion.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     5483 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_state_opt/test_symmetric_extension_hierarchy.py
+drwxr-xr-x   0 vrusso     (502) staff       (20)        0 2023-07-08 08:38:23.968996 toqito-1.0.6/tests/test_state_props/
+-rw-r--r--   0 vrusso     (502) staff       (20)       44 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_state_props/__init__.py
+-rw-r--r--   0 vrusso     (502) staff       (20)      996 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_state_props/test_concurrence.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     1611 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_state_props/test_entanglement_of_formation.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     2250 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_state_props/test_has_symmetric_extension.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     1306 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_state_props/test_in_separable_ball.py
+-rw-r--r--   0 vrusso     (502) staff       (20)      651 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_state_props/test_is_ensemble.py
+-rw-r--r--   0 vrusso     (502) staff       (20)      401 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_state_props/test_is_mixed.py
+-rw-r--r--   0 vrusso     (502) staff       (20)      854 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_state_props/test_is_mutually_orthogonal.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     1201 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_state_props/test_is_mutually_unbiased_basis.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     1226 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_state_props/test_is_npt.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     1222 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_state_props/test_is_ppt.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     2047 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_state_props/test_is_product.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     1128 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_state_props/test_is_pure.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     3502 2023-06-24 22:22:46.000000 toqito-1.0.6/tests/test_state_props/test_is_separable.py
+-rw-r--r--   0 vrusso     (502) staff       (20)      410 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_state_props/test_l1_norm_coherence.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     1324 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_state_props/test_log_negativity.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     1284 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_state_props/test_negativity.py
+-rw-r--r--   0 vrusso     (502) staff       (20)      716 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_state_props/test_purity.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     2970 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_state_props/test_schmidt_rank.py
+-rw-r--r--   0 vrusso     (502) staff       (20)      511 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_state_props/test_sk_vec_norm.py
+-rw-r--r--   0 vrusso     (502) staff       (20)      933 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_state_props/test_von_neumann_entropy.py
+drwxr-xr-x   0 vrusso     (502) staff       (20)        0 2023-07-08 08:38:23.975751 toqito-1.0.6/tests/test_states/
+-rw-r--r--   0 vrusso     (502) staff       (20)       24 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_states/__init__.py
+-rw-r--r--   0 vrusso     (502) staff       (20)      930 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_states/test_basis.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     1588 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_states/test_bell.py
+-rw-r--r--   0 vrusso     (502) staff       (20)      760 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_states/test_brauer.py
+-rw-r--r--   0 vrusso     (502) staff       (20)      612 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_states/test_breuer.py
+-rw-r--r--   0 vrusso     (502) staff       (20)      761 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_states/test_chessboard.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     2821 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_states/test_domino.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     1415 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_states/test_gen_bell.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     1847 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_states/test_ghz.py
+-rw-r--r--   0 vrusso     (502) staff       (20)      656 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_states/test_gisin.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     2659 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_states/test_horodecki.py
+-rw-r--r--   0 vrusso     (502) staff       (20)      459 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_states/test_isotropic.py
+-rw-r--r--   0 vrusso     (502) staff       (20)      852 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_states/test_max_entangled.py
+-rw-r--r--   0 vrusso     (502) staff       (20)      730 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_states/test_max_mixed.py
+-rw-r--r--   0 vrusso     (502) staff       (20)      427 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_states/test_singlet.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     2455 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_states/test_tile.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     1461 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_states/test_w_state.py
+-rw-r--r--   0 vrusso     (502) staff       (20)      729 2023-06-02 18:20:51.000000 toqito-1.0.6/tests/test_states/test_werner.py
+drwxr-xr-x   0 vrusso     (502) staff       (20)        0 2023-07-08 08:38:23.976045 toqito-1.0.6/toqito/
+-rw-r--r--   0 vrusso     (502) staff       (20)       59 2023-06-02 18:20:51.000000 toqito-1.0.6/toqito/__init__.py
+drwxr-xr-x   0 vrusso     (502) staff       (20)        0 2023-07-08 08:38:23.982354 toqito-1.0.6/toqito/channel_metrics/
+-rw-r--r--   0 vrusso     (502) staff       (20)      456 2023-06-24 22:22:46.000000 toqito-1.0.6/toqito/channel_metrics/__init__.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     3638 2023-06-05 15:52:22.000000 toqito-1.0.6/toqito/channel_metrics/channel_fidelity.py
+-rw-r--r--   0 vrusso     (502) staff       (20)      972 2023-06-24 22:22:46.000000 toqito-1.0.6/toqito/channel_metrics/completely_bounded_spectral_norm.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     2289 2023-06-24 22:22:46.000000 toqito-1.0.6/toqito/channel_metrics/completely_bounded_trace_norm.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     2224 2023-06-02 18:20:51.000000 toqito-1.0.6/toqito/channel_metrics/diamond_norm.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     8138 2023-06-24 22:22:46.000000 toqito-1.0.6/toqito/channel_metrics/fidelity_of_separability.py
+drwxr-xr-x   0 vrusso     (502) staff       (20)        0 2023-07-08 08:38:23.984567 toqito-1.0.6/toqito/channel_ops/
+-rw-r--r--   0 vrusso     (502) staff       (20)      347 2023-06-02 18:20:51.000000 toqito-1.0.6/toqito/channel_ops/__init__.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     5151 2023-06-24 22:22:46.000000 toqito-1.0.6/toqito/channel_ops/apply_channel.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     4456 2023-06-02 18:20:51.000000 toqito-1.0.6/toqito/channel_ops/choi_to_kraus.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     2959 2023-06-02 18:20:51.000000 toqito-1.0.6/toqito/channel_ops/dual_channel.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     2377 2023-06-02 18:20:51.000000 toqito-1.0.6/toqito/channel_ops/kraus_to_choi.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     6753 2023-06-02 18:20:51.000000 toqito-1.0.6/toqito/channel_ops/partial_channel.py
+drwxr-xr-x   0 vrusso     (502) staff       (20)        0 2023-07-08 08:38:23.987841 toqito-1.0.6/toqito/channel_props/
+-rw-r--r--   0 vrusso     (502) staff       (20)      562 2023-06-02 18:20:51.000000 toqito-1.0.6/toqito/channel_props/__init__.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     2792 2023-06-02 18:20:51.000000 toqito-1.0.6/toqito/channel_props/choi_rank.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     3050 2023-06-02 18:20:51.000000 toqito-1.0.6/toqito/channel_props/is_completely_positive.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     2598 2023-06-02 18:20:51.000000 toqito-1.0.6/toqito/channel_props/is_herm_preserving.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     2540 2023-06-02 18:20:51.000000 toqito-1.0.6/toqito/channel_props/is_positive.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     1988 2023-06-02 18:20:51.000000 toqito-1.0.6/toqito/channel_props/is_quantum_channel.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     3494 2023-06-24 22:22:46.000000 toqito-1.0.6/toqito/channel_props/is_trace_preserving.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     2368 2023-06-02 18:20:51.000000 toqito-1.0.6/toqito/channel_props/is_unital.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     2822 2023-06-02 18:20:51.000000 toqito-1.0.6/toqito/channel_props/is_unitary.py
+drwxr-xr-x   0 vrusso     (502) staff       (20)        0 2023-07-08 08:38:23.990908 toqito-1.0.6/toqito/channels/
+-rw-r--r--   0 vrusso     (502) staff       (20)      412 2023-06-02 18:20:51.000000 toqito-1.0.6/toqito/channels/__init__.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     4015 2023-06-02 18:20:51.000000 toqito-1.0.6/toqito/channels/choi.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     2916 2023-06-02 18:20:51.000000 toqito-1.0.6/toqito/channels/dephasing.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     3298 2023-06-02 18:20:51.000000 toqito-1.0.6/toqito/channels/depolarizing.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     7383 2023-06-24 22:22:46.000000 toqito-1.0.6/toqito/channels/partial_trace.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     7104 2023-06-24 22:22:46.000000 toqito-1.0.6/toqito/channels/partial_transpose.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     3117 2023-06-05 15:52:22.000000 toqito-1.0.6/toqito/channels/realignment.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     1678 2023-06-02 18:20:51.000000 toqito-1.0.6/toqito/channels/reduction.py
+drwxr-xr-x   0 vrusso     (502) staff       (20)        0 2023-07-08 08:38:23.994404 toqito-1.0.6/toqito/helper/
+-rw-r--r--   0 vrusso     (502) staff       (20)      425 2023-06-02 18:20:51.000000 toqito-1.0.6/toqito/helper/__init__.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     5929 2023-06-02 18:20:51.000000 toqito-1.0.6/toqito/helper/channel_dim.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     1090 2023-06-24 22:22:46.000000 toqito-1.0.6/toqito/helper/cvx_kron.py
+-rw-r--r--   0 vrusso     (502) staff       (20)      701 2023-06-02 18:20:51.000000 toqito-1.0.6/toqito/helper/expr_as_np_array.py
+-rw-r--r--   0 vrusso     (502) staff       (20)      748 2023-06-02 18:20:51.000000 toqito-1.0.6/toqito/helper/kp_norm.py
+-rw-r--r--   0 vrusso     (502) staff       (20)      447 2023-06-02 18:20:51.000000 toqito-1.0.6/toqito/helper/np_array_as_expr.py
+-rw-r--r--   0 vrusso     (502) staff       (20)    10189 2023-06-24 22:22:46.000000 toqito-1.0.6/toqito/helper/npa_hierarchy.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     2556 2023-06-02 18:20:51.000000 toqito-1.0.6/toqito/helper/update_odometer.py
+drwxr-xr-x   0 vrusso     (502) staff       (20)        0 2023-07-08 08:38:24.000187 toqito-1.0.6/toqito/matrices/
+-rw-r--r--   0 vrusso     (502) staff       (20)      512 2023-06-02 18:20:51.000000 toqito-1.0.6/toqito/matrices/__init__.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     1733 2023-06-02 18:20:51.000000 toqito-1.0.6/toqito/matrices/clock.py
+-rw-r--r--   0 vrusso     (502) staff       (20)      748 2023-06-02 18:20:51.000000 toqito-1.0.6/toqito/matrices/cnot.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     1816 2023-06-02 18:20:51.000000 toqito-1.0.6/toqito/matrices/fourier.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     4486 2023-06-02 18:20:51.000000 toqito-1.0.6/toqito/matrices/gell_mann.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     3064 2023-06-02 18:20:51.000000 toqito-1.0.6/toqito/matrices/gen_gell_mann.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     2688 2023-06-02 18:20:51.000000 toqito-1.0.6/toqito/matrices/gen_pauli.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     1793 2023-06-02 18:20:51.000000 toqito-1.0.6/toqito/matrices/hadamard.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     2119 2023-06-02 18:20:51.000000 toqito-1.0.6/toqito/matrices/iden.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     3004 2023-06-02 18:20:51.000000 toqito-1.0.6/toqito/matrices/pauli.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     1665 2023-06-02 18:20:51.000000 toqito-1.0.6/toqito/matrices/shift.py
+-rw-r--r--   0 vrusso     (502) staff       (20)      948 2023-06-24 22:22:46.000000 toqito-1.0.6/toqito/matrices/standard_basis.py
+drwxr-xr-x   0 vrusso     (502) staff       (20)        0 2023-07-08 08:38:24.002867 toqito-1.0.6/toqito/matrix_ops/
+-rw-r--r--   0 vrusso     (502) staff       (20)      437 2023-07-08 07:42:22.000000 toqito-1.0.6/toqito/matrix_ops/__init__.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     1785 2023-06-24 22:22:46.000000 toqito-1.0.6/toqito/matrix_ops/inner_product.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     2064 2023-06-24 22:22:46.000000 toqito-1.0.6/toqito/matrix_ops/outer_product.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     5043 2023-06-02 18:20:51.000000 toqito-1.0.6/toqito/matrix_ops/tensor.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     2345 2023-06-02 18:20:51.000000 toqito-1.0.6/toqito/matrix_ops/unvec.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     2158 2023-06-02 18:20:51.000000 toqito-1.0.6/toqito/matrix_ops/vec.py
+-rw-r--r--   0 vrusso     (502) staff       (20)      657 2023-07-08 07:42:22.000000 toqito-1.0.6/toqito/matrix_ops/vectors_from_gram_matrix.py
+-rw-r--r--   0 vrusso     (502) staff       (20)      392 2023-07-08 07:42:22.000000 toqito-1.0.6/toqito/matrix_ops/vectors_to_gram_matrix.py
+drwxr-xr-x   0 vrusso     (502) staff       (20)        0 2023-07-08 08:38:24.010058 toqito-1.0.6/toqito/matrix_props/
+-rw-r--r--   0 vrusso     (502) staff       (20)     1311 2023-06-24 22:22:46.000000 toqito-1.0.6/toqito/matrix_props/__init__.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     4184 2023-06-02 18:20:51.000000 toqito-1.0.6/toqito/matrix_props/is_block_positive.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     2341 2023-06-02 18:20:51.000000 toqito-1.0.6/toqito/matrix_props/is_commuting.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     2218 2023-06-02 18:20:51.000000 toqito-1.0.6/toqito/matrix_props/is_density.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     1994 2023-06-02 18:20:51.000000 toqito-1.0.6/toqito/matrix_props/is_diagonal.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     2119 2023-06-24 22:22:46.000000 toqito-1.0.6/toqito/matrix_props/is_diagonally_dominant.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     1780 2023-06-02 18:20:51.000000 toqito-1.0.6/toqito/matrix_props/is_hermitian.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     1716 2023-06-02 18:20:51.000000 toqito-1.0.6/toqito/matrix_props/is_idempotent.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     2042 2023-06-02 18:20:51.000000 toqito-1.0.6/toqito/matrix_props/is_identity.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     1896 2023-06-02 18:20:51.000000 toqito-1.0.6/toqito/matrix_props/is_normal.py
+-rw-r--r--   0 vrusso     (502) staff       (20)      488 2023-06-24 22:22:46.000000 toqito-1.0.6/toqito/matrix_props/is_orthonormal.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     1776 2023-06-02 18:20:51.000000 toqito-1.0.6/toqito/matrix_props/is_permutation.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     2015 2023-06-24 22:22:46.000000 toqito-1.0.6/toqito/matrix_props/is_positive_definite.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     1679 2023-06-02 18:20:51.000000 toqito-1.0.6/toqito/matrix_props/is_positive_semidefinite.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     1873 2023-06-02 18:20:51.000000 toqito-1.0.6/toqito/matrix_props/is_projection.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     1489 2023-06-02 18:20:51.000000 toqito-1.0.6/toqito/matrix_props/is_square.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     1773 2023-06-02 18:20:51.000000 toqito-1.0.6/toqito/matrix_props/is_symmetric.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     2371 2023-06-02 18:20:51.000000 toqito-1.0.6/toqito/matrix_props/is_unitary.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     2872 2023-06-05 15:52:22.000000 toqito-1.0.6/toqito/matrix_props/majorizes.py
+-rw-r--r--   0 vrusso     (502) staff       (20)    16195 2023-06-05 15:52:22.000000 toqito-1.0.6/toqito/matrix_props/sk_norm.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     1455 2023-06-24 22:22:46.000000 toqito-1.0.6/toqito/matrix_props/trace_norm.py
+drwxr-xr-x   0 vrusso     (502) staff       (20)        0 2023-07-08 08:38:24.011011 toqito-1.0.6/toqito/measurement_ops/
+-rw-r--r--   0 vrusso     (502) staff       (20)       95 2023-06-02 18:20:51.000000 toqito-1.0.6/toqito/measurement_ops/__init__.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     2131 2023-06-02 18:20:51.000000 toqito-1.0.6/toqito/measurement_ops/measure.py
+drwxr-xr-x   0 vrusso     (502) staff       (20)        0 2023-07-08 08:38:24.012191 toqito-1.0.6/toqito/measurement_props/
+-rw-r--r--   0 vrusso     (502) staff       (20)       96 2023-06-02 18:20:51.000000 toqito-1.0.6/toqito/measurement_props/__init__.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     3028 2023-06-02 18:20:51.000000 toqito-1.0.6/toqito/measurement_props/is_povm.py
+drwxr-xr-x   0 vrusso     (502) staff       (20)        0 2023-07-08 08:38:24.015302 toqito-1.0.6/toqito/nonlocal_games/
+-rw-r--r--   0 vrusso     (502) staff       (20)      317 2023-06-02 18:20:51.000000 toqito-1.0.6/toqito/nonlocal_games/__init__.py
+-rw-r--r--   0 vrusso     (502) staff       (20)    20206 2023-06-24 22:22:46.000000 toqito-1.0.6/toqito/nonlocal_games/extended_nonlocal_game.py
+-rw-r--r--   0 vrusso     (502) staff       (20)    26713 2023-06-02 18:20:51.000000 toqito-1.0.6/toqito/nonlocal_games/nonlocal_game.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     9590 2023-06-24 22:22:46.000000 toqito-1.0.6/toqito/nonlocal_games/quantum_hedging.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     9379 2023-06-24 22:22:46.000000 toqito-1.0.6/toqito/nonlocal_games/xor_game.py
+drwxr-xr-x   0 vrusso     (502) staff       (20)        0 2023-07-08 08:38:24.019113 toqito-1.0.6/toqito/perms/
+-rw-r--r--   0 vrusso     (502) staff       (20)      558 2023-06-02 18:20:51.000000 toqito-1.0.6/toqito/perms/__init__.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     3507 2023-06-02 18:20:51.000000 toqito-1.0.6/toqito/perms/antisymmetric_projection.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     2398 2023-06-02 18:20:51.000000 toqito-1.0.6/toqito/perms/perfect_matchings.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     1439 2023-06-02 18:20:51.000000 toqito-1.0.6/toqito/perms/perm_sign.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     2052 2023-06-02 18:20:51.000000 toqito-1.0.6/toqito/perms/permutation_operator.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     8635 2023-06-24 22:22:46.000000 toqito-1.0.6/toqito/perms/permute_systems.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     5127 2023-06-02 18:20:51.000000 toqito-1.0.6/toqito/perms/swap.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     2038 2023-06-02 18:20:51.000000 toqito-1.0.6/toqito/perms/swap_operator.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     3030 2023-06-02 18:20:51.000000 toqito-1.0.6/toqito/perms/symmetric_projection.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     1691 2023-06-02 18:20:51.000000 toqito-1.0.6/toqito/perms/unique_perms.py
+drwxr-xr-x   0 vrusso     (502) staff       (20)        0 2023-07-08 08:38:24.021472 toqito-1.0.6/toqito/random/
+-rw-r--r--   0 vrusso     (502) staff       (20)      353 2023-06-02 18:20:51.000000 toqito-1.0.6/toqito/random/__init__.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     3689 2023-06-02 18:20:51.000000 toqito-1.0.6/toqito/random/random_density_matrix.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     1396 2023-06-02 18:20:51.000000 toqito-1.0.6/toqito/random/random_ginibre.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     2595 2023-06-02 18:20:51.000000 toqito-1.0.6/toqito/random/random_povm.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     2505 2023-06-02 18:20:51.000000 toqito-1.0.6/toqito/random/random_state_vector.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     3197 2023-06-02 18:20:51.000000 toqito-1.0.6/toqito/random/random_unitary.py
+drwxr-xr-x   0 vrusso     (502) staff       (20)        0 2023-07-08 08:38:24.026002 toqito-1.0.6/toqito/state_metrics/
+-rw-r--r--   0 vrusso     (502) staff       (20)      713 2023-07-07 07:19:23.000000 toqito-1.0.6/toqito/state_metrics/__init__.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     2525 2023-07-07 07:19:23.000000 toqito-1.0.6/toqito/state_metrics/bures_angle.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     2533 2023-06-02 18:20:51.000000 toqito-1.0.6/toqito/state_metrics/bures_distance.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     3263 2023-06-02 18:20:51.000000 toqito-1.0.6/toqito/state_metrics/fidelity.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     8108 2023-06-24 22:22:46.000000 toqito-1.0.6/toqito/state_metrics/fidelity_of_separability.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     2154 2023-06-24 22:22:46.000000 toqito-1.0.6/toqito/state_metrics/helstrom_holevo.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     1433 2023-06-02 18:20:51.000000 toqito-1.0.6/toqito/state_metrics/hilbert_schmidt.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     1362 2023-06-24 22:22:46.000000 toqito-1.0.6/toqito/state_metrics/hilbert_schmidt_inner_product.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     4153 2023-06-02 18:20:51.000000 toqito-1.0.6/toqito/state_metrics/matsumoto_fidelity.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     2938 2023-06-02 18:20:51.000000 toqito-1.0.6/toqito/state_metrics/sub_fidelity.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     1964 2023-06-24 22:22:46.000000 toqito-1.0.6/toqito/state_metrics/trace_distance.py
+drwxr-xr-x   0 vrusso     (502) staff       (20)        0 2023-07-08 08:38:24.027107 toqito-1.0.6/toqito/state_ops/
+-rw-r--r--   0 vrusso     (502) staff       (20)      166 2023-06-02 18:20:51.000000 toqito-1.0.6/toqito/state_ops/__init__.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     2268 2023-06-02 18:20:51.000000 toqito-1.0.6/toqito/state_ops/pure_to_mixed.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     6454 2023-06-02 18:20:51.000000 toqito-1.0.6/toqito/state_ops/schmidt_decomposition.py
+drwxr-xr-x   0 vrusso     (502) staff       (20)        0 2023-07-08 08:38:24.030762 toqito-1.0.6/toqito/state_opt/
+-rw-r--r--   0 vrusso     (502) staff       (20)      402 2023-06-02 18:20:51.000000 toqito-1.0.6/toqito/state_opt/__init__.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     7303 2023-06-24 22:22:46.000000 toqito-1.0.6/toqito/state_opt/optimal_clone.py
+-rw-r--r--   0 vrusso     (502) staff       (20)    11336 2023-06-02 18:20:51.000000 toqito-1.0.6/toqito/state_opt/ppt_distinguishability.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     5153 2023-06-02 18:20:51.000000 toqito-1.0.6/toqito/state_opt/state_distinguishability.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     5204 2023-07-07 09:02:55.000000 toqito-1.0.6/toqito/state_opt/state_exclusion.py
+-rw-r--r--   0 vrusso     (502) staff       (20)      633 2023-06-02 18:20:51.000000 toqito-1.0.6/toqito/state_opt/state_helper.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     8872 2023-06-05 15:52:22.000000 toqito-1.0.6/toqito/state_opt/symmetric_extension_hierarchy.py
+drwxr-xr-x   0 vrusso     (502) staff       (20)        0 2023-07-08 08:38:24.038918 toqito-1.0.6/toqito/state_props/
+-rw-r--r--   0 vrusso     (502) staff       (20)     1245 2023-06-24 22:22:46.000000 toqito-1.0.6/toqito/state_props/__init__.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     2628 2023-06-02 18:20:51.000000 toqito-1.0.6/toqito/state_props/concurrence.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     4070 2023-06-05 15:52:22.000000 toqito-1.0.6/toqito/state_props/entanglement_of_formation.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     5579 2023-06-24 22:22:46.000000 toqito-1.0.6/toqito/state_props/has_symmetric_extension.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     3277 2023-06-02 18:20:51.000000 toqito-1.0.6/toqito/state_props/in_separable_ball.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     1802 2023-06-02 18:20:51.000000 toqito-1.0.6/toqito/state_props/is_ensemble.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     1226 2023-06-02 18:20:51.000000 toqito-1.0.6/toqito/state_props/is_mixed.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     2445 2023-06-02 18:20:51.000000 toqito-1.0.6/toqito/state_props/is_mutually_orthogonal.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     3639 2023-06-02 18:20:51.000000 toqito-1.0.6/toqito/state_props/is_mutually_unbiased_basis.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     1326 2023-06-24 22:22:46.000000 toqito-1.0.6/toqito/state_props/is_npt.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     3243 2023-06-24 22:22:46.000000 toqito-1.0.6/toqito/state_props/is_ppt.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     4799 2023-06-24 22:22:46.000000 toqito-1.0.6/toqito/state_props/is_product.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     2705 2023-06-02 18:20:51.000000 toqito-1.0.6/toqito/state_props/is_pure.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     7576 2023-06-24 22:22:46.000000 toqito-1.0.6/toqito/state_props/is_separable.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     1724 2023-06-02 18:20:51.000000 toqito-1.0.6/toqito/state_props/l1_norm_coherence.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     2775 2023-06-24 22:22:46.000000 toqito-1.0.6/toqito/state_props/log_negativity.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     2836 2023-06-24 22:22:46.000000 toqito-1.0.6/toqito/state_props/negativity.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     1835 2023-06-02 18:20:51.000000 toqito-1.0.6/toqito/state_props/purity.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     4285 2023-06-02 18:20:51.000000 toqito-1.0.6/toqito/state_props/schmidt_rank.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     2342 2023-06-02 18:20:51.000000 toqito-1.0.6/toqito/state_props/sk_vec_norm.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     3088 2023-06-02 18:20:51.000000 toqito-1.0.6/toqito/state_props/von_neumann_entropy.py
+drwxr-xr-x   0 vrusso     (502) staff       (20)        0 2023-07-08 08:38:24.046603 toqito-1.0.6/toqito/states/
+-rw-r--r--   0 vrusso     (502) staff       (20)      732 2023-06-02 18:20:51.000000 toqito-1.0.6/toqito/states/__init__.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     1471 2023-06-02 18:20:51.000000 toqito-1.0.6/toqito/states/basis.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     1902 2023-06-02 18:20:51.000000 toqito-1.0.6/toqito/states/bell.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     2384 2023-06-02 18:20:51.000000 toqito-1.0.6/toqito/states/brauer.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     1734 2023-06-02 18:20:51.000000 toqito-1.0.6/toqito/states/breuer.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     3157 2023-06-02 18:20:51.000000 toqito-1.0.6/toqito/states/chessboard.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     3547 2023-06-02 18:20:51.000000 toqito-1.0.6/toqito/states/domino.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     3631 2023-06-02 18:20:51.000000 toqito-1.0.6/toqito/states/gen_bell.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     3119 2023-06-02 18:20:51.000000 toqito-1.0.6/toqito/states/ghz.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     2507 2023-06-02 18:20:51.000000 toqito-1.0.6/toqito/states/gisin.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     6942 2023-06-02 18:20:51.000000 toqito-1.0.6/toqito/states/horodecki.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     2568 2023-06-02 18:20:51.000000 toqito-1.0.6/toqito/states/isotropic.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     1958 2023-06-02 18:20:51.000000 toqito-1.0.6/toqito/states/max_entangled.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     2114 2023-06-02 18:20:51.000000 toqito-1.0.6/toqito/states/max_mixed.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     2918 2023-06-02 18:20:51.000000 toqito-1.0.6/toqito/states/singlet.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     2479 2023-06-02 18:20:51.000000 toqito-1.0.6/toqito/states/tile.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     2599 2023-06-02 18:20:51.000000 toqito-1.0.6/toqito/states/w_state.py
+-rw-r--r--   0 vrusso     (502) staff       (20)     5740 2023-06-02 18:20:51.000000 toqito-1.0.6/toqito/states/werner.py
+drwxr-xr-x   0 vrusso     (502) staff       (20)        0 2023-07-08 08:38:23.979773 toqito-1.0.6/toqito.egg-info/
+-rw-r--r--   0 vrusso     (502) staff       (20)     4817 2023-07-08 08:38:23.000000 toqito-1.0.6/toqito.egg-info/PKG-INFO
+-rw-r--r--   0 vrusso     (502) staff       (20)    12618 2023-07-08 08:38:23.000000 toqito-1.0.6/toqito.egg-info/SOURCES.txt
+-rw-r--r--   0 vrusso     (502) staff       (20)        1 2023-07-08 08:38:23.000000 toqito-1.0.6/toqito.egg-info/dependency_links.txt
+-rw-r--r--   0 vrusso     (502) staff       (20)       41 2023-07-08 08:38:23.000000 toqito-1.0.6/toqito.egg-info/requires.txt
+-rw-r--r--   0 vrusso     (502) staff       (20)       13 2023-07-08 08:38:23.000000 toqito-1.0.6/toqito.egg-info/top_level.txt
```

### Comparing `toqito-1.0.5/LICENSE` & `toqito-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/PKG-INFO` & `toqito-1.0.6/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: toqito
-Version: 1.0.5
-Summary: Python toolkit for quantum information theory
-Home-page: https://github.com/vprusso/toqito
-Author: Vincent Russo
-Author-email: vincentrusso1@gmail.com
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Scientific/Engineering :: Physics
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # ![logo](./docs/figures/logo.svg "logo")
 
 (Theory of Quantum Information Toolkit)
 
 The `toqito` package is an open source Python library for studying various
 objects in quantum information, namely, states, channels, and measurements.
 
@@ -29,18 +12,19 @@
 `toqito` aims to fill the needs of quantum information researchers who want
 numerical and computational tools for manipulating quantum states,
 measurements, and channels. It can also be used as a tool to enhance the
 experience of students and instructors in classes pertaining to quantum
 information.
 
 
-[![build status](http://img.shields.io/travis/vprusso/toqito.svg?style=plastic)](https://travis-ci.org/vprusso/toqito)
+[![build status](https://github.com/vprusso/toqito/actions/workflows/build-test-actions.yml/badge.svg?style=plastic)](https://github.com/vprusso/toqito/actions/workflows/build-test-actions.yml/badge.svg)
 [![doc status](https://readthedocs.org/projects/toqito/badge/?version=latest&style=plastic)](https://toqito.readthedocs.io/en/latest/)
 [![codecov](https://codecov.io/gh/vprusso/toqito/branch/master/graph/badge.svg?style=plastic)](https://codecov.io/gh/vprusso/toqito)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.4743211.svg)](https://doi.org/10.5281/zenodo.4743211)
+[![Downloads](https://static.pepy.tech/personalized-badge/toqito?style=platic&period=total&units=none&left_color=black&right_color=brightgreen&left_text=Downloads)](https://pepy.tech/project/toqito)
 [![Unitary Fund](https://img.shields.io/badge/Supported%20By-UNITARY%20FUND-brightgreen.svg?style=plastic)](http://unitary.fund)
 
 ## Installing
 
 The preferred way to install the `toqito` package is via `pip`:
 
 ```
@@ -95,14 +79,22 @@
    howpublished = {\url{https://github.com/vprusso/toqito}},
    month        = May,
    year         = 2021,
    doi          = {10.5281/zenodo.4743211}
  }
 ```
 
+The `toqito` project has been used in the following works:
+ 
+- Philip, Aby, Soorya Rethinasamy, Vincent Russo, and Mark M. Wilde. "Quantum Steering Algorithm for Estimating Fidelity of Separability." arXiv preprint [arXiv:2303.07911](https://arxiv.org/abs/2303.07911) (2023).
+
+- Miszczak, Jarosław Adam. "Symbolic quantum programming for supporting applications of quantum computing technologies." arXiv preprint [arXiv:2302.09401](https://arxiv.org/abs/2302.09401) (2023).
+
+- Casalé, Balthazar, Giuseppe Di Molfetta, Sandrine Anthoine, and Hachem Kadri. "Large-Scale Quantum Separability Through a Reproducible Machine Learning Lens." arXiv preprint [arXiv:2306.09444](https://arxiv.org/abs/2306.09444) (2023).
+
 ## Contributing
 
 All contributions, bug reports, bug fixes, documentation improvements,
 enhancements, and ideas are welcome.
 
 A detailed overview on how to contribute can be found in the
 [contributing guide](https://github.com/vprusso/toqito/blob/master/.github/CONTRIBUTING.md).
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `toqito-1.0.5/pyproject.toml` & `toqito-1.0.6/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     | dist
   )/
 )
 '''
 
 [tool.poetry]
 name = "toqito"
-version = "1.0.5"
+version = "1.0.6"
 description = "Python tools for the study of quantum information."
 authors = [
     "Vincent Russo <vincentrusso1@gmail.com>"
 ]
 maintainers = [
     "Vincent Russo <vincentrusso1@gmail.com>"
 ]
@@ -53,18 +53,18 @@
 isort = "^5.9.3"
 myst-parser = "*"
 pep8 = "^1.7"
 pydocstyle = "^6.1.1"
 pylint = "^2.4"
 pytest = "*"
 pytest-cov = "*"
-mypy = "^0.750.0"
+mypy = "^1.3.0"
 coverage = "^4.5"
 coveralls = "^1.9"
-setuptools = "<=57.5.0"
-sphinx = "3.1.2"
+setuptools = ">65.5.1"
+sphinx = "6.2.1"
 sphinx_rtd_theme = "*"
 
 
 [build-system]
-requires = ["poetry>=0.12"]
+requires = ["setuptools","poetry>=0.12"]
 build-backend = "poetry.masonry.api"
```

### Comparing `toqito-1.0.5/setup.py` & `toqito-1.0.6/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 requirements = ["cvx", "cvxpy", "numpy", "picos", "scipy", "scikit-image"]
 
 setuptools.setup(
     name="toqito",
-    version="1.0.5",
+    version="1.0.6",
     author="Vincent Russo",
     author_email="vincentrusso1@gmail.com",
     description="Python toolkit for quantum information theory",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/vprusso/toqito",
     packages=setuptools.find_packages(),
```

### Comparing `toqito-1.0.5/tests/test_channel_metrics/test_channel_fidelity.py` & `toqito-1.0.6/tests/test_channel_metrics/test_channel_fidelity.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/tests/test_channel_metrics/test_diamond_norm.py` & `toqito-1.0.6/tests/test_channel_metrics/test_diamond_norm.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/tests/test_channel_ops/test_apply_channel.py` & `toqito-1.0.6/tests/test_channels/test_depolarizing.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,56 +1,37 @@
-"""Tests for apply_channel."""
+"""Test depolarizing."""
 import numpy as np
 
+from toqito.channels import depolarizing
 from toqito.channel_ops import apply_channel
-from toqito.perms import swap_operator
 
 
-def test_apply_channel_choi():
-    """
-    The swap operator is the Choi matrix of the transpose map.
+def test_depolarizing_complete_depolarizing():
+    """Maps every density matrix to the maximally-mixed state."""
+    test_input_mat = np.array(
+        [[1 / 2, 0, 0, 1 / 2], [0, 0, 0, 0], [0, 0, 0, 0], [1 / 2, 0, 0, 1 / 2]]
+    )
 
-    The following test is a (non-ideal, but illustrative) way of computing
-    the transpose of a matrix.
-    """
-    test_input_mat = np.array([[1, 4, 7], [2, 5, 8], [3, 6, 9]])
+    expected_res = 1 / 4 * np.identity(4)
 
-    expected_res = np.array([[1, 2, 3], [4, 5, 6], [7, 8, 9]])
+    res = apply_channel(test_input_mat, depolarizing(4))
 
-    res = apply_channel(test_input_mat, swap_operator(3))
-
-    bool_mat = np.isclose(res, expected_res)
+    bool_mat = np.isclose(expected_res, res)
     np.testing.assert_equal(np.all(bool_mat), True)
 
 
-def test_apply_channel_kraus():
-    """
-    Apply Kraus map.
-
-    The following test computes PHI(X) where X = [[1, 2], [3, 4]] and
-    where PHI is the superoperator defined by:
-    Phi(X) = [[1,5],[1,0],[0,2]] X [[0,1][2,3][4,5]].conj().T -
-    [[1,0],[0,0],[0,1]] X [[0,0][1,1],[0,0]].conj().T
-    """
-    test_input_mat = np.array([[1, 2], [3, 4]])
-
-    kraus_1 = np.array([[1, 5], [1, 0], [0, 2]])
-    kraus_2 = np.array([[0, 1], [2, 3], [4, 5]])
-    kraus_3 = np.array([[-1, 0], [0, 0], [0, -1]])
-    kraus_4 = np.array([[0, 0], [1, 1], [0, 0]])
-
-    expected_res = np.array([[22, 95, 174], [2, 8, 14], [8, 29, 64]])
-
-    res = apply_channel(test_input_mat, [[kraus_1, kraus_2], [kraus_3, kraus_4]])
+def test_depolarizing_partially_depolarizing():
+    """The partially depolarizing channel for `p = 0.5`."""
+    test_input_mat = np.array([[1, 2, 3, 4], [5, 6, 7, 8], [9, 10, 11, 12], [13, 14, 15, 16]])
+    param_p = 0.5
+
+    res = apply_channel(test_input_mat, depolarizing(4, param_p))
+    expected_res = (1 - param_p) * np.trace(test_input_mat) * np.identity(
+        4
+    ) / 4 + param_p * test_input_mat
 
-    bool_mat = np.isclose(res, expected_res)
+    bool_mat = np.isclose(expected_res, res)
     np.testing.assert_equal(np.all(bool_mat), True)
 
 
-def test_apply_channel_invalid_input():
-    """Invalid input for apply map."""
-    with np.testing.assert_raises(ValueError):
-        apply_channel(np.array([[1, 2], [3, 4]]), 2)
-
-
 if __name__ == "__main__":
     np.testing.run_module_suite()
```

### Comparing `toqito-1.0.5/tests/test_channel_ops/test_dual_channel.py` & `toqito-1.0.6/tests/test_channel_ops/test_dual_channel.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Tests for dual_channel."""
 import numpy as np
 
 from toqito.channel_ops import dual_channel
 from toqito.channels import choi
+from toqito.perms import swap_operator
 
 
 def test_dual_channel_kraus1():
     """Test dual_channel on a channel represented as Kraus operators (1d list, CP map)."""
     kraus_1 = np.array([[1, 0, 1j, 0]])
     kraus_2 = np.array([[0, 1, 0, 1j]])
 
@@ -69,18 +70,30 @@
     res = dual_channel(j, [3, 2])
 
     bool_mat = np.isclose(res, expected_res)
     np.testing.assert_equal(np.all(bool_mat), True)
 
 
 def test_dual_channel_nonsquare_matrix():
-    """If the channel is represented as a Choi matrix, it must be square."""
-    with np.testing.assert_raises(ValueError):
-        j = np.array([[1, 2, 3, 4], [4, 3, 2, 1]])
-        dual_channel(j)
+    """Dual of a channel that transposes 3x2 matrices."""
+    choi = swap_operator([2, 3])
+    choi_dual = dual_channel(choi, dims=[[3, 2], [2, 3]])
+    expected_choi_dual = np.array(
+        [
+            [1, 0, 0, 0, 0, 0],
+            [0, 0, 1, 0, 0, 0],
+            [0, 0, 0, 0, 1, 0],
+            [0, 1, 0, 0, 0, 0],
+            [0, 0, 0, 1, 0, 0],
+            [0, 0, 0, 0, 0, 1],
+        ]
+    )
+
+    bool_mat = np.isclose(choi_dual, expected_choi_dual)
+    np.testing.assert_equal(np.all(bool_mat), True)
 
 
 def test_dual_channel_not_matrix():
     """If the channel is represented as an array, it must be two-dimensional (a matrix)."""
     with np.testing.assert_raises(ValueError):
         j = np.array([1, 2, 3, 4])
         dual_channel(j)
```

### Comparing `toqito-1.0.5/tests/test_channel_ops/test_partial_channel.py` & `toqito-1.0.6/tests/test_channel_ops/test_partial_channel.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 """Tests for partial_channel."""
 import numpy as np
+import pytest
 
 from toqito.channel_ops import partial_channel
 from toqito.channels import depolarizing
+from toqito.matrices import pauli
 
 
 def test_partial_channel_depolarizing_first_system():
     """
     Perform the partial map using the depolarizing channel as the Choi
     matrix on first system.
     """
@@ -111,14 +113,42 @@
 
     expected_res = np.array(
         [
             [3.5, 0.0, 5.5, 0.0],
             [0.0, 3.5, 0.0, 5.5],
             [11.5, 0.0, 13.5, 0.0],
             [0.0, 11.5, 0.0, 13.5],
+        ]
+    )
+
+    bool_mat = np.isclose(expected_res, res)
+    np.testing.assert_equal(np.all(bool_mat), True)
+
+
+@pytest.mark.parametrize("nested", [1, 2, 3])
+def test_partial_channel_cpt_kraus(nested):
+    """
+    Perform the partial map using the Kraus representation of
+    the depolarizing channel.
+    """
+    rho = np.array([[1, 2, 3, 4], [5, 6, 7, 8], [9, 10, 11, 12], [13, 14, 15, 16]])
+    kraus = [0.5 * pauli(ind) for ind in range(4)]
+    if nested == 2:
+        kraus = [kraus]
+    elif nested == 3:
+        kraus = [[mat] for mat in kraus]
+
+    res = partial_channel(rho, kraus)
+
+    expected_res = np.array(
+        [
+            [3.5, 0.0, 5.5, 0.0],
+            [0.0, 3.5, 0.0, 5.5],
+            [11.5, 0.0, 13.5, 0.0],
+            [0.0, 11.5, 0.0, 13.5],
         ]
     )
 
     bool_mat = np.isclose(expected_res, res)
     np.testing.assert_equal(np.all(bool_mat), True)
```

### Comparing `toqito-1.0.5/tests/test_channel_props/test_choi_rank.py` & `toqito-1.0.6/tests/test_channel_props/test_choi_rank.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/tests/test_channel_props/test_is_completely_positive.py` & `toqito-1.0.6/tests/test_channel_props/test_is_completely_positive.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/tests/test_channel_props/test_is_herm_preserving.py` & `toqito-1.0.6/tests/test_channel_props/test_is_herm_preserving.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/tests/test_channel_props/test_is_positive.py` & `toqito-1.0.6/tests/test_channel_props/test_is_positive.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/tests/test_channel_props/test_is_quantum_channel.py` & `toqito-1.0.6/tests/test_channel_props/test_is_quantum_channel.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/tests/test_channel_props/test_is_trace_preserving.py` & `toqito-1.0.6/tests/test_channel_props/test_is_trace_preserving.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/tests/test_channels/test_choi.py` & `toqito-1.0.6/tests/test_channels/test_choi.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/tests/test_channels/test_dephasing.py` & `toqito-1.0.6/tests/test_channels/test_dephasing.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,18 +16,18 @@
     bool_mat = np.isclose(expected_res, res)
     np.testing.assert_equal(np.all(bool_mat), True)
 
 
 def test_dephasing_partially_dephasing():
     """The partially dephasing channel for `p = 0.5`."""
     test_input_mat = np.array([[1, 2, 3, 4], [5, 6, 7, 8], [9, 10, 11, 12], [13, 14, 15, 16]])
+    param_p = 0.5
 
-    expected_res = np.array([[17.5, 0, 0, 0], [0, 20, 0, 0], [0, 0, 22.5, 0], [0, 0, 0, 25]])
-
-    res = apply_channel(test_input_mat, dephasing(4, 0.5))
+    res = apply_channel(test_input_mat, dephasing(4, param_p))
+    expected_res = (1 - param_p) * np.diag(np.diag(test_input_mat)) + param_p * test_input_mat
 
     bool_mat = np.isclose(expected_res, res)
     np.testing.assert_equal(np.all(bool_mat), True)
 
 
 if __name__ == "__main__":
     np.testing.run_module_suite()
```

### Comparing `toqito-1.0.5/tests/test_channels/test_partial_trace.py` & `toqito-1.0.6/tests/test_channels/test_partial_trace.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,27 @@
     By specifying the `sys` argument, you can perform the partial trace
     the first subsystem instead:
     """
     test_input_mat = np.arange(1, 17).reshape(4, 4)
 
     expected_res = np.array([[12, 14], [20, 22]])
 
-    res = partial_trace(test_input_mat, 1)
+    res = partial_trace(test_input_mat, [0])
+
+    bool_mat = np.isclose(expected_res, res)
+    np.testing.assert_equal(np.all(bool_mat), True)
+
+
+def test_partial_trace_sys_int():
+    """Supply `sys` argument as int."""
+    test_input_mat = np.arange(1, 17).reshape(4, 4)
+
+    expected_res = np.array([[12, 14], [20, 22]])
+
+    res = partial_trace(test_input_mat, 0)
 
     bool_mat = np.isclose(expected_res, res)
     np.testing.assert_equal(np.all(bool_mat), True)
 
 
 def test_partial_trace_sys_int_dim_int():
     """
@@ -47,15 +59,15 @@
     By default, the partial_transpose function takes the trace over
     the second subsystem.
     """
     test_input_mat = np.arange(1, 17).reshape(4, 4)
 
     expected_res = np.array([[7, 11], [23, 27]])
 
-    res = partial_trace(test_input_mat, 2, 2)
+    res = partial_trace(test_input_mat, [1])
 
     bool_mat = np.isclose(expected_res, res)
     np.testing.assert_equal(np.all(bool_mat), True)
 
 
 def test_partial_trace_sys_int_dim_int_2():
     """
@@ -64,26 +76,26 @@
     By default, the partial_transpose function takes the trace over
     the second subsystem.
     """
     test_input_mat = np.arange(1, 17).reshape(4, 4)
 
     expected_res = 34
 
-    res = partial_trace(test_input_mat, 2, 1)
+    res = partial_trace(test_input_mat, [1], [1, 4])
 
     bool_mat = np.isclose(expected_res, res)
     np.testing.assert_equal(np.all(bool_mat), True)
 
 
 def test_partial_trace_4_by_4():
     """Test for 4-by-4 matrix."""
     test_input_mat = np.arange(1, 17).reshape(4, 4)
 
-    pt_1 = partial_trace(test_input_mat, [1], [2, 2])
-    pt_2 = partial_trace(test_input_mat, [2], [2, 2])
+    pt_1 = partial_trace(test_input_mat, [0], [2, 2])
+    pt_2 = partial_trace(test_input_mat, [1], [2, 2])
 
     expected_pt_1 = np.array([[12, 14], [20, 22]])
     bool_mat = np.isclose(expected_pt_1, pt_1)
     np.testing.assert_equal(np.all(bool_mat), True)
 
     expected_pt_2 = np.array([[7, 11], [23, 27]])
     bool_mat = np.isclose(expected_pt_2, pt_2)
@@ -91,131 +103,131 @@
 
 
 def test_partial_trace_8_by_8():
     """Test for 8-by-8 matrix."""
     test_input_mat = np.arange(1, 65).reshape(8, 8)
 
     # Trace out first subsystem:
-    pt_1 = partial_trace(test_input_mat, [1], [2, 2, 2])
+    pt_1 = partial_trace(test_input_mat, [0], [2, 2, 2])
     expected_pt_1 = np.array(
         [[38, 40, 42, 44], [54, 56, 58, 60], [70, 72, 74, 76], [86, 88, 90, 92]]
     )
     bool_mat = np.isclose(expected_pt_1, pt_1)
     np.testing.assert_equal(np.all(bool_mat), True)
 
     # Trace out second subsystem:
-    pt_2 = partial_trace(test_input_mat, [2], [2, 2, 2])
+    pt_2 = partial_trace(test_input_mat, [1], [2, 2, 2])
     expected_pt_2 = np.array(
         [[20, 22, 28, 30], [36, 38, 44, 46], [84, 86, 92, 94], [100, 102, 108, 110]]
     )
     bool_mat = np.isclose(expected_pt_2, pt_2)
     np.testing.assert_equal(np.all(bool_mat), True)
 
     # Trace out third subsystem:
-    pt_3 = partial_trace(test_input_mat, [3], [2, 2, 2])
+    pt_3 = partial_trace(test_input_mat, [2], [2, 2, 2])
     expected_pt_3 = np.array(
         [[11, 15, 19, 23], [43, 47, 51, 55], [75, 79, 83, 87], [107, 111, 115, 119]]
     )
     bool_mat = np.isclose(expected_pt_3, pt_3)
     np.testing.assert_equal(np.all(bool_mat), True)
 
     # Trace out first and second subsystem:
-    pt_1_2 = partial_trace(test_input_mat, [1, 2], [2, 2, 2])
+    pt_1_2 = partial_trace(test_input_mat, [0, 1], [2, 2, 2])
     expected_pt_1_2 = np.array([[112, 116], [144, 148]])
     bool_mat = np.isclose(expected_pt_1_2, pt_1_2)
     np.testing.assert_equal(np.all(bool_mat), True)
 
     # Trace out first and third subsystem:
-    pt_1_3 = partial_trace(test_input_mat, [1, 3], [2, 2, 2])
+    pt_1_3 = partial_trace(test_input_mat, [0, 2], [2, 2, 2])
     expected_pt_1_3 = np.array([[94, 102], [158, 166]])
     bool_mat = np.isclose(expected_pt_1_3, pt_1_3)
     np.testing.assert_equal(np.all(bool_mat), True)
 
     # Trace out second and third subsystem:
-    pt_2_3 = partial_trace(test_input_mat, [2, 3], [2, 2, 2])
+    pt_2_3 = partial_trace(test_input_mat, [1, 2], [2, 2, 2])
     expected_pt_2_3 = np.array([[58, 74], [186, 202]])
     bool_mat = np.isclose(expected_pt_2_3, pt_2_3)
     np.testing.assert_equal(np.all(bool_mat), True)
 
 
 def test_partial_trace_6_by_6_subsystems_2_3():
     """Test for 6-by-6 matrix for subsystems 2 x 3"""
     test_input_mat = np.arange(1, 37).reshape(6, 6)
 
     # Trace out first subsystem:
-    pt_1 = partial_trace(test_input_mat, [1], [2, 3])
+    pt_1 = partial_trace(test_input_mat, [0], [2, 3])
     expected_pt_1 = np.array([[23, 25, 27], [35, 37, 39], [47, 49, 51]])
     bool_mat = np.isclose(expected_pt_1, pt_1)
     np.testing.assert_equal(np.all(bool_mat), True)
 
     # Trace out second subsystem:
-    pt_2 = partial_trace(test_input_mat, [2], [2, 3])
+    pt_2 = partial_trace(test_input_mat, [1], [2, 3])
     expected_pt_2 = np.array([[24, 33], [78, 87]])
     bool_mat = np.isclose(expected_pt_2, pt_2)
     np.testing.assert_equal(np.all(bool_mat), True)
 
     # Trace out first and second subsystem:
-    pt_1_2 = partial_trace(test_input_mat, [1, 2], [2, 3])
+    pt_1_2 = partial_trace(test_input_mat, [0, 1], [2, 3])
     expected_pt_1_2 = np.array([[111]])
     bool_mat = np.isclose(expected_pt_1_2, pt_1_2)
     np.testing.assert_equal(np.all(bool_mat), True)
 
 
 def test_partial_trace_6_by_6_subsystems_3_2():
     """Test for 6-by-6 matrix for subsystems 3 x 2"""
     test_input_mat = np.arange(1, 37).reshape(6, 6)
 
     # Trace out first subsystem:
-    pt_1 = partial_trace(test_input_mat, [1], [3, 2])
+    pt_1 = partial_trace(test_input_mat, [0], [3, 2])
     expected_pt_1 = np.array([[45, 48], [63, 66]])
     bool_mat = np.isclose(expected_pt_1, pt_1)
     np.testing.assert_equal(np.all(bool_mat), True)
 
     # Trace out second subsystem:
-    pt_2 = partial_trace(test_input_mat, [2], [3, 2])
+    pt_2 = partial_trace(test_input_mat, [1], [3, 2])
     expected_pt_2 = np.array([[9, 13, 17], [33, 37, 41], [57, 61, 65]])
     bool_mat = np.isclose(expected_pt_2, pt_2)
     np.testing.assert_equal(np.all(bool_mat), True)
 
     # Trace out first and second subsystem:
-    pt_1_2 = partial_trace(test_input_mat, [1, 2], [3, 2])
+    pt_1_2 = partial_trace(test_input_mat, [0, 1], [3, 2])
     expected_pt_1_2 = np.array([[111]])
     bool_mat = np.isclose(expected_pt_1_2, pt_1_2)
     np.testing.assert_equal(np.all(bool_mat), True)
 
 
 def test_partial_trace_9_by_9_subsystems_3_3():
     """Test for 9-by-9 matrix for subsystems 3 x 3"""
     test_input_mat = np.arange(1, 82).reshape(9, 9)
 
     # Partial trace on first subsystem:
-    pt_1 = partial_trace(test_input_mat, [1], [3, 3])
+    pt_1 = partial_trace(test_input_mat, [0], [3, 3])
     expected_pt_1 = np.array([[93, 96, 99], [120, 123, 126], [147, 150, 153]])
     bool_mat = np.isclose(expected_pt_1, pt_1)
     np.testing.assert_equal(np.all(bool_mat), True)
 
     # Partial trace on second subsystem:
-    pt_2 = partial_trace(test_input_mat, [2], [3, 3])
+    pt_2 = partial_trace(test_input_mat, [1], [3, 3])
     expected_pt_2 = np.array([[33, 42, 51], [114, 123, 132], [195, 204, 213]])
     bool_mat = np.isclose(expected_pt_2, pt_2)
     np.testing.assert_equal(np.all(bool_mat), True)
 
     # Partial trace on first and second subsystems:
-    pt_1_2 = partial_trace(test_input_mat, [1, 2], [3, 3])
+    pt_1_2 = partial_trace(test_input_mat, [0, 1], [3, 3])
     expected_pt_1_2 = np.array([[369]])
     bool_mat = np.isclose(expected_pt_1_2, pt_1_2)
     np.testing.assert_equal(np.all(bool_mat), True)
 
 
 def test_partial_trace_16_by_16_subsystems_2_2_2_2():
     """Test for 16-by-16 matrix for subsystems (2 x 2) x (2 x 2)."""
     test_input_mat = np.arange(1, 257).reshape(16, 16)
 
     # Trace out first subsystem:
-    pt_1 = partial_trace(test_input_mat, [1], [2, 2, 2, 2])
+    pt_1 = partial_trace(test_input_mat, [0], [2, 2, 2, 2])
     expected_pt_1 = np.array(
         [
             [138, 140, 142, 144, 146, 148, 150, 152],
             [170, 172, 174, 176, 178, 180, 182, 184],
             [202, 204, 206, 208, 210, 212, 214, 216],
             [234, 236, 238, 240, 242, 244, 246, 248],
             [266, 268, 270, 272, 274, 276, 278, 280],
@@ -224,15 +236,15 @@
             [362, 364, 366, 368, 370, 372, 374, 376],
         ]
     )
     bool_mat = np.isclose(expected_pt_1, pt_1)
     np.testing.assert_equal(np.all(bool_mat), True)
 
     # Trace out second subsystem:
-    pt_2 = partial_trace(test_input_mat, [2], [2, 2, 2, 2])
+    pt_2 = partial_trace(test_input_mat, [1], [2, 2, 2, 2])
     expected_pt_2 = np.array(
         [
             [70, 72, 74, 76, 86, 88, 90, 92],
             [102, 104, 106, 108, 118, 120, 122, 124],
             [134, 136, 138, 140, 150, 152, 154, 156],
             [166, 168, 170, 172, 182, 184, 186, 188],
             [326, 328, 330, 332, 342, 344, 346, 348],
@@ -241,15 +253,15 @@
             [422, 424, 426, 428, 438, 440, 442, 444],
         ]
     )
     bool_mat = np.isclose(expected_pt_2, pt_2)
     np.testing.assert_equal(np.all(bool_mat), True)
 
     # Trace out third subsystem:
-    pt_3 = partial_trace(test_input_mat, [3], [2, 2, 2, 2])
+    pt_3 = partial_trace(test_input_mat, [2], [2, 2, 2, 2])
     expected_pt_3 = np.array(
         [
             [36, 38, 44, 46, 52, 54, 60, 62],
             [68, 70, 76, 78, 84, 86, 92, 94],
             [164, 166, 172, 174, 180, 182, 188, 190],
             [196, 198, 204, 206, 212, 214, 220, 222],
             [292, 294, 300, 302, 308, 310, 316, 318],
@@ -258,15 +270,15 @@
             [452, 454, 460, 462, 468, 470, 476, 478],
         ]
     )
     bool_mat = np.isclose(expected_pt_3, pt_3)
     np.testing.assert_equal(np.all(bool_mat), True)
 
     # Trace out fourth subsystem:
-    pt_4 = partial_trace(test_input_mat, [4], [2, 2, 2, 2])
+    pt_4 = partial_trace(test_input_mat, [3], [2, 2, 2, 2])
     expected_pt_4 = np.array(
         [
             [19, 23, 27, 31, 35, 39, 43, 47],
             [83, 87, 91, 95, 99, 103, 107, 111],
             [147, 151, 155, 159, 163, 167, 171, 175],
             [211, 215, 219, 223, 227, 231, 235, 239],
             [275, 279, 283, 287, 291, 295, 299, 303],
@@ -275,80 +287,80 @@
             [467, 471, 475, 479, 483, 487, 491, 495],
         ]
     )
     bool_mat = np.isclose(expected_pt_4, pt_4)
     np.testing.assert_equal(np.all(bool_mat), True)
 
     # Trace out first and second subsystem:
-    pt_1_2 = partial_trace(test_input_mat, [1, 2], [2, 2, 2, 2])
+    pt_1_2 = partial_trace(test_input_mat, [0, 1], [2, 2, 2, 2])
     expected_pt_1_2 = np.array(
         [
             [412, 416, 420, 424],
             [476, 480, 484, 488],
             [540, 544, 548, 552],
             [604, 608, 612, 616],
         ]
     )
 
     bool_mat = np.isclose(expected_pt_1_2, pt_1_2)
     np.testing.assert_equal(np.all(bool_mat), True)
 
     # Trace out first and third subsystem:
-    pt_1_3 = partial_trace(test_input_mat, [1, 3], [2, 2, 2, 2])
+    pt_1_3 = partial_trace(test_input_mat, [0, 2], [2, 2, 2, 2])
     expected_pt_1_3 = np.array(
         [
             [344, 348, 360, 364],
             [408, 412, 424, 428],
             [600, 604, 616, 620],
             [664, 668, 680, 684],
         ]
     )
     bool_mat = np.isclose(expected_pt_1_3, pt_1_3)
     np.testing.assert_equal(np.all(bool_mat), True)
 
     # Trace out first and fourth subsystem:
-    pt_1_4 = partial_trace(test_input_mat, [1, 4], [2, 2, 2, 2])
+    pt_1_4 = partial_trace(test_input_mat, [0, 3], [2, 2, 2, 2])
 
     expected_pt_1_4 = np.array(
         [[310, 318, 326, 334], [438, 446, 454, 462], [566, 574, 582, 590], [694, 702, 710, 718]]
     )
     bool_mat = np.isclose(expected_pt_1_4, pt_1_4)
     np.testing.assert_equal(np.all(bool_mat), True)
 
     # Trace out second and third subsystem:
-    pt_2_3 = partial_trace(test_input_mat, [2, 3], [2, 2, 2, 2])
+    pt_2_3 = partial_trace(test_input_mat, [1, 2], [2, 2, 2, 2])
     expected_pt_2_3 = np.array(
         [[208, 212, 240, 244], [272, 276, 304, 308], [720, 724, 752, 756], [784, 788, 816, 820]]
     )
     bool_mat = np.isclose(expected_pt_2_3, pt_2_3)
     np.testing.assert_equal(np.all(bool_mat), True)
 
     # Trace out second and fourth subsystem:
-    pt_2_4 = partial_trace(test_input_mat, [2, 4], [2, 2, 2, 2])
+    pt_2_4 = partial_trace(test_input_mat, [1, 3], [2, 2, 2, 2])
     expected_pt_2_4 = np.array(
         [[174, 182, 206, 214], [302, 310, 334, 342], [686, 694, 718, 726], [814, 822, 846, 854]]
     )
     bool_mat = np.isclose(expected_pt_2_4, pt_2_4)
     np.testing.assert_equal(np.all(bool_mat), True)
 
     # Trace out third and fourth subsystem:
-    pt_3_4 = partial_trace(test_input_mat, [3, 4], [2, 2, 2, 2])
+    pt_3_4 = partial_trace(test_input_mat, [2, 3], [2, 2, 2, 2])
     expected_pt_3_4 = np.array(
         [[106, 122, 138, 154], [362, 378, 394, 410], [618, 634, 650, 666], [874, 890, 906, 922]]
     )
     bool_mat = np.isclose(expected_pt_3_4, pt_3_4)
     np.testing.assert_equal(np.all(bool_mat), True)
 
 
 def test_partial_trace_16_by_16_subsystems_2_2_4():
     """Test for 16-by-16 matrix for subsystems 2 x 4."""
     test_input_mat = np.arange(1, 257).reshape(16, 16)
 
     # Trace out first subsystem:
-    pt_1 = partial_trace(test_input_mat, [1], [2, 2, 4])
+    pt_1 = partial_trace(test_input_mat, [0], [2, 2, 4])
     expected_pt_1 = np.array(
         [
             [138, 140, 142, 144, 146, 148, 150, 152],
             [170, 172, 174, 176, 178, 180, 182, 184],
             [202, 204, 206, 208, 210, 212, 214, 216],
             [234, 236, 238, 240, 242, 244, 246, 248],
             [266, 268, 270, 272, 274, 276, 278, 280],
@@ -357,15 +369,15 @@
             [362, 364, 366, 368, 370, 372, 374, 376],
         ]
     )
     bool_mat = np.isclose(expected_pt_1, pt_1)
     np.testing.assert_equal(np.all(bool_mat), True)
 
     # Trace out second subsystem:
-    pt_2 = partial_trace(test_input_mat, [2], [2, 2, 4])
+    pt_2 = partial_trace(test_input_mat, [1], [2, 2, 4])
     expected_pt_2 = np.array(
         [
             [70, 72, 74, 76, 86, 88, 90, 92],
             [102, 104, 106, 108, 118, 120, 122, 124],
             [134, 136, 138, 140, 150, 152, 154, 156],
             [166, 168, 170, 172, 182, 184, 186, 188],
             [326, 328, 330, 332, 342, 344, 346, 348],
@@ -374,66 +386,66 @@
             [422, 424, 426, 428, 438, 440, 442, 444],
         ]
     )
     bool_mat = np.isclose(expected_pt_2, pt_2)
     np.testing.assert_equal(np.all(bool_mat), True)
 
     # Trace out third subsystem:
-    pt_3 = partial_trace(test_input_mat, [3], [2, 2, 4])
+    pt_3 = partial_trace(test_input_mat, [2], [2, 2, 4])
     expected_pt_3 = np.array(
         [[106, 122, 138, 154], [362, 378, 394, 410], [618, 634, 650, 666], [874, 890, 906, 922]]
     )
     bool_mat = np.isclose(expected_pt_3, pt_3)
     np.testing.assert_equal(np.all(bool_mat), True)
 
     # Trace out first and second subsystem:
-    pt_1_2 = partial_trace(test_input_mat, [1, 2], [2, 2, 4])
+    pt_1_2 = partial_trace(test_input_mat, [0, 1], [2, 2, 4])
     expected_pt_1_2 = np.array(
         [
             [412, 416, 420, 424],
             [476, 480, 484, 488],
             [540, 544, 548, 552],
             [604, 608, 612, 616],
         ]
     )
     bool_mat = np.isclose(expected_pt_1_2, pt_1_2)
     np.testing.assert_equal(np.all(bool_mat), True)
 
     # Trace out first and third subsystem:
-    pt_1_3 = partial_trace(test_input_mat, [1, 3], [2, 2, 4])
+    pt_1_3 = partial_trace(test_input_mat, [0, 2], [2, 2, 4])
     expected_pt_1_3 = np.array([[756, 788], [1268, 1300]])
     bool_mat = np.isclose(expected_pt_1_3, pt_1_3)
     np.testing.assert_equal(np.all(bool_mat), True)
 
     # Trace out second and third subsystem:
-    pt_2_3 = partial_trace(test_input_mat, [2, 3], [2, 2, 4])
+    pt_2_3 = partial_trace(test_input_mat, [1, 2], [2, 2, 4])
     expected_pt_2_3 = np.array([[484, 548], [1508, 1572]])
     bool_mat = np.isclose(expected_pt_2_3, pt_2_3)
     np.testing.assert_equal(np.all(bool_mat), True)
 
 
 def test_partial_trace_16_by_16_subsystems_4_2_2():
     """Test for 16-by-16 matrix for subsystems 4 x 2."""
     test_input_mat = np.arange(1, 257).reshape(16, 16)
 
     # Trace out the first subsystem:
-    pt_1 = partial_trace(test_input_mat, [1], [4, 2, 2])
+    pt_1 = partial_trace(test_input_mat, [0], [4, 2, 2])
     expected_pt_1 = np.array(
         [
             [412, 416, 420, 424],
             [476, 480, 484, 488],
             [540, 544, 548, 552],
             [604, 608, 612, 616],
         ]
     )
     bool_mat = np.isclose(expected_pt_1, pt_1)
     np.testing.assert_equal(np.all(bool_mat), True)
 
     # Trace out the second subsystem:
-    pt_2 = partial_trace(test_input_mat, [2], [4, 2, 2])
+    pt_2 = partial_trace(test_input_mat, [1], [4, 2, 2])
     expected_pt_2 = np.array(
         [
             [36, 38, 44, 46, 52, 54, 60, 62],
             [68, 70, 76, 78, 84, 86, 92, 94],
             [164, 166, 172, 174, 180, 182, 188, 190],
             [196, 198, 204, 206, 212, 214, 220, 222],
             [292, 294, 300, 302, 308, 310, 316, 318],
@@ -442,15 +454,15 @@
             [452, 454, 460, 462, 468, 470, 476, 478],
         ]
     )
     bool_mat = np.isclose(expected_pt_2, pt_2)
     np.testing.assert_equal(np.all(bool_mat), True)
 
     # Trace out the third subsystem:
-    pt_3 = partial_trace(test_input_mat, [3], [4, 2, 2])
+    pt_3 = partial_trace(test_input_mat, [2], [4, 2, 2])
     expected_pt_3 = np.array(
         [
             [19, 23, 27, 31, 35, 39, 43, 47],
             [83, 87, 91, 95, 99, 103, 107, 111],
             [147, 151, 155, 159, 163, 167, 171, 175],
             [211, 215, 219, 223, 227, 231, 235, 239],
             [275, 279, 283, 287, 291, 295, 299, 303],
@@ -459,48 +471,48 @@
             [467, 471, 475, 479, 483, 487, 491, 495],
         ]
     )
     bool_mat = np.isclose(expected_pt_3, pt_3)
     np.testing.assert_equal(np.all(bool_mat), True)
 
     # Trace out the first and second subsystems:
-    pt_1_2 = partial_trace(test_input_mat, [1, 2], [4, 2, 2])
+    pt_1_2 = partial_trace(test_input_mat, [0, 1], [4, 2, 2])
     expected_pt_1_2 = np.array([[960, 968], [1088, 1096]])
     bool_mat = np.isclose(expected_pt_1_2, pt_1_2)
     np.testing.assert_equal(np.all(bool_mat), True)
 
     # Trace out the first and third subsystems:
-    pt_1_3 = partial_trace(test_input_mat, [1, 3], [4, 2, 2])
+    pt_1_3 = partial_trace(test_input_mat, [0, 2], [4, 2, 2])
     expected_pt_1_3 = np.array([[892, 908], [1148, 1164]])
     bool_mat = np.isclose(expected_pt_1_3, pt_1_3)
     np.testing.assert_equal(np.all(bool_mat), True)
 
     # Trace out the second and third subsystems:
-    pt_2_3 = partial_trace(test_input_mat, [2, 3], [4, 2, 2])
+    pt_2_3 = partial_trace(test_input_mat, [1, 2], [4, 2, 2])
     expected_pt_2_3 = np.array(
         [[106, 122, 138, 154], [362, 378, 394, 410], [618, 634, 650, 666], [874, 890, 906, 922]]
     )
     bool_mat = np.isclose(expected_pt_2_3, pt_2_3)
     np.testing.assert_equal(np.all(bool_mat), True)
 
 
 def test_partial_trace_16_by_16_subsystems_4_4():
     """Test for 16-by-16 matrix for subsystems 4 x 4."""
     test_input_mat = np.arange(1, 257).reshape(16, 16)
 
     # Trace out first subsystem:
-    pt_1 = partial_trace(test_input_mat, [1], [4, 4])
+    pt_1 = partial_trace(test_input_mat, [0], [4, 4])
     expected_pt_1 = np.array(
         [[412, 416, 420, 424], [476, 480, 484, 488], [540, 544, 548, 552], [604, 608, 612, 616]]
     )
     bool_mat = np.isclose(expected_pt_1, pt_1)
     np.testing.assert_equal(np.all(bool_mat), True)
 
     # Trace out second subsystem:
-    pt_2 = partial_trace(test_input_mat, [2], [4, 4])
+    pt_2 = partial_trace(test_input_mat, [1], [4, 4])
     expected_pt_2 = np.array(
         [[106, 122, 138, 154], [362, 378, 394, 410], [618, 634, 650, 666], [874, 890, 906, 922]]
     )
     bool_mat = np.isclose(expected_pt_2, pt_2)
     np.testing.assert_equal(np.all(bool_mat), True)
 
 
@@ -517,15 +529,15 @@
     # Trace out first and third subsystem:
     # Trace out first and fourth subsystem:
 
     # Trace out second and third subsystem:
     # Trace out second and fourth subsystem:
 
     # Trace out third and fourth subsystem:
-    pt_3_4 = partial_trace(test_input_mat, [3, 4], [4, 4, 2, 2])
+    pt_3_4 = partial_trace(test_input_mat, [2, 3], [4, 4, 2, 2])
     expected_pt_3_4 = np.array(
         [
             [394, 410, 426, 442, 458, 474, 490, 506, 522, 538, 554, 570, 586, 602, 618, 634],
             [
                 1418,
                 1434,
                 1450,
@@ -797,45 +809,45 @@
             ],
         ]
     )
     bool_mat = np.isclose(expected_pt_3_4, pt_3_4)
     np.testing.assert_equal(np.all(bool_mat), True)
 
     # Trace out first, second, and third subsystem:
-    pt_1_2_3 = partial_trace(test_input_mat, [1, 2, 3], [4, 4, 2, 2])
+    pt_1_2_3 = partial_trace(test_input_mat, [0, 1, 2], [4, 4, 2, 2])
     expected_pt_1_2_3 = np.array([[64512, 64544], [66560, 66592]])
     bool_mat = np.isclose(expected_pt_1_2_3, pt_1_2_3)
     np.testing.assert_equal(np.all(bool_mat), True)
 
     # Trace out first, third, and fourth subsystem:
-    pt_1_3_4 = partial_trace(test_input_mat, [1, 3, 4], [4, 4, 2, 2])
+    pt_1_3_4 = partial_trace(test_input_mat, [0, 2, 3], [4, 4, 2, 2])
     expected_pt_1_3_4 = np.array(
         [
             [26536, 26600, 26664, 26728],
             [30632, 30696, 30760, 30824],
             [34728, 34792, 34856, 34920],
             [38824, 38888, 38952, 39016],
         ]
     )
     bool_mat = np.isclose(expected_pt_1_3_4, pt_1_3_4)
     np.testing.assert_equal(np.all(bool_mat), True)
 
     # Trace out first, second, third, and fourth subsystem:
-    pt_1_2_3_4 = partial_trace(test_input_mat, [1, 2, 3, 4], [4, 4, 2, 2])
+    pt_1_2_3_4 = partial_trace(test_input_mat, [0, 1, 2, 3], [4, 4, 2, 2])
     expected_pt_1_2_3_4 = np.array([[131104]])
     bool_mat = np.isclose(expected_pt_1_2_3_4, pt_1_2_3_4)
     np.testing.assert_equal(np.all(bool_mat), True)
 
 
 def test_partial_trace_64_by_64_subsystems_4_4_4():
     """Test for 64-by-64 matrix for subsystems 4 x 4 x 4."""
     test_input_mat = np.arange(1, 4097).reshape(64, 64)
 
     # Trace out first subsystem:
-    pt_1 = partial_trace(test_input_mat, [1], [4, 4, 4])
+    pt_1 = partial_trace(test_input_mat, [0], [4, 4, 4])
     expected_pt_1 = np.array(
         [
             [
                 6244,
                 6248,
                 6252,
                 6256,
@@ -1128,54 +1140,54 @@
     np.testing.assert_equal(np.all(bool_mat), True)
 
     # Trace out second subsystem:
 
     # Trace out third subsystem:
 
     # Trace out first and second subsystem:
-    pt_1_2 = partial_trace(test_input_mat, [1, 2], [4, 4, 4])
+    pt_1_2 = partial_trace(test_input_mat, [0, 1], [4, 4, 4])
     expected_pt_1_2 = np.array(
         [
             [31216, 31232, 31248, 31264],
             [32240, 32256, 32272, 32288],
             [33264, 33280, 33296, 33312],
             [34288, 34304, 34320, 34336],
         ]
     )
     bool_mat = np.isclose(expected_pt_1_2, pt_1_2)
     np.testing.assert_equal(np.all(bool_mat), True)
 
     # Trace out first and third subsystem:
-    pt_1_3 = partial_trace(test_input_mat, [1, 3], [4, 4, 4])
+    pt_1_3 = partial_trace(test_input_mat, [0, 2], [4, 4, 4])
     expected_pt_1_3 = np.array(
         [
             [26536, 26600, 26664, 26728],
             [30632, 30696, 30760, 30824],
             [34728, 34792, 34856, 34920],
             [38824, 38888, 38952, 39016],
         ]
     )
     bool_mat = np.isclose(expected_pt_1_3, pt_1_3)
     np.testing.assert_equal(np.all(bool_mat), True)
 
     # Trace out second and third subsystem:
-    pt_2_3 = partial_trace(test_input_mat, [2, 3], [4, 4, 4])
+    pt_2_3 = partial_trace(test_input_mat, [1, 2], [4, 4, 4])
     expected_pt_2_3 = np.array(
         [
             [7816, 8072, 8328, 8584],
             [24200, 24456, 24712, 24968],
             [40584, 40840, 41096, 41352],
             [56968, 57224, 57480, 57736],
         ]
     )
     bool_mat = np.isclose(expected_pt_2_3, pt_2_3)
     np.testing.assert_equal(np.all(bool_mat), True)
 
     # Trace out first, second, and third subsystems:
-    pt_1_2_3 = partial_trace(test_input_mat, [1, 2, 3], [4, 4, 4])
+    pt_1_2_3 = partial_trace(test_input_mat, [0, 1, 2], [4, 4, 4])
     expected_pt_1_2_3 = np.array([[131104]])
 
     bool_mat = np.isclose(expected_pt_1_2_3, pt_1_2_3)
     np.testing.assert_equal(np.all(bool_mat), True)
 
 
 def test_partial_trace_invalid_sys_arg():
@@ -1185,15 +1197,15 @@
         partial_trace(rho, "invalid_input")
 
 
 def test_partial_trace_non_square_matrix_dim_2():
     """Matrix must be square for partial trace."""
     with np.testing.assert_raises(ValueError):
         rho = np.array([[1, 2, 3, 4], [5, 6, 7, 8], [9, 10, 11, 12]])
-        partial_trace(rho, 2, [2])
+        partial_trace(rho, [1], [2])
 
 
 def test_partial_trace_cvxpy():
     """Test partial trace on cvxpy objects."""
     x_var = cvxpy.Variable((4, 4), hermitian=True)
     x_pt = partial_trace(x_var)
     np.testing.assert_equal(isinstance(x_pt, Vstack), True)
```

### Comparing `toqito-1.0.5/tests/test_channels/test_partial_transpose.py` & `toqito-1.0.6/tests/test_channels/test_partial_transpose.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,32 +9,44 @@
 
 
 def test_partial_transpose_bipartite():
     """Partial transpose of bipartite systems."""
     rho = np.arange(16).reshape(4, 4)
 
     # Partial transpose of first subsystem:
-    res = partial_transpose(rho, [1], [2, 2])
+    res = partial_transpose(rho, [0], [2, 2])
     expected_res = np.array([[0, 1, 8, 9], [4, 5, 12, 13], [2, 3, 10, 11], [6, 7, 14, 15]])
     bool_mat = np.isclose(expected_res, res)
     np.testing.assert_equal(np.all(bool_mat), True)
 
     # Partial transpose of second subsystem:
-    res = partial_transpose(rho, [2], [2, 2])
+    res = partial_transpose(rho, [1], [2, 2])
     expected_res = np.array([[0, 4, 2, 6], [1, 5, 3, 7], [8, 12, 10, 14], [9, 13, 11, 15]])
     bool_mat = np.isclose(expected_res, res)
     np.testing.assert_equal(np.all(bool_mat), True)
 
     # Full transpose:
-    res = partial_transpose(rho, [1, 2], [2, 2])
+    res = partial_transpose(rho, [0, 1], [2, 2])
     expected_res = np.array([[0, 4, 8, 12], [1, 5, 9, 13], [2, 6, 10, 14], [3, 7, 11, 15]])
     bool_mat = np.isclose(expected_res, res)
     np.testing.assert_equal(np.all(bool_mat), True)
 
 
+def test_partial_transpose_sys_int():
+    """Partial transpose `sys` argument is provided as `int`."""
+    test_input_mat = np.arange(1, 17).reshape(4, 4)
+
+    expected_res = np.array([[1, 2, 9, 10], [5, 6, 13, 14], [3, 4, 11, 12], [7, 8, 15, 16]])
+
+    res = partial_transpose(test_input_mat, sys=0)
+
+    bool_mat = np.isclose(res, expected_res)
+    np.testing.assert_equal(np.all(bool_mat), True)
+
+
 def test_partial_transpose():
     """
     Default partial_transpose.
 
     By default, the partial_transpose function performs the transposition
     on the second subsystem.
     """
@@ -55,64 +67,64 @@
     By specifying the `sys` argument, you can perform the transposition on
     the first subsystem instead:
     """
     test_input_mat = np.arange(1, 17).reshape(4, 4)
 
     expected_res = np.array([[1, 2, 9, 10], [5, 6, 13, 14], [3, 4, 11, 12], [7, 8, 15, 16]])
 
-    res = partial_transpose(test_input_mat, 1)
+    res = partial_transpose(test_input_mat, [0])
 
     bool_mat = np.isclose(res, expected_res)
     np.testing.assert_equal(np.all(bool_mat), True)
 
 
 def test_partial_transpose_sys_vec():
     """Partial transpose on matrix with `sys` defined as vector."""
     test_input_mat = np.arange(1, 17).reshape(4, 4)
 
     expected_res = np.array([[1, 5, 9, 13], [2, 6, 10, 14], [3, 7, 11, 15], [4, 8, 12, 16]])
 
-    res = partial_transpose(test_input_mat, [1, 2])
+    res = partial_transpose(test_input_mat, [0, 1])
 
     bool_mat = np.isclose(res, expected_res)
     np.testing.assert_equal(np.all(bool_mat), True)
 
 
 def test_partial_transpose_sys_vec_dim_vec():
     """Variables `sys` and `dim` defined as vector."""
     test_input_mat = np.arange(1, 17).reshape(4, 4)
 
     expected_res = np.array([[1, 5, 9, 13], [2, 6, 10, 14], [3, 7, 11, 15], [4, 8, 12, 16]])
 
-    res = partial_transpose(test_input_mat, [1, 2], [2, 2])
+    res = partial_transpose(test_input_mat, [0, 1], [2, 2])
 
     bool_mat = np.isclose(res, expected_res)
     np.testing.assert_equal(np.all(bool_mat), True)
 
 
 def test_partial_transpose_norm_diff():
     """
     Apply partial transpose to first and second subsystem.
 
     Applying the transpose to both the first and second subsystems results
     in the standard transpose of the matrix.
     """
     test_input_mat = np.arange(1, 17).reshape(4, 4)
-    res = np.linalg.norm(partial_transpose(test_input_mat, [1, 2]) - test_input_mat.conj().T)
+    res = np.linalg.norm(partial_transpose(test_input_mat, [0, 1]) - test_input_mat.conj().T)
     expected_res = 0
 
     np.testing.assert_equal(np.isclose(res, expected_res), True)
 
 
 def test_partial_transpose_8_by_8_subsystems_2_2_2():
     """Partial transpose on a 8-by-8 matrix on 2 x 2 x 2 subsystems."""
     test_input_mat = np.arange(1, 65).reshape(8, 8)
 
     # Partial transpose on first subsystem:
-    pt_1 = partial_transpose(test_input_mat, [1], [2, 2, 2])
+    pt_1 = partial_transpose(test_input_mat, [0], [2, 2, 2])
     expected_pt_1 = np.array(
         [
             [1, 2, 3, 4, 33, 34, 35, 36],
             [9, 10, 11, 12, 41, 42, 43, 44],
             [17, 18, 19, 20, 49, 50, 51, 52],
             [25, 26, 27, 28, 57, 58, 59, 60],
             [5, 6, 7, 8, 37, 38, 39, 40],
@@ -121,15 +133,15 @@
             [29, 30, 31, 32, 61, 62, 63, 64],
         ]
     )
     bool_mat = np.isclose(expected_pt_1, pt_1)
     np.testing.assert_equal(np.all(bool_mat), True)
 
     # Partial transpose on second subsystem:
-    pt_2 = partial_transpose(test_input_mat, [2], [2, 2, 2])
+    pt_2 = partial_transpose(test_input_mat, [1], [2, 2, 2])
     expected_pt_2 = np.array(
         [
             [1, 2, 17, 18, 5, 6, 21, 22],
             [9, 10, 25, 26, 13, 14, 29, 30],
             [3, 4, 19, 20, 7, 8, 23, 24],
             [11, 12, 27, 28, 15, 16, 31, 32],
             [33, 34, 49, 50, 37, 38, 53, 54],
@@ -138,15 +150,15 @@
             [43, 44, 59, 60, 47, 48, 63, 64],
         ]
     )
     bool_mat = np.isclose(expected_pt_2, pt_2)
     np.testing.assert_equal(np.all(bool_mat), True)
 
     # Partial transpose on third subsystem:
-    pt_3 = partial_transpose(test_input_mat, [3], [2, 2, 2])
+    pt_3 = partial_transpose(test_input_mat, [2], [2, 2, 2])
     expected_pt_3 = np.array(
         [
             [1, 9, 3, 11, 5, 13, 7, 15],
             [2, 10, 4, 12, 6, 14, 8, 16],
             [17, 25, 19, 27, 21, 29, 23, 31],
             [18, 26, 20, 28, 22, 30, 24, 32],
             [33, 41, 35, 43, 37, 45, 39, 47],
@@ -155,15 +167,15 @@
             [50, 58, 52, 60, 54, 62, 56, 64],
         ]
     )
     bool_mat = np.isclose(expected_pt_3, pt_3)
     np.testing.assert_equal(np.all(bool_mat), True)
 
     # Partial transpose on first and second subsystem:
-    pt_1_2 = partial_transpose(test_input_mat, [1, 2], [2, 2, 2])
+    pt_1_2 = partial_transpose(test_input_mat, [0, 1], [2, 2, 2])
     expected_pt_1_2 = np.array(
         [
             [1, 2, 17, 18, 33, 34, 49, 50],
             [9, 10, 25, 26, 41, 42, 57, 58],
             [3, 4, 19, 20, 35, 36, 51, 52],
             [11, 12, 27, 28, 43, 44, 59, 60],
             [5, 6, 21, 22, 37, 38, 53, 54],
@@ -172,15 +184,15 @@
             [15, 16, 31, 32, 47, 48, 63, 64],
         ]
     )
     bool_mat = np.isclose(expected_pt_1_2, pt_1_2)
     np.testing.assert_equal(np.all(bool_mat), True)
 
     # Partial transpose on first and third subsystem:
-    pt_1_3 = partial_transpose(test_input_mat, [1, 3], [2, 2, 2])
+    pt_1_3 = partial_transpose(test_input_mat, [0, 2], [2, 2, 2])
     expected_pt_1_3 = np.array(
         [
             [1, 9, 3, 11, 33, 41, 35, 43],
             [2, 10, 4, 12, 34, 42, 36, 44],
             [17, 25, 19, 27, 49, 57, 51, 59],
             [18, 26, 20, 28, 50, 58, 52, 60],
             [5, 13, 7, 15, 37, 45, 39, 47],
@@ -189,15 +201,15 @@
             [22, 30, 24, 32, 54, 62, 56, 64],
         ]
     )
     bool_mat = np.isclose(expected_pt_1_3, pt_1_3)
     np.testing.assert_equal(np.all(bool_mat), True)
 
     # Partial transpose on second and third subsystem:
-    pt_2_3 = partial_transpose(test_input_mat, [2, 3], [2, 2, 2])
+    pt_2_3 = partial_transpose(test_input_mat, [1, 2], [2, 2, 2])
     expected_pt_2_3 = np.array(
         [
             [1, 9, 17, 25, 5, 13, 21, 29],
             [2, 10, 18, 26, 6, 14, 22, 30],
             [3, 11, 19, 27, 7, 15, 23, 31],
             [4, 12, 20, 28, 8, 16, 24, 32],
             [33, 41, 49, 57, 37, 45, 53, 61],
@@ -211,15 +223,15 @@
 
 
 def test_partial_transpose_8_by_8_subsystems_2_4():
     """Partial transpose on a 8-by-8 matrix on 2 x 4 subsystems."""
     test_input_mat = np.arange(1, 65).reshape(8, 8)
 
     # Partial transpose on the first subsystem:
-    pt_1 = partial_transpose(test_input_mat, [1], [2, 4])
+    pt_1 = partial_transpose(test_input_mat, [0], [2, 4])
     expected_pt_1 = np.array(
         [
             [1, 2, 3, 4, 33, 34, 35, 36],
             [9, 10, 11, 12, 41, 42, 43, 44],
             [17, 18, 19, 20, 49, 50, 51, 52],
             [25, 26, 27, 28, 57, 58, 59, 60],
             [5, 6, 7, 8, 37, 38, 39, 40],
@@ -228,15 +240,15 @@
             [29, 30, 31, 32, 61, 62, 63, 64],
         ]
     )
     bool_mat = np.isclose(expected_pt_1, pt_1)
     np.testing.assert_equal(np.all(bool_mat), True)
 
     # Partial transpose on the second subsystem:
-    pt_2 = partial_transpose(test_input_mat, [2], [2, 4])
+    pt_2 = partial_transpose(test_input_mat, [1], [2, 4])
     expected_pt_2 = np.array(
         [
             [1, 9, 17, 25, 5, 13, 21, 29],
             [2, 10, 18, 26, 6, 14, 22, 30],
             [3, 11, 19, 27, 7, 15, 23, 31],
             [4, 12, 20, 28, 8, 16, 24, 32],
             [33, 41, 49, 57, 37, 45, 53, 61],
@@ -245,15 +257,15 @@
             [36, 44, 52, 60, 40, 48, 56, 64],
         ]
     )
     bool_mat = np.isclose(expected_pt_2, pt_2)
     np.testing.assert_equal(np.all(bool_mat), True)
 
     # Partial transpose on the first and second subsystem:
-    pt_1_2 = partial_transpose(test_input_mat, [1, 2], [2, 4])
+    pt_1_2 = partial_transpose(test_input_mat, [0, 1], [2, 4])
     expected_pt_1_2 = np.array(
         [
             [1, 9, 17, 25, 33, 41, 49, 57],
             [2, 10, 18, 26, 34, 42, 50, 58],
             [3, 11, 19, 27, 35, 43, 51, 59],
             [4, 12, 20, 28, 36, 44, 52, 60],
             [5, 13, 21, 29, 37, 45, 53, 61],
@@ -267,15 +279,15 @@
 
 
 def test_partial_transpose_8_by_8_subsystems_4_2():
     """Partial transpose on a 8-by-8 matrix on 4 x 2 subsystems."""
     test_input_mat = np.arange(1, 65).reshape(8, 8)
 
     # Partial transpose on the first subsystem:
-    pt_1 = partial_transpose(test_input_mat, [1], [4, 2])
+    pt_1 = partial_transpose(test_input_mat, [0], [4, 2])
     expected_pt_1 = np.array(
         [
             [1, 2, 17, 18, 33, 34, 49, 50],
             [9, 10, 25, 26, 41, 42, 57, 58],
             [3, 4, 19, 20, 35, 36, 51, 52],
             [11, 12, 27, 28, 43, 44, 59, 60],
             [5, 6, 21, 22, 37, 38, 53, 54],
@@ -284,15 +296,15 @@
             [15, 16, 31, 32, 47, 48, 63, 64],
         ]
     )
     bool_mat = np.isclose(expected_pt_1, pt_1)
     np.testing.assert_equal(np.all(bool_mat), True)
 
     # Partial transpose on the second subsystem:
-    pt_2 = partial_transpose(test_input_mat, [2], [4, 2])
+    pt_2 = partial_transpose(test_input_mat, [1], [4, 2])
     expected_pt_2 = np.array(
         [
             [1, 9, 3, 11, 5, 13, 7, 15],
             [2, 10, 4, 12, 6, 14, 8, 16],
             [17, 25, 19, 27, 21, 29, 23, 31],
             [18, 26, 20, 28, 22, 30, 24, 32],
             [33, 41, 35, 43, 37, 45, 39, 47],
@@ -301,15 +313,15 @@
             [50, 58, 52, 60, 54, 62, 56, 64],
         ]
     )
     bool_mat = np.isclose(expected_pt_2, pt_2)
     np.testing.assert_equal(np.all(bool_mat), True)
 
     # Partial transpose on the first and second subsystem:
-    pt_1_2 = partial_transpose(test_input_mat, [1, 2], [4, 2])
+    pt_1_2 = partial_transpose(test_input_mat, [0, 1], [4, 2])
     expected_pt_1_2 = np.array(
         [
             [1, 9, 17, 25, 33, 41, 49, 57],
             [2, 10, 18, 26, 34, 42, 50, 58],
             [3, 11, 19, 27, 35, 43, 51, 59],
             [4, 12, 20, 28, 36, 44, 52, 60],
             [5, 13, 21, 29, 37, 45, 53, 61],
@@ -323,45 +335,45 @@
 
 
 def test_partial_transpose_6_by_6_subsystems_2_3():
     """Partial transpose on a 6-by-6 matrix on 2 x 3 subsystems."""
     test_input_mat = np.arange(1, 37).reshape(6, 6)
 
     # Partial transpose on first subsystem:
-    pt_1 = partial_transpose(test_input_mat, [1], [2, 3])
+    pt_1 = partial_transpose(test_input_mat, [0], [2, 3])
     expected_pt_1 = np.array(
         [
             [1, 2, 3, 19, 20, 21],
             [7, 8, 9, 25, 26, 27],
             [13, 14, 15, 31, 32, 33],
             [4, 5, 6, 22, 23, 24],
             [10, 11, 12, 28, 29, 30],
             [16, 17, 18, 34, 35, 36],
         ]
     )
     bool_mat = np.isclose(expected_pt_1, pt_1)
     np.testing.assert_equal(np.all(bool_mat), True)
 
     # Partial transpose on second subsystem:
-    pt_2 = partial_transpose(test_input_mat, [2], [2, 3])
+    pt_2 = partial_transpose(test_input_mat, [1], [2, 3])
     expected_pt_2 = np.array(
         [
             [1, 7, 13, 4, 10, 16],
             [2, 8, 14, 5, 11, 17],
             [3, 9, 15, 6, 12, 18],
             [19, 25, 31, 22, 28, 34],
             [20, 26, 32, 23, 29, 35],
             [21, 27, 33, 24, 30, 36],
         ]
     )
     bool_mat = np.isclose(expected_pt_2, pt_2)
     np.testing.assert_equal(np.all(bool_mat), True)
 
     # Partial transpose on first and second subsystems:
-    pt_1_2 = partial_transpose(test_input_mat, [1, 2], [2, 3])
+    pt_1_2 = partial_transpose(test_input_mat, [0, 1], [2, 3])
     expected_pt_1_2 = np.array(
         [
             [1, 7, 13, 19, 25, 31],
             [2, 8, 14, 20, 26, 32],
             [3, 9, 15, 21, 27, 33],
             [4, 10, 16, 22, 28, 34],
             [5, 11, 17, 23, 29, 35],
@@ -373,45 +385,45 @@
 
 
 def test_partial_transpose_6_by_6_subsystems_3_2():
     """Partial transpose on a 6-by-6 matrix on 3 x 2 subsystems."""
     test_input_mat = np.arange(1, 37).reshape(6, 6)
 
     # Partial transpose on first subsystem:
-    pt_1 = partial_transpose(test_input_mat, [1], [3, 2])
+    pt_1 = partial_transpose(test_input_mat, [0], [3, 2])
     expected_pt_1 = np.array(
         [
             [1, 2, 13, 14, 25, 26],
             [7, 8, 19, 20, 31, 32],
             [3, 4, 15, 16, 27, 28],
             [9, 10, 21, 22, 33, 34],
             [5, 6, 17, 18, 29, 30],
             [11, 12, 23, 24, 35, 36],
         ]
     )
     bool_mat = np.isclose(expected_pt_1, pt_1)
     np.testing.assert_equal(np.all(bool_mat), True)
 
     # Partial transpose on second subsystem:
-    pt_2 = partial_transpose(test_input_mat, [2], [3, 2])
+    pt_2 = partial_transpose(test_input_mat, [1], [3, 2])
     expected_pt_2 = np.array(
         [
             [1, 7, 3, 9, 5, 11],
             [2, 8, 4, 10, 6, 12],
             [13, 19, 15, 21, 17, 23],
             [14, 20, 16, 22, 18, 24],
             [25, 31, 27, 33, 29, 35],
             [26, 32, 28, 34, 30, 36],
         ]
     )
     bool_mat = np.isclose(expected_pt_2, pt_2)
     np.testing.assert_equal(np.all(bool_mat), True)
 
     # Partial transpose on first and second subsystems:
-    pt_1_2 = partial_transpose(test_input_mat, [1, 2], [3, 2])
+    pt_1_2 = partial_transpose(test_input_mat, [0, 1], [3, 2])
     expected_pt_1_2 = np.array(
         [
             [1, 7, 13, 19, 25, 31],
             [2, 8, 14, 20, 26, 32],
             [3, 9, 15, 21, 27, 33],
             [4, 10, 16, 22, 28, 34],
             [5, 11, 17, 23, 29, 35],
@@ -423,15 +435,15 @@
 
 
 def test_partial_transpose_16_by_16_subsystems_2_2_2_2():
     """Partial transpose on a 16-by-16 matrix on 2 x 2 x 2 x 2 subsystems."""
     rho = np.arange(256).reshape(16, 16)
 
     # Partial transpose of first subsystem:
-    res = partial_transpose(rho, [1], [2, 2, 2, 2])
+    res = partial_transpose(rho, [0], [2, 2, 2, 2])
     expected_res = np.array(
         [
             [0, 1, 2, 3, 4, 5, 6, 7, 128, 129, 130, 131, 132, 133, 134, 135],
             [16, 17, 18, 19, 20, 21, 22, 23, 144, 145, 146, 147, 148, 149, 150, 151],
             [32, 33, 34, 35, 36, 37, 38, 39, 160, 161, 162, 163, 164, 165, 166, 167],
             [48, 49, 50, 51, 52, 53, 54, 55, 176, 177, 178, 179, 180, 181, 182, 183],
             [64, 65, 66, 67, 68, 69, 70, 71, 192, 193, 194, 195, 196, 197, 198, 199],
@@ -448,15 +460,15 @@
             [120, 121, 122, 123, 124, 125, 126, 127, 248, 249, 250, 251, 252, 253, 254, 255],
         ]
     )
     bool_mat = np.isclose(expected_res, res)
     np.testing.assert_equal(np.all(bool_mat), True)
 
     # Partial transpose of second subsystem:
-    res = partial_transpose(rho, [2], [2, 2, 2, 2])
+    res = partial_transpose(rho, [1], [2, 2, 2, 2])
     expected_res = np.array(
         [
             [0, 1, 2, 3, 64, 65, 66, 67, 8, 9, 10, 11, 72, 73, 74, 75],
             [16, 17, 18, 19, 80, 81, 82, 83, 24, 25, 26, 27, 88, 89, 90, 91],
             [32, 33, 34, 35, 96, 97, 98, 99, 40, 41, 42, 43, 104, 105, 106, 107],
             [48, 49, 50, 51, 112, 113, 114, 115, 56, 57, 58, 59, 120, 121, 122, 123],
             [4, 5, 6, 7, 68, 69, 70, 71, 12, 13, 14, 15, 76, 77, 78, 79],
@@ -473,15 +485,15 @@
             [180, 181, 182, 183, 244, 245, 246, 247, 188, 189, 190, 191, 252, 253, 254, 255],
         ]
     )
     bool_mat = np.isclose(expected_res, res)
     np.testing.assert_equal(np.all(bool_mat), True)
 
     # Partial transpose of third subsystem
-    res = partial_transpose(rho, [3], [2, 2, 2, 2])
+    res = partial_transpose(rho, [2], [2, 2, 2, 2])
     expected_res = np.array(
         [
             [0, 1, 32, 33, 4, 5, 36, 37, 8, 9, 40, 41, 12, 13, 44, 45],
             [16, 17, 48, 49, 20, 21, 52, 53, 24, 25, 56, 57, 28, 29, 60, 61],
             [2, 3, 34, 35, 6, 7, 38, 39, 10, 11, 42, 43, 14, 15, 46, 47],
             [18, 19, 50, 51, 22, 23, 54, 55, 26, 27, 58, 59, 30, 31, 62, 63],
             [64, 65, 96, 97, 68, 69, 100, 101, 72, 73, 104, 105, 76, 77, 108, 109],
@@ -498,15 +510,15 @@
             [210, 211, 242, 243, 214, 215, 246, 247, 218, 219, 250, 251, 222, 223, 254, 255],
         ]
     )
     bool_mat = np.isclose(expected_res, res)
     np.testing.assert_equal(np.all(bool_mat), True)
 
     # Partial transpose of fourth subsystem
-    res = partial_transpose(rho, [4], [2, 2, 2, 2])
+    res = partial_transpose(rho, [3], [2, 2, 2, 2])
     expected_res = np.array(
         [
             [0, 16, 2, 18, 4, 20, 6, 22, 8, 24, 10, 26, 12, 28, 14, 30],
             [1, 17, 3, 19, 5, 21, 7, 23, 9, 25, 11, 27, 13, 29, 15, 31],
             [32, 48, 34, 50, 36, 52, 38, 54, 40, 56, 42, 58, 44, 60, 46, 62],
             [33, 49, 35, 51, 37, 53, 39, 55, 41, 57, 43, 59, 45, 61, 47, 63],
             [64, 80, 66, 82, 68, 84, 70, 86, 72, 88, 74, 90, 76, 92, 78, 94],
@@ -523,15 +535,15 @@
             [225, 241, 227, 243, 229, 245, 231, 247, 233, 249, 235, 251, 237, 253, 239, 255],
         ]
     )
     bool_mat = np.isclose(expected_res, res)
     np.testing.assert_equal(np.all(bool_mat), True)
 
     # Partial transpose of first and second subsystem:
-    res = partial_transpose(rho, [1, 2], [2, 2, 2, 2])
+    res = partial_transpose(rho, [0, 1], [2, 2, 2, 2])
     expected_res = np.array(
         [
             [0, 1, 2, 3, 64, 65, 66, 67, 128, 129, 130, 131, 192, 193, 194, 195],
             [16, 17, 18, 19, 80, 81, 82, 83, 144, 145, 146, 147, 208, 209, 210, 211],
             [32, 33, 34, 35, 96, 97, 98, 99, 160, 161, 162, 163, 224, 225, 226, 227],
             [48, 49, 50, 51, 112, 113, 114, 115, 176, 177, 178, 179, 240, 241, 242, 243],
             [4, 5, 6, 7, 68, 69, 70, 71, 132, 133, 134, 135, 196, 197, 198, 199],
@@ -548,15 +560,15 @@
             [60, 61, 62, 63, 124, 125, 126, 127, 188, 189, 190, 191, 252, 253, 254, 255],
         ]
     )
     bool_mat = np.isclose(expected_res, res)
     np.testing.assert_equal(np.all(bool_mat), True)
 
     # Partial transpose of first and third subsystem:
-    res = partial_transpose(rho, [1, 3], [2, 2, 2, 2])
+    res = partial_transpose(rho, [0, 2], [2, 2, 2, 2])
     expected_res = np.array(
         [
             [0, 1, 32, 33, 4, 5, 36, 37, 128, 129, 160, 161, 132, 133, 164, 165],
             [16, 17, 48, 49, 20, 21, 52, 53, 144, 145, 176, 177, 148, 149, 180, 181],
             [2, 3, 34, 35, 6, 7, 38, 39, 130, 131, 162, 163, 134, 135, 166, 167],
             [18, 19, 50, 51, 22, 23, 54, 55, 146, 147, 178, 179, 150, 151, 182, 183],
             [64, 65, 96, 97, 68, 69, 100, 101, 192, 193, 224, 225, 196, 197, 228, 229],
@@ -573,15 +585,15 @@
             [90, 91, 122, 123, 94, 95, 126, 127, 218, 219, 250, 251, 222, 223, 254, 255],
         ]
     )
     bool_mat = np.isclose(expected_res, res)
     np.testing.assert_equal(np.all(bool_mat), True)
 
     # Partial transpose of first and fourth subsystem
-    res = partial_transpose(rho, [1, 4], [2, 2, 2, 2])
+    res = partial_transpose(rho, [0, 3], [2, 2, 2, 2])
     expected_res = np.array(
         [
             [0, 16, 2, 18, 4, 20, 6, 22, 128, 144, 130, 146, 132, 148, 134, 150],
             [1, 17, 3, 19, 5, 21, 7, 23, 129, 145, 131, 147, 133, 149, 135, 151],
             [32, 48, 34, 50, 36, 52, 38, 54, 160, 176, 162, 178, 164, 180, 166, 182],
             [33, 49, 35, 51, 37, 53, 39, 55, 161, 177, 163, 179, 165, 181, 167, 183],
             [64, 80, 66, 82, 68, 84, 70, 86, 192, 208, 194, 210, 196, 212, 198, 214],
@@ -598,15 +610,15 @@
             [105, 121, 107, 123, 109, 125, 111, 127, 233, 249, 235, 251, 237, 253, 239, 255],
         ]
     )
     bool_mat = np.isclose(expected_res, res)
     np.testing.assert_equal(np.all(bool_mat), True)
 
     # Partial transpose of second and third subsystem:
-    res = partial_transpose(rho, [2, 3], [2, 2, 2, 2])
+    res = partial_transpose(rho, [1, 2], [2, 2, 2, 2])
     expected_res = np.array(
         [
             [0, 1, 32, 33, 64, 65, 96, 97, 8, 9, 40, 41, 72, 73, 104, 105],
             [16, 17, 48, 49, 80, 81, 112, 113, 24, 25, 56, 57, 88, 89, 120, 121],
             [2, 3, 34, 35, 66, 67, 98, 99, 10, 11, 42, 43, 74, 75, 106, 107],
             [18, 19, 50, 51, 82, 83, 114, 115, 26, 27, 58, 59, 90, 91, 122, 123],
             [4, 5, 36, 37, 68, 69, 100, 101, 12, 13, 44, 45, 76, 77, 108, 109],
@@ -623,15 +635,15 @@
             [150, 151, 182, 183, 214, 215, 246, 247, 158, 159, 190, 191, 222, 223, 254, 255],
         ]
     )
     bool_mat = np.isclose(expected_res, res)
     np.testing.assert_equal(np.all(bool_mat), True)
 
     # Partial transpose of second and fourth subsystem:
-    res = partial_transpose(rho, [2, 4], [2, 2, 2, 2])
+    res = partial_transpose(rho, [1, 3], [2, 2, 2, 2])
     expected_res = np.array(
         [
             [0, 16, 2, 18, 64, 80, 66, 82, 8, 24, 10, 26, 72, 88, 74, 90],
             [1, 17, 3, 19, 65, 81, 67, 83, 9, 25, 11, 27, 73, 89, 75, 91],
             [32, 48, 34, 50, 96, 112, 98, 114, 40, 56, 42, 58, 104, 120, 106, 122],
             [33, 49, 35, 51, 97, 113, 99, 115, 41, 57, 43, 59, 105, 121, 107, 123],
             [4, 20, 6, 22, 68, 84, 70, 86, 12, 28, 14, 30, 76, 92, 78, 94],
@@ -648,15 +660,15 @@
             [165, 181, 167, 183, 229, 245, 231, 247, 173, 189, 175, 191, 237, 253, 239, 255],
         ]
     )
     bool_mat = np.isclose(expected_res, res)
     np.testing.assert_equal(np.all(bool_mat), True)
 
     # Partial transpose of third and fourth subsystem
-    res = partial_transpose(rho, [3, 4], [2, 2, 2, 2])
+    res = partial_transpose(rho, [2, 3], [2, 2, 2, 2])
     expected_res = np.array(
         [
             [0, 16, 32, 48, 4, 20, 36, 52, 8, 24, 40, 56, 12, 28, 44, 60],
             [1, 17, 33, 49, 5, 21, 37, 53, 9, 25, 41, 57, 13, 29, 45, 61],
             [2, 18, 34, 50, 6, 22, 38, 54, 10, 26, 42, 58, 14, 30, 46, 62],
             [3, 19, 35, 51, 7, 23, 39, 55, 11, 27, 43, 59, 15, 31, 47, 63],
             [64, 80, 96, 112, 68, 84, 100, 116, 72, 88, 104, 120, 76, 92, 108, 124],
@@ -690,48 +702,48 @@
 def test_partial_transpose_non_square_matrix():
     """Matrix must be square."""
     with np.testing.assert_raises(ValueError):
         test_input_mat = np.array([[1, 2, 3, 4], [5, 6, 7, 8], [13, 14, 15, 16]])
         partial_transpose(test_input_mat)
 
 
+def test_partial_transpose_non_square():
+    """Test partial transpose on non square matrices ."""
+    rho = np.kron(np.eye(2, 3), np.ones((2, 3)))
+    rho = np.kron(rho, np.eye(2, 3))
+
+    dim = np.array([[2, 2, 2], [3, 3, 3]])
+
+    res = partial_transpose(rho, sys=1, dim=dim)
+
+    expected = np.kron(np.eye(2, 3), np.ones((3, 2)))
+    expected = np.kron(expected, np.eye(2, 3))
+    np.testing.assert_equal(np.allclose(res, expected), True)
+
+
 def test_partial_transpose_non_square_matrix_2():
     """Matrix must be square."""
     with np.testing.assert_raises(ValueError):
         rho = np.array([[1, 2, 3, 4], [5, 6, 7, 8], [9, 10, 11, 12]])
         partial_transpose(rho, 2, [2])
 
 
 def test_partial_transpose_cvxpy():
     """Test partial transpose on cvxpy objects."""
     x_var = cvxpy.Variable((4, 4), hermitian=True)
     x_pt = partial_transpose(x_var)
     np.testing.assert_equal(isinstance(x_pt, Vstack), True)
 
 
-def test_partial_transpose_non_square():
-    """Test partial transpose on non square matrices ."""
-    rho = np.kron(np.eye(2, 3), np.ones((2, 3)))
-    rho = np.kron(rho, np.eye(2, 3))
-
-    dim = np.array([[2, 2, 2], [3, 3, 3]])
-
-    res = partial_transpose(rho, sys=2, dim=dim)
-
-    expected = np.kron(np.eye(2, 3), np.ones((3, 2)))
-    expected = np.kron(expected, np.eye(2, 3))
-    np.testing.assert_equal(np.allclose(res, expected), True)
-
-
 def test_partial_transpose_three_subsystems():
     """Test partial transpose on 3 - subsystems ."""
     mat = np.arange(64).reshape((8, 8))
     input_mat = np.kron(np.eye(2, 2), mat)
 
-    res = partial_transpose(input_mat, sys=[2, 3, 4], dim=[2, 2, 2, 2])
+    res = partial_transpose(input_mat, [1, 2, 3], [2, 2, 2, 2])
 
     expected = np.kron(np.eye(2, 2), mat.T)
     np.testing.assert_equal(np.allclose(res, expected), True)
 
 
 if __name__ == "__main__":
     np.testing.run_module_suite()
```

### Comparing `toqito-1.0.5/tests/test_channels/test_realignment.py` & `toqito-1.0.6/tests/test_channels/test_realignment.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/tests/test_channels/test_reduction.py` & `toqito-1.0.6/tests/test_channels/test_reduction.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/tests/test_helper/test_expr_as_np_array.py` & `toqito-1.0.6/tests/test_helper/test_expr_as_np_array.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/tests/test_helper/test_npa_constraints.py` & `toqito-1.0.6/tests/test_helper/test_npa_constraints.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/tests/test_helper/test_update_odometer.py` & `toqito-1.0.6/tests/test_helper/test_update_odometer.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/tests/test_matrices/test_gell_mann.py` & `toqito-1.0.6/tests/test_matrices/test_gell_mann.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/tests/test_matrices/test_gen_gell_mann.py` & `toqito-1.0.6/tests/test_matrices/test_gen_gell_mann.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/tests/test_matrices/test_gen_pauli.py` & `toqito-1.0.6/tests/test_matrices/test_gen_pauli.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/tests/test_matrices/test_hadamard.py` & `toqito-1.0.6/tests/test_matrices/test_hadamard.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/tests/test_matrices/test_iden.py` & `toqito-1.0.6/tests/test_matrices/test_iden.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/tests/test_matrices/test_pauli.py` & `toqito-1.0.6/tests/test_matrices/test_pauli.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/tests/test_matrices/test_standard_basis.py` & `toqito-1.0.6/tests/test_matrices/test_standard_basis.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/tests/test_matrix_ops/test_outer_product.py` & `toqito-1.0.6/tests/test_matrix_ops/test_outer_product.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,39 +3,38 @@
 
 from toqito.matrix_ops import outer_product
 
 
 def test_outer_product():
     """Test with two vectors, no complications."""
 
-    v1, v2 = np.array([1,2,3]), np.array([4,5,6])
-    expected_res = np.array([[4,5,6],[8,10,12],[12,15,18]])
+    v1, v2 = np.array([1, 2, 3]), np.array([4, 5, 6])
+    expected_res = np.array([[4, 5, 6], [8, 10, 12], [12, 15, 18]])
     np.testing.assert_equal(outer_product(v1, v2), expected_res)
 
 
 def test_outer_product_negative():
     """Test with two vectors, with negative input/output values."""
 
-    v1, v2 = np.array([-1,2,3]), np.array([4,5,6])
-    expected_res = np.array([[-4,-5,-6],[8,10,12],[12,15,18]])
+    v1, v2 = np.array([-1, 2, 3]), np.array([4, 5, 6])
+    expected_res = np.array([[-4, -5, -6], [8, 10, 12], [12, 15, 18]])
     np.testing.assert_equal(outer_product(v1, v2), expected_res)
 
 
 def test_outer_product_different_dimensions():
     """Test with two vectors of different dimensions."""
 
-    v1, v2 = np.array([1,2,3]), np.array([4,5,6,7])
+    v1, v2 = np.array([1, 2, 3]), np.array([4, 5, 6, 7])
     with np.testing.assert_raises(ValueError):
         outer_product(v1, v2)
 
 
 def test_outer_product_different_dimensions_2():
     """Test with a vector and a 2d array."""
 
-    v1, v2 = np.array([1,2,3]), np.array([[4,5,6],[7,8,9]])
+    v1, v2 = np.array([1, 2, 3]), np.array([[4, 5, 6], [7, 8, 9]])
     with np.testing.assert_raises(ValueError):
         outer_product(v1, v2)
 
 
-
 if __name__ == "__main__":
     np.testing.run_module_suite()
```

### Comparing `toqito-1.0.5/tests/test_matrix_ops/test_tensor.py` & `toqito-1.0.6/tests/test_matrix_ops/test_tensor.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/tests/test_matrix_ops/test_unvec.py` & `toqito-1.0.6/tests/test_matrix_ops/test_unvec.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 def test_unvec_custom_dim():
     """Test standard unvec operation on a vector with custom dimension."""
     expected_res = np.array([[1], [3], [2], [4]])
 
     test_input_vec = np.array([1, 3, 2, 4])
 
-    res = unvec(test_input_vec, [1, 4])
+    res = unvec(test_input_vec, [4, 1])
 
     bool_mat = np.isclose(res, expected_res)
     np.testing.assert_equal(np.all(bool_mat), True)
 
 
 if __name__ == "__main__":
     np.testing.run_module_suite()
```

### Comparing `toqito-1.0.5/tests/test_matrix_props/test_is_block_positive.py` & `toqito-1.0.6/tests/test_matrix_props/test_is_block_positive.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """Test is_block_positive."""
 import numpy as np
 import pytest
 
 from toqito.states import bell
-from toqito.channels import choi, partial_transpose
+from toqito.channels import choi
 from toqito.perms import swap, swap_operator
 from toqito.matrix_props import is_block_positive
+from picos import partial_transpose
 
 
 @pytest.mark.parametrize("dim", [2, 3, 4])
 def test_swap_operator_is_block_positive(dim):
     """Test Swap is 1-block positive but not 2-block positive."""
     mat = swap_operator(dim)
     np.testing.assert_equal(is_block_positive(mat), True)
@@ -32,15 +33,15 @@
     is block positive.
     """
     b_0 = bell(0)
     b_3 = bell(3)
     v_0 = np.kron(b_0, b_0)
     y_mat = (
         np.kron(np.eye(4), b_0 @ b_0.T) / 2
-        + np.kron(b_3 @ b_3.T, partial_transpose(b_3 @ b_3.T, 1))
+        + np.kron(b_3 @ b_3.T, partial_transpose(b_3 @ b_3.T, [0]))
     ) / 3 - v_0 @ v_0.T / 4
     mat = swap(y_mat, [2, 3], [2, 2, 2, 2])
     np.testing.assert_equal(is_block_positive(mat), True)
 
 
 if __name__ == "__main__":
     np.testing.run_module_suite()
```

### Comparing `toqito-1.0.5/tests/test_matrix_props/test_is_commuting.py` & `toqito-1.0.6/tests/test_matrix_props/test_is_commuting.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/tests/test_matrix_props/test_is_density.py` & `toqito-1.0.6/tests/test_matrix_props/test_is_density.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/tests/test_matrix_props/test_is_diagonal.py` & `toqito-1.0.6/tests/test_matrix_props/test_is_diagonal.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/tests/test_matrix_props/test_is_hermitian.py` & `toqito-1.0.6/tests/test_matrix_props/test_is_hermitian.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/tests/test_matrix_props/test_is_idempotent.py` & `toqito-1.0.6/tests/test_matrix_props/test_is_idempotent.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/tests/test_matrix_props/test_is_identity.py` & `toqito-1.0.6/tests/test_matrix_props/test_is_identity.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/tests/test_matrix_props/test_is_normal.py` & `toqito-1.0.6/tests/test_matrix_props/test_is_normal.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/tests/test_matrix_props/test_is_orthonormal.py` & `toqito-1.0.6/tests/test_matrix_props/test_is_orthonormal.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/tests/test_matrix_props/test_is_permutation.py` & `toqito-1.0.6/tests/test_matrix_props/test_is_permutation.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/tests/test_matrix_props/test_is_positive_definite.py` & `toqito-1.0.6/tests/test_matrix_props/test_is_positive_definite.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,35 +12,45 @@
 
 def test_is_not_positive_definite():
     """Check that non-positive definite matrix returns False."""
     mat = np.array([[-1, -1], [-1, -1]])
     np.testing.assert_equal(is_positive_definite(mat), False)
 
     eps = 0
-    c_var = 1/np.sqrt(3)
-    gram = np.array([
-        [1, c_var, c_var, c_var], 
-        [c_var, 1, c_var*1j, (1 + c_var*1j)/2],
-        [c_var, -c_var*1j, 1, (1 - c_var*1j)/2],
-        [c_var, (1 - c_var*1j)/2, (1 + c_var*1j)/2, 1],
-    ])
+    c_var = 1 / np.sqrt(3)
+    gram = np.array(
+        [
+            [1, c_var, c_var, c_var],
+            [c_var, 1, c_var * 1j, (1 + c_var * 1j) / 2],
+            [c_var, -c_var * 1j, 1, (1 - c_var * 1j) / 2],
+            [c_var, (1 - c_var * 1j) / 2, (1 + c_var * 1j) / 2, 1],
+        ]
+    )
 
-    v_vec = np.array([
-        [1], 
-        [(-np.sqrt(3) + 1j)/2], 
-        [(-np.sqrt(3) - 1j)/2], 
-        [0],
-    ])
-    w_vec = np.array([
-        [0], 
-        [0], 
-        [0], 
-        [1],
-    ])
-    gram_eps = 1/(1 - 2 * eps) * (gram + eps * (v_vec @ v_vec.conj().T + w_vec @ w_vec.conj().T - 3 * np.identity(4)))
+    v_vec = np.array(
+        [
+            [1],
+            [(-np.sqrt(3) + 1j) / 2],
+            [(-np.sqrt(3) - 1j) / 2],
+            [0],
+        ]
+    )
+    w_vec = np.array(
+        [
+            [0],
+            [0],
+            [0],
+            [1],
+        ]
+    )
+    gram_eps = (
+        1
+        / (1 - 2 * eps)
+        * (gram + eps * (v_vec @ v_vec.conj().T + w_vec @ w_vec.conj().T - 3 * np.identity(4)))
+    )
     np.testing.assert_equal(is_positive_definite(gram_eps), False)
 
 
 def test_is_positive_definite_not_hermitian():
     """Input must be a Hermitian matrix."""
     mat = np.array([[1, 2, 3], [4, 5, 6], [7, 8, 9]])
     np.testing.assert_equal(is_positive_definite(mat), False)
```

### Comparing `toqito-1.0.5/tests/test_matrix_props/test_is_positive_semidefinite.py` & `toqito-1.0.6/tests/test_matrix_props/test_is_positive_semidefinite.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/tests/test_matrix_props/test_is_projection.py` & `toqito-1.0.6/tests/test_matrix_props/test_is_projection.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/tests/test_matrix_props/test_is_square.py` & `toqito-1.0.6/tests/test_matrix_props/test_is_square.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/tests/test_matrix_props/test_is_symmetric.py` & `toqito-1.0.6/tests/test_matrix_props/test_is_symmetric.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/tests/test_matrix_props/test_is_unitary.py` & `toqito-1.0.6/tests/test_matrix_props/test_is_unitary.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/tests/test_matrix_props/test_majorizes.py` & `toqito-1.0.6/tests/test_matrix_props/test_majorizes.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,19 +11,19 @@
     np.testing.assert_equal(majorizes([3, 0, 0], [1, 1, 1]), True)
 
 
 def test_majorizes_max_entangled():
     """Test that max entangled partial trace returns False."""
     v_vec = max_entangled(3)
     rho = v_vec * v_vec.conj().T
-    np.testing.assert_equal(majorizes(partial_trace(rho), rho), False)
+    np.testing.assert_equal(majorizes(partial_trace(rho, [1], [3, 3]), rho), False)
 
 
 def test_majorizes_max_entangled_flip():
     """Test that max entangled partial trace returns True (flipped args)."""
     v_vec = max_entangled(3)
     rho = v_vec * v_vec.conj().T
-    np.testing.assert_equal(majorizes(rho, partial_trace(rho)), True)
+    np.testing.assert_equal(majorizes(rho, partial_trace(rho, [1], [3, 3])), True)
 
 
 if __name__ == "__main__":
     np.testing.run_module_suite()
```

### Comparing `toqito-1.0.5/tests/test_matrix_props/test_sk_norm.py` & `toqito-1.0.6/tests/test_matrix_props/test_sk_norm.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,16 +53,16 @@
     # N. Johnston.
     # Norms and Cones in the Theory of Quantum Entanglement.
     # PhD thesis (arXiv:1207.1479)
     # Proposition 5.2.10 and Table 5.1
     expected = (1 + abs(min(0, a))) / (n * (n - a))
 
     lower_bound, upper_bound = sk_operator_norm(rho, k=1)
-    np.testing.assert_equal(np.allclose(lower_bound, expected), True)
-    np.testing.assert_equal(np.allclose(upper_bound, expected), True)
+    np.testing.assert_equal(np.allclose(lower_bound, expected, atol=1e-4), True)
+    np.testing.assert_equal(np.allclose(upper_bound, expected, atol=1e-4), True)
 
 
 def test_sk_norm_hermitian_not_psd():
     """Test S(k) norm of a Hermitian but not PSD matrix."""
     e_0 = basis(2, 0)
     e_00 = np.kron(e_0, e_0)
```

### Comparing `toqito-1.0.5/tests/test_measurement_ops/test_measure.py` & `toqito-1.0.6/tests/test_measurement_ops/test_measure.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/tests/test_measurement_props/test_is_povm.py` & `toqito-1.0.6/tests/test_measurement_props/test_is_povm.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/tests/test_nonlocal_games/test_extended_nonlocal_game.py` & `toqito-1.0.6/tests/test_nonlocal_games/test_extended_nonlocal_game.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/tests/test_nonlocal_games/test_nonlocal_game.py` & `toqito-1.0.6/tests/test_nonlocal_games/test_nonlocal_game.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/tests/test_nonlocal_games/test_quantum_hedging.py` & `toqito-1.0.6/tests/test_nonlocal_games/test_quantum_hedging.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/tests/test_perms/test_antisymmetric_projection.py` & `toqito-1.0.6/tests/test_perms/test_antisymmetric_projection.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/tests/test_perms/test_perfect_matchings.py` & `toqito-1.0.6/tests/test_perms/test_perfect_matchings.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/tests/test_perms/test_permutation_operator.py` & `toqito-1.0.6/tests/test_perms/test_permutation_operator.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/tests/test_perms/test_permute_systems.py` & `toqito-1.0.6/tests/test_perms/test_permute_systems.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/tests/test_perms/test_swap.py` & `toqito-1.0.6/tests/test_perms/test_swap.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/tests/test_perms/test_swap_operator.py` & `toqito-1.0.6/tests/test_perms/test_swap_operator.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/tests/test_perms/test_symmetric_projection.py` & `toqito-1.0.6/tests/test_perms/test_symmetric_projection.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/tests/test_random/test_random_density_matrix.py` & `toqito-1.0.6/tests/test_random/test_random_density_matrix.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/tests/test_random/test_random_povm.py` & `toqito-1.0.6/tests/test_random/test_random_povm.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/tests/test_random/test_random_state_vector.py` & `toqito-1.0.6/tests/test_random/test_random_state_vector.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/tests/test_random/test_random_unitary.py` & `toqito-1.0.6/tests/test_random/test_random_unitary.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/tests/test_state_metrics/test_bures_distance.py` & `toqito-1.0.6/tests/test_state_metrics/test_bures_distance.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/tests/test_state_metrics/test_fidelity.py` & `toqito-1.0.6/tests/test_state_metrics/test_fidelity.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/tests/test_state_metrics/test_helstrom_holevo.py` & `toqito-1.0.6/tests/test_state_metrics/test_helstrom_holevo.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/tests/test_state_metrics/test_hilbert_schmidt.py` & `toqito-1.0.6/tests/test_state_metrics/test_hilbert_schmidt.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/tests/test_state_metrics/test_hilbert_schmidt_inner_product.py` & `toqito-1.0.6/tests/test_state_metrics/test_hilbert_schmidt_inner_product.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,20 @@
-#!/usr/bin/python
-# -*- coding: utf-8 -*-
 """Tests for hilbert_schmidt."""
 
 import numpy as np
 from toqito.matrices.hadamard import hadamard
 from toqito.matrices.pauli import pauli
 from toqito.random.random_unitary import random_unitary
 
 from toqito.state_metrics import hilbert_schmidt_inner_product
 
 
 def test_hilbert_schmidt_inner_product_hadamard_hadamard():
     r"""Test Hilbert-Schmidt inner product between an unitary and itself should
-  return the dimension of the space the operator acts on"""
+    return the dimension of the space the operator acts on"""
 
     hadamard_mat = hadamard(1)
     hs_ip = hilbert_schmidt_inner_product(hadamard_mat, hadamard_mat)
     np.testing.assert_equal(np.isclose(hs_ip, 2), True)
 
 
 def test_hilbert_schmidt_inner_product_is_conjugate_symmetric():
@@ -30,23 +28,22 @@
 
 
 def test_hilbert_schmidt_inner_product_linearity():
     r"""Test Hilbert-Schmidt inner product acts linearly"""
 
     rand_unitary = random_unitary(2)
     random_hermitian_operator = rand_unitary + np.conj(rand_unitary.T)
-    b_mat_1 = pauli('I')
+    b_mat_1 = pauli("I")
     b_mat_2 = 2 * b_mat_1
     beta_1 = 0.3
     beta_2 = 0.8
-    lhs = beta_1 \
-        * hilbert_schmidt_inner_product(random_hermitian_operator,
-            b_mat_1) + beta_2 \
-        * hilbert_schmidt_inner_product(random_hermitian_operator,
-            b_mat_2)
-    rhs = hilbert_schmidt_inner_product(random_hermitian_operator,
-            beta_1 * b_mat_1 + beta_2 * b_mat_2)
+    lhs = beta_1 * hilbert_schmidt_inner_product(
+        random_hermitian_operator, b_mat_1
+    ) + beta_2 * hilbert_schmidt_inner_product(random_hermitian_operator, b_mat_2)
+    rhs = hilbert_schmidt_inner_product(
+        random_hermitian_operator, beta_1 * b_mat_1 + beta_2 * b_mat_2
+    )
     np.testing.assert_equal(np.isclose(lhs, rhs), True)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     np.testing.run_module_suite()
```

### Comparing `toqito-1.0.5/tests/test_state_metrics/test_matsumoto_fidelity.py` & `toqito-1.0.6/tests/test_state_metrics/test_matsumoto_fidelity.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/tests/test_state_metrics/test_sub_fidelity.py` & `toqito-1.0.6/tests/test_state_metrics/test_sub_fidelity.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/tests/test_state_metrics/test_trace_distance.py` & `toqito-1.0.6/tests/test_state_metrics/test_trace_distance.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/tests/test_state_metrics/test_trace_norm.py` & `toqito-1.0.6/tests/test_matrix_props/test_trace_norm.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Tests for trace_norm."""
 import numpy as np
 
-from toqito.state_metrics import trace_norm
+from toqito.matrix_props import trace_norm
 from toqito.states import basis
 
 
 def test_trace_norm():
     """Test trace norm."""
     e_0, e_1 = basis(2, 0), basis(2, 1)
     e_00 = np.kron(e_0, e_0)
```

### Comparing `toqito-1.0.5/tests/test_state_ops/test_pure_to_mixed.py` & `toqito-1.0.6/tests/test_state_ops/test_pure_to_mixed.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/tests/test_state_ops/test_schmidt_decomposition.py` & `toqito-1.0.6/tests/test_state_ops/test_schmidt_decomposition.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/tests/test_state_opt/test_optimal_clone.py` & `toqito-1.0.6/tests/test_state_opt/test_optimal_clone.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/tests/test_state_opt/test_ppt_distinguishability.py` & `toqito-1.0.6/tests/test_state_opt/test_ppt_distinguishability.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/tests/test_state_opt/test_state_distinguishability.py` & `toqito-1.0.6/tests/test_state_opt/test_state_distinguishability.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/tests/test_state_opt/test_symmetric_extension_hierarchy.py` & `toqito-1.0.6/tests/test_state_opt/test_symmetric_extension_hierarchy.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/tests/test_state_props/test_concurrence.py` & `toqito-1.0.6/tests/test_state_props/test_concurrence.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/tests/test_state_props/test_entanglement_of_formation.py` & `toqito-1.0.6/tests/test_state_props/test_entanglement_of_formation.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/tests/test_state_props/test_has_symmetric_extension.py` & `toqito-1.0.6/tests/test_state_props/test_has_symmetric_extension.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/tests/test_state_props/test_in_separable_ball.py` & `toqito-1.0.6/tests/test_state_props/test_in_separable_ball.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/tests/test_state_props/test_is_ensemble.py` & `toqito-1.0.6/tests/test_state_props/test_is_ensemble.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/tests/test_state_props/test_is_mutually_orthogonal.py` & `toqito-1.0.6/tests/test_state_props/test_is_mutually_orthogonal.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/tests/test_state_props/test_is_mutually_unbiased_basis.py` & `toqito-1.0.6/tests/test_state_props/test_is_mutually_unbiased_basis.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/tests/test_state_props/test_is_npt.py` & `toqito-1.0.6/tests/test_state_props/test_is_npt.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/tests/test_state_props/test_is_ppt.py` & `toqito-1.0.6/tests/test_state_props/test_is_ppt.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/tests/test_state_props/test_is_product.py` & `toqito-1.0.6/tests/test_state_props/test_is_product.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/tests/test_state_props/test_is_pure.py` & `toqito-1.0.6/tests/test_state_props/test_is_pure.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/tests/test_state_props/test_is_separable.py` & `toqito-1.0.6/tests/test_state_props/test_is_separable.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,40 +33,41 @@
     rho = bell(0) * bell(0).conj().T
     np.testing.assert_equal(is_separable(rho), False)
 
 
 def test_ppt_small_dimensions():
     """Determined to be separable via sufficiency of the PPT criterion in small dimensions."""
     e_0, e_1, e_2 = basis(3, 0), basis(3, 1), basis(3, 2)
-    psi = 1/np.sqrt(3) * e_0 + 1/np.sqrt(3) * e_1 + 1/np.sqrt(3) * e_2
+    psi = 1 / np.sqrt(3) * e_0 + 1 / np.sqrt(3) * e_1 + 1 / np.sqrt(3) * e_2
 
     e_0, e_1 = basis(2, 0), basis(2, 1)
-    phi = np.kron((1/np.sqrt(2) * e_0 + 1/np.sqrt(2) * e_1), psi)
+    phi = np.kron((1 / np.sqrt(2) * e_0 + 1 / np.sqrt(2) * e_1), psi)
     sigma = phi * phi.conj().T
     np.testing.assert_equal(is_separable(sigma), True)
 
 
 def test_ppt_low_rank():
     """Determined to be separable via the operational criterion for low-rank operators."""
     m = 6
     n = m
     rho = random_density_matrix(m)
     u, s, v_h = np.linalg.svd(rho)
-    rho_cut = u[:, :m-1] @ np.diag(s[:m-1]) @ v_h[:m-1]
+    rho_cut = u[:, : m - 1] @ np.diag(s[: m - 1]) @ v_h[: m - 1]
     rho_cut = rho_cut / np.trace(rho_cut)
-    pt_state_alice = partial_trace(rho_cut, 2, dim=[3, 2])
+    pt_state_alice = partial_trace(rho_cut, [1], [3, 2])
 
     np.testing.assert_equal(is_density(rho_cut), True)
-    np.testing.assert_equal(is_density(pt_state_alice), True)
+    np.testing.assert_equal(is_density(np.array(pt_state_alice)), True)
     np.testing.assert_equal(
-        np.linalg.matrix_rank(rho_cut) + np.linalg.matrix_rank(pt_state_alice) <= 2 * m * n - m - n + 2,
-        True
+        np.linalg.matrix_rank(rho_cut) + np.linalg.matrix_rank(pt_state_alice)
+        <= 2 * m * n - m - n + 2,
+        True,
     )
     # TODO
-    #np.testing.assert_equal(is_separable(rho), True)
+    # np.testing.assert_equal(is_separable(rho), True)
 
 
 def test_entangled_realignment_criterion():
     """Determined to be entangled via the realignment criterion."""
     # Construct bound entangled state:
     # :math:`\rho = \frac{1}{4} \mathbb{I}_3 \otimes \mathbb{I}_3 - \sum_{i=0}^4 | \psi_i \rangle \langle \psi_i |`
     rho = np.identity(9)
@@ -78,18 +79,18 @@
 
 
 def test_entangled_cross_norm_realignment_criterion():
     """Determined to be entangled by using Theorem 1 and Remark 1 of Quantum Inf. Comput., 3:193-202, 2003."""
     p_var, a_var, b_var = 0.4, 0.8, 0.64
     rho = np.array(
         [
-            [p_var * a_var ** 2, 0, 0, p_var * a_var * b_var],
-            [0, (1 - p_var) * a_var ** 2, (1 - p_var) * a_var * b_var, 0],
-            [0, (1 - p_var) * a_var * b_var, (1 - p_var) * a_var ** 2, 0],
-            [p_var * a_var * b_var, 0, 0, p_var * a_var ** 2],
+            [p_var * a_var**2, 0, 0, p_var * a_var * b_var],
+            [0, (1 - p_var) * a_var**2, (1 - p_var) * a_var * b_var, 0],
+            [0, (1 - p_var) * a_var * b_var, (1 - p_var) * a_var**2, 0],
+            [p_var * a_var * b_var, 0, 0, p_var * a_var**2],
         ]
     )
     np.testing.assert_equal(is_separable(rho), False)
 
 
 if __name__ == "__main__":
     np.testing.run_module_suite()
```

### Comparing `toqito-1.0.5/tests/test_state_props/test_log_negativity.py` & `toqito-1.0.6/tests/test_state_props/test_log_negativity.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/tests/test_state_props/test_negativity.py` & `toqito-1.0.6/tests/test_state_props/test_negativity.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/tests/test_state_props/test_purity.py` & `toqito-1.0.6/tests/test_state_props/test_purity.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/tests/test_state_props/test_schmidt_rank.py` & `toqito-1.0.6/tests/test_state_props/test_schmidt_rank.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/tests/test_state_props/test_von_neumann_entropy.py` & `toqito-1.0.6/tests/test_state_props/test_von_neumann_entropy.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/tests/test_states/test_basis.py` & `toqito-1.0.6/tests/test_states/test_basis.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/tests/test_states/test_bell.py` & `toqito-1.0.6/tests/test_states/test_bell.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/tests/test_states/test_brauer.py` & `toqito-1.0.6/tests/test_states/test_brauer.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/tests/test_states/test_breuer.py` & `toqito-1.0.6/tests/test_states/test_breuer.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/tests/test_states/test_chessboard.py` & `toqito-1.0.6/tests/test_states/test_chessboard.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/tests/test_states/test_domino.py` & `toqito-1.0.6/tests/test_states/test_domino.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/tests/test_states/test_gen_bell.py` & `toqito-1.0.6/tests/test_states/test_gen_bell.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/tests/test_states/test_ghz.py` & `toqito-1.0.6/tests/test_states/test_ghz.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/tests/test_states/test_gisin.py` & `toqito-1.0.6/tests/test_states/test_gisin.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/tests/test_states/test_horodecki.py` & `toqito-1.0.6/tests/test_states/test_horodecki.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/tests/test_states/test_max_entangled.py` & `toqito-1.0.6/tests/test_states/test_max_entangled.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/tests/test_states/test_max_mixed.py` & `toqito-1.0.6/tests/test_states/test_max_mixed.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/tests/test_states/test_tile.py` & `toqito-1.0.6/tests/test_states/test_tile.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/tests/test_states/test_w_state.py` & `toqito-1.0.6/tests/test_states/test_w_state.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/tests/test_states/test_werner.py` & `toqito-1.0.6/tests/test_states/test_werner.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/toqito/channel_metrics/channel_fidelity.py` & `toqito-1.0.6/toqito/channel_metrics/channel_fidelity.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Compute the channel fidelity between two quantum channels."""
 import cvxpy
 import numpy as np
 
-from toqito.channels import partial_trace
+from picos import partial_trace
 
 
 def channel_fidelity(choi_1: np.ndarray, choi_2: np.ndarray) -> float:
     r"""
     Compute the channel fidelity between two quantum channels [VW20]_.
 
     Let :math:`\Phi : \text{L}(\mathcal{Y}) \rightarrow \text{L}(\mathcal{X})` and
@@ -86,12 +86,12 @@
     q_var = cvxpy.Variable((choi_dim, choi_dim), complex=True)
 
     constraints = []
     objective = cvxpy.Maximize(lam)
 
     constraints.append(cvxpy.bmat([[choi_1, q_var.H], [q_var, choi_2]]) >> 0)
 
-    constraints.append(lam * np.identity(dim) <= cvxpy.real(partial_trace(q_var, [2], [dim, dim])))
+    constraints.append(lam * np.identity(dim) <= cvxpy.real(partial_trace(q_var, [1], [dim, dim])))
 
     problem = cvxpy.Problem(objective, constraints)
 
     return problem.solve(solver="CVXOPT")
```

### Comparing `toqito-1.0.5/toqito/channel_metrics/diamond_norm.py` & `toqito-1.0.6/toqito/channel_metrics/diamond_norm.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/toqito/channel_ops/apply_channel.py` & `toqito-1.0.6/toqito/channel_ops/apply_channel.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Apply channel to an operator."""
 from __future__ import annotations
 import numpy as np
+import itertools
 
 from toqito.matrix_ops import vec
 from toqito.perms import swap
 
 
 def apply_channel(mat: np.ndarray, phi_op: np.ndarray | list[list[np.ndarray]]) -> np.ndarray:
     r"""
@@ -97,31 +98,37 @@
     # Both of the following methods of applying the superoperator are much faster than naively
     # looping through the Kraus operators or constructing eigenvectors of a Choi matrix.
 
     # The superoperator was given as a list of Kraus operators:
     if isinstance(phi_op, list):
         s_phi_op = [len(phi_op), len(phi_op[0])]
 
-        # Map is completely positive.
-        if s_phi_op[1] == 1 or (s_phi_op[0] == 1 and s_phi_op[1] > 2):
-            for i in range(s_phi_op[0]):
-                phi_op[i][1] = phi_op[i][0].conj().T
-        else:
-            for i in range(s_phi_op[0]):
-                phi_op[i][1] = phi_op[i][1].conj().T
         phi_0_list = []
         phi_1_list = []
-        for i in range(s_phi_op[0]):
-            phi_0_list.append(phi_op[i][0])
-            phi_1_list.append(phi_op[i][1])
+
+        # Map is completely positive if input is given as:
+        # 1. [K1, K2, .. Kr]
+        # 2. [[K1], [K2], .. [Kr]]
+        # 3. [[K1, K2, .. Kr]] and r > 2
+        if isinstance(phi_op[0], np.ndarray):
+            phi_0_list = phi_op
+        elif s_phi_op[1] == 1 or (s_phi_op[0] == 1 and s_phi_op[1] > 2):
+            phi_0_list = list(itertools.chain(*phi_op))
+        else:
+            # Input is given as: [[A1, B1], [A2, B2], .. [Ar, Br]]
+            phi_0_list = [k_mat[0] for k_mat in phi_op]
+            phi_1_list = [k_mat[1].conj().T for k_mat in phi_op]
+
+        if not phi_1_list:
+            phi_1_list = [k_mat.conj().T for k_mat in phi_0_list]
 
         k_1 = np.concatenate(phi_0_list, axis=1)
         k_2 = np.concatenate(phi_1_list, axis=0)
 
-        a_mat = np.kron(np.identity(len(phi_op)), mat)
+        a_mat = np.kron(np.identity(len(phi_0_list)), mat)
         return k_1 @ a_mat @ k_2
 
     # The superoperator was given as a Choi matrix:
     if isinstance(phi_op, np.ndarray):
         mat_size = np.array(list(mat.shape))
         phi_size = np.array(list(phi_op.shape)) / mat_size
 
@@ -130,13 +137,14 @@
             swap(
                 phi_op.T,
                 [1, 2],
                 [[mat_size[1], phi_size[1]], [mat_size[0], phi_size[0]]],
                 True,
             ).T,
             (int(phi_size[0] * np.prod(mat_size)), int(phi_size[1])),
+            order="F",
         )
         return a_mat @ b_mat
     raise ValueError(
         "Invalid: The variable `phi_op` must either be a list of "
         "Kraus operators or as a Choi matrix."
     )
```

### Comparing `toqito-1.0.5/toqito/channel_ops/dual_channel.py` & `toqito-1.0.6/toqito/channel_ops/dual_channel.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 """Compute the dual of a map."""
 from __future__ import annotations
 import numpy as np
 
+from toqito.helper import channel_dim
 from toqito.matrix_props import is_square
 from toqito.perms import swap
 
 
 def dual_channel(
     phi_op: np.ndarray | list[np.ndarray] | list[list[np.ndarray]], dims: list[int] = None
 ) -> np.ndarray | list[list[np.ndarray]]:
     r"""
     Compute the dual of a map (quantum channel) [WatDChan18]_.
 
     The map can be represented as a Choi matrix, with optional specification of input
-    and output dimensions. In this case the Choi matrix of the dual channel is
-    returned, obtained by swapping input and output (see :func:`toqito.perms.swap`),
-    and complex conjugating all elements.
+    and output dimensions. If the input channel maps :math:`M_{r,c}` to :math:`M_{x,y}`
+    then :code:`dim` should be the list :code:`[[r,x], [c,y]]`. If it maps :math:`M_m`
+    to :math:`M_n`, then :code:`dim` can simply be the vector :code:`[m,n]`. In this
+    case the Choi matrix of the dual channel is returned, obtained by swapping input and
+    output (see :func:`toqito.perms.swap`), and complex conjugating all elements.
 
     The map can also be represented as a list of Kraus operators.
     A list of lists, each containing two elements, corresponds to the families
     of operators :math:`\{(A_a, B_a)\}` representing the map
 
     .. math::
         \Phi(X) = \sum_a A_a X B^*_a.
@@ -52,22 +55,13 @@
             return [[a.conj().T for a in x] for x in phi_op]
         if isinstance(phi_op[0], np.ndarray):
             return [a.conj().T for a in phi_op]
 
     # If phi_op is a `ndarray`, assume it is a Choi matrix.
     if isinstance(phi_op, np.ndarray):
         if len(phi_op.shape) == 2:
-            if not is_square(phi_op):
-                raise ValueError("Invalid: `phi_op` is not a valid Choi matrix (not square).")
-            if dims is None:
-                sqr = np.sqrt(phi_op.shape[0])
-                if sqr.is_integer():
-                    dims = [int(round(sqr))] * 2
-                else:
-                    raise ValueError(
-                        "The dimensions `dims` of the input and output should be specified."
-                    )
-            return swap(phi_op.conj(), dim=dims)
+            d_in, d_out, _ = channel_dim(phi_op, dim=dims, compute_env_dim=False)
+            return swap(phi_op.conj(), dim=[[d_in[0], d_out[0]], [d_in[1], d_out[1]]])
     raise ValueError(
         "Invalid: The variable `phi_op` must either be a list of "
         "Kraus operators or as a Choi matrix."
     )
```

### Comparing `toqito-1.0.5/toqito/channel_ops/kraus_to_choi.py` & `toqito-1.0.6/toqito/channel_ops/kraus_to_choi.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Compute the Choi matrix of a list of Kraus operators."""
 import numpy as np
 
 from toqito.states import max_entangled
 from toqito.channel_ops import partial_channel
+from toqito.helper import channel_dim
 
 
 def kraus_to_choi(kraus_ops: list[list[np.ndarray]], sys: int = 2) -> np.ndarray:
     r"""
     Compute the Choi matrix of a list of Kraus operators [WatKraus18]_.
 
     The Choi matrix of the list of Kraus operators, :code:`kraus_ops`. The default convention is
@@ -57,16 +58,16 @@
         Section: "Kraus representations".
         Cambridge University Press, 2018.
 
     :param kraus_ops: A list of Kraus operators.
     :param sys: The dimension of the system (default is 2).
     :return: The corresponding Choi matrix of the provided Kraus operators.
     """
-    dim_op_1 = kraus_ops[0][0].shape[0]
-    dim_op_2 = kraus_ops[0][0].shape[1]
+    dim_in, _, _ = channel_dim(kraus_ops)
+    dim_op_1, dim_op_2 = dim_in
 
     choi_mat = partial_channel(
         max_entangled(dim_op_1, False, False) * max_entangled(dim_op_2, False, False).conj().T,
         kraus_ops,
         sys,
         np.array([[dim_op_1, dim_op_1], [dim_op_2, dim_op_2]]),
     )
```

### Comparing `toqito-1.0.5/toqito/channel_ops/partial_channel.py` & `toqito-1.0.6/toqito/channel_ops/partial_channel.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Apply channel a subsystem of an operator."""
 from __future__ import annotations
 import numpy as np
+import itertools
 
 from toqito.channel_ops import apply_channel
 from toqito.states import max_entangled
 from toqito.perms import permute_systems
 
 
 def partial_channel(
@@ -89,19 +90,27 @@
     prod_dim_c1 = int(np.prod(dim[1, : sys - 1]))
     prod_dim_r2 = int(np.prod(dim[0, sys:]))
     prod_dim_c2 = int(np.prod(dim[1, sys:]))
 
     if isinstance(phi_map, list):
         # Compute the Kraus operators on the full system.
         s_phi_1, s_phi_2 = len(phi_map), len(phi_map[0])
+        phi_list = []
+        # Map is completely positive if input is given as:
+        # 1. [K1, K2, .. Kr]
+        # 2. [[K1], [K2], .. [Kr]]
+        # 3. [[K1, K2, .. Kr]] and r > 2
+        if isinstance(phi_map[0], np.ndarray):
+            phi_list = phi_map
+        elif s_phi_2 == 1 or s_phi_1 == 1 and s_phi_2 > 2:
+            phi_list = list(itertools.chain(*phi_map))
 
-        # Map is completely positive.
-        if s_phi_2 == 1 or s_phi_1 == 1 and s_phi_2 > 2:
+        if phi_list:
             phi = []
-            for m in phi_map:
+            for m in phi_list:
                 phi.append(
                     np.kron(
                         np.kron(np.identity(prod_dim_r1), m),
                         np.identity(prod_dim_r2),
                     )
                 )
             phi_x = apply_channel(rho, phi)
@@ -130,35 +139,35 @@
     # The `phi_map` variable is provided as a Choi matrix.
     if isinstance(phi_map, np.ndarray):
         dim_phi = phi_map.shape
 
         dim = np.array(
             [
                 [
-                    prod_dim_r2,
-                    prod_dim_r2,
-                    int(dim[0, sys - 1]),
-                    int(dim_phi[0] / dim[0, sys - 1]),
                     prod_dim_r1,
                     prod_dim_r1,
+                    int(dim[0, sys - 1]),
+                    int(dim_phi[0] / dim[0, sys - 1]),
+                    prod_dim_r2,
+                    prod_dim_r2,
                 ],
                 [
-                    prod_dim_c2,
-                    prod_dim_c2,
-                    int(dim[1, sys - 1]),
-                    int(dim_phi[1] / dim[1, sys - 1]),
                     prod_dim_c1,
                     prod_dim_c1,
+                    int(dim[1, sys - 1]),
+                    int(dim_phi[1] / dim[1, sys - 1]),
+                    prod_dim_c2,
+                    prod_dim_c2,
                 ],
             ]
         )
-        psi_r1 = max_entangled(prod_dim_r2, False, False)
-        psi_c1 = max_entangled(prod_dim_c2, False, False)
-        psi_r2 = max_entangled(prod_dim_r1, False, False)
-        psi_c2 = max_entangled(prod_dim_c1, False, False)
+        psi_r1 = max_entangled(prod_dim_r1, False, False)
+        psi_c1 = max_entangled(prod_dim_c1, False, False)
+        psi_r2 = max_entangled(prod_dim_r2, False, False)
+        psi_c2 = max_entangled(prod_dim_c2, False, False)
 
         phi_map = permute_systems(
             np.kron(np.kron(psi_r1 * psi_c1.conj().T, phi_map), psi_r2 * psi_c2.conj().T),
             [1, 3, 5, 2, 4, 6],
             dim,
         )
```

### Comparing `toqito-1.0.5/toqito/channel_props/__init__.py` & `toqito-1.0.6/toqito/channel_props/__init__.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/toqito/channel_props/choi_rank.py` & `toqito-1.0.6/toqito/channel_props/choi_rank.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/toqito/channel_props/is_completely_positive.py` & `toqito-1.0.6/toqito/channel_props/is_completely_positive.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/toqito/channel_props/is_herm_preserving.py` & `toqito-1.0.6/toqito/channel_props/is_herm_preserving.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/toqito/channel_props/is_positive.py` & `toqito-1.0.6/toqito/channel_props/is_positive.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/toqito/channel_props/is_quantum_channel.py` & `toqito-1.0.6/toqito/channel_props/is_quantum_channel.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/toqito/channel_props/is_trace_preserving.py` & `toqito-1.0.6/toqito/channel_props/is_trace_preserving.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Is channel trace-preserving."""
 from __future__ import annotations
 
 import numpy as np
 
 from toqito.matrix_props import is_identity
-from toqito.channels import partial_trace
+from picos import partial_trace
 
 
 def is_trace_preserving(
     phi: np.ndarray | list[list[np.ndarray]],
     rtol: float = 1e-05,
     atol: float = 1e-08,
     sys: int | list[int] = 2,
@@ -96,9 +96,12 @@
         phi_r = [B for _, B in phi]
 
         k_l = np.concatenate(phi_l, axis=0)
         k_r = np.concatenate(phi_r, axis=0)
 
         mat = k_l.conj().T @ k_r
     else:
-        mat = partial_trace(input_mat=phi, sys=sys, dim=dim)
-    return is_identity(mat, rtol=rtol, atol=atol)
+        if dim == None:
+            mat = partial_trace(phi, [sys - 1])
+        else:
+            mat = partial_trace(phi, [sys - 1], dim)
+    return is_identity(np.array(mat), rtol=rtol, atol=atol)
```

### Comparing `toqito-1.0.5/toqito/channel_props/is_unital.py` & `toqito-1.0.6/toqito/channel_props/is_unital.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,67 +1,70 @@
 """Determine whether channel is unital."""
 from __future__ import annotations
 
 import numpy as np
 
-from toqito.channel_ops import apply_channel, kraus_to_choi
+from toqito.channel_ops import apply_channel
 from toqito.matrix_props import is_identity
+from toqito.helper import channel_dim
 
 
 def is_unital(
     phi: np.ndarray | list[list[np.ndarray]],
     rtol: float = 1e-05,
     atol: float = 1e-08,
+    dim: int | list[int] | np.ndarray = None,
 ) -> bool:
     r"""
     Determine whether the given channel is unital [WatUnital18]_.
 
     A map :math:`\Phi \in \text{T} \left(\mathcal{X}, \mathcal{Y} \right)` is *unital* if it
     holds that
 
     .. math::
         \Phi(\mathbb{I}_{\mathcal{X}}) = \mathbb{I}_{\mathcal{Y}}.
 
+    If the input channel maps :math:`M_{r,c}` to :math:`M_{x,y}` then :code:`dim` should be the
+    list :code:`[[r,x], [c,y]]`. If it maps :math:`M_m` to :math:`M_n`, then :code:`dim` can simply
+    be the vector :code:`[m,n]`.
+
     Examples
     ==========
 
     Consider the channel whose Choi matrix is the swap operator. This channel is an example of a
     unital channel.
 
     >>> from toqito.perms import swap_operator
     >>> from toqito.channel_props import is_unital
     >>>
     >>> choi = swap_operator(3)
     >>> is_unital(choi)
     True
 
-    Alternatively, the channel whose Choi matrix is the depolarizing channel is an example of a
-    non-unital channel.
+    Additionally, the channel whose Choi matrix is the depolarizing channel is another example of
+    a unital channel.
 
     >>> from toqito.channels import depolarizing
     >>> from toqito.channel_props import is_unital
     >>>
     >>> choi = depolarizing(4)
     >>> is_unital(choi)
-    False
+    True
 
     References
     ==========
     .. [WatUnital18] Watrous, John.
         "The theory of quantum information."
         Chapter: Unital channels and majorization
         Cambridge University Press, 2018.
 
     :param phi: The channel provided as either a Choi matrix or a list of Kraus operators.
     :param rtol: The relative tolerance parameter (default 1e-05).
     :param atol: The absolute tolerance parameter (default 1e-08).
+    :param dim: A scalar, vector or matrix containing the input and output dimensions of PHI.
     :return: :code:`True` if the channel is unital, and :code:`False` otherwise.
     """
-    # If the variable `phi` is provided as a list, we assume this is a list of Kraus operators.
-    if isinstance(phi, list):
-        phi = kraus_to_choi(phi)
-
-    dim = int(np.sqrt(phi.shape[0]))
+    dim_in, _, _ = channel_dim(phi, dim=dim, allow_rect=False, compute_env_dim=False)
 
     # Channel is unital if :code:`mat` is the identity matrix.
-    mat = apply_channel(np.identity(dim), phi)
+    mat = apply_channel(np.identity(dim_in), phi)
     return is_identity(mat, rtol=rtol, atol=atol)
```

### Comparing `toqito-1.0.5/toqito/channel_props/is_unitary.py` & `toqito-1.0.6/toqito/channel_props/is_unitary.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Is channel unitary."""
 from __future__ import annotations
 
 import numpy as np
 
 from toqito.channel_ops import choi_to_kraus
+from toqito.matrix_props import is_unitary as is_unitary_matrix
 
 
 def is_unitary(phi: np.ndarray | list[list[np.ndarray]]) -> bool:
     r"""
     Given a quantum channel, determine if it is unitary [WatIU18]_.
 
     Let :math:`\mathcal{X}` be a complex Euclidean space an let :math:`U \in U(\mathcal{X})` be a
@@ -64,11 +65,26 @@
 
     :param phi: The channel provided as either a Choi matrix or a list of Kraus operators.
     :return: :code:`True` if the channel is a unitary channel, and :code:`False` otherwise.
     """
     # If the variable `phi` is provided as a ndarray, we assume this is a
     # Choi matrix.
     if isinstance(phi, np.ndarray):
-        phi = choi_to_kraus(phi)
+        try:
+            phi = choi_to_kraus(phi)
+        except ValueError:
+            # if we fail to obtain a Kraus representation then input/ouput spaces might be
+            # non squares or their dimensions are not equal. Hence the channel is not unitary.
+            return False
+
+    # If there is a unique Kraus operator and it's a unitary matrix then the channel is unitary.
+    if len(phi) != 1:
+        return False
+
+    u_mat = phi[0]
+    if isinstance(phi[0], list):
+        # we enter here if phi is specified as: [[U, U]] or [[U]]
+        u_mat = phi[0][0]
+        if len(phi[0]) > 2 or (len(phi[0]) == 2 and not np.allclose(phi[0][0], phi[0][1])):
+            return False
 
-    # If the length of the list of krauss operarator is equal to one, the channel is unitary.
-    return len(phi) == 1
+    return is_unitary_matrix(u_mat)
```

### Comparing `toqito-1.0.5/toqito/channels/choi.py` & `toqito-1.0.6/toqito/channels/choi.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/toqito/channels/dephasing.py` & `toqito-1.0.6/toqito/channels/dephasing.py`

 * *Files 19% similar despite different names*

```diff
@@ -62,18 +62,18 @@
     >>> from toqito.channel_ops import apply_channel
     >>> from toqito.channels import dephasing
     >>> import numpy as np
     >>> test_input_mat = np.array(
     >>>     [[1, 2, 3, 4], [5, 6, 7, 8], [9, 10, 11, 12], [13, 14, 15, 16]]
     >>> )
     >>> apply_channel(test_input_mat, dephasing(4, 0.5))
-    [[17.5  0.   0.   0. ]
-     [ 0.  20.   0.   0. ]
-     [ 0.   0.  22.5  0. ]
-     [ 0.   0.   0.  25. ]]
+    [[ 1.   1.   1.5  2. ]
+     [ 2.5  6.   3.5  4. ]
+     [ 4.5  5.  11.   6. ]
+     [ 6.5  7.   7.5 16. ]]
 
     References
     ==========
     .. [WatDeph18] Watrous, John.
         "The theory of quantum information."
         Section: "The completely dephasing channel".
         Cambridge University Press, 2018.
```

### Comparing `toqito-1.0.5/toqito/channels/depolarizing.py` & `toqito-1.0.6/toqito/channels/depolarizing.py`

 * *Files 9% similar despite different names*

```diff
@@ -38,45 +38,45 @@
                            \end{pmatrix}
 
     corresponding to one of the Bell states. Applying the depolarizing channel to :math:`\rho` we
     have that
 
     .. math::
         \Phi(\rho) = \frac{1}{4} \begin{pmatrix}
-                                    \frac{1}{2} & 0 & 0 & \frac{1}{2} \\
-                                    0 & 0 & 0 & 0 \\
-                                    0 & 0 & 0 & 0 \\
-                                    \frac{1}{2} & 0 & 0 & \frac{1}{2}
+                                    1 & 0 & 0 & 0 \\
+                                    0 & 1 & 0 & 0 \\
+                                    0 & 0 & 1 & 0 \\
+                                    0 & 0 & 0 & 1
                                  \end{pmatrix}.
 
     This can be observed in :code:`toqito` as follows.
 
     >>> from toqito.channel_ops import apply_channel
     >>> from toqito.channels import depolarizing
     >>> import numpy as np
     >>> test_input_mat = np.array(
     >>>     [[1 / 2, 0, 0, 1 / 2], [0, 0, 0, 0], [0, 0, 0, 0], [1 / 2, 0, 0, 1 / 2]]
     >>> )
     >>> apply_channel(test_input_mat, depolarizing(4))
-    [[0.125 0.    0.    0.125]
-     [0.    0.    0.    0.   ]
-     [0.    0.    0.    0.   ]
-     [0.125 0.    0.    0.125]]
+    [[0.25 0.   0.   0.  ]
+     [0.   0.25 0.   0.  ]
+     [0.   0.   0.25 0.  ]
+     [0.   0.   0.   0.25]]
 
     >>> from toqito.channel_ops import apply_channel
     >>> from toqito.channels import depolarizing
     >>> import numpy as np
     >>> test_input_mat = np.array(
     >>>     [[1, 2, 3, 4], [5, 6, 7, 8], [9, 10, 11, 12], [13, 14, 15, 16]]
     >>> )
     >>> apply_channel(test_input_mat, depolarizing(4, 0.5))
-    [[17.125  0.25   0.375  0.5  ]
-     [ 0.625 17.75   0.875  1.   ]
-     [ 1.125  1.25  18.375  1.5  ]
-     [ 1.625  1.75   1.875 19.   ]]
+    [[ 4.75  1.    1.5   2.  ]
+     [ 2.5   7.25  3.5   4.  ]
+     [ 4.5   5.    9.75  6.  ]
+     [ 6.5   7.    7.5  12.25]]
 
 
     References
     ==========
     .. [WikDepo] Wikipedia: Quantum depolarizing channel
         https://en.wikipedia.org/wiki/Quantum_depolarizing_channel
```

### Comparing `toqito-1.0.5/toqito/channels/partial_trace.py` & `toqito-1.0.6/toqito/channels/partial_trace.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from cvxpy.expressions.variable import Variable
 from toqito.perms import permute_systems
 from toqito.helper import expr_as_np_array, np_array_as_expr
 
 
 def partial_trace(
     input_mat: np.ndarray | Variable,
-    sys: int | list[int] = 2,
+    sys: int | list[int] = [1],
     dim: int | list[int] = None,
 ) -> np.ndarray | Expression:
     r"""
     Compute the partial trace of a matrix [WikPtrace]_.
 
     The *partial trace* is defined as
 
@@ -59,30 +59,30 @@
     >>> test_input_mat = np.array(
     >>>     [[1, 2, 3, 4], [5, 6, 7, 8], [9, 10, 11, 12], [13, 14, 15, 16]]
     >>> )
     >>> partial_trace(test_input_mat)
     [[ 7, 11],
      [23, 27]]
 
-    By specifying the :code:`sys = 1` argument, we can perform the partial trace over the first
+    By specifying the :code:`sys = [0]` argument, we can perform the partial trace over the first
     subsystem (instead of the default second subsystem as done above). Performing the partial
     trace over the first subsystem yields the following matrix
 
     .. math::
         X_{pt, 1} = \begin{pmatrix}
                         12 & 14 \\
                         20 & 22
                     \end{pmatrix}
 
     >>> from toqito.channels import partial_trace
     >>> import numpy as np
     >>> test_input_mat = np.array(
     >>>     [[1, 2, 3, 4], [5, 6, 7, 8], [9, 10, 11, 12], [13, 14, 15, 16]]
     >>> )
-    >>> partial_trace(test_input_mat, 1)
+    >>> partial_trace(test_input_mat, [0])
     [[12, 14],
      [20, 22]]
 
     We can also specify both dimension and system size as :code:`list` arguments. Consider the
     following :math:`16`-by-:math:`16` matrix.
 
     >>> from toqito.channels import partial_trace
@@ -107,15 +107,15 @@
      [241 242 243 244 245 246 247 248 249 250 251 252 253 254 255 256]]
 
     We can take the partial trace on the first and third subsystems and assume that the size of
     each of the 4 systems is of dimension 2.
 
     >>> from toqito.channels import partial_trace
     >>> import numpy as np
-    >>> partial_trace(test_input_mat, [1, 3], [2, 2, 2, 2])
+    >>> partial_trace(test_input_mat, [0, 2], [2, 2, 2, 2])
     [[344, 348, 360, 364],
      [408, 412, 424, 428],
      [600, 604, 616, 620],
      [664, 668, 680, 684]])
 
     References
     ==========
@@ -155,35 +155,37 @@
             )
         dim[1] = np.round(dim[1])
         num_sys = 2
 
     prod_dim = np.prod(dim)
     if isinstance(sys, list):
         if len(sys) == 1:
-            prod_dim_sys = np.prod(dim[sys[0] - 1])
+            prod_dim_sys = np.prod(dim[sys[0]])
         else:
             prod_dim_sys = 1
             for idx in sys:
-                prod_dim_sys *= dim[idx - 1]
+                prod_dim_sys *= dim[idx]
     elif isinstance(sys, int):
-        prod_dim_sys = np.prod(dim[sys - 1])
+        prod_dim_sys = np.prod(dim[sys])
     else:
         raise ValueError(
             "Invalid: The variable `sys` must either be of type int or of a list of ints."
         )
 
     sub_prod = prod_dim / prod_dim_sys
     sub_sys_vec = prod_dim * np.ones(int(sub_prod)) / sub_prod
 
+    if isinstance(sys, list):
+        sys = np.array(sys)
     if isinstance(sys, int):
-        sys = [sys]
-    set_diff = list(set(list(range(1, num_sys + 1))) - set(sys))
+        sys = np.array([sys])
+    set_diff = list(set(list(range(1, num_sys + 1))) - set(sys + 1))
 
     perm = set_diff
-    perm.extend(sys)
+    perm.extend(sys + 1)
 
     a_mat = permute_systems(input_mat, perm, dim)
 
     ret_mat = np.reshape(
         a_mat,
         [int(sub_sys_vec[0]), int(sub_prod), int(sub_sys_vec[0]), int(sub_prod)],
         order="F",
```

### Comparing `toqito-1.0.5/toqito/channels/partial_transpose.py` & `toqito-1.0.6/toqito/channels/partial_transpose.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from cvxpy.expressions.variable import Variable
 from toqito.perms import permute_systems
 from toqito.helper import expr_as_np_array, np_array_as_expr
 
 
 def partial_transpose(
     rho: np.ndarray | Variable,
-    sys: list[int] | np.ndarray | int = 2,
+    sys: list[int] | np.ndarray | int = [1],
     dim: list[int] | np.ndarray = None,
 ) -> np.ndarray | Expression:
     r"""Compute the partial transpose of a matrix [WikPtrans]_.
 
     The *partial transpose* is defined as
 
     .. math::
@@ -153,22 +153,22 @@
         # Force dim to be a row vector.
         dim = dim.T.flatten()
         dim = np.array([dim, dim])
 
     prod_dim_r = int(np.prod(dim[0, :]))
     prod_dim_c = int(np.prod(dim[1, :]))
 
-    sub_prod_r = np.prod(dim[0, sys - 1])
-    sub_prod_c = np.prod(dim[1, sys - 1])
+    sub_prod_r = np.prod(dim[0, sys])
+    sub_prod_c = np.prod(dim[1, sys])
 
     sub_sys_vec_r = prod_dim_r * np.ones(int(sub_prod_r)) / sub_prod_r
     sub_sys_vec_c = prod_dim_c * np.ones(int(sub_prod_c)) / sub_prod_c
 
-    set_diff = list(set(list(range(1, num_sys + 1))) - set(sys))
-    perm = sys.tolist()[:]
+    set_diff = list(set(list(range(1, num_sys + 1))) - set(sys + 1))
+    perm = (sys + 1).tolist()[:]
     perm.extend(set_diff)
 
     # Permute the subsystems so that we just have to do the partial transpose
     # on the first (potentially larger) subsystem.
     rho_permuted = permute_systems(rho, perm, dim)
 
     x_tmp = np.reshape(
@@ -188,12 +188,12 @@
             int(sub_sys_vec_r[0]) * int(sub_prod_c),
             int(sub_sys_vec_c[0]) * int(sub_prod_r),
         ],
         order="F",
     )
 
     # Return the subsystems back to their original positions.
-    dim[:, sys - 1] = np.flipud(dim[:, sys - 1])
+    dim[:, sys] = np.flipud(dim[:, sys])
 
     dim = dim[:, (np.array(perm) - 1).tolist()]
 
     return permute_systems(z_tmp, perm, dim, False, True)
```

### Comparing `toqito-1.0.5/toqito/channels/realignment.py` & `toqito-1.0.6/toqito/channels/realignment.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,13 +74,14 @@
 
     # Dimension is column vector.
     if min(dim.shape) == 1:
         dim = dim[:].T[0]
         dim = np.array([dim, dim])
 
     dim_x = np.array([[dim[0][1], dim[0][0]], [dim[1][0], dim[1][1]]])
+    dim_x = np.int_(dim_x)
     dim_y = np.array([[dim[1][0], dim[0][0]], [dim[0][1], dim[1][1]]])
 
     x_tmp = swap(input_mat, [1, 2], dim, True)
-    y_tmp = partial_transpose(x_tmp, sys=1, dim=dim_x)
+    y_tmp = partial_transpose(x_tmp, [0], dim_x)
 
     return swap(y_tmp, [1, 2], dim_y, True)
```

### Comparing `toqito-1.0.5/toqito/channels/reduction.py` & `toqito-1.0.6/toqito/channels/reduction.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/toqito/helper/cvx_kron.py` & `toqito-1.0.6/toqito/helper/cvx_kron.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,15 @@
 from __future__ import annotations
 
 import numpy as np
 import cvxpy
 from cvxpy.expressions.expression import Expression
 
 
-def cvx_kron(
-    expr_1: np.ndarray | Expression, expr_2: np.ndarray | Expression
-) -> Expression:
+def cvx_kron(expr_1: np.ndarray | Expression, expr_2: np.ndarray | Expression) -> Expression:
     """
     Compute Kronecker product between CVXPY objects.
 
     By default, CVXPY does not support taking the Kronecker product when the argument on the left is
     equal to a CVXPY object and the object on the right is equal to a numpy object.
 
     At most one of :code:`expr_1` and :code:`b` may be CVXPY Variable objects.
```

### Comparing `toqito-1.0.5/toqito/helper/expr_as_np_array.py` & `toqito-1.0.6/toqito/helper/expr_as_np_array.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/toqito/helper/kp_norm.py` & `toqito-1.0.6/toqito/helper/kp_norm.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/toqito/helper/npa_hierarchy.py` & `toqito-1.0.6/toqito/helper/npa_hierarchy.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,17 +57,15 @@
 
             conf.add((cnt_a, cnt_b))
 
     return base_k, conf
 
 
 # This function generates all non - equivalent words of length up to k.
-def _gen_words(
-    k: int | str, a_out: int, a_in: int, b_out: int, b_in: int
-) -> list[tuple[Symbol]]:
+def _gen_words(k: int | str, a_out: int, a_in: int, b_out: int, b_in: int) -> list[tuple[Symbol]]:
     # remove one outcome to avoid redundancy
     # since all projectors sum to identity.
     b_symbols = [Symbol("Bob", y, b) for y in range(b_in) for b in range(b_out - 1)]
     a_symbols = [Symbol("Alice", x, a) for x in range(a_in) for a in range(a_out - 1)]
 
     words = [(Symbol(""),)]
```

### Comparing `toqito-1.0.5/toqito/helper/update_odometer.py` & `toqito-1.0.6/toqito/helper/update_odometer.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/toqito/matrices/__init__.py` & `toqito-1.0.6/toqito/matrices/__init__.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/toqito/matrices/clock.py` & `toqito-1.0.6/toqito/matrices/clock.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/toqito/matrices/cnot.py` & `toqito-1.0.6/toqito/matrices/cnot.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/toqito/matrices/fourier.py` & `toqito-1.0.6/toqito/matrices/fourier.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/toqito/matrices/gell_mann.py` & `toqito-1.0.6/toqito/matrices/gell_mann.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/toqito/matrices/gen_gell_mann.py` & `toqito-1.0.6/toqito/matrices/gen_gell_mann.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/toqito/matrices/gen_pauli.py` & `toqito-1.0.6/toqito/matrices/gen_pauli.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/toqito/matrices/hadamard.py` & `toqito-1.0.6/toqito/matrices/hadamard.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/toqito/matrices/iden.py` & `toqito-1.0.6/toqito/matrices/iden.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/toqito/matrices/pauli.py` & `toqito-1.0.6/toqito/matrices/pauli.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/toqito/matrices/shift.py` & `toqito-1.0.6/toqito/matrices/shift.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/toqito/matrices/standard_basis.py` & `toqito-1.0.6/toqito/matrices/standard_basis.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,10 +22,8 @@
     :return: A list of numpy.ndarray of shape (n, 1).
     """
     first_basis_vector = np.zeros(dim) if flatten else np.zeros((dim, 1))
     first_basis_vector[0] = 1.0
 
     # The standard_basis is obtained by cyclic permutations of the first basis
     # vector
-    return [
-        np.array([first_basis_vector[i - j] for i in range(dim)]) for j in range(dim)
-    ]
+    return [np.array([first_basis_vector[i - j] for i in range(dim)]) for j in range(dim)]
```

### Comparing `toqito-1.0.5/toqito/matrix_ops/inner_product.py` & `toqito-1.0.6/toqito/matrix_ops/inner_product.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Inner product operation"""
 import numpy as np
 
+
 def inner_product(v1: np.ndarray, v2: np.ndarray) -> float:
     r"""
     Compute the inner product :math:`\langle v_1|v_2\rangle` of two vectors [WikInner]_.
 
     The inner product is calculated as follows:
 
     .. math::
@@ -35,13 +36,13 @@
     :param args: v1 and v2, both vectors of dimenstions :math:`(n,1)` where :math:`n>1`.
     :return: The computed inner product.
     """
 
     # Check for dimensional validity
     if not (v1.shape[0] == v2.shape[0] and v1.shape[0] > 1 and len(v1.shape) == 1):
         raise ValueError("Dimension mismatch")
-    
+
     res = 0
     for i in range(v1.shape[0]):
         res += v1[i] * v2[i]
-    
-    return res
+
+    return res
```

### Comparing `toqito-1.0.5/toqito/matrix_ops/outer_product.py` & `toqito-1.0.6/toqito/matrix_ops/outer_product.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Outer product operation"""
 import numpy as np
 
+
 def outer_product(v1: np.ndarray, v2: np.ndarray) -> np.ndarray:
     r"""
     Compute the outer product :math:`|v_1\rangle\langle v_2|` of two vectors.
 
     The outer product is calculated as follows:
 
     .. math::
@@ -13,15 +14,15 @@
     Example
     ==========
 
     The outer product of the vectors :math:`v1 = \begin{pmatrix}1 \\ 2 \\ 3 \end{pmatrix}` and :math:`v2 = \begin{pmatrix}4 \\ 5 \\ 6 \ \end{pmatrix}` looks as follows:
 
     .. math::
         \left|\begin{pmatrix}1\\2\\3\end{pmatrix}\right\rangle\left\langle\begin{pmatrix}4\\5\\6\end{pmatrix}\right|=\begin{pmatrix}1\\2\\3\end{pmatrix}\begin{pmatrix}4&5&6\end{pmatrix}=\begin{pmatrix}1\times4&1\times5&1\times6\\2\times4&2\times5&2\times6\\3\times4&3\times5&3\times6\end{pmatrix}=\begin{pmatrix}4&5&6\\8&10&12\\12&15&18\end{pmatrix}
-    
+
     In :code:`toqito`, this looks like this:
 
     >>> import numpy as np
     >>> from toqito.matrix_ops import outer_product
     >>> v1, v2 = np.array([1,2,3]), np.array([4,5,6])
     >>> outer_product(v1,v2)
     [[4, 5, 6],
@@ -30,18 +31,17 @@
 
     References
     ==========
     .. [WikOuter] Wikipedia: Outer Product
         https://en.wikipedia.org/wiki/Outer_product
     :raises ValueError: Vector dimensions are mismatched.
     :param args: v1 and v2, both vectors of dimensions :math:`(n,1)` where :math:`n>1`.
-    :return: The computed outer product.
-"""
+    :return: The computed outer product."""
     # Check for dimensional validity
     if not (v1.shape[0] == v2.shape[0] and v1.shape[0] > 1 and len(v1.shape) == 1):
         raise ValueError("Dimension mismatch")
 
     res = np.ndarray((v1.shape[0], v1.shape[0]))
     for i in range(v1.shape[0]):
         for j in range(v1.shape[0]):
-            res[i,j] = v1[i] * v2[j]
-    return res
+            res[i, j] = v1[i] * v2[j]
+    return res
```

### Comparing `toqito-1.0.5/toqito/matrix_ops/tensor.py` & `toqito-1.0.6/toqito/matrix_ops/tensor.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/toqito/matrix_ops/unvec.py` & `toqito-1.0.6/toqito/matrix_ops/unvec.py`

 * *Files 5% similar despite different names*

```diff
@@ -81,9 +81,9 @@
     :param shape: The shape of the output matrix; by default, the matrix is assumed to be square.
     :return: Returns a :code:`shape[0]`-by-:code:`shape[1]` matrix.
     """
     vector = np.asarray(vector)
     if shape is None:
         dim = int(np.sqrt(vector.size))
         shape = dim, dim
-    mat = vector.reshape(*shape).T
+    mat = vector.reshape(*shape, order="F")
     return mat
```

### Comparing `toqito-1.0.5/toqito/matrix_ops/vec.py` & `toqito-1.0.6/toqito/matrix_ops/vec.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/toqito/matrix_props/__init__.py` & `toqito-1.0.6/toqito/matrix_props/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 """Properties of matrices and vectors."""
 from toqito.matrix_props.is_square import is_square
 from toqito.matrix_props.is_diagonal import is_diagonal
 from toqito.matrix_props.is_normal import is_normal
+from toqito.matrix_props.is_orthonormal import is_orthonormal
 from toqito.matrix_props.is_symmetric import is_symmetric
 from toqito.matrix_props.is_hermitian import is_hermitian
 from toqito.matrix_props.is_identity import is_identity
 from toqito.matrix_props.is_idempotent import is_idempotent
 from toqito.matrix_props.is_permutation import is_permutation
 from toqito.matrix_props.is_positive_semidefinite import is_positive_semidefinite
 from toqito.matrix_props.is_positive_definite import is_positive_definite
 from toqito.matrix_props.is_density import is_density
 from toqito.matrix_props.is_commuting import is_commuting
 from toqito.matrix_props.is_projection import is_projection
 from toqito.matrix_props.is_unitary import is_unitary
 from toqito.matrix_props.majorizes import majorizes
 from toqito.matrix_props.sk_norm import sk_operator_norm
 from toqito.matrix_props.is_block_positive import is_block_positive
-from toqito.matrix_props.is_orthonormal import is_orthonormal
+from toqito.matrix_props.is_orthonormal import is_orthonormal
+from toqito.matrix_props.trace_norm import trace_norm
+from toqito.matrix_props.is_diagonally_dominant import is_diagonally_dominant
```

### Comparing `toqito-1.0.5/toqito/matrix_props/is_block_positive.py` & `toqito-1.0.6/toqito/matrix_props/is_block_positive.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/toqito/matrix_props/is_commuting.py` & `toqito-1.0.6/toqito/matrix_props/is_commuting.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/toqito/matrix_props/is_density.py` & `toqito-1.0.6/toqito/matrix_props/is_density.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/toqito/matrix_props/is_diagonal.py` & `toqito-1.0.6/toqito/matrix_props/is_diagonal.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/toqito/matrix_props/is_hermitian.py` & `toqito-1.0.6/toqito/matrix_props/is_hermitian.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/toqito/matrix_props/is_idempotent.py` & `toqito-1.0.6/toqito/matrix_props/is_idempotent.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/toqito/matrix_props/is_identity.py` & `toqito-1.0.6/toqito/matrix_props/is_identity.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/toqito/matrix_props/is_normal.py` & `toqito-1.0.6/toqito/matrix_props/is_normal.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/toqito/matrix_props/is_permutation.py` & `toqito-1.0.6/toqito/matrix_props/is_permutation.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/toqito/matrix_props/is_positive_definite.py` & `toqito-1.0.6/toqito/matrix_props/is_positive_definite.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -63,8 +63,8 @@
             # positive-definite. It will throw an error if this is not the case
             # that we catch here.
             np.linalg.cholesky(mat)
             return True
         except np.linalg.LinAlgError:
             return False
     else:
-        return False
+        return False
```

### Comparing `toqito-1.0.5/toqito/matrix_props/is_positive_semidefinite.py` & `toqito-1.0.6/toqito/matrix_props/is_positive_semidefinite.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/toqito/matrix_props/is_projection.py` & `toqito-1.0.6/toqito/matrix_props/is_projection.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/toqito/matrix_props/is_square.py` & `toqito-1.0.6/toqito/matrix_props/is_square.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/toqito/matrix_props/is_symmetric.py` & `toqito-1.0.6/toqito/matrix_props/is_symmetric.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/toqito/matrix_props/is_unitary.py` & `toqito-1.0.6/toqito/matrix_props/is_unitary.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/toqito/matrix_props/majorizes.py` & `toqito-1.0.6/toqito/matrix_props/majorizes.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,19 +30,19 @@
     The majorization criterion says that every separable state
     :math:`\rho \in \text{D}(\mathcal{A} \otimes \mathcal{B})` is such that
     :math:`\text{Tr}_{\mathcal{B}}(\rho)` majorizes
     :math:`\text{Tr}_{\mathcal{A}}(\rho)`.
 
     >>> from toqito.matrix_props import majorizes
     >>> from toqito.states import max_entangled
-    >>> from toqito.channels import partial_trace
+    >>> from picos import partial_trace
     >>>
     >>> v_vec = max_entangled(3)
     >>> rho = v_vec * v_vec.conj().T
-    >>> majorizes(partial_trace(rho), rho)
+    >>> majorizes(partial_trace(rho, [1]), rho)
     False
 
     References
     ==========
     .. [WikMajorization] Wikipedia: Majorization
        https://en.wikipedia.org/wiki/Majorization
```

### Comparing `toqito-1.0.5/toqito/matrix_props/sk_norm.py` & `toqito-1.0.6/toqito/matrix_props/sk_norm.py`

 * *Files 1% similar despite different names*

```diff
@@ -232,17 +232,17 @@
         or (is_positive and is_trans_exact and k == 1)
     ):
         rho = cvxpy.Variable((prod_dim, prod_dim), hermitian=True, name="rho")
         objective = cvxpy.Maximize(cvxpy.real(cvxpy.trace(mat @ rho)))
 
         constraints = [rho >> 0, cvxpy.real(cvxpy.trace(rho)) <= 1]
         if k == 1:
-            constraints.append(partial_transpose(rho, 2, dim) >> 0)
+            constraints.append(partial_transpose(rho, [1], dim) >> 0)
         else:
-            constraints.append(k * cvxpy.kron(partial_trace(rho, 2, dim), np.eye(dim[1])) >> rho)
+            constraints.append(k * cvxpy.kron(partial_trace(rho, [1], dim), np.eye(dim[1])) >> rho)
 
         problem = cvxpy.Problem(objective, constraints)
         cvx_optval = problem.solve()
         if problem.status != "optimal":
             raise ValueError("Numerical problems encountered.")
 
         upper_bound = min(upper_bound, np.real(cvx_optval))
@@ -272,23 +272,23 @@
                 sym_dim = [dim[0]] + [dim[1]] * j
                 prod_sym_dim = dim[0] * (dim[1] ** j)
                 sym_proj = np.kron(np.eye(dim[0]), symmetric_projection(dim[1], j))
 
                 rho = cvxpy.Variable((prod_sym_dim, prod_sym_dim), hermitian=True, name="rho")
                 objective = cvxpy.Maximize(
                     cvxpy.real(
-                        cvxpy.trace(mat @ partial_trace(rho, list(range(3, j + 2)), sym_dim))
+                        cvxpy.trace(mat @ partial_trace(rho, list(range(2, j + 1)), sym_dim))
                     )
                 )
 
                 constraints = [
                     rho >> 0,
                     cvxpy.real(cvxpy.trace(rho)) <= 1,
                     sym_proj @ rho @ sym_proj == rho,
-                    partial_transpose(rho, list(range(1, int(np.ceil(j / 2)) + 2)), sym_dim) >> 0,
+                    partial_transpose(rho, list(range(0, int(np.ceil(j / 2)) + 1)), sym_dim) >> 0,
                 ]
 
                 problem = cvxpy.Problem(objective, constraints)
                 cvx_optval = problem.solve()
                 if problem.status != "optimal":
                     raise ValueError("Numerical problems encountered.")
```

### Comparing `toqito-1.0.5/toqito/measurement_ops/measure.py` & `toqito-1.0.6/toqito/measurement_ops/measure.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/toqito/measurement_props/is_povm.py` & `toqito-1.0.6/toqito/measurement_props/is_povm.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/toqito/nonlocal_games/extended_nonlocal_game.py` & `toqito-1.0.6/toqito/nonlocal_games/extended_nonlocal_game.py`

 * *Files 1% similar despite different names*

```diff
@@ -458,15 +458,16 @@
         referee_dim, _, alice_out, bob_out, alice_in, bob_in = self.pred_mat.shape
 
         mat = defaultdict(cvxpy.Variable)
         for x_in in range(alice_in):
             for y_in in range(bob_in):
                 mat[x_in, y_in] = cvxpy.Variable(
                     (alice_out * referee_dim, bob_out * referee_dim),
-                    name=f"K(a, b | {x_in}, {y_in})", hermitian=True,
+                    name=f"K(a, b | {x_in}, {y_in})",
+                    hermitian=True,
                 )
 
         p_win = cvxpy.Constant(0)
         for a_out in range(alice_out):
             for b_out in range(bob_out):
                 for x_in in range(alice_in):
                     for y_in in range(bob_in):
```

### Comparing `toqito-1.0.5/toqito/nonlocal_games/nonlocal_game.py` & `toqito-1.0.6/toqito/nonlocal_games/nonlocal_game.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/toqito/nonlocal_games/quantum_hedging.py` & `toqito-1.0.6/toqito/nonlocal_games/quantum_hedging.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,17 +76,15 @@
 
         :param q_a: The fixed SDP variable.
         :param num_reps: The number of parallel repetitions.
         """
         self._q_a = q_a
         self._num_reps = num_reps
 
-        self._sys = list(range(1, 2 * self._num_reps, 2))
-        if len(self._sys) == 1:
-            self._sys = self._sys[0]
+        self._sys = list(range(0, 2 * self._num_reps - 1, 2))
 
         self._dim = 2 * np.ones((1, 2 * self._num_reps)).astype(int).flatten()
         self._dim = self._dim.tolist()
 
         # For the dual problem, the following unitary operator is used to
         # permute the subsystems of Alice and Bob which is defined by the
         # action:
```

### Comparing `toqito-1.0.5/toqito/nonlocal_games/xor_game.py` & `toqito-1.0.6/toqito/nonlocal_games/xor_game.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,183 +2,183 @@
 import cvxpy
 import numpy as np
 
 from toqito.nonlocal_games.nonlocal_game import NonlocalGame
 
 
 class XORGame:
-	r"""
-	Create two-player XOR game object.
+    r"""
+    Create two-player XOR game object.
 
-	Calculates the optimal probability that Alice and Bob win the game if they
-	are allowed to determine a join strategy beforehand, but not allowed to
-	communicate during the game itself.
-
-	The quantum value of an XOR game can be solved via the semidefinite program
-	from [CHTW04]_.
-
-	This function is adapted from the QETLAB package.
-
-	Examples
-	==========
-
-	The CHSH game
-
-	The CHSH game is a two-player nonlocal game with the following probability
-	distribution and question and answer sets [CSUU08]_.
-
-	.. math::
-		\begin{equation}
-			\begin{aligned} \pi(x,y) = \frac{1}{4}, \qquad (x,y) \in
-							\Sigma_A \times
-				\Sigma_B, \qquad \text{and} \qquad (a, b) \in \Gamma_A \times
-				\Gamma_B,
-			\end{aligned}
-		\end{equation}
-
-	where
-
-	.. math::
-		\begin{equation}
-			\Sigma_A = \{0, 1\}, \quad \Sigma_B = \{0, 1\}, \quad \Gamma_A =
-			\{0,1\}, \quad \text{and} \quad \Gamma_B = \{0, 1\}.
-		\end{equation}
-
-	Alice and Bob win the CHSH game if and only if the following equation is
-	satisfied
-
-	.. math::
-		\begin{equation}
-		a \oplus b = x \land y.
-		\end{equation}
-
-	Recall that :math:`\oplus` refers to the XOR operation.
-
-	The optimal quantum value of CHSH is :math:`\cos(\pi/8)^2 \approx 0.8536`
-	where the optimal classical value is :math:`3/4`.
-
-	In order to specify the CHSH game, we can define the probability matrix and
-	predicate matrix for the CHSH game as `numpy` arrays as follows.
-
-	>>> import numpy as np
-	>>> prob_mat = np.array([[1 / 4, 1 / 4], [1 / 4, 1 / 4]])
-	>>> pred_mat = np.array([[0, 0], [0, 1]])
-
-	In `toqito`, we can calculate both the quantum and classical value of the
-	CHSH game as follows.
-
-	>>> import numpy as np
-	>>> from toqito.nonlocal_games.xor_game import XORGame
-	>>> chsh = XORGame(prob_mat, pred_mat)
-	>>> chsh.quantum_value()
-	0.8535533885683664
-	>>>
-	>>> chsh.classical_value()
-	0.75
-
-	The odd cycle game
-
-	The odd cycle game is another XOR game [CHTW04]_. For this game, we can
-	specify the probability and predicate matrices as follows.
-
-	>>> prob_mat = np.array(
-	>>> [
-	>>>     [0.1, 0.1, 0, 0, 0],
-	>>>     [0, 0.1, 0.1, 0, 0],
-	>>>     [0, 0, 0.1, 0.1, 0],
-	>>>     [0, 0, 0, 0.1, 0.1],
-	>>>     [0.1, 0, 0, 0, 0.1],
-	>>> ]
-	>>> )
-	>>> pred_mat = np.array(
-	>>> [
-	>>>     [0, 1, 0, 0, 0],
-	>>>     [0, 0, 1, 0, 0],
-	>>>     [0, 0, 0, 1, 0],
-	>>>     [0, 0, 0, 0, 1],
-	>>>     [1, 0, 0, 0, 0],
-	>>> ]
-	>>> )
-
-	In :code:`toqito`, we can calculate both the quantum and classical value of
-	the odd cycle game as follows.
-
-	>>> import numpy as np
-	>>> from toqito.nonlocal_games.xor_game import XORGame
-	>>> odd_cycle = XORGame(prob_mat, pred_mat)
-	>>> odd_cycle.quantum_value()
-	0.9755282544736033
-	>>> odd_cycle.classical_value()
-	0.9
-
-	References
-	==========
-	.. [CSUU08] Richard Cleve, William Slofstra, Falk Unger, Sarvagya Upadhyay
-		"Strong parallel repetition theorem for quantum XOR proof systems",
-		2008,
-		https://arxiv.org/abs/quant-ph/0608146
-
-	.. [CHTW04] Richard Cleve, Peter Hoyer, Ben Toner, John Watrous
-		"Consequences and limits of nonlocal strategies."
-		Proceedings. 19th IEEE Annual Conference on Computational Complexity,
-		IEEE, 2004.
-		https://arxiv.org/abs/quant-ph/0404076
-	"""
-
-	def __init__(
-		self,
-		prob_mat: np.ndarray,
-		pred_mat: np.ndarray,
-		reps: int = 1,
-		tol: float = None,
-	) -> None:
-		"""
-		Construct XOR game object.
-
-		:raises ValueError: If dimension of probability matrix is not equal to
-							dimension of predicate matrix.
-		:param prob_mat: A matrix whose (q_0, q_1)-entry gives the probability that
-					 the referee will give Alice the value `q_0` and Bob the
-					 value `q_1`.
-		:param pred_mat: A binary matrix whose (q_0, q_1)-entry indicates the
-					 winning choice (either 0 or 1) when Alice and Bob receive
-					 values `q_0` and `q_1` from the referee.
-		:param tol: The error tolerance for the value.
-		"""
-		self.prob_mat = prob_mat
-		self.pred_mat = pred_mat
-		self.reps = reps
-
-		q_0, q_1 = self.prob_mat.shape
-		if tol is None:
-			self.tol = np.finfo(float).eps * q_0**2 * q_1**2
-		else:
-			self.tol = tol
-
-		# Perform some basic error checking to ensure the probability and
-		# predicate matrices are well-defined.
-		if (q_0, q_1) != self.pred_mat.shape:
-			raise ValueError(
-				"Invalid: The matrices `prob_mat` and `pred_mat` must"
-				" be matrices of the same size."
-			)
-		if -np.min(np.min(self.prob_mat)) > self.tol:
-			raise ValueError(
-				"Invalid: The variable `prob_mat` must be a "
-				"probability matrix: its entries must be "
-				"non-negative."
-			)
-		if np.abs(np.sum(np.sum(self.prob_mat)) - 1) > self.tol:
-			raise ValueError(
-				"Invalid: The variable `prob_mat` must be a "
-				"probability matrix: its entries must sum to 1."
-			)
+    Calculates the optimal probability that Alice and Bob win the game if they
+    are allowed to determine a join strategy beforehand, but not allowed to
+    communicate during the game itself.
+
+    The quantum value of an XOR game can be solved via the semidefinite program
+    from [CHTW04]_.
+
+    This function is adapted from the QETLAB package.
+
+    Examples
+    ==========
+
+    The CHSH game
+
+    The CHSH game is a two-player nonlocal game with the following probability
+    distribution and question and answer sets [CSUU08]_.
+
+    .. math::
+            \begin{equation}
+                    \begin{aligned} \pi(x,y) = \frac{1}{4}, \qquad (x,y) \in
+                                                    \Sigma_A \times
+                            \Sigma_B, \qquad \text{and} \qquad (a, b) \in \Gamma_A \times
+                            \Gamma_B,
+                    \end{aligned}
+            \end{equation}
+
+    where
+
+    .. math::
+            \begin{equation}
+                    \Sigma_A = \{0, 1\}, \quad \Sigma_B = \{0, 1\}, \quad \Gamma_A =
+                    \{0,1\}, \quad \text{and} \quad \Gamma_B = \{0, 1\}.
+            \end{equation}
+
+    Alice and Bob win the CHSH game if and only if the following equation is
+    satisfied
+
+    .. math::
+            \begin{equation}
+            a \oplus b = x \land y.
+            \end{equation}
+
+    Recall that :math:`\oplus` refers to the XOR operation.
+
+    The optimal quantum value of CHSH is :math:`\cos(\pi/8)^2 \approx 0.8536`
+    where the optimal classical value is :math:`3/4`.
+
+    In order to specify the CHSH game, we can define the probability matrix and
+    predicate matrix for the CHSH game as `numpy` arrays as follows.
+
+    >>> import numpy as np
+    >>> prob_mat = np.array([[1 / 4, 1 / 4], [1 / 4, 1 / 4]])
+    >>> pred_mat = np.array([[0, 0], [0, 1]])
+
+    In `toqito`, we can calculate both the quantum and classical value of the
+    CHSH game as follows.
+
+    >>> import numpy as np
+    >>> from toqito.nonlocal_games.xor_game import XORGame
+    >>> chsh = XORGame(prob_mat, pred_mat)
+    >>> chsh.quantum_value()
+    0.8535533885683664
+    >>>
+    >>> chsh.classical_value()
+    0.75
+
+    The odd cycle game
+
+    The odd cycle game is another XOR game [CHTW04]_. For this game, we can
+    specify the probability and predicate matrices as follows.
+
+    >>> prob_mat = np.array(
+    >>> [
+    >>>     [0.1, 0.1, 0, 0, 0],
+    >>>     [0, 0.1, 0.1, 0, 0],
+    >>>     [0, 0, 0.1, 0.1, 0],
+    >>>     [0, 0, 0, 0.1, 0.1],
+    >>>     [0.1, 0, 0, 0, 0.1],
+    >>> ]
+    >>> )
+    >>> pred_mat = np.array(
+    >>> [
+    >>>     [0, 1, 0, 0, 0],
+    >>>     [0, 0, 1, 0, 0],
+    >>>     [0, 0, 0, 1, 0],
+    >>>     [0, 0, 0, 0, 1],
+    >>>     [1, 0, 0, 0, 0],
+    >>> ]
+    >>> )
+
+    In :code:`toqito`, we can calculate both the quantum and classical value of
+    the odd cycle game as follows.
+
+    >>> import numpy as np
+    >>> from toqito.nonlocal_games.xor_game import XORGame
+    >>> odd_cycle = XORGame(prob_mat, pred_mat)
+    >>> odd_cycle.quantum_value()
+    0.9755282544736033
+    >>> odd_cycle.classical_value()
+    0.9
+
+    References
+    ==========
+    .. [CSUU08] Richard Cleve, William Slofstra, Falk Unger, Sarvagya Upadhyay
+            "Strong parallel repetition theorem for quantum XOR proof systems",
+            2008,
+            https://arxiv.org/abs/quant-ph/0608146
+
+    .. [CHTW04] Richard Cleve, Peter Hoyer, Ben Toner, John Watrous
+            "Consequences and limits of nonlocal strategies."
+            Proceedings. 19th IEEE Annual Conference on Computational Complexity,
+            IEEE, 2004.
+            https://arxiv.org/abs/quant-ph/0404076
+    """
+
+    def __init__(
+        self,
+        prob_mat: np.ndarray,
+        pred_mat: np.ndarray,
+        reps: int = 1,
+        tol: float = None,
+    ) -> None:
+        """
+        Construct XOR game object.
+
+        :raises ValueError: If dimension of probability matrix is not equal to
+                                                dimension of predicate matrix.
+        :param prob_mat: A matrix whose (q_0, q_1)-entry gives the probability that
+                                 the referee will give Alice the value `q_0` and Bob the
+                                 value `q_1`.
+        :param pred_mat: A binary matrix whose (q_0, q_1)-entry indicates the
+                                 winning choice (either 0 or 1) when Alice and Bob receive
+                                 values `q_0` and `q_1` from the referee.
+        :param tol: The error tolerance for the value.
+        """
+        self.prob_mat = prob_mat
+        self.pred_mat = pred_mat
+        self.reps = reps
+
+        q_0, q_1 = self.prob_mat.shape
+        if tol is None:
+            self.tol = np.finfo(float).eps * q_0**2 * q_1**2
+        else:
+            self.tol = tol
+
+        # Perform some basic error checking to ensure the probability and
+        # predicate matrices are well-defined.
+        if (q_0, q_1) != self.pred_mat.shape:
+            raise ValueError(
+                "Invalid: The matrices `prob_mat` and `pred_mat` must"
+                " be matrices of the same size."
+            )
+        if -np.min(np.min(self.prob_mat)) > self.tol:
+            raise ValueError(
+                "Invalid: The variable `prob_mat` must be a "
+                "probability matrix: its entries must be "
+                "non-negative."
+            )
+        if np.abs(np.sum(np.sum(self.prob_mat)) - 1) > self.tol:
+            raise ValueError(
+                "Invalid: The variable `prob_mat` must be a "
+                "probability matrix: its entries must sum to 1."
+            )
 
-	def quantum_value(self) -> float:
-		r"""
+    def quantum_value(self) -> float:
+        r"""
 		Compute the quantum value of the XOR game.
 
 		To obtain the quantum value of the XOR game, we calculate the following
 		simplified dual problem of the semidefinite program from the set of
 		notes: https://cs.uwaterloo.ca/~watrous/CS867.Winter2017/Notes/06.pdf
 
 		.. math::
@@ -202,119 +202,76 @@
 			D(x,y) = \pi(x, y) (-1)^{f(x,y)}
 
 		In other words, :math:`\pi(x, y)` corresponds to :code:`prob_mat[x, y]`,
 		and :math:`f(x,y)` corresponds to :code:`pred_mat[x, y]`.
 
 		:return: A value between [0, 1] representing the quantum value.
 		"""
-		alice_in, bob_in = self.prob_mat.shape
-		d_mat = np.zeros([alice_in, bob_in])
-
-		for x_alice in range(alice_in):
-			for y_bob in range(bob_in):
-				d_mat[x_alice, y_bob] = self.prob_mat[x_alice, y_bob] * (-1) ** (
-					self.pred_mat[x_alice, y_bob]
-				)
-
-		u_vec = cvxpy.Variable(alice_in, complex=False)
-		v_vec = cvxpy.Variable(bob_in, complex=False)
-
-		objective = cvxpy.Minimize(cvxpy.sum(u_vec) + cvxpy.sum(v_vec))
-		constraints = [
-			cvxpy.bmat(
-				[
-					[cvxpy.diag(u_vec), -d_mat],
-					[np.negative(d_mat.conj().T), cvxpy.diag(v_vec)],
-				]
-			)
-			>> 0
-		]
-
-		problem = cvxpy.Problem(objective, constraints)
-		problem.solve()
-
-		if self.reps == 1:
-			return np.real(problem.value) / 4 + 1 / 2
-		# It holds from (https://arxiv.org/abs/quant-ph/0608146) that the
-		# quantum value of any XOR game obeys strong parallel repetition. That
-		# is, it holds that:
-		#   \omega^*(G^{^n}) = \omega^*(G)^n,
-		# where G^{^n} denotes playing the game G n-times.
-		return (np.real(problem.value) / 4 + 1 / 2) ** self.reps
-
-	def classical_value(self) -> float:
-		"""
-		Compute the classical value of the XOR game.
-
-		:raises ValueError: Does not support parallel repetitions.
-		:return: A value between [0, 1] representing the classical value.
-		"""
-		if self.reps == 1:
-			q_0, q_1 = self.prob_mat.shape
+        alice_in, bob_in = self.prob_mat.shape
+        d_mat = np.zeros([alice_in, bob_in])
 
-			# At worst, out winning probability is 0. Now, try to improve.
-			val = 0
-
-			# Find the maximum probability of winning (this is NP-hard, so don't
-			# expect an easy way to do it: just loop over all strategies.
-
-			# Loop over Alice's answers
-			for a_ans in range(2**q_0):
-				# Loop over Bob's answers:
-				for b_ans in range(2**q_1):
-					a_vec = (a_ans >> np.arange(q_0)) & 1
-					b_vec = (b_ans >> np.arange(q_1)) & 1
-
-					# Now compute the winning probability under this strategy:
-					# XOR together Alice's responses and Bob's responses, then
-					# check where the XORed value equals the value in the given
-					# matrix. Where the values match, multiply by the
-					# probability of getting that pair of questions (i.e.,
-					# multiply by the probability of getting that pair of
-					# questions (i.e., multiply entry-wise by P) and then sum
-					# over the rows and columns.
-					classical_strategy = np.mod(
-						np.multiply(a_vec.conj().T.reshape(-1, 1), np.ones((1, q_1)))
-						+ np.multiply(np.ones((q_0, 1)), b_vec),
-						2,
-					)
-					p_win = np.sum(
-						np.sum(np.multiply(classical_strategy == self.pred_mat, self.prob_mat))
-					)
-					# Is this strategy better than other ones tried so far?
-					val = max(val, p_win)
-
-					# Already optimal? Quit.
-					if val >= 1 - self.tol:
-						return val
-			return val
-		raise ValueError(
-			"Error: toqito currently does not support "
-			"multiple repetitions for the classical value of "
-			"a nonlocal game."
-		)
-	
-	def nonsignaling_value(self) -> float:
-		"""
-		Compute the nonsignaling value of an XOR game by calling the exising function in the :code:`NonlocalGame` class.
-		
-		:return: A value between [0, 1] representing the nonsignaling value.
-		"""
-		return self.to_nonlocal_game().nonsignaling_value()
-	
-	def to_nonlocal_game(self) -> NonlocalGame:
-		"""
-		Given an XOR game, compute a predicate matrix representing the more generic :code:`NonlocalGame` equivalent.
-
-		:return: A :code:`NonlocalGame` object equivalent to the XOR game.
-		"""
-		q_0, q_1 = self.prob_mat.shape
-		xor_pred_mat = self.pred_mat
-		nlg_pred_mat = np.ndarray((2, 2, q_0, q_1))
-
-		for a in range(2):
-			for b in range(2):
-				for x in range(q_0):
-					for y in range(q_1):
-						nlg_pred_mat[a, b, x, y] = xor_pred_mat[x, y] == a ^ b
+        for x_alice in range(alice_in):
+            for y_bob in range(bob_in):
+                d_mat[x_alice, y_bob] = self.prob_mat[x_alice, y_bob] * (-1) ** (
+                    self.pred_mat[x_alice, y_bob]
+                )
+
+        u_vec = cvxpy.Variable(alice_in, complex=False)
+        v_vec = cvxpy.Variable(bob_in, complex=False)
+
+        objective = cvxpy.Minimize(cvxpy.sum(u_vec) + cvxpy.sum(v_vec))
+        constraints = [
+            cvxpy.bmat(
+                [
+                    [cvxpy.diag(u_vec), -d_mat],
+                    [np.negative(d_mat.conj().T), cvxpy.diag(v_vec)],
+                ]
+            )
+            >> 0
+        ]
+
+        problem = cvxpy.Problem(objective, constraints)
+        problem.solve()
+
+        if self.reps == 1:
+            return np.real(problem.value) / 4 + 1 / 2
+        # It holds from (https://arxiv.org/abs/quant-ph/0608146) that the
+        # quantum value of any XOR game obeys strong parallel repetition. That
+        # is, it holds that:
+        #   \omega^*(G^{^n}) = \omega^*(G)^n,
+        # where G^{^n} denotes playing the game G n-times.
+        return (np.real(problem.value) / 4 + 1 / 2) ** self.reps
+
+    def classical_value(self) -> float:
+        """
+        Compute the classical value of the XOR game.
+
+        :return: A value between [0, 1] representing the classical value.
+        """
+
+        return self.to_nonlocal_game().classical_value()
+
+    def nonsignaling_value(self) -> float:
+        """
+        Compute the nonsignaling value of an XOR game by calling the exising function in the :code:`NonlocalGame` class.
+
+        :return: A value between [0, 1] representing the nonsignaling value.
+        """
+        return self.to_nonlocal_game().nonsignaling_value()
+
+    def to_nonlocal_game(self) -> NonlocalGame:
+        """
+        Given an XOR game, compute a predicate matrix representing the more generic :code:`NonlocalGame` equivalent.
+
+        :return: A :code:`NonlocalGame` object equivalent to the XOR game.
+        """
+        q_0, q_1 = self.prob_mat.shape
+        xor_pred_mat = self.pred_mat
+        nlg_pred_mat = np.ndarray((2, 2, q_0, q_1))
+
+        for a in range(2):
+            for b in range(2):
+                for x in range(q_0):
+                    for y in range(q_1):
+                        nlg_pred_mat[a, b, x, y] = xor_pred_mat[x, y] == a ^ b
 
-		return NonlocalGame(self.prob_mat, nlg_pred_mat, reps=self.reps)
+        return NonlocalGame(self.prob_mat, nlg_pred_mat, reps=self.reps)
```

### Comparing `toqito-1.0.5/toqito/perms/__init__.py` & `toqito-1.0.6/toqito/perms/__init__.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/toqito/perms/antisymmetric_projection.py` & `toqito-1.0.6/toqito/perms/antisymmetric_projection.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/toqito/perms/perfect_matchings.py` & `toqito-1.0.6/toqito/perms/perfect_matchings.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/toqito/perms/perm_sign.py` & `toqito-1.0.6/toqito/perms/perm_sign.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/toqito/perms/permutation_operator.py` & `toqito-1.0.6/toqito/perms/permutation_operator.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/toqito/perms/permute_systems.py` & `toqito-1.0.6/toqito/perms/permute_systems.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 from toqito.matrix_ops import vec
 
 
 def permute_systems(
     input_mat: np.ndarray,
     perm: np.ndarray | list[int],
-    dim: np.ndarray |list[int] = None,
+    dim: np.ndarray | list[int] = None,
     row_only: bool = False,
     inv_perm: bool = False,
 ) -> np.ndarray:
     r"""
     Permute subsystems within a state or operator.
 
     Permutes the order of the subsystems of the vector or matrix :code:`input_mat` according to the
```

### Comparing `toqito-1.0.5/toqito/perms/swap.py` & `toqito-1.0.6/toqito/perms/swap.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/toqito/perms/swap_operator.py` & `toqito-1.0.6/toqito/perms/swap_operator.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/toqito/perms/symmetric_projection.py` & `toqito-1.0.6/toqito/perms/symmetric_projection.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/toqito/perms/unique_perms.py` & `toqito-1.0.6/toqito/perms/unique_perms.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/toqito/random/random_density_matrix.py` & `toqito-1.0.6/toqito/random/random_density_matrix.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/toqito/random/random_ginibre.py` & `toqito-1.0.6/toqito/random/random_ginibre.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/toqito/random/random_povm.py` & `toqito-1.0.6/toqito/random/random_povm.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/toqito/random/random_state_vector.py` & `toqito-1.0.6/toqito/random/random_state_vector.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/toqito/random/random_unitary.py` & `toqito-1.0.6/toqito/random/random_unitary.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/toqito/state_metrics/__init__.py` & `toqito-1.0.6/toqito/state_metrics/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Distance metrics for quantum states."""
-from toqito.state_metrics.trace_norm import trace_norm
 from toqito.state_metrics.hilbert_schmidt import hilbert_schmidt
 from toqito.state_metrics.hilbert_schmidt_inner_product import hilbert_schmidt_inner_product
 from toqito.state_metrics.helstrom_holevo import helstrom_holevo
 from toqito.state_metrics.fidelity import fidelity
+from toqito.state_metrics.fidelity_of_separability import fidelity_of_separability
 from toqito.state_metrics.sub_fidelity import sub_fidelity
 from toqito.state_metrics.trace_distance import trace_distance
 from toqito.state_metrics.bures_distance import bures_distance
+from toqito.state_metrics.bures_angle import bures_angle
 from toqito.state_metrics.matsumoto_fidelity import matsumoto_fidelity
```

### Comparing `toqito-1.0.5/toqito/state_metrics/bures_distance.py` & `toqito-1.0.6/toqito/state_metrics/bures_distance.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/toqito/state_metrics/fidelity.py` & `toqito-1.0.6/toqito/state_metrics/fidelity.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/toqito/state_metrics/helstrom_holevo.py` & `toqito-1.0.6/toqito/state_metrics/helstrom_holevo.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """Helstrom-Holevo metric."""
 import numpy as np
 
-from toqito.matrix_props import is_density
-from toqito.state_metrics import trace_norm
+from toqito.matrix_props import is_density, trace_norm
 
 
 def helstrom_holevo(rho: np.ndarray, sigma: np.ndarray) -> float:
     r"""
     Compute the Helstrom-Holevo distance between density matrices [WikHeHo]_.
 
     In general, the best success probability to discriminate two mixed states represented by
```

### Comparing `toqito-1.0.5/toqito/state_metrics/hilbert_schmidt.py` & `toqito-1.0.6/toqito/state_metrics/hilbert_schmidt.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/toqito/state_metrics/hilbert_schmidt_inner_product.py` & `toqito-1.0.6/toqito/state_metrics/hilbert_schmidt_inner_product.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Hilbert-Schmidt Inner Product."""
 import numpy as np
 
+
 def hilbert_schmidt_inner_product(a_mat: np.ndarray, b_mat: np.ndarray) -> complex:
     r"""
     Compute the Hilbert-Schmidt inner product between two matrices [WikHSO].
 
     The Hilbert-Schmidt inner product between :math:`a_mat` and :math:`b_mat` is
     defined as
```

### Comparing `toqito-1.0.5/toqito/state_metrics/matsumoto_fidelity.py` & `toqito-1.0.6/toqito/state_metrics/matsumoto_fidelity.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/toqito/state_metrics/sub_fidelity.py` & `toqito-1.0.6/toqito/state_metrics/sub_fidelity.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/toqito/state_metrics/trace_distance.py` & `toqito-1.0.6/toqito/state_metrics/trace_distance.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """Trace distance metric."""
 import numpy as np
 
-from toqito.matrix_props import is_density
-from toqito.state_metrics import trace_norm
+from toqito.matrix_props import is_density, trace_norm
 
 
 def trace_distance(rho: np.ndarray, sigma: np.ndarray) -> float:
     r"""
     Compute the trace distance between density operators `rho` and `sigma`.
 
     The trace distance between :math:`\rho` and :math:`\sigma` is defined as
```

### Comparing `toqito-1.0.5/toqito/state_metrics/trace_norm.py` & `toqito-1.0.6/toqito/matrix_props/trace_norm.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Trace norm metric."""
 import numpy as np
 
 
 def trace_norm(rho: np.ndarray) -> float:
     r"""
-    Compute the trace norm of the state [WikTn]_.
+    Compute the trace norm of the state [WikTn]_
+    as well as the operator 1-norm when inputting an operator.
 
     The trace norm :math:`||\rho||_1` of a density matrix :math:`\rho` is the sum of the singular
     values of :math:`\rho`. The singular values are the roots of the eigenvalues of
     :math:`\rho \rho^*`.
 
     Examples
     ==========
```

### Comparing `toqito-1.0.5/toqito/state_ops/pure_to_mixed.py` & `toqito-1.0.6/toqito/state_ops/pure_to_mixed.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/toqito/state_ops/schmidt_decomposition.py` & `toqito-1.0.6/toqito/state_ops/schmidt_decomposition.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/toqito/state_opt/optimal_clone.py` & `toqito-1.0.6/toqito/state_opt/optimal_clone.py`

 * *Files 2% similar despite different names*

```diff
@@ -156,14 +156,15 @@
 
     :return: The optimal value of performing a counterfeit attack.
     """
     num_spaces = 3
 
     sys = list(range(1, num_spaces * num_reps))
     sys = [elem for elem in sys if elem % num_spaces != 0]
+    sys = [elem - 1 for elem in sys]
 
     # The dimension of each subsystem is assumed to be of dimension 2.
     dim = 2 * np.ones((1, num_spaces * num_reps)).astype(int).flatten()
     dim = dim.tolist()
 
     x_var = cvxpy.Variable((8**num_reps, 8**num_reps), hermitian=True)
     if num_reps == 1:
```

### Comparing `toqito-1.0.5/toqito/state_opt/ppt_distinguishability.py` & `toqito-1.0.6/toqito/state_opt/ppt_distinguishability.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/toqito/state_opt/state_distinguishability.py` & `toqito-1.0.6/toqito/state_opt/state_distinguishability.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/toqito/state_opt/state_helper.py` & `toqito-1.0.6/toqito/state_opt/state_helper.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/toqito/state_opt/symmetric_extension_hierarchy.py` & `toqito-1.0.6/toqito/state_opt/symmetric_extension_hierarchy.py`

 * *Files 1% similar despite different names*

```diff
@@ -171,31 +171,32 @@
         if np.abs(dim[1] - np.round(dim[1])) >= 2 * dim_xy * np.finfo(float).eps:
             raise ValueError("If `dim` is a scalar, it must evenly divide the length of the state.")
         dim[1] = int(np.round(dim[1]))
 
     dim_x, dim_y = int(dim[0]), int(dim[1])
 
     dim_list = [dim_x] + [dim_y] * level
+    dim_list = np.int_(dim_list)
     # The `sys_list` variable contains the numbering pertaining to the symmetrically extended
     # spaces.
-    sys_list = list(range(3, 3 + level - 1))
+    sys_list = list(range(2, 2 + level - 1))
     sym = symmetric_projection(dim_y, level)
 
     dim_xyy = np.prod(dim_list)
     for k, _ in enumerate(states):
         meas.append(cvxpy.Variable((dim_xy, dim_xy), PSD=True))
         x_var.append(cvxpy.Variable((dim_xyy, dim_xyy), PSD=True))
         constraints.append(partial_trace(x_var[k], sys_list, dim_list) == meas[k])
         constraints.append(
             np.kron(np.identity(dim_x), sym) @ x_var[k] @ np.kron(np.identity(dim_x), sym)
             == x_var[k]
         )
-        constraints.append(partial_transpose(x_var[k], 1, dim_list) >> 0)
+        constraints.append(partial_transpose(x_var[k], [0], dim_list) >> 0)
         for sys in range(level - 1):
-            constraints.append(partial_transpose(x_var[k], sys + 3, dim_list) >> 0)
+            constraints.append(partial_transpose(x_var[k], [sys + 2], dim_list) >> 0)
 
         obj_func.append(probs[k] * cvxpy.trace(states[k].conj().T @ meas[k]))
 
     constraints.append(sum(meas) == np.identity(dim_xy))
 
     objective = cvxpy.Maximize(sum(obj_func))
     problem = cvxpy.Problem(objective, constraints)
```

### Comparing `toqito-1.0.5/toqito/state_props/__init__.py` & `toqito-1.0.6/toqito/state_props/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,9 +12,10 @@
 from toqito.state_props.log_negativity import log_negativity
 from toqito.state_props.purity import purity
 from toqito.state_props.schmidt_rank import schmidt_rank
 from toqito.state_props.von_neumann_entropy import von_neumann_entropy
 from toqito.state_props.entanglement_of_formation import entanglement_of_formation
 from toqito.state_props.l1_norm_coherence import l1_norm_coherence
 from toqito.state_props.in_separable_ball import in_separable_ball
+from toqito.state_props.is_separable import is_separable
 from toqito.state_props.has_symmetric_extension import has_symmetric_extension
 from toqito.state_props.sk_vec_norm import sk_vector_norm
```

### Comparing `toqito-1.0.5/toqito/state_props/concurrence.py` & `toqito-1.0.6/toqito/state_props/concurrence.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/toqito/state_props/entanglement_of_formation.py` & `toqito-1.0.6/toqito/state_props/entanglement_of_formation.py`

 * *Files 6% similar despite different names*

```diff
@@ -73,26 +73,26 @@
             )
         dim[1] = np.round(dim[1])
 
     if np.prod(dim) != max(dim_x, dim_y):
         raise ValueError(
             "Invalid dimension: Please provide local dimensions that match the size of `rho`."
         )
-
     # If :code:`rho` is a rank-1 density matrix, turn it into a vector instead
     # so we can compute the entanglement-of-formation easily.
     tmp_rho = scipy.linalg.orth(rho)
     if dim_x == dim_y and tmp_rho.shape[1] == 1:
         rho = tmp_rho
         dim_y = 1
 
     # Start computing entanglement-of-formation.
     if min(dim_x, dim_y) == 1:
         rho = rho[:]
-        return von_neumann_entropy(partial_trace(rho * rho.conj().T, 2, dim))
+        dim = [x for x in dim]
+        return von_neumann_entropy(partial_trace(rho * rho.conj().T, [1], dim))
 
     # Case: :code:`rho` is a density matrix.
     if dim_x == dim_y:
         # In the two-qubit case, we know how to compute the
         # entanglement-of-formation exactly.
         if dim_x == 4:
             rho_c = concurrence(rho)
```

### Comparing `toqito-1.0.5/toqito/state_props/has_symmetric_extension.py` & `toqito-1.0.6/toqito/state_props/has_symmetric_extension.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,24 @@
 """Determine whether there exists a symmetric extension for a given quantum state."""
 from __future__ import annotations
 import numpy as np
 
-from toqito.channels import partial_trace
+from picos import partial_trace
 from toqito.matrix_props import is_positive_semidefinite
 from toqito.state_opt import symmetric_extension_hierarchy
 from toqito.state_props import is_ppt
 
 
-def has_symmetric_extension(rho: np.ndarray, level: int = 2, dim: np.ndarray | int = None, ppt: bool = True, tol: float = 1e-4) -> bool:
+def has_symmetric_extension(
+    rho: np.ndarray,
+    level: int = 2,
+    dim: np.ndarray | int = None,
+    ppt: bool = True,
+    tol: float = 1e-4,
+) -> bool:
     r"""
     Determine whether there exists a symmetric extension for a given quantum state. [DPS02]_.
 
     Determining whether an operator possesses a symmetric extension at some level :code:`level`
     can be used as a check to determine if the operator is entangled or not.
 
     This function was adapted from QETLAB.
@@ -103,14 +109,16 @@
         dim = np.array([dim, len_mat / dim])
         if np.abs(dim[1] - np.round(dim[1])) >= 2 * len_mat * np.finfo(float).eps:
             raise ValueError(
                 "If `dim` is a scalar, it must evenly divide the length of the matrix."
             )
         dim[1] = int(np.round(dim[1]))
 
+    dim = np.int_(dim)
+
     dim_x, dim_y = int(dim[0]), int(dim[1])
     # In certain situations, we don't need semidefinite programming.
     if level == 1 or len_mat <= 6 and ppt:
         if not ppt:
             # In some cases, the problem is *really* trivial.
             return is_positive_semidefinite(rho)
 
@@ -118,15 +126,15 @@
         # (i.e., they're asking if the state is PPT).
         return is_ppt(rho, 2, dim) and is_positive_semidefinite(rho)
 
     # In the 2-qubit case, an analytic formula is known for whether or not a state has a
     # (2-copy, non-PPT) symmetric extension that is much faster to use than semidefinite
     # programming [CJKLZB14]_.
     if level == 2 and not ppt and dim_x == 2 and dim_y == 2:
-        return np.trace(np.linalg.matrix_power(partial_trace(rho, 1), 2)) >= np.trace(
+        return np.trace(np.linalg.matrix_power(partial_trace(rho, [0]), 2)) >= np.trace(
             np.linalg.matrix_power(rho, 2)
         ) - 4 * np.sqrt(np.linalg.det(rho))
 
     # Otherwise, use semidefinite programming to find a symmetric extension.
     # If the optimal value of the symmetric extension hierarchy is equal to 1,
     # this indicates that there does not exist a symmetric extension at
     # level :code:`level`.
```

### Comparing `toqito-1.0.5/toqito/state_props/in_separable_ball.py` & `toqito-1.0.6/toqito/state_props/in_separable_ball.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/toqito/state_props/is_ensemble.py` & `toqito-1.0.6/toqito/state_props/is_ensemble.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/toqito/state_props/is_mixed.py` & `toqito-1.0.6/toqito/state_props/is_mixed.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/toqito/state_props/is_mutually_orthogonal.py` & `toqito-1.0.6/toqito/state_props/is_mutually_orthogonal.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/toqito/state_props/is_mutually_unbiased_basis.py` & `toqito-1.0.6/toqito/state_props/is_mutually_unbiased_basis.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/toqito/state_props/is_npt.py` & `toqito-1.0.6/toqito/state_props/is_npt.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,15 @@
 from __future__ import annotations
 
 import numpy as np
 
 from toqito.state_props import is_ppt
 
 
-def is_npt(
-    mat: np.ndarray, sys: int = 2, dim: int | list[int] = None, tol: float = None
-) -> bool:
+def is_npt(mat: np.ndarray, sys: int = 2, dim: int | list[int] = None, tol: float = None) -> bool:
     r"""
     Determine whether or not a matrix has negative partial transpose [WikPPT]_.
 
     Yields either :code:`True` or :code:`False`, indicating that :code:`mat` does or does not have
     negative partial transpose (within numerical error). The variable :code:`mat` is assumed to act
     on bipartite space.
```

### Comparing `toqito-1.0.5/toqito/state_props/is_ppt.py` & `toqito-1.0.6/toqito/state_props/is_ppt.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,17 +3,15 @@
 
 import numpy as np
 
 from toqito.matrix_props import is_positive_semidefinite
 from toqito.channels import partial_transpose
 
 
-def is_ppt(
-    mat: np.ndarray, sys: int = 2, dim: int | list[int] = None, tol: float = None
-) -> bool:
+def is_ppt(mat: np.ndarray, sys: int = 2, dim: int | list[int] = None, tol: float = None) -> bool:
     r"""
     Determine whether or not a matrix has positive partial transpose [WikPPT]_.
 
     Yields either :code:`True` or :code:`False`, indicating that :code:`mat` does or does not have
     positive partial transpose (within numerical error). The variable :code:`mat` is assumed to act
     on bipartite space.
 
@@ -78,13 +76,14 @@
     :param tol: Tolerance with which to check whether `mat` is PPT.
     :return: Returns :code:`True` if :code:`mat` is PPT and :code:`False` if
              not.
     """
     eps = np.finfo(float).eps
 
     sqrt_rho_dims = np.round(np.sqrt(list(mat.shape)))
+    sqrt_rho_dims = np.int_(sqrt_rho_dims)
 
     if dim is None:
-        dim = np.array([[sqrt_rho_dims[0], sqrt_rho_dims[0]], [sqrt_rho_dims[1], sqrt_rho_dims[1]]])
+        dim = [[sqrt_rho_dims[0], sqrt_rho_dims[0]], [sqrt_rho_dims[1], sqrt_rho_dims[1]]]
     if tol is None:
         tol = np.sqrt(eps)
-    return is_positive_semidefinite(partial_transpose(mat, sys, dim), tol)
+    return is_positive_semidefinite(partial_transpose(mat, [sys - 1], dim), tol)
```

### Comparing `toqito-1.0.5/toqito/state_props/is_product.py` & `toqito-1.0.6/toqito/state_props/is_product.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,17 +3,15 @@
 
 import numpy as np
 
 from toqito.perms import permute_systems, swap
 from toqito.state_ops import schmidt_decomposition
 
 
-def is_product(
-    rho: np.ndarray, dim: int | list[int] | np.ndarray = None
-) -> bool | np.ndarray:
+def is_product(rho: np.ndarray, dim: int | list[int] | np.ndarray = None) -> bool | np.ndarray:
     r"""
     Determine if a given vector is a product state [WikProdState]_.
 
     If the input is deemed to be product, then the product decomposition is also
     returned.
 
     Examples
```

### Comparing `toqito-1.0.5/toqito/state_props/is_pure.py` & `toqito-1.0.6/toqito/state_props/is_pure.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/toqito/state_props/is_separable.py` & `toqito-1.0.6/toqito/state_props/is_separable.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 """Check if state is separable."""
 from __future__ import annotations
 
 import numpy as np
 
-from toqito.channels import partial_trace, realignment
-from toqito.matrix_props import is_positive_semidefinite
+from toqito.channels import realignment
+from toqito.matrix_props import is_positive_semidefinite, trace_norm
 from toqito.state_props import is_ppt, in_separable_ball
 from toqito.state_props.has_symmetric_extension import has_symmetric_extension
-from toqito.state_metrics import trace_norm
 from toqito.perms import swap
 
+from picos import partial_trace
+
 
 def is_separable(
-        state: np.ndarray, dim: None | int | list[int] = None, level: int = 2, tol: float = 1e-8) -> bool:
+    state: np.ndarray, dim: None | int | list[int] = None, level: int = 2, tol: float = 1e-8
+) -> bool:
     r"""
     Determine if a given state (given as a density matrix) is a separable state [WikSepState]_.
 
     Examples
     ==========
     Consider the following separable (by construction) state:
     .. math::
@@ -62,15 +64,15 @@
     :return: :code:`True` if :code:`rho` is separabale and :code:`False` otherwise.
     """
     if not is_positive_semidefinite(state):
         raise ValueError("Checking separability of non-positive semidefinite matrix is invalid.")
 
     state_len = state.shape[1]
     state_rank = np.linalg.matrix_rank(state)
-    state /= np.trace(state)
+    state = state / np.trace(state)
     eps = np.finfo(float).eps
 
     if dim is None:
         dim = int(np.round(np.sqrt(state_len)))
 
     if isinstance(dim, int):
         dim = np.array([dim, state_len / dim])
@@ -83,16 +85,18 @@
     max_dim = int(max(dim))
     prod_dim = int(np.prod(dim))
 
     if min_dim == 1:
         # Every positive semidefinite matrix is separable when one of the local dimensions is 1.
         return True
 
-    pt_state_alice = partial_trace(state, 2, dim)
-    pt_state_bob = partial_trace(state, 1, dim)
+    dim = [int(x) for x in dim]
+
+    pt_state_alice = partial_trace(state, [1], dim)
+    pt_state_bob = partial_trace(state, [0], dim)
 
     # Check the PPT criterion.
     if not is_ppt(state, 2, dim, tol):
         # Determined to be entangled via the PPT criterion.
         # A. Peres.
         # Separability criterion for density matrices.
         # Phys. Rev. Lett., 77:1413-1415, 1996.
@@ -103,16 +107,20 @@
     if prod_dim <= 6 or min(dim) <= 1:
         # Determined to be separable via sufficiency of the PPT criterion in small dimensions
         # M. Horodecki, P. Horodecki, and R. Horodecki.
         # Separability of mixed states: Necessary and sufficient conditions.
         # Also, see Horodecki Theorem in https://arxiv.org/pdf/0811.2803.pdf.
         return is_ppt(state, 2, dim, tol)
 
-    if state_rank + np.linalg.matrix_rank(pt_state_alice) <= 2 * state.shape[0] * state.shape[1] - state.shape[0] - state.shape[1] + 2 or \
-        state_rank + np.linalg.matrix_rank(pt_state_bob) <= 2 * state.shape[0] * state.shape[1] - state.shape[0] - state.shape[1] + 2:
+    if (
+        state_rank + np.linalg.matrix_rank(pt_state_alice)
+        <= 2 * state.shape[0] * state.shape[1] - state.shape[0] - state.shape[1] + 2
+        or state_rank + np.linalg.matrix_rank(pt_state_bob)
+        <= 2 * state.shape[0] * state.shape[1] - state.shape[0] - state.shape[1] + 2
+    ):
         # Determined to be separable via operational criterion of the PPT criterion for low-rank operators.
         # P. Horodecki, M. Lewenstein, G. Vidal, and I. Cirac.
         # Operational criterion and constructive checks for the separability of low-rank density matrices.
         # Phys. Rev. A, 62:032310, 2000.
         # TODO
         pass
 
@@ -121,32 +129,37 @@
         # Determined to be entangled via the realignment criterion.
         # K. Chen and L.-A. Wu.
         # A matrix realignment method for recognizing entanglement.
         # Quantum Inf. Comput., 3:193-202, 2003.
         return False
 
     # Another test that is strictly stronger than the realignment criterion.
-    if trace_norm(realignment(state - np.kron(pt_state_alice, pt_state_bob), dim)) > \
-            np.sqrt(1 - np.trace(pt_state_alice**2 @ pt_state_bob**2)):
+    if trace_norm(realignment(state - np.kron(pt_state_alice, pt_state_bob), dim)) > np.sqrt(
+        1 - np.trace(pt_state_alice**2 @ pt_state_bob**2)
+    ):
         # Determined to be entangled by using Theorem 1 of reference.
         # C.-J. Zhang, Y.-S. Zhang, S. Zhang, and G.-C. Guo.
         # Entanglement detection beyond the cross-norm or realignment criterion.
         # Phys. Rev. A, 77:060301(R), 2008.
         return False
 
     # Obtain sorted list of eigenvalues in descending order.
     eig_vals, _ = np.linalg.eig(state)
     lam = eig_vals[np.argsort(-eig_vals)]
 
     # There are some separability tests that work specifically in the qubit-qudit (i.e., 2 \otimes n) case. Check these tests.
     if min_dim == 2:
         # Check if X is separable from spectrum.
-        if (lam[0] - lam[2 * max_dim-1])**2 <= 4 * lam[2 * max_dim-2] * lam[2*max_dim] + tol**2:
+        if (lam[0] - lam[2 * max_dim - 1]) ** 2 <= 4 * lam[2 * max_dim - 2] * lam[
+            2 * max_dim
+        ] + tol**2:
             print("Determined to be separable by inspecting its eigenvalues.")
-            print("N. Johnston. Separability from spectrum for qubit-qudit states. Phys. Rev. A, 88:062330, 2013.")
+            print(
+                "N. Johnston. Separability from spectrum for qubit-qudit states. Phys. Rev. A, 88:062330, 2013."
+            )
             return True
 
     # For the rest of the block-matrix tests, we need the 2-dimensional subsystem to be the
     # first subsystem, so swap accordingly.
     if dim[0] > 2:
         Xt = swap(state, [1, 2], dim)
     else:
@@ -157,18 +170,18 @@
         # Determined to be separable by closeness to the maximally mixed state.
         # L. Gurvits and H. Barnum. Largest separable balls around the maximally mixed bipartite quantum state.
         # Phys. Rev. A, 66:062311, 2002.
         return True
 
     # Check if X is a rank-1 perturbation of the identity, which is
     # necessarily separable if it's PPT, which we have already checked.
-    if lam[1] - lam[prod_dim-1] < tol**2:
+    if lam[1] - lam[prod_dim - 1] < tol**2:
         # Determined to be separable by being a small rank-1 perturbation of the maximally-mixed state.
         # G. Vidal and R. Tarrach. Robustness of entanglement.
         # Phys. Rev. A, 59:141-155, 1999.
         return True
 
     # The search for symmetric extensions.
     for _ in range(2, level):
         if has_symmetric_extension(state, level):
             return True
-    return False
+    return False
```

### Comparing `toqito-1.0.5/toqito/state_props/l1_norm_coherence.py` & `toqito-1.0.6/toqito/state_props/l1_norm_coherence.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/toqito/state_props/log_negativity.py` & `toqito-1.0.6/toqito/state_props/log_negativity.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Logarithmic negativity property."""
 from __future__ import annotations
 
 import numpy as np
 
 from toqito.state_ops import pure_to_mixed
-from toqito.channels import partial_transpose
+from picos import partial_transpose
 
 
 def log_negativity(rho: np.ndarray, dim: list[int] | int = None) -> float:
     r"""
     Compute the log-negativity of a bipartite quantum state [WikLogNeg]_.
 
     The log-negativity of a subsystem can be defined in terms of a density matrix :math:`\rho`:
@@ -70,9 +70,11 @@
 
     if np.prod(dim) != rho_dims[0]:
         raise ValueError(
             "InvalidDim: Please provide local dimensions in the "
             "argument `dim` that match the size of `rho`."
         )
 
+    dim = [int(x) for x in dim]
+
     # Compute the log-negativity.
-    return np.log2(np.linalg.norm(partial_transpose(rho, 2, dim), ord="nuc"))
+    return np.log2(np.linalg.norm(partial_transpose(rho, [1], dim), ord="nuc"))
```

### Comparing `toqito-1.0.5/toqito/state_props/negativity.py` & `toqito-1.0.6/toqito/state_props/negativity.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Negativity property."""
 from __future__ import annotations
 
 import numpy as np
 
 from toqito.state_ops import pure_to_mixed
-from toqito.channels import partial_transpose
+from picos import partial_transpose
 
 
 def negativity(rho: np.ndarray, dim: list[int] | int = None) -> float:
     r"""
     Compute the negativity of a bipartite quantum state [WikNeg]_.
 
     The negativity of a subsystem can be defined in terms of a density matrix :math:`\rho`:
@@ -71,9 +71,11 @@
 
     if np.prod(dim) != rho_dims[0]:
         raise ValueError(
             "InvalidDim: Please provide local dimensions in the "
             "argument `dim` that match the size of `rho`."
         )
 
+    dim = [int(x) for x in dim]
+
     # Compute the negativity.
-    return (np.linalg.norm(partial_transpose(rho, 2, dim), ord="nuc") - 1) / 2
+    return (np.linalg.norm(partial_transpose(rho, [1], dim), ord="nuc") - 1) / 2
```

### Comparing `toqito-1.0.5/toqito/state_props/purity.py` & `toqito-1.0.6/toqito/state_props/purity.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/toqito/state_props/schmidt_rank.py` & `toqito-1.0.6/toqito/state_props/schmidt_rank.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/toqito/state_props/sk_vec_norm.py` & `toqito-1.0.6/toqito/state_props/sk_vec_norm.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/toqito/state_props/von_neumann_entropy.py` & `toqito-1.0.6/toqito/state_props/von_neumann_entropy.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/toqito/states/__init__.py` & `toqito-1.0.6/toqito/states/__init__.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/toqito/states/basis.py` & `toqito-1.0.6/toqito/states/basis.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/toqito/states/bell.py` & `toqito-1.0.6/toqito/states/bell.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/toqito/states/brauer.py` & `toqito-1.0.6/toqito/states/brauer.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/toqito/states/breuer.py` & `toqito-1.0.6/toqito/states/breuer.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/toqito/states/chessboard.py` & `toqito-1.0.6/toqito/states/chessboard.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/toqito/states/domino.py` & `toqito-1.0.6/toqito/states/domino.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/toqito/states/gen_bell.py` & `toqito-1.0.6/toqito/states/gen_bell.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/toqito/states/ghz.py` & `toqito-1.0.6/toqito/states/ghz.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/toqito/states/gisin.py` & `toqito-1.0.6/toqito/states/gisin.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/toqito/states/horodecki.py` & `toqito-1.0.6/toqito/states/horodecki.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/toqito/states/isotropic.py` & `toqito-1.0.6/toqito/states/isotropic.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/toqito/states/max_entangled.py` & `toqito-1.0.6/toqito/states/max_entangled.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/toqito/states/max_mixed.py` & `toqito-1.0.6/toqito/states/max_mixed.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/toqito/states/singlet.py` & `toqito-1.0.6/toqito/states/singlet.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/toqito/states/tile.py` & `toqito-1.0.6/toqito/states/tile.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/toqito/states/w_state.py` & `toqito-1.0.6/toqito/states/w_state.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/toqito/states/werner.py` & `toqito-1.0.6/toqito/states/werner.py`

 * *Files identical despite different names*

### Comparing `toqito-1.0.5/toqito.egg-info/SOURCES.txt` & `toqito-1.0.6/toqito.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,18 @@
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 tests/__init__.py
 tests/test_channel_metrics/__init__.py
 tests/test_channel_metrics/test_channel_fidelity.py
+tests/test_channel_metrics/test_completely_bounded_spectral_norm.py
+tests/test_channel_metrics/test_completely_bounded_trace_norm.py
 tests/test_channel_metrics/test_diamond_norm.py
+tests/test_channel_metrics/test_fidelity_of_separability.py
 tests/test_channel_ops/__init__.py
 tests/test_channel_ops/test_apply_channel.py
 tests/test_channel_ops/test_choi_to_kraus.py
 tests/test_channel_ops/test_dual_channel.py
 tests/test_channel_ops/test_kraus_to_choi.py
 tests/test_channel_ops/test_partial_channel.py
 tests/test_channel_props/__init__.py
@@ -27,14 +30,15 @@
 tests/test_channels/test_dephasing.py
 tests/test_channels/test_depolarizing.py
 tests/test_channels/test_partial_trace.py
 tests/test_channels/test_partial_transpose.py
 tests/test_channels/test_realignment.py
 tests/test_channels/test_reduction.py
 tests/test_helper/__init__.py
+tests/test_helper/test_channel_dim.py
 tests/test_helper/test_cvx_kron.py
 tests/test_helper/test_expr_as_np_array.py
 tests/test_helper/test_np_array_as_expr.py
 tests/test_helper/test_npa_constraints.py
 tests/test_helper/test_update_odometer.py
 tests/test_matrices/__init__.py
 tests/test_matrices/test_cnot.py
@@ -48,33 +52,37 @@
 tests/test_matrices/test_standard_basis.py
 tests/test_matrix_ops/__init__.py
 tests/test_matrix_ops/test_inner_product.py
 tests/test_matrix_ops/test_outer_product.py
 tests/test_matrix_ops/test_tensor.py
 tests/test_matrix_ops/test_unvec.py
 tests/test_matrix_ops/test_vec.py
+tests/test_matrix_ops/test_vectors_from_gram_matrix.py
+tests/test_matrix_ops/test_vectors_to_gram_matrix.py
 tests/test_matrix_props/__init__.py
 tests/test_matrix_props/test_is_block_positive.py
 tests/test_matrix_props/test_is_commuting.py
 tests/test_matrix_props/test_is_density.py
 tests/test_matrix_props/test_is_diagonal.py
+tests/test_matrix_props/test_is_diagonally_dominant.py
 tests/test_matrix_props/test_is_hermitian.py
 tests/test_matrix_props/test_is_idempotent.py
 tests/test_matrix_props/test_is_identity.py
 tests/test_matrix_props/test_is_normal.py
 tests/test_matrix_props/test_is_orthonormal.py
 tests/test_matrix_props/test_is_permutation.py
 tests/test_matrix_props/test_is_positive_definite.py
 tests/test_matrix_props/test_is_positive_semidefinite.py
 tests/test_matrix_props/test_is_projection.py
 tests/test_matrix_props/test_is_square.py
 tests/test_matrix_props/test_is_symmetric.py
 tests/test_matrix_props/test_is_unitary.py
 tests/test_matrix_props/test_majorizes.py
 tests/test_matrix_props/test_sk_norm.py
+tests/test_matrix_props/test_trace_norm.py
 tests/test_measurement_ops/__init__.py
 tests/test_measurement_ops/test_measure.py
 tests/test_measurement_props/__init__.py
 tests/test_measurement_props/test_is_povm.py
 tests/test_nonlocal_games/__init__.py
 tests/test_nonlocal_games/test_extended_nonlocal_game.py
 tests/test_nonlocal_games/test_nonlocal_game.py
@@ -93,23 +101,24 @@
 tests/test_random/__init__.py
 tests/test_random/test_random_density_matrix.py
 tests/test_random/test_random_ginibre.py
 tests/test_random/test_random_povm.py
 tests/test_random/test_random_state_vector.py
 tests/test_random/test_random_unitary.py
 tests/test_state_metrics/__init__.py
+tests/test_state_metrics/test_bures_angle.py
 tests/test_state_metrics/test_bures_distance.py
 tests/test_state_metrics/test_fidelity.py
+tests/test_state_metrics/test_fidelity_of_separability.py
 tests/test_state_metrics/test_helstrom_holevo.py
 tests/test_state_metrics/test_hilbert_schmidt.py
 tests/test_state_metrics/test_hilbert_schmidt_inner_product.py
 tests/test_state_metrics/test_matsumoto_fidelity.py
 tests/test_state_metrics/test_sub_fidelity.py
 tests/test_state_metrics/test_trace_distance.py
-tests/test_state_metrics/test_trace_norm.py
 tests/test_state_ops/__init__.py
 tests/test_state_ops/test_pure_to_mixed.py
 tests/test_state_ops/test_schmidt_decomposition.py
 tests/test_state_opt/__init__.py
 tests/test_state_opt/test_optimal_clone.py
 tests/test_state_opt/test_ppt_distinguishability.py
 tests/test_state_opt/test_state_distinguishability.py
@@ -158,15 +167,18 @@
 toqito.egg-info/PKG-INFO
 toqito.egg-info/SOURCES.txt
 toqito.egg-info/dependency_links.txt
 toqito.egg-info/requires.txt
 toqito.egg-info/top_level.txt
 toqito/channel_metrics/__init__.py
 toqito/channel_metrics/channel_fidelity.py
+toqito/channel_metrics/completely_bounded_spectral_norm.py
+toqito/channel_metrics/completely_bounded_trace_norm.py
 toqito/channel_metrics/diamond_norm.py
+toqito/channel_metrics/fidelity_of_separability.py
 toqito/channel_ops/__init__.py
 toqito/channel_ops/apply_channel.py
 toqito/channel_ops/choi_to_kraus.py
 toqito/channel_ops/dual_channel.py
 toqito/channel_ops/kraus_to_choi.py
 toqito/channel_ops/partial_channel.py
 toqito/channel_props/__init__.py
@@ -183,14 +195,15 @@
 toqito/channels/dephasing.py
 toqito/channels/depolarizing.py
 toqito/channels/partial_trace.py
 toqito/channels/partial_transpose.py
 toqito/channels/realignment.py
 toqito/channels/reduction.py
 toqito/helper/__init__.py
+toqito/helper/channel_dim.py
 toqito/helper/cvx_kron.py
 toqito/helper/expr_as_np_array.py
 toqito/helper/kp_norm.py
 toqito/helper/np_array_as_expr.py
 toqito/helper/npa_hierarchy.py
 toqito/helper/update_odometer.py
 toqito/matrices/__init__.py
@@ -207,33 +220,37 @@
 toqito/matrices/standard_basis.py
 toqito/matrix_ops/__init__.py
 toqito/matrix_ops/inner_product.py
 toqito/matrix_ops/outer_product.py
 toqito/matrix_ops/tensor.py
 toqito/matrix_ops/unvec.py
 toqito/matrix_ops/vec.py
+toqito/matrix_ops/vectors_from_gram_matrix.py
+toqito/matrix_ops/vectors_to_gram_matrix.py
 toqito/matrix_props/__init__.py
 toqito/matrix_props/is_block_positive.py
 toqito/matrix_props/is_commuting.py
 toqito/matrix_props/is_density.py
 toqito/matrix_props/is_diagonal.py
+toqito/matrix_props/is_diagonally_dominant.py
 toqito/matrix_props/is_hermitian.py
 toqito/matrix_props/is_idempotent.py
 toqito/matrix_props/is_identity.py
 toqito/matrix_props/is_normal.py
 toqito/matrix_props/is_orthonormal.py
 toqito/matrix_props/is_permutation.py
 toqito/matrix_props/is_positive_definite.py
 toqito/matrix_props/is_positive_semidefinite.py
 toqito/matrix_props/is_projection.py
 toqito/matrix_props/is_square.py
 toqito/matrix_props/is_symmetric.py
 toqito/matrix_props/is_unitary.py
 toqito/matrix_props/majorizes.py
 toqito/matrix_props/sk_norm.py
+toqito/matrix_props/trace_norm.py
 toqito/measurement_ops/__init__.py
 toqito/measurement_ops/measure.py
 toqito/measurement_props/__init__.py
 toqito/measurement_props/is_povm.py
 toqito/nonlocal_games/__init__.py
 toqito/nonlocal_games/extended_nonlocal_game.py
 toqito/nonlocal_games/nonlocal_game.py
@@ -252,23 +269,24 @@
 toqito/random/__init__.py
 toqito/random/random_density_matrix.py
 toqito/random/random_ginibre.py
 toqito/random/random_povm.py
 toqito/random/random_state_vector.py
 toqito/random/random_unitary.py
 toqito/state_metrics/__init__.py
+toqito/state_metrics/bures_angle.py
 toqito/state_metrics/bures_distance.py
 toqito/state_metrics/fidelity.py
+toqito/state_metrics/fidelity_of_separability.py
 toqito/state_metrics/helstrom_holevo.py
 toqito/state_metrics/hilbert_schmidt.py
 toqito/state_metrics/hilbert_schmidt_inner_product.py
 toqito/state_metrics/matsumoto_fidelity.py
 toqito/state_metrics/sub_fidelity.py
 toqito/state_metrics/trace_distance.py
-toqito/state_metrics/trace_norm.py
 toqito/state_ops/__init__.py
 toqito/state_ops/pure_to_mixed.py
 toqito/state_ops/schmidt_decomposition.py
 toqito/state_opt/__init__.py
 toqito/state_opt/optimal_clone.py
 toqito/state_opt/ppt_distinguishability.py
 toqito/state_opt/state_distinguishability.py
```

