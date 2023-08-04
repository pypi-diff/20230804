# Comparing `tmp/qiling-1.4.5.tar.gz` & `tmp/qiling-1.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qiling-1.4.5.tar", last modified: Sat Dec 31 13:18:18 2022, max compression
+gzip compressed data, was "qiling-1.4.6.tar", last modified: Fri Aug  4 02:50:32 2023, max compression
```

## Comparing `qiling-1.4.5.tar` & `qiling-1.4.6.tar`

### file list

```diff
@@ -1,781 +1,786 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 13:18:18.009490 qiling-1.4.5/
--rw-r--r--   0 runner    (1001) docker     (123)    17992 2022-12-31 13:18:00.000000 qiling-1.4.5/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)    11102 2022-12-31 13:18:18.009490 qiling-1.4.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10378 2022-12-31 13:18:00.000000 qiling-1.4.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 13:18:17.905489 qiling-1.4.5/qiling/
--rw-r--r--   0 runner    (1001) docker     (123)      223 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 13:18:17.913489 qiling-1.4.5/qiling/arch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3530 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/arch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2983 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/arm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/arm64.py
--rw-r--r--   0 runner    (1001) docker     (123)     7748 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/arm64_const.py
--rw-r--r--   0 runner    (1001) docker     (123)     2896 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/arm_const.py
--rw-r--r--   0 runner    (1001) docker     (123)     2643 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/arm_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5954 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/cortex_m.py
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/cortex_m_const.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 13:18:17.913489 qiling-1.4.5/qiling/arch/evm/
--rw-r--r--   0 runner    (1001) docker     (123)      173 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 13:18:17.913489 qiling-1.4.5/qiling/arch/evm/_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/_utils/address.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 13:18:17.913489 qiling-1.4.5/qiling/arch/evm/_utils/blake2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/_utils/blake2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/_utils/blake2/coders.py
--rw-r--r--   0 runner    (1001) docker     (123)     5964 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/_utils/blake2/compression.py
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/_utils/bn128.py
--rw-r--r--   0 runner    (1001) docker     (123)     4130 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/_utils/datatypes.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/_utils/generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3027 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/_utils/numeric.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/_utils/padding.py
--rw-r--r--   0 runner    (1001) docker     (123)      849 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/_utils/transactions.py
--rw-r--r--   0 runner    (1001) docker     (123)    45508 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/abc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/abi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 13:18:17.921489 qiling-1.4.5/qiling/arch/evm/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  4798907 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/analysis/signatures.json
--rw-r--r--   0 runner    (1001) docker     (123)     3698 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/analysis/signatures.py
--rw-r--r--   0 runner    (1001) docker     (123)     3874 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 13:18:17.921489 qiling-1.4.5/qiling/arch/evm/db/
--rw-r--r--   0 runner    (1001) docker     (123)      772 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3541 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/db/accesslog.py
--rw-r--r--   0 runner    (1001) docker     (123)    20659 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/db/account.py
--rw-r--r--   0 runner    (1001) docker     (123)     4301 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/db/atomic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 13:18:17.925489 qiling-1.4.5/qiling/arch/evm/db/backends/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/db/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2570 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/db/backends/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/db/backends/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2892 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/db/batch.py
--rw-r--r--   0 runner    (1001) docker     (123)      971 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/db/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     7518 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/db/diff.py
--rw-r--r--   0 runner    (1001) docker     (123)      440 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/db/hash_trie.py
--rw-r--r--   0 runner    (1001) docker     (123)    17123 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/db/journal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/db/keymap.py
--rw-r--r--   0 runner    (1001) docker     (123)    16716 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/db/slow_journal.py
--rw-r--r--   0 runner    (1001) docker     (123)    16386 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/db/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/db/witness.py
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/evm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3815 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2242 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 13:18:17.925489 qiling-1.4.5/qiling/arch/evm/precompiles/
--rw-r--r--   0 runner    (1001) docker     (123)      407 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/precompiles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      815 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/precompiles/blake2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/precompiles/ecadd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1433 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/precompiles/ecmul.py
--rw-r--r--   0 runner    (1001) docker     (123)     3374 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/precompiles/ecpairing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/precompiles/ecrecover.py
--rw-r--r--   0 runner    (1001) docker     (123)      491 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/precompiles/identity.py
--rw-r--r--   0 runner    (1001) docker     (123)     4021 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/precompiles/modexp.py
--rw-r--r--   0 runner    (1001) docker     (123)      695 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/precompiles/ripemd160.py
--rw-r--r--   0 runner    (1001) docker     (123)      565 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/precompiles/sha256.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 13:18:17.925489 qiling-1.4.5/qiling/arch/evm/rlp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/rlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/rlp/accounts.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/rlp/sedes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3111 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     8010 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 13:18:17.937489 qiling-1.4.5/qiling/arch/evm/vm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/vm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4538 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/vm/code_stream.py
--rw-r--r--   0 runner    (1001) docker     (123)    14940 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/vm/computation.py
--rw-r--r--   0 runner    (1001) docker     (123)     9067 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/vm/dbgcui.py
--rw-r--r--   0 runner    (1001) docker     (123)    11271 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/vm/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/vm/defaultconf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2088 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/vm/disassembler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3751 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/vm/evm.py
--rw-r--r--   0 runner    (1001) docker     (123)     9310 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/vm/exec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/vm/execution_context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 13:18:17.937489 qiling-1.4.5/qiling/arch/evm/vm/forks/
--rw-r--r--   0 runner    (1001) docker     (123)      393 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/vm/forks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 13:18:17.937489 qiling-1.4.5/qiling/arch/evm/vm/forks/berlin/
--rw-r--r--   0 runner    (1001) docker     (123)      197 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/vm/forks/berlin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      562 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/vm/forks/berlin/computation.py
--rw-r--r--   0 runner    (1001) docker     (123)      350 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/vm/forks/berlin/opcodes.py
--rw-r--r--   0 runner    (1001) docker     (123)      203 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/vm/forks/berlin/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 13:18:17.941489 qiling-1.4.5/qiling/arch/evm/vm/forks/byzantium/
--rw-r--r--   0 runner    (1001) docker     (123)     3914 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/vm/forks/byzantium/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      998 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/vm/forks/byzantium/computation.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/vm/forks/byzantium/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3636 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/vm/forks/byzantium/opcodes.py
--rw-r--r--   0 runner    (1001) docker     (123)      211 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/vm/forks/byzantium/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 13:18:17.941489 qiling-1.4.5/qiling/arch/evm/vm/forks/constantinople/
--rw-r--r--   0 runner    (1001) docker     (123)      222 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/vm/forks/constantinople/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      839 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/vm/forks/constantinople/computation.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/vm/forks/constantinople/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/vm/forks/constantinople/opcodes.py
--rw-r--r--   0 runner    (1001) docker     (123)      220 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/vm/forks/constantinople/state.py
--rw-r--r--   0 runner    (1001) docker     (123)      309 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/vm/forks/constantinople/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 13:18:17.945489 qiling-1.4.5/qiling/arch/evm/vm/forks/frontier/
--rw-r--r--   0 runner    (1001) docker     (123)      238 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/vm/forks/frontier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3484 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/vm/forks/frontier/computation.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/vm/forks/frontier/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    20917 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/vm/forks/frontier/opcodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     5700 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/vm/forks/frontier/state.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/vm/forks/frontier/transaction_context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 13:18:17.945489 qiling-1.4.5/qiling/arch/evm/vm/forks/homestead/
--rw-r--r--   0 runner    (1001) docker     (123)      253 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/vm/forks/homestead/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/vm/forks/homestead/computation.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/vm/forks/homestead/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      633 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/vm/forks/homestead/opcodes.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/vm/forks/homestead/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 13:18:17.945489 qiling-1.4.5/qiling/arch/evm/vm/forks/istanbul/
--rw-r--r--   0 runner    (1001) docker     (123)      213 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/vm/forks/istanbul/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/vm/forks/istanbul/computation.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/vm/forks/istanbul/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/vm/forks/istanbul/opcodes.py
--rw-r--r--   0 runner    (1001) docker     (123)      205 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/vm/forks/istanbul/state.py
--rw-r--r--   0 runner    (1001) docker     (123)      728 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/vm/forks/istanbul/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 13:18:17.945489 qiling-1.4.5/qiling/arch/evm/vm/forks/muir_glacier/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/vm/forks/muir_glacier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/vm/forks/muir_glacier/computation.py
--rw-r--r--   0 runner    (1001) docker     (123)      144 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/vm/forks/muir_glacier/opcodes.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/vm/forks/muir_glacier/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 13:18:17.945489 qiling-1.4.5/qiling/arch/evm/vm/forks/petersburg/
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/vm/forks/petersburg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/vm/forks/petersburg/computation.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/vm/forks/petersburg/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/vm/forks/petersburg/opcodes.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/vm/forks/petersburg/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 13:18:17.949489 qiling-1.4.5/qiling/arch/evm/vm/forks/spurious_dragon/
--rw-r--r--   0 runner    (1001) docker     (123)      498 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/vm/forks/spurious_dragon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2261 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/vm/forks/spurious_dragon/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/vm/forks/spurious_dragon/computation.py
--rw-r--r--   0 runner    (1001) docker     (123)      234 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/vm/forks/spurious_dragon/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/vm/forks/spurious_dragon/opcodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/vm/forks/spurious_dragon/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 13:18:17.949489 qiling-1.4.5/qiling/arch/evm/vm/forks/tangerine_whistle/
--rw-r--r--   0 runner    (1001) docker     (123)      469 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/vm/forks/tangerine_whistle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      408 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/vm/forks/tangerine_whistle/computation.py
--rw-r--r--   0 runner    (1001) docker     (123)      239 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/vm/forks/tangerine_whistle/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/vm/forks/tangerine_whistle/opcodes.py
--rw-r--r--   0 runner    (1001) docker     (123)      216 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/vm/forks/tangerine_whistle/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     2083 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/vm/gas_meter.py
--rw-r--r--   0 runner    (1001) docker     (123)      512 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/vm/host.py
--rw-r--r--   0 runner    (1001) docker     (123)     1691 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/vm/instruction.py
--rw-r--r--   0 runner    (1001) docker     (123)     3644 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/vm/interrupt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 13:18:17.953489 qiling-1.4.5/qiling/arch/evm/vm/logic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/vm/logic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5153 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/vm/logic/arithmetic.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/vm/logic/block.py
--rw-r--r--   0 runner    (1001) docker     (123)    14063 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/vm/logic/call.py
--rw-r--r--   0 runner    (1001) docker     (123)     3095 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/vm/logic/comparison.py
--rw-r--r--   0 runner    (1001) docker     (123)     6226 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/vm/logic/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/vm/logic/duplication.py
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/vm/logic/flow.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/vm/logic/invalid.py
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/vm/logic/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/vm/logic/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/vm/logic/sha3.py
--rw-r--r--   0 runner    (1001) docker     (123)     2303 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/vm/logic/stack.py
--rw-r--r--   0 runner    (1001) docker     (123)     3949 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/vm/logic/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/vm/logic/swap.py
--rw-r--r--   0 runner    (1001) docker     (123)     8669 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/vm/logic/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/vm/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3476 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/vm/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     2897 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/vm/mnemonics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/vm/opcode.py
--rw-r--r--   0 runner    (1001) docker     (123)     2531 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/vm/opcode_values.py
--rw-r--r--   0 runner    (1001) docker     (123)     9890 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/vm/opcodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     7536 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/vm/stack.py
--rw-r--r--   0 runner    (1001) docker     (123)     7957 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/vm/state.py
--rw-r--r--   0 runner    (1001) docker     (123)      994 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/vm/transaction_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2946 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/vm/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2905 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/evm/vm/vm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1958 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/mips.py
--rw-r--r--   0 runner    (1001) docker     (123)     3046 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/mips_const.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/msr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/ppc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2920 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/ppc_const.py
--rw-r--r--   0 runner    (1001) docker     (123)     3308 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/register.py
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/riscv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/riscv64.py
--rw-r--r--   0 runner    (1001) docker     (123)     9672 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/riscv_const.py
--rw-r--r--   0 runner    (1001) docker     (123)     4439 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3440 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/x86.py
--rw-r--r--   0 runner    (1001) docker     (123)     7149 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/x86_const.py
--rw-r--r--   0 runner    (1001) docker     (123)     7301 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/arch/x86_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 13:18:17.957489 qiling-1.4.5/qiling/cc/
--rw-r--r--   0 runner    (1001) docker     (123)     4824 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/cc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/cc/arm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2888 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/cc/intel.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/cc/mips.py
--rw-r--r--   0 runner    (1001) docker     (123)      637 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/cc/ppc.py
--rw-r--r--   0 runner    (1001) docker     (123)      679 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/cc/riscv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2204 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/const.py
--rw-r--r--   0 runner    (1001) docker     (123)    24075 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    24963 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/core_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/core_hooks_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2748 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/core_struct.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 13:18:17.957489 qiling-1.4.5/qiling/debugger/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/debugger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/debugger/debugger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/debugger/disassember.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 13:18:17.957489 qiling-1.4.5/qiling/debugger/gdb/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/debugger/gdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32121 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/debugger/gdb/gdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     2536 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/debugger/gdb/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 13:18:17.897489 qiling-1.4.5/qiling/debugger/gdb/xml/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 13:18:17.957489 qiling-1.4.5/qiling/debugger/gdb/xml/a8086/
--rw-r--r--   0 runner    (1001) docker     (123)    11440 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/debugger/gdb/xml/a8086/gdb_init_real_mode.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7372 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/debugger/gdb/xml/a8086/i386-32bit.xml
--rw-r--r--   0 runner    (1001) docker     (123)      204 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/debugger/gdb/xml/a8086/target.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 13:18:17.961490 qiling-1.4.5/qiling/debugger/gdb/xml/arm/
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/debugger/gdb/xml/arm/arm-core.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/debugger/gdb/xml/arm/arm-fpa.xml
--rw-r--r--   0 runner    (1001) docker     (123)      980 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/debugger/gdb/xml/arm/arm-m-profile.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/debugger/gdb/xml/arm/arm-vfpv2.xml
--rw-r--r--   0 runner    (1001) docker     (123)     2077 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/debugger/gdb/xml/arm/arm-vfpv3.xml
--rw-r--r--   0 runner    (1001) docker     (123)      532 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/debugger/gdb/xml/arm/target.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/debugger/gdb/xml/arm/xscale-iwmmxt.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 13:18:17.961490 qiling-1.4.5/qiling/debugger/gdb/xml/arm64/
--rw-r--r--   0 runner    (1001) docker     (123)     2362 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/debugger/gdb/xml/arm64/aarch64-core.xml
--rw-r--r--   0 runner    (1001) docker     (123)     3568 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/debugger/gdb/xml/arm64/aarch64-fpu.xml
--rw-r--r--   0 runner    (1001) docker     (123)      535 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/debugger/gdb/xml/arm64/target.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 13:18:17.961490 qiling-1.4.5/qiling/debugger/gdb/xml/mips/
--rw-r--r--   0 runner    (1001) docker     (123)      508 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/debugger/gdb/xml/mips/mips-cp0.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/debugger/gdb/xml/mips/mips-cpu.xml
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/debugger/gdb/xml/mips/mips-fpu.xml
--rw-r--r--   0 runner    (1001) docker     (123)      675 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/debugger/gdb/xml/mips/target.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 13:18:17.965489 qiling-1.4.5/qiling/debugger/gdb/xml/x86/
--rw-r--r--   0 runner    (1001) docker     (123)      778 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/debugger/gdb/xml/x86/32bit-avx.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/debugger/gdb/xml/x86/32bit-avx512.xml
--rw-r--r--   0 runner    (1001) docker     (123)     2889 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/debugger/gdb/xml/x86/32bit-core.xml
--rw-r--r--   0 runner    (1001) docker     (123)      433 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/debugger/gdb/xml/x86/32bit-linux.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/debugger/gdb/xml/x86/32bit-mpx.xml
--rw-r--r--   0 runner    (1001) docker     (123)      421 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/debugger/gdb/xml/x86/32bit-pkeys.xml
--rw-r--r--   0 runner    (1001) docker     (123)      471 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/debugger/gdb/xml/x86/32bit-segments.xml
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/debugger/gdb/xml/x86/32bit-sse.xml
--rw-r--r--   0 runner    (1001) docker     (123)      348 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/debugger/gdb/xml/x86/target.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 13:18:17.965489 qiling-1.4.5/qiling/debugger/gdb/xml/x8664/
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/debugger/gdb/xml/x8664/64bit-avx.xml
--rw-r--r--   0 runner    (1001) docker     (123)     4688 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/debugger/gdb/xml/x8664/64bit-avx512.xml
--rw-r--r--   0 runner    (1001) docker     (123)     3120 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/debugger/gdb/xml/x8664/64bit-core.xml
--rw-r--r--   0 runner    (1001) docker     (123)      433 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/debugger/gdb/xml/x8664/64bit-linux.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/debugger/gdb/xml/x8664/64bit-mpx.xml
--rw-r--r--   0 runner    (1001) docker     (123)      422 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/debugger/gdb/xml/x8664/64bit-pkeys.xml
--rw-r--r--   0 runner    (1001) docker     (123)      471 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/debugger/gdb/xml/x8664/64bit-segments.xml
--rw-r--r--   0 runner    (1001) docker     (123)     2480 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/debugger/gdb/xml/x8664/64bit-sse.xml
--rw-r--r--   0 runner    (1001) docker     (123)      442 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/debugger/gdb/xml/x8664/target.xml
--rw-r--r--   0 runner    (1001) docker     (123)     5414 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/debugger/gdb/xmlregs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 13:18:17.965489 qiling-1.4.5/qiling/debugger/qdb/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/debugger/qdb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 13:18:17.965489 qiling-1.4.5/qiling/debugger/qdb/arch/
--rw-r--r--   0 runner    (1001) docker     (123)      243 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/debugger/qdb/arch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/debugger/qdb/arch/arch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2898 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/debugger/qdb/arch/arch_arm.py
--rw-r--r--   0 runner    (1001) docker     (123)      704 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/debugger/qdb/arch/arch_mips.py
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/debugger/qdb/arch/arch_x86.py
--rw-r--r--   0 runner    (1001) docker     (123)     1822 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/debugger/qdb/arch/arch_x8664.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 13:18:17.965489 qiling-1.4.5/qiling/debugger/qdb/branch_predictor/
--rw-r--r--   0 runner    (1001) docker     (123)      347 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/debugger/qdb/branch_predictor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      996 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/debugger/qdb/branch_predictor/branch_predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)     9875 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/debugger/qdb/branch_predictor/branch_predictor_arm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3781 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/debugger/qdb/branch_predictor/branch_predictor_mips.py
--rw-r--r--   0 runner    (1001) docker     (123)     4425 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/debugger/qdb/branch_predictor/branch_predictor_x86.py
--rw-r--r--   0 runner    (1001) docker     (123)     4441 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/debugger/qdb/branch_predictor/branch_predictor_x8664.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/debugger/qdb/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     2505 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/debugger/qdb/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     5639 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/debugger/qdb/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/debugger/qdb/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)    17727 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/debugger/qdb/qdb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 13:18:17.969490 qiling-1.4.5/qiling/debugger/qdb/render/
--rw-r--r--   0 runner    (1001) docker     (123)      296 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/debugger/qdb/render/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7285 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/debugger/qdb/render/render.py
--rw-r--r--   0 runner    (1001) docker     (123)     2100 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/debugger/qdb/render/render_arm.py
--rw-r--r--   0 runner    (1001) docker     (123)      714 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/debugger/qdb/render/render_mips.py
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/debugger/qdb/render/render_x86.py
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/debugger/qdb/render/render_x8664.py
--rw-r--r--   0 runner    (1001) docker     (123)     8392 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/debugger/qdb/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    14755 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/debugger/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 13:18:17.969490 qiling-1.4.5/qiling/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/extensions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 13:18:17.969490 qiling-1.4.5/qiling/extensions/afl/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/extensions/afl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4737 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/extensions/afl/afl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 13:18:17.969490 qiling-1.4.5/qiling/extensions/coverage/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/extensions/coverage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 13:18:17.969490 qiling-1.4.5/qiling/extensions/coverage/formats/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/extensions/coverage/formats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      766 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/extensions/coverage/formats/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2252 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/extensions/coverage/formats/drcov.py
--rw-r--r--   0 runner    (1001) docker     (123)      769 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/extensions/coverage/formats/drcov_exact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/extensions/coverage/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 13:18:17.969490 qiling-1.4.5/qiling/extensions/idaplugin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/extensions/idaplugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    88625 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/extensions/idaplugin/qilingida.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 13:18:17.969490 qiling-1.4.5/qiling/extensions/mcu/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/extensions/mcu/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 13:18:17.969490 qiling-1.4.5/qiling/extensions/mcu/atmel/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/extensions/mcu/atmel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9084 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/extensions/mcu/atmel/sam3x8e.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 13:18:17.969490 qiling-1.4.5/qiling/extensions/mcu/bes/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/extensions/mcu/bes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/extensions/mcu/bes/bes2300.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 13:18:17.969490 qiling-1.4.5/qiling/extensions/mcu/gd32vf1/
--rw-r--r--   0 runner    (1001) docker     (123)      137 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/extensions/mcu/gd32vf1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8364 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/extensions/mcu/gd32vf1/gd32vf103.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 13:18:17.969490 qiling-1.4.5/qiling/extensions/mcu/nxp/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/extensions/mcu/nxp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13321 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/extensions/mcu/nxp/mk64f12.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 13:18:17.969490 qiling-1.4.5/qiling/extensions/mcu/stm32f1/
--rw-r--r--   0 runner    (1001) docker     (123)      137 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/extensions/mcu/stm32f1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7405 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/extensions/mcu/stm32f1/stm32f103.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 13:18:17.973490 qiling-1.4.5/qiling/extensions/mcu/stm32f4/
--rw-r--r--   0 runner    (1001) docker     (123)      665 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/extensions/mcu/stm32f4/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8483 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/extensions/mcu/stm32f4/stm32f401.py
--rw-r--r--   0 runner    (1001) docker     (123)    11150 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/extensions/mcu/stm32f4/stm32f405.py
--rw-r--r--   0 runner    (1001) docker     (123)    11517 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/extensions/mcu/stm32f4/stm32f407.py
--rw-r--r--   0 runner    (1001) docker     (123)     7704 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/extensions/mcu/stm32f4/stm32f410.py
--rw-r--r--   0 runner    (1001) docker     (123)     8651 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/extensions/mcu/stm32f4/stm32f411.py
--rw-r--r--   0 runner    (1001) docker     (123)    11067 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/extensions/mcu/stm32f4/stm32f412.py
--rw-r--r--   0 runner    (1001) docker     (123)    12811 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/extensions/mcu/stm32f4/stm32f413.py
--rw-r--r--   0 runner    (1001) docker     (123)    11436 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/extensions/mcu/stm32f4/stm32f415.py
--rw-r--r--   0 runner    (1001) docker     (123)    11803 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/extensions/mcu/stm32f4/stm32f417.py
--rw-r--r--   0 runner    (1001) docker     (123)    12978 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/extensions/mcu/stm32f4/stm32f423.py
--rw-r--r--   0 runner    (1001) docker     (123)    12868 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/extensions/mcu/stm32f4/stm32f427.py
--rw-r--r--   0 runner    (1001) docker     (123)    13167 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/extensions/mcu/stm32f4/stm32f429.py
--rw-r--r--   0 runner    (1001) docker     (123)    13210 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/extensions/mcu/stm32f4/stm32f437.py
--rw-r--r--   0 runner    (1001) docker     (123)    13408 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/extensions/mcu/stm32f4/stm32f439.py
--rw-r--r--   0 runner    (1001) docker     (123)    11968 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/extensions/mcu/stm32f4/stm32f446.py
--rw-r--r--   0 runner    (1001) docker     (123)    13408 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/extensions/mcu/stm32f4/stm32f469.py
--rw-r--r--   0 runner    (1001) docker     (123)    13750 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/extensions/mcu/stm32f4/stm32f479.py
--rw-r--r--   0 runner    (1001) docker     (123)    12606 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/extensions/multitask.py
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/extensions/pipe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 13:18:17.973490 qiling-1.4.5/qiling/extensions/r2/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/extensions/r2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9595 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/extensions/r2/r2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 13:18:17.973490 qiling-1.4.5/qiling/extensions/report/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/extensions/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2248 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/extensions/report/report.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 13:18:17.973490 qiling-1.4.5/qiling/extensions/sanitizers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/extensions/sanitizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4757 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/extensions/sanitizers/heap.py
--rw-r--r--   0 runner    (1001) docker     (123)     7521 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/extensions/trace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 13:18:17.973490 qiling-1.4.5/qiling/extensions/tracing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/extensions/tracing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 13:18:17.973490 qiling-1.4.5/qiling/extensions/tracing/formats/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/extensions/tracing/formats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      809 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/extensions/tracing/formats/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4744 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/extensions/tracing/formats/registers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3827 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/extensions/tracing/formats/tenet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/extensions/tracing/utils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4373 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/extensions/winsdkapi.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/host.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 13:18:17.973490 qiling-1.4.5/qiling/hw/
--rw-r--r--   0 runner    (1001) docker     (123)      402 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 13:18:17.973490 qiling-1.4.5/qiling/hw/analog/
--rw-r--r--   0 runner    (1001) docker     (123)      323 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/analog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3231 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/analog/mk64f12_adc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4250 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/analog/sam3xa_adc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2315 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/analog/sam3xa_dac.py
--rw-r--r--   0 runner    (1001) docker     (123)     5095 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/analog/sam3xa_pwm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/analog/stm32f1xx_adc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2477 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/analog/stm32f4xx_dac.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 13:18:17.973490 qiling-1.4.5/qiling/hw/char/
--rw-r--r--   0 runner    (1001) docker     (123)      351 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/char/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/char/gd32vf1xx_usart.py
--rw-r--r--   0 runner    (1001) docker     (123)     3906 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/char/mk64f12_uart.py
--rw-r--r--   0 runner    (1001) docker     (123)     3709 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/char/sam3xa_uart.py
--rw-r--r--   0 runner    (1001) docker     (123)     7555 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/char/sam3xa_uotghs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/char/stm32f1xx_usart.py
--rw-r--r--   0 runner    (1001) docker     (123)     3563 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/char/stm32f4xx_usart.py
--rw-r--r--   0 runner    (1001) docker     (123)     3503 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/connectivity.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 13:18:17.977490 qiling-1.4.5/qiling/hw/const/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/const/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      306 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/const/cm4_systick.py
--rw-r--r--   0 runner    (1001) docker     (123)    10740 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/const/gd32vf1xx_dma.py
--rw-r--r--   0 runner    (1001) docker     (123)     3698 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/const/gd32vf1xx_i2c.py
--rw-r--r--   0 runner    (1001) docker     (123)     8367 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/const/gd32vf1xx_rcu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/const/gd32vf1xx_rtc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2685 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/const/gd32vf1xx_spi.py
--rw-r--r--   0 runner    (1001) docker     (123)     8266 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/const/gd32vf1xx_timer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2716 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/const/gd32vf1xx_usart.py
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/const/mk64f12_adc.py
--rw-r--r--   0 runner    (1001) docker     (123)    10786 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/const/mk64f12_ftm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2832 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/const/mk64f12_mcg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/const/mk64f12_port.py
--rw-r--r--   0 runner    (1001) docker     (123)     4086 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/const/mk64f12_spi.py
--rw-r--r--   0 runner    (1001) docker     (123)     6059 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/const/mk64f12_uart.py
--rw-r--r--   0 runner    (1001) docker     (123)    13728 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/const/sam3xa_adc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3166 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/const/sam3xa_dac.py
--rw-r--r--   0 runner    (1001) docker     (123)    14847 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/const/sam3xa_pmc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3641 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/const/sam3xa_spi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3177 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/const/sam3xa_uart.py
--rw-r--r--   0 runner    (1001) docker     (123)    48924 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/const/sam3xa_uotghs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/const/stm32f1xx_adc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/const/stm32f1xx_dma.py
--rw-r--r--   0 runner    (1001) docker     (123)     3053 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/const/stm32f4xx_dma.py
--rw-r--r--   0 runner    (1001) docker     (123)     5691 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/const/stm32f4xx_eth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/const/stm32f4xx_i2c.py
--rw-r--r--   0 runner    (1001) docker     (123)      634 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/const/stm32f4xx_pwr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2904 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/const/stm32f4xx_rtc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/const/stm32f4xx_sdio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/const/stm32f4xx_spi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2842 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/const/stm32f4xx_tim.py
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/const/stm32f4xx_usart.py
--rw-r--r--   0 runner    (1001) docker     (123)     4790 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/const/stm32fxxx_rcc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 13:18:17.977490 qiling-1.4.5/qiling/hw/dma/
--rw-r--r--   0 runner    (1001) docker     (123)      258 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/dma/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4525 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/dma/gd32vf1xx_dma.py
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/dma/sam3xa_pdc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4206 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/dma/stm32f1xx_dma.py
--rw-r--r--   0 runner    (1001) docker     (123)     5093 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/dma/stm32f4xx_dma.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 13:18:17.977490 qiling-1.4.5/qiling/hw/external_device/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/external_device/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 13:18:17.977490 qiling-1.4.5/qiling/hw/external_device/lcd/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/external_device/lcd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14339 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/external_device/lcd/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     3929 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/external_device/lcd/lcd1602.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 13:18:17.977490 qiling-1.4.5/qiling/hw/external_device/oled/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/external_device/oled/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2582 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/external_device/oled/ssd1306.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 13:18:17.981490 qiling-1.4.5/qiling/hw/flash/
--rw-r--r--   0 runner    (1001) docker     (123)      226 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/flash/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      756 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/flash/sam3xa_efc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/flash/stm32f1xx_flash.py
--rw-r--r--   0 runner    (1001) docker     (123)     2325 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/flash/stm32f4xx_flash.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 13:18:17.981490 qiling-1.4.5/qiling/hw/gpio/
--rw-r--r--   0 runner    (1001) docker     (123)      383 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/gpio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3147 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/gpio/gd32vf1xx_gpio.py
--rw-r--r--   0 runner    (1001) docker     (123)      976 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/gpio/hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2507 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/gpio/mk64f12_gpio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1778 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/gpio/mk64f12_port.py
--rw-r--r--   0 runner    (1001) docker     (123)     6818 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/gpio/sam3xa_pio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/gpio/stm32f1xx_afio.py
--rw-r--r--   0 runner    (1001) docker     (123)     3089 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/gpio/stm32f1xx_gpio.py
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/gpio/stm32f4xx_gpio.py
--rw-r--r--   0 runner    (1001) docker     (123)     4712 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/hw.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 13:18:17.981490 qiling-1.4.5/qiling/hw/i2c/
--rw-r--r--   0 runner    (1001) docker     (123)      224 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/i2c/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/i2c/gd32vf1xx_i2c.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/i2c/stm32f1xx_i2c.py
--rw-r--r--   0 runner    (1001) docker     (123)     6957 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/i2c/stm32f4xx_i2c.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 13:18:17.981490 qiling-1.4.5/qiling/hw/intc/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/intc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      195 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/intc/cm3_nvic.py
--rw-r--r--   0 runner    (1001) docker     (123)      204 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/intc/cm4_nvic.py
--rw-r--r--   0 runner    (1001) docker     (123)     5128 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/intc/cm_nvic.py
--rw-r--r--   0 runner    (1001) docker     (123)    48917 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/intc/gd32vf1xx_eclic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2799 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/intc/stm32f1xx_exti.py
--rw-r--r--   0 runner    (1001) docker     (123)     1283 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/intc/stm32f4xx_exti.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 13:18:17.981490 qiling-1.4.5/qiling/hw/math/
--rw-r--r--   0 runner    (1001) docker     (123)      184 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/math/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      796 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/math/gd32vf1xx_crc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1909 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/math/stm32f4xx_crc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 13:18:17.981490 qiling-1.4.5/qiling/hw/mem/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/mem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/mem/cm_bitband.py
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/mem/kinetis_bme.py
--rw-r--r--   0 runner    (1001) docker     (123)      668 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/mem/remap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 13:18:17.985490 qiling-1.4.5/qiling/hw/misc/
--rw-r--r--   0 runner    (1001) docker     (123)      688 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/misc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/misc/cm3_scb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/misc/cm4_scb.py
--rw-r--r--   0 runner    (1001) docker     (123)     3734 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/misc/cm_scb.py
--rw-r--r--   0 runner    (1001) docker     (123)     2694 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/misc/gd32vf1xx_rcu.py
--rw-r--r--   0 runner    (1001) docker     (123)     2255 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/misc/mk64f12_mcg.py
--rw-r--r--   0 runner    (1001) docker     (123)     2235 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/misc/mk64f12_sim.py
--rw-r--r--   0 runner    (1001) docker     (123)      590 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/misc/mk64f12_smc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/misc/mk64f12_wdog.py
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/misc/sam3xa_wdt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2424 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/misc/stm32f1xx_rcc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/misc/stm32f4xx_dbg.py
--rw-r--r--   0 runner    (1001) docker     (123)     5605 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/misc/stm32f4xx_rcc.py
--rw-r--r--   0 runner    (1001) docker     (123)    22692 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/misc/stm32f4xx_rcc_derive.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/misc/stm32f4xx_syscfg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 13:18:17.985490 qiling-1.4.5/qiling/hw/net/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/net/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4559 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/net/stm32f4xx_eth.py
--rw-r--r--   0 runner    (1001) docker     (123)     8882 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/peripheral.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 13:18:17.985490 qiling-1.4.5/qiling/hw/power/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/power/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5267 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/power/sam3xa_pmc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/power/stm32f4xx_pwr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 13:18:17.985490 qiling-1.4.5/qiling/hw/sd/
--rw-r--r--   0 runner    (1001) docker     (123)      146 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/sd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3766 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/sd/stm32f4xx_sdio.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 13:18:17.985490 qiling-1.4.5/qiling/hw/spi/
--rw-r--r--   0 runner    (1001) docker     (123)      295 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/spi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/spi/gd32vf1xx_spi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2240 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/spi/mk64f12_spi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/spi/sam3xa_spi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/spi/stm32f1xx_spi.py
--rw-r--r--   0 runner    (1001) docker     (123)     4079 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/spi/stm32f4xx_spi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 13:18:17.985490 qiling-1.4.5/qiling/hw/timer/
--rw-r--r--   0 runner    (1001) docker     (123)      531 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/timer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/timer/cm3_systick.py
--rw-r--r--   0 runner    (1001) docker     (123)      219 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/timer/cm4_systick.py
--rw-r--r--   0 runner    (1001) docker     (123)     2133 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/timer/cm_systick.py
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/timer/gd32vf1xx_rtc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3605 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/timer/gd32vf1xx_timer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2741 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/timer/mk64f12_ftm.py
--rw-r--r--   0 runner    (1001) docker     (123)      352 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/timer/mk64f12_osc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/timer/mk64f12_rtc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/timer/sam3xa_tc.py
--rw-r--r--   0 runner    (1001) docker     (123)      206 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/timer/stm32f1xx_tim.py
--rw-r--r--   0 runner    (1001) docker     (123)     7556 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/timer/stm32f4xx_rtc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5447 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/timer/stm32f4xx_tim.py
--rw-r--r--   0 runner    (1001) docker     (123)      753 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/timer/timer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 13:18:17.985490 qiling-1.4.5/qiling/hw/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/utils/access.py
--rw-r--r--   0 runner    (1001) docker     (123)      319 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/utils/bcd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3589 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/hw/utils/serial.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 13:18:17.989490 qiling-1.4.5/qiling/loader/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/loader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/loader/blob.py
--rw-r--r--   0 runner    (1001) docker     (123)     3511 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/loader/dos.py
--rw-r--r--   0 runner    (1001) docker     (123)    27824 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/loader/elf.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/loader/evm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/loader/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)    27265 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/loader/macho.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 13:18:17.989490 qiling-1.4.5/qiling/loader/macho_parser/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/loader/macho_parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1855 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/loader/macho_parser/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     7669 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/loader/macho_parser/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2347 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/loader/macho_parser/header.py
--rw-r--r--   0 runner    (1001) docker     (123)    20949 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/loader/macho_parser/loadcommand.py
--rw-r--r--   0 runner    (1001) docker     (123)     5093 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/loader/macho_parser/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/loader/macho_parser/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4131 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/loader/mcu.py
--rw-r--r--   0 runner    (1001) docker     (123)    35203 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/loader/pe.py
--rw-r--r--   0 runner    (1001) docker     (123)    14477 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/loader/pe_uefi.py
--rw-r--r--   0 runner    (1001) docker     (123)     5329 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 13:18:17.989490 qiling-1.4.5/qiling/os/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 13:18:17.989490 qiling-1.4.5/qiling/os/blob/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/blob/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/blob/blob.py
--rw-r--r--   0 runner    (1001) docker     (123)      847 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     2953 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/disk.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 13:18:17.989490 qiling-1.4.5/qiling/os/dos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/dos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3283 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/dos/dos.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 13:18:17.989490 qiling-1.4.5/qiling/os/dos/interrupts/
--rw-r--r--   0 runner    (1001) docker     (123)      719 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/dos/interrupts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5887 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/dos/interrupts/int10.py
--rw-r--r--   0 runner    (1001) docker     (123)     4295 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/dos/interrupts/int13.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/dos/interrupts/int15.py
--rw-r--r--   0 runner    (1001) docker     (123)     5590 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/dos/interrupts/int16.py
--rw-r--r--   0 runner    (1001) docker     (123)      470 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/dos/interrupts/int19.py
--rw-r--r--   0 runner    (1001) docker     (123)     1872 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/dos/interrupts/int1a.py
--rw-r--r--   0 runner    (1001) docker     (123)      388 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/dos/interrupts/int20.py
--rw-r--r--   0 runner    (1001) docker     (123)     3168 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/dos/interrupts/int21.py
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/dos/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6405 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/fcall.py
--rw-r--r--   0 runner    (1001) docker     (123)     2452 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/filestruct.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 13:18:17.993490 qiling-1.4.5/qiling/os/freebsd/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/freebsd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8094 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/freebsd/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/freebsd/freebsd.py
--rw-r--r--   0 runner    (1001) docker     (123)     9681 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/freebsd/map_syscall.py
--rw-r--r--   0 runner    (1001) docker     (123)     3406 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/freebsd/syscall.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 13:18:17.993490 qiling-1.4.5/qiling/os/linux/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/linux/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      650 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/linux/fncc.py
--rw-r--r--   0 runner    (1001) docker     (123)    33971 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/linux/function_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     2119 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/linux/futex.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 13:18:17.993490 qiling-1.4.5/qiling/os/linux/kernel_api/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/linux/kernel_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/linux/kernel_api/hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     8802 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/linux/kernel_api/kernel_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6662 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/linux/linux.py
--rw-r--r--   0 runner    (1001) docker     (123)    57190 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/linux/map_syscall.py
--rw-r--r--   0 runner    (1001) docker     (123)     2335 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/linux/procfs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2636 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/linux/syscall.py
--rw-r--r--   0 runner    (1001) docker     (123)    10062 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/linux/syscall_nums.py
--rw-r--r--   0 runner    (1001) docker     (123)    22097 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/linux/thread.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/linux/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 13:18:17.993490 qiling-1.4.5/qiling/os/macos/
--rw-r--r--   0 runner    (1001) docker     (123)      567 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/macos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20023 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/macos/const.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 13:18:17.993490 qiling-1.4.5/qiling/os/macos/events/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/macos/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28415 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/macos/events/macos.py
--rw-r--r--   0 runner    (1001) docker     (123)    16695 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/macos/events/macos_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    47477 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/macos/events/macos_structs.py
--rw-r--r--   0 runner    (1001) docker     (123)      650 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/macos/fncc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 13:18:17.993490 qiling-1.4.5/qiling/os/macos/kernel_api/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/macos/kernel_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/macos/kernel_api/hook.py
--rw-r--r--   0 runner    (1001) docker     (123)    40954 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/macos/kernel_api/kernel_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4458 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/macos/kernel_func.py
--rw-r--r--   0 runner    (1001) docker     (123)     5569 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/macos/mach_port.py
--rw-r--r--   0 runner    (1001) docker     (123)     8334 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/macos/macos.py
--rw-r--r--   0 runner    (1001) docker     (123)    18029 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/macos/map_syscall.py
--rw-r--r--   0 runner    (1001) docker     (123)    57956 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/macos/structs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7626 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/macos/subsystems.py
--rw-r--r--   0 runner    (1001) docker     (123)    15943 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/macos/syscall.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/macos/task.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/macos/thread.py
--rw-r--r--   0 runner    (1001) docker     (123)     7048 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/macos/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5249 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/mapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 13:18:17.997490 qiling-1.4.5/qiling/os/mcu/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/mcu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      105 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/mcu/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/mcu/mcu.py
--rw-r--r--   0 runner    (1001) docker     (123)    27741 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     9017 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/os.py
--rw-r--r--   0 runner    (1001) docker     (123)    12508 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/path.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 13:18:17.997490 qiling-1.4.5/qiling/os/posix/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/posix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26600 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/posix/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     6121 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/posix/const_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     4945 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/posix/filestruct.py
--rw-r--r--   0 runner    (1001) docker     (123)    12443 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/posix/posix.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/posix/stat.py
--rw-r--r--   0 runner    (1001) docker     (123)     3906 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/posix/structs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 13:18:17.997490 qiling-1.4.5/qiling/os/posix/syscall/
--rw-r--r--   0 runner    (1001) docker     (123)      642 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/posix/syscall/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6506 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/posix/syscall/fcntl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1877 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/posix/syscall/futex.py
--rw-r--r--   0 runner    (1001) docker     (123)     3588 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/posix/syscall/ioctl.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9375 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/posix/syscall/mman.py
--rw-r--r--   0 runner    (1001) docker     (123)     2316 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/posix/syscall/net.py
--rw-r--r--   0 runner    (1001) docker     (123)      263 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/posix/syscall/personality.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/posix/syscall/poll.py
--rw-r--r--   0 runner    (1001) docker     (123)      968 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/posix/syscall/prctl.py
--rw-r--r--   0 runner    (1001) docker     (123)      225 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/posix/syscall/ptrace.py
--rw-r--r--   0 runner    (1001) docker     (123)      440 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/posix/syscall/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     1980 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/posix/syscall/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     5109 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/posix/syscall/sched.py
--rw-r--r--   0 runner    (1001) docker     (123)     2310 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/posix/syscall/select.py
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/posix/syscall/sendfile.py
--rw-r--r--   0 runner    (1001) docker     (123)      715 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/posix/syscall/signal.py
--rw-r--r--   0 runner    (1001) docker     (123)    24888 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/posix/syscall/socket.py
--rw-r--r--   0 runner    (1001) docker     (123)    61204 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/posix/syscall/stat.py
--rw-r--r--   0 runner    (1001) docker     (123)      259 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/posix/syscall/sysctl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/posix/syscall/sysinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2190 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/posix/syscall/time.py
--rw-r--r--   0 runner    (1001) docker     (123)      525 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/posix/syscall/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/posix/syscall/uio.py
--rw-r--r--   0 runner    (1001) docker     (123)    21153 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/posix/syscall/unistd.py
--rw-r--r--   0 runner    (1001) docker     (123)      614 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/posix/syscall/utsname.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/posix/syscall/wait.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 13:18:18.001490 qiling-1.4.5/qiling/os/qnx/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/qnx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2085 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/qnx/const.py
--rw-r--r--   0 runner    (1001) docker     (123)      896 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/qnx/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/qnx/map_msgtype.py
--rw-r--r--   0 runner    (1001) docker     (123)     3034 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/qnx/map_syscall.py
--rw-r--r--   0 runner    (1001) docker     (123)    14378 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/qnx/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     5193 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/qnx/qnx.py
--rw-r--r--   0 runner    (1001) docker     (123)     4726 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/qnx/structs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8609 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/qnx/syscall.py
--rw-r--r--   0 runner    (1001) docker     (123)     6771 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/qnx/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     4022 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     8619 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/struct.py
--rw-r--r--   0 runner    (1001) docker     (123)      791 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/thread.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 13:18:18.001490 qiling-1.4.5/qiling/os/uefi/
--rw-r--r--   0 runner    (1001) docker     (123)      781 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/uefi/PiMultiPhase.py
--rw-r--r--   0 runner    (1001) docker     (123)     3293 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/uefi/ProcessorBind.py
--rw-r--r--   0 runner    (1001) docker     (123)      870 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/uefi/UefiBaseType.py
--rw-r--r--   0 runner    (1001) docker     (123)      990 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/uefi/UefiMultiPhase.py
--rw-r--r--   0 runner    (1001) docker     (123)    11016 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/uefi/UefiSpec.py
--rw-r--r--   0 runner    (1001) docker     (123)      453 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/uefi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17107 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/uefi/bs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/uefi/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     5317 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/uefi/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     8421 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/uefi/ds.py
--rw-r--r--   0 runner    (1001) docker     (123)      714 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/uefi/fncc.py
--rw-r--r--   0 runner    (1001) docker     (123)   186697 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/uefi/guids.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2507 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/uefi/hob.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 13:18:18.005490 qiling-1.4.5/qiling/os/uefi/protocols/
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/uefi/protocols/EfiLoadedImageProtocol.py
--rw-r--r--   0 runner    (1001) docker     (123)     4636 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/uefi/protocols/EfiSmmAccess2Protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/uefi/protocols/EfiSmmBase2Protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)     3518 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/uefi/protocols/EfiSmmCpuProtocol.py
--rw-r--r--   0 runner    (1001) docker     (123)     3531 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/uefi/protocols/EfiSmmSwDispatch2Protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)     8224 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/uefi/protocols/PcdProtocol.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/uefi/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3275 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/uefi/protocols/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     6592 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/uefi/rt.py
--rw-r--r--   0 runner    (1001) docker     (123)     8860 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/uefi/smm.py
--rw-r--r--   0 runner    (1001) docker     (123)     9566 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/uefi/smst.py
--rw-r--r--   0 runner    (1001) docker     (123)     2626 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/uefi/st.py
--rw-r--r--   0 runner    (1001) docker     (123)   171340 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/uefi/type32.py
--rw-r--r--   0 runner    (1001) docker     (123)   190551 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/uefi/type64.py
--rw-r--r--   0 runner    (1001) docker     (123)     6717 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/uefi/uefi.py
--rw-r--r--   0 runner    (1001) docker     (123)     5113 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/uefi/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7135 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 13:18:18.005490 qiling-1.4.5/qiling/os/windows/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/windows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5545 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/windows/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2718 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/windows/clipboard.py
--rw-r--r--   0 runner    (1001) docker     (123)    22294 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/windows/const.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 13:18:18.005490 qiling-1.4.5/qiling/os/windows/dlls/
--rw-r--r--   0 runner    (1001) docker     (123)      519 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/windows/dlls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23603 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/windows/dlls/advapi32.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/windows/dlls/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     2402 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/windows/dlls/crypt32.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 13:18:18.009490 qiling-1.4.5/qiling/os/windows/dlls/kernel32/
--rw-r--r--   0 runner    (1001) docker     (123)      665 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/windows/dlls/kernel32/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      467 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/windows/dlls/kernel32/consoleapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/windows/dlls/kernel32/consoleapi2.py
--rw-r--r--   0 runner    (1001) docker     (123)      486 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/windows/dlls/kernel32/consoleapi3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/windows/dlls/kernel32/debugapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     4736 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/windows/dlls/kernel32/errhandlingapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/windows/dlls/kernel32/fibersapi.py
--rw-r--r--   0 runner    (1001) docker     (123)    21419 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/windows/dlls/kernel32/fileapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/windows/dlls/kernel32/handleapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/windows/dlls/kernel32/heapapi.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/windows/dlls/kernel32/interlockedapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/windows/dlls/kernel32/ioapiset.py
--rw-r--r--   0 runner    (1001) docker     (123)     8322 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/windows/dlls/kernel32/libloaderapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2933 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/windows/dlls/kernel32/memoryapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3236 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/windows/dlls/kernel32/processenv.py
--rw-r--r--   0 runner    (1001) docker     (123)    10055 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/windows/dlls/kernel32/processthreadsapi.py
--rw-r--r--   0 runner    (1001) docker     (123)      735 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/windows/dlls/kernel32/profileapi.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/windows/dlls/kernel32/psapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     7096 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/windows/dlls/kernel32/stringapiset.py
--rw-r--r--   0 runner    (1001) docker     (123)    10530 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/windows/dlls/kernel32/synchapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     6651 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/windows/dlls/kernel32/sysinfoapi.py
--rw-r--r--   0 runner    (1001) docker     (123)      564 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/windows/dlls/kernel32/timezoneapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/windows/dlls/kernel32/tlhelp32.py
--rw-r--r--   0 runner    (1001) docker     (123)    19709 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/windows/dlls/kernel32/winbase.py
--rw-r--r--   0 runner    (1001) docker     (123)     4652 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/windows/dlls/kernel32/winnls.py
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/windows/dlls/kernel32/winnt.py
--rw-r--r--   0 runner    (1001) docker     (123)      702 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/windows/dlls/kernel32/wow64apiset.py
--rw-r--r--   0 runner    (1001) docker     (123)      427 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/windows/dlls/mscoree.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/windows/dlls/msi.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/windows/dlls/msvbvm60.py
--rw-r--r--   0 runner    (1001) docker     (123)    16303 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/windows/dlls/msvcrt.py
--rw-r--r--   0 runner    (1001) docker     (123)    14460 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/windows/dlls/ntdll.py
--rw-r--r--   0 runner    (1001) docker     (123)    36731 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/windows/dlls/ntoskrnl.py
--rw-r--r--   0 runner    (1001) docker     (123)     2390 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/windows/dlls/ole32.py
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/windows/dlls/oleaut32.py
--rw-r--r--   0 runner    (1001) docker     (123)     5098 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/windows/dlls/shell32.py
--rw-r--r--   0 runner    (1001) docker     (123)     2579 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/windows/dlls/shlwapi.py
--rw-r--r--   0 runner    (1001) docker     (123)      230 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/windows/dlls/ucrtbased.py
--rw-r--r--   0 runner    (1001) docker     (123)    21177 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/windows/dlls/user32.py
--rw-r--r--   0 runner    (1001) docker     (123)     8815 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/windows/dlls/wininet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4081 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/windows/dlls/wsock32.py
--rw-r--r--   0 runner    (1001) docker     (123)      560 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/windows/dlls/wudplatform.py
--rw-r--r--   0 runner    (1001) docker     (123)     4186 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/windows/fiber.py
--rw-r--r--   0 runner    (1001) docker     (123)      810 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/windows/fncc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2404 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/windows/handle.py
--rw-r--r--   0 runner    (1001) docker     (123)     8924 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/windows/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    58818 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/windows/structs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4505 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/windows/thread.py
--rw-r--r--   0 runner    (1001) docker     (123)     9091 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/windows/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8616 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/windows/wdk_const.py
--rw-r--r--   0 runner    (1001) docker     (123)     7587 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/os/windows/windows.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 13:18:18.009490 qiling-1.4.5/qiling/profiles/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/profiles/dos.ql
--rw-r--r--   0 runner    (1001) docker     (123)      442 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/profiles/freebsd.ql
--rw-r--r--   0 runner    (1001) docker     (123)      908 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/profiles/linux.ql
--rw-r--r--   0 runner    (1001) docker     (123)      581 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/profiles/macos.ql
--rw-r--r--   0 runner    (1001) docker     (123)      576 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/profiles/qnx.ql
--rw-r--r--   0 runner    (1001) docker     (123)      807 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/profiles/uefi.ql
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/profiles/windows.ql
--rw-r--r--   0 runner    (1001) docker     (123)    14357 2022-12-31 13:18:00.000000 qiling-1.4.5/qiling/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 13:18:17.909489 qiling-1.4.5/qiling.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11102 2022-12-31 13:18:17.000000 qiling-1.4.5/qiling.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    22996 2022-12-31 13:18:17.000000 qiling-1.4.5/qiling.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-31 13:18:17.000000 qiling-1.4.5/qiling.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      653 2022-12-31 13:18:17.000000 qiling-1.4.5/qiling.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2022-12-31 13:18:17.000000 qiling-1.4.5/qiling.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)    11241 2022-12-31 13:18:00.000000 qiling-1.4.5/qltool
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-31 13:18:18.009490 qiling-1.4.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2844 2022-12-31 13:18:00.000000 qiling-1.4.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 02:50:32.320298 qiling-1.4.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    17992 2023-08-04 02:50:09.000000 qiling-1.4.6/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)    11102 2023-08-04 02:50:32.320298 qiling-1.4.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10378 2023-08-04 02:50:09.000000 qiling-1.4.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 02:50:32.244294 qiling-1.4.6/qiling/
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 02:50:32.248294 qiling-1.4.6/qiling/arch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/arch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3258 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/arm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/arm64.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7748 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/arm64_const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/arm_const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/arm_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5954 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/cortex_m.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/cortex_m_const.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 02:50:32.248294 qiling-1.4.6/qiling/arch/evm/
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 02:50:32.248294 qiling-1.4.6/qiling/arch/evm/_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/_utils/address.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 02:50:32.248294 qiling-1.4.6/qiling/arch/evm/_utils/blake2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/_utils/blake2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/_utils/blake2/coders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5964 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/_utils/blake2/compression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/_utils/bn128.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/_utils/datatypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/_utils/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/_utils/numeric.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/_utils/padding.py
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/_utils/transactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45508 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/abi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 02:50:32.256294 qiling-1.4.6/qiling/arch/evm/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  4798907 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/analysis/signatures.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3698 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/analysis/signatures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 02:50:32.256294 qiling-1.4.6/qiling/arch/evm/db/
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/db/accesslog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20659 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/db/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/db/atomic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 02:50:32.256294 qiling-1.4.6/qiling/arch/evm/db/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/db/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/db/backends/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/db/backends/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/db/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/db/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7518 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/db/diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/db/hash_trie.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17123 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/db/journal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/db/keymap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16716 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/db/slow_journal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16386 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/db/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/db/witness.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/evm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 02:50:32.256294 qiling-1.4.6/qiling/arch/evm/precompiles/
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/precompiles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/precompiles/blake2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/precompiles/ecadd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/precompiles/ecmul.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/precompiles/ecpairing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/precompiles/ecrecover.py
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/precompiles/identity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4021 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/precompiles/modexp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/precompiles/ripemd160.py
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/precompiles/sha256.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 02:50:32.256294 qiling-1.4.6/qiling/arch/evm/rlp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/rlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/rlp/accounts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/rlp/sedes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8010 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 02:50:32.260295 qiling-1.4.6/qiling/arch/evm/vm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/vm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4538 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/vm/code_stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14940 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/vm/computation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9067 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/vm/dbgcui.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11271 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/vm/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/vm/defaultconf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/vm/disassembler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/vm/evm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9310 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/vm/exec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/vm/execution_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 02:50:32.260295 qiling-1.4.6/qiling/arch/evm/vm/forks/
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/vm/forks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 02:50:32.260295 qiling-1.4.6/qiling/arch/evm/vm/forks/berlin/
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/vm/forks/berlin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/vm/forks/berlin/computation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/vm/forks/berlin/opcodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/vm/forks/berlin/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 02:50:32.260295 qiling-1.4.6/qiling/arch/evm/vm/forks/byzantium/
+-rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/vm/forks/byzantium/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/vm/forks/byzantium/computation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/vm/forks/byzantium/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/vm/forks/byzantium/opcodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/vm/forks/byzantium/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 02:50:32.264295 qiling-1.4.6/qiling/arch/evm/vm/forks/constantinople/
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/vm/forks/constantinople/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/vm/forks/constantinople/computation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/vm/forks/constantinople/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/vm/forks/constantinople/opcodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/vm/forks/constantinople/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/vm/forks/constantinople/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 02:50:32.264295 qiling-1.4.6/qiling/arch/evm/vm/forks/frontier/
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/vm/forks/frontier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/vm/forks/frontier/computation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/vm/forks/frontier/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20917 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/vm/forks/frontier/opcodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5700 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/vm/forks/frontier/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/vm/forks/frontier/transaction_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 02:50:32.264295 qiling-1.4.6/qiling/arch/evm/vm/forks/homestead/
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/vm/forks/homestead/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/vm/forks/homestead/computation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/vm/forks/homestead/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/vm/forks/homestead/opcodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/vm/forks/homestead/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 02:50:32.264295 qiling-1.4.6/qiling/arch/evm/vm/forks/istanbul/
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/vm/forks/istanbul/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/vm/forks/istanbul/computation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/vm/forks/istanbul/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/vm/forks/istanbul/opcodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/vm/forks/istanbul/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/vm/forks/istanbul/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 02:50:32.264295 qiling-1.4.6/qiling/arch/evm/vm/forks/muir_glacier/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/vm/forks/muir_glacier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/vm/forks/muir_glacier/computation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/vm/forks/muir_glacier/opcodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/vm/forks/muir_glacier/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 02:50:32.264295 qiling-1.4.6/qiling/arch/evm/vm/forks/petersburg/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/vm/forks/petersburg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/vm/forks/petersburg/computation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/vm/forks/petersburg/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/vm/forks/petersburg/opcodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/vm/forks/petersburg/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 02:50:32.264295 qiling-1.4.6/qiling/arch/evm/vm/forks/spurious_dragon/
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/vm/forks/spurious_dragon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/vm/forks/spurious_dragon/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/vm/forks/spurious_dragon/computation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/vm/forks/spurious_dragon/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/vm/forks/spurious_dragon/opcodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/vm/forks/spurious_dragon/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 02:50:32.268295 qiling-1.4.6/qiling/arch/evm/vm/forks/tangerine_whistle/
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/vm/forks/tangerine_whistle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/vm/forks/tangerine_whistle/computation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/vm/forks/tangerine_whistle/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/vm/forks/tangerine_whistle/opcodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/vm/forks/tangerine_whistle/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/vm/gas_meter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/vm/host.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/vm/instruction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/vm/interrupt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 02:50:32.268295 qiling-1.4.6/qiling/arch/evm/vm/logic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/vm/logic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5153 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/vm/logic/arithmetic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/vm/logic/block.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14063 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/vm/logic/call.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/vm/logic/comparison.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6226 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/vm/logic/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/vm/logic/duplication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/vm/logic/flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/vm/logic/invalid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/vm/logic/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/vm/logic/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/vm/logic/sha3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/vm/logic/stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3949 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/vm/logic/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/vm/logic/swap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8669 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/vm/logic/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/vm/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/vm/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/vm/mnemonics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/vm/opcode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/vm/opcode_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9890 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/vm/opcodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7536 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/vm/stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7957 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/vm/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/vm/transaction_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/vm/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/evm/vm/vm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/mips.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/mips_const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/msr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/ppc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/ppc_const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/register.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/riscv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/riscv64.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9672 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/riscv_const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/x86.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7391 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/x86_const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7351 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/arch/x86_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 02:50:32.268295 qiling-1.4.6/qiling/cc/
+-rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/cc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/cc/arm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/cc/intel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/cc/mips.py
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/cc/ppc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/cc/riscv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24551 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26318 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/core_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/core_hooks_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/core_struct.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 02:50:32.268295 qiling-1.4.6/qiling/debugger/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/debugger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/debugger/debugger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/debugger/disassember.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 02:50:32.268295 qiling-1.4.6/qiling/debugger/gdb/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/debugger/gdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32511 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/debugger/gdb/gdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/debugger/gdb/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 02:50:32.240294 qiling-1.4.6/qiling/debugger/gdb/xml/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 02:50:32.268295 qiling-1.4.6/qiling/debugger/gdb/xml/a8086/
+-rw-r--r--   0 runner    (1001) docker     (123)    11440 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/debugger/gdb/xml/a8086/gdb_init_real_mode.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7372 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/debugger/gdb/xml/a8086/i386-32bit.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/debugger/gdb/xml/a8086/target.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 02:50:32.272295 qiling-1.4.6/qiling/debugger/gdb/xml/arm/
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/debugger/gdb/xml/arm/arm-core.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/debugger/gdb/xml/arm/arm-fpa.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/debugger/gdb/xml/arm/arm-m-profile.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/debugger/gdb/xml/arm/arm-vfpv2.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/debugger/gdb/xml/arm/arm-vfpv3.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/debugger/gdb/xml/arm/target.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/debugger/gdb/xml/arm/xscale-iwmmxt.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 02:50:32.272295 qiling-1.4.6/qiling/debugger/gdb/xml/arm64/
+-rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/debugger/gdb/xml/arm64/aarch64-core.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     3568 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/debugger/gdb/xml/arm64/aarch64-fpu.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/debugger/gdb/xml/arm64/target.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 02:50:32.272295 qiling-1.4.6/qiling/debugger/gdb/xml/mips/
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/debugger/gdb/xml/mips/mips-cp0.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/debugger/gdb/xml/mips/mips-cpu.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/debugger/gdb/xml/mips/mips-fpu.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/debugger/gdb/xml/mips/target.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 02:50:32.272295 qiling-1.4.6/qiling/debugger/gdb/xml/x86/
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/debugger/gdb/xml/x86/32bit-avx.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/debugger/gdb/xml/x86/32bit-avx512.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/debugger/gdb/xml/x86/32bit-core.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/debugger/gdb/xml/x86/32bit-linux.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/debugger/gdb/xml/x86/32bit-mpx.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/debugger/gdb/xml/x86/32bit-pkeys.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/debugger/gdb/xml/x86/32bit-segments.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/debugger/gdb/xml/x86/32bit-sse.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/debugger/gdb/xml/x86/target.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 02:50:32.272295 qiling-1.4.6/qiling/debugger/gdb/xml/x8664/
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/debugger/gdb/xml/x8664/64bit-avx.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     4688 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/debugger/gdb/xml/x8664/64bit-avx512.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/debugger/gdb/xml/x8664/64bit-core.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/debugger/gdb/xml/x8664/64bit-linux.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/debugger/gdb/xml/x8664/64bit-mpx.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/debugger/gdb/xml/x8664/64bit-pkeys.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/debugger/gdb/xml/x8664/64bit-segments.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/debugger/gdb/xml/x8664/64bit-sse.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/debugger/gdb/xml/x8664/target.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     5414 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/debugger/gdb/xmlregs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 02:50:32.272295 qiling-1.4.6/qiling/debugger/qdb/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/debugger/qdb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 02:50:32.272295 qiling-1.4.6/qiling/debugger/qdb/arch/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/debugger/qdb/arch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/debugger/qdb/arch/arch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2898 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/debugger/qdb/arch/arch_arm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/debugger/qdb/arch/arch_mips.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/debugger/qdb/arch/arch_x86.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/debugger/qdb/arch/arch_x8664.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 02:50:32.276296 qiling-1.4.6/qiling/debugger/qdb/branch_predictor/
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/debugger/qdb/branch_predictor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/debugger/qdb/branch_predictor/branch_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9875 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/debugger/qdb/branch_predictor/branch_predictor_arm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3781 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/debugger/qdb/branch_predictor/branch_predictor_mips.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4425 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/debugger/qdb/branch_predictor/branch_predictor_x86.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4441 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/debugger/qdb/branch_predictor/branch_predictor_x8664.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/debugger/qdb/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/debugger/qdb/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5639 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/debugger/qdb/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/debugger/qdb/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17988 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/debugger/qdb/qdb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 02:50:32.276296 qiling-1.4.6/qiling/debugger/qdb/render/
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/debugger/qdb/render/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7190 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/debugger/qdb/render/render.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/debugger/qdb/render/render_arm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/debugger/qdb/render/render_mips.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/debugger/qdb/render/render_x86.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/debugger/qdb/render/render_x8664.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8392 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/debugger/qdb/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14755 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/debugger/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 02:50:32.276296 qiling-1.4.6/qiling/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/extensions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 02:50:32.276296 qiling-1.4.6/qiling/extensions/afl/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/extensions/afl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4789 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/extensions/afl/afl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 02:50:32.276296 qiling-1.4.6/qiling/extensions/coverage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/extensions/coverage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 02:50:32.276296 qiling-1.4.6/qiling/extensions/coverage/formats/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/extensions/coverage/formats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/extensions/coverage/formats/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/extensions/coverage/formats/drcov.py
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/extensions/coverage/formats/drcov_exact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6800 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/extensions/coverage/formats/history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/extensions/coverage/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 02:50:32.276296 qiling-1.4.6/qiling/extensions/idaplugin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/extensions/idaplugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    88695 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/extensions/idaplugin/qilingida.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 02:50:32.276296 qiling-1.4.6/qiling/extensions/mcu/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/extensions/mcu/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 02:50:32.276296 qiling-1.4.6/qiling/extensions/mcu/atmel/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/extensions/mcu/atmel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9084 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/extensions/mcu/atmel/sam3x8e.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 02:50:32.276296 qiling-1.4.6/qiling/extensions/mcu/bes/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/extensions/mcu/bes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/extensions/mcu/bes/bes2300.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 02:50:32.276296 qiling-1.4.6/qiling/extensions/mcu/gd32vf1/
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/extensions/mcu/gd32vf1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8364 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/extensions/mcu/gd32vf1/gd32vf103.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 02:50:32.276296 qiling-1.4.6/qiling/extensions/mcu/nxp/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/extensions/mcu/nxp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13321 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/extensions/mcu/nxp/mk64f12.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 02:50:32.280296 qiling-1.4.6/qiling/extensions/mcu/stm32f1/
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/extensions/mcu/stm32f1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7405 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/extensions/mcu/stm32f1/stm32f103.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 02:50:32.280296 qiling-1.4.6/qiling/extensions/mcu/stm32f4/
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/extensions/mcu/stm32f4/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8483 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/extensions/mcu/stm32f4/stm32f401.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11150 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/extensions/mcu/stm32f4/stm32f405.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11517 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/extensions/mcu/stm32f4/stm32f407.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7704 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/extensions/mcu/stm32f4/stm32f410.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8651 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/extensions/mcu/stm32f4/stm32f411.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11067 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/extensions/mcu/stm32f4/stm32f412.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12811 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/extensions/mcu/stm32f4/stm32f413.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11436 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/extensions/mcu/stm32f4/stm32f415.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11803 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/extensions/mcu/stm32f4/stm32f417.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12978 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/extensions/mcu/stm32f4/stm32f423.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12868 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/extensions/mcu/stm32f4/stm32f427.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13167 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/extensions/mcu/stm32f4/stm32f429.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13210 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/extensions/mcu/stm32f4/stm32f437.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13408 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/extensions/mcu/stm32f4/stm32f439.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11968 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/extensions/mcu/stm32f4/stm32f446.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13408 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/extensions/mcu/stm32f4/stm32f469.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13750 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/extensions/mcu/stm32f4/stm32f479.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12606 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/extensions/multitask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/extensions/pipe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 02:50:32.280296 qiling-1.4.6/qiling/extensions/r2/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/extensions/r2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9595 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/extensions/r2/r2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 02:50:32.280296 qiling-1.4.6/qiling/extensions/report/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/extensions/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/extensions/report/report.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 02:50:32.280296 qiling-1.4.6/qiling/extensions/sanitizers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/extensions/sanitizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/extensions/sanitizers/heap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8310 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/extensions/trace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 02:50:32.280296 qiling-1.4.6/qiling/extensions/tracing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/extensions/tracing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 02:50:32.280296 qiling-1.4.6/qiling/extensions/tracing/formats/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/extensions/tracing/formats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/extensions/tracing/formats/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4744 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/extensions/tracing/formats/registers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/extensions/tracing/formats/tenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/extensions/tracing/utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5006 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/extensions/winsdkapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/host.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 02:50:32.280296 qiling-1.4.6/qiling/hw/
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 02:50:32.284296 qiling-1.4.6/qiling/hw/analog/
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/analog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/analog/mk64f12_adc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4250 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/analog/sam3xa_adc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/analog/sam3xa_dac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5095 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/analog/sam3xa_pwm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/analog/stm32f1xx_adc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/analog/stm32f4xx_dac.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 02:50:32.284296 qiling-1.4.6/qiling/hw/char/
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/char/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/char/gd32vf1xx_usart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/char/mk64f12_uart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/char/sam3xa_uart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7561 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/char/sam3xa_uotghs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/char/stm32f1xx_usart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3845 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/char/stm32f4xx_usart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3503 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/connectivity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 02:50:32.288296 qiling-1.4.6/qiling/hw/const/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/const/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/const/cm4_systick.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10740 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/const/gd32vf1xx_dma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3698 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/const/gd32vf1xx_i2c.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8367 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/const/gd32vf1xx_rcu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/const/gd32vf1xx_rtc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/const/gd32vf1xx_spi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8266 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/const/gd32vf1xx_timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/const/gd32vf1xx_usart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/const/mk64f12_adc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10786 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/const/mk64f12_ftm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/const/mk64f12_mcg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/const/mk64f12_port.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/const/mk64f12_spi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6059 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/const/mk64f12_uart.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13728 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/const/sam3xa_adc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/const/sam3xa_dac.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14847 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/const/sam3xa_pmc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/const/sam3xa_spi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/const/sam3xa_uart.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48924 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/const/sam3xa_uotghs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/const/stm32f1xx_adc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/const/stm32f1xx_dma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/const/stm32f4xx_dma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6339 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/const/stm32f4xx_eth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/const/stm32f4xx_i2c.py
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/const/stm32f4xx_pwr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/const/stm32f4xx_rtc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/const/stm32f4xx_sdio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/const/stm32f4xx_spi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/const/stm32f4xx_tim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/const/stm32f4xx_usart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/const/stm32fxxx_rcc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 02:50:32.288296 qiling-1.4.6/qiling/hw/dma/
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/dma/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4525 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/dma/gd32vf1xx_dma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/dma/sam3xa_pdc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/dma/stm32f1xx_dma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5342 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/dma/stm32f4xx_dma.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 02:50:32.288296 qiling-1.4.6/qiling/hw/external_device/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/external_device/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 02:50:32.288296 qiling-1.4.6/qiling/hw/external_device/lcd/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/external_device/lcd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14339 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/external_device/lcd/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3929 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/external_device/lcd/lcd1602.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 02:50:32.288296 qiling-1.4.6/qiling/hw/external_device/oled/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/external_device/oled/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/external_device/oled/ssd1306.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 02:50:32.288296 qiling-1.4.6/qiling/hw/flash/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/flash/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/flash/sam3xa_efc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/flash/stm32f1xx_flash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/flash/stm32f4xx_flash.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 02:50:32.288296 qiling-1.4.6/qiling/hw/gpio/
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/gpio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/gpio/gd32vf1xx_gpio.py
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/gpio/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/gpio/mk64f12_gpio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/gpio/mk64f12_port.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6818 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/gpio/sam3xa_pio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/gpio/stm32f1xx_afio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/gpio/stm32f1xx_gpio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/gpio/stm32f4xx_gpio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/hw.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 02:50:32.288296 qiling-1.4.6/qiling/hw/i2c/
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/i2c/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/i2c/gd32vf1xx_i2c.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/i2c/stm32f1xx_i2c.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8406 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/i2c/stm32f4xx_i2c.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 02:50:32.292297 qiling-1.4.6/qiling/hw/intc/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/intc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/intc/cm3_nvic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/intc/cm4_nvic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5128 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/intc/cm_nvic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48923 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/intc/gd32vf1xx_eclic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/intc/stm32f1xx_exti.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/intc/stm32f4xx_exti.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 02:50:32.292297 qiling-1.4.6/qiling/hw/math/
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/math/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/math/gd32vf1xx_crc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/math/stm32f4xx_crc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 02:50:32.292297 qiling-1.4.6/qiling/hw/mem/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/mem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/mem/cm_bitband.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/mem/kinetis_bme.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/mem/remap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 02:50:32.292297 qiling-1.4.6/qiling/hw/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/misc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/misc/cm3_scb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/misc/cm4_scb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3734 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/misc/cm_scb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/misc/gd32vf1xx_rcu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/misc/mk64f12_mcg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/misc/mk64f12_sim.py
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/misc/mk64f12_smc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/misc/mk64f12_wdog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/misc/sam3xa_wdt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/misc/stm32f1xx_rcc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/misc/stm32f4xx_dbg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6364 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/misc/stm32f4xx_rcc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24708 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/misc/stm32f4xx_rcc_derive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/misc/stm32f4xx_syscfg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 02:50:32.292297 qiling-1.4.6/qiling/hw/net/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/net/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4559 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/net/stm32f4xx_eth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8882 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/peripheral.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 02:50:32.292297 qiling-1.4.6/qiling/hw/power/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/power/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5273 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/power/sam3xa_pmc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/power/stm32f4xx_pwr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 02:50:32.292297 qiling-1.4.6/qiling/hw/sd/
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/sd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3766 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/sd/stm32f4xx_sdio.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 02:50:32.292297 qiling-1.4.6/qiling/hw/spi/
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/spi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/spi/gd32vf1xx_spi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/spi/mk64f12_spi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/spi/sam3xa_spi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/spi/stm32f1xx_spi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4085 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/spi/stm32f4xx_spi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 02:50:32.296297 qiling-1.4.6/qiling/hw/timer/
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/timer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/timer/cm3_systick.py
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/timer/cm4_systick.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/timer/cm_systick.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/timer/gd32vf1xx_rtc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3605 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/timer/gd32vf1xx_timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/timer/mk64f12_ftm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/timer/mk64f12_osc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/timer/mk64f12_rtc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/timer/sam3xa_tc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/timer/stm32f1xx_tim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7700 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/timer/stm32f4xx_rtc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5447 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/timer/stm32f4xx_tim.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/timer/timer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 02:50:32.296297 qiling-1.4.6/qiling/hw/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/utils/access.py
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/utils/bcd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3589 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/hw/utils/serial.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 02:50:32.296297 qiling-1.4.6/qiling/loader/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/loader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/loader/blob.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/loader/dos.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28117 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/loader/elf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/loader/evm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/loader/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27265 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/loader/macho.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 02:50:32.296297 qiling-1.4.6/qiling/loader/macho_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/loader/macho_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/loader/macho_parser/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7669 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/loader/macho_parser/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/loader/macho_parser/header.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20949 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/loader/macho_parser/loadcommand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5093 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/loader/macho_parser/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/loader/macho_parser/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4131 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/loader/mcu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38388 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/loader/pe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14477 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/loader/pe_uefi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5824 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 02:50:32.300297 qiling-1.4.6/qiling/os/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 02:50:32.300297 qiling-1.4.6/qiling/os/blob/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/blob/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/blob/blob.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/disk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 02:50:32.300297 qiling-1.4.6/qiling/os/dos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/dos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/dos/dos.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 02:50:32.300297 qiling-1.4.6/qiling/os/dos/interrupts/
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/dos/interrupts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6796 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/dos/interrupts/int10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/dos/interrupts/int13.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/dos/interrupts/int15.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5758 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/dos/interrupts/int16.py
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/dos/interrupts/int19.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/dos/interrupts/int1a.py
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/dos/interrupts/int20.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/dos/interrupts/int21.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/dos/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7344 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/fcall.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/filestruct.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 02:50:32.300297 qiling-1.4.6/qiling/os/freebsd/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/freebsd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8094 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/freebsd/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/freebsd/freebsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9681 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/freebsd/map_syscall.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3406 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/freebsd/syscall.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 02:50:32.300297 qiling-1.4.6/qiling/os/linux/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/linux/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/linux/fncc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34268 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/linux/function_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/linux/futex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 02:50:32.304297 qiling-1.4.6/qiling/os/linux/kernel_api/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/linux/kernel_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/linux/kernel_api/hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8802 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/linux/kernel_api/kernel_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6944 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/linux/linux.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65914 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/linux/map_syscall.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/linux/procfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/linux/syscall.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11061 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/linux/syscall_nums.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22106 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/linux/thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/linux/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 02:50:32.304297 qiling-1.4.6/qiling/os/macos/
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/macos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20320 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/macos/const.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 02:50:32.304297 qiling-1.4.6/qiling/os/macos/events/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/macos/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28463 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/macos/events/macos.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16695 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/macos/events/macos_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49943 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/macos/events/macos_structs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/macos/fncc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 02:50:32.304297 qiling-1.4.6/qiling/os/macos/kernel_api/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/macos/kernel_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/macos/kernel_api/hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40954 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/macos/kernel_api/kernel_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4458 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/macos/kernel_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5623 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/macos/mach_port.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8334 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/macos/macos.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18029 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/macos/map_syscall.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57956 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/macos/structs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7626 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/macos/subsystems.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15961 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/macos/syscall.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/macos/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/macos/thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7048 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/macos/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8486 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/mapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 02:50:32.304297 qiling-1.4.6/qiling/os/mcu/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/mcu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/mcu/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/mcu/mcu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27741 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9972 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/os.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12942 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/path.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 02:50:32.304297 qiling-1.4.6/qiling/os/posix/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/posix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28375 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/posix/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6127 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/posix/const_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4945 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/posix/filestruct.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15089 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/posix/posix.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/posix/stat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/posix/structs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 02:50:32.308297 qiling-1.4.6/qiling/os/posix/syscall/
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/posix/syscall/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/posix/syscall/fcntl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/posix/syscall/futex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3600 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/posix/syscall/ioctl.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8628 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/posix/syscall/mman.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4479 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/posix/syscall/msg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/posix/syscall/net.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/posix/syscall/personality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/posix/syscall/poll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/posix/syscall/prctl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/posix/syscall/ptrace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/posix/syscall/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/posix/syscall/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5109 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/posix/syscall/sched.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/posix/syscall/select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/posix/syscall/sendfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4670 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/posix/syscall/shm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/posix/syscall/signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25015 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/posix/syscall/socket.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64407 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/posix/syscall/stat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/posix/syscall/syscall.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/posix/syscall/sysctl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/posix/syscall/sysinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/posix/syscall/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/posix/syscall/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/posix/syscall/uio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23435 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/posix/syscall/unistd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/posix/syscall/utsname.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/posix/syscall/wait.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 02:50:32.308297 qiling-1.4.6/qiling/os/qnx/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/qnx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/qnx/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/qnx/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/qnx/map_msgtype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/qnx/map_syscall.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14378 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/qnx/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5061 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/qnx/qnx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4726 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/qnx/structs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8609 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/qnx/syscall.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7239 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/qnx/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4022 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8619 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/struct.py
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/thread.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 02:50:32.312297 qiling-1.4.6/qiling/os/uefi/
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/uefi/PiMultiPhase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/uefi/ProcessorBind.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/uefi/UefiBaseType.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/uefi/UefiMultiPhase.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13404 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/uefi/UefiSpec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/uefi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20134 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/uefi/bs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/uefi/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6088 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/uefi/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9858 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/uefi/ds.py
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/uefi/fncc.py
+-rw-r--r--   0 runner    (1001) docker     (123)   186697 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/uefi/guids.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/uefi/hob.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 02:50:32.312297 qiling-1.4.6/qiling/os/uefi/protocols/
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/uefi/protocols/EfiLoadedImageProtocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5158 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/uefi/protocols/EfiSmmAccess2Protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/uefi/protocols/EfiSmmBase2Protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4607 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/uefi/protocols/EfiSmmCpuProtocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/uefi/protocols/EfiSmmSwDispatch2Protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10057 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/uefi/protocols/PcdProtocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/uefi/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/uefi/protocols/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7711 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/uefi/rt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10468 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/uefi/smm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11333 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/uefi/smst.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/uefi/st.py
+-rw-r--r--   0 runner    (1001) docker     (123)   171340 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/uefi/type32.py
+-rw-r--r--   0 runner    (1001) docker     (123)   190551 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/uefi/type64.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7661 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/uefi/uefi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5602 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/uefi/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7615 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 02:50:32.316298 qiling-1.4.6/qiling/os/windows/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/windows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5546 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/windows/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/windows/clipboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22367 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/windows/const.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 02:50:32.316298 qiling-1.4.6/qiling/os/windows/dlls/
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/windows/dlls/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23603 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/windows/dlls/advapi32.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/windows/dlls/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/windows/dlls/crypt32.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 02:50:32.320298 qiling-1.4.6/qiling/os/windows/dlls/kernel32/
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/windows/dlls/kernel32/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/windows/dlls/kernel32/consoleapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/windows/dlls/kernel32/consoleapi2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/windows/dlls/kernel32/consoleapi3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/windows/dlls/kernel32/debugapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/windows/dlls/kernel32/errhandlingapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/windows/dlls/kernel32/fibersapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24713 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/windows/dlls/kernel32/fileapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/windows/dlls/kernel32/handleapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/windows/dlls/kernel32/heapapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/windows/dlls/kernel32/interlockedapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/windows/dlls/kernel32/ioapiset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8224 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/windows/dlls/kernel32/libloaderapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/windows/dlls/kernel32/memoryapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3236 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/windows/dlls/kernel32/processenv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10001 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/windows/dlls/kernel32/processthreadsapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/windows/dlls/kernel32/profileapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/windows/dlls/kernel32/psapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7096 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/windows/dlls/kernel32/stringapiset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10530 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/windows/dlls/kernel32/synchapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6651 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/windows/dlls/kernel32/sysinfoapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/windows/dlls/kernel32/timezoneapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/windows/dlls/kernel32/tlhelp32.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19684 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/windows/dlls/kernel32/winbase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4652 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/windows/dlls/kernel32/winnls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/windows/dlls/kernel32/winnt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/windows/dlls/kernel32/wow64apiset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/windows/dlls/mscoree.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/windows/dlls/msi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/windows/dlls/msvbvm60.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16277 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/windows/dlls/msvcrt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14754 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/windows/dlls/ntdll.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36940 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/windows/dlls/ntoskrnl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/windows/dlls/ole32.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/windows/dlls/oleaut32.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5098 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/windows/dlls/shell32.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/windows/dlls/shlwapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/windows/dlls/ucrtbased.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21189 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/windows/dlls/user32.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8815 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/windows/dlls/wininet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/windows/dlls/wsock32.py
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/windows/dlls/wudplatform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/windows/fiber.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/windows/fncc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/windows/handle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8924 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/windows/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58936 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/windows/structs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/windows/thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10151 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/windows/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8616 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/windows/wdk_const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7530 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/os/windows/windows.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 02:50:32.320298 qiling-1.4.6/qiling/profiles/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/profiles/dos.ql
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/profiles/freebsd.ql
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/profiles/linux.ql
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/profiles/macos.ql
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/profiles/qnx.ql
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/profiles/uefi.ql
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/profiles/windows.ql
+-rw-r--r--   0 runner    (1001) docker     (123)    14394 2023-08-04 02:50:09.000000 qiling-1.4.6/qiling/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 02:50:32.244294 qiling-1.4.6/qiling.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11102 2023-08-04 02:50:32.000000 qiling-1.4.6/qiling.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    23148 2023-08-04 02:50:32.000000 qiling-1.4.6/qiling.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 02:50:32.000000 qiling-1.4.6/qiling.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-08-04 02:50:32.000000 qiling-1.4.6/qiling.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-04 02:50:32.000000 qiling-1.4.6/qiling.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11761 2023-08-04 02:50:09.000000 qiling-1.4.6/qltool
+-rw-r--r--   0 runner    (1001) docker     (123)    18840 2023-08-04 02:50:09.000000 qiling-1.4.6/qltui.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 02:50:32.320298 qiling-1.4.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-08-04 02:50:09.000000 qiling-1.4.6/setup.py
```

### Comparing `qiling-1.4.5/COPYING` & `qiling-1.4.6/COPYING`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/PKG-INFO` & `qiling-1.4.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qiling
-Version: 1.4.5
+Version: 1.4.6
 Summary: Qiling is an advanced binary emulation framework that cross-platform-architecture
 Home-page: http://qiling.io
 Maintainer: KaiJern Lau (xwings)
 Maintainer-email: info@qiling.io
 License: GPLv2
 Keywords: qiling binary emulator framework malware analysis UEFI IoT
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `qiling-1.4.5/README.md` & `qiling-1.4.6/README.md`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/arch/arch.py` & `qiling-1.4.6/qiling/arch/arch.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/arch/arm.py` & `qiling-1.4.6/qiling/arch/arm.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python3
 #
 # Cross Platform and Multi Architecture Advanced Binary Emulation Framework
 #
 
-from functools import cached_property
+from functools import cached_property, lru_cache
 
 from unicorn import Uc, UC_ARCH_ARM, UC_MODE_ARM, UC_MODE_THUMB, UC_MODE_BIG_ENDIAN
 from capstone import Cs, CS_ARCH_ARM, CS_MODE_ARM, CS_MODE_THUMB, CS_MODE_BIG_ENDIAN
 from keystone import Ks, KS_ARCH_ARM, KS_MODE_ARM, KS_MODE_THUMB, KS_MODE_BIG_ENDIAN
 
 from qiling import Qiling
 from qiling.arch.arch import QlArch
@@ -66,44 +66,52 @@
     def effective_pc(self) -> int:
         """Get effective PC value, taking Thumb mode into account.
         """
 
         # append 1 to pc if in thumb mode, or 0 otherwise
         return self.regs.pc | int(self.is_thumb)
 
+    @lru_cache(maxsize=4)
+    def __cached_disasm(self, mode: int) -> Cs:
+        return Cs(CS_ARCH_ARM, mode)
+
     @property
     def disassembler(self) -> Cs:
-        # note: we do not cache the disassembler instance; rather we refresh it
-        # each time to make sure current endianess and thumb mode are taken into
-        # account
+        # note: since endianess and thumb mode might change during execution, we cannot
+        # cache the disassembler instance directly; rather we pick the appropriate cached
+        # instance
 
         mode = CS_MODE_ARM
 
         if self.endian == QL_ENDIAN.EB:
             mode += CS_MODE_BIG_ENDIAN
 
         if self.is_thumb:
             mode += CS_MODE_THUMB
 
-        return Cs(CS_ARCH_ARM, mode)
+        return self.__cached_disasm(mode)
+
+    @lru_cache(maxsize=4)
+    def __cached_asm(self, mode: int) -> Ks:
+        return Ks(KS_ARCH_ARM, mode)
 
     @property
     def assembler(self) -> Ks:
-        # note: we do not cache the assembler instance; rather we refresh it
-        # each time to make sure current endianess and thumb mode are taken into
-        # account
+        # note: since endianess and thumb mode might change during execution, we cannot
+        # cache the assembler instance directly; rather we pick the appropriate cached
+        # instance
 
         mode = KS_MODE_ARM
 
         if self.endian == QL_ENDIAN.EB:
             mode += KS_MODE_BIG_ENDIAN
 
         if self.is_thumb:
             mode += KS_MODE_THUMB
 
-        return Ks(KS_ARCH_ARM, mode)
+        return self.__cached_asm(mode)
 
     def enable_vfp(self) -> None:
         # set full access to cp10 and cp11
         self.regs.c1_c0_2 = self.regs.c1_c0_2 | (0b11 << 20) | (0b11 << 22)
 
         self.regs.fpexc = (1 << 30)
```

### Comparing `qiling-1.4.5/qiling/arch/arm64.py` & `qiling-1.4.6/qiling/arch/arm64.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/arch/arm64_const.py` & `qiling-1.4.6/qiling/arch/arm64_const.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/arch/arm_const.py` & `qiling-1.4.6/qiling/arch/arm_const.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/arch/arm_utils.py` & `qiling-1.4.6/qiling/arch/arm_utils.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/arch/cortex_m.py` & `qiling-1.4.6/qiling/arch/cortex_m.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/arch/cortex_m_const.py` & `qiling-1.4.6/qiling/arch/cortex_m_const.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/arch/evm/_utils/address.py` & `qiling-1.4.6/qiling/arch/evm/_utils/address.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/arch/evm/_utils/blake2/coders.py` & `qiling-1.4.6/qiling/arch/evm/_utils/blake2/coders.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/arch/evm/_utils/blake2/compression.py` & `qiling-1.4.6/qiling/arch/evm/_utils/blake2/compression.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/arch/evm/_utils/bn128.py` & `qiling-1.4.6/qiling/arch/evm/_utils/bn128.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/arch/evm/_utils/datatypes.py` & `qiling-1.4.6/qiling/arch/evm/_utils/datatypes.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/arch/evm/_utils/generator.py` & `qiling-1.4.6/qiling/arch/evm/_utils/generator.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/arch/evm/_utils/numeric.py` & `qiling-1.4.6/qiling/arch/evm/_utils/numeric.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/arch/evm/_utils/transactions.py` & `qiling-1.4.6/qiling/arch/evm/_utils/transactions.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/arch/evm/abc.py` & `qiling-1.4.6/qiling/arch/evm/abc.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/arch/evm/abi.py` & `qiling-1.4.6/qiling/arch/evm/abi.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/arch/evm/analysis/signatures.json` & `qiling-1.4.6/qiling/arch/evm/analysis/signatures.json`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/arch/evm/analysis/signatures.py` & `qiling-1.4.6/qiling/arch/evm/analysis/signatures.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/arch/evm/constants.py` & `qiling-1.4.6/qiling/arch/evm/constants.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/arch/evm/db/__init__.py` & `qiling-1.4.6/qiling/arch/evm/db/__init__.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/arch/evm/db/accesslog.py` & `qiling-1.4.6/qiling/arch/evm/db/accesslog.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/arch/evm/db/account.py` & `qiling-1.4.6/qiling/arch/evm/db/account.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/arch/evm/db/atomic.py` & `qiling-1.4.6/qiling/arch/evm/db/atomic.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/arch/evm/db/backends/base.py` & `qiling-1.4.6/qiling/arch/evm/db/backends/base.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/arch/evm/db/backends/memory.py` & `qiling-1.4.6/qiling/arch/evm/db/backends/memory.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/arch/evm/db/batch.py` & `qiling-1.4.6/qiling/arch/evm/db/batch.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/arch/evm/db/cache.py` & `qiling-1.4.6/qiling/arch/evm/db/cache.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/arch/evm/db/diff.py` & `qiling-1.4.6/qiling/arch/evm/db/diff.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/arch/evm/db/journal.py` & `qiling-1.4.6/qiling/arch/evm/db/journal.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/arch/evm/db/keymap.py` & `qiling-1.4.6/qiling/arch/evm/db/keymap.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/arch/evm/db/slow_journal.py` & `qiling-1.4.6/qiling/arch/evm/db/slow_journal.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/arch/evm/db/storage.py` & `qiling-1.4.6/qiling/arch/evm/db/storage.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/arch/evm/db/witness.py` & `qiling-1.4.6/qiling/arch/evm/db/witness.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/arch/evm/evm.py` & `qiling-1.4.6/qiling/arch/evm/evm.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/arch/evm/exceptions.py` & `qiling-1.4.6/qiling/arch/evm/exceptions.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/arch/evm/hooks.py` & `qiling-1.4.6/qiling/arch/evm/hooks.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/arch/evm/precompiles/blake2.py` & `qiling-1.4.6/qiling/arch/evm/precompiles/blake2.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/arch/evm/precompiles/ecadd.py` & `qiling-1.4.6/qiling/arch/evm/precompiles/ecadd.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/arch/evm/precompiles/ecmul.py` & `qiling-1.4.6/qiling/arch/evm/precompiles/ecmul.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/arch/evm/precompiles/ecpairing.py` & `qiling-1.4.6/qiling/arch/evm/precompiles/ecpairing.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/arch/evm/precompiles/ecrecover.py` & `qiling-1.4.6/qiling/arch/evm/precompiles/ecrecover.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/arch/evm/precompiles/modexp.py` & `qiling-1.4.6/qiling/arch/evm/precompiles/modexp.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/arch/evm/precompiles/ripemd160.py` & `qiling-1.4.6/qiling/arch/evm/precompiles/ripemd160.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/arch/evm/precompiles/sha256.py` & `qiling-1.4.6/qiling/arch/evm/precompiles/sha256.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/arch/evm/rlp/accounts.py` & `qiling-1.4.6/qiling/arch/evm/rlp/accounts.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/arch/evm/typing.py` & `qiling-1.4.6/qiling/arch/evm/typing.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/arch/evm/validation.py` & `qiling-1.4.6/qiling/arch/evm/validation.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/arch/evm/vm/code_stream.py` & `qiling-1.4.6/qiling/arch/evm/vm/code_stream.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/arch/evm/vm/computation.py` & `qiling-1.4.6/qiling/arch/evm/vm/computation.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/arch/evm/vm/dbgcui.py` & `qiling-1.4.6/qiling/arch/evm/vm/dbgcui.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/arch/evm/vm/debug.py` & `qiling-1.4.6/qiling/arch/evm/vm/debug.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/arch/evm/vm/disassembler.py` & `qiling-1.4.6/qiling/arch/evm/vm/disassembler.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/arch/evm/vm/evm.py` & `qiling-1.4.6/qiling/arch/evm/vm/evm.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,28 +10,28 @@
 from eth_typing.evm import Address
 from .forks import *
 from .. import constants
 from .vm import BaseVM
 from .utils import bytecode_to_bytes, runtime_code_detector
 from ..abi import QlArchEVMABI
 
-# Code name	                    Release date	Release block   Opcode supported    
+# Code name                        Release date    Release block   Opcode supported    
 
-# Frontier                      2015-07-30	    0               Yes                 
-# Ice Age	                    2015-09-08	    200,000         -                   
-# Homestead	                    2016-03-15	    1,150,000       Yes                 
-# DAO Fork (unplanned)	        2016-07-20	    1,920,000       -                   
-# Tangerine Whistle (unplanned)	2016-10-18	    2,463,000       Yes                   
-# Spurious Dragon	            2016-11-23	    2,675,000       Yes                 
-# Byzantium	                    2017-10-16	    4,370,000       Yes                 
-# Constantinople	            2019-02-28	    7,280,000       Yes                 
-# Petersburg (unplanned)	    2019-02-28	    7,280,000       Yes                 
-# Istanbul	                    2019-12-08	    9,069,000       Yes                   
-# Muir Glacier	                2020-01-01	    9,200,000       Yes                 
-# Berlin         	            TBD	            TBD             Yes                 
+# Frontier                      2015-07-30        0               Yes                 
+# Ice Age                        2015-09-08        200,000         -                   
+# Homestead                        2016-03-15        1,150,000       Yes                 
+# DAO Fork (unplanned)            2016-07-20        1,920,000       -                   
+# Tangerine Whistle (unplanned)    2016-10-18        2,463,000       Yes                   
+# Spurious Dragon                2016-11-23        2,675,000       Yes                 
+# Byzantium                        2017-10-16        4,370,000       Yes                 
+# Constantinople                2019-02-28        7,280,000       Yes                 
+# Petersburg (unplanned)        2019-02-28        7,280,000       Yes                 
+# Istanbul                        2019-12-08        9,069,000       Yes                   
+# Muir Glacier                    2020-01-01        9,200,000       Yes                 
+# Berlin                         TBD                TBD             Yes                 
 
 
 father_VMs = {
     constants.FRONTIER_FORK:FrontierVM,
     constants.HOMESTEAD_FORK:HomesteadVM,
     constants.TANGERINE_WHISTLE_FORK:TangerineWhistleVM,
     constants.SPURIOUS_DRAGON_FORK:SpuriousDragonVM,
```

### Comparing `qiling-1.4.5/qiling/arch/evm/vm/exec.py` & `qiling-1.4.6/qiling/arch/evm/vm/exec.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/arch/evm/vm/execution_context.py` & `qiling-1.4.6/qiling/arch/evm/vm/execution_context.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/arch/evm/vm/forks/berlin/computation.py` & `qiling-1.4.6/qiling/arch/evm/vm/forks/berlin/computation.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/arch/evm/vm/forks/byzantium/__init__.py` & `qiling-1.4.6/qiling/arch/evm/vm/forks/byzantium/__init__.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/arch/evm/vm/forks/byzantium/computation.py` & `qiling-1.4.6/qiling/arch/evm/vm/forks/byzantium/computation.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/arch/evm/vm/forks/byzantium/opcodes.py` & `qiling-1.4.6/qiling/arch/evm/vm/forks/byzantium/opcodes.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/arch/evm/vm/forks/constantinople/computation.py` & `qiling-1.4.6/qiling/arch/evm/vm/forks/constantinople/computation.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/arch/evm/vm/forks/constantinople/opcodes.py` & `qiling-1.4.6/qiling/arch/evm/vm/forks/constantinople/opcodes.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/arch/evm/vm/forks/frontier/computation.py` & `qiling-1.4.6/qiling/arch/evm/vm/forks/frontier/computation.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/arch/evm/vm/forks/frontier/constants.py` & `qiling-1.4.6/qiling/arch/evm/vm/forks/frontier/constants.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/arch/evm/vm/forks/frontier/opcodes.py` & `qiling-1.4.6/qiling/arch/evm/vm/forks/frontier/opcodes.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/arch/evm/vm/forks/frontier/state.py` & `qiling-1.4.6/qiling/arch/evm/vm/forks/frontier/state.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/arch/evm/vm/forks/homestead/computation.py` & `qiling-1.4.6/qiling/arch/evm/vm/forks/homestead/computation.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/arch/evm/vm/forks/homestead/opcodes.py` & `qiling-1.4.6/qiling/arch/evm/vm/forks/homestead/opcodes.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/arch/evm/vm/forks/homestead/state.py` & `qiling-1.4.6/qiling/arch/evm/vm/forks/homestead/state.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/arch/evm/vm/forks/istanbul/computation.py` & `qiling-1.4.6/qiling/arch/evm/vm/forks/istanbul/computation.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/arch/evm/vm/forks/istanbul/constants.py` & `qiling-1.4.6/qiling/arch/evm/vm/forks/istanbul/constants.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/arch/evm/vm/forks/istanbul/opcodes.py` & `qiling-1.4.6/qiling/arch/evm/vm/forks/istanbul/opcodes.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/arch/evm/vm/forks/istanbul/storage.py` & `qiling-1.4.6/qiling/arch/evm/vm/forks/istanbul/storage.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/arch/evm/vm/forks/muir_glacier/computation.py` & `qiling-1.4.6/qiling/arch/evm/vm/forks/muir_glacier/computation.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/arch/evm/vm/forks/petersburg/__init__.py` & `qiling-1.4.6/qiling/arch/evm/vm/forks/petersburg/__init__.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/arch/evm/vm/forks/petersburg/computation.py` & `qiling-1.4.6/qiling/arch/evm/vm/forks/petersburg/computation.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/arch/evm/vm/forks/petersburg/opcodes.py` & `qiling-1.4.6/qiling/arch/evm/vm/forks/petersburg/opcodes.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/arch/evm/vm/forks/spurious_dragon/_utils.py` & `qiling-1.4.6/qiling/arch/evm/vm/forks/spurious_dragon/_utils.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/arch/evm/vm/forks/spurious_dragon/computation.py` & `qiling-1.4.6/qiling/arch/evm/vm/forks/spurious_dragon/computation.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/arch/evm/vm/forks/spurious_dragon/opcodes.py` & `qiling-1.4.6/qiling/arch/evm/vm/forks/spurious_dragon/opcodes.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/arch/evm/vm/forks/spurious_dragon/state.py` & `qiling-1.4.6/qiling/arch/evm/vm/forks/spurious_dragon/state.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/arch/evm/vm/forks/tangerine_whistle/opcodes.py` & `qiling-1.4.6/qiling/arch/evm/vm/forks/tangerine_whistle/opcodes.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/arch/evm/vm/gas_meter.py` & `qiling-1.4.6/qiling/arch/evm/vm/gas_meter.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/arch/evm/vm/host.py` & `qiling-1.4.6/qiling/arch/evm/vm/host.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/arch/evm/vm/instruction.py` & `qiling-1.4.6/qiling/arch/evm/vm/instruction.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/arch/evm/vm/interrupt.py` & `qiling-1.4.6/qiling/arch/evm/vm/interrupt.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/arch/evm/vm/logic/arithmetic.py` & `qiling-1.4.6/qiling/arch/evm/vm/logic/arithmetic.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/arch/evm/vm/logic/block.py` & `qiling-1.4.6/qiling/arch/evm/vm/logic/block.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/arch/evm/vm/logic/call.py` & `qiling-1.4.6/qiling/arch/evm/vm/logic/call.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/arch/evm/vm/logic/comparison.py` & `qiling-1.4.6/qiling/arch/evm/vm/logic/comparison.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/arch/evm/vm/logic/context.py` & `qiling-1.4.6/qiling/arch/evm/vm/logic/context.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/arch/evm/vm/logic/duplication.py` & `qiling-1.4.6/qiling/arch/evm/vm/logic/duplication.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/arch/evm/vm/logic/flow.py` & `qiling-1.4.6/qiling/arch/evm/vm/logic/flow.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/arch/evm/vm/logic/invalid.py` & `qiling-1.4.6/qiling/arch/evm/vm/logic/invalid.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/arch/evm/vm/logic/logging.py` & `qiling-1.4.6/qiling/arch/evm/vm/logic/logging.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/arch/evm/vm/logic/memory.py` & `qiling-1.4.6/qiling/arch/evm/vm/logic/memory.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/arch/evm/vm/logic/sha3.py` & `qiling-1.4.6/qiling/arch/evm/vm/logic/sha3.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/arch/evm/vm/logic/stack.py` & `qiling-1.4.6/qiling/arch/evm/vm/logic/stack.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/arch/evm/vm/logic/storage.py` & `qiling-1.4.6/qiling/arch/evm/vm/logic/storage.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/arch/evm/vm/logic/swap.py` & `qiling-1.4.6/qiling/arch/evm/vm/logic/swap.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/arch/evm/vm/logic/system.py` & `qiling-1.4.6/qiling/arch/evm/vm/logic/system.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/arch/evm/vm/memory.py` & `qiling-1.4.6/qiling/arch/evm/vm/memory.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/arch/evm/vm/message.py` & `qiling-1.4.6/qiling/arch/evm/vm/message.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/arch/evm/vm/mnemonics.py` & `qiling-1.4.6/qiling/arch/evm/vm/mnemonics.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/arch/evm/vm/opcode.py` & `qiling-1.4.6/qiling/arch/evm/vm/opcode.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/arch/evm/vm/opcode_values.py` & `qiling-1.4.6/qiling/arch/evm/vm/opcode_values.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/arch/evm/vm/opcodes.py` & `qiling-1.4.6/qiling/arch/evm/vm/opcodes.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/arch/evm/vm/stack.py` & `qiling-1.4.6/qiling/arch/evm/vm/stack.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/arch/evm/vm/state.py` & `qiling-1.4.6/qiling/arch/evm/vm/state.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/arch/evm/vm/transaction_context.py` & `qiling-1.4.6/qiling/arch/evm/vm/transaction_context.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/arch/evm/vm/utils.py` & `qiling-1.4.6/qiling/arch/evm/vm/utils.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/arch/evm/vm/vm.py` & `qiling-1.4.6/qiling/arch/evm/vm/vm.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/arch/mips.py` & `qiling-1.4.6/qiling/arch/mips.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/arch/mips_const.py` & `qiling-1.4.6/qiling/arch/mips_const.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/arch/msr.py` & `qiling-1.4.6/qiling/arch/msr.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/arch/ppc.py` & `qiling-1.4.6/qiling/arch/ppc.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/arch/ppc_const.py` & `qiling-1.4.6/qiling/arch/ppc_const.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/arch/register.py` & `qiling-1.4.6/qiling/arch/register.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/arch/riscv.py` & `qiling-1.4.6/qiling/arch/riscv.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/arch/riscv64.py` & `qiling-1.4.6/qiling/arch/riscv64.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/arch/riscv_const.py` & `qiling-1.4.6/qiling/arch/riscv_const.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/arch/utils.py` & `qiling-1.4.6/qiling/arch/utils.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/arch/x86.py` & `qiling-1.4.6/qiling/arch/x86.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/arch/x86_const.py` & `qiling-1.4.6/qiling/arch/x86_const.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,54 +1,56 @@
 #!/usr/bin/env python3
 #
 # Cross Platform and Multi Architecture Advanced Binary Emulation Framework
 #
 
 from unicorn.x86_const import *
 
-QL_X86_F_GRANULARITY = 0x8
-QL_X86_F_PROT_32 = 0x4
-QL_X86_F_LONG = 0x2
-QL_X86_F_AVAILABLE = 0x1
-
-QL_X86_A_PRESENT = 0x80
-
-QL_X86_A_PRIV_3 = 0x60
-QL_X86_A_PRIV_2 = 0x40
-QL_X86_A_PRIV_1 = 0x20
-QL_X86_A_PRIV_0 = 0x0
-
-QL_X86_A_CODE = 0x10
-QL_X86_A_DATA = 0x10
-QL_X86_A_TSS = 0x0
-QL_X86_A_GATE = 0x0
-QL_X86_A_EXEC = 0x8
-
-QL_X86_A_DATA_WRITABLE = 0x2
-QL_X86_A_CODE_READABLE = 0x2
-QL_X86_A_DIR_CON_BIT = 0x4
-
-QL_X86_S_GDT = 0x0
-QL_X86_S_LDT = 0x4
-QL_X86_S_PRIV_3 = 0x3
-QL_X86_S_PRIV_2 = 0x2
-QL_X86_S_PRIV_1 = 0x1
-QL_X86_S_PRIV_0 = 0x0
+# segment descriptor bits [47:40]
+QL_X86_A_DATA_A = (1 << 0)
+QL_X86_A_DATA_W = (1 << 1)
+QL_X86_A_DATA_E = (1 << 2)
+QL_X86_A_DATA   = (0 << 3)
+
+QL_X86_A_CODE_A = (1 << 0)
+QL_X86_A_CODE_R = (1 << 1)
+QL_X86_A_CODE_C = (1 << 2)
+QL_X86_A_CODE   = (1 << 3)
+
+QL_X86_A_DESC_SYSTEM = (0 << 4)  # S
+QL_X86_A_DESC_CODE   = (1 << 4)
+QL_X86_A_DESC_DATA   = (1 << 4)
+
+QL_X86_A_PRIV_0 = (0b00 << 5)  # DPL
+QL_X86_A_PRIV_1 = (0b01 << 5)
+QL_X86_A_PRIV_2 = (0b10 << 5)
+QL_X86_A_PRIV_3 = (0b11 << 5)
+
+QL_X86_A_PRESENT = (1 << 7)
+
+# segment descriptor bits [55:52]
+QL_X86_F_AVAILABLE   = (1 << 0)  # AVL
+QL_X86_F_LONG        = (1 << 1)  # L
+QL_X86_F_OPSIZE_32   = (1 << 2)  # D/B
+QL_X86_F_GRANULARITY = (1 << 3)  # G
+
+# segment selector bits
+QL_X86_SEGSEL_RPL_MASK = 0b11
+QL_X86_SEGSEL_TI_GDT = (0 << 2)
+QL_X86_SEGSEL_TI_LDT = (1 << 2)
 
 QL_X86_GDT_ADDR = 0x30000
 QL_X86_GDT_LIMIT = 0x1000
 QL_X86_GDT_ENTRY_SIZE = 0x8
 
 # These msr registers are x86 specific
 IA32_FS_BASE_MSR = 0xC0000100
 IA32_GS_BASE_MSR = 0xC0000101
 IA32_APIC_BASE_MSR = 0x1B
 
-# WINDOWS SETUP VALUE
-# Linux also needs these
 GS_SEGMENT_ADDR = 0x6000000
 GS_SEGMENT_SIZE = (20 << 20)    # 20 MB
 
 FS_SEGMENT_ADDR = 0x6000
 FS_SEGMENT_SIZE = 0x6000
```

### Comparing `qiling-1.4.5/qiling/arch/x86_utils.py` & `qiling-1.4.6/qiling/arch/x86_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -84,20 +84,20 @@
 
         entry = base_hi << 56 | flags << 52 | limit_hi << 48 | access << 40 | base_lo << 16 | limit_lo
 
         return entry.to_bytes(8, 'little', signed=False)
 
     @staticmethod
     def make_selector(idx: int, rpl: int) -> int:
-        assert rpl & ~0b11 == 0
+        assert rpl & ~QL_X86_SEGSEL_RPL_MASK == 0
 
-        return (idx << 3) | QL_X86_S_GDT | rpl
+        return (idx << 3) | QL_X86_SEGSEL_TI_GDT | rpl
 
     def register_gdt_segment(self, index: int, seg_base: int, seg_limit: int, access: int) -> int:
-        flags = QL_X86_F_PROT_32
+        flags = QL_X86_F_OPSIZE_32
 
         # is this a huge segment?
         if seg_limit > (1 << 16):
             # on 4K granularity the lower 12 bits are implicitly all set
             assert seg_limit & ((1 << 12) - 1) == 0xfff
 
             seg_limit >>= 12
@@ -135,53 +135,53 @@
     def setup_gs(self, base: int, size: int) -> None:
         pass
 
 
 class SegmentManager86(SegmentManager):
     def setup_cs_ds_ss_es(self, base: int, size: int) -> None:
         # While debugging the linux kernel segment, the cs segment was found on the third segment of gdt.
-        access = QL_X86_A_PRESENT | QL_X86_A_CODE | QL_X86_A_CODE_READABLE | QL_X86_A_PRIV_3 | QL_X86_A_EXEC | QL_X86_A_DIR_CON_BIT
+        access = QL_X86_A_PRESENT | QL_X86_A_PRIV_3 | QL_X86_A_DESC_CODE | QL_X86_A_CODE | QL_X86_A_CODE_C | QL_X86_A_CODE_R
         selector = self.gdtm.register_gdt_segment(3, base, size - 1, access)
 
         self.arch.regs.cs = selector
 
         # TODO : The section permission here should be QL_X86_A_PRIV_3, but I do n’t know why it can only be set to QL_X86_A_PRIV_0.
         # While debugging the Linux kernel segment, I found that the three segments DS, SS, and ES all point to the same location in the GDT table.
         # This position is the fifth segment table of GDT.
-        access = QL_X86_A_PRESENT | QL_X86_A_DATA | QL_X86_A_DATA_WRITABLE | QL_X86_A_PRIV_0 | QL_X86_A_DIR_CON_BIT
+        access = QL_X86_A_PRESENT | QL_X86_A_PRIV_0 | QL_X86_A_DESC_DATA | QL_X86_A_DATA | QL_X86_A_DATA_E | QL_X86_A_DATA_W
         selector = self.gdtm.register_gdt_segment(5, base, size - 1, access)
 
         self.arch.regs.ds = selector
         self.arch.regs.ss = selector
         self.arch.regs.es = selector
 
     def setup_fs(self, base: int, size: int) -> None:
-        access = QL_X86_A_PRESENT | QL_X86_A_DATA | QL_X86_A_DATA_WRITABLE | QL_X86_A_PRIV_3 | QL_X86_A_DIR_CON_BIT
+        access = QL_X86_A_PRESENT | QL_X86_A_PRIV_3 | QL_X86_A_DESC_DATA | QL_X86_A_DATA | QL_X86_A_DATA_E | QL_X86_A_DATA_W
         selector = self.gdtm.register_gdt_segment(14, base, size - 1, access)
 
         self.arch.regs.fs = selector
 
     def setup_gs(self, base: int, size: int) -> None:
-        access = QL_X86_A_PRESENT | QL_X86_A_DATA | QL_X86_A_DATA_WRITABLE | QL_X86_A_PRIV_3 | QL_X86_A_DIR_CON_BIT
+        access = QL_X86_A_PRESENT | QL_X86_A_PRIV_3 | QL_X86_A_DESC_DATA | QL_X86_A_DATA | QL_X86_A_DATA_E | QL_X86_A_DATA_W
         selector = self.gdtm.register_gdt_segment(15, base, size - 1, access)
 
         self.arch.regs.gs = selector
 
 
 class SegmentManager64(SegmentManager):
     def setup_cs_ds_ss_es(self, base: int, size: int) -> None:
         # While debugging the linux kernel segment, the cs segment was found on the sixth segment of gdt.
-        access = QL_X86_A_PRESENT | QL_X86_A_CODE | QL_X86_A_CODE_READABLE | QL_X86_A_PRIV_3 | QL_X86_A_EXEC | QL_X86_A_DIR_CON_BIT
+        access = QL_X86_A_PRESENT | QL_X86_A_PRIV_3 | QL_X86_A_DESC_CODE | QL_X86_A_CODE | QL_X86_A_CODE_C | QL_X86_A_CODE_R
         selector = self.gdtm.register_gdt_segment(6, base, size - 1, access)
 
         self.arch.regs.cs = selector
 
         # TODO : The section permission here should be QL_X86_A_PRIV_3, but I do n’t know why it can only be set to QL_X86_A_PRIV_0.
         # When I debug the Linux kernel, I find that only the SS is set to the fifth segment table, and the rest are not set.
-        access = QL_X86_A_PRESENT | QL_X86_A_DATA | QL_X86_A_DATA_WRITABLE | QL_X86_A_PRIV_0 | QL_X86_A_DIR_CON_BIT
+        access = QL_X86_A_PRESENT | QL_X86_A_PRIV_0 | QL_X86_A_DESC_DATA | QL_X86_A_DATA | QL_X86_A_DATA_E | QL_X86_A_DATA_W
         selector = self.gdtm.register_gdt_segment(5, base, size - 1, access)
 
         # self.arch.regs.ds = selector
         self.arch.regs.ss = selector
         # self.arch.regs.es = selector
 
     def setup_fs(self, base: int, size: int) -> None:
```

### Comparing `qiling-1.4.5/qiling/cc/arm.py` & `qiling-1.4.6/qiling/cc/arm.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,16 +16,15 @@
     """
 
     @staticmethod
     def getNumSlots(argbits: int) -> int:
         return 1
 
     def setReturnAddress(self, addr: int) -> None:
-        # TODO: do we need to update LR?
-        self.arch.stack_push(addr)
+        self.arch.regs.lr = addr
 
     def unwind(self, nslots: int) -> int:
         # TODO: cleanup?
         return self.arch.stack_pop()
 
 class aarch64(QlArmBaseCC):
     _retaddr_on_stack = False
```

### Comparing `qiling-1.4.5/qiling/cc/intel.py` & `qiling-1.4.6/qiling/cc/intel.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,106 +1,106 @@
 #!/usr/bin/env python3
 # 
 # Cross Platform and Multi Architecture Advanced Binary Emulation Framework
 
 from unicorn.x86_const import (
-	UC_X86_REG_EAX,	UC_X86_REG_RAX, UC_X86_REG_RCX, UC_X86_REG_RDI,
-	UC_X86_REG_RDX,	UC_X86_REG_RSI,	UC_X86_REG_R8, UC_X86_REG_R9,
-	UC_X86_REG_R10
+    UC_X86_REG_EAX,    UC_X86_REG_RAX, UC_X86_REG_RCX, UC_X86_REG_RDI,
+    UC_X86_REG_RDX,    UC_X86_REG_RSI,    UC_X86_REG_R8, UC_X86_REG_R9,
+    UC_X86_REG_R10
 )
 
 from qiling.cc import QlCommonBaseCC
 
 class QlIntelBaseCC(QlCommonBaseCC):
-	"""Calling convention base class for Intel-based systems.
-	Supports arguments passing over registers and stack.
-	"""
-
-	def setReturnAddress(self, addr: int) -> None:
-		self.arch.stack_push(addr)
-
-	def unwind(self, nslots: int) -> int:
-		# no cleanup; just pop out the return address
-		return self.arch.stack_pop()
+    """Calling convention base class for Intel-based systems.
+    Supports arguments passing over registers and stack.
+    """
+
+    def setReturnAddress(self, addr: int) -> None:
+        self.arch.stack_push(addr)
+
+    def unwind(self, nslots: int) -> int:
+        # no cleanup; just pop out the return address
+        return self.arch.stack_pop()
 
 class QlIntel64(QlIntelBaseCC):
-	"""Calling convention base class for Intel-based 64-bit systems.
-	"""
+    """Calling convention base class for Intel-based 64-bit systems.
+    """
 
-	_retreg = UC_X86_REG_RAX
+    _retreg = UC_X86_REG_RAX
 
-	@staticmethod
-	def getNumSlots(argbits: int) -> int:
-		return max(argbits, 64) // 64
+    @staticmethod
+    def getNumSlots(argbits: int) -> int:
+        return max(argbits, 64) // 64
 
 class QlIntel32(QlIntelBaseCC):
-	"""Calling convention base class for Intel-based 32-bit systems.
-	"""
+    """Calling convention base class for Intel-based 32-bit systems.
+    """
 
-	_retreg = UC_X86_REG_EAX
+    _retreg = UC_X86_REG_EAX
 
-	@staticmethod
-	def getNumSlots(argbits: int) -> int:
-		return max(argbits, 32) // 32
+    @staticmethod
+    def getNumSlots(argbits: int) -> int:
+        return max(argbits, 32) // 32
 
-	def getRawParam(self, slot: int, nbits: int = 0) -> int:
-		__super_getparam = super().getRawParam
+    def getRawParam(self, slot: int, nbits: int = 0) -> int:
+        __super_getparam = super().getRawParam
 
-		if nbits == 64:
-			lo = __super_getparam(slot)
-			hi = __super_getparam(slot + 1)
+        if nbits == 64:
+            lo = __super_getparam(slot)
+            hi = __super_getparam(slot + 1)
 
-			val = (hi << 32) | lo
-		else:
-			val = __super_getparam(slot, nbits)
+            val = (hi << 32) | lo
+        else:
+            val = __super_getparam(slot, nbits)
 
-		return val
+        return val
 
 class amd64(QlIntel64):
-	"""Default calling convention for POSIX (x86-64).
-	First 6 arguments are passed in regs, the rest are passed on the stack.
-	"""
+    """Default calling convention for POSIX (x86-64).
+    First 6 arguments are passed in regs, the rest are passed on the stack.
+    """
 
-	_argregs = (UC_X86_REG_RDI, UC_X86_REG_RSI, UC_X86_REG_RDX, UC_X86_REG_R10, UC_X86_REG_R8, UC_X86_REG_R9) + (None, ) * 10
+    _argregs = (UC_X86_REG_RDI, UC_X86_REG_RSI, UC_X86_REG_RDX, UC_X86_REG_R10, UC_X86_REG_R8, UC_X86_REG_R9) + (None, ) * 10
 
 class ms64(QlIntel64):
-	"""Default calling convention for Windows and UEFI (x86-64).
-	First 4 arguments are passed in regs, the rest are passed on the stack.
+    """Default calling convention for Windows and UEFI (x86-64).
+    First 4 arguments are passed in regs, the rest are passed on the stack.
 
-	Each stack frame starts with a shadow space in size of 4 items, corresponding
-	to the first arguments passed in regs.
-	"""
+    Each stack frame starts with a shadow space in size of 4 items, corresponding
+    to the first arguments passed in regs.
+    """
 
-	_argregs = (UC_X86_REG_RCX, UC_X86_REG_RDX, UC_X86_REG_R8, UC_X86_REG_R9) + (None, ) * 12
-	_shadow = 4
+    _argregs = (UC_X86_REG_RCX, UC_X86_REG_RDX, UC_X86_REG_R8, UC_X86_REG_R9) + (None, ) * 12
+    _shadow = 4
 
 class macosx64(QlIntel64):
-	"""Default calling convention for Mac OS (x86-64).
-	First 6 arguments are passed in regs, the rest are passed on the stack.
-	"""
+    """Default calling convention for Mac OS (x86-64).
+    First 6 arguments are passed in regs, the rest are passed on the stack.
+    """
 
-	_argregs = (UC_X86_REG_RDI, UC_X86_REG_RSI, UC_X86_REG_RDX, UC_X86_REG_RCX, UC_X86_REG_R8, UC_X86_REG_R9) + (None, ) * 10
+    _argregs = (UC_X86_REG_RDI, UC_X86_REG_RSI, UC_X86_REG_RDX, UC_X86_REG_RCX, UC_X86_REG_R8, UC_X86_REG_R9) + (None, ) * 10
 
 class cdecl(QlIntel32):
-	"""Calling convention used by all operating systems (x86).
-	All arguments are passed on the stack.
+    """Calling convention used by all operating systems (x86).
+    All arguments are passed on the stack.
 
-	The caller is resopnsible to unwind the stack.
-	"""
+    The caller is resopnsible to unwind the stack.
+    """
 
-	_argregs = (None, ) * 16
+    _argregs = (None, ) * 16
 
 class stdcall(QlIntel32):
-	"""Calling convention used by all operating systems (x86).
-	All arguments are passed on the stack.
+    """Calling convention used by all operating systems (x86).
+    All arguments are passed on the stack.
 
-	The callee is resopnsible to unwind the stack.
-	"""
+    The callee is resopnsible to unwind the stack.
+    """
 
-	_argregs = (None, ) * 16
+    _argregs = (None, ) * 16
 
-	def unwind(self, nslots: int) -> int:
-		retaddr = super().unwind(nslots)
+    def unwind(self, nslots: int) -> int:
+        retaddr = super().unwind(nslots)
 
-		self.arch.regs.arch_sp += (nslots * self._asize)
+        self.arch.regs.arch_sp += (nslots * self._asize)
 
-		return retaddr
+        return retaddr
```

### Comparing `qiling-1.4.5/qiling/cc/ppc.py` & `qiling-1.4.6/qiling/cc/ppc.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,7 +17,10 @@
 
     _retreg = UC_PPC_REG_3
     _argregs = (UC_PPC_REG_3, UC_PPC_REG_4, UC_PPC_REG_5, UC_PPC_REG_6, UC_PPC_REG_7, UC_PPC_REG_8) + (None, ) * 10
 
     @staticmethod
     def getNumSlots(argbits: int):
         return 1
+
+    def setReturnAddress(self, addr: int):
+        self.arch.regs.lr = addr
```

### Comparing `qiling-1.4.5/qiling/const.py` & `qiling-1.4.6/qiling/const.py`

 * *Files 4% similar despite different names*

```diff
@@ -62,14 +62,20 @@
 
 class QL_STOP(Flag):
     NONE = 0
     STACK_POINTER = (1 << 0)
     EXIT_TRAP = (1 << 1)
 
 
+class QL_STATE(Enum):
+    NOT_SET = 0
+    STARTED = 1
+    STOPPED = 2
+
+
 QL_ARCH_INTERPRETER: Final = (QL_ARCH.EVM,)
 
 QL_OS_POSIX: Final = (QL_OS.LINUX, QL_OS.FREEBSD, QL_OS.MACOS, QL_OS.QNX)
 QL_OS_BAREMETAL: Final = (QL_OS.MCU,)
 
 
 QL_HOOK_BLOCK = 0b0001
@@ -78,15 +84,15 @@
 T = TypeVar('T', bound=Enum)
 
 
 def __casefold_enum(e: Type[T]) -> Mapping[str, T]:
     '''Create a casefolded mapping of an enum to allow case-insensitive lookup.
     '''
 
-    return dict((k.casefold(), v) for k, v in e._member_map_.items())
+    return dict((k.casefold(), v) for k, v in e.__members__.items())
 
 
 debugger_map = __casefold_enum(QL_DEBUGGER)
 arch_map     = __casefold_enum(QL_ARCH)
 os_map       = __casefold_enum(QL_OS)
 verbose_map  = __casefold_enum(QL_VERBOSE)
```

### Comparing `qiling-1.4.5/qiling/core.py` & `qiling-1.4.6/qiling/core.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,40 +16,40 @@
     from logging import Logger
     from .arch.arch import QlArch
     from .os.os import QlOs
     from .os.memory import QlMemoryManager
     from .hw.hw import QlHwManager
     from .loader.loader import QlLoader
 
-from .const import QL_ARCH, QL_ENDIAN, QL_OS, QL_STOP, QL_VERBOSE, QL_ARCH_INTERPRETER, QL_OS_BAREMETAL
+from .const import QL_ARCH, QL_ENDIAN, QL_OS, QL_STATE, QL_STOP, QL_VERBOSE, QL_ARCH_INTERPRETER, QL_OS_BAREMETAL
 from .exception import QlErrorFileNotFound, QlErrorArch, QlErrorOsType
 from .host import QlHost
 from .log import *
 from .utils import *
 from .core_struct import QlCoreStructs
 from .core_hooks import QlCoreHooks
 
 
 class Qiling(QlCoreHooks, QlCoreStructs):
     def __init__(
             self,
-            argv: Sequence[str] = None,
+            argv: Sequence[str] = [],
             rootfs: str = r'.',
             env: MutableMapping[AnyStr, AnyStr] = {},
-            code: bytes = None,
-            ostype: Union[str, QL_OS] = None,
-            archtype: Union[str, QL_ARCH] = None,
+            code: Optional[bytes] = None,
+            ostype: Optional[QL_OS] = None,
+            archtype: Optional[QL_ARCH] = None,
             verbose: QL_VERBOSE = QL_VERBOSE.DEFAULT,
-            profile: str = None,
+            profile: Optional[Union[str, Mapping]] = None,
             console: bool = True,
-            log_file=None,
-            log_override=None,
+            log_file: Optional[str] = None,
+            log_override: Optional['Logger'] = None,
             log_plain: bool = False,
             multithread: bool = False,
-            filter = None,
+            filter: Optional[str] = None,
             stop: QL_STOP = QL_STOP.NONE,
             *,
             endian: Optional[QL_ENDIAN] = None,
             thumb: bool = False,
             libcache: bool = False
     ):
         """ Create a Qiling instance.
@@ -86,40 +86,43 @@
 
         """
         Qiling Framework Core Engine
         """
         ##############
         # argv setup #
         ##############
-        if argv is None:
-            argv = ['qilingcode']
+        if argv:
+            if code:
+                raise AttributeError('argv and code are mutually execlusive')
 
-        elif not os.path.exists(argv[0]):
-            raise QlErrorFileNotFound(f'Target binary not found: "{argv[0]}"')
+            target = argv[0]
+
+            if not os.path.isfile(target):
+                raise QlErrorFileNotFound(f'Target binary not found: "{target}"')
+        else:
+            # an empty argv list means we are going to execute a shellcode. to keep
+            # the 'path' api compatible, we insert a dummy placeholder
+
+            argv = ['']
 
         self._argv = argv
 
         ################
         # rootfs setup #
         ################
-        if not os.path.exists(rootfs):
+        if not os.path.isdir(rootfs):
             raise QlErrorFileNotFound(f'Target rootfs not found: "{rootfs}"')
 
         self._rootfs = rootfs
 
         #################
         # arch os setup #
         #################
-        if type(archtype) is str:
-            archtype = arch_convert(archtype)
 
-        if type(ostype) is str:
-            ostype = os_convert(ostype)
-
-        # if provided arch was invalid or not provided, guess arch and os
+        # if arch was not provided, guess arch and os
         if archtype is None:
             guessed_archtype, guessed_ostype, guessed_archendian = ql_guess_emu_env(self.path)
 
             archtype = guessed_archtype
 
             if ostype is None:
                 ostype = guessed_ostype
@@ -128,33 +131,36 @@
                 endian = guessed_archendian
 
         # if arch was set but os was not, try to guess it by arch
         elif ostype is None:
             ostype = arch_os_convert(archtype)
 
         # arch should have been determined by now; fail if not
-        if type(archtype) is not QL_ARCH:
-            raise QlErrorArch(f'Unknown or unsupported architecture: "{archtype}"')
+        if archtype is None:
+            raise QlErrorArch(f'Unknown or unsupported architecture')
 
         # os should have been determined by now; fail if not
-        if type(ostype) is not QL_OS:
-            raise QlErrorOsType(f'Unknown or unsupported operating system: "{ostype}"')
+        if ostype is None:
+            raise QlErrorOsType(f'Unknown or unsupported operating system')
 
         # if endianess is still undetermined, set it to little-endian.
         # this setting is ignored for architectures with predefined endianess
         if endian is None:
             endian = QL_ENDIAN.EL
 
         self._arch = select_arch(archtype, endian, thumb)(self)
 
         # Once we finish setting up arch, we can init QlCoreStructs and QlCoreHooks
         if not self.interpreter:
             QlCoreStructs.__init__(self, self.arch.endian, self.arch.bits)
             QlCoreHooks.__init__(self, self.uc)
 
+        # emulation has not been started yet
+        self._state = QL_STATE.NOT_SET
+
         ##########
         # Logger #
         ##########
         self._log_file_fd = setup_logger(self, log_file, console, log_override, log_plain)
 
         self.filter = filter
         self.verbose = verbose
@@ -490,14 +496,21 @@
             - `QL_STOP.STACK_POINTER` : Stop execution on a negative stackpointer
             - `QL_STOP.EXIT_TRAP`     : Stop execution when the pc value enters a guarded region
 
         Returns: configured options
         """
         return self._stop_options
 
+    @property
+    def emu_state(self) -> QL_STATE:
+        """Query emulation state.
+        """
+
+        return self._state
+
     def do_bin_patch(self):
         ba = self.loader.load_address
 
         for offset, code in self.patch_bin:
             self.mem.write(ba + offset, code)
 
     def do_lib_patch(self):
@@ -683,19 +696,19 @@
             self.os.restore(saved_states["os_context"])
 
         if "loader" in saved_states:
             self.loader.restore(saved_states["loader"])
 
     # Map "ql_path" to any objects which implements QlFsMappedObject.
     def add_fs_mapper(self, ql_path: Union["PathLike", str], real_dest):
-        self.os.fs_mapper.add_fs_mapping(ql_path, real_dest)
+        self.os.fs_mapper.add_mapping(ql_path, real_dest)
 
     # Remove "ql_path" mapping.
     def remove_fs_mapper(self, ql_path: Union["PathLike", str]):
-        self.os.fs_mapper.remove_fs_mapping(ql_path)
+        self.os.fs_mapper.remove_mapping(ql_path)
 
     # push to stack bottom, and update stack register
     def stack_push(self, data):
         return self.arch.stack_push(data)
 
     # pop from stack bottom, and update stack register
     def stack_pop(self):
@@ -710,25 +723,26 @@
     # NOTE: unlike stack_push(), this does not change stack register
     def stack_write(self, offset, data):
         return self.arch.stack_write(offset, data)
 
     # stop emulation
     def emu_stop(self):
         self.uc.emu_stop()
+        self._state = QL_STATE.STOPPED
 
     # stop emulation
     def stop(self):
         if self.multithread:
             self.os.thread_management.stop()
 
         elif self.baremetal:
             self.os.stop()
 
         else:
-            self.uc.emu_stop()
+            self.emu_stop()
 
     # start emulation
     def emu_start(self, begin: int, end: int, timeout: int = 0, count: int = 0):
         """Start emulation.
 
         Args:
             begin   : emulation starting address
@@ -745,13 +759,17 @@
         # by determining the endianess by address lsb. either way this condition should not be here
         if getattr(self.arch, '_init_thumb', False):
             begin |= 0b1
 
         # reset exception status before emulation starts
         self._internal_exception = None
 
+        self._state = QL_STATE.STARTED
+
         # effectively start the emulation. this returns only after uc.emu_stop is called
         self.uc.emu_start(begin, end, timeout, count)
 
+        self._state = QL_STATE.STOPPED
+
         # if an exception was raised during emulation, propagate it up
         if self.internal_exception is not None:
             raise self.internal_exception
```

### Comparing `qiling-1.4.5/qiling/core_hooks.py` & `qiling-1.4.6/qiling/core_hooks.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,33 +1,64 @@
 #!/usr/bin/env python3
-# 
+#
 # Cross Platform and Multi Architecture Advanced Binary Emulation Framework
 #
 
 ##############################################
 # These are part of the core.py Qiling class #
 # handling hooks                             #
 ##############################################
 
-import functools
+from __future__ import annotations
+
+from functools import wraps
 from typing import Any, Callable, MutableMapping, MutableSequence, Protocol
 from typing import TYPE_CHECKING
 
-from unicorn import Uc
-from unicorn.unicorn_const import *
+from unicorn.unicorn_const import (
+    UC_HOOK_INTR,
+    UC_HOOK_INSN,
+    UC_HOOK_CODE,
+    UC_HOOK_BLOCK,
+
+    UC_HOOK_MEM_READ_UNMAPPED,      # attempt to read from an unmapped memory location
+    UC_HOOK_MEM_WRITE_UNMAPPED,     # attempt to write to an unmapped memory location
+    UC_HOOK_MEM_FETCH_UNMAPPED,     # attempt to fetch from an unmapped memory location
+    UC_HOOK_MEM_UNMAPPED,           # any of the 3 above
+
+    UC_HOOK_MEM_READ_PROT,          # attempt to read from a non-readable memory location
+    UC_HOOK_MEM_WRITE_PROT,         # attempt to write to a write-protected memory location
+    UC_HOOK_MEM_FETCH_PROT,         # attempt to fetch from a non-executable memory location
+    UC_HOOK_MEM_PROT,               # any of the 3 above
+
+    UC_HOOK_MEM_READ_INVALID,       # UC_HOOK_MEM_READ_UNMAPPED | UC_HOOK_MEM_READ_PROT
+    UC_HOOK_MEM_WRITE_INVALID,      # UC_HOOK_MEM_WRITE_UNMAPPED | UC_HOOK_MEM_WRITE_INVALID
+    UC_HOOK_MEM_FETCH_INVALID,      # UC_HOOK_MEM_FETCH_UNMAPPED | UC_HOOK_MEM_FETCH_INVALID
+    UC_HOOK_MEM_INVALID,            # any of the 3 above
+
+    UC_HOOK_MEM_READ,               # valid memory read
+    UC_HOOK_MEM_WRITE,              # valid memory write
+    UC_HOOK_MEM_FETCH,              # valid instruction fetch
+    UC_HOOK_MEM_VALID,              # any of the 3 above
+
+    UC_HOOK_MEM_READ_AFTER,
+    UC_HOOK_INSN_INVALID
+)
 
 from .core_hooks_types import Hook, HookAddr, HookIntr, HookRet
 from .const import QL_HOOK_BLOCK
 from .exception import QlErrorCoreHook
 
 if TYPE_CHECKING:
+    from unicorn import Uc
     from qiling import Qiling
 
+
 class MemHookCallback(Protocol):
-    def __call__(self, __ql: 'Qiling', __access: int, __address: int, __size: int, __value: int, *__context: Any) -> Any:
+    def __call__(self, __ql: Qiling, __access: int, __address: int, __size: int, __value: int, *__context: Any) -> Any:
         """Memory access hook callback.
 
         Args:
             __ql      : the associated qiling instance
             __access  : the intercepted memory access type, one of UC_HOOK_MEM_* constants
             __addr    : the target memory location
             __size    : size of intercepted memory access
@@ -36,63 +67,65 @@
 
         Returns:
             an integer with `QL_HOOK_BLOCK` mask set to block execution of remaining hooks
             (if any) or `None`
         """
         pass
 
+
 class TraceHookCalback(Protocol):
-    def __call__(self, __ql: 'Qiling', __address: int, __size: int, *__context: Any) -> Any:
+    def __call__(self, __ql: Qiling, __address: int, __size: int, *__context: Any) -> Any:
         """Execution hook callback.
 
         Args:
             __ql      : the associated qiling instance
             __address : address of the instruction to be executed
             __size    : instruction size
             __context : additional context passed on hook creation. if no context was passed, this argument should be omitted
 
         Returns:
             an integer with `QL_HOOK_BLOCK` mask set to block execution of remaining hooks
             (if any) or `None`
         """
         pass
 
+
 class AddressHookCallback(Protocol):
-    def __call__(self, __ql: 'Qiling', *__context: Any) -> Any:
+    def __call__(self, __ql: Qiling, *__context: Any) -> Any:
         """Address hook callback.
 
         Args:
             __ql      : the associated qiling instance
             __context : additional context passed on hook creation. if no context was passed, this argument should be omitted
 
         Returns:
             an integer with `QL_HOOK_BLOCK` mask set to block execution of remaining hooks
             (if any) or `None`
         """
         pass
 
+
 class InterruptHookCallback(Protocol):
-    def __call__(self, __ql: 'Qiling', intno: int, *__context: Any) -> Any:
+    def __call__(self, __ql: Qiling, intno: int, *__context: Any) -> Any:
         """Interrupt hook callback.
 
         Args:
             __ql      : the associated qiling instance
             __intno   : the intercepted interrupt number
             __context : additional context passed on hook creation. if no context was passed, this argument should be omitted
 
         Returns:
             an integer with `QL_HOOK_BLOCK` mask set to block execution of remaining hooks
             (if any) or `None`
         """
         pass
 
 
-def hookcallback(ql: 'Qiling', callback: Callable):
-
-    functools.wraps(callback)
+def hookcallback(ql: Qiling, callback: Callable):
+    @wraps(callback)
     def wrapper(*args, **kwargs):
         try:
             return callback(*args, **kwargs)
         except (KeyboardInterrupt, Exception) as ex:
             ql.stop()
             ql._internal_exception = ex
 
@@ -109,18 +142,18 @@
 
         self._insn_hook: MutableMapping[int, MutableSequence[Hook]] = {}
         self._insn_hook_fuc: MutableMapping[int, int] = {}
 
         self._addr_hook: MutableMapping[int, MutableSequence[HookAddr]] = {}
         self._addr_hook_fuc: MutableMapping[int, int] = {}
 
-
     ########################
     # Callback definitions #
     ########################
+
     def _hook_intr_cb(self, uc: Uc, intno: int, pack_data) -> None:
         """Interrupt hooks dispatcher.
         """
 
         ql, hook_type = pack_data
         handled = False
 
@@ -138,15 +171,14 @@
 
                     if type(ret) is int and ret & QL_HOOK_BLOCK:
                         break
 
         if not handled:
             raise QlErrorCoreHook("_hook_intr_cb : not handled")
 
-
     def _hook_insn_cb(self, uc: Uc, *args):
         """Instruction hooks dispatcher.
         """
 
         *hook_args, (ql, insn_type) = args
         retval = None
 
@@ -162,15 +194,14 @@
 
                     if type(ret) is int and ret & QL_HOOK_BLOCK:
                         break
 
         # use the last return value received
         return retval
 
-
     def _hook_trace_cb(self, uc: Uc, addr: int, size: int, pack_data) -> None:
         """Code and block hooks dispatcher.
         """
 
         ql, hook_type = pack_data
 
         if hook_type in self._hook:
@@ -179,15 +210,14 @@
             for hook in hooks_list:
                 if hook.bound_check(addr, size):
                     ret = hook.call(ql, addr, size)
 
                     if type(ret) is int and ret & QL_HOOK_BLOCK:
                         break
 
-
     def _hook_mem_cb(self, uc: Uc, access: int, addr: int, size: int, value: int, pack_data):
         """Memory access hooks dispatcher.
         """
 
         ql, hook_type = pack_data
         handled = False
 
@@ -203,15 +233,14 @@
                         break
 
         if not handled and hook_type & (UC_HOOK_MEM_UNMAPPED | UC_HOOK_MEM_PROT):
             raise QlErrorCoreHook("_hook_mem_cb : not handled")
 
         return True
 
-
     def _hook_insn_invalid_cb(self, uc: Uc, pack_data) -> None:
         """Invalid instruction hooks dispatcher.
         """
 
         ql, hook_type = pack_data
         handled = False
 
@@ -224,15 +253,14 @@
 
                 if type(ret) is int and ret & QL_HOOK_BLOCK:
                     break
 
         if not handled:
             raise QlErrorCoreHook("_hook_insn_invalid_cb : not handled")
 
-
     def _hook_addr_cb(self, uc: Uc, addr: int, size: int, pack_data):
         """Address hooks dispatcher.
         """
 
         ql = pack_data
 
         if addr in self._addr_hook:
@@ -243,26 +271,25 @@
 
                 if type(ret) is int and ret & QL_HOOK_BLOCK:
                     break
 
     ###############
     # Class Hooks #
     ###############
+
     def _ql_hook_internal(self, hook_type: int, callback: Callable, context: Any, *args) -> int:
         _callback = hookcallback(self, callback)
 
         return self._h_uc.hook_add(hook_type, _callback, (self, context), 1, 0, *args)
 
-
     def _ql_hook_addr_internal(self, callback: Callable, address: int) -> int:
         _callback = hookcallback(self, callback)
 
         return self._h_uc.hook_add(UC_HOOK_CODE, _callback, self, address, address)
 
-
     def _ql_hook(self, hook_type: int, h: Hook, *args) -> None:
 
         def __handle_intr(t: int) -> None:
             if t not in self._hook_fuc:
                 self._hook_fuc[t] = self._ql_hook_internal(t, self._hook_intr_cb, t)
 
             if t not in self._hook:
@@ -326,15 +353,14 @@
             (UC_HOOK_INSN_INVALID,       __handle_invalid_insn)
         )
 
         for t, handler in type_handlers:
             if hook_type & t:
                 handler(t)
 
-
     def ql_hook(self, hook_type: int, callback: Callable, user_data: Any = None, begin: int = 1, end: int = 0, *args) -> HookRet:
         """Intercept certain emulation events within a specified range.
 
         Args:
             hook_type : event type to intercept; this argument is used as a bitmap and may encode multiple
             events to hook with the same calback. see UC_HOOK_* constants for available events
             callback  : a method to call upon interception; callback signature may vary
@@ -351,15 +377,14 @@
         """
 
         hook = Hook(callback, user_data, begin, end)
         self._ql_hook(hook_type, hook, *args)
 
         return HookRet(self, hook_type, hook)
 
-
     def hook_code(self, callback: TraceHookCalback, user_data: Any = None, begin: int = 1, end: int = 0) -> HookRet:
         """Intercept assembly instructions before they get executed.
 
         Args:
             callback  : a method to call upon interception
             user_data : an additional context to pass to callback (default: `None`)
             begin     : start of memory range to watch
@@ -370,20 +395,18 @@
 
         Returns:
             Hook handle
         """
 
         return self.ql_hook(UC_HOOK_CODE, callback, user_data, begin, end)
 
-
     # TODO: remove; this is a special case of hook_intno(-1)
     def hook_intr(self, callback, user_data=None, begin=1, end=0):
         return self.ql_hook(UC_HOOK_INTR, callback, user_data, begin, end)
 
-
     def hook_block(self, callback: TraceHookCalback, user_data: Any = None, begin: int = 1, end: int = 0) -> HookRet:
         """Intercept landings in new basic blocks in a specified range.
 
         Args:
             callback  : a method to call upon interception
             user_data : an additional context to pass to callback (default: `None`)
             begin     : start of memory range to watch
@@ -394,15 +417,14 @@
 
         Returns:
             Hook handle
         """
 
         return self.ql_hook(UC_HOOK_BLOCK, callback, user_data, begin, end)
 
-
     def hook_mem_unmapped(self, callback: MemHookCallback, user_data: Any = None, begin: int = 1, end: int = 0) -> HookRet:
         """Intercept illegal accesses to unmapped memory in a specified range.
 
         Args:
             callback  : a method to call upon interception
             user_data : an additional context to pass to callback (default: `None`)
             begin     : start of memory range to watch
@@ -413,15 +435,14 @@
 
         Returns:
             Hook handle
         """
 
         return self.ql_hook(UC_HOOK_MEM_UNMAPPED, callback, user_data, begin, end)
 
-
     def hook_mem_read_invalid(self, callback: MemHookCallback, user_data: Any = None, begin: int = 1, end: int = 0) -> HookRet:
         """Intercept illegal reading attempts from a specified range.
 
         Args:
             callback  : a method to call upon interception
             user_data : an additional context to pass to callback (default: `None`)
             begin     : start of memory range to watch
@@ -432,15 +453,14 @@
 
         Returns:
             Hook handle
         """
 
         return self.ql_hook(UC_HOOK_MEM_READ_INVALID, callback, user_data, begin, end)
 
-
     def hook_mem_write_invalid(self, callback: MemHookCallback, user_data: Any = None, begin: int = 1, end: int = 0) -> HookRet:
         """Intercept illegal writing attempts to a specified range.
 
         Args:
             callback  : a method to call upon interception
             user_data : an additional context to pass to callback (default: `None`)
             begin     : start of memory range to watch
@@ -451,15 +471,14 @@
 
         Returns:
             Hook handle
         """
 
         return self.ql_hook(UC_HOOK_MEM_WRITE_INVALID, callback, user_data, begin, end)
 
-
     def hook_mem_fetch_invalid(self, callback: MemHookCallback, user_data: Any = None, begin: int = 1, end: int = 0) -> HookRet:
         """Intercept illegal code fetching attempts from a specified range.
 
         Args:
             callback  : a method to call upon interception
             user_data : an additional context to pass to callback (default: `None`)
             begin     : start of memory range to watch
@@ -470,15 +489,14 @@
 
         Returns:
             Hook handle
         """
 
         return self.ql_hook(UC_HOOK_MEM_FETCH_INVALID, callback, user_data, begin, end)
 
-
     def hook_mem_valid(self, callback: MemHookCallback, user_data: Any = None, begin: int = 1, end: int = 0) -> HookRet:
         """Intercept benign memory accesses within a specified range.
         This is equivalent to hooking memory reads, writes and fetches.
 
         Args:
             callback  : a method to call upon interception
             user_data : an additional context to pass to callback (default: `None`)
@@ -490,15 +508,14 @@
 
         Returns:
             Hook handle
         """
 
         return self.ql_hook(UC_HOOK_MEM_VALID, callback, user_data, begin, end)
 
-
     def hook_mem_invalid(self, callback: MemHookCallback, user_data: Any = None, begin: int = 1, end: int = 0) -> HookRet:
         """Intercept invalid memory accesses within a specified range.
         This is equivalent to hooking invalid memory reads, writes and fetches.
 
         Args:
             callback  : a method to call upon interception
             user_data : an additional context to pass to callback (default: `None`)
@@ -510,15 +527,14 @@
 
         Returns:
             Hook handle
         """
 
         return self.ql_hook(UC_HOOK_MEM_INVALID, callback, user_data, begin, end)
 
-
     def hook_address(self, callback: AddressHookCallback, address: int, user_data: Any = None) -> HookRet:
         """Intercept execution from a certain memory address.
 
         Args:
             callback  : a method to call upon interception
             address   : memory location to watch
             user_data : an additional context to pass to callback (default: `None`)
@@ -536,15 +552,14 @@
             self._addr_hook[address] = []
 
         self._addr_hook[address].append(hook)
 
         # note: assuming 0 is not a valid hook type
         return HookRet(self, 0, hook)
 
-
     def hook_intno(self, callback: InterruptHookCallback, intno: int, user_data: Any = None) -> HookRet:
         """Intercept interrupts.
 
         Args:
             callback  : a method to call upon interception
             intono    : interrupt vector number to intercept, or -1 for any
             user_data : an additional context to pass to callback (default: `None`)
@@ -554,15 +569,14 @@
         """
 
         hook = HookIntr(callback, intno, user_data)
         self._ql_hook(UC_HOOK_INTR, hook)
 
         return HookRet(self, UC_HOOK_INTR, hook)
 
-
     def hook_mem_read(self, callback: MemHookCallback, user_data: Any = None, begin: int = 1, end: int = 0) -> HookRet:
         """Intercept benign memory reads from a specified range.
 
         Args:
             callback  : a method to call upon interception
             user_data : an additional context to pass to callback (default: `None`)
             begin     : start of memory range to watch
@@ -573,15 +587,14 @@
 
         Returns:
             Hook handle
         """
 
         return self.ql_hook(UC_HOOK_MEM_READ, callback, user_data, begin, end)
 
-
     def hook_mem_write(self, callback: MemHookCallback, user_data: Any = None, begin: int = 1, end: int = 0) -> HookRet:
         """Intercept benign memory writes to a specified range.
 
         Args:
             callback  : a method to call upon interception
             user_data : an additional context to pass to callback (default: `None`)
             begin     : start of memory range to watch
@@ -592,15 +605,14 @@
 
         Returns:
             Hook handle
         """
 
         return self.ql_hook(UC_HOOK_MEM_WRITE, callback, user_data, begin, end)
 
-
     def hook_mem_fetch(self, callback: MemHookCallback, user_data: Any = None, begin: int = 1, end: int = 0) -> HookRet:
         """Intercept benign code fetches from a specified range.
 
         Args:
             callback  : a method to call upon interception
             user_data : an additional context to pass to callback (default: `None`)
             begin     : start of memory range to watch
@@ -611,15 +623,14 @@
 
         Returns:
             Hook handle
         """
 
         return self.ql_hook(UC_HOOK_MEM_FETCH, callback, user_data, begin, end)
 
-
     def hook_insn(self, callback, insn_type: int, user_data: Any = None, begin: int = 1, end: int = 0) -> HookRet:
         """Intercept execution of a certain instruction type within a specified range.
 
         Args:
             callback  : a method to call upon interception; the callback arguments list differs
             based on the instruction type
             insn_type : instruction type to intercept
@@ -633,15 +644,14 @@
 
         Returns:
             Hook handle
         """
 
         return self.ql_hook(UC_HOOK_INSN, callback, user_data, begin, end, insn_type)
 
-
     def hook_del(self, hret: HookRet) -> None:
         """Unregister an existing hook and release its resources.
 
         Args:
             hret : hook handle
         """
 
@@ -688,28 +698,26 @@
             __handle_addr(h.addr)
             return
 
         for t, handler in type_handlers:
             if hook_type & t:
                 handler(t)
 
-
     def clear_hooks(self):
         for ptr in self._hook_fuc.values():
             self._h_uc.hook_del(ptr)
 
         for ptr in self._insn_hook_fuc.values():
             self._h_uc.hook_del(ptr)
 
         for ptr in self._addr_hook_fuc.values():
             self._h_uc.hook_del(ptr)
 
         self.clear_ql_hooks()
 
-
     def clear_ql_hooks(self):
         self._hook = {}
         self._hook_fuc = {}
 
         self._insn_hook = {}
         self._insn_hook_fuc = {}
```

### Comparing `qiling-1.4.5/qiling/core_hooks_types.py` & `qiling-1.4.6/qiling/core_hooks_types.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/core_struct.py` & `qiling-1.4.6/qiling/core_struct.py`

 * *Files 20% similar despite different names*

```diff
@@ -15,85 +15,85 @@
 from .const import QL_ENDIAN
 from .exception import QlErrorStructConversion
 
 ReadableBuffer = Union[bytes, bytearray, memoryview]
 
 # Don't assume self is Qiling.
 class QlCoreStructs:
-	def __init__(self, endian: QL_ENDIAN, bit: int):
-		modifier = {
-			QL_ENDIAN.EL: '<',
-			QL_ENDIAN.EB: '>'
-		}[endian]
+    def __init__(self, endian: QL_ENDIAN, bit: int):
+        modifier = {
+            QL_ENDIAN.EL: '<',
+            QL_ENDIAN.EB: '>'
+        }[endian]
 
-		self._fmt8   = f'{modifier}B'
-		self._fmt8s  = f'{modifier}b'
-		self._fmt16  = f'{modifier}H'
-		self._fmt16s = f'{modifier}h'
-		self._fmt32  = f'{modifier}I'
-		self._fmt32s = f'{modifier}i'
-		self._fmt64  = f'{modifier}Q'
-		self._fmt64s = f'{modifier}q'
+        self._fmt8   = f'{modifier}B'
+        self._fmt8s  = f'{modifier}b'
+        self._fmt16  = f'{modifier}H'
+        self._fmt16s = f'{modifier}h'
+        self._fmt32  = f'{modifier}I'
+        self._fmt32s = f'{modifier}i'
+        self._fmt64  = f'{modifier}Q'
+        self._fmt64s = f'{modifier}q'
 
-		handlers = {
-			64 : (self.pack64, self.pack64s, self.unpack64, self.unpack64s),
-			32 : (self.pack32, self.pack32s, self.unpack32, self.unpack32s),
-			16 : (self.pack16, self.pack16s, self.unpack16, self.unpack16s),
-		}
+        handlers = {
+            64 : (self.pack64, self.pack64s, self.unpack64, self.unpack64s),
+            32 : (self.pack32, self.pack32s, self.unpack32, self.unpack32s),
+            16 : (self.pack16, self.pack16s, self.unpack16, self.unpack16s),
+        }
 
-		if bit not in handlers:
-			raise QlErrorStructConversion("Unsupported Qiling struct conversion")
+        if bit not in handlers:
+            raise QlErrorStructConversion("Unsupported Qiling struct conversion")
 
-		p, ps, up, ups = handlers[bit]
+        p, ps, up, ups = handlers[bit]
 
-		self.pack    = p
-		self.packs   = ps
-		self.unpack  = up
-		self.unpacks = ups
+        self.pack    = p
+        self.packs   = ps
+        self.unpack  = up
+        self.unpacks = ups
 
-	def pack64(self, x: int, /) -> bytes:
-		return struct.pack(self._fmt64, x)
+    def pack64(self, x: int, /) -> bytes:
+        return struct.pack(self._fmt64, x)
 
-	def pack64s(self, x: int, /) -> bytes:
-		return struct.pack(self._fmt64s, x)
+    def pack64s(self, x: int, /) -> bytes:
+        return struct.pack(self._fmt64s, x)
 
-	def unpack64(self, x: ReadableBuffer, /) -> int:
-		return struct.unpack(self._fmt64, x)[0]
+    def unpack64(self, x: ReadableBuffer, /) -> int:
+        return struct.unpack(self._fmt64, x)[0]
 
-	def unpack64s(self, x: ReadableBuffer, /) -> int:
-		return struct.unpack(self._fmt64s, x)[0]
+    def unpack64s(self, x: ReadableBuffer, /) -> int:
+        return struct.unpack(self._fmt64s, x)[0]
 
-	def pack32(self, x: int, /) -> bytes:
-		return struct.pack(self._fmt32, x)
+    def pack32(self, x: int, /) -> bytes:
+        return struct.pack(self._fmt32, x)
 
-	def pack32s(self, x: int, /) -> bytes:
-		return struct.pack(self._fmt32s, x)
+    def pack32s(self, x: int, /) -> bytes:
+        return struct.pack(self._fmt32s, x)
 
-	def unpack32(self, x: ReadableBuffer, /) -> int:
-		return struct.unpack(self._fmt32, x)[0]
+    def unpack32(self, x: ReadableBuffer, /) -> int:
+        return struct.unpack(self._fmt32, x)[0]
 
-	def unpack32s(self, x: ReadableBuffer, /) -> int:
-		return struct.unpack(self._fmt32s, x)[0]
+    def unpack32s(self, x: ReadableBuffer, /) -> int:
+        return struct.unpack(self._fmt32s, x)[0]
 
-	def pack16(self, x: int, /) -> bytes:
-		return struct.pack(self._fmt16, x)
+    def pack16(self, x: int, /) -> bytes:
+        return struct.pack(self._fmt16, x)
 
-	def pack16s(self, x: int, /) -> bytes:
-		return struct.pack(self._fmt16s, x)
+    def pack16s(self, x: int, /) -> bytes:
+        return struct.pack(self._fmt16s, x)
 
-	def unpack16(self, x: ReadableBuffer, /) -> int:
-		return struct.unpack(self._fmt16, x)[0]
+    def unpack16(self, x: ReadableBuffer, /) -> int:
+        return struct.unpack(self._fmt16, x)[0]
 
-	def unpack16s(self, x: ReadableBuffer, /) -> int:
-		return struct.unpack(self._fmt16s, x)[0]
+    def unpack16s(self, x: ReadableBuffer, /) -> int:
+        return struct.unpack(self._fmt16s, x)[0]
 
-	def pack8(self, x: int, /) -> bytes:
-		return struct.pack(self._fmt8, x)
+    def pack8(self, x: int, /) -> bytes:
+        return struct.pack(self._fmt8, x)
 
-	def pack8s(self, x: int, /) -> bytes:
-		return struct.pack(self._fmt8s, x)
+    def pack8s(self, x: int, /) -> bytes:
+        return struct.pack(self._fmt8s, x)
 
-	def unpack8(self, x: ReadableBuffer, /) -> int:
-		return struct.unpack(self._fmt8, x)[0]
+    def unpack8(self, x: ReadableBuffer, /) -> int:
+        return struct.unpack(self._fmt8, x)[0]
 
-	def unpack8s(self, x: ReadableBuffer, /) -> int:
-		return struct.unpack(self._fmt8s, x)[0]
+    def unpack8s(self, x: ReadableBuffer, /) -> int:
+        return struct.unpack(self._fmt8s, x)[0]
```

### Comparing `qiling-1.4.5/qiling/debugger/disassember.py` & `qiling-1.4.6/qiling/debugger/disassember.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/debugger/gdb/gdb.py` & `qiling-1.4.6/qiling/debugger/gdb/gdb.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     UC_ERR_READ_UNMAPPED,  UC_ERR_WRITE_UNMAPPED,  UC_ERR_FETCH_UNMAPPED,
     UC_ERR_READ_PROT,      UC_ERR_WRITE_PROT,      UC_ERR_FETCH_PROT,
     UC_ERR_READ_UNALIGNED, UC_ERR_WRITE_UNALIGNED, UC_ERR_FETCH_UNALIGNED,
     UC_ERR_INSN_INVALID
 )
 
 from qiling import Qiling
-from qiling.const import QL_ARCH, QL_ENDIAN, QL_OS
+from qiling.const import QL_ARCH, QL_ENDIAN, QL_OS, QL_STATE
 from qiling.debugger import QlDebugger
 from qiling.debugger.gdb.xmlregs import QlGdbFeatures
 from qiling.debugger.gdb.utils import QlGdbUtils
 from qiling.os.linux.procfs import QlProcFS
 
 # gdb logging prompt
 PROMPT = r'gdb>'
@@ -74,44 +74,50 @@
 
         if type(port) is str:
             port = int(port, 0)
 
         self.ip = ip
         self.port = port
 
-        if ql.baremetal:
-            load_address = ql.loader.load_address
-            exit_point = load_address + os.path.getsize(ql.path)
-        elif ql.code:
-            load_address = ql.os.entry_point
-            exit_point = load_address + len(ql.code)
-        else:
-            load_address = ql.loader.load_address
-            exit_point = load_address + os.path.getsize(ql.path)
-
-        if ql.baremetal:
-            entry_point = ql.loader.entry_point
-        elif ql.os.type in (QL_OS.LINUX, QL_OS.FREEBSD) and not ql.code:
-            entry_point = ql.os.elf_entry
-        else:
-            entry_point = ql.os.entry_point
-
-        # though linkers set the entry point LSB to indicate arm thumb mode, the
-        # effective entry point address is aligned. make sure we have it aligned
-        if hasattr(ql.arch, 'is_thumb'):
-            entry_point &= ~0b1
-
-        # Only part of the binary file will be debugged.
-        if ql.entry_point is not None:
-            entry_point = ql.entry_point
+        def __get_attach_addr() -> int:
+            if ql.baremetal:
+                entry_point = ql.loader.entry_point
 
-        if ql.exit_point is not None:
-            exit_point = ql.exit_point
+            elif ql.os.type in (QL_OS.LINUX, QL_OS.FREEBSD) and not ql.code:
+                entry_point = ql.os.elf_entry
 
-        self.gdb = QlGdbUtils(ql, entry_point, exit_point)
+            else:
+                entry_point = ql.os.entry_point
+
+            # though linkers set the entry point LSB to indicate arm thumb mode, the
+            # effective entry point address is aligned. make sure we have it aligned
+            if hasattr(ql.arch, 'is_thumb'):
+                entry_point &= ~0b1
+
+            return entry_point
+
+        def __get_detach_addr() -> int:
+            if ql.baremetal:
+                base = ql.loader.load_address
+                size = os.path.getsize(ql.path)
+
+            elif ql.code:
+                base = ql.os.entry_point
+                size = len(ql.code)
+
+            else:
+                base = ql.loader.load_address
+                size = os.path.getsize(ql.path)
+
+            return base + size
+
+        attach_addr = __get_attach_addr() if ql.entry_point is None else ql.entry_point
+        detach_addr = __get_detach_addr() if ql.exit_point is None else ql.exit_point
+
+        self.gdb = QlGdbUtils(ql, attach_addr, detach_addr)
 
         self.features = QlGdbFeatures(self.ql.arch.type, self.ql.os.type)
         self.regsmap = self.features.regsmap
 
         self.fake_procfs: MutableMapping[int, IO] = {}
 
     def run(self):
@@ -289,19 +295,19 @@
         def handle_m(subcmd: str) -> Reply:
             """Read target memory.
             """
 
             addr, size = (int(p, 16) for p in subcmd.split(','))
 
             try:
-                data = self.ql.mem.read(addr, size).hex()
-            except UcError:
-                return 'E14'
+                data = self.ql.mem.read(addr, size)
+            except UcError as ex:
+                return f'E{ex.errno:02d}'
             else:
-                return data
+                return data.hex()
 
         def handle_M(subcmd: str) -> Reply:
             """Write target memory.
             """
 
             addr, data = subcmd.split(',')
             size, data = data.split(':')
@@ -309,16 +315,16 @@
             addr = int(addr, 16)
             data = bytes.fromhex(data)
 
             assert len(data) == size
 
             try:
                 self.ql.mem.write(addr, data)
-            except UcError:
-                return 'E01'
+            except UcError as ex:
+                return f'E{ex.errno:02d}'
             else:
                 return REPLY_OK
 
         def handle_p(subcmd: str) -> Reply:
             """Read register value by index.
             """
 
@@ -669,14 +675,19 @@
 
         def handle_s(subcmd: str) -> Reply:
             """Perform a single step.
             """
 
             self.gdb.resume_emu(steps=1)
 
+            # if emulation has been stopped, signal program termination
+            if self.ql.emu_state is QL_STATE.STOPPED:
+                return f'S{SIGTERM:02x}'
+
+            # otherwise, this is just single stepping
             return f'S{SIGTRAP:02x}'
 
         def handle_X(subcmd: str) -> Reply:
             """Write data to memory.
             """
 
             params, data = subcmd.split(':', maxsplit=1)
@@ -684,16 +695,16 @@
 
             if length != len(data):
                 return 'E00'
 
             try:
                 if data:
                     self.ql.mem.write(addr, data.encode(ENCODING))
-            except UcError:
-                return 'E01'
+            except UcError as ex:
+                return f'E{ex.errno:02d}'
             else:
                 return REPLY_OK
 
         def handle_Z(subcmd: str) -> Reply:
             """Insert breakpoints or watchpoints.
             """
 
@@ -828,15 +839,15 @@
             # remote connection closed
             if not incoming:
                 break
 
             buffer += incoming
 
             # discard incoming acks
-            if buffer[0:1] == REPLY_ACK:
+            if buffer.startswith(REPLY_ACK):
                 del buffer[0]
 
             packet = pattern.match(buffer)
 
             # if there is no match, the rest of the packet might be missing
             if not packet:
                 continue
```

### Comparing `qiling-1.4.5/qiling/debugger/gdb/utils.py` & `qiling-1.4.6/qiling/debugger/gdb/utils.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/debugger/gdb/xml/a8086/gdb_init_real_mode.txt` & `qiling-1.4.6/qiling/debugger/gdb/xml/a8086/gdb_init_real_mode.txt`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/debugger/gdb/xml/a8086/i386-32bit.xml` & `qiling-1.4.6/qiling/debugger/gdb/xml/a8086/i386-32bit.xml`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/debugger/gdb/xml/arm/arm-core.xml` & `qiling-1.4.6/qiling/debugger/gdb/xml/arm/arm-core.xml`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/debugger/gdb/xml/arm/arm-fpa.xml` & `qiling-1.4.6/qiling/debugger/gdb/xml/arm/arm-fpa.xml`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/debugger/gdb/xml/arm/arm-m-profile.xml` & `qiling-1.4.6/qiling/debugger/gdb/xml/arm/arm-m-profile.xml`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/debugger/gdb/xml/arm/arm-vfpv2.xml` & `qiling-1.4.6/qiling/debugger/gdb/xml/arm/arm-vfpv2.xml`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/debugger/gdb/xml/arm/arm-vfpv3.xml` & `qiling-1.4.6/qiling/debugger/gdb/xml/arm/arm-vfpv3.xml`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/debugger/gdb/xml/arm/target.xml` & `qiling-1.4.6/qiling/debugger/gdb/xml/arm/target.xml`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/debugger/gdb/xml/arm/xscale-iwmmxt.xml` & `qiling-1.4.6/qiling/debugger/gdb/xml/arm/xscale-iwmmxt.xml`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/debugger/gdb/xml/arm64/aarch64-core.xml` & `qiling-1.4.6/qiling/debugger/gdb/xml/arm64/aarch64-core.xml`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/debugger/gdb/xml/arm64/aarch64-fpu.xml` & `qiling-1.4.6/qiling/debugger/gdb/xml/arm64/aarch64-fpu.xml`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/debugger/gdb/xml/arm64/target.xml` & `qiling-1.4.6/qiling/debugger/gdb/xml/arm64/target.xml`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/debugger/gdb/xml/mips/mips-cpu.xml` & `qiling-1.4.6/qiling/debugger/gdb/xml/mips/mips-cpu.xml`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/debugger/gdb/xml/mips/mips-fpu.xml` & `qiling-1.4.6/qiling/debugger/gdb/xml/mips/mips-fpu.xml`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/debugger/gdb/xml/mips/target.xml` & `qiling-1.4.6/qiling/debugger/gdb/xml/mips/target.xml`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/debugger/gdb/xml/x86/32bit-avx.xml` & `qiling-1.4.6/qiling/debugger/gdb/xml/x86/32bit-avx.xml`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/debugger/gdb/xml/x86/32bit-avx512.xml` & `qiling-1.4.6/qiling/debugger/gdb/xml/x86/32bit-avx512.xml`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/debugger/gdb/xml/x86/32bit-core.xml` & `qiling-1.4.6/qiling/debugger/gdb/xml/x86/32bit-core.xml`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/debugger/gdb/xml/x86/32bit-mpx.xml` & `qiling-1.4.6/qiling/debugger/gdb/xml/x86/32bit-mpx.xml`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/debugger/gdb/xml/x86/32bit-sse.xml` & `qiling-1.4.6/qiling/debugger/gdb/xml/x86/32bit-sse.xml`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/debugger/gdb/xml/x8664/64bit-avx.xml` & `qiling-1.4.6/qiling/debugger/gdb/xml/x8664/64bit-avx.xml`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/debugger/gdb/xml/x8664/64bit-avx512.xml` & `qiling-1.4.6/qiling/debugger/gdb/xml/x8664/64bit-avx512.xml`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/debugger/gdb/xml/x8664/64bit-core.xml` & `qiling-1.4.6/qiling/debugger/gdb/xml/x8664/64bit-core.xml`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/debugger/gdb/xml/x8664/64bit-mpx.xml` & `qiling-1.4.6/qiling/debugger/gdb/xml/x8664/64bit-mpx.xml`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/debugger/gdb/xml/x8664/64bit-sse.xml` & `qiling-1.4.6/qiling/debugger/gdb/xml/x8664/64bit-sse.xml`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/debugger/gdb/xmlregs.py` & `qiling-1.4.6/qiling/debugger/gdb/xmlregs.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/debugger/qdb/arch/arch.py` & `qiling-1.4.6/qiling/debugger/qdb/arch/arch.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/debugger/qdb/arch/arch_arm.py` & `qiling-1.4.6/qiling/debugger/qdb/arch/arch_arm.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/debugger/qdb/arch/arch_mips.py` & `qiling-1.4.6/qiling/debugger/qdb/arch/arch_mips.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/debugger/qdb/arch/arch_x86.py` & `qiling-1.4.6/qiling/debugger/qdb/arch/arch_x86.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/debugger/qdb/arch/arch_x8664.py` & `qiling-1.4.6/qiling/debugger/qdb/arch/arch_x8664.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/debugger/qdb/branch_predictor/branch_predictor.py` & `qiling-1.4.6/qiling/debugger/qdb/branch_predictor/branch_predictor.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/debugger/qdb/branch_predictor/branch_predictor_arm.py` & `qiling-1.4.6/qiling/debugger/qdb/branch_predictor/branch_predictor_arm.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/debugger/qdb/branch_predictor/branch_predictor_mips.py` & `qiling-1.4.6/qiling/debugger/qdb/branch_predictor/branch_predictor_mips.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/debugger/qdb/branch_predictor/branch_predictor_x86.py` & `qiling-1.4.6/qiling/debugger/qdb/branch_predictor/branch_predictor_x86.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/debugger/qdb/branch_predictor/branch_predictor_x8664.py` & `qiling-1.4.6/qiling/debugger/qdb/branch_predictor/branch_predictor_x8664.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/debugger/qdb/context.py` & `qiling-1.4.6/qiling/debugger/qdb/context.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from typing import Optional
 
 from unicorn import UC_ERR_READ_UNMAPPED
 import unicorn
 
 from capstone import CsInsn
 
-from .misc import read_int
+from .misc import read_int, InvalidInsn
 
 class Context:
     """
     base class for accessing context of running qiling instance
     """
 
     def __init__(self, ql):
@@ -44,17 +44,17 @@
         """
         helper function for disassembling
         """
 
         md = self.ql.arch.disassembler
         md.detail = detail
 
-        if (addr := self.read_insn(address)):
-            return next(md.disasm(addr, address), None)
-        return None
+        if (bytes_read := self.read_insn(address)):
+            return next(md.disasm(bytes_read, address), InvalidInsn(bytes_read, address))
+        return InvalidInsn(bytes_read, address)
 
     def try_read(self, address: int, size: int) -> Optional[bytes]:
         """
         try to read data from ql.mem
         """
 
         result = None
```

### Comparing `qiling-1.4.5/qiling/debugger/qdb/memory.py` & `qiling-1.4.6/qiling/debugger/qdb/memory.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/debugger/qdb/misc.py` & `qiling-1.4.6/qiling/debugger/qdb/misc.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 #!/usr/bin/env python3
 #
 # Cross Platform and Multi Architecture Advanced Binary Emulation Framework
 #
 
 from typing import AnyStr, Callable, Optional
 
+from dataclasses import dataclass
+
 import ast
 
 def check_and_eval(line: str):
     """
     This function will valid all type of nodes and evaluate it if nothing went wrong
     """
 
@@ -21,14 +23,27 @@
 
     checker = AST_checker()
     ast_tree = ast.parse(line)
     checker.visit(ast_tree)
 
     return eval(line)
 
+@dataclass
+class InvalidInsn:
+    """
+    class for displaying invalid instruction
+    """
+    bytes: bytes
+    address: bytes
+    mnemonic: str = 'invalid'
+    op_str: str = ''
+
+    def __post_init__(self):
+        self.size = len(self.bytes)
+
 
 class Breakpoint:
     """
     dummy class for breakpoint
     """
     def __init__(self, addr: int):
         self.addr = addr
```

### Comparing `qiling-1.4.5/qiling/debugger/qdb/qdb.py` & `qiling-1.4.6/qiling/debugger/qdb/qdb.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,18 +74,21 @@
                 self.do_context()
 
         self.ql.hook_code(bp_handler, self.bp_list)
 
         if self.ql.os.type == QL_OS.BLOB:
             self.ql.loader.entry_point = self.ql.loader.load_address
 
-        elif init_hook and self.ql.loader.entry_point != init_hook:
+        elif init_hook and self.ql.loader.entry_point != int(init_hook, 0):
             self.do_breakpoint(init_hook)
 
-        self.cur_addr = self.ql.loader.entry_point
+        if self.ql.entry_point:
+            self.cur_addr = self.ql.entry_point
+        else:
+            self.cur_addr = self.ql.loader.entry_point
 
         self.init_state = self.ql.save()
 
         if self._script:
             run_qdb_script(self, self._script)
         else:
             self.do_context()
@@ -112,15 +115,15 @@
         internal function for emulating instruction
         """
 
         if not address:
             address = self.cur_addr
 
         if getattr(self.ql.arch, 'is_thumb', False):
-            address |= 1
+            address |= 0b1
 
         # assume we're running PE if on Windows
         if self.ql.os.type == QL_OS.WINDOWS:
             self.ql.count = count
             self.ql.entry_point = address
             self.ql.os.run()
 
@@ -153,14 +156,15 @@
         """
 
         def inner(self, *args, **kwargs):
             if self.ql is None:
                 qdb_print(QDB_MSG.ERROR, "The program is not being run.")
             else:
                 func(self, *args, **kwargs)
+
         return inner
 
     def parseline(self, line: str) -> Tuple[Optional[str], Optional[str], str]:
         """
         Parse the line into a command name and a string containing
         the arguments.  Returns a tuple containing (command, args, line).
         'command' and 'args' may be None if the line couldn't be parsed.
@@ -209,25 +213,27 @@
         """
 
         self._run()
 
     @SnapshotManager.snapshot
     @save_reg_dump
     @check_ql_alive
-    def do_step_in(self, *args) -> Optional[bool]:
+    def do_step_in(self, step: str = '', *args) -> Optional[bool]:
         """
         execute one instruction at a time, will enter subroutine
         """
-
         prophecy = self.predictor.predict()
 
         if prophecy.where is True:
-            return True
+            qdb_print(QDB_MSG.INFO, 'program exited due to code end hitted')
+            self.do_context()
+            return False
+
+        step = 1 if step == '' else int(step)
 
-        step = 1
         # make sure follow branching
         if prophecy.going is True and self.ql.arch.type == QL_ARCH.MIPS:
             step += 1
 
         self._run(count=step)
         self.do_context()
 
@@ -570,15 +576,14 @@
         """
         handle Ctrl+D
         """
 
         if input(f"{color.RED}[!] Are you sure about saying good bye ~ ? [Y/n]{color.END} ").strip() == "Y":
             self.do_quit()
 
-
     do_r = do_run
     do_s = do_step_in
     do_n = do_step_over
     do_a = do_show_args
     do_j = do_jump
     do_m = do_mark
     do_q = do_quit
```

### Comparing `qiling-1.4.5/qiling/debugger/qdb/render/render.py` & `qiling-1.4.6/qiling/debugger/qdb/render/render.py`

 * *Files 2% similar despite different names*

```diff
@@ -153,14 +153,15 @@
     def print_asm(self, insn: CsInsn, to_jump: bool = False) -> None:
         """
         helper function for printing assembly instructions, indicates where we are and the branch prediction
         provided by BranchPredictor
         """
 
         opcode = "".join(f"{b:02x}" for b in insn.bytes)
+
         trace_line = f"0x{insn.address:08x} │ {opcode:15s} {insn.mnemonic:10} {insn.op_str:35s}"
 
         cursor = "►" if self.cur_addr == insn.address else " "
 
         jump_sign = f"{color.RED}✓{color.END}" if to_jump else " "
 
         print(f"{jump_sign}  {cursor}   {color.DARKGRAY}{trace_line}{color.END}")
@@ -207,20 +208,17 @@
 
         lines = {}
         past_list = []
         from_addr = self.cur_addr - self.disasm_num
         to_addr = self.cur_addr + self.disasm_num
 
         cur_addr = from_addr
-        while cur_addr != to_addr:
+        while cur_addr <= to_addr:
             insn = self.disasm(cur_addr)
-            # cur_addr += self.arch_insn_size
             cur_addr += insn.size
-            if not insn:
-                continue
             past_list.append(insn)
 
         bk_list = []
         fd_list = []
         cur_insn = None
         for each in past_list:
             if each.address < self.cur_addr:
```

### Comparing `qiling-1.4.5/qiling/debugger/qdb/render/render_arm.py` & `qiling-1.4.6/qiling/debugger/qdb/render/render_arm.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/debugger/qdb/render/render_mips.py` & `qiling-1.4.6/qiling/debugger/qdb/render/render_mips.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/debugger/qdb/render/render_x86.py` & `qiling-1.4.6/qiling/debugger/qdb/render/render_x86.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/debugger/qdb/render/render_x8664.py` & `qiling-1.4.6/qiling/debugger/qdb/render/render_x8664.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/debugger/qdb/utils.py` & `qiling-1.4.6/qiling/debugger/qdb/utils.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/debugger/utils.py` & `qiling-1.4.6/qiling/debugger/utils.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/exception.py` & `qiling-1.4.6/qiling/exception.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/extensions/afl/afl.py` & `qiling-1.4.6/qiling/extensions/afl/afl.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,40 +24,41 @@
             :param bool always_validate: If this is set to False, validate_crash_callback will be only triggered if
             uc_emu_start (which is called internally by afl_fuzz) returns an error. Or the validate_crash_callback will
             be triggered every time.
             :param int persistent_iters: Fuzz how many times before forking a new child.
             :raises UcAflError: If something wrong happens with the fuzzer.
         """
 
-        ql.uc.ctl_exits_enabled(True)
-        ql.uc.ctl_set_exits(exits)
-
         def _dummy_fuzz_callback(_ql: "Qiling"):
             if isinstance(_ql.arch, QlArchARM):
                 pc = _ql.arch.effective_pc
             else:
                 pc = _ql.arch.regs.arch_pc
             try:
                 _ql.uc.emu_start(pc, 0, 0, 0)
             except UcError as e:
                 return e.errno
             
             return UC_ERR_OK
         
-        return ql_afl_fuzz_custom(ql, input_file, place_input_callback, _dummy_fuzz_callback, 
+        return ql_afl_fuzz_custom(ql, input_file, place_input_callback, _dummy_fuzz_callback, exits,
                                   validate_crash_callback, always_validate, persistent_iters)
 
 def ql_afl_fuzz_custom(ql: Qiling,
                        input_file: str,
                        place_input_callback: Callable[["Qiling", bytes, int], bool],
                        fuzzing_callback: Callable[["Qiling"], int],
+                       exits: List[int] = [],
                        validate_crash_callback: Callable[["Qiling", bytes, int], bool] = None,
                        always_validate: bool = False,
                        persistent_iters: int = 1):
 
+        ql.uc.ctl_exits_enabled(True)
+        ql.uc.ctl_set_exits(exits)
+
         def _ql_afl_place_input_wrapper(uc, input_bytes, iters, data):
             (ql, cb, _, _) = data
 
             if cb:
                 return cb(ql, input_bytes, iters)
             else:
                 return False
```

### Comparing `qiling-1.4.5/qiling/extensions/coverage/formats/base.py` & `qiling-1.4.6/qiling/extensions/coverage/formats/base.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/extensions/coverage/formats/drcov.py` & `qiling-1.4.6/qiling/extensions/coverage/formats/drcov.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/extensions/coverage/formats/drcov_exact.py` & `qiling-1.4.6/qiling/extensions/coverage/formats/drcov_exact.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/extensions/coverage/utils.py` & `qiling-1.4.6/qiling/extensions/coverage/utils.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/extensions/idaplugin/qilingida.py` & `qiling-1.4.6/qiling/extensions/idaplugin/qilingida.py`

 * *Files 0% similar despite different names*

```diff
@@ -497,14 +497,15 @@
         self.AddLine(view_title)
         self.AddLine("")
 
         reglist = QlEmuMisc.get_reg_map(ql)
         line = ""
         cols = 3
         reglist = [reglist[i:i+cols] for i in range(0,len(reglist),cols)]
+        arch = ql.arch.type
         for regs in reglist:
             for reg in regs:
                 line += COLSTR(" %4s: " % str(reg), SCOLOR_REG)
                 regvalue = ql.arch.regs.read(reg)
                 if arch in [QL_ARCH.X8664, QL_ARCH.ARM64]:
                     value_format = "0x%.16X"
                 else:
@@ -894,15 +895,15 @@
 
         self.exit_addr = self.ql.os.exit_point
         if self.ql.os.type == QL_OS.LINUX:
             f = open(self.ql.path, 'rb')
             elffile = ELFFile(f)
             elf_header = elffile.header
             if elf_header['e_type'] == 'ET_EXEC':
-                self.baseaddr = self.ql.os.elf_mem_start
+                self.baseaddr = self.ql.loader.images[0].base
             elif elf_header['e_type'] == 'ET_DYN':
                 if self.ql.arch.bits == 32:
                     self.baseaddr = int(self.ql.os.profile.get("OS32", "load_address"), 16)
                 elif self.ql.arch.bits == 64:
                     self.baseaddr = int(self.ql.os.profile.get("OS64", "load_address"), 16)
         else:
             self.baseaddr = 0x0
@@ -2022,14 +2023,15 @@
                 logging.info(filename)
                 scriptname,_ = os.path.splitext(filename)
                 logging.info(scriptname)
                 sys.path.append(modulepath)
                 module = importlib.import_module(scriptname)
 
                 if is_reload:
+                    del self.userobj
                     importlib.reload(module)
                 cls = getattr(module, classname)
                 return cls()
             except Exception as e:
                 logging.exception("")
                 return None
```

### Comparing `qiling-1.4.5/qiling/extensions/mcu/atmel/sam3x8e.py` & `qiling-1.4.6/qiling/extensions/mcu/atmel/sam3x8e.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/extensions/mcu/bes/bes2300.py` & `qiling-1.4.6/qiling/extensions/mcu/bes/bes2300.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/extensions/mcu/gd32vf1/gd32vf103.py` & `qiling-1.4.6/qiling/extensions/mcu/gd32vf1/gd32vf103.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/extensions/mcu/nxp/mk64f12.py` & `qiling-1.4.6/qiling/extensions/mcu/nxp/mk64f12.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/extensions/mcu/stm32f1/stm32f103.py` & `qiling-1.4.6/qiling/extensions/mcu/stm32f1/stm32f103.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/extensions/mcu/stm32f4/__init__.py` & `qiling-1.4.6/qiling/extensions/mcu/stm32f4/__init__.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/extensions/mcu/stm32f4/stm32f401.py` & `qiling-1.4.6/qiling/extensions/mcu/stm32f4/stm32f401.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/extensions/mcu/stm32f4/stm32f405.py` & `qiling-1.4.6/qiling/extensions/mcu/stm32f4/stm32f405.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/extensions/mcu/stm32f4/stm32f407.py` & `qiling-1.4.6/qiling/extensions/mcu/stm32f4/stm32f407.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/extensions/mcu/stm32f4/stm32f410.py` & `qiling-1.4.6/qiling/extensions/mcu/stm32f4/stm32f410.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/extensions/mcu/stm32f4/stm32f411.py` & `qiling-1.4.6/qiling/extensions/mcu/stm32f4/stm32f411.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/extensions/mcu/stm32f4/stm32f412.py` & `qiling-1.4.6/qiling/extensions/mcu/stm32f4/stm32f412.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/extensions/mcu/stm32f4/stm32f413.py` & `qiling-1.4.6/qiling/extensions/mcu/stm32f4/stm32f413.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/extensions/mcu/stm32f4/stm32f415.py` & `qiling-1.4.6/qiling/extensions/mcu/stm32f4/stm32f415.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/extensions/mcu/stm32f4/stm32f417.py` & `qiling-1.4.6/qiling/extensions/mcu/stm32f4/stm32f417.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/extensions/mcu/stm32f4/stm32f423.py` & `qiling-1.4.6/qiling/extensions/mcu/stm32f4/stm32f423.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/extensions/mcu/stm32f4/stm32f427.py` & `qiling-1.4.6/qiling/extensions/mcu/stm32f4/stm32f427.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/extensions/mcu/stm32f4/stm32f429.py` & `qiling-1.4.6/qiling/extensions/mcu/stm32f4/stm32f429.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/extensions/mcu/stm32f4/stm32f437.py` & `qiling-1.4.6/qiling/extensions/mcu/stm32f4/stm32f437.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/extensions/mcu/stm32f4/stm32f439.py` & `qiling-1.4.6/qiling/extensions/mcu/stm32f4/stm32f439.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/extensions/mcu/stm32f4/stm32f446.py` & `qiling-1.4.6/qiling/extensions/mcu/stm32f4/stm32f446.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/extensions/mcu/stm32f4/stm32f469.py` & `qiling-1.4.6/qiling/extensions/mcu/stm32f4/stm32f469.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/extensions/mcu/stm32f4/stm32f479.py` & `qiling-1.4.6/qiling/extensions/mcu/stm32f4/stm32f479.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/extensions/multitask.py` & `qiling-1.4.6/qiling/extensions/multitask.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/extensions/r2/r2.py` & `qiling-1.4.6/qiling/extensions/r2/r2.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/extensions/report/report.py` & `qiling-1.4.6/qiling/extensions/report/report.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/extensions/sanitizers/heap.py` & `qiling-1.4.6/qiling/extensions/sanitizers/heap.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/extensions/trace.py` & `qiling-1.4.6/qiling/extensions/trace.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,220 +11,220 @@
 
 from qiling import Qiling
 
 TraceRecord = Tuple[CsInsn, Iterable[Tuple[int, int]]]
 
 # <WORKAROUND>
 def __uc2_workaround() -> Mapping[int, int]:
-	"""Starting from Unicorn2, Unicorn and Capstone Intel registers definitions are
-	no longer aligned and cannot be used interchangebly. This temporary workaround
-	maps capstone x86 registers definitions to unicorn x86 registers definitions.
+    """Starting from Unicorn2, Unicorn and Capstone Intel registers definitions are
+    no longer aligned and cannot be used interchangebly. This temporary workaround
+    maps capstone x86 registers definitions to unicorn x86 registers definitions.
 
-	see: https://github.com/unicorn-engine/unicorn/issues/1492
-	"""
+    see: https://github.com/unicorn-engine/unicorn/issues/1492
+    """
 
-	from capstone import x86_const as cs_x86_const
-	from unicorn import x86_const as uc_x86_const
+    from capstone import x86_const as cs_x86_const
+    from unicorn import x86_const as uc_x86_const
 
-	def __canonicalized_mapping(module, prefix: str) -> Mapping[str, int]:
-		return dict((k[len(prefix):], getattr(module, k)) for k in dir(module) if k.startswith(prefix))
+    def __canonicalized_mapping(module, prefix: str) -> Mapping[str, int]:
+        return dict((k[len(prefix):], getattr(module, k)) for k in dir(module) if k.startswith(prefix))
 
-	cs_x86_regs = __canonicalized_mapping(cs_x86_const, 'X86_REG')
-	uc_x86_regs = __canonicalized_mapping(uc_x86_const, 'UC_X86_REG')
+    cs_x86_regs = __canonicalized_mapping(cs_x86_const, 'X86_REG')
+    uc_x86_regs = __canonicalized_mapping(uc_x86_const, 'UC_X86_REG')
 
-	return dict((cs_x86_regs[k], uc_x86_regs[k]) for k in cs_x86_regs if k in uc_x86_regs)
+    return dict((cs_x86_regs[k], uc_x86_regs[k]) for k in cs_x86_regs if k in uc_x86_regs)
 
 CS_UC_REGS = __uc2_workaround()
 # </WORKAROUND>
 
 def __get_trace_records(ql: Qiling, address: int, size: int, md: Cs) -> Iterator[TraceRecord]:
-	"""[private] Acquire trace info for the current instruction and yield as a trace record.
-	A trace record is a parsed instruction paired to a list of registers and their values.
+    """[private] Acquire trace info for the current instruction and yield as a trace record.
+    A trace record is a parsed instruction paired to a list of registers and their values.
 
-	This method might yield more than one record for a single instruction.
-	"""
+    This method might yield more than one record for a single instruction.
+    """
 
-	# unicorn denotes unsupported instructions by a magic size value. though these instructions
-	# are not emulated, capstone can still parse them.
-	if size == 0xf1f1f1f1:
-		# note that invalid instructions will generate a StopIteration exception here
-		yield next(__get_trace_records(ql, address, 16, md))
-		return
-
-	# a trace line is generated even for hook addresses that do not contain meaningful opcodes.
-	# in that case, make it look like a nop
-	if address in ql._addr_hook:
-		buf = b'\x90'
-	else:
-		buf = ql.mem.read(address, size)
-
-	for insn in md.disasm(buf, address):
-		# BUG: insn.regs_read doesn't work well, so we use insn.regs_access()[0]
-		state = tuple((reg, ql.arch.regs.read(CS_UC_REGS[reg])) for reg in insn.regs_access()[0])
+    # unicorn denotes unsupported instructions by a magic size value. though these instructions
+    # are not emulated, capstone can still parse them.
+    if size == 0xf1f1f1f1:
+        # note that invalid instructions will generate a StopIteration exception here
+        yield next(__get_trace_records(ql, address, 16, md))
+        return
+
+    # a trace line is generated even for hook addresses that do not contain meaningful opcodes.
+    # in that case, make it look like a nop
+    if address in ql._addr_hook:
+        buf = b'\x90'
+    else:
+        buf = ql.mem.read(address, size)
+
+    for insn in md.disasm(buf, address):
+        # BUG: insn.regs_read doesn't work well, so we use insn.regs_access()[0]
+        state = tuple((reg, ql.arch.regs.read(CS_UC_REGS[reg])) for reg in insn.regs_access()[0])
 
-		yield (insn, state)
+        yield (insn, state)
 
 def __to_trace_line(record: TraceRecord, symsmap: Mapping[int, str] = {}) -> str:
-	"""[private] Transform trace info into a formatted trace line.
-	"""
+    """[private] Transform trace info into a formatted trace line.
+    """
 
-	insn, state = record
+    insn, state = record
 
-	# when the rip register is referenced from within an instruction it is expected to point
-	# to the next instruction boundary. since unicorn has not executed the instruction yet
-	# is uses the cpu state resulted from the previous instruction - and rip points to the
-	# current instruction instead of the next one.
-	#
-	# here we patch rip value recorded in state to point to the next instruction boundary
-	state = tuple((reg, val + insn.size if reg == X86_REG_RIP else val) for reg, val in state)
-
-	def __read_reg(reg: int) -> int:
-		"""[internal] Read a register value from the recorded state. Only registers that were
-		referenced by the current instruction can be read.
-		"""
-
-		return 0 if reg == X86_REG_INVALID else next(v for r, v in state if r == reg)
-
-	def __resolve(address: int) -> str:
-		"""[internal] Find the symbol that matches to the specified address (if any).
-		"""
-
-		return symsmap.get(address, '')
-
-	def __parse_op(op: X86Op) -> str:
-		"""[internal] Parse an operand and return its string representation. Indirect memory
-		references will be substitued by the effective address they refer to. If the referenced
-		address is associated with a symbol, it will be substitued by that symbol.
-		"""
-
-		if op.type == CS_OP_REG:
-			return insn.reg_name(op.value.reg) or '?'
-
-		elif op.type == CS_OP_IMM:
-			imm = op.value.imm
-
-			return __resolve(imm) or f'{imm:#x}'
-
-		elif op.type == CS_OP_MEM:
-			mem = op.value.mem
-
-			base  = __read_reg(mem.base)
-			index = __read_reg(mem.index)
-			scale = mem.scale
-			disp  = mem.disp
-
-			ea = base + index * scale + disp
-			seg = f'{insn.reg_name(mem.segment)}:' if mem.segment else ''
-
-			# we construct the string representation for each operand; denote memory
-			# dereferenes with the appropriate 'ptr' prefix. the 'lea' instruction is
-			# an exception since it does not use that notation.
-			if insn.id == X86_INS_LEA:
-				qualifier = f''
-			else:
-				ptr = {
-					1: 'byte',
-					2: 'word',
-					4: 'dword',
-					8: 'qword',
-					10: 'fword',
-					16: 'xmmword'
-				}[op.size]
-
-				qualifier = f'{ptr} ptr '
-
-			return f'{qualifier}{seg}[{__resolve(ea) or f"{ea:#x}"}]'
+    # when the rip register is referenced from within an instruction it is expected to point
+    # to the next instruction boundary. since unicorn has not executed the instruction yet
+    # is uses the cpu state resulted from the previous instruction - and rip points to the
+    # current instruction instead of the next one.
+    #
+    # here we patch rip value recorded in state to point to the next instruction boundary
+    state = tuple((reg, val + insn.size if reg == X86_REG_RIP else val) for reg, val in state)
+
+    def __read_reg(reg: int) -> int:
+        """[internal] Read a register value from the recorded state. Only registers that were
+        referenced by the current instruction can be read.
+        """
+
+        return 0 if reg == X86_REG_INVALID else next(v for r, v in state if r == reg)
+
+    def __resolve(address: int) -> str:
+        """[internal] Find the symbol that matches to the specified address (if any).
+        """
+
+        return symsmap.get(address, '')
+
+    def __parse_op(op: X86Op) -> str:
+        """[internal] Parse an operand and return its string representation. Indirect memory
+        references will be substitued by the effective address they refer to. If the referenced
+        address is associated with a symbol, it will be substitued by that symbol.
+        """
+
+        if op.type == CS_OP_REG:
+            return insn.reg_name(op.value.reg) or '?'
+
+        elif op.type == CS_OP_IMM:
+            imm = op.value.imm
+
+            return __resolve(imm) or f'{imm:#x}'
+
+        elif op.type == CS_OP_MEM:
+            mem = op.value.mem
+
+            base  = __read_reg(mem.base)
+            index = __read_reg(mem.index)
+            scale = mem.scale
+            disp  = mem.disp
+
+            ea = base + index * scale + disp
+            seg = f'{insn.reg_name(mem.segment)}:' if mem.segment else ''
+
+            # we construct the string representation for each operand; denote memory
+            # dereferenes with the appropriate 'ptr' prefix. the 'lea' instruction is
+            # an exception since it does not use that notation.
+            if insn.id == X86_INS_LEA:
+                qualifier = f''
+            else:
+                ptr = {
+                    1: 'byte',
+                    2: 'word',
+                    4: 'dword',
+                    8: 'qword',
+                    10: 'fword',
+                    16: 'xmmword'
+                }[op.size]
+
+                qualifier = f'{ptr} ptr '
+
+            return f'{qualifier}{seg}[{__resolve(ea) or f"{ea:#x}"}]'
 
-		# unexpected op type
-		raise RuntimeError
+        # unexpected op type
+        raise RuntimeError
 
-	operands = ', '.join(__parse_op(o) for o in insn.operands)
-	reads = ', '.join(f'{insn.reg_name(reg)} = {val:#x}' for reg, val in state)
+    operands = ', '.join(__parse_op(o) for o in insn.operands)
+    reads = ', '.join(f'{insn.reg_name(reg)} = {val:#x}' for reg, val in state)
 
-	return f'{insn.address:08x} | {insn.bytes.hex():24s} {insn.mnemonic:10} {operands:56s} | {reads}'
+    return f'{insn.address:08x} | {insn.bytes.hex():24s} {insn.mnemonic:10} {operands:56s} | {reads}'
 
 def enable_full_trace(ql: Qiling):
-	"""Enable instruction-level tracing.
+    """Enable instruction-level tracing.
 
-	Trace line will be emitted for each instruction before it gets executed. The info
-	includes static data along with the relevant registers state and symbols resolving.
+    Trace line will be emitted for each instruction before it gets executed. The info
+    includes static data along with the relevant registers state and symbols resolving.
 
-	Args:
-		ql: qiling instance
-	"""
+    Args:
+        ql: qiling instance
+    """
 
-	# enable detailed disassembly info
-	md = ql.arch.disassembler
-	md.detail = True
+    # enable detailed disassembly info
+    md = ql.arch.disassembler
+    md.detail = True
 
-	assert md.arch == CS_ARCH_X86, 'currently available only for intel architecture'
+    assert md.arch == CS_ARCH_X86, 'currently available only for intel architecture'
 
-	# if available, use symbols map to resolve memory accesses
-	symsmap = getattr(ql.loader, 'symsmap', {})
+    # if available, use symbols map to resolve memory accesses
+    symsmap = getattr(ql.loader, 'symsmap', {})
 
-	# show trace lines in a darker color so they would be easily distinguished from
-	# ordinary log records
-	faded_color = "\033[2m"
-	reset_color = "\033[0m"
+    # show trace lines in a darker color so they would be easily distinguished from
+    # ordinary log records
+    faded_color = "\033[2m"
+    reset_color = "\033[0m"
 
-	def __trace_hook(ql: Qiling, address: int, size: int):
-		"""[internal] Trace hook callback.
-		"""
+    def __trace_hook(ql: Qiling, address: int, size: int):
+        """[internal] Trace hook callback.
+        """
 
-		for record in __get_trace_records(ql, address, size, md):
-			line = __to_trace_line(record, symsmap)
+        for record in __get_trace_records(ql, address, size, md):
+            line = __to_trace_line(record, symsmap)
 
-			ql.log.debug(f'{faded_color}{line}{reset_color}')
+            ql.log.debug(f'{faded_color}{line}{reset_color}')
 
-	ql.hook_code(__trace_hook)
+    ql.hook_code(__trace_hook)
 
 def enable_history_trace(ql: Qiling, nrecords: int):
-	"""Enable instruction-level tracing in history mode.
+    """Enable instruction-level tracing in history mode.
 
-	To allow faster execution, the trace info collected throughout program execution is not
-	emitted and undergo as minimal post-processing as possible. When program crahses, the
-	last `nrecords` trace lines are shown.
+    To allow faster execution, the trace info collected throughout program execution is not
+    emitted and undergo as minimal post-processing as possible. When program crahses, the
+    last `nrecords` trace lines are shown.
 
-	Args:
-		ql: qiling instance
-		nrecords: number of last records to show
-	"""
+    Args:
+        ql: qiling instance
+        nrecords: number of last records to show
+    """
 
-	# enable detailed disassembly info
-	md = ql.arch.disassembler
-	md.detail = True
+    # enable detailed disassembly info
+    md = ql.arch.disassembler
+    md.detail = True
 
-	assert md.arch == CS_ARCH_X86, 'currently available only for intel architecture'
+    assert md.arch == CS_ARCH_X86, 'currently available only for intel architecture'
 
-	# if available, use symbols map to resolve memory accesses
-	symsmap = getattr(ql.loader, 'symsmap', {})
+    # if available, use symbols map to resolve memory accesses
+    symsmap = getattr(ql.loader, 'symsmap', {})
 
-	history: Deque[TraceRecord] = deque(maxlen=nrecords)
+    history: Deque[TraceRecord] = deque(maxlen=nrecords)
 
-	def __trace_hook(ql: Qiling, address: int, size: int):
-		"""[internal] Trace hook callback.
-		"""
+    def __trace_hook(ql: Qiling, address: int, size: int):
+        """[internal] Trace hook callback.
+        """
 
-		history.extend(__get_trace_records(ql, address, size, md))
+        history.extend(__get_trace_records(ql, address, size, md))
 
-	ql.hook_code(__trace_hook)
+    ql.hook_code(__trace_hook)
 
-	# replace the emulation error handler with our own so we can emit the trace
-	# records when program crashes. before we do that, we save the original one
-	# so we can call it.
+    # replace the emulation error handler with our own so we can emit the trace
+    # records when program crashes. before we do that, we save the original one
+    # so we can call it.
 
-	orig_emu_error = ql.os.emu_error
+    orig_emu_error = ql.os.emu_error
 
-	def __emu_error(*args):
-		# first run the original emulation error handler
-		orig_emu_error(*args)
+    def __emu_error(*args):
+        # first run the original emulation error handler
+        orig_emu_error(*args)
 
-		# then parse and emit the trace info we collected
-		ql.log.error(f'History:')
-		for record in history:
-			line = __to_trace_line(record, symsmap)
+        # then parse and emit the trace info we collected
+        ql.log.error(f'History:')
+        for record in history:
+            line = __to_trace_line(record, symsmap)
 
-			ql.log.error(line)
+            ql.log.error(line)
 
-		ql.log.error(f'')
+        ql.log.error(f'')
 
-	ql.os.emu_error = __emu_error
+    ql.os.emu_error = __emu_error
```

### Comparing `qiling-1.4.5/qiling/extensions/tracing/formats/base.py` & `qiling-1.4.6/qiling/extensions/tracing/formats/base.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/extensions/tracing/formats/registers.py` & `qiling-1.4.6/qiling/extensions/tracing/formats/registers.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/extensions/tracing/formats/tenet.py` & `qiling-1.4.6/qiling/extensions/tracing/formats/tenet.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/extensions/tracing/utils.py` & `qiling-1.4.6/qiling/extensions/tracing/utils.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/host.py` & `qiling-1.4.6/qiling/host.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/hw/analog/mk64f12_adc.py` & `qiling-1.4.6/qiling/hw/analog/mk64f12_adc.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/hw/analog/sam3xa_adc.py` & `qiling-1.4.6/qiling/hw/analog/sam3xa_adc.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/hw/analog/sam3xa_dac.py` & `qiling-1.4.6/qiling/hw/analog/sam3xa_dac.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/hw/analog/sam3xa_pwm.py` & `qiling-1.4.6/qiling/hw/analog/sam3xa_pwm.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/hw/analog/stm32f1xx_adc.py` & `qiling-1.4.6/qiling/hw/analog/stm32f1xx_adc.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/hw/analog/stm32f4xx_dac.py` & `qiling-1.4.6/qiling/hw/analog/stm32f4xx_dac.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/hw/char/gd32vf1xx_usart.py` & `qiling-1.4.6/qiling/hw/char/gd32vf1xx_usart.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/hw/char/mk64f12_uart.py` & `qiling-1.4.6/qiling/hw/char/mk64f12_uart.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/hw/char/sam3xa_uart.py` & `qiling-1.4.6/qiling/hw/char/sam3xa_uart.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/hw/char/sam3xa_uotghs.py` & `qiling-1.4.6/qiling/hw/char/sam3xa_uotghs.py`

 * *Files 0% similar despite different names*

```diff
@@ -102,15 +102,15 @@
     def __init__(self, ql, label, intn = None):
         super().__init__(ql, label)
 
         self.instance = self.struct()
         self.intn = intn
 
     @QlPeripheral.monitor()
-    def read(self, offset: int, size: int) -> int:		
+    def read(self, offset: int, size: int) -> int:        
         buf = ctypes.create_string_buffer(size)
         ctypes.memmove(buf, ctypes.addressof(self.instance) + offset, size)
         return int.from_bytes(buf.raw, byteorder='little')
 
     @QlPeripheral.monitor()
     def write(self, offset: int, size: int, value: int):
         if offset == self.struct.CTRL.offset:
```

### Comparing `qiling-1.4.5/qiling/hw/char/stm32f1xx_usart.py` & `qiling-1.4.6/qiling/hw/char/stm32f1xx_usart.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/hw/char/stm32f4xx_usart.py` & `qiling-1.4.6/qiling/hw/char/stm32f4xx_usart.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,48 +8,48 @@
 from qiling.hw.peripheral import QlPeripheral
 from qiling.hw.connectivity import QlConnectivityPeripheral
 from qiling.hw.const.stm32f4xx_usart import USART_SR, USART_CR1
 
 class STM32F4xxUsart(QlConnectivityPeripheral):
     class Type(ctypes.Structure):
         """ the structure available in :
-			stm32f413xx.h
-			stm32f407xx.h
-			stm32f469xx.h
-			stm32f446xx.h
-			stm32f427xx.h
-			stm32f401xc.h
-			stm32f415xx.h
-			stm32f412cx.h
-			stm32f410rx.h
-			stm32f410tx.h
-			stm32f439xx.h
-			stm32f412vx.h
-			stm32f417xx.h
-			stm32f479xx.h
-			stm32f429xx.h
-			stm32f412rx.h
-			stm32f423xx.h
-			stm32f437xx.h
-			stm32f412zx.h
-			stm32f401xe.h
-			stm32f410cx.h
-			stm32f405xx.h
-			stm32f411xe.h
-		"""
+            stm32f413xx.h
+            stm32f407xx.h
+            stm32f469xx.h
+            stm32f446xx.h
+            stm32f427xx.h
+            stm32f401xc.h
+            stm32f415xx.h
+            stm32f412cx.h
+            stm32f410rx.h
+            stm32f410tx.h
+            stm32f439xx.h
+            stm32f412vx.h
+            stm32f417xx.h
+            stm32f479xx.h
+            stm32f429xx.h
+            stm32f412rx.h
+            stm32f423xx.h
+            stm32f437xx.h
+            stm32f412zx.h
+            stm32f401xe.h
+            stm32f410cx.h
+            stm32f405xx.h
+            stm32f411xe.h
+        """
 
         _fields_ = [
-			('SR'  , ctypes.c_uint32),  # USART Status register,                   Address offset: 0x00
-			('DR'  , ctypes.c_uint32),  # USART Data register,                     Address offset: 0x04
-			('BRR' , ctypes.c_uint32),  # USART Baud rate register,                Address offset: 0x08
-			('CR1' , ctypes.c_uint32),  # USART Control register 1,                Address offset: 0x0C
-			('CR2' , ctypes.c_uint32),  # USART Control register 2,                Address offset: 0x10
-			('CR3' , ctypes.c_uint32),  # USART Control register 3,                Address offset: 0x14
-			('GTPR', ctypes.c_uint32),  # USART Guard time and prescaler register, Address offset: 0x18
-		]
+            ('SR'  , ctypes.c_uint32),  # USART Status register,                   Address offset: 0x00
+            ('DR'  , ctypes.c_uint32),  # USART Data register,                     Address offset: 0x04
+            ('BRR' , ctypes.c_uint32),  # USART Baud rate register,                Address offset: 0x08
+            ('CR1' , ctypes.c_uint32),  # USART Control register 1,                Address offset: 0x0C
+            ('CR2' , ctypes.c_uint32),  # USART Control register 2,                Address offset: 0x10
+            ('CR3' , ctypes.c_uint32),  # USART Control register 3,                Address offset: 0x14
+            ('GTPR', ctypes.c_uint32),  # USART Guard time and prescaler register, Address offset: 0x18
+        ]
 
     
     def __init__(self, ql, label, intn=None):
         super().__init__(ql, label)
         
         self.instance = self.struct(
             SR = USART_SR.RESET,
```

### Comparing `qiling-1.4.5/qiling/hw/connectivity.py` & `qiling-1.4.6/qiling/hw/connectivity.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/hw/const/gd32vf1xx_dma.py` & `qiling-1.4.6/qiling/hw/const/gd32vf1xx_dma.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/hw/const/gd32vf1xx_i2c.py` & `qiling-1.4.6/qiling/hw/const/gd32vf1xx_i2c.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/hw/const/gd32vf1xx_rcu.py` & `qiling-1.4.6/qiling/hw/const/gd32vf1xx_rcu.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/hw/const/gd32vf1xx_rtc.py` & `qiling-1.4.6/qiling/hw/const/gd32vf1xx_rtc.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/hw/const/gd32vf1xx_spi.py` & `qiling-1.4.6/qiling/hw/const/gd32vf1xx_spi.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/hw/const/gd32vf1xx_timer.py` & `qiling-1.4.6/qiling/hw/const/gd32vf1xx_timer.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/hw/const/gd32vf1xx_usart.py` & `qiling-1.4.6/qiling/hw/const/gd32vf1xx_usart.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/hw/const/mk64f12_adc.py` & `qiling-1.4.6/qiling/hw/const/mk64f12_adc.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/hw/const/mk64f12_ftm.py` & `qiling-1.4.6/qiling/hw/const/mk64f12_ftm.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/hw/const/mk64f12_mcg.py` & `qiling-1.4.6/qiling/hw/const/mk64f12_mcg.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/hw/const/mk64f12_port.py` & `qiling-1.4.6/qiling/hw/const/mk64f12_port.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/hw/const/mk64f12_spi.py` & `qiling-1.4.6/qiling/hw/const/mk64f12_spi.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/hw/const/mk64f12_uart.py` & `qiling-1.4.6/qiling/hw/const/mk64f12_uart.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/hw/const/sam3xa_adc.py` & `qiling-1.4.6/qiling/hw/const/sam3xa_adc.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/hw/const/sam3xa_dac.py` & `qiling-1.4.6/qiling/hw/const/sam3xa_dac.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/hw/const/sam3xa_pmc.py` & `qiling-1.4.6/qiling/hw/const/sam3xa_pmc.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/hw/const/sam3xa_spi.py` & `qiling-1.4.6/qiling/hw/const/sam3xa_spi.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/hw/const/sam3xa_uart.py` & `qiling-1.4.6/qiling/hw/const/sam3xa_uart.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/hw/const/sam3xa_uotghs.py` & `qiling-1.4.6/qiling/hw/const/sam3xa_uotghs.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/hw/const/stm32f4xx_eth.py` & `qiling-1.4.6/qiling/hw/const/stm32f4xx_eth.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,272 +1,272 @@
 from enum import IntEnum
 
 
 class ETH_MACCR(IntEnum):
-	WD   = 1 << 23
-	JD   = 1 << 22
-	IFG  = 0x7 << 17
-	CSD  = 1 << 16
-	FES  = 1 << 14
-	ROD  = 1 << 13
-	LM   = 1 << 12
-	DM   = 1 << 11
-	IPCO = 1 << 10
-	RD   = 1 << 9
-	APCS = 1 << 7
-	BL   = 0x3 << 5
-	DC   = 1 << 4
-	TE   = 1 << 3
-	RE   = 1 << 2
+    WD   = 1 << 23
+    JD   = 1 << 22
+    IFG  = 0x7 << 17
+    CSD  = 1 << 16
+    FES  = 1 << 14
+    ROD  = 1 << 13
+    LM   = 1 << 12
+    DM   = 1 << 11
+    IPCO = 1 << 10
+    RD   = 1 << 9
+    APCS = 1 << 7
+    BL   = 0x3 << 5
+    DC   = 1 << 4
+    TE   = 1 << 3
+    RE   = 1 << 2
 
 class ETH_MACFFR(IntEnum):
-	RA                          = 1 << 31
-	HPF                         = 1 << 10
-	SAF                         = 1 << 9
-	SAIF                        = 1 << 8
-	PCF                         = 0x3 << 6
-	PCF_BlockAll                = 1 << 6
-	PCF_ForwardAll              = 1 << 7
-	PCF_ForwardPassedAddrFilter = 0x3 << 6
-	BFD                         = 1 << 5
-	PAM                         = 1 << 4
-	DAIF                        = 1 << 3
-	HM                          = 1 << 2
-	HU                          = 1 << 1
-	PM                          = 1 << 0
+    RA                          = 1 << 31
+    HPF                         = 1 << 10
+    SAF                         = 1 << 9
+    SAIF                        = 1 << 8
+    PCF                         = 0x3 << 6
+    PCF_BlockAll                = 1 << 6
+    PCF_ForwardAll              = 1 << 7
+    PCF_ForwardPassedAddrFilter = 0x3 << 6
+    BFD                         = 1 << 5
+    PAM                         = 1 << 4
+    DAIF                        = 1 << 3
+    HM                          = 1 << 2
+    HU                          = 1 << 1
+    PM                          = 1 << 0
 
 class ETH_MACMIIAR(IntEnum):
-	PA        = 0x1f << 11
-	MR        = 0x1f << 6
-	CR        = 0x7 << 2
-	CR_Div62  = 1 << 2
-	CR_Div16  = 1 << 3
-	CR_Div26  = 0x3 << 2
-	CR_Div102 = 1 << 4
-	MW        = 1 << 1
-	MB        = 1 << 0
+    PA        = 0x1f << 11
+    MR        = 0x1f << 6
+    CR        = 0x7 << 2
+    CR_Div62  = 1 << 2
+    CR_Div16  = 1 << 3
+    CR_Div26  = 0x3 << 2
+    CR_Div102 = 1 << 4
+    MW        = 1 << 1
+    MB        = 1 << 0
 
 class ETH_MACFCR(IntEnum):
-	PT           = 0xffff << 16
-	ZQPD         = 1 << 7
-	PLT          = 0x3 << 4
-	PLT_Minus28  = 1 << 4
-	PLT_Minus144 = 1 << 5
-	PLT_Minus256 = 0x3 << 4
-	UPFD         = 1 << 3
-	RFCE         = 1 << 2
-	TFCE         = 1 << 1
-	FCBBPA       = 1 << 0
+    PT           = 0xffff << 16
+    ZQPD         = 1 << 7
+    PLT          = 0x3 << 4
+    PLT_Minus28  = 1 << 4
+    PLT_Minus144 = 1 << 5
+    PLT_Minus256 = 0x3 << 4
+    UPFD         = 1 << 3
+    RFCE         = 1 << 2
+    TFCE         = 1 << 1
+    FCBBPA       = 1 << 0
 
 class ETH_MACVLANTR(IntEnum):
-	VLANTC = 1 << 16
-	VLANTI = 0xffff << 0
+    VLANTC = 1 << 16
+    VLANTI = 0xffff << 0
 
 class ETH_MACPMTCSR(IntEnum):
-	WFFRPR = 1 << 31
-	GU     = 1 << 9
-	WFR    = 1 << 6
-	MPR    = 1 << 5
-	WFE    = 1 << 2
-	MPE    = 1 << 1
-	PD     = 1 << 0
+    WFFRPR = 1 << 31
+    GU     = 1 << 9
+    WFR    = 1 << 6
+    MPR    = 1 << 5
+    WFE    = 1 << 2
+    MPE    = 1 << 1
+    PD     = 1 << 0
 
 class ETH_MACDBGR(IntEnum):
-	TFF                 = 1 << 25
-	TFNE                = 1 << 24
-	TFWA                = 1 << 22
-	TFRS                = 0x3 << 20
-	TFRS_WRITING        = 0x3 << 20
-	TFRS_WAITING        = 1 << 21
-	TFRS_READ           = 1 << 20
-	MTP                 = 1 << 19
-	MTFCS               = 0x3 << 17
-	MTFCS_TRANSFERRING  = 0x3 << 17
-	MTFCS_GENERATINGPCF = 1 << 18
-	MTFCS_WAITING       = 1 << 17
-	MMTEA               = 1 << 16
-	RFFL                = 0x3 << 8
-	RFFL_FL             = 0x3 << 8
-	RFFL_ABOVEFCT       = 1 << 9
-	RFFL_BELOWFCT       = 1 << 8
-	RFRCS               = 0x3 << 5
-	RFRCS_FLUSHING      = 0x3 << 5
-	RFRCS_STATUSREADING = 1 << 6
-	RFRCS_DATAREADING   = 1 << 5
-	RFWRA               = 1 << 4
-	MSFRWCS             = 0x3 << 1
-	MMRPEA              = 1 << 0
+    TFF                 = 1 << 25
+    TFNE                = 1 << 24
+    TFWA                = 1 << 22
+    TFRS                = 0x3 << 20
+    TFRS_WRITING        = 0x3 << 20
+    TFRS_WAITING        = 1 << 21
+    TFRS_READ           = 1 << 20
+    MTP                 = 1 << 19
+    MTFCS               = 0x3 << 17
+    MTFCS_TRANSFERRING  = 0x3 << 17
+    MTFCS_GENERATINGPCF = 1 << 18
+    MTFCS_WAITING       = 1 << 17
+    MMTEA               = 1 << 16
+    RFFL                = 0x3 << 8
+    RFFL_FL             = 0x3 << 8
+    RFFL_ABOVEFCT       = 1 << 9
+    RFFL_BELOWFCT       = 1 << 8
+    RFRCS               = 0x3 << 5
+    RFRCS_FLUSHING      = 0x3 << 5
+    RFRCS_STATUSREADING = 1 << 6
+    RFRCS_DATAREADING   = 1 << 5
+    RFWRA               = 1 << 4
+    MSFRWCS             = 0x3 << 1
+    MMRPEA              = 1 << 0
 
 class ETH_MACSR(IntEnum):
-	TSTS   = 1 << 9
-	MMCTS  = 1 << 6
-	MMMCRS = 1 << 5
-	MMCS   = 1 << 4
-	PMTS   = 1 << 3
+    TSTS   = 1 << 9
+    MMCTS  = 1 << 6
+    MMMCRS = 1 << 5
+    MMCS   = 1 << 4
+    PMTS   = 1 << 3
 
 class ETH_MACIMR(IntEnum):
-	TSTIM = 1 << 9
-	PMTIM = 1 << 3
+    TSTIM = 1 << 9
+    PMTIM = 1 << 3
 
 class ETH_MACA1HR(IntEnum):
-	AE     = 1 << 31
-	SA     = 1 << 30
-	MBC    = 0x3f << 24
-	MACA1H = 0xffff << 0
+    AE     = 1 << 31
+    SA     = 1 << 30
+    MBC    = 0x3f << 24
+    MACA1H = 0xffff << 0
 
 class ETH_MACA2HR(IntEnum):
-	AE     = 1 << 31
-	SA     = 1 << 30
-	MBC    = 0x3f << 24
-	MACA2H = 0xffff << 0
+    AE     = 1 << 31
+    SA     = 1 << 30
+    MBC    = 0x3f << 24
+    MACA2H = 0xffff << 0
 
 class ETH_MACA3HR(IntEnum):
-	AE     = 1 << 31
-	SA     = 1 << 30
-	MBC    = 0x3f << 24
-	MACA3H = 0xffff << 0
+    AE     = 1 << 31
+    SA     = 1 << 30
+    MBC    = 0x3f << 24
+    MACA3H = 0xffff << 0
 
 class ETH_MMCCR(IntEnum):
-	MCFHP = 1 << 5
-	MCP   = 1 << 4
-	MCF   = 1 << 3
-	ROR   = 1 << 2
-	CSR   = 1 << 1
-	CR    = 1 << 0
+    MCFHP = 1 << 5
+    MCP   = 1 << 4
+    MCF   = 1 << 3
+    ROR   = 1 << 2
+    CSR   = 1 << 1
+    CR    = 1 << 0
 
 class ETH_MMCRIR(IntEnum):
-	RGUFS = 1 << 17
-	RFAES = 1 << 6
-	RFCES = 1 << 5
+    RGUFS = 1 << 17
+    RFAES = 1 << 6
+    RFCES = 1 << 5
 
 class ETH_MMCTIR(IntEnum):
-	TGFS    = 1 << 21
-	TGFMSCS = 1 << 15
-	TGFSCS  = 1 << 14
+    TGFS    = 1 << 21
+    TGFMSCS = 1 << 15
+    TGFSCS  = 1 << 14
 
 class ETH_MMCRIMR(IntEnum):
-	RGUFM = 1 << 17
-	RFAEM = 1 << 6
-	RFCEM = 1 << 5
+    RGUFM = 1 << 17
+    RFAEM = 1 << 6
+    RFCEM = 1 << 5
 
 class ETH_MMCTIMR(IntEnum):
-	TGFM    = 1 << 21
-	TGFMSCM = 1 << 15
-	TGFSCM  = 1 << 14
+    TGFM    = 1 << 21
+    TGFMSCM = 1 << 15
+    TGFSCM  = 1 << 14
 
 class ETH_PTPTSCR(IntEnum):
-	TSCNT = 0x3 << 16
-	TSARU = 1 << 5
-	TSITE = 1 << 4
-	TSSTU = 1 << 3
-	TSSTI = 1 << 2
-	TSFCU = 1 << 1
-	TSE   = 1 << 0
+    TSCNT = 0x3 << 16
+    TSARU = 1 << 5
+    TSITE = 1 << 4
+    TSSTU = 1 << 3
+    TSSTI = 1 << 2
+    TSFCU = 1 << 1
+    TSE   = 1 << 0
 
 class ETH_PTPTSSR(IntEnum):
-	TSSMRME    = 1 << 15
-	TSSEME     = 1 << 14
-	TSSIPV4FE  = 1 << 13
-	TSSIPV6FE  = 1 << 12
-	TSSPTPOEFE = 1 << 11
-	TSPTPPSV2E = 1 << 10
-	TSSSR      = 1 << 9
-	TSSARFE    = 1 << 8
-	TSTTR      = 1 << 5
-	TSSO       = 1 << 4
+    TSSMRME    = 1 << 15
+    TSSEME     = 1 << 14
+    TSSIPV4FE  = 1 << 13
+    TSSIPV6FE  = 1 << 12
+    TSSPTPOEFE = 1 << 11
+    TSPTPPSV2E = 1 << 10
+    TSSSR      = 1 << 9
+    TSSARFE    = 1 << 8
+    TSTTR      = 1 << 5
+    TSSO       = 1 << 4
 
 class ETH_PTPSSIR(IntEnum):
-	STSSI = 0xff << 0
+    STSSI = 0xff << 0
 
 class ETH_PTPTSLR(IntEnum):
-	STPNS = 1 << 31
-	STSS  = 0x7fffffff << 0
+    STPNS = 1 << 31
+    STSS  = 0x7fffffff << 0
 
 class ETH_PTPTSLUR(IntEnum):
-	TSUPNS = 1 << 31
-	TSUSS  = 0x7fffffff << 0
+    TSUPNS = 1 << 31
+    TSUSS  = 0x7fffffff << 0
 
 class ETH_DMABMR(IntEnum):
-	AAB  = 1 << 25
-	FPM  = 1 << 24
-	USP  = 1 << 23
-	RDP  = 0x3f << 17
-	FB   = 1 << 16
-	RTPR = 0x3 << 14
-	PBL  = 0x3f << 8
-	EDE  = 1 << 7
-	DSL  = 0x1f << 2
-	DA   = 1 << 1
-	SR   = 1 << 0
+    AAB  = 1 << 25
+    FPM  = 1 << 24
+    USP  = 1 << 23
+    RDP  = 0x3f << 17
+    FB   = 1 << 16
+    RTPR = 0x3 << 14
+    PBL  = 0x3f << 8
+    EDE  = 1 << 7
+    DSL  = 0x1f << 2
+    DA   = 1 << 1
+    SR   = 1 << 0
 
 class ETH_DMASR(IntEnum):
-	TSTS             = 1 << 29
-	PMTS             = 1 << 28
-	MMCS             = 1 << 27
-	EBS              = 0x7 << 23
-	EBS_DescAccess   = 1 << 25
-	EBS_ReadTransf   = 1 << 24
-	EBS_DataTransfTx = 1 << 23
-	TPS              = 0x7 << 20
-	TPS_Fetching     = 1 << 20
-	TPS_Waiting      = 1 << 21
-	TPS_Reading      = 0x3 << 20
-	TPS_Suspended    = 0x3 << 21
-	TPS_Closing      = 0x7 << 20
-	RPS              = 0x7 << 17
-	RPS_Fetching     = 1 << 17
-	RPS_Waiting      = 0x3 << 17
-	RPS_Suspended    = 1 << 19
-	RPS_Closing      = 0x5 << 17
-	RPS_Queuing      = 0x7 << 17
-	NIS              = 1 << 16
-	AIS              = 1 << 15
-	ERS              = 1 << 14
-	FBES             = 1 << 13
-	ETS              = 1 << 10
-	RWTS             = 1 << 9
-	RPSS             = 1 << 8
-	RBUS             = 1 << 7
-	RS               = 1 << 6
-	TUS              = 1 << 5
-	ROS              = 1 << 4
-	TJTS             = 1 << 3
-	TBUS             = 1 << 2
-	TPSS             = 1 << 1
-	TS               = 1 << 0
+    TSTS             = 1 << 29
+    PMTS             = 1 << 28
+    MMCS             = 1 << 27
+    EBS              = 0x7 << 23
+    EBS_DescAccess   = 1 << 25
+    EBS_ReadTransf   = 1 << 24
+    EBS_DataTransfTx = 1 << 23
+    TPS              = 0x7 << 20
+    TPS_Fetching     = 1 << 20
+    TPS_Waiting      = 1 << 21
+    TPS_Reading      = 0x3 << 20
+    TPS_Suspended    = 0x3 << 21
+    TPS_Closing      = 0x7 << 20
+    RPS              = 0x7 << 17
+    RPS_Fetching     = 1 << 17
+    RPS_Waiting      = 0x3 << 17
+    RPS_Suspended    = 1 << 19
+    RPS_Closing      = 0x5 << 17
+    RPS_Queuing      = 0x7 << 17
+    NIS              = 1 << 16
+    AIS              = 1 << 15
+    ERS              = 1 << 14
+    FBES             = 1 << 13
+    ETS              = 1 << 10
+    RWTS             = 1 << 9
+    RPSS             = 1 << 8
+    RBUS             = 1 << 7
+    RS               = 1 << 6
+    TUS              = 1 << 5
+    ROS              = 1 << 4
+    TJTS             = 1 << 3
+    TBUS             = 1 << 2
+    TPSS             = 1 << 1
+    TS               = 1 << 0
 
 class ETH_DMAOMR(IntEnum):
-	DTCEFD = 1 << 26
-	RSF    = 1 << 25
-	DFRF   = 1 << 24
-	TSF    = 1 << 21
-	FTF    = 1 << 20
-	TTC    = 0x7 << 14
-	ST     = 1 << 13
-	FEF    = 1 << 7
-	FGF    = 1 << 6
-	RTC    = 0x3 << 3
-	OSF    = 1 << 2
-	SR     = 1 << 1
+    DTCEFD = 1 << 26
+    RSF    = 1 << 25
+    DFRF   = 1 << 24
+    TSF    = 1 << 21
+    FTF    = 1 << 20
+    TTC    = 0x7 << 14
+    ST     = 1 << 13
+    FEF    = 1 << 7
+    FGF    = 1 << 6
+    RTC    = 0x3 << 3
+    OSF    = 1 << 2
+    SR     = 1 << 1
 
 class ETH_DMAIER(IntEnum):
-	NISE  = 1 << 16
-	AISE  = 1 << 15
-	ERIE  = 1 << 14
-	FBEIE = 1 << 13
-	ETIE  = 1 << 10
-	RWTIE = 1 << 9
-	RPSIE = 1 << 8
-	RBUIE = 1 << 7
-	RIE   = 1 << 6
-	TUIE  = 1 << 5
-	ROIE  = 1 << 4
-	TJTIE = 1 << 3
-	TBUIE = 1 << 2
-	TPSIE = 1 << 1
-	TIE   = 1 << 0
+    NISE  = 1 << 16
+    AISE  = 1 << 15
+    ERIE  = 1 << 14
+    FBEIE = 1 << 13
+    ETIE  = 1 << 10
+    RWTIE = 1 << 9
+    RPSIE = 1 << 8
+    RBUIE = 1 << 7
+    RIE   = 1 << 6
+    TUIE  = 1 << 5
+    ROIE  = 1 << 4
+    TJTIE = 1 << 3
+    TBUIE = 1 << 2
+    TPSIE = 1 << 1
+    TIE   = 1 << 0
 
 class ETH_DMAMFBOCR(IntEnum):
-	OFOC = 1 << 28
-	MFA  = 0x7ff << 17
-	OMFC = 1 << 16
-	MFC  = 0xffff << 0
+    OFOC = 1 << 28
+    MFA  = 0x7ff << 17
+    OMFC = 1 << 16
+    MFC  = 0xffff << 0
```

### Comparing `qiling-1.4.5/qiling/hw/const/stm32f4xx_i2c.py` & `qiling-1.4.6/qiling/hw/const/stm32f4xx_spi.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,93 +2,68 @@
 # 
 # Cross Platform and Multi Architecture Advanced Binary Emulation Framework
 #
 
 from enum import IntEnum
 
 
-class I2C_CR1(IntEnum):
-	PE        = 1 << 0
-	SMBUS     = 1 << 1
-	SMBTYPE   = 1 << 3
-	ENARP     = 1 << 4
-	ENPEC     = 1 << 5
-	ENGC      = 1 << 6
-	NOSTRETCH = 1 << 7
-	START     = 1 << 8
-	STOP      = 1 << 9
-	ACK       = 1 << 10
-	POS       = 1 << 11
-	PEC       = 1 << 12
-	ALERT     = 1 << 13
-	SWRST     = 1 << 15
-
-	RW_MASK = PE|SMBUS|SMBTYPE|ENARP|ENPEC|ENGC|NOSTRETCH|START|STOP|ACK|POS|ALERT|SWRST
-
-class I2C_CR2(IntEnum):
-	FREQ    = 0x3f << 0
-	ITERREN = 1 << 8
-	ITEVTEN = 1 << 9
-	ITBUFEN = 1 << 10
-	DMAEN   = 1 << 11
-	LAST    = 1 << 12
-
-class I2C_OAR1(IntEnum):
-	ADD0    = 1 << 0
-	ADD1    = 1 << 1
-	ADD2    = 1 << 2
-	ADD3    = 1 << 3
-	ADD4    = 1 << 4
-	ADD5    = 1 << 5
-	ADD6    = 1 << 6
-	ADD7    = 1 << 7
-	ADD8    = 1 << 8
-	ADD9    = 1 << 9
-	ADDMODE = 1 << 15
-
-	ADDR1_7B = 0x7f << 1
-	ADDR1_10B = 0x3ff
-
-class I2C_OAR2(IntEnum):
-	ENDUAL = 1 << 0
-	ADDR2   = 0x7f << 1
-
-class I2C_DR(IntEnum):
-	DR = 0xff << 0
-
-class I2C_SR1(IntEnum):
-	SB       = 1 << 0
-	ADDR     = 1 << 1
-	BTF      = 1 << 2
-	ADD10    = 1 << 3
-	STOPF    = 1 << 4
-	RXNE     = 1 << 6
-	TXE      = 1 << 7
-	BERR     = 1 << 8
-	ARLO     = 1 << 9
-	AF       = 1 << 10
-	OVR      = 1 << 11
-	PECERR   = 1 << 12
-	TIMEOUT  = 1 << 14
-	SMBALERT = 1 << 15
-
-class I2C_SR2(IntEnum):
-	MSL        = 1 << 0
-	BSY        = 1 << 1
-	TRA        = 1 << 2
-	GENCALL    = 1 << 4
-	SMBDEFAULT = 1 << 5
-	SMBHOST    = 1 << 6
-	DALF       = 1 << 7
-	PEC        = 0xff << 8
-
-class I2C_CCR(IntEnum):
-	CCR = 0xfff << 0
-	DTY = 1 << 14
-	FS  = 1 << 15
-
-class I2C_TRISE(IntEnum):
-	TRISE = 0x3f << 0
-
-class I2C_FLTR(IntEnum):
-	DNF   = 0xf << 0
-	ANOFF = 1 << 4
+class SPI_CR1(IntEnum):
+    CPHA     = 1 << 0
+    CPOL     = 1 << 1
+    MSTR     = 1 << 2
+    BR       = 0x7 << 3
+    SPE      = 1 << 6
+    LSBFIRST = 1 << 7
+    SSI      = 1 << 8
+    SSM      = 1 << 9
+    RXONLY   = 1 << 10
+    DFF      = 1 << 11
+    CRCNEXT  = 1 << 12
+    CRCEN    = 1 << 13
+    BIDIOE   = 1 << 14
+    BIDIMODE = 1 << 15
+
+    RW_MASK = 0xffff
+
+class SPI_CR2(IntEnum):
+    RXDMAEN = 1 << 0
+    TXDMAEN = 1 << 1
+    SSOE    = 1 << 2
+    FRF     = 1 << 4
+    ERRIE   = 1 << 5
+    RXNEIE  = 1 << 6
+    TXEIE   = 1 << 7
+
+    RW_MASK = RXDMAEN|TXDMAEN|SSOE|FRF|ERRIE|RXNEIE|TXEIE
+
+class SPI_SR(IntEnum):
+    RXNE   = 1 << 0
+    TXE    = 1 << 1
+    CHSIDE = 1 << 2
+    UDR    = 1 << 3
+    CRCERR = 1 << 4
+    MODF   = 1 << 5
+    OVR    = 1 << 6
+    BSY    = 1 << 7
+    FRE    = 1 << 8
+
+class SPI_CRCPR(IntEnum):
+    CRCPOLY = 0xffff
+
+class SPI_I2SCFGR(IntEnum):
+    CHLEN   = 1 << 0
+    DATLEN  = 0x3 << 1
+    CKPOL   = 1 << 3
+    I2SSTD  = 0x3 << 4
+    PCMSYNC = 1 << 7
+    I2SCFG  = 0x3 << 8
+    I2SE    = 1 << 10
+    I2SMOD  = 1 << 11
+
+    RW_MASK = CHLEN|DATLEN|CKPOL|I2SSTD|PCMSYNC|I2SCFG|I2SE|I2SMOD
+
+class SPI_I2SPR(IntEnum):
+    I2SDIV = 0xff << 0
+    ODD    = 1 << 8
+    MCKOE  = 1 << 9
+
+    RW_MASK = I2SDIV|ODD|MCKOE
```

### Comparing `qiling-1.4.5/qiling/hw/const/stm32f4xx_pwr.py` & `qiling-1.4.6/qiling/hw/const/stm32f4xx_pwr.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,34 +3,34 @@
 # Cross Platform and Multi Architecture Advanced Binary Emulation Framework
 #
 
 from enum import IntEnum
 
 
 class PWR_CR(IntEnum):
-	LPDS   = 1 << 0
-	PDDS   = 1 << 1
-	CWUF   = 1 << 2
-	CSBF   = 1 << 3
-	PVDE   = 1 << 4
-	PLS    = 0x7 << 5
-	DBP    = 1 << 8
-	FPDS   = 1 << 9
-	LPLVDS = 1 << 10
-	MRLVDS = 1 << 11
-	ADCDC1 = 1 << 13
-	VOS    = 0x3 << 14
-	ODEN   = 1 << 16
-	ODSWEN = 1 << 17
-	UDEN   = 0x3 << 18
+    LPDS   = 1 << 0
+    PDDS   = 1 << 1
+    CWUF   = 1 << 2
+    CSBF   = 1 << 3
+    PVDE   = 1 << 4
+    PLS    = 0x7 << 5
+    DBP    = 1 << 8
+    FPDS   = 1 << 9
+    LPLVDS = 1 << 10
+    MRLVDS = 1 << 11
+    ADCDC1 = 1 << 13
+    VOS    = 0x3 << 14
+    ODEN   = 1 << 16
+    ODSWEN = 1 << 17
+    UDEN   = 0x3 << 18
 
 class PWR_CSR(IntEnum):
-	WUF     = 1 << 0
-	SBF     = 1 << 1
-	PVDO    = 1 << 2
-	BRR     = 1 << 3
-	EWUP    = 1 << 8
-	BRE     = 1 << 9
-	VOSRDY  = 1 << 14
-	ODRDY   = 1 << 16
-	ODSWRDY = 1 << 17
-	UDRDY   = 0x3 << 18
+    WUF     = 1 << 0
+    SBF     = 1 << 1
+    PVDO    = 1 << 2
+    BRR     = 1 << 3
+    EWUP    = 1 << 8
+    BRE     = 1 << 9
+    VOSRDY  = 1 << 14
+    ODRDY   = 1 << 16
+    ODSWRDY = 1 << 17
+    UDRDY   = 0x3 << 18
```

### Comparing `qiling-1.4.5/qiling/hw/const/stm32f4xx_rtc.py` & `qiling-1.4.6/qiling/hw/const/stm32f1xx_adc.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,168 +1,100 @@
 #!/usr/bin/env python3
-# 
+#
 # Cross Platform and Multi Architecture Advanced Binary Emulation Framework
 #
 
-
 from enum import IntEnum
 
 
-class RTC_TR(IntEnum):
-	PM  = 1 << 22
-	HT  = 0x3 << 20
-	HU  = 0xf << 16
-	MNT = 0x7 << 12
-	MNU = 0xf << 8
-	ST  = 0x7 << 4
-	SU  = 0xf << 0
-
-class RTC_DR(IntEnum):
-	YT  = 0xf << 20
-	YU  = 0xf << 16
-	WDU = 0x7 << 13
-	MT  = 1 << 12
-	MU  = 0xf << 8
-	DT  = 0x3 << 4
-	D   = 0xf << 0
-
-class RTC_CR(IntEnum):
-	COE     = 1 << 23
-	OSEL    = 0x3 << 21
-	POL     = 1 << 20
-	COSEL   = 1 << 19
-	BKP     = 1 << 18
-	SUB1H   = 1 << 17
-	ADD1H   = 1 << 16
-	TSIE    = 1 << 15
-	WUTIE   = 1 << 14
-	ALRBIE  = 1 << 13
-	ALRAIE  = 1 << 12
-	TSE     = 1 << 11
-	WUTE    = 1 << 10
-	ALRBE   = 1 << 9
-	ALRAE   = 1 << 8
-	DCE     = 1 << 7
-	FMT     = 1 << 6
-	BYPSHAD = 1 << 5
-	REFCKON = 1 << 4
-	TSEDGE  = 1 << 3
-	WUCKSEL = 0x7 << 0
-
-class RTC_ISR(IntEnum):
-	RECALPF = 1 << 16
-	TAMP1F  = 1 << 13
-	TAMP2F  = 1 << 14
-	TSOVF   = 1 << 12
-	TSF     = 1 << 11
-	WUTF    = 1 << 10
-	ALRBF   = 1 << 9
-	ALRAF   = 1 << 8
-	INIT    = 1 << 7
-	INITF   = 1 << 6
-	RSF     = 1 << 5
-	INITS   = 1 << 4
-	SHPF    = 1 << 3
-	WUTWF   = 1 << 2
-	ALRBWF  = 1 << 1
-	ALRAWF  = 1 << 0
-
-class RTC_PRER(IntEnum):
-	PREDIV_A = 0x7f << 16
-	PREDIV_S = 0x7fff << 0
-
-class RTC_WUTR(IntEnum):
-	WUT = 0xffff << 0
-
-class RTC_CALIBR(IntEnum):
-	DCS = 1 << 7
-	DC  = 0x1f << 0
-
-class RTC_ALRMAR(IntEnum):
-	MSK4  = 1 << 31
-	WDSEL = 1 << 30
-	DT    = 0x3 << 28
-	D     = 0xf << 24
-	MSK3  = 1 << 23
-	PM    = 1 << 22
-	HT    = 0x3 << 20
-	HU    = 0xf << 16
-	MSK2  = 1 << 15
-	MNT   = 0x7 << 12
-	MNU   = 0xf << 8
-	MSK1  = 1 << 7
-	ST    = 0x7 << 4
-	SU    = 0xf << 0
-
-class RTC_ALRMBR(IntEnum):
-	MSK4  = 1 << 31
-	WDSEL = 1 << 30
-	DT    = 0x3 << 28
-	D     = 0xf << 24
-	MSK3  = 1 << 23
-	PM    = 1 << 22
-	HT    = 0x3 << 20
-	HU    = 0xf << 16
-	MSK2  = 1 << 15
-	MNT   = 0x7 << 12
-	MNU   = 0xf << 8
-	MSK1  = 1 << 7
-	ST    = 0x7 << 4
-	SU    = 0xf << 0
-
-class RTC_WPR(IntEnum):
-	KEY = 0xff << 0
-
-class RTC_SSR(IntEnum):
-	SS = 0xffff << 0
-
-class RTC_SHIFTR(IntEnum):
-	SUBFS = 0x7fff << 0
-	ADD1S = 1 << 31
-
-class RTC_TSTR(IntEnum):
-	PM  = 1 << 22
-	HT  = 0x3 << 20
-	HU  = 0xf << 16
-	MNT = 0x7 << 12
-	MNU = 0xf << 8
-	ST  = 0x7 << 4
-	SU  = 0xf << 0
-
-class RTC_TSDR(IntEnum):
-	WDU = 0x7 << 13
-	MT  = 1 << 12
-	MU  = 0xf << 8
-	DT  = 0x3 << 4
-	D   = 0xf << 0
-
-class RTC_TSSSR(IntEnum):
-	SS = 0xffff << 0
-
-class RTC_CALR(IntEnum):
-	CALP   = 1 << 15
-	CALW8  = 1 << 14
-	CALW16 = 1 << 13
-	CALM   = 0x1ff << 0
-
-class RTC_TAFCR(IntEnum):
-	ALARMOUTTYPE = 1 << 18
-	TSINSEL      = 1 << 17
-	TAMP1INSEL   = 1 << 16
-	TAMPPUDIS    = 1 << 15
-	TAMPPRCH     = 0x3 << 13
-	TAMPFLT      = 0x3 << 11
-	TAMPFREQ     = 0x7 << 8
-	TAMPTS       = 1 << 7
-	TAMP2TRG     = 1 << 4
-	TAMP2E       = 1 << 3
-	TAMPIE       = 1 << 2
-	TAMP1TRG     = 1 << 1
-	TAMP1E       = 1 << 0
-
-class RTC_ALRMASSR(IntEnum):
-	MASKSS = 0xf << 24
-	SS     = 0x7fff << 0
-
-class RTC_ALRMBSSR(IntEnum):
-	MASKSS = 0xf << 24
-	SS     = 0x7fff << 0
+class ADC_SR(IntEnum):
+    AWD   = 1 << 0
+    EOS   = 1 << 1
+    JEOS  = 1 << 2
+    JSTRT = 1 << 3
+    STRT  = 1 << 4
+
+class ADC_CR1(IntEnum):
+    AWDCH   = 0x1f << 0
+    EOSIE   = 1 << 5
+    AWDIE   = 1 << 6
+    JEOSIE  = 1 << 7
+    SCAN    = 1 << 8
+    AWDSGL  = 1 << 9
+    JAUTO   = 1 << 10
+    DISCEN  = 1 << 11
+    JDISCEN = 1 << 12
+    DISCNUM = 0x7 << 13
+    DALMOD  = 0xf << 16
+    JAWDEN  = 1 << 22
+    AWDEN   = 1 << 23
+
+class ADC_CR2(IntEnum):
+    ADON     = 1 << 0
+    CONT     = 1 << 1
+    CAL      = 1 << 2
+    RSTCAL   = 1 << 3
+    DMA      = 1 << 8
+    ALIGN    = 1 << 11
+    JEXTSEL  = 0x7 << 12
+    JEXTTRIG = 1 << 15
+    EXTSEL   = 0x7 << 17
+    EXTTRIG  = 1 << 20
+    JSWSTART = 1 << 21
+    SWSTART  = 1 << 22
+    TSVREFE  = 1 << 23
+
+class ADC_SMPR1(IntEnum):
+    SMP10 = 0x7 << 0
+    SMP11 = 0x7 << 3
+    SMP12 = 0x7 << 6
+    SMP13 = 0x7 << 9
+    SMP14 = 0x7 << 12
+    SMP15 = 0x7 << 15
+    SMP16 = 0x7 << 18
+    SMP17 = 0x7 << 21
+
+class ADC_SMPR2(IntEnum):
+    SMP0 = 0x7 << 0
+    SMP1 = 0x7 << 3
+    SMP2 = 0x7 << 6
+    SMP3 = 0x7 << 9
+    SMP4 = 0x7 << 12
+    SMP5 = 0x7 << 15
+    SMP6 = 0x7 << 18
+    SMP7 = 0x7 << 21
+    SMP8 = 0x7 << 24
+    SMP9 = 0x7 << 27
+
+class ADC_SQR1(IntEnum):
+    SQ13 = 0x1f << 0
+    SQ14 = 0x1f << 5
+    SQ15 = 0x1f << 10
+    SQ16 = 0x1f << 15
+    L    = 0xf << 20
+
+class ADC_SQR2(IntEnum):
+    SQ7  = 0x1f << 0
+    SQ8  = 0x1f << 5
+    SQ9  = 0x1f << 10
+    SQ10 = 0x1f << 15
+    SQ11 = 0x1f << 20
+    SQ12 = 0x1f << 25
+
+class ADC_SQR3(IntEnum):
+    SQ1 = 0x1f << 0
+    SQ2 = 0x1f << 5
+    SQ3 = 0x1f << 10
+    SQ4 = 0x1f << 15
+    SQ5 = 0x1f << 20
+    SQ6 = 0x1f << 25
+
+class ADC_JSQR(IntEnum):
+    JSQ1 = 0x1f << 0
+    JSQ2 = 0x1f << 5
+    JSQ3 = 0x1f << 10
+    JSQ4 = 0x1f << 15
+    JL   = 0x3 << 20
+
+class ADC_DR(IntEnum):
+    DATA     = 0xffff << 0
+    ADC2DATA = 0xffff << 16
```

### Comparing `qiling-1.4.5/qiling/hw/const/stm32f4xx_sdio.py` & `qiling-1.4.6/qiling/hw/const/stm32f4xx_sdio.py`

 * *Files 27% similar despite different names*

```diff
@@ -3,103 +3,103 @@
 # Cross Platform and Multi Architecture Advanced Binary Emulation Framework
 #
 
 from enum import IntEnum
 
 
 class SDIO_CLKCR(IntEnum):
-	CLKDIV  = 0xff << 0
-	CLKEN   = 1 << 8
-	PWRSAV  = 1 << 9
-	BYPASS  = 1 << 10
-	WIDBUS  = 0x3 << 11
-	NEGEDGE = 1 << 13
-	HWFC_EN = 1 << 14
+    CLKDIV  = 0xff << 0
+    CLKEN   = 1 << 8
+    PWRSAV  = 1 << 9
+    BYPASS  = 1 << 10
+    WIDBUS  = 0x3 << 11
+    NEGEDGE = 1 << 13
+    HWFC_EN = 1 << 14
 
 class SDIO_CMD(IntEnum):
-	CMDINDEX    = 0x3f << 0
-	WAITRESP    = 0x3 << 6
-	WAITINT     = 1 << 8
-	WAITPEND    = 1 << 9
-	CPSMEN      = 1 << 10
-	SDIOSUSPEND = 1 << 11
-	ENCMDCOMPL  = 1 << 12
-	NIEN        = 1 << 13
-	CEATACMD    = 1 << 14
+    CMDINDEX    = 0x3f << 0
+    WAITRESP    = 0x3 << 6
+    WAITINT     = 1 << 8
+    WAITPEND    = 1 << 9
+    CPSMEN      = 1 << 10
+    SDIOSUSPEND = 1 << 11
+    ENCMDCOMPL  = 1 << 12
+    NIEN        = 1 << 13
+    CEATACMD    = 1 << 14
 
 class SDIO_DCTRL(IntEnum):
-	DTEN       = 1 << 0
-	DTDIR      = 1 << 1
-	DTMODE     = 1 << 2
-	DMAEN      = 1 << 3
-	DBLOCKSIZE = 0xf << 4
-	RWSTART    = 1 << 8
-	RWSTOP     = 1 << 9
-	RWMOD      = 1 << 10
-	SDIOEN     = 1 << 11
+    DTEN       = 1 << 0
+    DTDIR      = 1 << 1
+    DTMODE     = 1 << 2
+    DMAEN      = 1 << 3
+    DBLOCKSIZE = 0xf << 4
+    RWSTART    = 1 << 8
+    RWSTOP     = 1 << 9
+    RWMOD      = 1 << 10
+    SDIOEN     = 1 << 11
 
 class SDIO_STA(IntEnum):
-	CCRCFAIL = 1 << 0
-	DCRCFAIL = 1 << 1
-	CTIMEOUT = 1 << 2
-	DTIMEOUT = 1 << 3
-	TXUNDERR = 1 << 4
-	RXOVERR  = 1 << 5
-	CMDREND  = 1 << 6
-	CMDSENT  = 1 << 7
-	DATAEND  = 1 << 8
-	STBITERR = 1 << 9
-	DBCKEND  = 1 << 10
-	CMDACT   = 1 << 11
-	TXACT    = 1 << 12
-	RXACT    = 1 << 13
-	TXFIFOHE = 1 << 14
-	RXFIFOHF = 1 << 15
-	TXFIFOF  = 1 << 16
-	RXFIFOF  = 1 << 17
-	TXFIFOE  = 1 << 18
-	RXFIFOE  = 1 << 19
-	TXDAVL   = 1 << 20
-	RXDAVL   = 1 << 21
-	SDIOIT   = 1 << 22
-	CEATAEND = 1 << 23
+    CCRCFAIL = 1 << 0
+    DCRCFAIL = 1 << 1
+    CTIMEOUT = 1 << 2
+    DTIMEOUT = 1 << 3
+    TXUNDERR = 1 << 4
+    RXOVERR  = 1 << 5
+    CMDREND  = 1 << 6
+    CMDSENT  = 1 << 7
+    DATAEND  = 1 << 8
+    STBITERR = 1 << 9
+    DBCKEND  = 1 << 10
+    CMDACT   = 1 << 11
+    TXACT    = 1 << 12
+    RXACT    = 1 << 13
+    TXFIFOHE = 1 << 14
+    RXFIFOHF = 1 << 15
+    TXFIFOF  = 1 << 16
+    RXFIFOF  = 1 << 17
+    TXFIFOE  = 1 << 18
+    RXFIFOE  = 1 << 19
+    TXDAVL   = 1 << 20
+    RXDAVL   = 1 << 21
+    SDIOIT   = 1 << 22
+    CEATAEND = 1 << 23
 
 class SDIO_ICR(IntEnum):
-	CCRCFAILC = 1 << 0
-	DCRCFAILC = 1 << 1
-	CTIMEOUTC = 1 << 2
-	DTIMEOUTC = 1 << 3
-	TXUNDERRC = 1 << 4
-	RXOVERRC  = 1 << 5
-	CMDRENDC  = 1 << 6
-	CMDSENTC  = 1 << 7
-	DATAENDC  = 1 << 8
-	STBITERRC = 1 << 9
-	DBCKENDC  = 1 << 10
-	SDIOITC   = 1 << 22
-	CEATAENDC = 1 << 23
+    CCRCFAILC = 1 << 0
+    DCRCFAILC = 1 << 1
+    CTIMEOUTC = 1 << 2
+    DTIMEOUTC = 1 << 3
+    TXUNDERRC = 1 << 4
+    RXOVERRC  = 1 << 5
+    CMDRENDC  = 1 << 6
+    CMDSENTC  = 1 << 7
+    DATAENDC  = 1 << 8
+    STBITERRC = 1 << 9
+    DBCKENDC  = 1 << 10
+    SDIOITC   = 1 << 22
+    CEATAENDC = 1 << 23
 
 class SDIO_MASK(IntEnum):
-	CCRCFAILIE = 1 << 0
-	DCRCFAILIE = 1 << 1
-	CTIMEOUTIE = 1 << 2
-	DTIMEOUTIE = 1 << 3
-	TXUNDERRIE = 1 << 4
-	RXOVERRIE  = 1 << 5
-	CMDRENDIE  = 1 << 6
-	CMDSENTIE  = 1 << 7
-	DATAENDIE  = 1 << 8
-	STBITERRIE = 1 << 9
-	DBCKENDIE  = 1 << 10
-	CMDACTIE   = 1 << 11
-	TXACTIE    = 1 << 12
-	RXACTIE    = 1 << 13
-	TXFIFOHEIE = 1 << 14
-	RXFIFOHFIE = 1 << 15
-	TXFIFOFIE  = 1 << 16
-	RXFIFOFIE  = 1 << 17
-	TXFIFOEIE  = 1 << 18
-	RXFIFOEIE  = 1 << 19
-	TXDAVLIE   = 1 << 20
-	RXDAVLIE   = 1 << 21
-	SDIOITIE   = 1 << 22
-	CEATAENDIE = 1 << 23
+    CCRCFAILIE = 1 << 0
+    DCRCFAILIE = 1 << 1
+    CTIMEOUTIE = 1 << 2
+    DTIMEOUTIE = 1 << 3
+    TXUNDERRIE = 1 << 4
+    RXOVERRIE  = 1 << 5
+    CMDRENDIE  = 1 << 6
+    CMDSENTIE  = 1 << 7
+    DATAENDIE  = 1 << 8
+    STBITERRIE = 1 << 9
+    DBCKENDIE  = 1 << 10
+    CMDACTIE   = 1 << 11
+    TXACTIE    = 1 << 12
+    RXACTIE    = 1 << 13
+    TXFIFOHEIE = 1 << 14
+    RXFIFOHFIE = 1 << 15
+    TXFIFOFIE  = 1 << 16
+    RXFIFOFIE  = 1 << 17
+    TXFIFOEIE  = 1 << 18
+    RXFIFOEIE  = 1 << 19
+    TXDAVLIE   = 1 << 20
+    RXDAVLIE   = 1 << 21
+    SDIOITIE   = 1 << 22
+    CEATAENDIE = 1 << 23
```

### Comparing `qiling-1.4.5/qiling/hw/const/stm32f4xx_tim.py` & `qiling-1.4.6/qiling/hw/const/stm32f4xx_rtc.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,176 +1,168 @@
 #!/usr/bin/env python3
 # 
 # Cross Platform and Multi Architecture Advanced Binary Emulation Framework
 #
 
+
 from enum import IntEnum
 
 
-class TIM_CR1(IntEnum):
-	CEN  = 1 << 0
-	UDIS = 1 << 1
-	URS  = 1 << 2
-	OPM  = 1 << 3
-	DIR  = 1 << 4
-	CMS  = 0x3 << 5
-	ARPE = 1 << 7
-	CKD  = 0x3 << 8
-
-class TIM_CR2(IntEnum):
-	CCPC  = 1 << 0
-	CCS   = 1 << 2
-	CCDS  = 1 << 3
-	MMS   = 0x7 << 4
-	TI1S  = 1 << 7
-	OIS1  = 1 << 8
-	OIS1N = 1 << 9
-	OIS2  = 1 << 10
-	OIS2N = 1 << 11
-	OIS3  = 1 << 12
-	OIS3N = 1 << 13
-	OIS4  = 1 << 14
-
-class TIM_SMCR(IntEnum):
-	SMS  = 0x7 << 0
-	TS   = 0x7 << 4
-	MSM  = 1 << 7
-	ETF  = 0xf << 8
-	ETPS = 0x3 << 12
-	ECE  = 1 << 14
-	ETP  = 1 << 15
-
-class TIM_DIER(IntEnum):
-	UIE   = 1 << 0
-	CC1IE = 1 << 1
-	CC2IE = 1 << 2
-	CC3IE = 1 << 3
-	CC4IE = 1 << 4
-	COMIE = 1 << 5
-	TIE   = 1 << 6
-	BIE   = 1 << 7
-	UDE   = 1 << 8
-	CC1DE = 1 << 9
-	CC2DE = 1 << 10
-	CC3DE = 1 << 11
-	CC4DE = 1 << 12
-	COMDE = 1 << 13
-	TDE   = 1 << 14
-
-class TIM_SR(IntEnum):
-	UIF   = 1 << 0
-	CC1IF = 1 << 1
-	CC2IF = 1 << 2
-	CC3IF = 1 << 3
-	CC4IF = 1 << 4
-	COMIF = 1 << 5
-	TIF   = 1 << 6
-	BIF   = 1 << 7
-	CC1OF = 1 << 9
-	CC2OF = 1 << 10
-	CC3OF = 1 << 11
-	CC4OF = 1 << 12
-
-class TIM_EGR(IntEnum):
-	UG   = 1 << 0
-	CC1G = 1 << 1
-	CC2G = 1 << 2
-	CC3G = 1 << 3
-	CC4G = 1 << 4
-	COMG = 1 << 5
-	TG   = 1 << 6
-	BG   = 1 << 7
-
-class TIM_CCMR1(IntEnum):
-	CC1S   = 0x3 << 0
-	OC1FE  = 1 << 2
-	OC1PE  = 1 << 3
-	OC1M   = 0x7 << 4
-	OC1CE  = 1 << 7
-	CC2S   = 0x3 << 8
-	OC2FE  = 1 << 10
-	OC2PE  = 1 << 11
-	OC2M   = 0x7 << 12
-	OC2CE  = 1 << 15
-	IC1PSC = 0x3 << 2
-	IC1F   = 0xf << 4
-	IC2PSC = 0x3 << 10
-	IC2F   = 0xf << 12
-
-class TIM_CCMR2(IntEnum):
-	CC3S   = 0x3 << 0
-	OC3FE  = 1 << 2
-	OC3PE  = 1 << 3
-	OC3M   = 0x7 << 4
-	OC3CE  = 1 << 7
-	CC4S   = 0x3 << 8
-	OC4FE  = 1 << 10
-	OC4PE  = 1 << 11
-	OC4M   = 0x7 << 12
-	OC4CE  = 1 << 15
-	IC3PSC = 0x3 << 2
-	IC3F   = 0xf << 4
-	IC4PSC = 0x3 << 10
-	IC4F   = 0xf << 12
-
-class TIM_CCER(IntEnum):
-	CC1E  = 1 << 0
-	CC1P  = 1 << 1
-	CC1NE = 1 << 2
-	CC1NP = 1 << 3
-	CC2E  = 1 << 4
-	CC2P  = 1 << 5
-	CC2NE = 1 << 6
-	CC2NP = 1 << 7
-	CC3E  = 1 << 8
-	CC3P  = 1 << 9
-	CC3NE = 1 << 10
-	CC3NP = 1 << 11
-	CC4E  = 1 << 12
-	CC4P  = 1 << 13
-	CC4NP = 1 << 15
-
-class TIM_CNT(IntEnum):
-	CNT = 0xffffffff << 0
-
-class TIM_PSC(IntEnum):
-	PSC = 0xffff << 0
-
-class TIM_ARR(IntEnum):
-	ARR = 0xffffffff << 0
-
-class TIM_RCR(IntEnum):
-	REP = 0xff << 0
-
-class TIM_CCR1(IntEnum):
-	CCR1 = 0xffff << 0
-
-class TIM_CCR2(IntEnum):
-	CCR2 = 0xffff << 0
-
-class TIM_CCR3(IntEnum):
-	CCR3 = 0xffff << 0
-
-class TIM_CCR4(IntEnum):
-	CCR4 = 0xffff << 0
-
-class TIM_BDTR(IntEnum):
-	DTG  = 0xff << 0
-	LOCK = 0x3 << 8
-	OSSI = 1 << 10
-	OSSR = 1 << 11
-	BKE  = 1 << 12
-	BKP  = 1 << 13
-	AOE  = 1 << 14
-	MOE  = 1 << 15
-
-class TIM_DCR(IntEnum):
-	DBA = 0x1f << 0
-	DBL = 0x1f << 8
-
-class TIM_DMAR(IntEnum):
-	DMAB = 0xffff << 0
-
-class TIM_OR(IntEnum):
-	TI1_RMP  = 0x3 << 0
-	TI4_RMP  = 0x3 << 6
-	ITR1_RMP = 0x3 << 10
+class RTC_TR(IntEnum):
+    PM  = 1 << 22
+    HT  = 0x3 << 20
+    HU  = 0xf << 16
+    MNT = 0x7 << 12
+    MNU = 0xf << 8
+    ST  = 0x7 << 4
+    SU  = 0xf << 0
+
+class RTC_DR(IntEnum):
+    YT  = 0xf << 20
+    YU  = 0xf << 16
+    WDU = 0x7 << 13
+    MT  = 1 << 12
+    MU  = 0xf << 8
+    DT  = 0x3 << 4
+    D   = 0xf << 0
+
+class RTC_CR(IntEnum):
+    COE     = 1 << 23
+    OSEL    = 0x3 << 21
+    POL     = 1 << 20
+    COSEL   = 1 << 19
+    BKP     = 1 << 18
+    SUB1H   = 1 << 17
+    ADD1H   = 1 << 16
+    TSIE    = 1 << 15
+    WUTIE   = 1 << 14
+    ALRBIE  = 1 << 13
+    ALRAIE  = 1 << 12
+    TSE     = 1 << 11
+    WUTE    = 1 << 10
+    ALRBE   = 1 << 9
+    ALRAE   = 1 << 8
+    DCE     = 1 << 7
+    FMT     = 1 << 6
+    BYPSHAD = 1 << 5
+    REFCKON = 1 << 4
+    TSEDGE  = 1 << 3
+    WUCKSEL = 0x7 << 0
+
+class RTC_ISR(IntEnum):
+    RECALPF = 1 << 16
+    TAMP1F  = 1 << 13
+    TAMP2F  = 1 << 14
+    TSOVF   = 1 << 12
+    TSF     = 1 << 11
+    WUTF    = 1 << 10
+    ALRBF   = 1 << 9
+    ALRAF   = 1 << 8
+    INIT    = 1 << 7
+    INITF   = 1 << 6
+    RSF     = 1 << 5
+    INITS   = 1 << 4
+    SHPF    = 1 << 3
+    WUTWF   = 1 << 2
+    ALRBWF  = 1 << 1
+    ALRAWF  = 1 << 0
+
+class RTC_PRER(IntEnum):
+    PREDIV_A = 0x7f << 16
+    PREDIV_S = 0x7fff << 0
+
+class RTC_WUTR(IntEnum):
+    WUT = 0xffff << 0
+
+class RTC_CALIBR(IntEnum):
+    DCS = 1 << 7
+    DC  = 0x1f << 0
+
+class RTC_ALRMAR(IntEnum):
+    MSK4  = 1 << 31
+    WDSEL = 1 << 30
+    DT    = 0x3 << 28
+    D     = 0xf << 24
+    MSK3  = 1 << 23
+    PM    = 1 << 22
+    HT    = 0x3 << 20
+    HU    = 0xf << 16
+    MSK2  = 1 << 15
+    MNT   = 0x7 << 12
+    MNU   = 0xf << 8
+    MSK1  = 1 << 7
+    ST    = 0x7 << 4
+    SU    = 0xf << 0
+
+class RTC_ALRMBR(IntEnum):
+    MSK4  = 1 << 31
+    WDSEL = 1 << 30
+    DT    = 0x3 << 28
+    D     = 0xf << 24
+    MSK3  = 1 << 23
+    PM    = 1 << 22
+    HT    = 0x3 << 20
+    HU    = 0xf << 16
+    MSK2  = 1 << 15
+    MNT   = 0x7 << 12
+    MNU   = 0xf << 8
+    MSK1  = 1 << 7
+    ST    = 0x7 << 4
+    SU    = 0xf << 0
+
+class RTC_WPR(IntEnum):
+    KEY = 0xff << 0
+
+class RTC_SSR(IntEnum):
+    SS = 0xffff << 0
+
+class RTC_SHIFTR(IntEnum):
+    SUBFS = 0x7fff << 0
+    ADD1S = 1 << 31
+
+class RTC_TSTR(IntEnum):
+    PM  = 1 << 22
+    HT  = 0x3 << 20
+    HU  = 0xf << 16
+    MNT = 0x7 << 12
+    MNU = 0xf << 8
+    ST  = 0x7 << 4
+    SU  = 0xf << 0
+
+class RTC_TSDR(IntEnum):
+    WDU = 0x7 << 13
+    MT  = 1 << 12
+    MU  = 0xf << 8
+    DT  = 0x3 << 4
+    D   = 0xf << 0
+
+class RTC_TSSSR(IntEnum):
+    SS = 0xffff << 0
+
+class RTC_CALR(IntEnum):
+    CALP   = 1 << 15
+    CALW8  = 1 << 14
+    CALW16 = 1 << 13
+    CALM   = 0x1ff << 0
+
+class RTC_TAFCR(IntEnum):
+    ALARMOUTTYPE = 1 << 18
+    TSINSEL      = 1 << 17
+    TAMP1INSEL   = 1 << 16
+    TAMPPUDIS    = 1 << 15
+    TAMPPRCH     = 0x3 << 13
+    TAMPFLT      = 0x3 << 11
+    TAMPFREQ     = 0x7 << 8
+    TAMPTS       = 1 << 7
+    TAMP2TRG     = 1 << 4
+    TAMP2E       = 1 << 3
+    TAMPIE       = 1 << 2
+    TAMP1TRG     = 1 << 1
+    TAMP1E       = 1 << 0
+
+class RTC_ALRMASSR(IntEnum):
+    MASKSS = 0xf << 24
+    SS     = 0x7fff << 0
+
+class RTC_ALRMBSSR(IntEnum):
+    MASKSS = 0xf << 24
+    SS     = 0x7fff << 0
```

### Comparing `qiling-1.4.5/qiling/hw/const/stm32f4xx_usart.py` & `qiling-1.4.6/qiling/hw/const/stm32f4xx_usart.py`

 * *Files 18% similar despite different names*

```diff
@@ -16,19 +16,19 @@
     ORE  = 1 << 3
     NF   = 1 << 2
     FE   = 1 << 1
     PE   = 1 << 0
     RESET = TXE | TC
 
 class USART_DR(IntEnum):
-	DR = 0x1ff << 0
+    DR = 0x1ff << 0
 
 class USART_BRR(IntEnum):
-	DIV_Fraction = 0xf << 0
-	DIV_Mantissa = 0xfff << 4
+    DIV_Fraction = 0xf << 0
+    DIV_Mantissa = 0xfff << 4
 
 class USART_CR1(IntEnum):    
     OVER8  = 1 << 15
     UE     = 1 << 13
     M      = 1 << 12
     WAKE   = 1 << 11
     PCE    = 1 << 10
@@ -40,34 +40,34 @@
     IDLEIE = 1 << 4
     TE     = 1 << 3
     RE     = 1 << 2
     RWU    = 1 << 1
     SBK    = 1 << 0
 
 class USART_CR2(IntEnum):
-	ADD   = 0xf << 0
-	LBDL  = 1 << 5
-	LBDIE = 1 << 6
-	LBCL  = 1 << 8
-	CPHA  = 1 << 9
-	CPOL  = 1 << 10
-	CLKEN = 1 << 11
-	STOP  = 0x3 << 12
-	LINEN = 1 << 14
+    ADD   = 0xf << 0
+    LBDL  = 1 << 5
+    LBDIE = 1 << 6
+    LBCL  = 1 << 8
+    CPHA  = 1 << 9
+    CPOL  = 1 << 10
+    CLKEN = 1 << 11
+    STOP  = 0x3 << 12
+    LINEN = 1 << 14
 
 class USART_CR3(IntEnum):
-	EIE    = 1 << 0
-	IREN   = 1 << 1
-	IRLP   = 1 << 2
-	HDSEL  = 1 << 3
-	NACK   = 1 << 4
-	SCEN   = 1 << 5
-	DMAR   = 1 << 6
-	DMAT   = 1 << 7
-	RTSE   = 1 << 8
-	CTSE   = 1 << 9
-	CTSIE  = 1 << 10
-	ONEBIT = 1 << 11
+    EIE    = 1 << 0
+    IREN   = 1 << 1
+    IRLP   = 1 << 2
+    HDSEL  = 1 << 3
+    NACK   = 1 << 4
+    SCEN   = 1 << 5
+    DMAR   = 1 << 6
+    DMAT   = 1 << 7
+    RTSE   = 1 << 8
+    CTSE   = 1 << 9
+    CTSIE  = 1 << 10
+    ONEBIT = 1 << 11
 
 class USART_GTPR(IntEnum):
-	PSC = 0xff << 0
-	GT  = 0xff << 8
+    PSC = 0xff << 0
+    GT  = 0xff << 8
```

### Comparing `qiling-1.4.5/qiling/hw/dma/gd32vf1xx_dma.py` & `qiling-1.4.6/qiling/hw/dma/gd32vf1xx_dma.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/hw/dma/sam3xa_pdc.py` & `qiling-1.4.6/qiling/hw/dma/sam3xa_pdc.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/hw/dma/stm32f1xx_dma.py` & `qiling-1.4.6/qiling/hw/dma/stm32f1xx_dma.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/hw/dma/stm32f4xx_dma.py` & `qiling-1.4.6/qiling/hw/dma/stm32f4xx_dma.py`

 * *Files 16% similar despite different names*

```diff
@@ -65,44 +65,44 @@
         if self.NDTR == 0:
             self.CR &= ~DMA_SxCR.EN
             return True
         
 class STM32F4xxDma(QlPeripheral):
     class Type(ctypes.Structure):
         """ the structure available in :
-			stm32f413xx.h
-			stm32f407xx.h
-			stm32f469xx.h
-			stm32f446xx.h
-			stm32f427xx.h
-			stm32f401xc.h
-			stm32f415xx.h
-			stm32f412cx.h
-			stm32f410rx.h
-			stm32f410tx.h
-			stm32f439xx.h
-			stm32f412vx.h
-			stm32f417xx.h
-			stm32f479xx.h
-			stm32f429xx.h
-			stm32f412rx.h
-			stm32f423xx.h
-			stm32f437xx.h
-			stm32f412zx.h
-			stm32f401xe.h
-			stm32f410cx.h
-			stm32f405xx.h
-			stm32f411xe.h 
-		"""
+            stm32f413xx.h
+            stm32f407xx.h
+            stm32f469xx.h
+            stm32f446xx.h
+            stm32f427xx.h
+            stm32f401xc.h
+            stm32f415xx.h
+            stm32f412cx.h
+            stm32f410rx.h
+            stm32f410tx.h
+            stm32f439xx.h
+            stm32f412vx.h
+            stm32f417xx.h
+            stm32f479xx.h
+            stm32f429xx.h
+            stm32f412rx.h
+            stm32f423xx.h
+            stm32f437xx.h
+            stm32f412zx.h
+            stm32f401xe.h
+            stm32f410cx.h
+            stm32f405xx.h
+            stm32f411xe.h 
+        """
 
         _fields_ = [
-			('LISR' , ctypes.c_uint32),  # DMA low interrupt status register,      Address offset: 0x00
-			('HISR' , ctypes.c_uint32),  # DMA high interrupt status register,     Address offset: 0x04
-			('LIFCR', ctypes.c_uint32),  # DMA low interrupt flag clear register,  Address offset: 0x08
-			('HIFCR', ctypes.c_uint32),  # DMA high interrupt flag clear register, Address offset: 0x0C
+            ('LISR' , ctypes.c_uint32),  # DMA low interrupt status register,      Address offset: 0x00
+            ('HISR' , ctypes.c_uint32),  # DMA high interrupt status register,     Address offset: 0x04
+            ('LIFCR', ctypes.c_uint32),  # DMA low interrupt flag clear register,  Address offset: 0x08
+            ('HIFCR', ctypes.c_uint32),  # DMA high interrupt flag clear register, Address offset: 0x0C
             ('stream', Stream * 8),
         ]
 
     def __init__(
             self, ql, label, 
             stream0_intn=None,
             stream1_intn=None,
```

### Comparing `qiling-1.4.5/qiling/hw/external_device/lcd/const.py` & `qiling-1.4.6/qiling/hw/external_device/lcd/const.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/hw/external_device/lcd/lcd1602.py` & `qiling-1.4.6/qiling/hw/external_device/lcd/lcd1602.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/hw/external_device/oled/ssd1306.py` & `qiling-1.4.6/qiling/hw/external_device/oled/ssd1306.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/hw/flash/sam3xa_efc.py` & `qiling-1.4.6/qiling/hw/flash/sam3xa_efc.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/hw/flash/stm32f1xx_flash.py` & `qiling-1.4.6/qiling/hw/flash/stm32f1xx_flash.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     def __init__(self, ql: Qiling, label: str, intn: int = None):
         super().__init__(ql, label)
 
         self.intn = intn
         self.instance = self.struct()
 
     @QlPeripheral.monitor()
-    def read(self, offset: int, size: int) -> int:		
+    def read(self, offset: int, size: int) -> int:        
         buf = ctypes.create_string_buffer(size)
         ctypes.memmove(buf, ctypes.addressof(self.instance) + offset, size)
         return int.from_bytes(buf.raw, byteorder='little')
     
     @QlPeripheral.monitor()
     def write(self, offset: int, size: int, value: int):
         data = (value).to_bytes(size, 'little')
```

### Comparing `qiling-1.4.5/qiling/hw/flash/stm32f4xx_flash.py` & `qiling-1.4.6/qiling/hw/flash/stm32f4xx_flash.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     def __init__(self, ql: Qiling, label: str, intn: int = None):
         super().__init__(ql, label)
 
         self.intn = intn
         self.instance = self.struct()
 
     @QlPeripheral.monitor()
-    def read(self, offset: int, size: int) -> int:		
+    def read(self, offset: int, size: int) -> int:        
         buf = ctypes.create_string_buffer(size)
         ctypes.memmove(buf, ctypes.addressof(self.instance) + offset, size)
         return int.from_bytes(buf.raw, byteorder='little')
     
     @QlPeripheral.monitor()
     def write(self, offset: int, size: int, value: int):
         data = (value).to_bytes(size, 'little')
```

### Comparing `qiling-1.4.5/qiling/hw/gpio/gd32vf1xx_gpio.py` & `qiling-1.4.6/qiling/hw/gpio/gd32vf1xx_gpio.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
             OCTL  =  0x00000000,
             BOP   =  0x00000000,
             BC    =  0x00000000,
             LOCK  =  0x00000000,
         )
 
     @QlPeripheral.monitor()
-    def read(self, offset: int, size: int) -> int:		
+    def read(self, offset: int, size: int) -> int:        
         buf = ctypes.create_string_buffer(size)
         ctypes.memmove(buf, ctypes.addressof(self.instance) + offset, size)
         return int.from_bytes(buf.raw, byteorder='little')
     
     @QlPeripheral.monitor()
     def write(self, offset: int, size: int, value: int):
         if offset == self.struct.OCTL.offset:
```

### Comparing `qiling-1.4.5/qiling/hw/gpio/hooks.py` & `qiling-1.4.6/qiling/hw/gpio/hooks.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/hw/gpio/mk64f12_gpio.py` & `qiling-1.4.6/qiling/hw/gpio/mk64f12_gpio.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/hw/gpio/mk64f12_port.py` & `qiling-1.4.6/qiling/hw/gpio/mk64f12_port.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/hw/gpio/sam3xa_pio.py` & `qiling-1.4.6/qiling/hw/gpio/sam3xa_pio.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/hw/gpio/stm32f1xx_afio.py` & `qiling-1.4.6/qiling/hw/gpio/stm32f1xx_afio.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
     def __init__(self, ql, label):
         super().__init__(ql, label)
 
         self.instance = self.struct()
 
     @QlPeripheral.monitor()
-    def read(self, offset: int, size: int) -> int:		
+    def read(self, offset: int, size: int) -> int:        
         buf = ctypes.create_string_buffer(size)
         ctypes.memmove(buf, ctypes.addressof(self.instance) + offset, size)
         return int.from_bytes(buf.raw, byteorder='little')
 
     @QlPeripheral.monitor()
     def write(self, offset: int, size: int, value: int):
         data = (value).to_bytes(size, 'little')
```

### Comparing `qiling-1.4.5/qiling/hw/gpio/stm32f1xx_gpio.py` & `qiling-1.4.6/qiling/hw/gpio/stm32f1xx_gpio.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/hw/gpio/stm32f4xx_gpio.py` & `qiling-1.4.6/qiling/hw/gpio/stm32f4xx_gpio.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
             stm32f423xx.h
             stm32f437xx.h
             stm32f412zx.h
             stm32f401xe.h
             stm32f410cx.h
             stm32f405xx.h
             stm32f411xe.h 
-		"""
+        """
 
         _fields_ = [
             ('MODER'  , ctypes.c_uint32),      # GPIO port mode register,               Address offset: 0x00
             ('OTYPER' , ctypes.c_uint32),      # GPIO port output type register,        Address offset: 0x04
             ('OSPEEDR', ctypes.c_uint32),      # GPIO port output speed register,       Address offset: 0x08
             ('PUPDR'  , ctypes.c_uint32),      # GPIO port pull-up/pull-down register,  Address offset: 0x0C
             ('IDR'    , ctypes.c_uint32),      # GPIO port input data register,         Address offset: 0x10
```

### Comparing `qiling-1.4.5/qiling/hw/hw.py` & `qiling-1.4.6/qiling/hw/hw.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/hw/i2c/gd32vf1xx_i2c.py` & `qiling-1.4.6/qiling/hw/i2c/gd32vf1xx_i2c.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/hw/i2c/stm32f1xx_i2c.py` & `qiling-1.4.6/qiling/hw/i2c/stm32f1xx_i2c.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/hw/i2c/stm32f4xx_i2c.py` & `qiling-1.4.6/qiling/hw/i2c/stm32f4xx_i2c.py`

 * *Files 27% similar despite different names*

```diff
@@ -9,230 +9,230 @@
 from qiling.hw.peripheral import QlPeripheral
 from qiling.hw.connectivity import QlConnectivityPeripheral
 from qiling.hw.const.stm32f4xx_i2c import I2C_CR1, I2C_CR2, I2C_SR1, I2C_SR2, I2C_DR, I2C_OAR1, I2C_OAR2
 from qiling.hw.utils.access import Access, AccessSequence, Action
 
 
 class STM32F4xxI2c(QlConnectivityPeripheral):
-	class Type(ctypes.Structure):
-		""" the structure is available in :
-			stm32f423xx.h
-			stm32f469xx.h
-			stm32f427xx.h
-			stm32f479xx.h
-			stm32f413xx.h
-			stm32f429xx.h
-			stm32f439xx.h
-			stm32f412cx.h
-			stm32f412rx.h
-			stm32f410tx.h
-			stm32f410cx.h
-			stm32f412zx.h
-			stm32f446xx.h
-			stm32f401xc.h
-			stm32f437xx.h
-			stm32f401xe.h
-			stm32f412vx.h
-			stm32f410rx.h
-			stm32f411xe.h 
-		"""
-
-		_fields_ = [
-			('CR1'  , ctypes.c_uint32),  # I2C Control register 1,     Address offset: 0x00
-			('CR2'  , ctypes.c_uint32),  # I2C Control register 2,     Address offset: 0x04
-			('OAR1' , ctypes.c_uint32),  # I2C Own address register 1, Address offset: 0x08
-			('OAR2' , ctypes.c_uint32),  # I2C Own address register 2, Address offset: 0x0C
-			('DR'   , ctypes.c_uint32),  # I2C Data register,          Address offset: 0x10
-			('SR1'  , ctypes.c_uint32),  # I2C Status register 1,      Address offset: 0x14
-			('SR2'  , ctypes.c_uint32),  # I2C Status register 2,      Address offset: 0x18
-			('CCR'  , ctypes.c_uint32),  # I2C Clock control register, Address offset: 0x1C
-			('TRISE', ctypes.c_uint32),  # I2C TRISE register,         Address offset: 0x20
-			('FLTR' , ctypes.c_uint32),  # I2C FLTR register,          Address offset: 0x24
-		]
-
-	def __init__(self, ql, label, ev_intn=None, er_intn=None):
-		super().__init__(ql, label, 2)		
-
-		self.history = AccessSequence()
-
-		self.ev_intn = ev_intn # event interrupt
-		self.er_intn = er_intn # error interrupt		
-		
-		self.reset()
-
-	def reset(self):
-		self.instance = self.struct(
-			TRISE = 0x0002
-		)
-
-	@QlPeripheral.recorder()
-	@QlPeripheral.monitor()
-	def read(self, offset: int, size: int) -> int:	
-		buf = ctypes.create_string_buffer(size)
-		ctypes.memmove(buf, ctypes.addressof(self.instance) + offset, size)
-
-		if self.history.match([
-			Access(Action.READ, self.struct.SR1.offset),
-			Access(Action.READ, self.struct.SR2.offset)
-		]):				
-			self.instance.SR1 &= ~I2C_SR1.ADDR
-
-		return int.from_bytes(buf.raw, byteorder='little')
-
-	@QlPeripheral.recorder()
-	@QlPeripheral.monitor()
-	def write(self, offset: int, size: int, value: int):
-		if offset in [self.struct.SR1.offset, self.struct.SR2.offset]:
-			return		
-
-		if offset == self.struct.CR1.offset:
-			self.instance.CR1 = value & I2C_CR1.RW_MASK
-
-			if value & I2C_CR1.START:
-				self.generate_start()
-
-			if value & I2C_CR1.STOP:
-				self.generate_stop()
-
-			return
-
-		if offset == self.struct.DR.offset:
-			self.instance.DR = value & I2C_DR.DR
-			self.instance.SR1 &= ~I2C_SR1.TXE
-
-			if self.is_master_mode():
-				if self.is_7bit_mode():	
-					if self.instance.SR2 & I2C_SR2.TRA:
-						self.send_data()
-
-					else:
-						self.send_address()					
-
-				# TODO 10-bit mode
-
-			return
-
-		data = (value).to_bytes(size, 'little')
-		ctypes.memmove(ctypes.addressof(self.instance) + offset, data, size)
-
-	## I2C Control register 2 (I2C_CR2)
-	def send_event_interrupt(self):
-		"""
-			ITBUFEN: Buffer interrupt enable
-				0: TxE = 1 or RxNE = 1 does not generate any interrupt.
-				1: TxE = 1 or RxNE = 1 generates Event Interrupt (whatever the state of DMAEN)
-
-			ITEVTEN: Event interrupt enable
-				0: Event interrupt disabled
-				1: Event interrupt enabled
-				This interrupt is generated when:
-				- SB = 1 (Master)
-				- ADDR = 1 (Master/Slave)
-				- ADD10= 1 (Master)
-				- STOPF = 1 (Slave)
-				- BTF = 1 with no TxE or RxNE event
-				- TxE event to 1 if ITBUFEN = 1
-				- RxNE event to 1if ITBUFEN = 1
-		"""
-		if self.ev_intn is None:
-			return
-		
-		if not self.instance.CR2 & I2C_CR2.ITEVTEN:
-			return
-
-		BUF_IT = I2C_SR1.TXE|I2C_SR1.RXNE
-		SLAVE_IT = I2C_SR1.STOPF|I2C_SR1.ADDR|I2C_SR1.BTF
-		MASTER_IT = I2C_SR1.SB|I2C_SR1.ADDR|I2C_SR1.ADD10|I2C_SR1.BTF
-
-		if  (self.instance.CR2 & I2C_CR2.ITBUFEN and self.instance.SR1 & BUF_IT) or \
-			(self.is_slave_mode()           and self.instance.SR1 & SLAVE_IT) or \
-			(self.is_master_mode()          and self.instance.SR1 & MASTER_IT):
-			self.ql.hw.nvic.set_pending(self.ev_intn)
-
-	## I2C Status register 1 (I2C_SR1)
-	def generate_start(self):
-		"""
-		  	SB: Start bit (Master mode)
-			0: No Start condition
-			1: Start condition generated.
-		- Set when a Start condition generated.
-		- Cleared by software by reading the SR1 register followed by writing the DR register, or by hardware when PE=0
-		"""
-
-		# TODO: generate a start condition
-		self.fetch_device_address()
-		self.instance.SR1 |= I2C_SR1.SB
-		self.instance.CR1 &= ~I2C_CR1.START
-
-		self.set_master_mode()
-
-	def generate_stop(self):
-		# TODO: generate a stop condition
-		self.instance.CR1 &= ~I2C_CR1.STOP
-		
-		self.instance.SR1 |= I2C_SR1.STOPF
-		self.instance.SR1 &= ~I2C_SR1.ADDR
-		
-		self.set_slave_mode()
-		self.instance.SR2 &= ~I2C_SR2.TRA
-	
-	def send_address(self):
-		if self.instance.DR == self.instance.OAR1 >> 1:
-			
-			# TODO: send ACK
-			self.instance.SR1 &= ~I2C_SR1.SB
-			self.instance.SR1 |= I2C_SR1.ADDR | I2C_SR1.TXE | I2C_SR1.AF
-			self.instance.SR2 |= I2C_SR2.TRA
-
-	def send_data(self):
-		self.instance.SR1 |= I2C_SR1.BTF | I2C_SR1.TXE
-
-		self.send_to_user(self.instance.DR)
-
-	## I2C Status register 2 (I2C_SR2)
-	def is_master_mode(self):
-		"""
-		  	I2C Status register 2 (I2C_SR2) MSL bit
-			0: Slave Mode
-			1: Master Mode
-		"""
-		return self.instance.SR2 & I2C_SR2.MSL
-
-	def is_slave_mode(self):
-		return not self.is_master_mode()
-
-	def set_master_mode(self):
-		"""
-			I2C Status register 2 (I2C_SR2) MSL bit
-			- Set by hardware as soon as the interface is in Master mode (SB=1)			
-		"""
-		self.instance.SR2 |= I2C_SR2.MSL
-	
-	def set_slave_mode(self):		
-		"""
-			I2C Status register 2 (I2C_SR2) MSL bit
-			- Cleared by hardware after detecting a Stop condition on the bus 
-			  or a loss of arbitration (ARLO=1), or by hardware when PE=0.
-		"""
-		self.instance.SR2 &= ~I2C_SR2.MSL
-
-	## I2C Own address register 1 (I2C_OAR1)
-	def is_7bit_mode(self):
-		return self.instance.OAR2 & I2C_OAR2.ENDUAL or not self.instance.OAR1 & I2C_OAR1.ADDMODE
-
-	def fetch_device_address(self):
-		# dual addressing mode
-		if self.instance.OAR2 & I2C_OAR2.ENDUAL:
-			self.instance.OAR1 = self.device_list[0].address << 1
-			self.instance.OAR2 = I2C_OAR2.ENDUAL | (self.device_list[1].address << 1)
-
-		# single device, 10-bit slave address
-		elif self.instance.OAR1 & I2C_OAR1.ADDMODE: 
-			self.instance.OAR1 = I2C_OAR1.ADDMODE | self.device_list[0].address
-		
-		# single device, 7-bit slave address
-		else:
-			self.instance.OAR1 = self.device_list[0].address << 1
-
-	@QlConnectivityPeripheral.device_handler
-	def step(self):
-		self.send_event_interrupt()
+    class Type(ctypes.Structure):
+        """ the structure is available in :
+            stm32f423xx.h
+            stm32f469xx.h
+            stm32f427xx.h
+            stm32f479xx.h
+            stm32f413xx.h
+            stm32f429xx.h
+            stm32f439xx.h
+            stm32f412cx.h
+            stm32f412rx.h
+            stm32f410tx.h
+            stm32f410cx.h
+            stm32f412zx.h
+            stm32f446xx.h
+            stm32f401xc.h
+            stm32f437xx.h
+            stm32f401xe.h
+            stm32f412vx.h
+            stm32f410rx.h
+            stm32f411xe.h 
+        """
+
+        _fields_ = [
+            ('CR1'  , ctypes.c_uint32),  # I2C Control register 1,     Address offset: 0x00
+            ('CR2'  , ctypes.c_uint32),  # I2C Control register 2,     Address offset: 0x04
+            ('OAR1' , ctypes.c_uint32),  # I2C Own address register 1, Address offset: 0x08
+            ('OAR2' , ctypes.c_uint32),  # I2C Own address register 2, Address offset: 0x0C
+            ('DR'   , ctypes.c_uint32),  # I2C Data register,          Address offset: 0x10
+            ('SR1'  , ctypes.c_uint32),  # I2C Status register 1,      Address offset: 0x14
+            ('SR2'  , ctypes.c_uint32),  # I2C Status register 2,      Address offset: 0x18
+            ('CCR'  , ctypes.c_uint32),  # I2C Clock control register, Address offset: 0x1C
+            ('TRISE', ctypes.c_uint32),  # I2C TRISE register,         Address offset: 0x20
+            ('FLTR' , ctypes.c_uint32),  # I2C FLTR register,          Address offset: 0x24
+        ]
+
+    def __init__(self, ql, label, ev_intn=None, er_intn=None):
+        super().__init__(ql, label, 2)        
+
+        self.history = AccessSequence()
+
+        self.ev_intn = ev_intn # event interrupt
+        self.er_intn = er_intn # error interrupt        
+        
+        self.reset()
+
+    def reset(self):
+        self.instance = self.struct(
+            TRISE = 0x0002
+        )
+
+    @QlPeripheral.recorder()
+    @QlPeripheral.monitor()
+    def read(self, offset: int, size: int) -> int:    
+        buf = ctypes.create_string_buffer(size)
+        ctypes.memmove(buf, ctypes.addressof(self.instance) + offset, size)
+
+        if self.history.match([
+            Access(Action.READ, self.struct.SR1.offset),
+            Access(Action.READ, self.struct.SR2.offset)
+        ]):                
+            self.instance.SR1 &= ~I2C_SR1.ADDR
+
+        return int.from_bytes(buf.raw, byteorder='little')
+
+    @QlPeripheral.recorder()
+    @QlPeripheral.monitor()
+    def write(self, offset: int, size: int, value: int):
+        if offset in [self.struct.SR1.offset, self.struct.SR2.offset]:
+            return        
+
+        if offset == self.struct.CR1.offset:
+            self.instance.CR1 = value & I2C_CR1.RW_MASK
+
+            if value & I2C_CR1.START:
+                self.generate_start()
+
+            if value & I2C_CR1.STOP:
+                self.generate_stop()
+
+            return
+
+        if offset == self.struct.DR.offset:
+            self.instance.DR = value & I2C_DR.DR
+            self.instance.SR1 &= ~I2C_SR1.TXE
+
+            if self.is_master_mode():
+                if self.is_7bit_mode():    
+                    if self.instance.SR2 & I2C_SR2.TRA:
+                        self.send_data()
+
+                    else:
+                        self.send_address()                    
+
+                # TODO 10-bit mode
+
+            return
+
+        data = (value).to_bytes(size, 'little')
+        ctypes.memmove(ctypes.addressof(self.instance) + offset, data, size)
+
+    ## I2C Control register 2 (I2C_CR2)
+    def send_event_interrupt(self):
+        """
+            ITBUFEN: Buffer interrupt enable
+                0: TxE = 1 or RxNE = 1 does not generate any interrupt.
+                1: TxE = 1 or RxNE = 1 generates Event Interrupt (whatever the state of DMAEN)
+
+            ITEVTEN: Event interrupt enable
+                0: Event interrupt disabled
+                1: Event interrupt enabled
+                This interrupt is generated when:
+                - SB = 1 (Master)
+                - ADDR = 1 (Master/Slave)
+                - ADD10= 1 (Master)
+                - STOPF = 1 (Slave)
+                - BTF = 1 with no TxE or RxNE event
+                - TxE event to 1 if ITBUFEN = 1
+                - RxNE event to 1if ITBUFEN = 1
+        """
+        if self.ev_intn is None:
+            return
+        
+        if not self.instance.CR2 & I2C_CR2.ITEVTEN:
+            return
+
+        BUF_IT = I2C_SR1.TXE|I2C_SR1.RXNE
+        SLAVE_IT = I2C_SR1.STOPF|I2C_SR1.ADDR|I2C_SR1.BTF
+        MASTER_IT = I2C_SR1.SB|I2C_SR1.ADDR|I2C_SR1.ADD10|I2C_SR1.BTF
+
+        if  (self.instance.CR2 & I2C_CR2.ITBUFEN and self.instance.SR1 & BUF_IT) or \
+            (self.is_slave_mode()           and self.instance.SR1 & SLAVE_IT) or \
+            (self.is_master_mode()          and self.instance.SR1 & MASTER_IT):
+            self.ql.hw.nvic.set_pending(self.ev_intn)
+
+    ## I2C Status register 1 (I2C_SR1)
+    def generate_start(self):
+        """
+              SB: Start bit (Master mode)
+            0: No Start condition
+            1: Start condition generated.
+        - Set when a Start condition generated.
+        - Cleared by software by reading the SR1 register followed by writing the DR register, or by hardware when PE=0
+        """
+
+        # TODO: generate a start condition
+        self.fetch_device_address()
+        self.instance.SR1 |= I2C_SR1.SB
+        self.instance.CR1 &= ~I2C_CR1.START
+
+        self.set_master_mode()
+
+    def generate_stop(self):
+        # TODO: generate a stop condition
+        self.instance.CR1 &= ~I2C_CR1.STOP
+        
+        self.instance.SR1 |= I2C_SR1.STOPF
+        self.instance.SR1 &= ~I2C_SR1.ADDR
+        
+        self.set_slave_mode()
+        self.instance.SR2 &= ~I2C_SR2.TRA
+    
+    def send_address(self):
+        if self.instance.DR == self.instance.OAR1 >> 1:
+            
+            # TODO: send ACK
+            self.instance.SR1 &= ~I2C_SR1.SB
+            self.instance.SR1 |= I2C_SR1.ADDR | I2C_SR1.TXE | I2C_SR1.AF
+            self.instance.SR2 |= I2C_SR2.TRA
+
+    def send_data(self):
+        self.instance.SR1 |= I2C_SR1.BTF | I2C_SR1.TXE
+
+        self.send_to_user(self.instance.DR)
+
+    ## I2C Status register 2 (I2C_SR2)
+    def is_master_mode(self):
+        """
+              I2C Status register 2 (I2C_SR2) MSL bit
+            0: Slave Mode
+            1: Master Mode
+        """
+        return self.instance.SR2 & I2C_SR2.MSL
+
+    def is_slave_mode(self):
+        return not self.is_master_mode()
+
+    def set_master_mode(self):
+        """
+            I2C Status register 2 (I2C_SR2) MSL bit
+            - Set by hardware as soon as the interface is in Master mode (SB=1)            
+        """
+        self.instance.SR2 |= I2C_SR2.MSL
+    
+    def set_slave_mode(self):        
+        """
+            I2C Status register 2 (I2C_SR2) MSL bit
+            - Cleared by hardware after detecting a Stop condition on the bus 
+              or a loss of arbitration (ARLO=1), or by hardware when PE=0.
+        """
+        self.instance.SR2 &= ~I2C_SR2.MSL
+
+    ## I2C Own address register 1 (I2C_OAR1)
+    def is_7bit_mode(self):
+        return self.instance.OAR2 & I2C_OAR2.ENDUAL or not self.instance.OAR1 & I2C_OAR1.ADDMODE
+
+    def fetch_device_address(self):
+        # dual addressing mode
+        if self.instance.OAR2 & I2C_OAR2.ENDUAL:
+            self.instance.OAR1 = self.device_list[0].address << 1
+            self.instance.OAR2 = I2C_OAR2.ENDUAL | (self.device_list[1].address << 1)
+
+        # single device, 10-bit slave address
+        elif self.instance.OAR1 & I2C_OAR1.ADDMODE: 
+            self.instance.OAR1 = I2C_OAR1.ADDMODE | self.device_list[0].address
+        
+        # single device, 7-bit slave address
+        else:
+            self.instance.OAR1 = self.device_list[0].address << 1
+
+    @QlConnectivityPeripheral.device_handler
+    def step(self):
+        self.send_event_interrupt()
```

### Comparing `qiling-1.4.5/qiling/hw/intc/cm_nvic.py` & `qiling-1.4.6/qiling/hw/intc/cm_nvic.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/hw/intc/gd32vf1xx_eclic.py` & `qiling-1.4.6/qiling/hw/intc/gd32vf1xx_eclic.py`

 * *Files 0% similar despite different names*

```diff
@@ -721,15 +721,15 @@
             CLICINTCTL_83  =  0x00000000,
             CLICINTCTL_84  =  0x00000000,
             CLICINTCTL_85  =  0x00000000,
             CLICINTCTL_86  =  0x00000000,
         )
 
     @QlPeripheral.monitor()
-    def read(self, offset: int, size: int) -> int:		
+    def read(self, offset: int, size: int) -> int:        
         buf = ctypes.create_string_buffer(size)
         ctypes.memmove(buf, ctypes.addressof(self.instance) + offset, size)
         return int.from_bytes(buf.raw, byteorder='little')
     
     @QlPeripheral.monitor()
     def write(self, offset: int, size: int, value: int):
         data = (value).to_bytes(size, 'little')
```

### Comparing `qiling-1.4.5/qiling/hw/intc/stm32f1xx_exti.py` & `qiling-1.4.6/qiling/hw/intc/stm32f1xx_exti.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
             exti0_intn    , exti1_intn    , exti2_intn    , exti3_intn,
             exti4_intn    , exti9_5_intn  , exti9_5_intn  , exti9_5_intn,
             exti9_5_intn  , exti9_5_intn  , exti15_10_intn, exti15_10_intn,
             exti15_10_intn, exti15_10_intn, exti15_10_intn, exti15_10_intn
         ]
     
     @QlPeripheral.monitor()
-    def read(self, offset: int, size: int) -> int:		
+    def read(self, offset: int, size: int) -> int:        
         buf = ctypes.create_string_buffer(size)
         ctypes.memmove(buf, ctypes.addressof(self.instance) + offset, size)
         return int.from_bytes(buf.raw, byteorder='little')
 
     @QlPeripheral.monitor()
     def write(self, offset: int, size: int, value: int):
         if offset == self.struct.SWIER.offset:
```

### Comparing `qiling-1.4.5/qiling/hw/intc/stm32f4xx_exti.py` & `qiling-1.4.6/qiling/hw/intc/stm32f4xx_exti.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,40 +6,40 @@
 import ctypes
 from qiling.hw.peripheral import QlPeripheral
 
 
 class STM32F4xxExti(QlPeripheral):
     class Type(ctypes.Structure):
         """ the structure available in :
-			stm32f413xx.h
-			stm32f407xx.h
-			stm32f469xx.h
-			stm32f446xx.h
-			stm32f427xx.h
-			stm32f401xc.h
-			stm32f415xx.h
-			stm32f412cx.h
-			stm32f410rx.h
-			stm32f410tx.h
-			stm32f439xx.h
-			stm32f412vx.h
-			stm32f417xx.h
-			stm32f479xx.h
-			stm32f429xx.h
-			stm32f412rx.h
-			stm32f423xx.h
-			stm32f437xx.h
-			stm32f412zx.h
-			stm32f401xe.h
-			stm32f410cx.h
-			stm32f405xx.h
-			stm32f411xe.h 
-		"""
+            stm32f413xx.h
+            stm32f407xx.h
+            stm32f469xx.h
+            stm32f446xx.h
+            stm32f427xx.h
+            stm32f401xc.h
+            stm32f415xx.h
+            stm32f412cx.h
+            stm32f410rx.h
+            stm32f410tx.h
+            stm32f439xx.h
+            stm32f412vx.h
+            stm32f417xx.h
+            stm32f479xx.h
+            stm32f429xx.h
+            stm32f412rx.h
+            stm32f423xx.h
+            stm32f437xx.h
+            stm32f412zx.h
+            stm32f401xe.h
+            stm32f410cx.h
+            stm32f405xx.h
+            stm32f411xe.h 
+        """
 
         _fields_ = [
-			('IMR'  , ctypes.c_uint32),  # EXTI Interrupt mask register,            Address offset: 0x00
-			('EMR'  , ctypes.c_uint32),  # EXTI Event mask register,                Address offset: 0x04
-			('RTSR' , ctypes.c_uint32),  # EXTI Rising trigger selection register,  Address offset: 0x08
-			('FTSR' , ctypes.c_uint32),  # EXTI Falling trigger selection register, Address offset: 0x0C
-			('SWIER', ctypes.c_uint32),  # EXTI Software interrupt event register,  Address offset: 0x10
-			('PR'   , ctypes.c_uint32),  # EXTI Pending register,                   Address offset: 0x14
+            ('IMR'  , ctypes.c_uint32),  # EXTI Interrupt mask register,            Address offset: 0x00
+            ('EMR'  , ctypes.c_uint32),  # EXTI Event mask register,                Address offset: 0x04
+            ('RTSR' , ctypes.c_uint32),  # EXTI Rising trigger selection register,  Address offset: 0x08
+            ('FTSR' , ctypes.c_uint32),  # EXTI Falling trigger selection register, Address offset: 0x0C
+            ('SWIER', ctypes.c_uint32),  # EXTI Software interrupt event register,  Address offset: 0x10
+            ('PR'   , ctypes.c_uint32),  # EXTI Pending register,                   Address offset: 0x14
         ]
```

### Comparing `qiling-1.4.5/qiling/hw/math/gd32vf1xx_crc.py` & `qiling-1.4.6/qiling/hw/math/gd32vf1xx_crc.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/hw/mem/cm_bitband.py` & `qiling-1.4.6/qiling/hw/mem/cm_bitband.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/hw/mem/kinetis_bme.py` & `qiling-1.4.6/qiling/hw/mem/kinetis_bme.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/hw/mem/remap.py` & `qiling-1.4.6/qiling/hw/mem/remap.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/hw/misc/__init__.py` & `qiling-1.4.6/qiling/hw/misc/__init__.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/hw/misc/cm3_scb.py` & `qiling-1.4.6/qiling/hw/misc/cm3_scb.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/hw/misc/cm4_scb.py` & `qiling-1.4.6/qiling/hw/misc/cm4_scb.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/hw/misc/cm_scb.py` & `qiling-1.4.6/qiling/hw/misc/cm_scb.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/hw/misc/gd32vf1xx_rcu.py` & `qiling-1.4.6/qiling/hw/misc/gd32vf1xx_rcu.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
             CFG1    =  0x00000000,
             DSV     =  0x00000000,
         )
 
         self.intn = intn
 
     @QlPeripheral.monitor()
-    def read(self, offset: int, size: int) -> int:		
+    def read(self, offset: int, size: int) -> int:        
         buf = ctypes.create_string_buffer(size)
         ctypes.memmove(buf, ctypes.addressof(self.instance) + offset, size)
         return int.from_bytes(buf.raw, byteorder='little')
     
     @QlPeripheral.monitor()
     def write(self, offset: int, size: int, value: int):
         data = (value).to_bytes(size, 'little')
```

### Comparing `qiling-1.4.5/qiling/hw/misc/mk64f12_mcg.py` & `qiling-1.4.6/qiling/hw/misc/mk64f12_mcg.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/hw/misc/mk64f12_sim.py` & `qiling-1.4.6/qiling/hw/misc/mk64f12_sim.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/hw/misc/mk64f12_smc.py` & `qiling-1.4.6/qiling/hw/misc/mk64f12_smc.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/hw/misc/mk64f12_wdog.py` & `qiling-1.4.6/qiling/hw/misc/mk64f12_wdog.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/hw/misc/sam3xa_wdt.py` & `qiling-1.4.6/qiling/hw/misc/sam3xa_wdt.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/hw/misc/stm32f1xx_rcc.py` & `qiling-1.4.6/qiling/hw/timer/cm_systick.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,82 +1,66 @@
 #!/usr/bin/env python3
 # 
 # Cross Platform and Multi Architecture Advanced Binary Emulation Framework
 #
 
 import ctypes
+from qiling.arch.cortex_m_const import IRQ
 from qiling.hw.peripheral import QlPeripheral
-from qiling.hw.const.stm32fxxx_rcc import RCC_CR, RCC_CFGR, RCC_CSR
+from qiling.hw.timer.timer import QlTimerPeripheral
+from qiling.hw.const.cm4_systick import SYSTICK_CTRL
 
 
-class STM32F1xxRcc(QlPeripheral):
+class CortexMSysTick(QlTimerPeripheral):
     class Type(ctypes.Structure):
-        """ the structure is available in :
-                stm32f101xb
-                stm32f101xe
-                stm32f101xg
-                stm32f102xb
-                stm32f103xb
-                stm32f103xe
-                stm32f103xg
-        """
-
         _fields_ = [
-            ("CR"      , ctypes.c_uint32),
-            ("CFGR"    , ctypes.c_uint32),
-            ("CIR"     , ctypes.c_uint32),
-            ("APB2RSTR", ctypes.c_uint32),
-            ("APB1RSTR", ctypes.c_uint32),
-            ("AHBENR"  , ctypes.c_uint32),
-            ("APB2ENR" , ctypes.c_uint32),
-            ("APB1ENR" , ctypes.c_uint32),
-            ("BDCR"    , ctypes.c_uint32),
-            ("CSR"     , ctypes.c_uint32),
+            ('CTRL' , ctypes.c_uint32),
+            ('LOAD' , ctypes.c_int32),
+            ('VAL'  , ctypes.c_int32),
+            ('CALIB', ctypes.c_uint32),
         ]
-    
-    def __init__(self, ql, label, intn=None):
+
+    def __init__(self, ql, label):
         super().__init__(ql, label)
 
         self.instance = self.struct(
-            CR     = 0x00000083,
-            AHBENR = 0x00000014,
-            CSR    = 0x0C000000,
+            CALIB = 0xC0000000
         )
 
-        self.rdyon = {
-			'CR': [
-				(RCC_CR.HSIRDY   , RCC_CR.HSION   ),
-				(RCC_CR.HSERDY   , RCC_CR.HSEON   ),
-				(RCC_CR.PLLRDY   , RCC_CR.PLLON   ),
-				(RCC_CR.PLLI2SRDY, RCC_CR.PLLI2SON),
-			],
-			'CFGR': [
-				(RCC_CFGR.SWS_0, RCC_CFGR.SW_0),
-				(RCC_CFGR.SWS_1, RCC_CFGR.SW_1),
-			],
-			'CSR': [
-				(RCC_CSR.LSIRDY, RCC_CSR.LSION)
-			]
-		}
+    def step(self):
+        if not self.instance.CTRL & SYSTICK_CTRL.ENABLE:
+            return
 
-        self.intn = intn
+        if self.instance.VAL <= 0:
+            self.instance.CTRL |= SYSTICK_CTRL.COUNTFLAG
+            self.instance.VAL = self.instance.LOAD
+            
+        else:
+            self.instance.VAL -= self.ratio
+
+            if self.instance.VAL <= 0:                
+                if self.instance.CTRL & SYSTICK_CTRL.TICKINT:
+                    self.ql.hw.nvic.set_pending(IRQ.SYSTICK)
 
     @QlPeripheral.monitor()
-    def read(self, offset: int, size: int) -> int:		
+    def read(self, offset: int, size: int) -> int:
         buf = ctypes.create_string_buffer(size)
         ctypes.memmove(buf, ctypes.addressof(self.instance) + offset, size)
+
+        if offset == self.struct.CTRL.offset:
+            self.instance.CTRL &= ~SYSTICK_CTRL.COUNTFLAG        
         return int.from_bytes(buf.raw, byteorder='little')
 
     @QlPeripheral.monitor()
     def write(self, offset: int, size: int, value: int):
-        data = (value).to_bytes(size, 'little')
-        ctypes.memmove(ctypes.addressof(self.instance) + offset, data, size)
+        # ignore the reserved bit
+        if offset == self.struct.CTRL.offset:
+            value &= SYSTICK_CTRL.MASK
+        else:
+            value &= 0xffffff # only low-24 bit available
+
+        # restart the timer
+        if offset == self.struct.LOAD.offset:            
+            self.instance.VAL = value
 
-    def step(self):
-        for reg, rdyon in self.rdyon.items():
-            value = getattr(self.instance, reg)
-            for rdy, on in rdyon:
-                if value & on:
-                    value |= rdy
-                else:
-                    value &= ~rdy
-            setattr(self.instance, reg, value)
+        data = (value).to_bytes(size, 'little')
+        ctypes.memmove(ctypes.addressof(self.instance) + offset, data, size)
```

### Comparing `qiling-1.4.5/qiling/hw/misc/stm32f4xx_dbg.py` & `qiling-1.4.6/qiling/hw/misc/stm32f4xx_dbg.py`

 * *Files 8% similar despite different names*

```diff
@@ -48,15 +48,15 @@
         super().__init__(ql, label)
 
         self.instance = self.struct(
             IDCODE = dev_id,
         )
 
     @QlPeripheral.monitor()
-    def read(self, offset: int, size: int) -> int:		
+    def read(self, offset: int, size: int) -> int:        
         buf = ctypes.create_string_buffer(size)
         ctypes.memmove(buf, ctypes.addressof(self.instance) + offset, size)
         return int.from_bytes(buf.raw, byteorder='little')
     
     @QlPeripheral.monitor()
     def write(self, offset: int, size: int, value: int):
         data = (value).to_bytes(size, 'little')
```

### Comparing `qiling-1.4.5/qiling/hw/misc/stm32f4xx_rcc.py` & `qiling-1.4.6/qiling/hw/misc/stm32f4xx_rcc.py`

 * *Files 27% similar despite different names*

```diff
@@ -5,106 +5,106 @@
 
 import ctypes
 from qiling.hw.peripheral import QlPeripheral
 from qiling.hw.const.stm32fxxx_rcc import RCC_CR, RCC_CFGR, RCC_CSR
 
 
 class STM32F4xxRcc(QlPeripheral):
-	class Type(ctypes.Structure):
-		""" the structure available in :
-			stm32f401xc.h
-			stm32f401xe.h
-			stm32f411xe.h 
-		"""
-
-		_fields_ = [
-			('CR'        , ctypes.c_uint32),      # RCC clock control register,                                  Address offset: 0x00
-			('PLLCFGR'   , ctypes.c_uint32),      # RCC PLL configuration register,                              Address offset: 0x04
-			('CFGR'      , ctypes.c_uint32),      # RCC clock configuration register,                            Address offset: 0x08
-			('CIR'       , ctypes.c_uint32),      # RCC clock interrupt register,                                Address offset: 0x0C
-			('AHB1RSTR'  , ctypes.c_uint32),      # RCC AHB1 peripheral reset register,                          Address offset: 0x10
-			('AHB2RSTR'  , ctypes.c_uint32),      # RCC AHB2 peripheral reset register,                          Address offset: 0x14
-			('AHB3RSTR'  , ctypes.c_uint32),      # RCC AHB3 peripheral reset register,                          Address offset: 0x18
-			('RESERVED0' , ctypes.c_uint32),      # Reserved, 0x1C
-			('APB1RSTR'  , ctypes.c_uint32),      # RCC APB1 peripheral reset register,                          Address offset: 0x20
-			('APB2RSTR'  , ctypes.c_uint32),      # RCC APB2 peripheral reset register,                          Address offset: 0x24
-			('RESERVED1' , ctypes.c_uint32 * 2),  # Reserved, 0x28-0x2C
-			('AHB1ENR'   , ctypes.c_uint32),      # RCC AHB1 peripheral clock register,                          Address offset: 0x30
-			('AHB2ENR'   , ctypes.c_uint32),      # RCC AHB2 peripheral clock register,                          Address offset: 0x34
-			('AHB3ENR'   , ctypes.c_uint32),      # RCC AHB3 peripheral clock register,                          Address offset: 0x38
-			('RESERVED2' , ctypes.c_uint32),      # Reserved, 0x3C
-			('APB1ENR'   , ctypes.c_uint32),      # RCC APB1 peripheral clock enable register,                   Address offset: 0x40
-			('APB2ENR'   , ctypes.c_uint32),      # RCC APB2 peripheral clock enable register,                   Address offset: 0x44
-			('RESERVED3' , ctypes.c_uint32 * 2),  # Reserved, 0x48-0x4C
-			('AHB1LPENR' , ctypes.c_uint32),      # RCC AHB1 peripheral clock enable in low power mode register, Address offset: 0x50
-			('AHB2LPENR' , ctypes.c_uint32),      # RCC AHB2 peripheral clock enable in low power mode register, Address offset: 0x54
-			('AHB3LPENR' , ctypes.c_uint32),      # RCC AHB3 peripheral clock enable in low power mode register, Address offset: 0x58
-			('RESERVED4' , ctypes.c_uint32),      # Reserved, 0x5C
-			('APB1LPENR' , ctypes.c_uint32),      # RCC APB1 peripheral clock enable in low power mode register, Address offset: 0x60
-			('APB2LPENR' , ctypes.c_uint32),      # RCC APB2 peripheral clock enable in low power mode register, Address offset: 0x64
-			('RESERVED5' , ctypes.c_uint32 * 2),  # Reserved, 0x68-0x6C
-			('BDCR'      , ctypes.c_uint32),      # RCC Backup domain control register,                          Address offset: 0x70
-			('CSR'       , ctypes.c_uint32),      # RCC clock control & status register,                         Address offset: 0x74
-			('RESERVED6' , ctypes.c_uint32 * 2),  # Reserved, 0x78-0x7C
-			('SSCGR'     , ctypes.c_uint32),      # RCC spread spectrum clock generation register,               Address offset: 0x80
-			('PLLI2SCFGR', ctypes.c_uint32),      # RCC PLLI2S configuration register,                           Address offset: 0x84
-			('RESERVED7' , ctypes.c_uint32),      # Reserved, 0x88
-			('DCKCFGR'   , ctypes.c_uint32),      # RCC Dedicated Clocks configuration register,                 Address offset: 0x8C
-		]
-
-	def __init__(self, ql, label, intn=None):
-		super().__init__(ql, label)
-
-		self.instance = self.struct(
-			CR         = 0x00000083,
-			PLLCFGR    = 0x24003010,
-			AHB1LPENR  = 0x0061900F,
-			AHB2LPENR  = 0x00000080,
-			APB1LPENR  = 0x10E2C80F,
-			APB2LPENR  = 0x00077930,
-			CSR        = 0x0E000000,
-			PLLI2SCFGR = 0x24003000,
-		)
-
-		self.rdyon = {
-			'CR': [
-				(RCC_CR.HSIRDY   , RCC_CR.HSION   ),
-				(RCC_CR.HSERDY   , RCC_CR.HSEON   ),
-				(RCC_CR.PLLRDY   , RCC_CR.PLLON   ),
-				(RCC_CR.PLLI2SRDY, RCC_CR.PLLI2SON),
-			],
-			'CFGR': [
-				(RCC_CFGR.SWS_0, RCC_CFGR.SW_0),
-				(RCC_CFGR.SWS_1, RCC_CFGR.SW_1),
-			],
-			'CSR': [
-				(RCC_CSR.LSIRDY, RCC_CSR.LSION)
-			]
-		}
-
-		self.intn = intn
-
-	@QlPeripheral.monitor()
-	def read(self, offset: int, size: int) -> int:		
-		buf = ctypes.create_string_buffer(size)
-		ctypes.memmove(buf, ctypes.addressof(self.instance) + offset, size)
-		return int.from_bytes(buf.raw, byteorder='little')
-
-	@QlPeripheral.monitor()
-	def write(self, offset: int, size: int, value: int):
-		if offset == self.struct.CR.offset:
-			value = (self.instance.CR & RCC_CR.RO_MASK) | (value & RCC_CR.RW_MASK)
-		elif offset == self.struct.CFGR.offset:
-			value = (self.instance.CFGR & RCC_CFGR.RO_MASK) | (value & RCC_CFGR.RW_MASK)
-
-		data = (value).to_bytes(size, 'little')
-		ctypes.memmove(ctypes.addressof(self.instance) + offset, data, size)
-
-	def step(self):
-		for reg, rdyon in self.rdyon.items():
-			value = getattr(self.instance, reg)
-			for rdy, on in rdyon:
-				if value & on:
-					value |= rdy
-				else:
-					value &= ~rdy
-			setattr(self.instance, reg, value)
+    class Type(ctypes.Structure):
+        """ the structure available in :
+            stm32f401xc.h
+            stm32f401xe.h
+            stm32f411xe.h 
+        """
+
+        _fields_ = [
+            ('CR'        , ctypes.c_uint32),      # RCC clock control register,                                  Address offset: 0x00
+            ('PLLCFGR'   , ctypes.c_uint32),      # RCC PLL configuration register,                              Address offset: 0x04
+            ('CFGR'      , ctypes.c_uint32),      # RCC clock configuration register,                            Address offset: 0x08
+            ('CIR'       , ctypes.c_uint32),      # RCC clock interrupt register,                                Address offset: 0x0C
+            ('AHB1RSTR'  , ctypes.c_uint32),      # RCC AHB1 peripheral reset register,                          Address offset: 0x10
+            ('AHB2RSTR'  , ctypes.c_uint32),      # RCC AHB2 peripheral reset register,                          Address offset: 0x14
+            ('AHB3RSTR'  , ctypes.c_uint32),      # RCC AHB3 peripheral reset register,                          Address offset: 0x18
+            ('RESERVED0' , ctypes.c_uint32),      # Reserved, 0x1C
+            ('APB1RSTR'  , ctypes.c_uint32),      # RCC APB1 peripheral reset register,                          Address offset: 0x20
+            ('APB2RSTR'  , ctypes.c_uint32),      # RCC APB2 peripheral reset register,                          Address offset: 0x24
+            ('RESERVED1' , ctypes.c_uint32 * 2),  # Reserved, 0x28-0x2C
+            ('AHB1ENR'   , ctypes.c_uint32),      # RCC AHB1 peripheral clock register,                          Address offset: 0x30
+            ('AHB2ENR'   , ctypes.c_uint32),      # RCC AHB2 peripheral clock register,                          Address offset: 0x34
+            ('AHB3ENR'   , ctypes.c_uint32),      # RCC AHB3 peripheral clock register,                          Address offset: 0x38
+            ('RESERVED2' , ctypes.c_uint32),      # Reserved, 0x3C
+            ('APB1ENR'   , ctypes.c_uint32),      # RCC APB1 peripheral clock enable register,                   Address offset: 0x40
+            ('APB2ENR'   , ctypes.c_uint32),      # RCC APB2 peripheral clock enable register,                   Address offset: 0x44
+            ('RESERVED3' , ctypes.c_uint32 * 2),  # Reserved, 0x48-0x4C
+            ('AHB1LPENR' , ctypes.c_uint32),      # RCC AHB1 peripheral clock enable in low power mode register, Address offset: 0x50
+            ('AHB2LPENR' , ctypes.c_uint32),      # RCC AHB2 peripheral clock enable in low power mode register, Address offset: 0x54
+            ('AHB3LPENR' , ctypes.c_uint32),      # RCC AHB3 peripheral clock enable in low power mode register, Address offset: 0x58
+            ('RESERVED4' , ctypes.c_uint32),      # Reserved, 0x5C
+            ('APB1LPENR' , ctypes.c_uint32),      # RCC APB1 peripheral clock enable in low power mode register, Address offset: 0x60
+            ('APB2LPENR' , ctypes.c_uint32),      # RCC APB2 peripheral clock enable in low power mode register, Address offset: 0x64
+            ('RESERVED5' , ctypes.c_uint32 * 2),  # Reserved, 0x68-0x6C
+            ('BDCR'      , ctypes.c_uint32),      # RCC Backup domain control register,                          Address offset: 0x70
+            ('CSR'       , ctypes.c_uint32),      # RCC clock control & status register,                         Address offset: 0x74
+            ('RESERVED6' , ctypes.c_uint32 * 2),  # Reserved, 0x78-0x7C
+            ('SSCGR'     , ctypes.c_uint32),      # RCC spread spectrum clock generation register,               Address offset: 0x80
+            ('PLLI2SCFGR', ctypes.c_uint32),      # RCC PLLI2S configuration register,                           Address offset: 0x84
+            ('RESERVED7' , ctypes.c_uint32),      # Reserved, 0x88
+            ('DCKCFGR'   , ctypes.c_uint32),      # RCC Dedicated Clocks configuration register,                 Address offset: 0x8C
+        ]
+
+    def __init__(self, ql, label, intn=None):
+        super().__init__(ql, label)
+
+        self.instance = self.struct(
+            CR         = 0x00000083,
+            PLLCFGR    = 0x24003010,
+            AHB1LPENR  = 0x0061900F,
+            AHB2LPENR  = 0x00000080,
+            APB1LPENR  = 0x10E2C80F,
+            APB2LPENR  = 0x00077930,
+            CSR        = 0x0E000000,
+            PLLI2SCFGR = 0x24003000,
+        )
+
+        self.rdyon = {
+            'CR': [
+                (RCC_CR.HSIRDY   , RCC_CR.HSION   ),
+                (RCC_CR.HSERDY   , RCC_CR.HSEON   ),
+                (RCC_CR.PLLRDY   , RCC_CR.PLLON   ),
+                (RCC_CR.PLLI2SRDY, RCC_CR.PLLI2SON),
+            ],
+            'CFGR': [
+                (RCC_CFGR.SWS_0, RCC_CFGR.SW_0),
+                (RCC_CFGR.SWS_1, RCC_CFGR.SW_1),
+            ],
+            'CSR': [
+                (RCC_CSR.LSIRDY, RCC_CSR.LSION)
+            ]
+        }
+
+        self.intn = intn
+
+    @QlPeripheral.monitor()
+    def read(self, offset: int, size: int) -> int:        
+        buf = ctypes.create_string_buffer(size)
+        ctypes.memmove(buf, ctypes.addressof(self.instance) + offset, size)
+        return int.from_bytes(buf.raw, byteorder='little')
+
+    @QlPeripheral.monitor()
+    def write(self, offset: int, size: int, value: int):
+        if offset == self.struct.CR.offset:
+            value = (self.instance.CR & RCC_CR.RO_MASK) | (value & RCC_CR.RW_MASK)
+        elif offset == self.struct.CFGR.offset:
+            value = (self.instance.CFGR & RCC_CFGR.RO_MASK) | (value & RCC_CFGR.RW_MASK)
+
+        data = (value).to_bytes(size, 'little')
+        ctypes.memmove(ctypes.addressof(self.instance) + offset, data, size)
+
+    def step(self):
+        for reg, rdyon in self.rdyon.items():
+            value = getattr(self.instance, reg)
+            for rdy, on in rdyon:
+                if value & on:
+                    value |= rdy
+                else:
+                    value &= ~rdy
+            setattr(self.instance, reg, value)
```

### Comparing `qiling-1.4.5/qiling/hw/misc/stm32f4xx_rcc_derive.py` & `qiling-1.4.6/qiling/hw/misc/stm32f4xx_rcc_derive.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,266 +6,266 @@
 import ctypes
 from .stm32f4xx_rcc import STM32F4xxRcc
 
 
 class STM32F4xxRccV1(STM32F4xxRcc):
     class Type(ctypes.Structure):
         """ the structure available in :
-			stm32f413xx.h
-			stm32f412vx.h
-			stm32f412rx.h
-			stm32f423xx.h
-			stm32f412zx.h 
-		"""
+            stm32f413xx.h
+            stm32f412vx.h
+            stm32f412rx.h
+            stm32f423xx.h
+            stm32f412zx.h 
+        """
 
         _fields_ = [
-			('CR'        , ctypes.c_uint32),      # RCC clock control register,                                  Address offset: 0x00
-			('PLLCFGR'   , ctypes.c_uint32),      # RCC PLL configuration register,                              Address offset: 0x04
-			('CFGR'      , ctypes.c_uint32),      # RCC clock configuration register,                            Address offset: 0x08
-			('CIR'       , ctypes.c_uint32),      # RCC clock interrupt register,                                Address offset: 0x0C
-			('AHB1RSTR'  , ctypes.c_uint32),      # RCC AHB1 peripheral reset register,                          Address offset: 0x10
-			('AHB2RSTR'  , ctypes.c_uint32),      # RCC AHB2 peripheral reset register,                          Address offset: 0x14
-			('AHB3RSTR'  , ctypes.c_uint32),      # RCC AHB3 peripheral reset register,                          Address offset: 0x18
-			('RESERVED0' , ctypes.c_uint32),      # Reserved, 0x1C
-			('APB1RSTR'  , ctypes.c_uint32),      # RCC APB1 peripheral reset register,                          Address offset: 0x20
-			('APB2RSTR'  , ctypes.c_uint32),      # RCC APB2 peripheral reset register,                          Address offset: 0x24
-			('RESERVED1' , ctypes.c_uint32 * 2),  # Reserved, 0x28-0x2C
-			('AHB1ENR'   , ctypes.c_uint32),      # RCC AHB1 peripheral clock register,                          Address offset: 0x30
-			('AHB2ENR'   , ctypes.c_uint32),      # RCC AHB2 peripheral clock register,                          Address offset: 0x34
-			('AHB3ENR'   , ctypes.c_uint32),      # RCC AHB3 peripheral clock register,                          Address offset: 0x38
-			('RESERVED2' , ctypes.c_uint32),      # Reserved, 0x3C
-			('APB1ENR'   , ctypes.c_uint32),      # RCC APB1 peripheral clock enable register,                   Address offset: 0x40
-			('APB2ENR'   , ctypes.c_uint32),      # RCC APB2 peripheral clock enable register,                   Address offset: 0x44
-			('RESERVED3' , ctypes.c_uint32 * 2),  # Reserved, 0x48-0x4C
-			('AHB1LPENR' , ctypes.c_uint32),      # RCC AHB1 peripheral clock enable in low power mode register, Address offset: 0x50
-			('AHB2LPENR' , ctypes.c_uint32),      # RCC AHB2 peripheral clock enable in low power mode register, Address offset: 0x54
-			('AHB3LPENR' , ctypes.c_uint32),      # RCC AHB3 peripheral clock enable in low power mode register, Address offset: 0x58
-			('RESERVED4' , ctypes.c_uint32),      # Reserved, 0x5C
-			('APB1LPENR' , ctypes.c_uint32),      # RCC APB1 peripheral clock enable in low power mode register, Address offset: 0x60
-			('APB2LPENR' , ctypes.c_uint32),      # RCC APB2 peripheral clock enable in low power mode register, Address offset: 0x64
-			('RESERVED5' , ctypes.c_uint32 * 2),  # Reserved, 0x68-0x6C
-			('BDCR'      , ctypes.c_uint32),      # RCC Backup domain control register,                          Address offset: 0x70
-			('CSR'       , ctypes.c_uint32),      # RCC clock control & status register,                         Address offset: 0x74
-			('RESERVED6' , ctypes.c_uint32 * 2),  # Reserved, 0x78-0x7C
-			('SSCGR'     , ctypes.c_uint32),      # RCC spread spectrum clock generation register,               Address offset: 0x80
-			('PLLI2SCFGR', ctypes.c_uint32),      # RCC PLLI2S configuration register,                           Address offset: 0x84
-			('RESERVED7' , ctypes.c_uint32),      # Reserved, 0x84
-			('DCKCFGR'   , ctypes.c_uint32),      # RCC Dedicated Clocks configuration register,                 Address offset: 0x8C
-			('CKGATENR'  , ctypes.c_uint32),      # RCC Clocks Gated ENable Register,                            Address offset: 0x90
-			('DCKCFGR2'  , ctypes.c_uint32),      # RCC Dedicated Clocks configuration register 2,               Address offset: 0x94
-		]
+            ('CR'        , ctypes.c_uint32),      # RCC clock control register,                                  Address offset: 0x00
+            ('PLLCFGR'   , ctypes.c_uint32),      # RCC PLL configuration register,                              Address offset: 0x04
+            ('CFGR'      , ctypes.c_uint32),      # RCC clock configuration register,                            Address offset: 0x08
+            ('CIR'       , ctypes.c_uint32),      # RCC clock interrupt register,                                Address offset: 0x0C
+            ('AHB1RSTR'  , ctypes.c_uint32),      # RCC AHB1 peripheral reset register,                          Address offset: 0x10
+            ('AHB2RSTR'  , ctypes.c_uint32),      # RCC AHB2 peripheral reset register,                          Address offset: 0x14
+            ('AHB3RSTR'  , ctypes.c_uint32),      # RCC AHB3 peripheral reset register,                          Address offset: 0x18
+            ('RESERVED0' , ctypes.c_uint32),      # Reserved, 0x1C
+            ('APB1RSTR'  , ctypes.c_uint32),      # RCC APB1 peripheral reset register,                          Address offset: 0x20
+            ('APB2RSTR'  , ctypes.c_uint32),      # RCC APB2 peripheral reset register,                          Address offset: 0x24
+            ('RESERVED1' , ctypes.c_uint32 * 2),  # Reserved, 0x28-0x2C
+            ('AHB1ENR'   , ctypes.c_uint32),      # RCC AHB1 peripheral clock register,                          Address offset: 0x30
+            ('AHB2ENR'   , ctypes.c_uint32),      # RCC AHB2 peripheral clock register,                          Address offset: 0x34
+            ('AHB3ENR'   , ctypes.c_uint32),      # RCC AHB3 peripheral clock register,                          Address offset: 0x38
+            ('RESERVED2' , ctypes.c_uint32),      # Reserved, 0x3C
+            ('APB1ENR'   , ctypes.c_uint32),      # RCC APB1 peripheral clock enable register,                   Address offset: 0x40
+            ('APB2ENR'   , ctypes.c_uint32),      # RCC APB2 peripheral clock enable register,                   Address offset: 0x44
+            ('RESERVED3' , ctypes.c_uint32 * 2),  # Reserved, 0x48-0x4C
+            ('AHB1LPENR' , ctypes.c_uint32),      # RCC AHB1 peripheral clock enable in low power mode register, Address offset: 0x50
+            ('AHB2LPENR' , ctypes.c_uint32),      # RCC AHB2 peripheral clock enable in low power mode register, Address offset: 0x54
+            ('AHB3LPENR' , ctypes.c_uint32),      # RCC AHB3 peripheral clock enable in low power mode register, Address offset: 0x58
+            ('RESERVED4' , ctypes.c_uint32),      # Reserved, 0x5C
+            ('APB1LPENR' , ctypes.c_uint32),      # RCC APB1 peripheral clock enable in low power mode register, Address offset: 0x60
+            ('APB2LPENR' , ctypes.c_uint32),      # RCC APB2 peripheral clock enable in low power mode register, Address offset: 0x64
+            ('RESERVED5' , ctypes.c_uint32 * 2),  # Reserved, 0x68-0x6C
+            ('BDCR'      , ctypes.c_uint32),      # RCC Backup domain control register,                          Address offset: 0x70
+            ('CSR'       , ctypes.c_uint32),      # RCC clock control & status register,                         Address offset: 0x74
+            ('RESERVED6' , ctypes.c_uint32 * 2),  # Reserved, 0x78-0x7C
+            ('SSCGR'     , ctypes.c_uint32),      # RCC spread spectrum clock generation register,               Address offset: 0x80
+            ('PLLI2SCFGR', ctypes.c_uint32),      # RCC PLLI2S configuration register,                           Address offset: 0x84
+            ('RESERVED7' , ctypes.c_uint32),      # Reserved, 0x84
+            ('DCKCFGR'   , ctypes.c_uint32),      # RCC Dedicated Clocks configuration register,                 Address offset: 0x8C
+            ('CKGATENR'  , ctypes.c_uint32),      # RCC Clocks Gated ENable Register,                            Address offset: 0x90
+            ('DCKCFGR2'  , ctypes.c_uint32),      # RCC Dedicated Clocks configuration register 2,               Address offset: 0x94
+        ]
 
 class STM32F4xxRccV2(STM32F4xxRcc):
     class Type(ctypes.Structure):
         """ the structure available in :
-			stm32f407xx.h
-			stm32f415xx.h
-			stm32f417xx.h
-			stm32f405xx.h 
-		"""
+            stm32f407xx.h
+            stm32f415xx.h
+            stm32f417xx.h
+            stm32f405xx.h 
+        """
 
         _fields_ = [
-			('CR'        , ctypes.c_uint32),      # RCC clock control register,                                  Address offset: 0x00
-			('PLLCFGR'   , ctypes.c_uint32),      # RCC PLL configuration register,                              Address offset: 0x04
-			('CFGR'      , ctypes.c_uint32),      # RCC clock configuration register,                            Address offset: 0x08
-			('CIR'       , ctypes.c_uint32),      # RCC clock interrupt register,                                Address offset: 0x0C
-			('AHB1RSTR'  , ctypes.c_uint32),      # RCC AHB1 peripheral reset register,                          Address offset: 0x10
-			('AHB2RSTR'  , ctypes.c_uint32),      # RCC AHB2 peripheral reset register,                          Address offset: 0x14
-			('AHB3RSTR'  , ctypes.c_uint32),      # RCC AHB3 peripheral reset register,                          Address offset: 0x18
-			('RESERVED0' , ctypes.c_uint32),      # Reserved, 0x1C
-			('APB1RSTR'  , ctypes.c_uint32),      # RCC APB1 peripheral reset register,                          Address offset: 0x20
-			('APB2RSTR'  , ctypes.c_uint32),      # RCC APB2 peripheral reset register,                          Address offset: 0x24
-			('RESERVED1' , ctypes.c_uint32 * 2),  # Reserved, 0x28-0x2C
-			('AHB1ENR'   , ctypes.c_uint32),      # RCC AHB1 peripheral clock register,                          Address offset: 0x30
-			('AHB2ENR'   , ctypes.c_uint32),      # RCC AHB2 peripheral clock register,                          Address offset: 0x34
-			('AHB3ENR'   , ctypes.c_uint32),      # RCC AHB3 peripheral clock register,                          Address offset: 0x38
-			('RESERVED2' , ctypes.c_uint32),      # Reserved, 0x3C
-			('APB1ENR'   , ctypes.c_uint32),      # RCC APB1 peripheral clock enable register,                   Address offset: 0x40
-			('APB2ENR'   , ctypes.c_uint32),      # RCC APB2 peripheral clock enable register,                   Address offset: 0x44
-			('RESERVED3' , ctypes.c_uint32 * 2),  # Reserved, 0x48-0x4C
-			('AHB1LPENR' , ctypes.c_uint32),      # RCC AHB1 peripheral clock enable in low power mode register, Address offset: 0x50
-			('AHB2LPENR' , ctypes.c_uint32),      # RCC AHB2 peripheral clock enable in low power mode register, Address offset: 0x54
-			('AHB3LPENR' , ctypes.c_uint32),      # RCC AHB3 peripheral clock enable in low power mode register, Address offset: 0x58
-			('RESERVED4' , ctypes.c_uint32),      # Reserved, 0x5C
-			('APB1LPENR' , ctypes.c_uint32),      # RCC APB1 peripheral clock enable in low power mode register, Address offset: 0x60
-			('APB2LPENR' , ctypes.c_uint32),      # RCC APB2 peripheral clock enable in low power mode register, Address offset: 0x64
-			('RESERVED5' , ctypes.c_uint32 * 2),  # Reserved, 0x68-0x6C
-			('BDCR'      , ctypes.c_uint32),      # RCC Backup domain control register,                          Address offset: 0x70
-			('CSR'       , ctypes.c_uint32),      # RCC clock control & status register,                         Address offset: 0x74
-			('RESERVED6' , ctypes.c_uint32 * 2),  # Reserved, 0x78-0x7C
-			('SSCGR'     , ctypes.c_uint32),      # RCC spread spectrum clock generation register,               Address offset: 0x80
-			('PLLI2SCFGR', ctypes.c_uint32),      # RCC PLLI2S configuration register,                           Address offset: 0x84
-		]
+            ('CR'        , ctypes.c_uint32),      # RCC clock control register,                                  Address offset: 0x00
+            ('PLLCFGR'   , ctypes.c_uint32),      # RCC PLL configuration register,                              Address offset: 0x04
+            ('CFGR'      , ctypes.c_uint32),      # RCC clock configuration register,                            Address offset: 0x08
+            ('CIR'       , ctypes.c_uint32),      # RCC clock interrupt register,                                Address offset: 0x0C
+            ('AHB1RSTR'  , ctypes.c_uint32),      # RCC AHB1 peripheral reset register,                          Address offset: 0x10
+            ('AHB2RSTR'  , ctypes.c_uint32),      # RCC AHB2 peripheral reset register,                          Address offset: 0x14
+            ('AHB3RSTR'  , ctypes.c_uint32),      # RCC AHB3 peripheral reset register,                          Address offset: 0x18
+            ('RESERVED0' , ctypes.c_uint32),      # Reserved, 0x1C
+            ('APB1RSTR'  , ctypes.c_uint32),      # RCC APB1 peripheral reset register,                          Address offset: 0x20
+            ('APB2RSTR'  , ctypes.c_uint32),      # RCC APB2 peripheral reset register,                          Address offset: 0x24
+            ('RESERVED1' , ctypes.c_uint32 * 2),  # Reserved, 0x28-0x2C
+            ('AHB1ENR'   , ctypes.c_uint32),      # RCC AHB1 peripheral clock register,                          Address offset: 0x30
+            ('AHB2ENR'   , ctypes.c_uint32),      # RCC AHB2 peripheral clock register,                          Address offset: 0x34
+            ('AHB3ENR'   , ctypes.c_uint32),      # RCC AHB3 peripheral clock register,                          Address offset: 0x38
+            ('RESERVED2' , ctypes.c_uint32),      # Reserved, 0x3C
+            ('APB1ENR'   , ctypes.c_uint32),      # RCC APB1 peripheral clock enable register,                   Address offset: 0x40
+            ('APB2ENR'   , ctypes.c_uint32),      # RCC APB2 peripheral clock enable register,                   Address offset: 0x44
+            ('RESERVED3' , ctypes.c_uint32 * 2),  # Reserved, 0x48-0x4C
+            ('AHB1LPENR' , ctypes.c_uint32),      # RCC AHB1 peripheral clock enable in low power mode register, Address offset: 0x50
+            ('AHB2LPENR' , ctypes.c_uint32),      # RCC AHB2 peripheral clock enable in low power mode register, Address offset: 0x54
+            ('AHB3LPENR' , ctypes.c_uint32),      # RCC AHB3 peripheral clock enable in low power mode register, Address offset: 0x58
+            ('RESERVED4' , ctypes.c_uint32),      # Reserved, 0x5C
+            ('APB1LPENR' , ctypes.c_uint32),      # RCC APB1 peripheral clock enable in low power mode register, Address offset: 0x60
+            ('APB2LPENR' , ctypes.c_uint32),      # RCC APB2 peripheral clock enable in low power mode register, Address offset: 0x64
+            ('RESERVED5' , ctypes.c_uint32 * 2),  # Reserved, 0x68-0x6C
+            ('BDCR'      , ctypes.c_uint32),      # RCC Backup domain control register,                          Address offset: 0x70
+            ('CSR'       , ctypes.c_uint32),      # RCC clock control & status register,                         Address offset: 0x74
+            ('RESERVED6' , ctypes.c_uint32 * 2),  # Reserved, 0x78-0x7C
+            ('SSCGR'     , ctypes.c_uint32),      # RCC spread spectrum clock generation register,               Address offset: 0x80
+            ('PLLI2SCFGR', ctypes.c_uint32),      # RCC PLLI2S configuration register,                           Address offset: 0x84
+        ]
 
 class STM32F4xxRccV3(STM32F4xxRcc):
     class Type(ctypes.Structure):
         """ the structure available in :
-			stm32f469xx.h
-			stm32f427xx.h
-			stm32f439xx.h
-			stm32f479xx.h
-			stm32f429xx.h
-			stm32f437xx.h 
-		"""
+            stm32f469xx.h
+            stm32f427xx.h
+            stm32f439xx.h
+            stm32f479xx.h
+            stm32f429xx.h
+            stm32f437xx.h 
+        """
 
         _fields_ = [
-			('CR'        , ctypes.c_uint32),      # RCC clock control register,                                  Address offset: 0x00
-			('PLLCFGR'   , ctypes.c_uint32),      # RCC PLL configuration register,                              Address offset: 0x04
-			('CFGR'      , ctypes.c_uint32),      # RCC clock configuration register,                            Address offset: 0x08
-			('CIR'       , ctypes.c_uint32),      # RCC clock interrupt register,                                Address offset: 0x0C
-			('AHB1RSTR'  , ctypes.c_uint32),      # RCC AHB1 peripheral reset register,                          Address offset: 0x10
-			('AHB2RSTR'  , ctypes.c_uint32),      # RCC AHB2 peripheral reset register,                          Address offset: 0x14
-			('AHB3RSTR'  , ctypes.c_uint32),      # RCC AHB3 peripheral reset register,                          Address offset: 0x18
-			('RESERVED0' , ctypes.c_uint32),      # Reserved, 0x1C
-			('APB1RSTR'  , ctypes.c_uint32),      # RCC APB1 peripheral reset register,                          Address offset: 0x20
-			('APB2RSTR'  , ctypes.c_uint32),      # RCC APB2 peripheral reset register,                          Address offset: 0x24
-			('RESERVED1' , ctypes.c_uint32 * 2),  # Reserved, 0x28-0x2C
-			('AHB1ENR'   , ctypes.c_uint32),      # RCC AHB1 peripheral clock register,                          Address offset: 0x30
-			('AHB2ENR'   , ctypes.c_uint32),      # RCC AHB2 peripheral clock register,                          Address offset: 0x34
-			('AHB3ENR'   , ctypes.c_uint32),      # RCC AHB3 peripheral clock register,                          Address offset: 0x38
-			('RESERVED2' , ctypes.c_uint32),      # Reserved, 0x3C
-			('APB1ENR'   , ctypes.c_uint32),      # RCC APB1 peripheral clock enable register,                   Address offset: 0x40
-			('APB2ENR'   , ctypes.c_uint32),      # RCC APB2 peripheral clock enable register,                   Address offset: 0x44
-			('RESERVED3' , ctypes.c_uint32 * 2),  # Reserved, 0x48-0x4C
-			('AHB1LPENR' , ctypes.c_uint32),      # RCC AHB1 peripheral clock enable in low power mode register, Address offset: 0x50
-			('AHB2LPENR' , ctypes.c_uint32),      # RCC AHB2 peripheral clock enable in low power mode register, Address offset: 0x54
-			('AHB3LPENR' , ctypes.c_uint32),      # RCC AHB3 peripheral clock enable in low power mode register, Address offset: 0x58
-			('RESERVED4' , ctypes.c_uint32),      # Reserved, 0x5C
-			('APB1LPENR' , ctypes.c_uint32),      # RCC APB1 peripheral clock enable in low power mode register, Address offset: 0x60
-			('APB2LPENR' , ctypes.c_uint32),      # RCC APB2 peripheral clock enable in low power mode register, Address offset: 0x64
-			('RESERVED5' , ctypes.c_uint32 * 2),  # Reserved, 0x68-0x6C
-			('BDCR'      , ctypes.c_uint32),      # RCC Backup domain control register,                          Address offset: 0x70
-			('CSR'       , ctypes.c_uint32),      # RCC clock control & status register,                         Address offset: 0x74
-			('RESERVED6' , ctypes.c_uint32 * 2),  # Reserved, 0x78-0x7C
-			('SSCGR'     , ctypes.c_uint32),      # RCC spread spectrum clock generation register,               Address offset: 0x80
-			('PLLI2SCFGR', ctypes.c_uint32),      # RCC PLLI2S configuration register,                           Address offset: 0x84
-			('PLLSAICFGR', ctypes.c_uint32),      # RCC PLLSAI configuration register,                           Address offset: 0x88
-			('DCKCFGR'   , ctypes.c_uint32),      # RCC Dedicated Clocks configuration register,                 Address offset: 0x8C
-		]
+            ('CR'        , ctypes.c_uint32),      # RCC clock control register,                                  Address offset: 0x00
+            ('PLLCFGR'   , ctypes.c_uint32),      # RCC PLL configuration register,                              Address offset: 0x04
+            ('CFGR'      , ctypes.c_uint32),      # RCC clock configuration register,                            Address offset: 0x08
+            ('CIR'       , ctypes.c_uint32),      # RCC clock interrupt register,                                Address offset: 0x0C
+            ('AHB1RSTR'  , ctypes.c_uint32),      # RCC AHB1 peripheral reset register,                          Address offset: 0x10
+            ('AHB2RSTR'  , ctypes.c_uint32),      # RCC AHB2 peripheral reset register,                          Address offset: 0x14
+            ('AHB3RSTR'  , ctypes.c_uint32),      # RCC AHB3 peripheral reset register,                          Address offset: 0x18
+            ('RESERVED0' , ctypes.c_uint32),      # Reserved, 0x1C
+            ('APB1RSTR'  , ctypes.c_uint32),      # RCC APB1 peripheral reset register,                          Address offset: 0x20
+            ('APB2RSTR'  , ctypes.c_uint32),      # RCC APB2 peripheral reset register,                          Address offset: 0x24
+            ('RESERVED1' , ctypes.c_uint32 * 2),  # Reserved, 0x28-0x2C
+            ('AHB1ENR'   , ctypes.c_uint32),      # RCC AHB1 peripheral clock register,                          Address offset: 0x30
+            ('AHB2ENR'   , ctypes.c_uint32),      # RCC AHB2 peripheral clock register,                          Address offset: 0x34
+            ('AHB3ENR'   , ctypes.c_uint32),      # RCC AHB3 peripheral clock register,                          Address offset: 0x38
+            ('RESERVED2' , ctypes.c_uint32),      # Reserved, 0x3C
+            ('APB1ENR'   , ctypes.c_uint32),      # RCC APB1 peripheral clock enable register,                   Address offset: 0x40
+            ('APB2ENR'   , ctypes.c_uint32),      # RCC APB2 peripheral clock enable register,                   Address offset: 0x44
+            ('RESERVED3' , ctypes.c_uint32 * 2),  # Reserved, 0x48-0x4C
+            ('AHB1LPENR' , ctypes.c_uint32),      # RCC AHB1 peripheral clock enable in low power mode register, Address offset: 0x50
+            ('AHB2LPENR' , ctypes.c_uint32),      # RCC AHB2 peripheral clock enable in low power mode register, Address offset: 0x54
+            ('AHB3LPENR' , ctypes.c_uint32),      # RCC AHB3 peripheral clock enable in low power mode register, Address offset: 0x58
+            ('RESERVED4' , ctypes.c_uint32),      # Reserved, 0x5C
+            ('APB1LPENR' , ctypes.c_uint32),      # RCC APB1 peripheral clock enable in low power mode register, Address offset: 0x60
+            ('APB2LPENR' , ctypes.c_uint32),      # RCC APB2 peripheral clock enable in low power mode register, Address offset: 0x64
+            ('RESERVED5' , ctypes.c_uint32 * 2),  # Reserved, 0x68-0x6C
+            ('BDCR'      , ctypes.c_uint32),      # RCC Backup domain control register,                          Address offset: 0x70
+            ('CSR'       , ctypes.c_uint32),      # RCC clock control & status register,                         Address offset: 0x74
+            ('RESERVED6' , ctypes.c_uint32 * 2),  # Reserved, 0x78-0x7C
+            ('SSCGR'     , ctypes.c_uint32),      # RCC spread spectrum clock generation register,               Address offset: 0x80
+            ('PLLI2SCFGR', ctypes.c_uint32),      # RCC PLLI2S configuration register,                           Address offset: 0x84
+            ('PLLSAICFGR', ctypes.c_uint32),      # RCC PLLSAI configuration register,                           Address offset: 0x88
+            ('DCKCFGR'   , ctypes.c_uint32),      # RCC Dedicated Clocks configuration register,                 Address offset: 0x8C
+        ]
 
 class STM32F446Rcc(STM32F4xxRcc):
     class Type(ctypes.Structure):
         """ the structure available in :
-			stm32f446xx.h 
-		"""
+            stm32f446xx.h 
+        """
 
         _fields_ = [
-			('CR'        , ctypes.c_uint32),      # RCC clock control register,                                  Address offset: 0x00
-			('PLLCFGR'   , ctypes.c_uint32),      # RCC PLL configuration register,                              Address offset: 0x04
-			('CFGR'      , ctypes.c_uint32),      # RCC clock configuration register,                            Address offset: 0x08
-			('CIR'       , ctypes.c_uint32),      # RCC clock interrupt register,                                Address offset: 0x0C
-			('AHB1RSTR'  , ctypes.c_uint32),      # RCC AHB1 peripheral reset register,                          Address offset: 0x10
-			('AHB2RSTR'  , ctypes.c_uint32),      # RCC AHB2 peripheral reset register,                          Address offset: 0x14
-			('AHB3RSTR'  , ctypes.c_uint32),      # RCC AHB3 peripheral reset register,                          Address offset: 0x18
-			('RESERVED0' , ctypes.c_uint32),      # Reserved, 0x1C
-			('APB1RSTR'  , ctypes.c_uint32),      # RCC APB1 peripheral reset register,                          Address offset: 0x20
-			('APB2RSTR'  , ctypes.c_uint32),      # RCC APB2 peripheral reset register,                          Address offset: 0x24
-			('RESERVED1' , ctypes.c_uint32 * 2),  # Reserved, 0x28-0x2C
-			('AHB1ENR'   , ctypes.c_uint32),      # RCC AHB1 peripheral clock register,                          Address offset: 0x30
-			('AHB2ENR'   , ctypes.c_uint32),      # RCC AHB2 peripheral clock register,                          Address offset: 0x34
-			('AHB3ENR'   , ctypes.c_uint32),      # RCC AHB3 peripheral clock register,                          Address offset: 0x38
-			('RESERVED2' , ctypes.c_uint32),      # Reserved, 0x3C
-			('APB1ENR'   , ctypes.c_uint32),      # RCC APB1 peripheral clock enable register,                   Address offset: 0x40
-			('APB2ENR'   , ctypes.c_uint32),      # RCC APB2 peripheral clock enable register,                   Address offset: 0x44
-			('RESERVED3' , ctypes.c_uint32 * 2),  # Reserved, 0x48-0x4C
-			('AHB1LPENR' , ctypes.c_uint32),      # RCC AHB1 peripheral clock enable in low power mode register, Address offset: 0x50
-			('AHB2LPENR' , ctypes.c_uint32),      # RCC AHB2 peripheral clock enable in low power mode register, Address offset: 0x54
-			('AHB3LPENR' , ctypes.c_uint32),      # RCC AHB3 peripheral clock enable in low power mode register, Address offset: 0x58
-			('RESERVED4' , ctypes.c_uint32),      # Reserved, 0x5C
-			('APB1LPENR' , ctypes.c_uint32),      # RCC APB1 peripheral clock enable in low power mode register, Address offset: 0x60
-			('APB2LPENR' , ctypes.c_uint32),      # RCC APB2 peripheral clock enable in low power mode register, Address offset: 0x64
-			('RESERVED5' , ctypes.c_uint32 * 2),  # Reserved, 0x68-0x6C
-			('BDCR'      , ctypes.c_uint32),      # RCC Backup domain control register,                          Address offset: 0x70
-			('CSR'       , ctypes.c_uint32),      # RCC clock control & status register,                         Address offset: 0x74
-			('RESERVED6' , ctypes.c_uint32 * 2),  # Reserved, 0x78-0x7C
-			('SSCGR'     , ctypes.c_uint32),      # RCC spread spectrum clock generation register,               Address offset: 0x80
-			('PLLI2SCFGR', ctypes.c_uint32),      # RCC PLLI2S configuration register,                           Address offset: 0x84
-			('PLLSAICFGR', ctypes.c_uint32),      # RCC PLLSAI configuration register,                           Address offset: 0x88
-			('DCKCFGR'   , ctypes.c_uint32),      # RCC Dedicated Clocks configuration register,                 Address offset: 0x8C
-			('CKGATENR'  , ctypes.c_uint32),      # RCC Clocks Gated ENable Register,                            Address offset: 0x90
-			('DCKCFGR2'  , ctypes.c_uint32),      # RCC Dedicated Clocks configuration register 2,               Address offset: 0x94
-		]
+            ('CR'        , ctypes.c_uint32),      # RCC clock control register,                                  Address offset: 0x00
+            ('PLLCFGR'   , ctypes.c_uint32),      # RCC PLL configuration register,                              Address offset: 0x04
+            ('CFGR'      , ctypes.c_uint32),      # RCC clock configuration register,                            Address offset: 0x08
+            ('CIR'       , ctypes.c_uint32),      # RCC clock interrupt register,                                Address offset: 0x0C
+            ('AHB1RSTR'  , ctypes.c_uint32),      # RCC AHB1 peripheral reset register,                          Address offset: 0x10
+            ('AHB2RSTR'  , ctypes.c_uint32),      # RCC AHB2 peripheral reset register,                          Address offset: 0x14
+            ('AHB3RSTR'  , ctypes.c_uint32),      # RCC AHB3 peripheral reset register,                          Address offset: 0x18
+            ('RESERVED0' , ctypes.c_uint32),      # Reserved, 0x1C
+            ('APB1RSTR'  , ctypes.c_uint32),      # RCC APB1 peripheral reset register,                          Address offset: 0x20
+            ('APB2RSTR'  , ctypes.c_uint32),      # RCC APB2 peripheral reset register,                          Address offset: 0x24
+            ('RESERVED1' , ctypes.c_uint32 * 2),  # Reserved, 0x28-0x2C
+            ('AHB1ENR'   , ctypes.c_uint32),      # RCC AHB1 peripheral clock register,                          Address offset: 0x30
+            ('AHB2ENR'   , ctypes.c_uint32),      # RCC AHB2 peripheral clock register,                          Address offset: 0x34
+            ('AHB3ENR'   , ctypes.c_uint32),      # RCC AHB3 peripheral clock register,                          Address offset: 0x38
+            ('RESERVED2' , ctypes.c_uint32),      # Reserved, 0x3C
+            ('APB1ENR'   , ctypes.c_uint32),      # RCC APB1 peripheral clock enable register,                   Address offset: 0x40
+            ('APB2ENR'   , ctypes.c_uint32),      # RCC APB2 peripheral clock enable register,                   Address offset: 0x44
+            ('RESERVED3' , ctypes.c_uint32 * 2),  # Reserved, 0x48-0x4C
+            ('AHB1LPENR' , ctypes.c_uint32),      # RCC AHB1 peripheral clock enable in low power mode register, Address offset: 0x50
+            ('AHB2LPENR' , ctypes.c_uint32),      # RCC AHB2 peripheral clock enable in low power mode register, Address offset: 0x54
+            ('AHB3LPENR' , ctypes.c_uint32),      # RCC AHB3 peripheral clock enable in low power mode register, Address offset: 0x58
+            ('RESERVED4' , ctypes.c_uint32),      # Reserved, 0x5C
+            ('APB1LPENR' , ctypes.c_uint32),      # RCC APB1 peripheral clock enable in low power mode register, Address offset: 0x60
+            ('APB2LPENR' , ctypes.c_uint32),      # RCC APB2 peripheral clock enable in low power mode register, Address offset: 0x64
+            ('RESERVED5' , ctypes.c_uint32 * 2),  # Reserved, 0x68-0x6C
+            ('BDCR'      , ctypes.c_uint32),      # RCC Backup domain control register,                          Address offset: 0x70
+            ('CSR'       , ctypes.c_uint32),      # RCC clock control & status register,                         Address offset: 0x74
+            ('RESERVED6' , ctypes.c_uint32 * 2),  # Reserved, 0x78-0x7C
+            ('SSCGR'     , ctypes.c_uint32),      # RCC spread spectrum clock generation register,               Address offset: 0x80
+            ('PLLI2SCFGR', ctypes.c_uint32),      # RCC PLLI2S configuration register,                           Address offset: 0x84
+            ('PLLSAICFGR', ctypes.c_uint32),      # RCC PLLSAI configuration register,                           Address offset: 0x88
+            ('DCKCFGR'   , ctypes.c_uint32),      # RCC Dedicated Clocks configuration register,                 Address offset: 0x8C
+            ('CKGATENR'  , ctypes.c_uint32),      # RCC Clocks Gated ENable Register,                            Address offset: 0x90
+            ('DCKCFGR2'  , ctypes.c_uint32),      # RCC Dedicated Clocks configuration register 2,               Address offset: 0x94
+        ]
 
     class Type(ctypes.Structure):
         """ the structure available in :
-			stm32f469xx.h
-			stm32f427xx.h
-			stm32f439xx.h
-			stm32f479xx.h
-			stm32f429xx.h
-			stm32f437xx.h 
-		"""
+            stm32f469xx.h
+            stm32f427xx.h
+            stm32f439xx.h
+            stm32f479xx.h
+            stm32f429xx.h
+            stm32f437xx.h 
+        """
 
         _fields_ = [
-			('CR'        , ctypes.c_uint32),      # RCC clock control register,                                  Address offset: 0x00
-			('PLLCFGR'   , ctypes.c_uint32),      # RCC PLL configuration register,                              Address offset: 0x04
-			('CFGR'      , ctypes.c_uint32),      # RCC clock configuration register,                            Address offset: 0x08
-			('CIR'       , ctypes.c_uint32),      # RCC clock interrupt register,                                Address offset: 0x0C
-			('AHB1RSTR'  , ctypes.c_uint32),      # RCC AHB1 peripheral reset register,                          Address offset: 0x10
-			('AHB2RSTR'  , ctypes.c_uint32),      # RCC AHB2 peripheral reset register,                          Address offset: 0x14
-			('AHB3RSTR'  , ctypes.c_uint32),      # RCC AHB3 peripheral reset register,                          Address offset: 0x18
-			('RESERVED0' , ctypes.c_uint32),      # Reserved, 0x1C
-			('APB1RSTR'  , ctypes.c_uint32),      # RCC APB1 peripheral reset register,                          Address offset: 0x20
-			('APB2RSTR'  , ctypes.c_uint32),      # RCC APB2 peripheral reset register,                          Address offset: 0x24
-			('RESERVED1' , ctypes.c_uint32 * 2),  # Reserved, 0x28-0x2C
-			('AHB1ENR'   , ctypes.c_uint32),      # RCC AHB1 peripheral clock register,                          Address offset: 0x30
-			('AHB2ENR'   , ctypes.c_uint32),      # RCC AHB2 peripheral clock register,                          Address offset: 0x34
-			('AHB3ENR'   , ctypes.c_uint32),      # RCC AHB3 peripheral clock register,                          Address offset: 0x38
-			('RESERVED2' , ctypes.c_uint32),      # Reserved, 0x3C
-			('APB1ENR'   , ctypes.c_uint32),      # RCC APB1 peripheral clock enable register,                   Address offset: 0x40
-			('APB2ENR'   , ctypes.c_uint32),      # RCC APB2 peripheral clock enable register,                   Address offset: 0x44
-			('RESERVED3' , ctypes.c_uint32 * 2),  # Reserved, 0x48-0x4C
-			('AHB1LPENR' , ctypes.c_uint32),      # RCC AHB1 peripheral clock enable in low power mode register, Address offset: 0x50
-			('AHB2LPENR' , ctypes.c_uint32),      # RCC AHB2 peripheral clock enable in low power mode register, Address offset: 0x54
-			('AHB3LPENR' , ctypes.c_uint32),      # RCC AHB3 peripheral clock enable in low power mode register, Address offset: 0x58
-			('RESERVED4' , ctypes.c_uint32),      # Reserved, 0x5C
-			('APB1LPENR' , ctypes.c_uint32),      # RCC APB1 peripheral clock enable in low power mode register, Address offset: 0x60
-			('APB2LPENR' , ctypes.c_uint32),      # RCC APB2 peripheral clock enable in low power mode register, Address offset: 0x64
-			('RESERVED5' , ctypes.c_uint32 * 2),  # Reserved, 0x68-0x6C
-			('BDCR'      , ctypes.c_uint32),      # RCC Backup domain control register,                          Address offset: 0x70
-			('CSR'       , ctypes.c_uint32),      # RCC clock control & status register,                         Address offset: 0x74
-			('RESERVED6' , ctypes.c_uint32 * 2),  # Reserved, 0x78-0x7C
-			('SSCGR'     , ctypes.c_uint32),      # RCC spread spectrum clock generation register,               Address offset: 0x80
-			('PLLI2SCFGR', ctypes.c_uint32),      # RCC PLLI2S configuration register,                           Address offset: 0x84
-			('PLLSAICFGR', ctypes.c_uint32),      # RCC PLLSAI configuration register,                           Address offset: 0x88
-			('DCKCFGR'   , ctypes.c_uint32),      # RCC Dedicated Clocks configuration register,                 Address offset: 0x8C
-		]
+            ('CR'        , ctypes.c_uint32),      # RCC clock control register,                                  Address offset: 0x00
+            ('PLLCFGR'   , ctypes.c_uint32),      # RCC PLL configuration register,                              Address offset: 0x04
+            ('CFGR'      , ctypes.c_uint32),      # RCC clock configuration register,                            Address offset: 0x08
+            ('CIR'       , ctypes.c_uint32),      # RCC clock interrupt register,                                Address offset: 0x0C
+            ('AHB1RSTR'  , ctypes.c_uint32),      # RCC AHB1 peripheral reset register,                          Address offset: 0x10
+            ('AHB2RSTR'  , ctypes.c_uint32),      # RCC AHB2 peripheral reset register,                          Address offset: 0x14
+            ('AHB3RSTR'  , ctypes.c_uint32),      # RCC AHB3 peripheral reset register,                          Address offset: 0x18
+            ('RESERVED0' , ctypes.c_uint32),      # Reserved, 0x1C
+            ('APB1RSTR'  , ctypes.c_uint32),      # RCC APB1 peripheral reset register,                          Address offset: 0x20
+            ('APB2RSTR'  , ctypes.c_uint32),      # RCC APB2 peripheral reset register,                          Address offset: 0x24
+            ('RESERVED1' , ctypes.c_uint32 * 2),  # Reserved, 0x28-0x2C
+            ('AHB1ENR'   , ctypes.c_uint32),      # RCC AHB1 peripheral clock register,                          Address offset: 0x30
+            ('AHB2ENR'   , ctypes.c_uint32),      # RCC AHB2 peripheral clock register,                          Address offset: 0x34
+            ('AHB3ENR'   , ctypes.c_uint32),      # RCC AHB3 peripheral clock register,                          Address offset: 0x38
+            ('RESERVED2' , ctypes.c_uint32),      # Reserved, 0x3C
+            ('APB1ENR'   , ctypes.c_uint32),      # RCC APB1 peripheral clock enable register,                   Address offset: 0x40
+            ('APB2ENR'   , ctypes.c_uint32),      # RCC APB2 peripheral clock enable register,                   Address offset: 0x44
+            ('RESERVED3' , ctypes.c_uint32 * 2),  # Reserved, 0x48-0x4C
+            ('AHB1LPENR' , ctypes.c_uint32),      # RCC AHB1 peripheral clock enable in low power mode register, Address offset: 0x50
+            ('AHB2LPENR' , ctypes.c_uint32),      # RCC AHB2 peripheral clock enable in low power mode register, Address offset: 0x54
+            ('AHB3LPENR' , ctypes.c_uint32),      # RCC AHB3 peripheral clock enable in low power mode register, Address offset: 0x58
+            ('RESERVED4' , ctypes.c_uint32),      # Reserved, 0x5C
+            ('APB1LPENR' , ctypes.c_uint32),      # RCC APB1 peripheral clock enable in low power mode register, Address offset: 0x60
+            ('APB2LPENR' , ctypes.c_uint32),      # RCC APB2 peripheral clock enable in low power mode register, Address offset: 0x64
+            ('RESERVED5' , ctypes.c_uint32 * 2),  # Reserved, 0x68-0x6C
+            ('BDCR'      , ctypes.c_uint32),      # RCC Backup domain control register,                          Address offset: 0x70
+            ('CSR'       , ctypes.c_uint32),      # RCC clock control & status register,                         Address offset: 0x74
+            ('RESERVED6' , ctypes.c_uint32 * 2),  # Reserved, 0x78-0x7C
+            ('SSCGR'     , ctypes.c_uint32),      # RCC spread spectrum clock generation register,               Address offset: 0x80
+            ('PLLI2SCFGR', ctypes.c_uint32),      # RCC PLLI2S configuration register,                           Address offset: 0x84
+            ('PLLSAICFGR', ctypes.c_uint32),      # RCC PLLSAI configuration register,                           Address offset: 0x88
+            ('DCKCFGR'   , ctypes.c_uint32),      # RCC Dedicated Clocks configuration register,                 Address offset: 0x8C
+        ]
 
 class STM32F412Rcc(STM32F4xxRcc):
     class Type(ctypes.Structure):
         """ the structure available in :
-			stm32f412cx.h 
-		"""
+            stm32f412cx.h 
+        """
 
         _fields_ = [
-			('CR'        , ctypes.c_uint32),      # RCC clock control register,                                  Address offset: 0x00
-			('PLLCFGR'   , ctypes.c_uint32),      # RCC PLL configuration register,                              Address offset: 0x04
-			('CFGR'      , ctypes.c_uint32),      # RCC clock configuration register,                            Address offset: 0x08
-			('CIR'       , ctypes.c_uint32),      # RCC clock interrupt register,                                Address offset: 0x0C
-			('AHB1RSTR'  , ctypes.c_uint32),      # RCC AHB1 peripheral reset register,                          Address offset: 0x10
-			('AHB2RSTR'  , ctypes.c_uint32),      # RCC AHB2 peripheral reset register,                          Address offset: 0x14
-			('RESERVED0' , ctypes.c_uint32 * 2),  # Reserved, 0x18-0x1C
-			('APB1RSTR'  , ctypes.c_uint32),      # RCC APB1 peripheral reset register,                          Address offset: 0x20
-			('APB2RSTR'  , ctypes.c_uint32),      # RCC APB2 peripheral reset register,                          Address offset: 0x24
-			('RESERVED1' , ctypes.c_uint32 * 2),  # Reserved, 0x28-0x2C
-			('AHB1ENR'   , ctypes.c_uint32),      # RCC AHB1 peripheral clock register,                          Address offset: 0x30
-			('AHB2ENR'   , ctypes.c_uint32),      # RCC AHB2 peripheral clock register,                          Address offset: 0x34
-			('RESERVED2' , ctypes.c_uint32 * 2),  # Reserved, 0x38-0x3C
-			('APB1ENR'   , ctypes.c_uint32),      # RCC APB1 peripheral clock enable register,                   Address offset: 0x40
-			('APB2ENR'   , ctypes.c_uint32),      # RCC APB2 peripheral clock enable register,                   Address offset: 0x44
-			('RESERVED3' , ctypes.c_uint32 * 2),  # Reserved, 0x48-0x4C
-			('AHB1LPENR' , ctypes.c_uint32),      # RCC AHB1 peripheral clock enable in low power mode register, Address offset: 0x50
-			('AHB2LPENR' , ctypes.c_uint32),      # RCC AHB2 peripheral clock enable in low power mode register, Address offset: 0x54
-			('RESERVED4' , ctypes.c_uint32 * 2),  # Reserved, 0x58-0x5C
-			('APB1LPENR' , ctypes.c_uint32),      # RCC APB1 peripheral clock enable in low power mode register, Address offset: 0x60
-			('APB2LPENR' , ctypes.c_uint32),      # RCC APB2 peripheral clock enable in low power mode register, Address offset: 0x64
-			('RESERVED5' , ctypes.c_uint32 * 2),  # Reserved, 0x68-0x6C
-			('BDCR'      , ctypes.c_uint32),      # RCC Backup domain control register,                          Address offset: 0x70
-			('CSR'       , ctypes.c_uint32),      # RCC clock control & status register,                         Address offset: 0x74
-			('RESERVED6' , ctypes.c_uint32 * 2),  # Reserved, 0x78-0x7C
-			('SSCGR'     , ctypes.c_uint32),      # RCC spread spectrum clock generation register,               Address offset: 0x80
-			('PLLI2SCFGR', ctypes.c_uint32),      # RCC PLLI2S configuration register,                           Address offset: 0x84
-			('RESERVED7' , ctypes.c_uint32),      # Reserved, 0x88
-			('DCKCFGR'   , ctypes.c_uint32),      # RCC Dedicated Clocks configuration register,                 Address offset: 0x8C
-			('CKGATENR'  , ctypes.c_uint32),      # RCC Clocks Gated ENable Register,                           Address offset: 0x90
-			('DCKCFGR2'  , ctypes.c_uint32),      # RCC Dedicated Clocks configuration register 2,               Address offset: 0x94
-		]
+            ('CR'        , ctypes.c_uint32),      # RCC clock control register,                                  Address offset: 0x00
+            ('PLLCFGR'   , ctypes.c_uint32),      # RCC PLL configuration register,                              Address offset: 0x04
+            ('CFGR'      , ctypes.c_uint32),      # RCC clock configuration register,                            Address offset: 0x08
+            ('CIR'       , ctypes.c_uint32),      # RCC clock interrupt register,                                Address offset: 0x0C
+            ('AHB1RSTR'  , ctypes.c_uint32),      # RCC AHB1 peripheral reset register,                          Address offset: 0x10
+            ('AHB2RSTR'  , ctypes.c_uint32),      # RCC AHB2 peripheral reset register,                          Address offset: 0x14
+            ('RESERVED0' , ctypes.c_uint32 * 2),  # Reserved, 0x18-0x1C
+            ('APB1RSTR'  , ctypes.c_uint32),      # RCC APB1 peripheral reset register,                          Address offset: 0x20
+            ('APB2RSTR'  , ctypes.c_uint32),      # RCC APB2 peripheral reset register,                          Address offset: 0x24
+            ('RESERVED1' , ctypes.c_uint32 * 2),  # Reserved, 0x28-0x2C
+            ('AHB1ENR'   , ctypes.c_uint32),      # RCC AHB1 peripheral clock register,                          Address offset: 0x30
+            ('AHB2ENR'   , ctypes.c_uint32),      # RCC AHB2 peripheral clock register,                          Address offset: 0x34
+            ('RESERVED2' , ctypes.c_uint32 * 2),  # Reserved, 0x38-0x3C
+            ('APB1ENR'   , ctypes.c_uint32),      # RCC APB1 peripheral clock enable register,                   Address offset: 0x40
+            ('APB2ENR'   , ctypes.c_uint32),      # RCC APB2 peripheral clock enable register,                   Address offset: 0x44
+            ('RESERVED3' , ctypes.c_uint32 * 2),  # Reserved, 0x48-0x4C
+            ('AHB1LPENR' , ctypes.c_uint32),      # RCC AHB1 peripheral clock enable in low power mode register, Address offset: 0x50
+            ('AHB2LPENR' , ctypes.c_uint32),      # RCC AHB2 peripheral clock enable in low power mode register, Address offset: 0x54
+            ('RESERVED4' , ctypes.c_uint32 * 2),  # Reserved, 0x58-0x5C
+            ('APB1LPENR' , ctypes.c_uint32),      # RCC APB1 peripheral clock enable in low power mode register, Address offset: 0x60
+            ('APB2LPENR' , ctypes.c_uint32),      # RCC APB2 peripheral clock enable in low power mode register, Address offset: 0x64
+            ('RESERVED5' , ctypes.c_uint32 * 2),  # Reserved, 0x68-0x6C
+            ('BDCR'      , ctypes.c_uint32),      # RCC Backup domain control register,                          Address offset: 0x70
+            ('CSR'       , ctypes.c_uint32),      # RCC clock control & status register,                         Address offset: 0x74
+            ('RESERVED6' , ctypes.c_uint32 * 2),  # Reserved, 0x78-0x7C
+            ('SSCGR'     , ctypes.c_uint32),      # RCC spread spectrum clock generation register,               Address offset: 0x80
+            ('PLLI2SCFGR', ctypes.c_uint32),      # RCC PLLI2S configuration register,                           Address offset: 0x84
+            ('RESERVED7' , ctypes.c_uint32),      # Reserved, 0x88
+            ('DCKCFGR'   , ctypes.c_uint32),      # RCC Dedicated Clocks configuration register,                 Address offset: 0x8C
+            ('CKGATENR'  , ctypes.c_uint32),      # RCC Clocks Gated ENable Register,                           Address offset: 0x90
+            ('DCKCFGR2'  , ctypes.c_uint32),      # RCC Dedicated Clocks configuration register 2,               Address offset: 0x94
+        ]
```

### Comparing `qiling-1.4.5/qiling/hw/misc/stm32f4xx_syscfg.py` & `qiling-1.4.6/qiling/hw/misc/stm32f4xx_syscfg.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 import ctypes
 from qiling.hw.peripheral import QlPeripheral
 
 
 class STM32F4xxSyscfg(QlPeripheral):
     class Type(ctypes.Structure):
         """ the structure available in :
-			stm32f407xx.h
-			stm32f469xx.h
-			stm32f427xx.h
-			stm32f401xc.h
-			stm32f415xx.h
-			stm32f439xx.h
-			stm32f417xx.h
-			stm32f479xx.h
-			stm32f429xx.h
-			stm32f437xx.h
-			stm32f401xe.h
-			stm32f405xx.h
-			stm32f411xe.h 
-		"""
+            stm32f407xx.h
+            stm32f469xx.h
+            stm32f427xx.h
+            stm32f401xc.h
+            stm32f415xx.h
+            stm32f439xx.h
+            stm32f417xx.h
+            stm32f479xx.h
+            stm32f429xx.h
+            stm32f437xx.h
+            stm32f401xe.h
+            stm32f405xx.h
+            stm32f411xe.h 
+        """
 
         _fields_ = [
-			('MEMRMP'  , ctypes.c_uint32),      # SYSCFG memory remap register,                      Address offset: 0x00
-			('PMC'     , ctypes.c_uint32),      # SYSCFG peripheral mode configuration register,     Address offset: 0x04
-			('EXTICR'  , ctypes.c_uint32 * 4),  # SYSCFG external interrupt configuration registers, Address offset: 0x08-0x14
-			('RESERVED', ctypes.c_uint32 * 2),  # Reserved, 0x18-0x1C
-			('CMPCR'   , ctypes.c_uint32),      # SYSCFG Compensation cell control register,         Address offset: 0x20
-		]
+            ('MEMRMP'  , ctypes.c_uint32),      # SYSCFG memory remap register,                      Address offset: 0x00
+            ('PMC'     , ctypes.c_uint32),      # SYSCFG peripheral mode configuration register,     Address offset: 0x04
+            ('EXTICR'  , ctypes.c_uint32 * 4),  # SYSCFG external interrupt configuration registers, Address offset: 0x08-0x14
+            ('RESERVED', ctypes.c_uint32 * 2),  # Reserved, 0x18-0x1C
+            ('CMPCR'   , ctypes.c_uint32),      # SYSCFG Compensation cell control register,         Address offset: 0x20
+        ]
```

### Comparing `qiling-1.4.5/qiling/hw/net/stm32f4xx_eth.py` & `qiling-1.4.6/qiling/hw/net/stm32f4xx_eth.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/hw/peripheral.py` & `qiling-1.4.6/qiling/hw/peripheral.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/hw/power/sam3xa_pmc.py` & `qiling-1.4.6/qiling/hw/power/sam3xa_pmc.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,15 @@
     def __init__(self, ql: Qiling, label: str, intn = None):
         super().__init__(ql, label)
 
         self.instance = self.struct()
         self.intn = intn
 
     @QlPeripheral.monitor()
-    def read(self, offset: int, size: int) -> int:		
+    def read(self, offset: int, size: int) -> int:        
         buf = ctypes.create_string_buffer(size)
         ctypes.memmove(buf, ctypes.addressof(self.instance) + offset, size)
         return int.from_bytes(buf.raw, byteorder='little')
 
     @QlPeripheral.monitor()
     def write(self, offset: int, size: int, value: int):
         if offset == self.struct.CKGR_MOR.offset:
```

### Comparing `qiling-1.4.5/qiling/hw/sd/stm32f4xx_sdio.py` & `qiling-1.4.6/qiling/hw/sd/stm32f4xx_sdio.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/hw/spi/gd32vf1xx_spi.py` & `qiling-1.4.6/qiling/hw/spi/gd32vf1xx_spi.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/hw/spi/mk64f12_spi.py` & `qiling-1.4.6/qiling/hw/spi/mk64f12_spi.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/hw/spi/sam3xa_spi.py` & `qiling-1.4.6/qiling/hw/spi/sam3xa_spi.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/hw/spi/stm32f1xx_spi.py` & `qiling-1.4.6/qiling/hw/spi/stm32f1xx_spi.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/hw/spi/stm32f4xx_spi.py` & `qiling-1.4.6/qiling/hw/spi/stm32f4xx_spi.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,15 +86,15 @@
         if offset == self.struct.CR1.offset:
             value &= SPI_CR1.RW_MASK
 
         elif offset == self.struct.CR2.offset:
             value &= SPI_CR2.RW_MASK
         
         elif offset == self.struct.CRCPR.offset:
-            value &= SPI_CRCPR.CRCPOLY		
+            value &= SPI_CRCPR.CRCPOLY        
 
         elif offset == self.struct.I2SCFGR.offset:
             value &= SPI_I2SCFGR.RW_MASK
 
         elif offset == self.struct.I2SPR.offset:
             value &= SPI_I2SPR.RW_MASK
```

### Comparing `qiling-1.4.5/qiling/hw/timer/__init__.py` & `qiling-1.4.6/qiling/hw/timer/__init__.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/hw/timer/gd32vf1xx_rtc.py` & `qiling-1.4.6/qiling/hw/timer/gd32vf1xx_rtc.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/hw/timer/gd32vf1xx_timer.py` & `qiling-1.4.6/qiling/hw/timer/gd32vf1xx_timer.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/hw/timer/mk64f12_ftm.py` & `qiling-1.4.6/qiling/hw/timer/mk64f12_ftm.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/hw/timer/mk64f12_rtc.py` & `qiling-1.4.6/qiling/hw/timer/mk64f12_rtc.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/hw/timer/sam3xa_tc.py` & `qiling-1.4.6/qiling/hw/timer/sam3xa_tc.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/hw/timer/stm32f4xx_rtc.py` & `qiling-1.4.6/qiling/hw/timer/stm32f4xx_rtc.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,38 +9,38 @@
 from qiling.hw.peripheral import QlPeripheral
 from qiling.hw.const.stm32f4xx_rtc import RTC_TR, RTC_ISR
 
 
 class STM32F4xxRtc(QlPeripheral):
     class Type(ctypes.Structure):
         """ the structure is available in :
-		        stm32f423xx.h
-		        stm32f469xx.h
-		        stm32f427xx.h
-		        stm32f479xx.h
-		        stm32f413xx.h
-		        stm32f429xx.h
-		        stm32f439xx.h
-		        stm32f415xx.h
-		        stm32f412cx.h
-		        stm32f412rx.h
-		        stm32f410tx.h
-		        stm32f410cx.h
-		        stm32f412zx.h
-		        stm32f405xx.h
-		        stm32f407xx.h
-		        stm32f417xx.h
-		        stm32f446xx.h
-		        stm32f401xc.h
-		        stm32f437xx.h
-		        stm32f401xe.h
-		        stm32f412vx.h
-		        stm32f410rx.h
-		        stm32f411xe.h 
-		"""
+                stm32f423xx.h
+                stm32f469xx.h
+                stm32f427xx.h
+                stm32f479xx.h
+                stm32f413xx.h
+                stm32f429xx.h
+                stm32f439xx.h
+                stm32f415xx.h
+                stm32f412cx.h
+                stm32f412rx.h
+                stm32f410tx.h
+                stm32f410cx.h
+                stm32f412zx.h
+                stm32f405xx.h
+                stm32f407xx.h
+                stm32f417xx.h
+                stm32f446xx.h
+                stm32f401xc.h
+                stm32f437xx.h
+                stm32f401xe.h
+                stm32f412vx.h
+                stm32f410rx.h
+                stm32f411xe.h 
+        """
 
         _fields_ = [
             ('TR'          , ctypes.c_uint32),  # RTC time register,                                        Address offset: 0x00
             ('DR'          , ctypes.c_uint32),  # RTC date register,                                        Address offset: 0x04
             ('CR'          , ctypes.c_uint32),  # RTC control register,                                     Address offset: 0x08
             ('ISR'         , ctypes.c_uint32),  # RTC initialization and status register,                   Address offset: 0x0C
             ('PRER'        , ctypes.c_uint32),  # RTC prescaler register,                                   Address offset: 0x10
```

### Comparing `qiling-1.4.5/qiling/hw/timer/stm32f4xx_tim.py` & `qiling-1.4.6/qiling/hw/timer/stm32f4xx_tim.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/hw/timer/timer.py` & `qiling-1.4.6/qiling/hw/timer/timer.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/hw/utils/access.py` & `qiling-1.4.6/qiling/hw/utils/access.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/hw/utils/serial.py` & `qiling-1.4.6/qiling/hw/utils/serial.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/loader/blob.py` & `qiling-1.4.6/qiling/loader/blob.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/loader/dos.py` & `qiling-1.4.6/qiling/loader/dos.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,15 +80,15 @@
             sp = 0xfff0
             ss = cs
 
             base_address = (cs << 4) + ip
 
             # https://en.wikipedia.org/wiki/Master_boot_record#BIOS_to_MBR_interface
             if not self.ql.os.fs_mapper.has_mapping(0x80):
-                self.ql.os.fs_mapper.add_fs_mapping(0x80, QlDisk(path, 0x80))
+                self.ql.os.fs_mapper.add_mapping(0x80, QlDisk(path, 0x80))
 
             # 0x80 -> first drive
             self.ql.arch.regs.dx = 0x80
         else:
             raise NotImplementedError()
 
         self.ql.arch.regs.cs = cs
```

### Comparing `qiling-1.4.5/qiling/loader/elf.py` & `qiling-1.4.6/qiling/loader/elf.py`

 * *Files 2% similar despite different names*

```diff
@@ -193,20 +193,24 @@
                         raise RuntimeError
 
                 else:
                     load_regions.append((lbound, ubound, perms))
 
             # map the memory regions
             for lbound, ubound, perms in load_regions:
-                try:
-                    self.ql.mem.map(lbound, ubound - lbound, perms, os.path.basename(info))
-                except QlMemoryMappedError:
-                    self.ql.log.exception(f'Failed to map {lbound:#x}-{ubound:#x}')
-                else:
-                    self.ql.log.debug(f'Mapped {lbound:#x}-{ubound:#x}')
+                size = ubound - lbound
+
+                # there might be a region with zero size. in this case, do not mmap it
+                if size:
+                    try:
+                        self.ql.mem.map(lbound, size, perms, os.path.basename(info))
+                    except QlMemoryMappedError:
+                        self.ql.log.exception(f'Failed to map {lbound:#x}-{ubound:#x}')
+                    else:
+                        self.ql.log.debug(f'Mapped {lbound:#x}-{ubound:#x}')
 
             # load loadable segments contents to memory
             for seg in load_segments:
                 self.ql.mem.write(load_address + seg['p_vaddr'], seg.data())
 
             return load_regions[0][0], load_regions[-1][1]
 
@@ -226,32 +230,37 @@
         interp_seg = next(elffile.iter_segments(type='PT_INTERP'), None)
         interp_path = str(interp_seg.get_interp_name()) if interp_seg else ''
 
         interp_address = 0
 
         # load the interpreter, if there is one
         if interp_path:
-            interp_local_path = os.path.normpath(self.ql.rootfs + interp_path)
-            self.ql.log.debug(f'Interpreter path: {interp_local_path}')
+            interp_vpath = self.ql.os.path.virtual_abspath(interp_path)
+            interp_hpath = self.ql.os.path.virtual_to_host_path(interp_path)
+
+            self.ql.log.debug(f'Interpreter path: {interp_vpath}')
+
+            if not self.ql.os.path.is_safe_host_path(interp_hpath):
+                raise PermissionError(f'unsafe path: {interp_hpath}')
 
-            with open(interp_local_path, 'rb') as infile:
+            with open(interp_hpath, 'rb') as infile:
                 interp = ELFFile(infile)
                 min_vaddr = min(seg['p_vaddr'] for seg in interp.iter_segments(type='PT_LOAD'))
 
                 # determine interpreter base address
                 # some old interpreters may not be PIE: p_vaddr of the first LOAD segment is not zero
                 # we should load interpreter at the address p_vaddr specified in such situation
                 interp_address = self.profile.getint('interp_address') if min_vaddr == 0 else 0
                 self.ql.log.debug(f'Interpreter addr: {interp_address:#x}')
 
                 # load interpreter segments data to memory
-                interp_start, interp_end = load_elf_segments(interp, interp_address, interp_local_path)
+                interp_start, interp_end = load_elf_segments(interp, interp_address, interp_vpath)
 
                 # add interpreter to the loaded images list
-                self.images.append(Image(interp_start, interp_end, os.path.abspath(interp_local_path)))
+                self.images.append(Image(interp_start, interp_end, interp_hpath))
 
                 # determine entry point
                 entry_point = interp_address + interp['e_entry']
 
         # set mmap addr
         mmap_address = self.profile.getint('mmap_address')
         self.ql.log.debug(f'mmap_address is : {mmap_address:#x}')
@@ -264,15 +273,15 @@
         new_stack = stack_addr
 
         def __push_str(top: int, s: str) -> int:
             """Write a string to stack memory and adjust the top of stack accordingly.
             Top of stack remains aligned to pointer size
             """
 
-            data = s.encode('utf-8') + b'\x00'
+            data = s.encode('latin') + b'\x00'
             top = self.ql.mem.align(top - len(data), self.ql.arch.pointersize)
             self.ql.mem.write(top, data)
 
             return top
 
         # write argc
         elf_table.extend(self.ql.pack(len(argv)))
@@ -349,15 +358,14 @@
         self.auxv = new_stack + bytes_before_auxv
 
         self.stack_address = new_stack
         self.load_address = load_address
         self.init_sp = self.ql.arch.regs.arch_sp
 
         self.ql.os.entry_point = self.entry_point = entry_point
-        self.ql.os.elf_mem_start = mem_start
         self.ql.os.elf_entry = self.elf_entry
         self.ql.os.function_hook = FunctionHook(self.ql, elf_phdr, elf_phnum, elf_phent, load_address, mem_end)
 
         # If there is a loader, we ignore exit
         self.skip_exit_check = (self.elf_entry != self.entry_point)
 
         # map vsyscall section for some specific needs
```

### Comparing `qiling-1.4.5/qiling/loader/evm.py` & `qiling-1.4.6/qiling/loader/evm.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/loader/loader.py` & `qiling-1.4.6/qiling/loader/loader.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 #!/usr/bin/env python3
-# 
+#
 # Cross Platform and Multi Architecture Advanced Binary Emulation Framework
 #
 
+from __future__ import annotations
+
 import os
-from typing import Any, Mapping, MutableSequence, NamedTuple, Optional
+from typing import TYPE_CHECKING, Any, Mapping, MutableSequence, NamedTuple, Optional
+
+if TYPE_CHECKING:
+    from qiling import Qiling
 
-from qiling import Qiling
 
 class Image(NamedTuple):
     base: int
     end: int
     path: str
 
+
 class QlLoader:
     def __init__(self, ql: Qiling):
         self.ql = ql
         self.env = self.ql.env
         self.argv = self.ql.argv
         self.images: MutableSequence[Image] = []
         self.skip_exit_check = False
```

### Comparing `qiling-1.4.5/qiling/loader/macho.py` & `qiling-1.4.6/qiling/loader/macho.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/loader/macho_parser/const.py` & `qiling-1.4.6/qiling/loader/macho_parser/const.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/loader/macho_parser/data.py` & `qiling-1.4.6/qiling/loader/macho_parser/data.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/loader/macho_parser/header.py` & `qiling-1.4.6/qiling/loader/macho_parser/header.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/loader/macho_parser/loadcommand.py` & `qiling-1.4.6/qiling/loader/macho_parser/loadcommand.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/loader/macho_parser/parser.py` & `qiling-1.4.6/qiling/loader/macho_parser/parser.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/loader/macho_parser/utils.py` & `qiling-1.4.6/qiling/loader/macho_parser/utils.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/loader/mcu.py` & `qiling-1.4.6/qiling/loader/mcu.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/loader/pe.py` & `qiling-1.4.6/qiling/loader/pe.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,39 @@
 #!/usr/bin/env python3
 #
 # Cross Platform and Multi Architecture Advanced Binary Emulation Framework
 #
 
-import os, pefile, pickle, secrets, ntpath
-from typing import Any, Dict, MutableMapping, NamedTuple, Optional, Mapping, Sequence, Tuple, Union
+from __future__ import annotations
+
+import os
+import pefile
+import pickle
+import secrets
+import ntpath
+from typing import TYPE_CHECKING, Any, Dict, MutableMapping, NamedTuple, Optional, Mapping, Sequence, Tuple, Union
 
 from unicorn import UcError
 from unicorn.x86_const import UC_X86_REG_CR4, UC_X86_REG_CR8
 
-from qiling import Qiling
 from qiling.arch.x86_const import FS_SEGMENT_ADDR, GS_SEGMENT_ADDR
-from qiling.const import QL_ARCH
+from qiling.const import QL_ARCH, QL_STATE
 from qiling.exception import QlErrorArch
 from qiling.os.const import POINTER
 from qiling.os.windows.api import HINSTANCE, DWORD, LPVOID
 from qiling.os.windows.fncc import CDECL
 from qiling.os.windows.utils import has_lib_ext
 from qiling.os.windows.structs import *
 from .loader import QlLoader, Image
 
+if TYPE_CHECKING:
+    from logging import Logger
+    from qiling import Qiling
+
+
 class QlPeCacheEntry(NamedTuple):
     ba: int
     data: bytearray
     cmdlines: Sequence
     import_symbols: MutableMapping[int, dict]
     import_table: MutableMapping[Union[str, int], int]
 
@@ -178,15 +188,15 @@
 
             if not self.ql.mem.is_available(image_base, image_size):
                 image_base = self.ql.mem.find_free_space(image_size, minaddr=image_base, align=0x10000)
                 self.ql.log.debug(f'DLL preferred base address is taken, loading to: {image_base:#x}')
                 relocate = True
 
             if relocate:
-                with ShowProgress(0.1337):
+                with ShowProgress(self.ql.log, 0.1337):
                     dll.relocate_image(image_base)
 
             data = bytearray(dll.get_memory_mapped_image())
             assert image_size >= len(data)
 
             cmdlines = []
 
@@ -243,21 +253,16 @@
             # DllMain of system libraries may fail due to incomplete or inaccurate
             # mock implementation. due to unicorn limitations, recovering from such
             # errors may be possible only if the function was not invoked from within
             # a hook.
             #
             # in case of a dll loaded from a hooked API call, failures would not be
             # recoverable and we have to give up its DllMain.
-            if not self.ql.os.PE_RUN:
-
-                # temporarily set PE_RUN to allow proper fcall unwinding during
-                # execution of DllMain
-                self.ql.os.PE_RUN = True
+            if self.ql.emu_state is not QL_STATE.STARTED:
                 self.call_dll_entrypoint(dll, dll_base, dll_len, dll_name)
-                self.ql.os.PE_RUN = False
 
         self.ql.log.info(f'Done loading {dll_name}')
 
         return dll_base
 
     def call_dll_entrypoint(self, dll: pefile.PE, dll_base: int, dll_len: int, dll_name: str):
         entry_address = dll.OPTIONAL_HEADER.AddressOfEntryPoint
@@ -549,14 +554,18 @@
 
     def init_exports(self, pe: pefile.PE):
         if not Process.directory_exists(pe, 'IMAGE_DIRECTORY_ENTRY_EXPORT'):
             return
 
         # Do a full load if IMAGE_DIRECTORY_ENTRY_EXPORT is present so we can load the exports
         pe.full_load()
+        
+        # address corner case for malformed export tables where IMAGE_DIRECTORY_ENTRY_EXPORT exists, but DIRECTORY_ENTRY_EXPORT does not
+        if not hasattr(pe, 'DIRECTORY_ENTRY_EXPORT'): 
+            return
 
         iat = {}
 
         # parse directory entry export
         for entry in pe.DIRECTORY_ENTRY_EXPORT.symbols:
             ea = self.pe_image_address + entry.address
 
@@ -860,49 +869,129 @@
             for each in self.init_dlls:
                 super().load_dll(each, self.is_driver)
 
         # move entry_point to ql.os
         self.ql.os.entry_point = self.entry_point
         self.init_sp = self.ql.arch.regs.arch_sp
 
+
 class ShowProgress:
-    """Display a progress animation while performing a time
-    consuming task.
+    """Display a progress animation while performing a time consuming task.
 
     Example:
-        >>> with ShowProgress(0.1):
+        >>> with ShowProgress(logger, 0.15):
         ...     do_some_time_consuming_task()
     """
 
-    def __init__(self, interval: float) -> None:
-        import sys
-        from threading import Thread, Event
+    # animation frames: a sequence of chars or strings to display. any sequence of string elements
+    # may be used as long as they are of the same length.
+    #
+    # for example: ['>   ', '>>  ', ' >> ', '  >>', '   >', '    ']
+    _frames_ = r'/-\|'
 
-        # animation frames; any sequence of chars or strings may be used, as long
-        # as they are of the same length. e.g. ['>   ', '>>  ', ' >> ', '  >>', '   >', '    ']
-        frames = r'/-\|'
-        stream = sys.stderr
+    # animation marker: this is used to tell animation log records from the rest.
+    _marker_ = r'$__ql_anim__'
+
+    def __init__(self, logger: Logger, interval: float) -> None:
+        from typing import List, Callable
+        from threading import Thread, Event
 
         def show_animation():
             i = 0
 
             while not self.stopped.wait(interval):
-                # TODO: find a proper way to use the logger for that
-                print(f'[{frames[i % len(frames)]}]', end='\r', flush=True, file=stream)
+                frame = self._frames_[i % len(self._frames_)]
+                logger.info(f'{self._marker_}{frame}')
+
                 i += 1
 
-        def show_nothing():
-            pass
+        self.stopped = Event()
+        self.thread = Thread(target=show_animation)
 
-        # avoid flooding log files with animation frames
-        action = show_animation if stream.isatty() else show_nothing
+        self.logger = logger
+        self.handlers_restorers: List[Callable[[], None]] = []
 
-        self.stopped = Event()
-        self.thread = Thread(target=action)
+    def __setup_handlers(self):
+        from logging import Filter, Formatter, LogRecord, StreamHandler
+
+        # while progress animation is useful on tty streams, it is not very useful on log files
+        # and most probably just flood the log files with animation frames.
+        #
+        # to avoid such flooding an animation filter is added to the non-tty stream handlers to
+        # filter out the animation records. in addition, tty stream handlers are assigned with
+        # an animation formatter to display the animation frames nicely.
+        #
+        # when the animation context exits, all the changes made to the handlers are reverted.
+
+        def has_anim_marker(rec: LogRecord) -> bool:
+            """Tell whether a log record is an animation record or not.
+            """
+
+            return rec.getMessage().startswith(ShowProgress._marker_)
+
+        def strip_anim_marker(rec: LogRecord) -> None:
+            """Remove animation marker from log record.
+            """
+
+            rec.message = rec.message[len(ShowProgress._marker_):]
+
+        class AnimFormatter(Formatter):
+            """A log record formatter that removes animation markers.
+            """
+
+            def formatMessage(self, record: LogRecord) -> str:
+                if has_anim_marker(record):
+                    strip_anim_marker(record)
+
+                return super().formatMessage(record)
+
+        class AnimFilter(Filter):
+            """A log record filter that thwarts animation records.
+            """
+
+            def filter(self, record: LogRecord) -> bool:
+                return not has_anim_marker(record)
+
+        # the animation frames will be displayed within brackets
+        anim_formatter = AnimFormatter('[%(message)s]')
+        anim_filter = AnimFilter()
+
+        for h in self.logger.handlers:
+            # if this is a tty stream handler, modify some of its attributes to
+            # let the animation display correctly
+            if isinstance(h, StreamHandler) and h.stream.isatty():
+                orig_terminator = h.terminator
+                orig_formatter = h.formatter
+
+                h.terminator = '\r'
+                h.setFormatter(anim_formatter)
+
+                def __restore_modified() -> None:
+                    h.terminator = orig_terminator
+                    h.setFormatter(orig_formatter)
+
+                restorer = __restore_modified
+
+            # otherwise, apply a filter that will ignore animation records
+            else:
+                h.addFilter(anim_filter)
+
+                def __restore_silenced() -> None:
+                    h.removeFilter(anim_filter)
+
+                restorer = __restore_silenced
+
+            self.handlers_restorers.append(restorer)
+
+    def __restore_handlers(self) -> None:
+        for restorer in self.handlers_restorers:
+            restorer()
 
     def __enter__(self):
+        self.__setup_handlers()
         self.thread.start()
 
         return self
 
-    def __exit__(self, *args) -> None:
+    def __exit__(self, extype, value, traceback):
         self.stopped.set()
+        self.__restore_handlers()
```

### Comparing `qiling-1.4.5/qiling/loader/pe_uefi.py` & `qiling-1.4.6/qiling/loader/pe_uefi.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/log.py` & `qiling-1.4.6/qiling/log.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,57 +1,65 @@
 #!/usr/bin/env python3
 #
 # Cross Platform and Multi Architecture Advanced Binary Emulation Framework
 #
 
+from __future__ import annotations
+
 import copy
 import logging
 import os
 import re
 import weakref
 
-from typing import Optional, TextIO
+from typing import TYPE_CHECKING, Optional, TextIO
+from logging import Filter, Formatter, LogRecord, Logger, NullHandler, StreamHandler, FileHandler
 
 from qiling.const import QL_VERBOSE
 
+if TYPE_CHECKING:
+    from qiling import Qiling
+
+
 QL_INSTANCE_ID = 114514
 
 FMT_STR = '%(levelname)s\t%(message)s'
 
+
 class COLOR:
-    WHITE   = '\033[37m'
     CRIMSON = '\033[31m'
     RED     = '\033[91m'
     GREEN   = '\033[92m'
     YELLOW  = '\033[93m'
     BLUE    = '\033[94m'
     MAGENTA = '\033[95m'
-    CYAN    = '\033[96m'
-    ENDC    = '\033[0m'
+    DEFAULT = '\033[39m'
 
-class QlBaseFormatter(logging.Formatter):
+
+class QlBaseFormatter(Formatter):
     __level_tag = {
         'WARNING'  : '[!]',
         'INFO'     : '[=]',
         'DEBUG'    : '[+]',
         'CRITICAL' : '[x]',
         'ERROR'    : '[x]'
     }
 
-    def __init__(self, ql, *args, **kwargs):
+    def __init__(self, ql: Qiling, *args, **kwargs):
         super().__init__(*args, **kwargs)
-        self.ql = weakref.proxy(ql)
+
+        self.ql: Qiling = weakref.proxy(ql)
 
     def get_level_tag(self, level: str) -> str:
         return self.__level_tag[level]
 
     def get_thread_tag(self, thread: str) -> str:
         return thread
 
-    def format(self, record: logging.LogRecord):
+    def format(self, record: LogRecord):
         # In case we have multiple formatters, we have to keep a copy of the record.
         record = copy.copy(record)
 
         # early logging may access ql.os when it is not yet set
         try:
             cur_thread = self.ql.os.thread_management.cur_thread
         except AttributeError:
@@ -60,52 +68,56 @@
             tid = self.get_thread_tag(str(cur_thread))
 
         level = self.get_level_tag(record.levelname)
         record.levelname = f'{level} {tid}'
 
         return super().format(record)
 
+
 class QlColoredFormatter(QlBaseFormatter):
     __level_color = {
         'WARNING'  : COLOR.YELLOW,
         'INFO'     : COLOR.BLUE,
         'DEBUG'    : COLOR.MAGENTA,
         'CRITICAL' : COLOR.CRIMSON,
         'ERROR'    : COLOR.RED
     }
 
     def get_level_tag(self, level: str) -> str:
         s = super().get_level_tag(level)
 
-        return f'{self.__level_color[level]}{s}{COLOR.ENDC}'
+        return f'{self.__level_color[level]}{s}{COLOR.DEFAULT}'
 
     def get_thread_tag(self, tid: str) -> str:
         s = super().get_thread_tag(tid)
 
-        return f'{COLOR.GREEN}{s}{COLOR.ENDC}'
+        return f'{COLOR.GREEN}{s}{COLOR.DEFAULT}'
+
 
-class RegexFilter(logging.Filter):
+class RegexFilter(Filter):
     def update_filter(self, regexp: str):
         self._filter = re.compile(regexp)
 
-    def filter(self, record: logging.LogRecord):
+    def filter(self, record: LogRecord):
         msg = record.getMessage()
 
         return self._filter.match(msg) is not None
 
+
 def resolve_logger_level(verbose: QL_VERBOSE) -> int:
     return {
         QL_VERBOSE.DISABLED : logging.CRITICAL,
         QL_VERBOSE.OFF      : logging.WARNING,
         QL_VERBOSE.DEFAULT  : logging.INFO,
         QL_VERBOSE.DEBUG    : logging.DEBUG,
         QL_VERBOSE.DISASM   : logging.DEBUG,
         QL_VERBOSE.DUMP     : logging.DEBUG
     }[verbose]
 
+
 def __is_color_terminal(stream: TextIO) -> bool:
     """Determine whether standard output is attached to a color terminal.
 
     see: https://stackoverflow.com/questions/53574442/how-to-reliably-test-color-capability-of-an-output-terminal-in-python3
     """
 
     def __handle_nt(fd: int) -> bool:
@@ -138,51 +150,63 @@
         'posix' : __handle_posix
     }
 
     handler = handlers.get(os.name, __default)
 
     return handler(stream.fileno())
 
-def setup_logger(ql, log_file: Optional[str], console: bool, log_override: Optional[logging.Logger], log_plain: bool):
+
+def setup_logger(ql: Qiling, log_file: Optional[str], console: bool, log_override: Optional[Logger], log_plain: bool):
     global QL_INSTANCE_ID
 
     # If there is an override for our logger, then use it.
     if log_override is not None:
         log = log_override
     else:
         # We should leave the root logger untouched.
         log = logging.getLogger(f'qiling{QL_INSTANCE_ID}')
         QL_INSTANCE_ID += 1
 
         # Disable propagation to avoid duplicate output.
         log.propagate = False
+
         # Clear all handlers and filters.
-        log.handlers = []
-        log.filters = []
+        log.handlers.clear()
+        log.filters.clear()
 
         # Do we have console output?
         if console:
-            handler = logging.StreamHandler()
+            handler = StreamHandler()
 
-            if log_plain or not __is_color_terminal(handler.stream):
+            # adhere to the NO_COLOR convention (see: https://no-color.org/)
+            no_color = os.getenv('NO_COLOR', False)
+
+            if no_color or log_plain or not __is_color_terminal(handler.stream):
                 formatter = QlBaseFormatter(ql, FMT_STR)
             else:
                 formatter = QlColoredFormatter(ql, FMT_STR)
 
             handler.setFormatter(formatter)
             log.addHandler(handler)
         else:
-            handler = logging.NullHandler()
+            handler = NullHandler()
             log.addHandler(handler)
 
         # Do we have to write log to a file?
         if log_file is not None:
-            handler = logging.FileHandler(log_file)
+            handler = FileHandler(log_file)
             formatter = QlBaseFormatter(ql, FMT_STR)
             handler.setFormatter(formatter)
             log.addHandler(handler)
 
     log.setLevel(logging.INFO)
 
+    # optimize logging speed by avoiding the collection of unnecesary logging properties
+    logging._srcfile = None
+    logging.logThreads = False
+    logging.logProcesses = False
+    logging.logMultiprocessing = False
+
     return log
 
+
 __all__ = ['RegexFilter', 'setup_logger', 'resolve_logger_level']
```

### Comparing `qiling-1.4.5/qiling/os/blob/blob.py` & `qiling-1.4.6/qiling/os/blob/blob.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/os/const.py` & `qiling-1.4.6/qiling/os/const.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/os/disk.py` & `qiling-1.4.6/qiling/os/disk.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/os/dos/dos.py` & `qiling-1.4.6/qiling/os/dos/dos.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/os/dos/interrupts/__init__.py` & `qiling-1.4.6/qiling/os/dos/interrupts/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -18,18 +18,18 @@
 
 IntHandler = Callable[[Qiling], None]
 
 # http://spike.scu.edu.au/~barry/interrupts.html
 # http://www2.ift.ulaval.ca/~marchand/ift17583/dosints.pdf
 
 handlers: Mapping[int, IntHandler] = {
-	0x10: int10.handler,
-	0x13: int13.handler,
-	0x15: int15.handler,
-	0x16: int16.handler,
-	0x19: int19.handler,
-	0x1a: int1a.handler,
-	0x20: int20.handler,
-	0x21: int21.handler
+    0x10: int10.handler,
+    0x13: int13.handler,
+    0x15: int15.handler,
+    0x16: int16.handler,
+    0x19: int19.handler,
+    0x1a: int1a.handler,
+    0x20: int20.handler,
+    0x21: int21.handler
 }
 
 __all__ = ['handlers']
```

### Comparing `qiling-1.4.5/qiling/os/dos/interrupts/int16.py` & `qiling-1.4.6/qiling/os/dos/interrupts/int16.py`

 * *Files 10% similar despite different names*

```diff
@@ -115,63 +115,63 @@
     #'LWIN':   [[0xE0, 0x5B], [0xE0, 0xDB]], 
     #'RWIN':   [[0xE0, 0x5C], [0xE0, 0xDC]], 
     # No scan code for pause key released
     #'PAUSE':  [[0xE1, 0x1D, 0x45, 0xE1, 0x9D, 0xC5], []],
 }
 
 def parse_key(ky):
-	# https://stackoverflow.com/questions/27200597/c-ncurses-key-backspace-not-working
-	# https://stackoverflow.com/questions/44943249/detecting-key-backspace-in-ncurses
+    # https://stackoverflow.com/questions/27200597/c-ncurses-key-backspace-not-working
+    # https://stackoverflow.com/questions/44943249/detecting-key-backspace-in-ncurses
 
-	# oh my curses...
-	if ky == curses.KEY_BACKSPACE or ky == 127:
-		ky = ord(b'\b')
+    # oh my curses...
+    if ky == curses.KEY_BACKSPACE or ky == 127:
+        ky = ord(b'\b')
 
-	return ky
+    return ky
 
 def get_scan_code(ch):
-	return SCANCODES.get(ch, 0)
+    return SCANCODES.get(ch, 0)
 
 def __leaf_00(ql: Qiling):
-	curses.nonl()
-	key = parse_key(ql.os.stdscr.getch())
-	ql.log.debug(f"Get key: {hex(key)}")
-	if curses.ascii.isascii(key):
-		ql.arch.regs.al = key
-	else:
-		ql.arch.regs.al = 0
-	ql.arch.regs.ah = get_scan_code(key)
-	curses.nl()
+    curses.nonl()
+    key = parse_key(ql.os.stdscr.getch())
+    ql.log.debug(f"Get key: {hex(key)}")
+    if curses.ascii.isascii(key):
+        ql.arch.regs.al = key
+    else:
+        ql.arch.regs.al = 0
+    ql.arch.regs.ah = get_scan_code(key)
+    curses.nl()
 
 def __leaf_01(ql: Qiling):
-	curses.nonl()
-	# set non-blocking
-	ql.os.stdscr.timeout(0)
-	key = parse_key(ql.os.stdscr.getch())
-
-	if key == -1:
-		ql.os.set_zf()
-		ql.arch.regs.ax = 0
-	else:
-		ql.log.debug(f"Has key: {hex(key)} ({curses.ascii.unctrl(key)})")
-		ql.arch.regs.al = key
-		ql.arch.regs.ah = get_scan_code(key)
-		ql.os.clear_zf()
-		# Buffer shouldn't be removed in this interrupt.
-		curses.ungetch(key)
+    curses.nonl()
+    # set non-blocking
+    ql.os.stdscr.timeout(0)
+    key = parse_key(ql.os.stdscr.getch())
+
+    if key == -1:
+        ql.os.set_zf()
+        ql.arch.regs.ax = 0
+    else:
+        ql.log.debug(f"Has key: {hex(key)} ({curses.ascii.unctrl(key)})")
+        ql.arch.regs.al = key
+        ql.arch.regs.ah = get_scan_code(key)
+        ql.os.clear_zf()
+        # Buffer shouldn't be removed in this interrupt.
+        curses.ungetch(key)
 
-	ql.os.stdscr.timeout(-1)
-	curses.nl()
+    ql.os.stdscr.timeout(-1)
+    curses.nl()
 
 def handler(ql: Qiling):
-	ah = ql.arch.regs.ah
+    ah = ql.arch.regs.ah
 
-	leaffunc = {
-		0x00 : __leaf_00,
-		0x01 : __leaf_01
-	}.get(ah)
-
-	if leaffunc is None:
-		ql.log.exception(f'leaf {ah:02x}h of INT 16h is not implemented')
-		raise NotImplementedError()
+    leaffunc = {
+        0x00 : __leaf_00,
+        0x01 : __leaf_01
+    }.get(ah)
+
+    if leaffunc is None:
+        ql.log.exception(f'leaf {ah:02x}h of INT 16h is not implemented')
+        raise NotImplementedError()
 
-	leaffunc(ql)
+    leaffunc(ql)
```

### Comparing `qiling-1.4.5/qiling/os/dos/utils.py` & `qiling-1.4.6/qiling/os/dos/utils.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/os/fcall.py` & `qiling-1.4.6/qiling/os/fcall.py`

 * *Files 20% similar despite different names*

```diff
@@ -15,198 +15,198 @@
 CallHook = Callable[[Qiling, int, Mapping], int]
 OnEnterHook = Callable[[Qiling, int, Mapping], Tuple[int, Mapping]]
 OnExitHook = Callable[[Qiling, int, Mapping, int], int]
 
 TypedArg = Tuple[Any, str, Any]
 
 class QlFunctionCall:
-	def __init__(self, ql: Qiling, cc: QlCC, accessors: Mapping[int, Accessor] = {}) -> None:
-		"""Initialize function call handler.
+    def __init__(self, ql: Qiling, cc: QlCC, accessors: Mapping[int, Accessor] = {}) -> None:
+        """Initialize function call handler.
 
-		Args:
-			ql: qiling instance
-			cc: calling convention instance to handle the call
-			accessors: a mapping of parameter types to methods that read and write their values (optional)
-		"""
+        Args:
+            ql: qiling instance
+            cc: calling convention instance to handle the call
+            accessors: a mapping of parameter types to methods that read and write their values (optional)
+        """
 
-		self.ql = ql
-		self.cc = cc
+        self.ql = ql
+        self.cc = cc
 
-		def __make_accessor(nbits: int) -> Accessor:
-			reader = lambda si: cc.getRawParam(si, nbits)
-			writer = lambda si, val: cc.setRawParam(si, val, nbits)
-			nslots = cc.getNumSlots(nbits)
+        def __make_accessor(nbits: int) -> Accessor:
+            reader = lambda si: cc.getRawParam(si, nbits)
+            writer = lambda si, val: cc.setRawParam(si, val, nbits)
+            nslots = cc.getNumSlots(nbits)
 
-			return (reader, writer, nslots)
+            return (reader, writer, nslots)
 
-		# default parameter accessors: readers, writers and slots count
-		self.accessors: MutableMapping[int, Accessor] = {
-			PARAM_INT8 : __make_accessor(8),
-			PARAM_INT16: __make_accessor(16),
-			PARAM_INT32: __make_accessor(32),
-			PARAM_INT64: __make_accessor(64),
-			PARAM_INTN : __make_accessor(0)
-		}
+        # default parameter accessors: readers, writers and slots count
+        self.accessors: MutableMapping[int, Accessor] = {
+            PARAM_INT8 : __make_accessor(8),
+            PARAM_INT16: __make_accessor(16),
+            PARAM_INT32: __make_accessor(32),
+            PARAM_INT64: __make_accessor(64),
+            PARAM_INTN : __make_accessor(0)
+        }
 
-		# let the user override default accessors or add custom ones
-		self.accessors.update(accessors)
+        # let the user override default accessors or add custom ones
+        self.accessors.update(accessors)
 
-	def readEllipsis(self, ptypes: Sequence[Any]) -> Iterator[int]:
-		"""
-		"""
+    def readEllipsis(self, ptypes: Sequence[Any]) -> Iterator[int]:
+        """
+        """
 
-		default = self.accessors[PARAM_INTN]
+        default = self.accessors[PARAM_INTN]
 
-		# count skipped slots
-		si = sum(self.accessors.get(typ, default)[2] for typ in ptypes)
+        # count skipped slots
+        si = sum(self.accessors.get(typ, default)[2] for typ in ptypes)
 
-		while True:
-			read, _, nslots = default
+        while True:
+            read, _, nslots = default
 
-			yield read(si)
-			si += nslots
+            yield read(si)
+            si += nslots
 
-	def readParams(self, ptypes: Sequence[Any]) -> Sequence[int]:
-		"""Walk the function parameters list and get their values.
+    def readParams(self, ptypes: Sequence[Any]) -> Sequence[int]:
+        """Walk the function parameters list and get their values.
 
-		Args:
-			ptypes: a sequence of parameters types to read
+        Args:
+            ptypes: a sequence of parameters types to read
 
-		Returns: parameters raw values
-		"""
+        Returns: parameters raw values
+        """
 
-		default = self.accessors[PARAM_INTN]
+        default = self.accessors[PARAM_INTN]
 
-		si = 0
-		values = []
+        si = 0
+        values = []
 
-		for typ in ptypes:
-			read, _, nslots = self.accessors.get(typ, default)
+        for typ in ptypes:
+            read, _, nslots = self.accessors.get(typ, default)
 
-			val = read(si)
-			si += nslots
+            val = read(si)
+            si += nslots
 
-			values.append(val)
+            values.append(val)
 
-		return values
+        return values
 
-	def writeParams(self, params: Sequence[Tuple[Any, int]]) -> None:
-		"""Walk the function parameters list and set their values.
+    def writeParams(self, params: Sequence[Tuple[Any, int]]) -> None:
+        """Walk the function parameters list and set their values.
 
-		Args:
-			params: a sequence of 2-tuples containing parameters types and values
-		"""
+        Args:
+            params: a sequence of 2-tuples containing parameters types and values
+        """
 
-		default = self.accessors[PARAM_INTN]
+        default = self.accessors[PARAM_INTN]
 
-		si = 0
+        si = 0
 
-		for typ, val in params:
-			_, write, nslots = self.accessors.get(typ, default)
+        for typ, val in params:
+            _, write, nslots = self.accessors.get(typ, default)
 
-			write(si, val)
-			si += nslots
+            write(si, val)
+            si += nslots
 
-	def __count_slots(self, ptypes: Iterable[Any]) -> int:
-		default = self.accessors[PARAM_INTN]
+    def __count_slots(self, ptypes: Iterable[Any]) -> int:
+        default = self.accessors[PARAM_INTN]
 
-		return sum(self.accessors.get(typ, default)[2] for typ in ptypes)
+        return sum(self.accessors.get(typ, default)[2] for typ in ptypes)
 
-	@staticmethod
-	def __get_typed_args(proto: Mapping[str, Any], args: Mapping[str, Any]) -> Iterable[TypedArg]:
-		types = list(proto.values())
-		names = list(args.keys())
-		values = list(args.values())
+    @staticmethod
+    def __get_typed_args(proto: Mapping[str, Any], args: Mapping[str, Any]) -> Iterable[TypedArg]:
+        types = list(proto.values())
+        names = list(args.keys())
+        values = list(args.values())
 
-		# variadic functions are invoked with unknown set of arguments which
-		# do not explicitly appear in prototype (there is an ellipsis instead).
-		#
-		# when a hooked variadic function is called, it updates the arguments
-		# mapping with the additional arguments it was given. that makes the
-		# arguments mapping longer than the prototype mapping; in other words:
-		# at this point we may have more values and names than types.
-		#
-		# here we expand the types list to meet names length, in such a case.
-		if len(names) > len(types):
-			types.extend([None] * (len(names) - len(types)))
+        # variadic functions are invoked with unknown set of arguments which
+        # do not explicitly appear in prototype (there is an ellipsis instead).
+        #
+        # when a hooked variadic function is called, it updates the arguments
+        # mapping with the additional arguments it was given. that makes the
+        # arguments mapping longer than the prototype mapping; in other words:
+        # at this point we may have more values and names than types.
+        #
+        # here we expand the types list to meet names length, in such a case.
+        if len(names) > len(types):
+            types.extend([None] * (len(names) - len(types)))
 
-		return tuple(zip(types, names, values))
+        return tuple(zip(types, names, values))
 
-	def call(self, func: CallHook, proto: Mapping[str, Any], params: Mapping[str, Any], hook_onenter: Optional[OnEnterHook], hook_onexit: Optional[OnExitHook], passthru: bool) -> Tuple[Iterable[TypedArg], int, int]:
-		"""Execute a hooked function.
+    def call(self, func: CallHook, proto: Mapping[str, Any], params: Mapping[str, Any], hook_onenter: Optional[OnEnterHook], hook_onexit: Optional[OnExitHook], passthru: bool) -> Tuple[Iterable[TypedArg], int, int]:
+        """Execute a hooked function.
 
-		Args:
-			func: function hook
-			proto: function's parameters types list
-			params: a mapping of parameter names to their values 
-			hook_onenter: a hook to call before entering function hook
-			hook_onexit: a hook to call after returning from function hook
-			passthru: whether to skip stack frame unwinding
+        Args:
+            func: function hook
+            proto: function's parameters types list
+            params: a mapping of parameter names to their values 
+            hook_onenter: a hook to call before entering function hook
+            hook_onexit: a hook to call after returning from function hook
+            passthru: whether to skip stack frame unwinding
 
-		Returns: resolved params mapping, return value, return address
-		"""
+        Returns: resolved params mapping, return value, return address
+        """
 
-		ql = self.ql
-		pc = ql.arch.regs.arch_pc
+        ql = self.ql
+        pc = ql.arch.regs.arch_pc
 
-		# if set, fire up the on-enter hook and let it override original args set
-		if hook_onenter:
-			overrides = hook_onenter(ql, pc, params)
+        # if set, fire up the on-enter hook and let it override original args set
+        if hook_onenter:
+            overrides = hook_onenter(ql, pc, params)
 
-			if overrides is not None:
-				pc, params = overrides
+            if overrides is not None:
+                pc, params = overrides
 
-		# call function
-		retval = func(ql, pc, params)
+        # call function
+        retval = func(ql, pc, params)
 
-		# if set, fire up the on-exit hook and let it override the return value
-		if hook_onexit:
-			override = hook_onexit(ql, pc, params, retval)
+        # if set, fire up the on-exit hook and let it override the return value
+        if hook_onexit:
+            override = hook_onexit(ql, pc, params, retval)
 
-			if override is not None:
-				retval = override
+            if override is not None:
+                retval = override
 
-		# set return value
-		if retval is not None:
-			self.cc.setReturnValue(retval)
+        # set return value
+        if retval is not None:
+            self.cc.setReturnValue(retval)
 
-		targs = QlFunctionCall.__get_typed_args(proto, params)
+        targs = QlFunctionCall.__get_typed_args(proto, params)
 
-		# TODO: resolve return value
+        # TODO: resolve return value
 
-		# unwind stack frame; note that function prototype sometimes does not
-		# reflect the actual number of arguments passed to the function, like
-		# in variadic functions (e.g. printf-like functions). in such case the
-		# function frame would not be unwinded entirely and cause the program
-		# to fail or produce funny results.
-		# 
-		# nevertheless this type of functions never unwind their own frame,
-		# exactly for the reason they are not aware of the actual number of
-		# arguments they got. since the caller is responsible for unwinding
-		# we should be good.
+        # unwind stack frame; note that function prototype sometimes does not
+        # reflect the actual number of arguments passed to the function, like
+        # in variadic functions (e.g. printf-like functions). in such case the
+        # function frame would not be unwinded entirely and cause the program
+        # to fail or produce funny results.
+        # 
+        # nevertheless this type of functions never unwind their own frame,
+        # exactly for the reason they are not aware of the actual number of
+        # arguments they got. since the caller is responsible for unwinding
+        # we should be good.
 
-		nslots = self.__count_slots(proto.values())
-		retaddr = -1 if passthru else self.cc.unwind(nslots)
+        nslots = self.__count_slots(proto.values())
+        retaddr = -1 if passthru else self.cc.unwind(nslots)
 
-		return targs, retval, retaddr
+        return targs, retval, retaddr
 
-	def call_native(self, addr: int, args: Sequence[Tuple[Any, int]], ret: Optional[int]) -> None:
-		"""Call a native function after properly staging its arguments and return address.
+    def call_native(self, addr: int, args: Sequence[Tuple[Any, int]], ret: Optional[int]) -> None:
+        """Call a native function after properly staging its arguments and return address.
 
-		Args:
-			addr: function entry point
-			args: a sequence of 2-tuples containing parameters types and values to pass to the function; may be empty
-			ret: return address; may be None
-		"""
+        Args:
+            addr: function entry point
+            args: a sequence of 2-tuples containing parameters types and values to pass to the function; may be empty
+            ret: return address; may be None
+        """
 
-		# reserve slots for arguments
-		nslots = self.__count_slots(atype for atype, _ in args)
-		self.cc.reserve(nslots)
+        # reserve slots for arguments
+        nslots = self.__count_slots(atype for atype, _ in args)
+        self.cc.reserve(nslots)
 
-		if ret is not None:
-			self.cc.setReturnAddress(ret)
+        if ret is not None:
+            self.cc.setReturnAddress(ret)
 
-		# set arguments values
-		self.writeParams(args)
+        # set arguments values
+        self.writeParams(args)
 
-		# call
-		self.ql.arch.regs.arch_pc = addr
+        # call
+        self.ql.arch.regs.arch_pc = addr
```

### Comparing `qiling-1.4.5/qiling/os/freebsd/const.py` & `qiling-1.4.6/qiling/os/freebsd/const.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/os/freebsd/freebsd.py` & `qiling-1.4.6/qiling/os/freebsd/freebsd.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,48 +1,45 @@
 #!/usr/bin/env python3
-# 
+#
 # Cross Platform and Multi Architecture Advanced Binary Emulation Framework
 #
 
 from unicorn import UcError
 from unicorn.x86_const import UC_X86_INS_SYSCALL
 
 from qiling.arch.x86_utils import GDTManager, SegmentManager86
 from qiling.const import QL_OS
 from qiling.os.posix.posix import QlOsPosix
 
+
 class QlOsFreebsd(QlOsPosix):
     type = QL_OS.FREEBSD
 
     def __init__(self, ql):
         super(QlOsFreebsd, self).__init__(ql)
 
-        self.elf_mem_start = 0x0
         self.load()
 
-
     def load(self):
         gdtm = GDTManager(self.ql)
 
         # setup gdt and segments selectors
         segm = SegmentManager86(self.ql.arch, gdtm)
         segm.setup_cs_ds_ss_es(0, 4 << 30)
 
         self.ql.hook_insn(self.hook_syscall, UC_X86_INS_SYSCALL)
 
-
     def hook_syscall(self, ql):
         return self.load_syscall()
 
-
     def run(self):
         if self.ql.exit_point is not None:
             self.exit_point = self.ql.exit_point
 
-        if  self.ql.entry_point is not None:
+        if self.ql.entry_point is not None:
             self.ql.loader.elf_entry = self.ql.entry_point
 
         try:
             if self.ql.code:
                 self.ql.emu_start(self.entry_point, (self.entry_point + len(self.ql.code)), self.ql.timeout, self.ql.count)
             else:
                 if self.ql.loader.elf_entry != self.ql.loader.entry_point:
```

### Comparing `qiling-1.4.5/qiling/os/freebsd/map_syscall.py` & `qiling-1.4.6/qiling/os/freebsd/map_syscall.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/os/freebsd/syscall.py` & `qiling-1.4.6/qiling/os/freebsd/syscall.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/os/linux/fncc.py` & `qiling-1.4.6/qiling/os/linux/fncc.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/os/linux/function_hook.py` & `qiling-1.4.6/qiling/os/linux/function_hook.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,47 +5,47 @@
 
 import struct
 
 
 from qiling.const import *
 
 PT_DYNAMIC      = 2
-DT_NULL 		= 0
-DT_NEEDED 		= 1
-DT_PLTRELSZ 	= 2
-DT_PLTGOT 		= 3
-DT_HASH 		= 4
-DT_STRTAB 		= 5
-DT_SYMTAB 		= 6
-DT_RELA 		= 7
-DT_RELASZ 		= 8
-DT_RELAENT 		= 9
-DT_STRSZ 		= 10
-DT_SYMENT 		= 11
-DT_INIT 		= 12
-DT_FINI 		= 13
-DT_SONAME 		= 14
-DT_RPATH 		= 15
-DT_SYMBOLIC 	= 16
-DT_REL 			= 17
-DT_RELSZ 		= 18
-DT_RELENT 		= 19
-DT_PLTREL 		= 20
-DT_DEBUG 		= 21
-DT_TEXTREL 		= 22
-DT_JMPREL 		= 23
-DT_BIND_NOW 	= 24
-DT_INIT_ARRAY 	= 25
-DT_FINI_ARRAY 	= 26
+DT_NULL         = 0
+DT_NEEDED         = 1
+DT_PLTRELSZ     = 2
+DT_PLTGOT         = 3
+DT_HASH         = 4
+DT_STRTAB         = 5
+DT_SYMTAB         = 6
+DT_RELA         = 7
+DT_RELASZ         = 8
+DT_RELAENT         = 9
+DT_STRSZ         = 10
+DT_SYMENT         = 11
+DT_INIT         = 12
+DT_FINI         = 13
+DT_SONAME         = 14
+DT_RPATH         = 15
+DT_SYMBOLIC     = 16
+DT_REL             = 17
+DT_RELSZ         = 18
+DT_RELENT         = 19
+DT_PLTREL         = 20
+DT_DEBUG         = 21
+DT_TEXTREL         = 22
+DT_JMPREL         = 23
+DT_BIND_NOW     = 24
+DT_INIT_ARRAY     = 25
+DT_FINI_ARRAY     = 26
 DT_INIT_ARRAYSZ = 27
 DT_FINI_ARRAYSZ = 28
-DT_RUNPATH 		= 29
-DT_FLAGS 		= 30
-DT_ENCODING 	= 32
-DT_GNU_HASH	    = 0x6ffffef5
+DT_RUNPATH         = 29
+DT_FLAGS         = 30
+DT_ENCODING     = 32
+DT_GNU_HASH        = 0x6ffffef5
 
 DT_MIPS_LOCAL_GOTNO = 0x7000000a
 DT_MIPS_SYMTABNO = 0x70000011
 DT_MIPS_GOTSYM = 0x70000013
 
 class HookFunc:
     def __init__(self, ql, fn):
@@ -634,22 +634,22 @@
         self.use_list = {}
         self.hook_list = {}
 
         self.hook_int = False
 
     def parse_program_header32(self):
         # typedef struct elf32_phdr{
-        # Elf32_Word	p_type;
-        # Elf32_Off	p_offset;
-        # Elf32_Addr	p_vaddr;
-        # Elf32_Addr	p_paddr;
-        # Elf32_Word	p_filesz;
-        # Elf32_Word	p_memsz;
-        # Elf32_Word	p_flags;
-        # Elf32_Word	p_align;
+        # Elf32_Word    p_type;
+        # Elf32_Off    p_offset;
+        # Elf32_Addr    p_vaddr;
+        # Elf32_Addr    p_paddr;
+        # Elf32_Word    p_filesz;
+        # Elf32_Word    p_memsz;
+        # Elf32_Word    p_flags;
+        # Elf32_Word    p_align;
         # } Elf32_Phdr;
 
         # /* 32-bit ELF base types. */
         # typedef uint32_t Elf32_Addr;
         # typedef uint16_t Elf32_Half;
         # typedef uint32_t Elf32_Off;
         # typedef int32_t  Elf32_Sword;
@@ -665,28 +665,28 @@
             yield P
         return
 
     def parse_program_header64(self):
         # typedef struct elf64_phdr {
         # Elf64_Word p_type;
         # Elf64_Word p_flags;
-        # Elf64_Off p_offset;		/* Segment file offset */
-        # Elf64_Addr p_vaddr;		/* Segment virtual address */
-        # Elf64_Addr p_paddr;		/* Segment physical address */
-        # Elf64_Xword p_filesz;		/* Segment size in file */
-        # Elf64_Xword p_memsz;		/* Segment size in memory */
-        # Elf64_Xword p_align;		/* Segment alignment, file & memory */
+        # Elf64_Off p_offset;        /* Segment file offset */
+        # Elf64_Addr p_vaddr;        /* Segment virtual address */
+        # Elf64_Addr p_paddr;        /* Segment physical address */
+        # Elf64_Xword p_filesz;        /* Segment size in file */
+        # Elf64_Xword p_memsz;        /* Segment size in memory */
+        # Elf64_Xword p_align;        /* Segment alignment, file & memory */
         # } Elf64_Phdr;
 
         # /* 64-bit ELF base types. */
         # typedef uint64_t Elf64_Addr;
         # typedef uint16_t Elf64_Half;
-        # typedef int16_t	 Elf64_SHalf;
+        # typedef int16_t     Elf64_SHalf;
         # typedef uint64_t Elf64_Off;
-        # typedef int32_t	 Elf64_Sword;
+        # typedef int32_t     Elf64_Sword;
         # typedef uint32_t Elf64_Word;
         # typedef uint64_t Elf64_Xword;
         # typedef int64_t  Elf64_Sxword;
 
         Psize = int(self.phentsize)
         Pnum = int(self.phnum)
         Pdata = self.ql.mem.read(self.phoff, Pnum * Psize)
@@ -702,28 +702,28 @@
             return self.parse_program_header64()
         elif self.ql.arch.bits == 32:
             return self.parse_program_header32()
 
     def parse_dynamic64(self):
         # typedef struct
         # {
-        # Elf64_Sxword	d_tag;			/* Dynamic entry type */
+        # Elf64_Sxword    d_tag;            /* Dynamic entry type */
         # union
         #     {
-        #     Elf64_Xword d_val;		/* Integer value */
-        #     Elf64_Addr d_ptr;			/* Address value */
+        #     Elf64_Xword d_val;        /* Integer value */
+        #     Elf64_Addr d_ptr;            /* Address value */
         #     } d_un;
         # } Elf64_Dyn;
 
         # /* 64-bit ELF base types. */
         # typedef uint64_t Elf64_Addr;
         # typedef uint16_t Elf64_Half;
-        # typedef int16_t	 Elf64_SHalf;
+        # typedef int16_t     Elf64_SHalf;
         # typedef uint64_t Elf64_Off;
-        # typedef int32_t	 Elf64_Sword;
+        # typedef int32_t     Elf64_Sword;
         # typedef uint32_t Elf64_Word;
         # typedef uint64_t Elf64_Xword;
         # typedef int64_t  Elf64_Sxword;
 
         Dsize = ELF64_Dyn.Dyn_SIZE
         idx = 0
 
@@ -735,19 +735,19 @@
             if D.d_tag == DT_NULL:
                 break
         return
     
     def parse_dynamic32(self):
         # typedef struct
         # {
-        # Elf32_Sword	d_tag;			/* Dynamic entry type */
+        # Elf32_Sword    d_tag;            /* Dynamic entry type */
         # union
         #     {
-        #     Elf32_Word d_val;			/* Integer value */
-        #     Elf32_Addr d_ptr;			/* Address value */
+        #     Elf32_Word d_val;            /* Integer value */
+        #     Elf32_Addr d_ptr;            /* Address value */
         #     } d_un;
         # } Elf32_Dyn;
 
         # /* 32-bit ELF base types. */
         # typedef uint32_t Elf32_Addr;
         # typedef uint16_t Elf32_Half;
         # typedef uint32_t Elf32_Off;
```

### Comparing `qiling-1.4.5/qiling/os/linux/futex.py` & `qiling-1.4.6/qiling/os/linux/futex.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/os/linux/kernel_api/hook.py` & `qiling-1.4.6/qiling/os/linux/kernel_api/hook.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/os/linux/kernel_api/kernel_api.py` & `qiling-1.4.6/qiling/os/linux/kernel_api/kernel_api.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/os/linux/linux.py` & `qiling-1.4.6/qiling/os/linux/linux.py`

 * *Files 14% similar despite different names*

```diff
@@ -44,15 +44,14 @@
 
         self.fcall = QlFunctionCall(ql, cc)
 
         self.thread_class = None
         self.futexm = None
         self.fh = None
         self.function_after_load_list = []
-        self.elf_mem_start = 0x0
         self.load()
 
     def load(self):
         self.futexm = futex.QlLinuxFutexManagement()
 
         # ARM
         if self.ql.arch.type == QL_ARCH.ARM:
@@ -114,23 +113,30 @@
         elif self.ql.arch.type == QL_ARCH.PPC:
             self.ql.arch.enable_float()
             self.ql.hook_intno(self.hook_syscall, 8)
             self.thread_class = None
 
         # on fork or execve, do not inherit opened files tagged as 'close on exec'
         for i in range(len(self.fd)):
-            if getattr(self.fd[i], 'close_on_exec', 0):
+            if getattr(self.fd[i], 'close_on_exec', False):
                 self.fd[i] = None
 
     def setup_procfs(self):
-        self.fs_mapper.add_fs_mapping(r'/proc/self/auxv',    partial(QlProcFS.self_auxv, self))
-        self.fs_mapper.add_fs_mapping(r'/proc/self/cmdline', partial(QlProcFS.self_cmdline, self))
-        self.fs_mapper.add_fs_mapping(r'/proc/self/environ', partial(QlProcFS.self_environ, self))
-        self.fs_mapper.add_fs_mapping(r'/proc/self/exe',     partial(QlProcFS.self_exe, self))
-        self.fs_mapper.add_fs_mapping(r'/proc/self/maps',    partial(QlProcFS.self_map, self.ql.mem))
+        files = (
+            (r'/proc/self/auxv',    lambda: partial(QlProcFS.self_auxv, self)),
+            (r'/proc/self/cmdline', lambda: partial(QlProcFS.self_cmdline, self)),
+            (r'/proc/self/environ', lambda: partial(QlProcFS.self_environ, self)),
+            (r'/proc/self/exe',     lambda: partial(QlProcFS.self_exe, self)),
+            (r'/proc/self/maps',    lambda: partial(QlProcFS.self_map, self.ql.mem))
+        )
+
+        for filename, wrapper in files:
+            # add mapping only if the user has not already mapped it
+            if not self.fs_mapper.has_mapping(filename):
+                self.fs_mapper.add_mapping(filename, wrapper())
 
     def hook_syscall(self, ql, intno = None):
         return self.load_syscall()
 
     def register_function_after_load(self, function):
         if function not in self.function_after_load_list:
             self.function_after_load_list.append(function)
@@ -157,20 +163,22 @@
                     self.ql.os.thread_management = thread_management
                     thread_management.run()
 
                 else:
                     if self.ql.entry_point is not None:
                         self.ql.loader.elf_entry = self.ql.entry_point
 
+                    # do we have an interp?
                     elif self.ql.loader.elf_entry != self.ql.loader.entry_point:
                         entry_address = self.ql.loader.elf_entry
 
                         if self.ql.arch.type == QL_ARCH.ARM:
                             entry_address &= ~1
 
+                        # start running interp, but stop when elf entry point is reached
                         self.ql.emu_start(self.ql.loader.entry_point, entry_address, self.ql.timeout)
                         self.ql.do_lib_patch()
                         self.run_function_after_load()
                         self.ql.loader.skip_exit_check = False
                         self.ql.write_exit_trap()
 
                     self.ql.emu_start(self.ql.loader.elf_entry, self.exit_point, self.ql.timeout, self.ql.count)
```

### Comparing `qiling-1.4.5/qiling/os/linux/procfs.py` & `qiling-1.4.6/qiling/os/linux/procfs.py`

 * *Files 27% similar despite different names*

```diff
@@ -12,14 +12,18 @@
 class FsMappedStream(io.BytesIO):
     """Wrap stream objects to make them look like a QlFsMappedObject.
     """
 
     def __init__(self, fname: str, *args) -> None:
         super().__init__(*args)
 
+        # note that the name property should reflect the actual file name
+        # on the host file system, and here we get a virtual file name
+        # instead. we should be fine, however, since there is no file
+        # backing this object anyway
         self.name = fname
 
 
 class QlProcFS:
 
     @staticmethod
     def self_auxv(os: 'QlOsLinux') -> QlFsMappedObject:
@@ -38,24 +42,24 @@
             auxv_data.extend(os.ql.mem.read(auxv_addr, nbytes))
             auxv_addr += nbytes
 
         return FsMappedStream(r'/proc/self/auxv', auxv_data)
 
     @staticmethod
     def self_cmdline(os: 'QlOsLinux') -> QlFsMappedObject:
-        entries = (arg.encode('utf-8') for arg in os.ql.argv)
+        entries = (arg.encode('latin') for arg in os.ql.argv)
         cmdline = b'\x00'.join(entries) + b'\x00'
 
         return FsMappedStream(r'/proc/self/cmdline', cmdline)
 
     @staticmethod
     def self_environ(os: 'QlOsLinux') -> QlFsMappedObject:
         def __to_bytes(s: AnyStr) -> bytes:
             if isinstance(s, str):
-                return s.encode('utf-8')
+                return s.encode('latin')
 
             return s
 
         entries = (b'='.join((__to_bytes(k), __to_bytes(v))) for k, v in os.ql.env.items())
         environ = b'\x00'.join(entries) + b'\x00'
 
         return FsMappedStream(r'/proc/self/environ', environ)
@@ -69,10 +73,10 @@
 
     @staticmethod
     def self_map(mem: 'QlMemoryManager') -> QlFsMappedObject:
         content = bytearray()
         mapinfo = mem.get_mapinfo()
 
         for lbound, ubound, perms, label, container in mapinfo:
-            content += f"{lbound:x}-{ubound:x}\t{perms}p\t0\t00:00\t0\t{container if container else label}\n".encode("utf-8")
+            content += f"{lbound:x}-{ubound:x}\t{perms}p\t0\t00:00\t0\t{container if container else label}\n".encode("latin")
 
         return FsMappedStream(r'/proc/self/map', content)
```

### Comparing `qiling-1.4.5/qiling/os/linux/syscall.py` & `qiling-1.4.6/qiling/os/linux/syscall.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #!/usr/bin/env python3
-# 
+#
 # Cross Platform and Multi Architecture Advanced Binary Emulation Framework
 #
 
 from qiling import Qiling
 from qiling.arch.x86_const import *
 from qiling.const import QL_ARCH
 
@@ -44,15 +44,15 @@
 
         ql.log.debug("set_thread_area base : 0x%x limit is : 0x%x" % (base, limit))
 
         if index == -1:
             index = ql.os.gdtm.get_free_idx(12)
 
         if index in (12, 13, 14):
-            access = QL_X86_A_PRESENT | QL_X86_A_DATA | QL_X86_A_DATA_WRITABLE | QL_X86_A_PRIV_3 | QL_X86_A_DIR_CON_BIT
+            access = QL_X86_A_PRESENT | QL_X86_A_PRIV_3 | QL_X86_A_DESC_DATA | QL_X86_A_DATA | QL_X86_A_DATA_E | QL_X86_A_DATA_W
 
             ql.os.gdtm.register_gdt_segment(index, base, limit, access)
             ql.mem.write_ptr(u_info_addr, index, 4)
         else:
             ql.log.warning(f"Wrong index {index} from address {hex(u_info_addr)}")
             return -1
```

### Comparing `qiling-1.4.5/qiling/os/linux/thread.py` & `qiling-1.4.6/qiling/os/linux/thread.py`

 * *Files 2% similar despite different names*

```diff
@@ -379,15 +379,15 @@
         base = self.ql.unpack32(u_info[4 : 8])
         limit = self.ql.unpack32(u_info[8 : 12])
 
         if index == -1:
             index = self.ql.os.gdtm.get_free_idx(12)
 
         if index in (12, 13, 14):
-            access = QL_X86_A_PRESENT | QL_X86_A_DATA | QL_X86_A_DATA_WRITABLE | QL_X86_A_PRIV_3 | QL_X86_A_DIR_CON_BIT
+            access = QL_X86_A_PRESENT | QL_X86_A_PRIV_3 | QL_X86_A_DESC_DATA | QL_X86_A_DATA | QL_X86_A_DATA_E | QL_X86_A_DATA_W
 
             self.ql.os.gdtm.register_gdt_segment(index, base, limit, access)
             self.ql.mem.write_ptr(tls_addr, index, 4)
         else:
             raise
 
         self.tls = self.__read_tls()
```

### Comparing `qiling-1.4.5/qiling/os/macos/__init__.py` & `qiling-1.4.6/qiling/os/macos/__init__.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/os/macos/const.py` & `qiling-1.4.6/qiling/os/macos/const.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # 
 # Cross Platform and Multi Architecture Advanced Binary Emulation Framework
 #
 
 # basic values
 PAGE_SIZE                   = 0x1000
 VMMAP_PAGE_SIZE             = 0x100000
-MAX_FD_SIZE					= 0xFF
+MAX_FD_SIZE                    = 0xFF
 MAX_PATH_SIZE               = 0x800
 
 # GS
 MSR_KERNEL_GS_BASE          = 0xc0000102
 
 # kernel flags
 KERN_SUCCESS                = 0
@@ -72,69 +72,69 @@
 CPU_ARCH_ABI64      =   0x01000000
 CPU_TYPE_X86        =   7
 CPU_TYPE_I386       =   CPU_TYPE_X86
 CPU_TYPE_X86_64     =   CPU_ARCH_ABI64 | CPU_TYPE_X86
 
 # mach mag flags
 MACH_MSG_SUCCESS                =   0x00000000
-MACH_MSG_MASK			        =   0x00003e00
-MACH_MSG_IPC_SPACE		        =   0x00002000
-MACH_MSG_VM_SPACE		        =   0x00001000
-MACH_MSG_IPC_KERNEL		        =   0x00000800
-MACH_MSG_VM_KERNEL		        =   0x00000400
-MACH_SEND_IN_PROGRESS		    =   0x10000001
-MACH_SEND_INVALID_DATA		    =   0x10000002
-MACH_SEND_INVALID_DEST		    =   0x10000003
-MACH_SEND_TIMED_OUT		        =   0x10000004
-MACH_SEND_INVALID_VOUCHER	    =   0x10000005
-MACH_SEND_INTERRUPTED		    =   0x10000007
-MACH_SEND_MSG_TOO_SMALL		    =   0x10000008
-MACH_SEND_INVALID_REPLY		    =   0x10000009
-MACH_SEND_INVALID_RIGHT		    =   0x1000000a
-MACH_SEND_INVALID_NOTIFY	    =   0x1000000b
-MACH_SEND_INVALID_MEMORY	    =   0x1000000c
-MACH_SEND_NO_BUFFER		        =   0x1000000d
-MACH_SEND_TOO_LARGE		        =   0x1000000e
-MACH_SEND_INVALID_TYPE		    =   0x1000000f
-MACH_SEND_INVALID_HEADER	    =   0x10000010
-MACH_SEND_INVALID_TRAILER	    =   0x10000011
-MACH_SEND_INVALID_RT_OOL_SIZE	=   0x10000015
-MACH_RCV_IN_PROGRESS		    =   0x10004001
-MACH_RCV_INVALID_NAME		    =   0x10004002
-MACH_RCV_TIMED_OUT		        =   0x10004003
-MACH_RCV_TOO_LARGE		        =   0x10004004
-MACH_RCV_INTERRUPTED		    =   0x10004005
-MACH_RCV_PORT_CHANGED		    =   0x10004006
-MACH_RCV_INVALID_NOTIFY		    =   0x10004007
-MACH_RCV_INVALID_DATA		    =   0x10004008
-MACH_RCV_PORT_DIED		        =   0x10004009
-MACH_RCV_IN_SET			        =   0x1000400a
-MACH_RCV_HEADER_ERROR		    =   0x1000400b
-MACH_RCV_BODY_ERROR		        =   0x1000400c
-MACH_RCV_INVALID_TYPE		    =   0x1000400d
-MACH_RCV_SCATTER_SMALL		    =   0x1000400e
-MACH_RCV_INVALID_TRAILER	    =   0x1000400f
+MACH_MSG_MASK                    =   0x00003e00
+MACH_MSG_IPC_SPACE                =   0x00002000
+MACH_MSG_VM_SPACE                =   0x00001000
+MACH_MSG_IPC_KERNEL                =   0x00000800
+MACH_MSG_VM_KERNEL                =   0x00000400
+MACH_SEND_IN_PROGRESS            =   0x10000001
+MACH_SEND_INVALID_DATA            =   0x10000002
+MACH_SEND_INVALID_DEST            =   0x10000003
+MACH_SEND_TIMED_OUT                =   0x10000004
+MACH_SEND_INVALID_VOUCHER        =   0x10000005
+MACH_SEND_INTERRUPTED            =   0x10000007
+MACH_SEND_MSG_TOO_SMALL            =   0x10000008
+MACH_SEND_INVALID_REPLY            =   0x10000009
+MACH_SEND_INVALID_RIGHT            =   0x1000000a
+MACH_SEND_INVALID_NOTIFY        =   0x1000000b
+MACH_SEND_INVALID_MEMORY        =   0x1000000c
+MACH_SEND_NO_BUFFER                =   0x1000000d
+MACH_SEND_TOO_LARGE                =   0x1000000e
+MACH_SEND_INVALID_TYPE            =   0x1000000f
+MACH_SEND_INVALID_HEADER        =   0x10000010
+MACH_SEND_INVALID_TRAILER        =   0x10000011
+MACH_SEND_INVALID_RT_OOL_SIZE    =   0x10000015
+MACH_RCV_IN_PROGRESS            =   0x10004001
+MACH_RCV_INVALID_NAME            =   0x10004002
+MACH_RCV_TIMED_OUT                =   0x10004003
+MACH_RCV_TOO_LARGE                =   0x10004004
+MACH_RCV_INTERRUPTED            =   0x10004005
+MACH_RCV_PORT_CHANGED            =   0x10004006
+MACH_RCV_INVALID_NOTIFY            =   0x10004007
+MACH_RCV_INVALID_DATA            =   0x10004008
+MACH_RCV_PORT_DIED                =   0x10004009
+MACH_RCV_IN_SET                    =   0x1000400a
+MACH_RCV_HEADER_ERROR            =   0x1000400b
+MACH_RCV_BODY_ERROR                =   0x1000400c
+MACH_RCV_INVALID_TYPE            =   0x1000400d
+MACH_RCV_SCATTER_SMALL            =   0x1000400e
+MACH_RCV_INVALID_TRAILER        =   0x1000400f
 MACH_RCV_IN_PROGRESS_TIMED      =   0x10004011
 
 # CS opetions
-CS_OPS_STATUS		        = 0
-CS_OPS_MARKINVALID	        = 1
-CS_OPS_MARKHARD		        = 2
-CS_OPS_MARKKILL		        = 3
-CS_OPS_CDHASH		        = 5
-CS_OPS_PIDOFFSET	        = 6
+CS_OPS_STATUS                = 0
+CS_OPS_MARKINVALID            = 1
+CS_OPS_MARKHARD                = 2
+CS_OPS_MARKKILL                = 3
+CS_OPS_CDHASH                = 5
+CS_OPS_PIDOFFSET            = 6
 CS_OPS_ENTITLEMENTS_BLOB    = 7
-CS_OPS_MARKRESTRICT	        = 8
-CS_OPS_SET_STATUS	        = 9
-CS_OPS_BLOB		            = 10
-CS_OPS_IDENTITY		        = 11
-CS_OPS_CLEARINSTALLER	    = 12
+CS_OPS_MARKRESTRICT            = 8
+CS_OPS_SET_STATUS            = 9
+CS_OPS_BLOB                    = 10
+CS_OPS_IDENTITY                = 11
+CS_OPS_CLEARINSTALLER        = 12
 CS_OPS_CLEARPLATFORM        = 13
 CS_OPS_TEAMID               = 14
-CS_MAX_TEAMID_LEN	        = 64
+CS_MAX_TEAMID_LEN            = 64
 
 # code signing attributes of a proc
 CS_VALID                    = 0x00000001
 CS_ADHOC                    = 0x00000002
 CS_GET_TASK_ALLOW           = 0x00000004
 CS_INSTALLER                = 0x00000008
 CS_FORCED_LV                = 0x00000010
@@ -160,15 +160,15 @@
 CS_DEBUGGED                 = 0x10000000
 CS_SIGNED                   = 0x20000000
 CS_DEV_CODE                 = 0x40000000
 CS_DATAVAULT_CONTROLLER     = 0x80000000
 CS_ENTITLEMENT_FLAGS        = (CS_GET_TASK_ALLOW | CS_INSTALLER | CS_DATAVAULT_CONTROLLER | CS_NVRAM_UNRESTRICTED)
 
 # executeable segment flags
-CS_EXECSEG_MAIN_BINARY	    = 0x1
+CS_EXECSEG_MAIN_BINARY        = 0x1
 CS_EXECSEG_ALLOW_UNSIGNED   =0x10
 CS_EXECSEG_DEBUGGER         = 0x20
 CS_EXECSEG_JIT              = 0x40
 CS_EXECSEG_SKIP_LV          = 0x80
 CS_EXECSEG_CAN_LOAD_CDHASH  = 0x100
 CS_EXECSEG_CAN_EXEC_CDHASH  = 0x200
 
@@ -185,15 +185,15 @@
 MACH_SEND_ALWAYS            = 0x00010000
 MACH_SEND_TRAILER           = 0x00020000
 MACH_SEND_NOIMPORTANCE      = 0x00040000
 MACH_SEND_NODENAP           = MACH_SEND_NOIMPORTANCE
 MACH_SEND_IMPORTANCE        = 0x00080000
 MACH_SEND_SYNC_OVERRIDE     = 0x00100000
 MACH_SEND_PROPAGATE_QOS     = 0x00200000
-MACH_SEND_SYNC_USE_THRPRI	= MACH_SEND_PROPAGATE_QOS
+MACH_SEND_SYNC_USE_THRPRI    = MACH_SEND_PROPAGATE_QOS
 MACH_SEND_KERNEL            = 0x00400000
 MACH_RCV_TIMEOUT            = 0x00000100
 MACH_RCV_NOTIFY             = 0x00000200
 MACH_RCV_INTERRUPT          = 0x00000400
 MACH_RCV_VOUCHER            = 0x00000800
 MACH_RCV_OVERWRITE          = 0x00001000
 MACH_RCV_SYNC_WAIT          = 0x00004000
@@ -321,18 +321,18 @@
 EPROTO          = 100
 ETIME           = 101
 EOPNOTSUPP      = 102
 ELAST           = 102
 
 
 # shared region 
-SHARED_REGION_BASE_I386	            = 0x90000000
+SHARED_REGION_BASE_I386                = 0x90000000
 SHARED_REGION_SIZE_I386             = 0x20000000
-SHARED_REGION_NESTING_BASE_I386	    = 0x90000000
-SHARED_REGION_NESTING_SIZE_I386	    = 0x20000000
+SHARED_REGION_NESTING_BASE_I386        = 0x90000000
+SHARED_REGION_NESTING_SIZE_I386        = 0x20000000
 SHARED_REGION_NESTING_MIN_I386      = 0x00200000
 SHARED_REGION_NESTING_MAX_I386      = 0xFFE00000
 SHARED_REGION_BASE_X86_64           = 0x00007FFF00000000
 SHARED_REGION_SIZE_X86_64           = 0x00000000FFE00000
 SHARED_REGION_NESTING_BASE_X86_64   = 0x00007FFF00000000
 SHARED_REGION_NESTING_SIZE_X86_64   = 0x00000000FFE00000
 SHARED_REGION_NESTING_MIN_X86_64    = 0x0000000000200000
@@ -499,17 +499,17 @@
 COMM_PAGE_THIS_VERSION              = 13      # in ver 13, _COMM_PAGE_NT_SHIFT defaults to 0 (was 32) 
 
 COMM_PAGE_CPU_CAPABILITIES          = 0x020   # uint32_t _cpu_capabilities (retained for compatibility) */
 COMM_PAGE_NCPUS                     = 0x022   # uint8_t number of configured CPUs (hw.logicalcpu at boot time) */
 COMM_PAGE_UNUSED0                   = 0x024   # 2 unused bytes, previouly reserved for expansion of cpu_capabilities */
 COMM_PAGE_CACHE_LINESIZE            = 0x026   # uint16_t cache line size */
 
-COMM_PAGE_SCHED_GEN                 = 0x028	  # uint32_t scheduler generation number (count of pre-emptions) */
+COMM_PAGE_SCHED_GEN                 = 0x028      # uint32_t scheduler generation number (count of pre-emptions) */
 COMM_PAGE_MEMORY_PRESSURE           = 0x02c   # uint32_t copy of vm_memory_pressure */
-COMM_PAGE_SPIN_COUNT                = 0x030	  # uint32_t max spin count for mutex's */
+COMM_PAGE_SPIN_COUNT                = 0x030      # uint32_t max spin count for mutex's */
 
 COMM_PAGE_ACTIVE_CPUS               = 0x034   # uint8_t number of active CPUs (hw.activecpu) */
 COMM_PAGE_PHYSICAL_CPUS             = 0x035   # uint8_t number of physical CPUs (hw.physicalcpu_max) */
 COMM_PAGE_LOGICAL_CPUS              = 0x036   # uint8_t number of logical CPUs (hw.logicalcpu_max) */
 COMM_PAGE_UNUSED1                   = 0x037   # 1 unused bytes */
 COMM_PAGE_MEMORY_SIZE               = 0x038   # uint64_t max memory size */
```

### Comparing `qiling-1.4.5/qiling/os/macos/events/macos.py` & `qiling-1.4.6/qiling/os/macos/events/macos.py`

 * *Files 1% similar despite different names*

```diff
@@ -578,38 +578,38 @@
         parent_vnode.v_name = POINTER64(tmp_name)
         parent_vnode.updateToMem()
 
         self.emit("KAUTH_VNODE", EV_KAUTH_VNODE, [self.cred.base, 0, action.value, 0, self.vnode.base, tmp_addr])
 
 # arguments passed to KAUTH_FILEOP_OPEN listeners
 #           arg0 is pointer to vnode (vnode *) for given user path.
-# 	    arg1 is pointer to path (char *) passed in to open.
+#         arg1 is pointer to path (char *) passed in to open.
 # arguments passed to KAUTH_FILEOP_CLOSE listeners
 #           arg0 is pointer to vnode (vnode *) for file to be closed.
-# 	    arg1 is pointer to path (char *) of file to be closed.
-# 	    arg2 is close flags.
+#         arg1 is pointer to path (char *) of file to be closed.
+#         arg2 is close flags.
 # arguments passed to KAUTH_FILEOP_WILL_RENAME listeners
-# 	    arg0 is pointer to vnode (vnode *) of the file being renamed
-# 	    arg1 is pointer to the "from" path (char *)
-# 	    arg2 is pointer to the "to" path (char *)
+#         arg0 is pointer to vnode (vnode *) of the file being renamed
+#         arg1 is pointer to the "from" path (char *)
+#         arg2 is pointer to the "to" path (char *)
 # arguments passed to KAUTH_FILEOP_RENAME listeners
-# 	    arg0 is pointer to "from" path (char *).
-# 	    arg1 is pointer to "to" path (char *).
+#         arg0 is pointer to "from" path (char *).
+#         arg1 is pointer to "to" path (char *).
 # arguments passed to KAUTH_FILEOP_EXCHANGE listeners
-# 	    arg0 is pointer to file 1 path (char *).
-# 	    arg1 is pointer to file 2 path (char *).
+#         arg0 is pointer to file 1 path (char *).
+#         arg1 is pointer to file 2 path (char *).
 # arguments passed to KAUTH_FILEOP_LINK listeners
-# 	    arg0 is pointer to path to file we are linking to (char *).
-# 	    arg1 is pointer to path to the new link file (char *).
+#         arg0 is pointer to path to file we are linking to (char *).
+#         arg1 is pointer to path to the new link file (char *).
 # arguments passed to KAUTH_FILEOP_EXEC listeners
-# 	    arg0 is pointer to vnode (vnode *) for executable.
-# 	    arg1 is pointer to path (char *) to executable.
+#         arg0 is pointer to vnode (vnode *) for executable.
+#         arg1 is pointer to path (char *) to executable.
 # arguments passed to KAUTH_FILEOP_DELETE listeners
-# 	    arg0 is pointer to vnode (vnode *) of file/dir that was deleted.
-# 	    arg1 is pointer to path (char *) of file/dir that was deleted.
+#         arg0 is pointer to vnode (vnode *) of file/dir that was deleted.
+#         arg1 is pointer to path (char *) of file/dir that was deleted.
     @init_ev_ctx
     def kauth_fileop(self, action, params={}):
         path = self.ql.os.heap.alloc(len(self.current_proc) + 1)
         self.ql.mem.write(path, self.current_proc.encode() + b"\x00")
         if action == Kauth.KAUTH_FILEOP_OPEN:
             self.emit("KAUTH_FILEOP", MacOSEventType.EV_KAUTH_FILEOP, [self.cred.base, 0, action.value, self.vnode.base, path, 0, 0])
         elif action == Kauth.KAUTH_FILEOP_CLOSE:
```

### Comparing `qiling-1.4.5/qiling/os/macos/events/macos_policy.py` & `qiling-1.4.6/qiling/os/macos/events/macos_policy.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/os/macos/events/macos_structs.py` & `qiling-1.4.6/qiling/os/macos/events/macos_structs.py`

 * *Files 12% similar despite different names*

```diff
@@ -58,24 +58,24 @@
     EV_KAUTH_VNODE = ()
     EV_KAUTH_FILEOP = ()
     EV_IPF_INPUT = ()
     EV_IPF_OUTPUT = ()
     EV_IPF_DETACH = ()
 
 # enum {
-# 	sock_evt_connecting             = 1,
-# 	sock_evt_connected              = 2,
-# 	sock_evt_disconnecting          = 3,
-# 	sock_evt_disconnected           = 4,
-# 	sock_evt_flush_read             = 5,
-# 	sock_evt_shutdown               = 6, /* param points to an integer specifying how (read, write, or both) see man 2 shutdown */
-# 	sock_evt_cantrecvmore           = 7,
-# 	sock_evt_cantsendmore           = 8,
-# 	sock_evt_closing                = 9,
-# 	sock_evt_bound                  = 10
+#     sock_evt_connecting             = 1,
+#     sock_evt_connected              = 2,
+#     sock_evt_disconnecting          = 3,
+#     sock_evt_disconnected           = 4,
+#     sock_evt_flush_read             = 5,
+#     sock_evt_shutdown               = 6, /* param points to an integer specifying how (read, write, or both) see man 2 shutdown */
+#     sock_evt_cantrecvmore           = 7,
+#     sock_evt_cantsendmore           = 8,
+#     sock_evt_closing                = 9,
+#     sock_evt_bound                  = 10
 # };
 
 base_event_socket = 0x1000
 
 class SocketEvent(enum.Enum):
     CONNECTING = 0x1001
     CONNECTED = 0x1002
@@ -127,15 +127,15 @@
     IPPROTO_XTP             = 36
     IPPROTO_DDP             = 37
     IPPROTO_CMTP            = 38
     IPPROTO_TPXX            = 39
     IPPROTO_IL              = 40
     IPPROTO_IPV6            = 41
     IPPROTO_SDRP            = 42
-    IPPROTO_ROUTING 	    = 43
+    IPPROTO_ROUTING         = 43
     IPPROTO_FRAGMENT        = 44
     IPPROTO_IDRP            = 45
     IPPROTO_RSVP            = 46
     IPPROTO_GRE             = 47
     IPPROTO_MHRP            = 48
     IPPROTO_BHA             = 49
     IPPROTO_ESP             = 50
@@ -210,26 +210,26 @@
     KAUTH_FILEOP_EXCHANGE = 4
     KAUTH_FILEOP_LINK = 5
     KAUTH_FILEOP_EXEC = 6
     KAUTH_FILEOP_DELETE = 7
     KAUTH_FILEOP_WILL_RENAME = 8
 
 # struct sysctl_oid {
-# 	struct sysctl_oid_list *oid_parent;
-# 	SLIST_ENTRY(sysctl_oid) oid_link;
-# 	int		oid_number;
-# 	int		oid_kind;
-# 	void		*oid_arg1;
-# 	int		oid_arg2;
-# 	const char	*oid_name;
-# 	int 		(*oid_handler) SYSCTL_HANDLER_ARGS;
-# 	const char	*oid_fmt;
-# 	const char	*oid_descr; /* offsetof() field / long description */
-# 	int		oid_version;
-# 	int		oid_refcnt;
+#     struct sysctl_oid_list *oid_parent;
+#     SLIST_ENTRY(sysctl_oid) oid_link;
+#     int        oid_number;
+#     int        oid_kind;
+#     void        *oid_arg1;
+#     int        oid_arg2;
+#     const char    *oid_name;
+#     int         (*oid_handler) SYSCTL_HANDLER_ARGS;
+#     const char    *oid_fmt;
+#     const char    *oid_descr; /* offsetof() field / long description */
+#     int        oid_version;
+#     int        oid_refcnt;
 # };
 
 class sysctl_oid_t(ctypes.Structure):
     class slist_entry(ctypes.Structure):
         _fields_ = (
             ("sle_next", POINTER64),
         )
@@ -270,19 +270,19 @@
                 self.ql.log.info("%s: Struct( 0x%x )" % (field[0], getattr(self, field[0]).sle_next.value))
             else:
                 self.ql.log.info("%s: 0x%x" % (field[0], getattr(self, field[0])))
 
 class sysctl_args_t(ctypes.Structure):
     _fields_ = (
         ("name", ctypes.c_int32 * 2),
-	("namelen", ctypes.c_uint32),
-	("old", POINTER64),
-	("oldlenp", POINTER64),
-	("new", POINTER64),
-	("newlen", ctypes.c_uint64),
+    ("namelen", ctypes.c_uint32),
+    ("old", POINTER64),
+    ("oldlenp", POINTER64),
+    ("new", POINTER64),
+    ("newlen", ctypes.c_uint64),
     )
 
     def __init__(self, ql, base):
         self.ql = ql
         self.base = base
 
     def updateToMem(self):
@@ -292,20 +292,20 @@
         data = self.ql.mem.read(self.base, ctypes.sizeof(self))
         newObj = type(self).from_buffer(data)
         newObj.ql = self.ql
         newObj.base = self.base
         return newObj
 
 # struct sysctlbyname_args {
-#     const char * 	name
-#     size_t 	namelen
-#     void * 	old
-#     size_t * 	oldlenp
-#     void * 	new
-#     size_t 	newlen
+#     const char *     name
+#     size_t     namelen
+#     void *     old
+#     size_t *     oldlenp
+#     void *     new
+#     size_t     newlen
 #  }
 
 class sysctlbyname_args_t(ctypes.Structure):
     _fields_ = (
         ("name", POINTER64),
         ("namelen", ctypes.c_size_t),
         ("old", POINTER64),
@@ -325,24 +325,24 @@
         data = self.ql.mem.read(self.base, ctypes.sizeof(self))
         newObj = type(self).from_buffer(data)
         newObj.ql = self.ql
         newObj.base = self.base
         return newObj
 
 # struct sysctl_req {
-# 	struct proc	*p;
-# 	int		lock;
-# 	user_addr_t	oldptr;		/* pointer to user supplied buffer */
-# 	size_t		oldlen;		/* user buffer length (also returned) */
-# 	size_t		oldidx;		/* total data iteratively copied out */
-# 	int		(*oldfunc)(struct sysctl_req *, const void *, size_t);
-# 	user_addr_t	newptr;		/* buffer containing new value */
-# 	size_t		newlen;		/* length of new value */
-# 	size_t		newidx;		/* total data iteratively copied in */
-# 	int		(*newfunc)(struct sysctl_req *, void *, size_t);
+#     struct proc    *p;
+#     int        lock;
+#     user_addr_t    oldptr;        /* pointer to user supplied buffer */
+#     size_t        oldlen;        /* user buffer length (also returned) */
+#     size_t        oldidx;        /* total data iteratively copied out */
+#     int        (*oldfunc)(struct sysctl_req *, const void *, size_t);
+#     user_addr_t    newptr;        /* buffer containing new value */
+#     size_t        newlen;        /* length of new value */
+#     size_t        newidx;        /* total data iteratively copied in */
+#     int        (*newfunc)(struct sysctl_req *, void *, size_t);
 # };
 
 class sysctl_req_t(ctypes.Structure):
     _fields_ = (
         ("p", POINTER64),
         ("lock", ctypes.c_int32),
         ("oldptr", POINTER64),
@@ -367,34 +367,34 @@
         newObj = type(self).from_buffer(data)
         newObj.ql = self.ql
         newObj.base = self.base
         return newObj
 
 # struct kern_ctl_reg
 # {
-# 	/* control information */
-# 	char		ctl_name[MAX_KCTL_NAME];
-# 	u_int32_t	ctl_id;
-# 	u_int32_t	ctl_unit;
+#     /* control information */
+#     char        ctl_name[MAX_KCTL_NAME];
+#     u_int32_t    ctl_id;
+#     u_int32_t    ctl_unit;
 # 
 #     /* control settings */
-#     u_int32_t	ctl_flags;
-#     u_int32_t	ctl_sendsize;
-#     u_int32_t	ctl_recvsize;
+#     u_int32_t    ctl_flags;
+#     u_int32_t    ctl_sendsize;
+#     u_int32_t    ctl_recvsize;
 # 
 #     /* Dispatch functions */
-#     ctl_connect_func	ctl_connect;
-#     ctl_disconnect_func	ctl_disconnect;
-#     ctl_send_func		ctl_send;
-#     ctl_setopt_func		ctl_setopt;
-#     ctl_getopt_func		ctl_getopt;
+#     ctl_connect_func    ctl_connect;
+#     ctl_disconnect_func    ctl_disconnect;
+#     ctl_send_func        ctl_send;
+#     ctl_setopt_func        ctl_setopt;
+#     ctl_getopt_func        ctl_getopt;
 # #ifdef KERNEL_PRIVATE
-#     ctl_rcvd_func		ctl_rcvd;	/* Only valid if CTL_FLAG_REG_EXTENDED is set */
-#     ctl_send_list_func		ctl_send_list;	/* Only valid if CTL_FLAG_REG_EXTENDED is set */
-# 	ctl_bind_func		ctl_bind;
+#     ctl_rcvd_func        ctl_rcvd;    /* Only valid if CTL_FLAG_REG_EXTENDED is set */
+#     ctl_send_list_func        ctl_send_list;    /* Only valid if CTL_FLAG_REG_EXTENDED is set */
+#     ctl_bind_func        ctl_bind;
 # #endif /* KERNEL_PRIVATE */
 # };
 
 class kern_ctl_reg_t(ctypes.Structure):
     _fields_ = (
         ("ctl_name", ctypes.c_char * 96),
         ("ctl_id", ctypes.c_uint32),
@@ -433,20 +433,20 @@
             elif isinstance(getattr(self, field[0]), int):
                 self.ql.log.info("%s: %d" % (field[0], getattr(self, field[0])))
             elif isinstance(getattr(self, field[0]), bytes):
                 self.ql.log.info("%s: %s" % (field[0], getattr(self, field[0]).decode()))
 
 
 # struct sockaddr_ctl {
-#     u_char	sc_len;		/* depends on size of bundle ID string */
-#     u_char	sc_family;	/* AF_SYSTEM */
-#     u_int16_t 	ss_sysaddr;	/* AF_SYS_KERNCONTROL */
-#     u_int32_t	sc_id; 		/* Controller unique identifier  */
-#     u_int32_t 	sc_unit;	/* Developer private unit number */
-#     u_int32_t 	sc_reserved[5];
+#     u_char    sc_len;        /* depends on size of bundle ID string */
+#     u_char    sc_family;    /* AF_SYSTEM */
+#     u_int16_t     ss_sysaddr;    /* AF_SYS_KERNCONTROL */
+#     u_int32_t    sc_id;         /* Controller unique identifier  */
+#     u_int32_t     sc_unit;    /* Developer private unit number */
+#     u_int32_t     sc_reserved[5];
 # };
 
 class sockaddr_ctl_t(ctypes.Structure):
     _fields_ = (
         ("sc_len", ctypes.c_ubyte),
         ("sc_family", ctypes.c_ubyte),
         ("ss_sysaddr", ctypes.c_uint16),
@@ -466,20 +466,20 @@
         data = self.ql.mem.read(self.base, ctypes.sizeof(self))
         newObj = type(self).from_buffer(data)
         newObj.ql = self.ql
         newObj.base = self.base
         return newObj
 
 # struct m_hdr {
-# 	struct mbuf	*mh_next;	/* next buffer in chain */
-# 	struct mbuf	*mh_nextpkt;	/* next chain in queue/record */
-# 	caddr_t		mh_data;	/* location of data */
-# 	int32_t		mh_len;		/* amount of data in this mbuf */
-# 	u_int16_t	mh_type;	/* type of data in this mbuf */
-# 	u_int16_t	mh_flags;	/* flags; see below */
+#     struct mbuf    *mh_next;    /* next buffer in chain */
+#     struct mbuf    *mh_nextpkt;    /* next chain in queue/record */
+#     caddr_t        mh_data;    /* location of data */
+#     int32_t        mh_len;        /* amount of data in this mbuf */
+#     u_int16_t    mh_type;    /* type of data in this mbuf */
+#     u_int16_t    mh_flags;    /* flags; see below */
 # }
 
 class m_hdr_t(ctypes.Structure):
     _fields_ = (
         ("mh_next", POINTER64),
         ("mh_nextpkt", POINTER64),
         ("mh_data", POINTER64),
@@ -492,26 +492,26 @@
     _fields_ = (
         ("packet_tags", POINTER64),
     )
 
 # struct tcp_pktinfo {
 #     union {
 #         struct {
-#                 u_int32_t segsz;	/* segment size (actual MSS) */
-#                 u_int32_t start_seq;	/* start seq of this packet */
+#                 u_int32_t segsz;    /* segment size (actual MSS) */
+#                 u_int32_t start_seq;    /* start seq of this packet */
 #         } __tx;
 #         struct {
-#                 u_int16_t lro_pktlen;	/* max seg size encountered */
-#                 u_int8_t  lro_npkts;	/* # of coalesced TCP pkts */
-#                 u_int8_t  lro_timediff;	/* time spent in LRO */
+#                 u_int16_t lro_pktlen;    /* max seg size encountered */
+#                 u_int8_t  lro_npkts;    /* # of coalesced TCP pkts */
+#                 u_int8_t  lro_timediff;    /* time spent in LRO */
 #         } __rx;
 #     } __offload;
 #     union {
-#         u_int32_t	pri;		/* send msg priority */
-#         u_int32_t	seq;		/* recv msg sequence # */
+#         u_int32_t    pri;        /* send msg priority */
+#         u_int32_t    seq;        /* recv msg sequence # */
 #     } __msgattr;
 # };
 class tcp_pktinfo_t(ctypes.Structure):
     class __offload_u(ctypes.Union):
         class __tx_t(ctypes.Structure):
             _fields_ = (
                 ("segsz", ctypes.c_uint32),
@@ -534,31 +534,31 @@
         )
     _fields_ = (
         ("__offload", __offload_u),
         ("__msgattr", __msgattr_u),
     )
 
 # struct mptcp_pktinfo {
-#     u_int64_t	mtpi_dsn;	/* MPTCP Data Sequence Number */
-#     u_int32_t	mtpi_rel_seq;	/* Relative Seq Number */
-#     u_int16_t	mtpi_length;	/* Length of mapping */
-#     u_int16_t	mtpi_csum;
+#     u_int64_t    mtpi_dsn;    /* MPTCP Data Sequence Number */
+#     u_int32_t    mtpi_rel_seq;    /* Relative Seq Number */
+#     u_int16_t    mtpi_length;    /* Length of mapping */
+#     u_int16_t    mtpi_csum;
 # };
 class mptcp_pktinfo_t(ctypes.Structure):
     _fields_ = (
         ("mtpi_dsn", ctypes.c_uint64),
         ("mtpi_rel_seq", ctypes.c_uint32),
         ("mtpi_length", ctypes.c_uint16),
         ("mtpi_csum", ctypes.c_uint16),
     )
 
 # struct tcp_mtag {
 #     union {
-#         struct tcp_pktinfo	tm_tcp;		/* TCP and below */
-#         struct mptcp_pktinfo	tm_mptcp;	/* MPTCP-TCP only */
+#         struct tcp_pktinfo    tm_tcp;        /* TCP and below */
+#         struct mptcp_pktinfo    tm_mptcp;    /* MPTCP-TCP only */
 #     };
 # };
 class tcp_mtag_t(ctypes.Structure):
     class pktinfo_u(ctypes.Union):
         _fields_ = (
             ("tm_tcp", tcp_pktinfo_t),
             ("tm_mptcp", mptcp_pktinfo_t),
@@ -566,71 +566,71 @@
     _anonymous_ = ("tmp_union",)
     _fields_ = (
         ("tmp_union", pktinfo_u),
     )
 
 # struct proto_mtag_ {
 #     union {
-#         struct tcp_mtag	tcp;		/* TCP specific */
+#         struct tcp_mtag    tcp;        /* TCP specific */
 #     } __pr_u;
 # };
 class proto_mtag__t(ctypes.Structure):
     class __pr_u_u(ctypes.Union):
         _fields_ = (
             ("tcp", tcp_mtag_t),
         )
     _fields_ = (
         ("__pr_u", __pr_u_u),
     )
 
 # struct pf_mtag {
-#     u_int16_t	pftag_flags;	/* PF_TAG flags */
-#     u_int16_t	pftag_rtableid;	/* alternate routing table id */
-#     u_int16_t	pftag_tag;
-#     u_int16_t	pftag_routed;
+#     u_int16_t    pftag_flags;    /* PF_TAG flags */
+#     u_int16_t    pftag_rtableid;    /* alternate routing table id */
+#     u_int16_t    pftag_tag;
+#     u_int16_t    pftag_routed;
 # #if PF_ECN
-#     void		*pftag_hdr;	/* saved hdr pos in mbuf, for ECN */
+#     void        *pftag_hdr;    /* saved hdr pos in mbuf, for ECN */
 # #endif /* PF_ECN */
 # };
 class pf_mtag_t(ctypes.Structure):
     _fields_ = (
         ("pftag_flags", ctypes.c_int16),
         ("pftag_rtableid", ctypes.c_int16),
         ("pftag_tag", ctypes.c_int16),
         ("pftag_routed", ctypes.c_int16),
     )
 
 # struct necp_mtag_ {
-#     u_int32_t	necp_policy_id;
-#     u_int32_t	necp_last_interface_index;
-#     u_int32_t	necp_route_rule_id;
-#     u_int32_t	necp_app_id;
+#     u_int32_t    necp_policy_id;
+#     u_int32_t    necp_last_interface_index;
+#     u_int32_t    necp_route_rule_id;
+#     u_int32_t    necp_app_id;
 # };
 class necp_mtag__t(ctypes.Structure):
     _fields_ = (
         ("necp_policy_id", ctypes.c_int32),
         ("necp_last_interface_index", ctypes.c_int32),
         ("necp_route_rule_id", ctypes.c_int32),
         ("necp_app_id", ctypes.c_int32),
     )
 
 
 
 # struct {
 #     union {
-#         u_int8_t	__mpriv8[16];
-#         u_int16_t	__mpriv16[8];
+#         u_int8_t    __mpriv8[16];
+#         u_int16_t    __mpriv16[8];
 #         struct {
 #             union {
-#                 u_int8_t	__val8[4];
-#                 u_int16_t	__val16[2];
-#                 u_int32_t	__val32;
+#                 u_int8_t    __val8[4];
+#                 u_int16_t    __val16[2];
+#                 u_int32_t    __val32;
 #             } __mpriv32_u;
 #         } __mpriv32[4];
-#         u_int64_t	__mpriv64[2];
+#         u_int64_t    __mpriv64[2];
 #     } __mpriv_u;
 # } pkt_mpriv __attribute__((aligned(4)));
 class pkt_mpriv_t(ctypes.Structure):
     class __mpriv_u_u(ctypes.Union):
         class __mpriv32_t(ctypes.Structure):
             class __mpriv32_u_u(ctypes.Union):
                 _fields_ = (
@@ -646,71 +646,71 @@
             ("__mpriv64", ctypes.c_uint64 * 2),
         )
     _fields_ = (
         ("__mpriv_u", __mpriv_u_u),
     )
 
 # struct pkthdr {
-# 	struct ifnet *rcvif;		/* rcv interface */
-# 	void	*pkt_hdr;		/* pointer to packet header */
-# 	int32_t	len;			/* total packet length */
-# 	u_int32_t csum_flags;		/* flags regarding checksum */
-# 	union {
-# 		struct {
-# 			u_int16_t val;	 /* checksum value */
-# 			u_int16_t start; /* checksum start offset */
-# 		} _csum_rx;
-# 		struct {
-# 			u_int16_t start; /* checksum start offset */
-# 			u_int16_t stuff; /* checksum stuff offset */
-# 		} _csum_tx;
-# 		u_int32_t csum_data;	/* data field used by csum routines */
-# 	};
-# 	u_int16_t vlan_tag;		/* VLAN tag, host byte order */
-# 	u_int8_t pkt_proto;		/* IPPROTO value */
-# 	u_int8_t pkt_flowsrc;		/* FLOWSRC values */
-# 	u_int32_t pkt_flowid;		/* flow ID */
-# 	u_int32_t pkt_flags;		/* PKTF flags (see below) */
-# 	u_int32_t pkt_svc;		/* MBUF_SVC value */
+#     struct ifnet *rcvif;        /* rcv interface */
+#     void    *pkt_hdr;        /* pointer to packet header */
+#     int32_t    len;            /* total packet length */
+#     u_int32_t csum_flags;        /* flags regarding checksum */
+#     union {
+#         struct {
+#             u_int16_t val;     /* checksum value */
+#             u_int16_t start; /* checksum start offset */
+#         } _csum_rx;
+#         struct {
+#             u_int16_t start; /* checksum start offset */
+#             u_int16_t stuff; /* checksum stuff offset */
+#         } _csum_tx;
+#         u_int32_t csum_data;    /* data field used by csum routines */
+#     };
+#     u_int16_t vlan_tag;        /* VLAN tag, host byte order */
+#     u_int8_t pkt_proto;        /* IPPROTO value */
+#     u_int8_t pkt_flowsrc;        /* FLOWSRC values */
+#     u_int32_t pkt_flowid;        /* flow ID */
+#     u_int32_t pkt_flags;        /* PKTF flags (see below) */
+#     u_int32_t pkt_svc;        /* MBUF_SVC value */
 # 
-# 	u_int32_t pkt_compl_context;		/* Packet completion context */
+#     u_int32_t pkt_compl_context;        /* Packet completion context */
 # 
-# 	union {
-# 		struct {
-# 			u_int16_t src;		/* ifindex of src addr i/f */
-# 			u_int16_t src_flags;	/* src PKT_IFAIFF flags */
-# 			u_int16_t dst;		/* ifindex of dst addr i/f */
-# 			u_int16_t dst_flags;	/* dst PKT_IFAIFF flags */
-# 		} _pkt_iaif;
-# 		u_int64_t pkt_ifainfo;	/* data field used by ifainfo */
-# 		struct {
-# 			u_int32_t if_data; /* bytes in interface queue */
-# 			u_int32_t sndbuf_data; /* bytes in socket buffer */
-# 		} _pkt_bsr;	/* Buffer status report used by cellular interface */
-# 	};
-# 	u_int64_t pkt_timestamp;	/* enqueue time */
+#     union {
+#         struct {
+#             u_int16_t src;        /* ifindex of src addr i/f */
+#             u_int16_t src_flags;    /* src PKT_IFAIFF flags */
+#             u_int16_t dst;        /* ifindex of dst addr i/f */
+#             u_int16_t dst_flags;    /* dst PKT_IFAIFF flags */
+#         } _pkt_iaif;
+#         u_int64_t pkt_ifainfo;    /* data field used by ifainfo */
+#         struct {
+#             u_int32_t if_data; /* bytes in interface queue */
+#             u_int32_t sndbuf_data; /* bytes in socket buffer */
+#         } _pkt_bsr;    /* Buffer status report used by cellular interface */
+#     };
+#     u_int64_t pkt_timestamp;    /* enqueue time */
 # 
-# 	SLIST_HEAD(packet_tags, m_tag) tags; /* list of external tags */
-# 	union builtin_mtag builtin_mtag;
-# 	struct {
-# 		union {
-# 			u_int8_t	__mpriv8[16];
-# 			u_int16_t	__mpriv16[8];
-# 			struct {
-# 				union {
-# 					u_int8_t	__val8[4];
-# 					u_int16_t	__val16[2];
-# 					u_int32_t	__val32;
-# 				} __mpriv32_u;
-# 			}		__mpriv32[4];
-# 			u_int64_t	__mpriv64[2];
-# 		} __mpriv_u;
-# 	} pkt_mpriv __attribute__((aligned(4)));
-# 	u_int32_t redzone;		/* red zone */
-# 	u_int32_t pkt_compl_callbacks;	/* Packet completion callbacks */
+#     SLIST_HEAD(packet_tags, m_tag) tags; /* list of external tags */
+#     union builtin_mtag builtin_mtag;
+#     struct {
+#         union {
+#             u_int8_t    __mpriv8[16];
+#             u_int16_t    __mpriv16[8];
+#             struct {
+#                 union {
+#                     u_int8_t    __val8[4];
+#                     u_int16_t    __val16[2];
+#                     u_int32_t    __val32;
+#                 } __mpriv32_u;
+#             }        __mpriv32[4];
+#             u_int64_t    __mpriv64[2];
+#         } __mpriv_u;
+#     } pkt_mpriv __attribute__((aligned(4)));
+#     u_int32_t redzone;        /* red zone */
+#     u_int32_t pkt_compl_callbacks;    /* Packet completion callbacks */
 # };
 
 class pkthdr_t(ctypes.Structure):
     class chksum_union(ctypes.Union):
         class _csum_rx_t(ctypes.Structure):
             _fields_ = (
                 ("val", ctypes.c_uint16),
@@ -743,27 +743,27 @@
         _fields_ = (
             ("_pkt_iaif", _pkt_iaif_t),
             ("pkt_ifainfo", ctypes.c_uint64),
             ("_pkt_bsr", _pkt_bsr_t),
         )
 
 #     union builtin_mtag {
-# 	struct {
-# 		struct proto_mtag_ _proto_mtag;	/* built-in protocol-specific tag */
-# 		struct pf_mtag	_pf_mtag;	/* built-in PF tag */
-# 		struct necp_mtag_ _necp_mtag; /* built-in NECP tag */
-# 	} _net_mtag;
-# 	struct driver_mtag_ _drv_mtag;
+#     struct {
+#         struct proto_mtag_ _proto_mtag;    /* built-in protocol-specific tag */
+#         struct pf_mtag    _pf_mtag;    /* built-in PF tag */
+#         struct necp_mtag_ _necp_mtag; /* built-in NECP tag */
+#     } _net_mtag;
+#     struct driver_mtag_ _drv_mtag;
 #     }
     class builtin_mtag_u(ctypes.Union):
 #         struct driver_mtag_ {
-#             uintptr_t		_drv_tx_compl_arg;
-#             uintptr_t		_drv_tx_compl_data;
-#             kern_return_t		_drv_tx_status;
-#             uint16_t		_drv_flowid;
+#             uintptr_t        _drv_tx_compl_arg;
+#             uintptr_t        _drv_tx_compl_data;
+#             kern_return_t        _drv_tx_status;
+#             uint16_t        _drv_flowid;
 #         };
         class driver_mtag__t(ctypes.Structure):
             _fields_ = (
                 ("_drv_tx_compl_arg", POINTER64),
                 ("_drv_tx_compl_data", POINTER64),
                 ("_drv_tx_status", ctypes.c_int32),
                 ("_drv_flowid", ctypes.c_int16),
@@ -799,27 +799,27 @@
         ("builtin_mtag", builtin_mtag_u),
         ("pkt_mpriv", pkt_mpriv_t),
         ("redzone", ctypes.c_uint32),
         ("pkt_compl_callbacks", ctypes.c_uint32),
     )
 
 # struct m_ext {
-# 	caddr_t	ext_buf;		/* start of buffer */
-# 	m_ext_free_func_t ext_free;	/* free routine if not the usual */
-# 	u_int	ext_size;		/* size of buffer, for ext_free */
-# 	caddr_t	ext_arg;		/* additional ext_free argument */
-# 	struct ext_ref {
-# 		struct mbuf *paired;
-# 		u_int16_t minref;
-# 		u_int16_t refcnt;
-# 		u_int16_t prefcnt;
-# 		u_int16_t flags;
-# 		u_int32_t priv;
-# 		uintptr_t ext_token;
-# 	} *ext_refflags;
+#     caddr_t    ext_buf;        /* start of buffer */
+#     m_ext_free_func_t ext_free;    /* free routine if not the usual */
+#     u_int    ext_size;        /* size of buffer, for ext_free */
+#     caddr_t    ext_arg;        /* additional ext_free argument */
+#     struct ext_ref {
+#         struct mbuf *paired;
+#         u_int16_t minref;
+#         u_int16_t refcnt;
+#         u_int16_t prefcnt;
+#         u_int16_t flags;
+#         u_int32_t priv;
+#         uintptr_t ext_token;
+#     } *ext_refflags;
 # };
 class ext_ref(ctypes.Structure):
     _fields_ = (
         ("paired", POINTER64),
         ("minref", ctypes.c_uint16),
         ("refcnt", ctypes.c_uint16),
         ("prefcnt", ctypes.c_uint16),
@@ -833,31 +833,31 @@
         ("ext_free", POINTER64),
         ("ext_size", ctypes.c_uint32),
         ("ext_arg", POINTER64),
         ("ext_refflags", POINTER64),
     )
 
 # struct mbuf {
-# 	struct m_hdr m_hdr;
-# 	union {
-# 		struct {
-# 			struct pkthdr MH_pkthdr;	/* M_PKTHDR set */
-# 			union {
-# 				struct m_ext MH_ext;	/* M_EXT set */
-# 				char	MH_databuf[_MHLEN];
-# 			} MH_dat;
-# 		} MH;
-# 		char	M_databuf[_MLEN];		/* !M_PKTHDR, !M_EXT */
-# 	} M_dat;
-# };
-
-#define	MSIZESHIFT	8			/* 256 */
-#define	MSIZE		(1 << MSIZESHIFT)	/* size of an mbuf */
-#define	_MLEN		(MSIZE - sizeof(struct m_hdr))	/* normal data len */
-#define	_MHLEN		(_MLEN - sizeof(struct pkthdr))	/* data len w/pkthdr */
+#     struct m_hdr m_hdr;
+#     union {
+#         struct {
+#             struct pkthdr MH_pkthdr;    /* M_PKTHDR set */
+#             union {
+#                 struct m_ext MH_ext;    /* M_EXT set */
+#                 char    MH_databuf[_MHLEN];
+#             } MH_dat;
+#         } MH;
+#         char    M_databuf[_MLEN];        /* !M_PKTHDR, !M_EXT */
+#     } M_dat;
+# };
+
+#define    MSIZESHIFT    8            /* 256 */
+#define    MSIZE        (1 << MSIZESHIFT)    /* size of an mbuf */
+#define    _MLEN        (MSIZE - sizeof(struct m_hdr))    /* normal data len */
+#define    _MHLEN        (_MLEN - sizeof(struct pkthdr))    /* data len w/pkthdr */
 
 MSIZESHIFT = 8
 MSIZE = (1 << MSIZESHIFT)
 _MLEN = (MSIZE - ctypes.sizeof(m_hdr_t))
 _MHLEN = (_MLEN - ctypes.sizeof(pkthdr_t))
 
 class mbuf_t(ctypes.Structure):
@@ -893,20 +893,20 @@
         newObj = type(self).from_buffer(data)
         newObj.ql = self.ql
         newObj.base = self.base
         return newObj
 
 # enum sopt_dir { SOPT_GET, SOPT_SET };
 # struct sockopt {
-# 	enum sopt_dir sopt_dir; /* is this a get or a set? */
-# 	int	sopt_level;	/* second arg of [gs]etsockopt */
-# 	int	sopt_name;	/* third arg of [gs]etsockopt */
-# 	void* sopt_val;	/* fourth arg of [gs]etsockopt */
-# 	size_t	sopt_valsize;	/* (almost) fifth arg of [gs]etsockopt */
-# 	void *sopt_p;	/* calling process or null if kernel */
+#     enum sopt_dir sopt_dir; /* is this a get or a set? */
+#     int    sopt_level;    /* second arg of [gs]etsockopt */
+#     int    sopt_name;    /* third arg of [gs]etsockopt */
+#     void* sopt_val;    /* fourth arg of [gs]etsockopt */
+#     size_t    sopt_valsize;    /* (almost) fifth arg of [gs]etsockopt */
+#     void *sopt_p;    /* calling process or null if kernel */
 # };
 
 class sockopt_t(ctypes.Structure):
     _fields_ = (
         ("sopt_dir", ctypes.c_uint64),
         ("sopt_level", ctypes.c_int32),
         ("sopt_name", ctypes.c_int32),
@@ -926,44 +926,44 @@
         data = self.ql.mem.read(self.base, ctypes.sizeof(self))
         newObj = type(self).from_buffer(data)
         newObj.ql = self.ql
         newObj.base = self.base
         return newObj
 
 # struct sflt_filter {
-# 	sflt_handle                     sf_handle;
-# 	int                             sf_flags;
-# 	char                            *sf_name;
+#     sflt_handle                     sf_handle;
+#     int                             sf_flags;
+#     char                            *sf_name;
 # 
-# 	sf_unregistered_func            sf_unregistered;
-# 	sf_attach_func                  sf_attach;
-# 	sf_detach_func                  sf_detach;
+#     sf_unregistered_func            sf_unregistered;
+#     sf_attach_func                  sf_attach;
+#     sf_detach_func                  sf_detach;
 # 
-# 	sf_notify_func                  sf_notify;
-# 	sf_getpeername_func             sf_getpeername;
-# 	sf_getsockname_func             sf_getsockname;
-# 	sf_data_in_func                 sf_data_in;
-# 	sf_data_out_func                sf_data_out;
-# 	sf_connect_in_func              sf_connect_in;
-# 	sf_connect_out_func             sf_connect_out;
-# 	sf_bind_func                    sf_bind;
-# 	sf_setoption_func               sf_setoption;
-# 	sf_getoption_func               sf_getoption;
-# 	sf_listen_func                  sf_listen;
-# 	sf_ioctl_func                   sf_ioctl;
-# 	/*
-# 	 * The following are valid only if SFLT_EXTENDED flag is set.
-# 	 * Initialize sf_ext_len to sizeof sflt_filter_ext structure.
-# 	 * Filters must also initialize reserved fields with zeroes.
-# 	 */
-# 	struct sflt_filter_ext {
-# 		unsigned int            sf_ext_len;
-# 		sf_accept_func          sf_ext_accept;
-# 		void                    *sf_ext_rsvd[5];        /* Reserved */
-# 	} sf_ext;
+#     sf_notify_func                  sf_notify;
+#     sf_getpeername_func             sf_getpeername;
+#     sf_getsockname_func             sf_getsockname;
+#     sf_data_in_func                 sf_data_in;
+#     sf_data_out_func                sf_data_out;
+#     sf_connect_in_func              sf_connect_in;
+#     sf_connect_out_func             sf_connect_out;
+#     sf_bind_func                    sf_bind;
+#     sf_setoption_func               sf_setoption;
+#     sf_getoption_func               sf_getoption;
+#     sf_listen_func                  sf_listen;
+#     sf_ioctl_func                   sf_ioctl;
+#     /*
+#      * The following are valid only if SFLT_EXTENDED flag is set.
+#      * Initialize sf_ext_len to sizeof sflt_filter_ext structure.
+#      * Filters must also initialize reserved fields with zeroes.
+#      */
+#     struct sflt_filter_ext {
+#         unsigned int            sf_ext_len;
+#         sf_accept_func          sf_ext_accept;
+#         void                    *sf_ext_rsvd[5];        /* Reserved */
+#     } sf_ext;
 # };
 
 class sflt_filter_t(ctypes.Structure):
     class sflt_filter_ext(ctypes.Structure):
         _fields_ = (
             ("sf_ext_len", ctypes.c_uint32),
             ("sf_ext_accept", POINTER64),
@@ -1013,24 +1013,24 @@
                 self.ql.log.info("%s: 0x%x" % (field[0], getattr(self, field[0]).value))
             elif isinstance(getattr(self, field[0]), int):
                 self.ql.log.info("%s: %d" % (field[0], getattr(self, field[0])))
             elif isinstance(getattr(self, field[0]), bytes):
                 self.ql.log.info("%s: %s" % (field[0], getattr(self, field[0]).decode()))
 
 # struct sockaddr_in {
-# 	__uint8_t	sin_len;
-# 	sa_family_t	sin_family;
-# 	in_port_t	sin_port;
-# 	struct	in_addr sin_addr;
-# 	char		sin_zero[8];
+#     __uint8_t    sin_len;
+#     sa_family_t    sin_family;
+#     in_port_t    sin_port;
+#     struct    in_addr sin_addr;
+#     char        sin_zero[8];
 # };
 
 class sockaddr_in_t(ctypes.Structure):
 #     struct in_addr {
-# 	in_addr_t s_addr;
+#     in_addr_t s_addr;
 #     };
     class in_addr_t(ctypes.Structure):
         _fields_ = (
             ("s_addr", ctypes.c_uint32),
         )
     _fields_ = (
         ("sin_len", ctypes.c_uint8),
@@ -1052,17 +1052,17 @@
         newObj = type(self).from_buffer(data)
         newObj.ql = self.ql
         newObj.base = self.base
         return newObj
 
 # #define ETHER_ADDR_LEN          6
 # typedef struct  ether_header {
-# 	u_char  ether_dhost[ETHER_ADDR_LEN];
-# 	u_char  ether_shost[ETHER_ADDR_LEN];
-# 	u_short ether_type;
+#     u_char  ether_dhost[ETHER_ADDR_LEN];
+#     u_char  ether_shost[ETHER_ADDR_LEN];
+#     u_short ether_type;
 # } ether_header_t;
 class ether_header_t(ctypes.Structure):
     _fields_ = (
         ("ether_dhost", ctypes.c_ubyte * 6),
         ("ether_shost", ctypes.c_ubyte * 6),
         ("ether_type", ctypes.c_ushort),
     )
@@ -1127,30 +1127,30 @@
                 self.ql.log.info("%s: 0x%x" % (field[0], getattr(self, field[0]).value))
             elif isinstance(getattr(self, field[0]), int):
                 self.ql.log.info("%s: %d" % (field[0], getattr(self, field[0])))
             elif isinstance(getattr(self, field[0]), bytes):
                 self.ql.log.info("%s: %s" % (field[0], getattr(self, field[0]).decode()))
 
 # struct ucred {
-# 	TAILQ_ENTRY(ucred)	cr_link; /* never modify this without KAUTH_CRED_HASH_LOCK */
-# 	u_long	cr_ref;			/* reference count */
-# 	
+#     TAILQ_ENTRY(ucred)    cr_link; /* never modify this without KAUTH_CRED_HASH_LOCK */
+#     u_long    cr_ref;            /* reference count */
+#     
 # struct posix_cred {
-# 	uid_t	cr_uid;			/* effective user id */
-# 	uid_t	cr_ruid;		/* real user id */
-# 	uid_t	cr_svuid;		/* saved user id */
-# 	short	cr_ngroups;		/* number of groups in advisory list */
-# 	gid_t	cr_groups[NGROUPS];	/* advisory group list */
-# 	gid_t	cr_rgid;		/* real group id */
-# 	gid_t	cr_svgid;		/* saved group id */
-# 	uid_t	cr_gmuid;		/* UID for group membership purposes */
-# 	int	cr_flags;		/* flags on credential */
+#     uid_t    cr_uid;            /* effective user id */
+#     uid_t    cr_ruid;        /* real user id */
+#     uid_t    cr_svuid;        /* saved user id */
+#     short    cr_ngroups;        /* number of groups in advisory list */
+#     gid_t    cr_groups[NGROUPS];    /* advisory group list */
+#     gid_t    cr_rgid;        /* real group id */
+#     gid_t    cr_svgid;        /* saved group id */
+#     uid_t    cr_gmuid;        /* UID for group membership purposes */
+#     int    cr_flags;        /* flags on credential */
 # } cr_posix;
-# 	struct label	*cr_label;	/* MAC label */
-# 	struct au_session cr_audit;		/* user auditing data */
+#     struct label    *cr_label;    /* MAC label */
+#     struct au_session cr_audit;        /* user auditing data */
 # };
 
 class ucred_t(ctypes.Structure):
     class cr_entry(ctypes.Structure):
         _fields_ = (
             ("tqe_next", POINTER64),
             ("tqe_prev", POINTER64),
@@ -1191,19 +1191,19 @@
         data = self.ql.mem.read(self.base, ctypes.sizeof(self))
         newObj = type(self).from_buffer(data)
         newObj.ql = self.ql
         newObj.base = self.base
         return newObj
 
 # struct label {
-#     int	l_flags;
+#     int    l_flags;
 #     union {
-#             void	*l_ptr;
-#             long	 l_long;
-#     }	l_perpolicy[MAC_MAX_SLOTS];
+#             void    *l_ptr;
+#             long     l_long;
+#     }    l_perpolicy[MAC_MAX_SLOTS];
 # };
 
 class label_t(ctypes.Structure):
     class l_perpolicy_t(ctypes.Union):
         _fields_ = (
             ("l_ptr", POINTER64),
             ("l_long", ctypes.c_long),
@@ -1224,56 +1224,56 @@
         data = self.ql.mem.read(self.base, ctypes.sizeof(self))
         newObj = type(self).from_buffer(data)
         newObj.ql = self.ql
         newObj.base = self.base
         return newObj
 
 # struct vnode {
-# 	lck_mtx_t v_lock;			/* vnode mutex */
-# 	TAILQ_ENTRY(vnode) v_freelist;		/* vnode freelist */
-# 	TAILQ_ENTRY(vnode) v_mntvnodes;		/* vnodes for mount point */
-#         TAILQ_HEAD(, namecache) v_ncchildren;	/* name cache entries that regard us as their parent */
-#         LIST_HEAD(, namecache) v_nclinks;	/* name cache entries that name this vnode */
-#         vnode_t	 v_defer_reclaimlist;		/* in case we have to defer the reclaim to avoid recursion */
-#         uint32_t v_listflag;			/* flags protected by the vnode_list_lock (see below) */
-# 	uint32_t v_flag;			/* vnode flags (see below) */
-# 	uint16_t v_lflag;			/* vnode local and named ref flags */
-# 	uint8_t	 v_iterblkflags;		/* buf iterator flags */
-# 	uint8_t	 v_references;			/* number of times io_count has been granted */
-# 	int32_t	 v_kusecount;			/* count of in-kernel refs */
-# 	int32_t	 v_usecount;			/* reference count of users */
-# 	int32_t	 v_iocount;			/* iocounters */
-# 	void *   v_owner;			/* act that owns the vnode */
-# 	uint16_t v_type;			/* vnode type */
-# 	uint16_t v_tag;				/* type of underlying data */
-# 	uint32_t v_id;				/* identity of vnode contents */
-# 	union {
-# 		struct mount	*vu_mountedhere;/* ptr to mounted vfs (VDIR) */
-# 		struct socket	*vu_socket;	/* unix ipc (VSOCK) */
-# 		struct specinfo	*vu_specinfo;	/* device (VCHR, VBLK) */
-# 		struct fifoinfo	*vu_fifoinfo;	/* fifo (VFIFO) */
-# 	        struct ubc_info *vu_ubcinfo;	/* valid for (VREG) */
-# 	} v_un;
-# 	struct	buflists v_cleanblkhd;		/* clean blocklist head */
-# 	struct	buflists v_dirtyblkhd;		/* dirty blocklist head */
-# 	struct klist v_knotes;			/* knotes attached to this vnode */
-#         kauth_cred_t	v_cred;			/* last authorized credential */
-#         kauth_action_t	v_authorized_actions;	/* current authorized actions for v_cred */
-#         int		v_cred_timestamp;	/* determine if entry is stale for MNTK_AUTH_OPAQUE */
-#         int		v_nc_generation;	/* changes when nodes are removed from the name cache */
-# 	int32_t		v_numoutput;			/* num of writes in progress */
-# 	int32_t		v_writecount;			/* reference count of writers */
-# 	const char *v_name;			/* name component of the vnode */
-# 	vnode_t v_parent;			/* pointer to parent vnode */
-# 	struct lockf	*v_lockf;		/* advisory lock list head */
-# 	int 	(**v_op)(void *);		/* vnode operations vector */
-# 	mount_t v_mount;			/* ptr to vfs we are in */
-# 	void *	v_data;				/* private data for fs */
-# 	struct label *v_label;			/* MAC security label */
-# 	vnode_resolve_t v_resolve;		/* trigger vnode resolve info (VDIR only) */
+#     lck_mtx_t v_lock;            /* vnode mutex */
+#     TAILQ_ENTRY(vnode) v_freelist;        /* vnode freelist */
+#     TAILQ_ENTRY(vnode) v_mntvnodes;        /* vnodes for mount point */
+#         TAILQ_HEAD(, namecache) v_ncchildren;    /* name cache entries that regard us as their parent */
+#         LIST_HEAD(, namecache) v_nclinks;    /* name cache entries that name this vnode */
+#         vnode_t     v_defer_reclaimlist;        /* in case we have to defer the reclaim to avoid recursion */
+#         uint32_t v_listflag;            /* flags protected by the vnode_list_lock (see below) */
+#     uint32_t v_flag;            /* vnode flags (see below) */
+#     uint16_t v_lflag;            /* vnode local and named ref flags */
+#     uint8_t     v_iterblkflags;        /* buf iterator flags */
+#     uint8_t     v_references;            /* number of times io_count has been granted */
+#     int32_t     v_kusecount;            /* count of in-kernel refs */
+#     int32_t     v_usecount;            /* reference count of users */
+#     int32_t     v_iocount;            /* iocounters */
+#     void *   v_owner;            /* act that owns the vnode */
+#     uint16_t v_type;            /* vnode type */
+#     uint16_t v_tag;                /* type of underlying data */
+#     uint32_t v_id;                /* identity of vnode contents */
+#     union {
+#         struct mount    *vu_mountedhere;/* ptr to mounted vfs (VDIR) */
+#         struct socket    *vu_socket;    /* unix ipc (VSOCK) */
+#         struct specinfo    *vu_specinfo;    /* device (VCHR, VBLK) */
+#         struct fifoinfo    *vu_fifoinfo;    /* fifo (VFIFO) */
+#             struct ubc_info *vu_ubcinfo;    /* valid for (VREG) */
+#     } v_un;
+#     struct    buflists v_cleanblkhd;        /* clean blocklist head */
+#     struct    buflists v_dirtyblkhd;        /* dirty blocklist head */
+#     struct klist v_knotes;            /* knotes attached to this vnode */
+#         kauth_cred_t    v_cred;            /* last authorized credential */
+#         kauth_action_t    v_authorized_actions;    /* current authorized actions for v_cred */
+#         int        v_cred_timestamp;    /* determine if entry is stale for MNTK_AUTH_OPAQUE */
+#         int        v_nc_generation;    /* changes when nodes are removed from the name cache */
+#     int32_t        v_numoutput;            /* num of writes in progress */
+#     int32_t        v_writecount;            /* reference count of writers */
+#     const char *v_name;            /* name component of the vnode */
+#     vnode_t v_parent;            /* pointer to parent vnode */
+#     struct lockf    *v_lockf;        /* advisory lock list head */
+#     int     (**v_op)(void *);        /* vnode operations vector */
+#     mount_t v_mount;            /* ptr to vfs we are in */
+#     void *    v_data;                /* private data for fs */
+#     struct label *v_label;            /* MAC security label */
+#     vnode_resolve_t v_resolve;        /* trigger vnode resolve info (VDIR only) */
 # };
 class vnode_t(ctypes.Structure):
     class tailq_entry(ctypes.Structure):
         _fields_ = (
             ("tqe_next", POINTER64),
             ("tqe_prev", POINTER64),
         )
@@ -1348,40 +1348,40 @@
         data = self.ql.mem.read(self.base, ctypes.sizeof(self))
         newObj = type(self).from_buffer(data)
         newObj.ql = self.ql
         newObj.base = self.base
         return newObj
 
 # struct fileglob {
-# 	LIST_ENTRY(fileglob) f_msglist;/* list of active files */
-# 	int32_t	fg_flag;		/* see fcntl.h */
-# 	int32_t	fg_count;	/* reference count */
-# 	int32_t	fg_msgcount;	/* references from message queue */
-# 	int32_t fg_lflags;	/* file global flags */
-# 	kauth_cred_t fg_cred;	/* credentials associated with descriptor */
-# 	const struct fileops {
-# 		file_type_t	fo_type;	/* descriptor type */
-# 		int	(*fo_read)	(struct fileproc *fp, struct uio *uio,
-# 					 int flags, vfs_context_t ctx);
-# 		int	(*fo_write)	(struct fileproc *fp, struct uio *uio,
-# 					 int flags, vfs_context_t ctx);
-# 		int	(*fo_ioctl)	(struct fileproc *fp, u_long com,
-# 					 caddr_t data, vfs_context_t ctx);
-# 		int	(*fo_select)	(struct fileproc *fp, int which,
-# 					 void *wql, vfs_context_t ctx);
-# 		int	(*fo_close)	(struct fileglob *fg, vfs_context_t ctx);
-# 		int	(*fo_kqfilter)	(struct fileproc *fp, struct knote *kn,
-# 					 struct kevent_internal_s *kev, vfs_context_t ctx);
-# 		int	(*fo_drain)	(struct fileproc *fp, vfs_context_t ctx);
-# 	} *fg_ops;
-# 	off_t	fg_offset;
-# 	void 	*fg_data;	/* vnode or socket or SHM or semaphore */
-# 	void	*fg_vn_data;	/* Per fd vnode data, used for directories */
-# 	lck_mtx_t fg_lock;
-# 	struct label *fg_label;  /* JMM - use the one in the cred? */
+#     LIST_ENTRY(fileglob) f_msglist;/* list of active files */
+#     int32_t    fg_flag;        /* see fcntl.h */
+#     int32_t    fg_count;    /* reference count */
+#     int32_t    fg_msgcount;    /* references from message queue */
+#     int32_t fg_lflags;    /* file global flags */
+#     kauth_cred_t fg_cred;    /* credentials associated with descriptor */
+#     const struct fileops {
+#         file_type_t    fo_type;    /* descriptor type */
+#         int    (*fo_read)    (struct fileproc *fp, struct uio *uio,
+#                      int flags, vfs_context_t ctx);
+#         int    (*fo_write)    (struct fileproc *fp, struct uio *uio,
+#                      int flags, vfs_context_t ctx);
+#         int    (*fo_ioctl)    (struct fileproc *fp, u_long com,
+#                      caddr_t data, vfs_context_t ctx);
+#         int    (*fo_select)    (struct fileproc *fp, int which,
+#                      void *wql, vfs_context_t ctx);
+#         int    (*fo_close)    (struct fileglob *fg, vfs_context_t ctx);
+#         int    (*fo_kqfilter)    (struct fileproc *fp, struct knote *kn,
+#                      struct kevent_internal_s *kev, vfs_context_t ctx);
+#         int    (*fo_drain)    (struct fileproc *fp, vfs_context_t ctx);
+#     } *fg_ops;
+#     off_t    fg_offset;
+#     void     *fg_data;    /* vnode or socket or SHM or semaphore */
+#     void    *fg_vn_data;    /* Per fd vnode data, used for directories */
+#     lck_mtx_t fg_lock;
+#     struct label *fg_label;  /* JMM - use the one in the cred? */
 # };
 
 class fileglob_t(ctypes.Structure):
     class list_entry(ctypes.Structure):
         _fields_ = (
             ("le_next", POINTER64),
             ("le_prev", POINTER64),
@@ -1455,19 +1455,19 @@
         data = self.ql.mem.read(self.base, ctypes.sizeof(self))
         newObj = type(self).from_buffer(data)
         newObj.ql = self.ql
         newObj.base = self.base
         return newObj
 
 # struct ipf_filter {
-# 	void		*cookie;
-# 	const char	*name;
-# 	ipf_input_func	ipf_input;
-# 	ipf_output_func	ipf_output;
-# 	ipf_detach_func	ipf_detach;
+#     void        *cookie;
+#     const char    *name;
+#     ipf_input_func    ipf_input;
+#     ipf_output_func    ipf_output;
+#     ipf_detach_func    ipf_detach;
 # };
 class ipf_filter_t(ctypes.Structure):
     _fields_ = (
         ("cookie", POINTER64),
         ("name", POINTER64),
         ("ipf_input", POINTER64),
         ("ipf_output", POINTER64),
```

### Comparing `qiling-1.4.5/qiling/os/macos/fncc.py` & `qiling-1.4.6/qiling/os/macos/fncc.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/os/macos/kernel_api/hook.py` & `qiling-1.4.6/qiling/os/macos/kernel_api/hook.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/os/macos/kernel_api/kernel_api.py` & `qiling-1.4.6/qiling/os/macos/kernel_api/kernel_api.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/os/macos/kernel_func.py` & `qiling-1.4.6/qiling/os/macos/kernel_func.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/os/macos/mach_port.py` & `qiling-1.4.6/qiling/os/macos/mach_port.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,20 +7,20 @@
 
 from struct import pack, unpack
 
 from qiling.const import *
 
 # define in kernel osfmk/mach/message.h
 # mach_msg_header_t:
-#   mach_msg_bits_t	msgh_bits;                  unsigned int 
-#   mach_msg_size_t	msgh_size;                  4 bytes
-#   mach_port_t		msgh_remote_port;           4 bytes
-#   mach_port_t		msgh_local_port;            4 bytes
-#   mach_port_name_t	msgh_voucher_port;      4 bytes
-#   mach_msg_id_t		msgh_id;                4 bytes
+#   mach_msg_bits_t    msgh_bits;                  unsigned int 
+#   mach_msg_size_t    msgh_size;                  4 bytes
+#   mach_port_t        msgh_remote_port;           4 bytes
+#   mach_port_t        msgh_local_port;            4 bytes
+#   mach_port_name_t    msgh_voucher_port;      4 bytes
+#   mach_msg_id_t        msgh_id;                4 bytes
 class MachMsgHeader():
 
     def __init__(self, ql):
         self.header_size = 24
         self.ql = ql
         self.msgh_bits = None
         self.msgh_size = None
@@ -132,17 +132,17 @@
         self.ql.log.debug("Reply-> Header: {}, Content: {}".format(out_msg.header, out_msg.content))
 
     def get_thread_port(self, MachoThread):
         return MachoThread.port.name
 
 # XNU define struct :
 # struct mach_msg_overwrite_trap_args {
-# 	PAD_ARG_(user_addr_t, msg);                     addr length
-# 	PAD_ARG_(mach_msg_option_t, option);            int
-# 	PAD_ARG_(mach_msg_size_t, send_size);           unsigned int
-# 	PAD_ARG_(mach_msg_size_t, rcv_size);            unsigned int
-# 	PAD_ARG_(mach_port_name_t, rcv_name);           unsigned int 
-# 	PAD_ARG_(mach_msg_timeout_t, timeout);          unsigned int
-# 	PAD_ARG_(mach_msg_priority_t, override);        unsigned int
-# 	PAD_ARG_8
-# 	PAD_ARG_(user_addr_t, rcv_msg);  /* Unused on mach_msg_trap */  addr length
+#     PAD_ARG_(user_addr_t, msg);                     addr length
+#     PAD_ARG_(mach_msg_option_t, option);            int
+#     PAD_ARG_(mach_msg_size_t, send_size);           unsigned int
+#     PAD_ARG_(mach_msg_size_t, rcv_size);            unsigned int
+#     PAD_ARG_(mach_port_name_t, rcv_name);           unsigned int 
+#     PAD_ARG_(mach_msg_timeout_t, timeout);          unsigned int
+#     PAD_ARG_(mach_msg_priority_t, override);        unsigned int
+#     PAD_ARG_8
+#     PAD_ARG_(user_addr_t, rcv_msg);  /* Unused on mach_msg_trap */  addr length
 # };
```

### Comparing `qiling-1.4.5/qiling/os/macos/macos.py` & `qiling-1.4.6/qiling/os/macos/macos.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/os/macos/map_syscall.py` & `qiling-1.4.6/qiling/os/macos/map_syscall.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/os/macos/structs.py` & `qiling-1.4.6/qiling/os/macos/structs.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/os/macos/subsystems.py` & `qiling-1.4.6/qiling/os/macos/subsystems.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/os/macos/syscall.py` & `qiling-1.4.6/qiling/os/macos/syscall.py`

 * *Files 1% similar despite different names*

```diff
@@ -259,16 +259,16 @@
     else:
         ql.mem.write(attributeBuffer, attr)
         set_eflags_cf(ql, 0x0)
         return KERN_SUCCESS
 
 # 0xc2
 # struct rlimit {
-#     rlim_t	rlim_cur;		/* current (soft) limit */       uint64
-#     rlim_t	rlim_max;		/* maximum value for rlim_cur */ uint64
+#     rlim_t    rlim_cur;        /* current (soft) limit */       uint64
+#     rlim_t    rlim_max;        /* maximum value for rlim_cur */ uint64
 # };
 def ql_syscall_getrlimit(ql, which, rlp, *args, **kw):
     ql.log.debug("getrlimit(which:0x%x, rlp:0x%x)" % (which, rlp))
     _RLIMIT_POSIX_FLAG = 0x1000
     RLIM_NLIMITS = 9
     which = which & _RLIMIT_POSIX_FLAG
     if which >= RLIM_NLIMITS:
```

### Comparing `qiling-1.4.5/qiling/os/macos/thread.py` & `qiling-1.4.6/qiling/os/macos/thread.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/os/macos/utils.py` & `qiling-1.4.6/qiling/os/macos/utils.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/os/mcu/mcu.py` & `qiling-1.4.6/qiling/os/mcu/mcu.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/os/memory.py` & `qiling-1.4.6/qiling/os/memory.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/os/os.py` & `qiling-1.4.6/qiling/os/os.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 #!/usr/bin/env python3
 #
 # Cross Platform and Multi Architecture Advanced Binary Emulation Framework
 #
 
 import sys
-from typing import Any, Hashable, Iterable, Optional, Callable, Mapping, Sequence, TextIO, Tuple
+from io import UnsupportedOperation
+from typing import Any, Dict, Iterable, Optional, Callable, Mapping, Sequence, TextIO, Tuple, Union
 
 from unicorn import UcError
 
 from qiling import Qiling
-from qiling.const import QL_OS, QL_INTERCEPT, QL_OS_POSIX
+from qiling.const import QL_OS, QL_STATE, QL_INTERCEPT, QL_OS_POSIX
 from qiling.os.const import STRING, WSTRING, GUID
 from qiling.os.fcall import QlFunctionCall, TypedArg
 
-from .filestruct import ql_file
+from .filestruct import PersistentQlFile
 from .mapper import QlFsMapper
 from .stats import QlOsStats
 from .utils import QlOsUtils
 from .path import QlOsPath
 
+
 class QlOs:
     type: QL_OS
 
     Resolver = Callable[[int], Any]
 
     def __init__(self, ql: Qiling, resolvers: Mapping[Any, Resolver] = {}):
         self.ql = ql
@@ -42,31 +44,39 @@
 
         if self.type in QL_OS_POSIX + (QL_OS.WINDOWS, QL_OS.DOS):
             cwd = self.profile.get("MISC", "current_path")
 
             self.path = QlOsPath(ql.rootfs, cwd, self.type)
             self.fs_mapper = QlFsMapper(self.path)
 
-        self.user_defined_api = {
-            QL_INTERCEPT.CALL : {},
+        self.user_defined_api: Dict[QL_INTERCEPT, Dict[Union[int, str], Callable]] = {
+            QL_INTERCEPT.CALL:  {},
             QL_INTERCEPT.ENTER: {},
-            QL_INTERCEPT.EXIT : {}
+            QL_INTERCEPT.EXIT:  {}
         }
 
-        # IDAPython has some hack on standard io streams and thus they don't have corresponding fds.
         try:
-            import ida_idaapi
-        except ImportError:
-            self._stdin  = ql_file('stdin',  sys.stdin.fileno())
-            self._stdout = ql_file('stdout', sys.stdout.fileno())
-            self._stderr = ql_file('stderr', sys.stderr.fileno())
-        else:
+            # Qiling may be used on interactive shells (ex: IDLE) or embedded python
+            # interpreters (ex: IDA Python). such environments use their own version
+            # for the standard streams which usually do not support certain operations,
+            # such as fileno(). here we use this to determine how we are going to use
+            # the environment standard streams
+            sys.stdin.fileno()
+        except UnsupportedOperation:
+            # Qiling is used on an interactive shell or embedded python interpreter.
+            # if the internal stream buffer is accessible, we should use it
             self._stdin  = getattr(sys.stdin,  'buffer', sys.stdin)
             self._stdout = getattr(sys.stdout, 'buffer', sys.stdout)
             self._stderr = getattr(sys.stderr, 'buffer', sys.stderr)
+        else:
+            # Qiling is used in a script, or on an environment that supports ordinary
+            # stanard streams
+            self._stdin  = PersistentQlFile('stdin',  sys.stdin.fileno())
+            self._stdout = PersistentQlFile('stdout', sys.stdout.fileno())
+            self._stderr = PersistentQlFile('stderr', sys.stderr.fileno())
 
         # defult exit point
         self.exit_point = {
             16: 0xfffff,            # 20bit address lane
             32: 0x8fffffff,
             64: 0xffffffffffffffff
         }.get(self.ql.arch.bits, None)
@@ -191,24 +201,26 @@
 
         # print
         self.utils.print_function(pc, func.__name__, pargs, retval, passthru)
 
         # append syscall to list
         self.stats.log_api_call(pc, func.__name__, args, retval, retaddr)
 
-        # [Windows and UEFI] if emulation has stopped, do not update the return address
-        if hasattr(self, 'PE_RUN') and not self.PE_RUN:
-            passthru = True
-
         if not passthru:
-            self.ql.arch.regs.arch_pc = retaddr
+            # WORKAROUND: we avoid modifying the pc register in case the emulation has stopped.
+            # this is used to work around a unicorn issue in which emulation continues despite
+            # of calling emu_stop if the pc register is modified.
+            #
+            # see: https://github.com/unicorn-engine/unicorn/issues/1579
+            if self.ql.emu_state is not QL_STATE.STOPPED:
+                self.ql.arch.regs.arch_pc = retaddr
 
         return retval
 
-    def set_api(self, target: Hashable, handler: Callable, intercept: QL_INTERCEPT = QL_INTERCEPT.CALL):
+    def set_api(self, target: Union[int, str], handler: Callable, intercept: QL_INTERCEPT = QL_INTERCEPT.CALL):
         """Either hook or replace an OS API with a custom one.
 
         Args:
             target: target API identifier
             handler: function to call
             intercept:
                 `QL_INTERCEPT.CALL` : run handler instead of the existing target implementation
@@ -220,15 +232,15 @@
 
     # os main method; derivatives must implement one of their own
     def run(self) -> None:
         raise NotImplementedError
 
     def stop(self):
         if self.ql.multithread:
-            self.thread_management.stop() 
+            self.thread_management.stop()
         else:
             self.ql.emu_stop()
 
     def emu_error(self):
         self.ql.log.error(f'CPU Context:')
         for reg in self.ql.arch.regs.register_mapping:
             if isinstance(reg, str):
```

### Comparing `qiling-1.4.5/qiling/os/path.py` & `qiling-1.4.6/qiling/os/path.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 #!/usr/bin/env python3
-# 
+#
 # Cross Platform and Multi Architecture Advanced Binary Emulation Framework
 #
 
 from typing import Optional, Union
 from pathlib import Path, PurePosixPath, PureWindowsPath
 
 from qiling.const import QL_OS, QL_OS_POSIX
 
 AnyPurePath = Union[PurePosixPath, PureWindowsPath]
 
+
 class QlOsPath:
     """Virtual to host path manipulations helper.
     """
 
     def __init__(self, rootfs: str, cwd: str, emulos: QL_OS) -> None:
         """Initialize a path manipulation object.
 
@@ -57,14 +58,18 @@
 
             while path.parts[0] == pardir:
                 path = path.relative_to(pardir)
 
         return path
 
     @property
+    def root(self) -> str:
+        return str(self._cwd_anchor)
+
+    @property
     def cwd(self) -> str:
         return str(self._cwd_anchor / self._cwd_vpath)
 
     @cwd.setter
     def cwd(self, virtpath: str) -> None:
         vpath = self.PureVirtualPath(virtpath)
 
@@ -270,14 +275,26 @@
         """
 
         resolved = Path(hostpath).resolve(strict=False)
         virtpath = self._cwd_anchor / resolved.relative_to(self._rootfs_path)
 
         return str(virtpath)
 
+    def is_virtual_abspath(self, virtpath: str) -> bool:
+        """Determine whether a given virtual path is absolute.
+
+        Args:
+            virtpath : virtual path to query
+
+        Returns: `True` if `virtpath` is an absolute path, `False` if relative
+        """
+
+        vpath = self.PureVirtualPath(virtpath)
+
+        return vpath.is_absolute()
 
     def virtual_abspath(self, virtpath: str) -> str:
         """Convert a relative virtual path to an absolute virtual path based
         on the current working directory.
 
         Args:
             virtpath : relative virtual path
@@ -342,8 +359,7 @@
         """
 
         # only relevant if the emulated file system is NT-based
         if self.PureVirtualPath is PureWindowsPath:
             return QlOsPath.__host_casefold_path(hostpath)
 
         return hostpath
-
```

### Comparing `qiling-1.4.5/qiling/os/posix/const.py` & `qiling-1.4.6/qiling/os/posix/const.py`

 * *Files 14% similar despite different names*

```diff
@@ -107,50 +107,50 @@
     "IP_DROP_SOURCE_MEMBERSHIP" : 0x0028,
     "IP_MSFILTER"               : 0x0029,
     "IP_MULTICAST_ALL"          : 0x0031,
 }
 
 # https://github.com/torvalds/linux/blob/master/include/uapi/linux/tcp.h
 linux_socket_tcp_options = {
-    "TCP_NODELAY"				: 0x1,
-    "TCP_MAXSEG"				: 0x2,
-    "TCP_CORK"					: 0x3,
-    "TCP_KEEPIDLE"				: 0x4,
-    "TCP_KEEPINTVL"				: 0x5,
-    "TCP_KEEPCNT"				: 0x6,
-    "TCP_SYNCNT"				: 0x7,
-    "TCP_LINGER2"				: 0x8,
-    "TCP_DEFER_ACCEPT"			: 0x9,
-    "TCP_WINDOW_CLAMP"			: 0xa,
-    "TCP_INFO"					: 0xb,
-    "TCP_QUICKACK"				: 0xc,
-    "TCP_CONGESTION"			: 0xd,
-    "TCP_MD5SIG"				: 0xe,
-    "TCP_THIN_LINEAR_TIMEOUTS"	: 0x10,
-    "TCP_THIN_DUPACK"			: 0x11,
-    "TCP_USER_TIMEOUT"			: 0x12,
-    "TCP_REPAIR"				: 0x13,
-    "TCP_REPAIR_QUEUE"			: 0x14,
-    "TCP_QUEUE_SEQ"				: 0x15,
-    "TCP_REPAIR_OPTIONS"		: 0x16,
-    "TCP_FASTOPEN"				: 0x17,
-    "TCP_TIMESTAMP"				: 0x18,
-    "TCP_NOTSENT_LOWAT"			: 0x19,
-    "TCP_CC_INFO"				: 0x1a,
-    "TCP_SAVE_SYN"				: 0x1b,
-    "TCP_SAVED_SYN"				: 0x1c,
-    "TCP_REPAIR_WINDOW"			: 0x1d,
-    "TCP_FASTOPEN_CONNECT"		: 0x1e,
-    "TCP_ULP"					: 0x1f,
-    "TCP_MD5SIG_EXT"			: 0x20,
-    "TCP_FASTOPEN_KEY"			: 0x21,
-    "TCP_FASTOPEN_NO_COOKIE"	: 0x22,
-    "TCP_ZEROCOPY_RECEIVE"		: 0x23,
-    "TCP_INQ"					: 0x24,
-    "TCP_TX_DELAY"				: 0x25,
+    "TCP_NODELAY"                : 0x1,
+    "TCP_MAXSEG"                : 0x2,
+    "TCP_CORK"                    : 0x3,
+    "TCP_KEEPIDLE"                : 0x4,
+    "TCP_KEEPINTVL"                : 0x5,
+    "TCP_KEEPCNT"                : 0x6,
+    "TCP_SYNCNT"                : 0x7,
+    "TCP_LINGER2"                : 0x8,
+    "TCP_DEFER_ACCEPT"            : 0x9,
+    "TCP_WINDOW_CLAMP"            : 0xa,
+    "TCP_INFO"                    : 0xb,
+    "TCP_QUICKACK"                : 0xc,
+    "TCP_CONGESTION"            : 0xd,
+    "TCP_MD5SIG"                : 0xe,
+    "TCP_THIN_LINEAR_TIMEOUTS"    : 0x10,
+    "TCP_THIN_DUPACK"            : 0x11,
+    "TCP_USER_TIMEOUT"            : 0x12,
+    "TCP_REPAIR"                : 0x13,
+    "TCP_REPAIR_QUEUE"            : 0x14,
+    "TCP_QUEUE_SEQ"                : 0x15,
+    "TCP_REPAIR_OPTIONS"        : 0x16,
+    "TCP_FASTOPEN"                : 0x17,
+    "TCP_TIMESTAMP"                : 0x18,
+    "TCP_NOTSENT_LOWAT"            : 0x19,
+    "TCP_CC_INFO"                : 0x1a,
+    "TCP_SAVE_SYN"                : 0x1b,
+    "TCP_SAVED_SYN"                : 0x1c,
+    "TCP_REPAIR_WINDOW"            : 0x1d,
+    "TCP_FASTOPEN_CONNECT"        : 0x1e,
+    "TCP_ULP"                    : 0x1f,
+    "TCP_MD5SIG_EXT"            : 0x20,
+    "TCP_FASTOPEN_KEY"            : 0x21,
+    "TCP_FASTOPEN_NO_COOKIE"    : 0x22,
+    "TCP_ZEROCOPY_RECEIVE"        : 0x23,
+    "TCP_INQ"                    : 0x24,
+    "TCP_TX_DELAY"                : 0x25,
 }
 
 macos_socket_ip_options = {
     "IP_TOS"                   : 0x0003,
     "IP_TTL"                   : 0x0004,
     "IP_HDRINCL"               : 0x0002,
     "IP_OPTIONS"               : 0x0001,
@@ -719,22 +719,22 @@
     MAP_ANONYMOUS  = 0x00080000
     MAP_SYSRAM     = 0x01000000
 
     # define this alias for compatibility with other os flags
     MAP_UNINITIALIZED = MAP_NOINIT
 
 # fcntl flags
-F_DUPFD		= 0
-F_GETFD		= 1
-F_SETFD		= 2
-F_GETFL		= 3
-F_SETFL		= 4
-F_GETLK		= 5
-F_SETLK		= 6
-F_SETLKW	= 7
+F_DUPFD        = 0
+F_GETFD        = 1
+F_SETFD        = 2
+F_GETFL        = 3
+F_SETFL        = 4
+F_GETLK        = 5
+F_SETLK        = 6
+F_SETLKW    = 7
 
 FD_CLOEXEC = 1
 
 AT_FDCWD = -100
 AT_EMPTY_PATH = 0x1000
 
 # error code
@@ -999,15 +999,51 @@
     128: 'EKEYREVOKED',
     129: 'EKEYREJECTED',
     130: 'EOWNERDEAD',
     131: 'ENOTRECOVERABLE',
 }
 
 # shm syscall
-IPC_CREAT = 8**3
-IPC_EXCL = 2*(8**3)
-IPC_NOWAIT = 4*(8**3)
-
-SHM_RDONLY = 8**4
-SHM_RND = 2*(8**4)
-SHM_REMAP= 4*(8**4)
-SHM_EXEC = 1*(8**5)
+IPC_PRIVATE = 0
+
+# see: https://elixir.bootlin.com/linux/v5.19.17/source/include/uapi/linux/ipc.h
+IPC_CREAT  = 0o0001000  # create if key is nonexistent
+IPC_EXCL   = 0o0002000  # fail if key exists
+IPC_NOWAIT = 0o0004000  # return error on wait
+
+# see: https://elixir.bootlin.com/linux/v5.19.17/source/include/uapi/linux/shm.h
+SHM_W       = 0o000200
+SHM_R       = 0o000400
+SHM_HUGETLB = 0o004000  # segment will use huge TLB pages
+SHM_RDONLY	= 0o010000  # read-only access
+SHM_RND		= 0o020000	# round attach address to SHMLBA boundary
+SHM_REMAP	= 0o040000	# take-over region on attach
+SHM_EXEC	= 0o100000	# execution access
+
+SHMMNI = 4096   # max num of segs system wide
+
+# see: https://elixir.bootlin.com/linux/v5.19.17/source/include/uapi/asm-generic/hugetlb_encode.h
+HUGETLB_FLAG_ENCODE_SHIFT = 26
+HUGETLB_FLAG_ENCODE_MASK  = 0x3f
+
+# see: https://elixir.bootlin.com/linux/v5.19.17/source/include/uapi/linux/msg.h
+MSG_NOERROR = 0o10000  # no error if message is too big
+MSG_EXCEPT = 0o20000  # recv any msg except of specified type
+MSG_COPY = 0o40000  # copy (not remove) all queue messages
+
+MSGMNI = 32000 # <= IPCMNI, max # of msg queue identifiers
+MSGMAX = 8192 # <= INT_MAX, max size of message (bytes)
+MSGMNB = 16384 # <= INT_MAX, default max size of a message queue
+
+# ipc syscall
+SEMOP       = 1
+SEMGET      = 2
+SEMCTL      = 3
+SEMTIMEDOP  = 4
+MSGSND      = 11
+MSGRCV      = 12
+MSGGET      = 13
+MSGCTL      = 14
+SHMAT       = 21
+SHMDT       = 22
+SHMGET      = 23
+SHMCTL      = 24
```

### Comparing `qiling-1.4.5/qiling/os/posix/const_mapping.py` & `qiling-1.4.6/qiling/os/posix/const_mapping.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,20 +152,21 @@
     }[archtype]
 
     return _constant_mapping(p, socket_domain_map)
 
 
 def socket_tcp_option_mapping(t: int, archtype: QL_ARCH) -> str:
     socket_option_map = {
-        QL_ARCH.X86: linux_socket_tcp_options,
+        QL_ARCH.X86:   linux_socket_tcp_options,
         QL_ARCH.X8664: linux_socket_tcp_options,
-        QL_ARCH.ARM: linux_socket_tcp_options,
+        QL_ARCH.ARM:   linux_socket_tcp_options,
         QL_ARCH.ARM64: linux_socket_tcp_options,
-        QL_ARCH.MIPS: linux_socket_tcp_options,
+        QL_ARCH.MIPS:  linux_socket_tcp_options,
     }[archtype]
+
     return _constant_mapping(t, socket_option_map)
 
 
 def socket_level_mapping(t: int, archtype: QL_ARCH) -> str:
     socket_level_map = {
         QL_ARCH.X86:   linux_x86_socket_level,
         QL_ARCH.X8664: linux_x86_socket_level,
```

### Comparing `qiling-1.4.5/qiling/os/posix/filestruct.py` & `qiling-1.4.6/qiling/os/posix/filestruct.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/os/posix/posix.py` & `qiling-1.4.6/qiling/os/posix/posix.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #!/usr/bin/env python3
-# 
+#
 # Cross Platform and Multi Architecture Advanced Binary Emulation Framework
 #
 
+from collections import deque
 from inspect import signature, Parameter
-from typing import TextIO, Union, Callable, IO, List, Optional
+from typing import Dict, TextIO, Tuple, Union, Callable, IO, List, Optional
 
 from unicorn.arm64_const import UC_ARM64_REG_X8, UC_ARM64_REG_X16
 from unicorn.arm_const import (
     UC_ARM_REG_R0, UC_ARM_REG_R1, UC_ARM_REG_R2, UC_ARM_REG_R3,
     UC_ARM_REG_R4, UC_ARM_REG_R5, UC_ARM_REG_R7, UC_ARM_REG_R12
 )
 from unicorn.mips_const import UC_MIPS_REG_V0
@@ -22,15 +23,15 @@
 from unicorn.ppc_const import UC_PPC_REG_0
 
 from qiling import Qiling
 from qiling.cc import QlCC, intel, arm, mips, riscv, ppc
 from qiling.const import QL_ARCH, QL_OS, QL_INTERCEPT
 from qiling.exception import QlErrorSyscallNotFound
 from qiling.os.os import QlOs
-from qiling.os.posix.const import NR_OPEN, errors
+from qiling.os.posix.const import MSGMNB, NR_OPEN, errors
 from qiling.utils import ql_get_module, ql_get_module_function
 
 SYSCALL_PREF: str = f'ql_syscall_'
 
 class intel32(intel.QlIntel32):
     _argregs = (UC_X86_REG_EBX, UC_X86_REG_ECX, UC_X86_REG_EDX, UC_X86_REG_ESI, UC_X86_REG_EDI, UC_X86_REG_EBP)
 
@@ -68,15 +69,15 @@
 class QlFileDes:
     def __init__(self):
         self.__fds: List[Optional[IO]] = [None] * NR_OPEN
 
     def __len__(self):
         return len(self.__fds)
 
-    def __getitem__(self, idx: Union[slice, int]):
+    def __getitem__(self, idx: int):
         return self.__fds[idx]
 
     def __setitem__(self, idx: int, val: Optional[IO]):
         self.__fds[idx] = val
 
     def __iter__(self):
         return iter(self.__fds)
@@ -87,14 +88,106 @@
     def save(self):
         return self.__fds
 
     def restore(self, fds):
         self.__fds = fds
 
 
+# vaguely reflects a shmid64_ds structure
+class QlShmId:
+
+    def __init__(self, key: int, uid: int, gid: int, mode: int, segsz: int) -> None:
+        # ipc64_perm
+        self.key = key
+        self.uid = uid
+        self.gid = gid
+        self.mode = mode
+
+        self.segsz = segsz
+
+        # track the memory locations this segment is currently attached to
+        self.attach: List[int] = []
+
+
+class QlShm:
+    def __init__(self) -> None:
+        self.__shm: Dict[int, QlShmId] = {}
+        self.__id: int = 0x0F000000
+
+    def __len__(self) -> int:
+        return len(self.__shm)
+
+    def add(self, shm: QlShmId) -> int:
+        shmid = self.__id
+        self.__shm[shmid] = shm
+
+        self.__id += 0x1000
+
+        return shmid
+
+    def remove(self, shmid: int) -> None:
+        del self.__shm[shmid]
+
+    def get_by_key(self, key: int) -> Tuple[int, Optional[QlShmId]]:
+        return next(((shmid, shmobj) for shmid, shmobj in self.__shm.items() if shmobj.key == key), (-1, None))
+
+    def get_by_id(self, shmid: int) -> Optional[QlShmId]:
+        return self.__shm.get(shmid, None)
+
+    def get_by_attaddr(self, shmaddr: int) -> Optional[QlShmId]:
+        return next((shmobj for shmobj in self.__shm.values() if shmobj.attach.count(shmaddr) > 0), None)
+
+
+class QlMsgBuf:
+    def __init__(self, mtype: int, mtext: bytes) -> None:
+        self.mtype = mtype
+        self.mtext = mtext
+
+
+# vaguely reflects a msqid64_ds structure
+class QlMsqId:
+    def __init__(self, key: int, uid: int, gid: int, mode: int) -> None:
+        # ipc64_perm
+        self.key = key
+        self.uid = uid
+        self.gid = gid
+        self.mode = mode
+
+        self.queue = deque(maxlen=MSGMNB)
+    
+    def __len__(self):
+        return len(self.queue)
+
+
+class QlMsq:
+    def __init__(self) -> None:
+        self.__msq: Dict[int, QlMsqId] = {}
+        self.__id: int = 0x0F000000
+
+    def __len__(self) -> int:
+        return len(self.__msq)
+
+    def add(self, msq: QlMsqId) -> int:
+        msqid = self.__id
+        self.__msq[msqid] = msq
+
+        self.__id += 0x1000
+
+        return msqid
+
+    def remove(self, msqid: int) -> None:
+        del self.__msq[msqid]
+
+    def get_by_key(self, key: int) -> Tuple[int, Optional[QlMsqId]]:
+        return next(((msqid, msqobj) for msqid, msqobj in self.__msq.items() if msqobj.key == key), (-1, None))
+
+    def get_by_id(self, msqid: int) -> Optional[QlMsqId]:
+        return self.__msq.get(msqid, None)
+    
+
 class QlOsPosix(QlOs):
 
     def __init__(self, ql: Qiling):
         super().__init__(ql)
 
         self.ql = ql
         self.sigaction_act = [0] * 256
@@ -106,17 +199,17 @@
 
         conf = self.profile['NETWORK']
         self.ipv6 = conf.getboolean('ipv6')
         self.bindtolocalhost = conf.getboolean('bindtolocalhost')
         self.ifrname_ovr = conf.get('ifrname_override')
 
         self.posix_syscall_hooks = {
-            QL_INTERCEPT.CALL : {},
+            QL_INTERCEPT.CALL:  {},
             QL_INTERCEPT.ENTER: {},
-            QL_INTERCEPT.EXIT : {}
+            QL_INTERCEPT.EXIT:  {}
         }
 
         self.__syscall_id_reg = {
             QL_ARCH.ARM64   : UC_ARM64_REG_X8,
             QL_ARCH.ARM     : UC_ARM_REG_R7,
             QL_ARCH.MIPS    : UC_MIPS_REG_V0,
             QL_ARCH.X86     : UC_X86_REG_EAX,
@@ -153,15 +246,16 @@
         # the QlOs constructor cannot assign the standard streams using their designated properties since
         # it runs before the _fd array is declared. instead, it assigns them to the private members and here
         # we force _fd to update manually.
         self.stdin  = self._stdin
         self.stdout = self._stdout
         self.stderr = self._stderr
 
-        self._shms = {}
+        self._shm = QlShm()
+        self._msq = QlMsq()
 
     def __get_syscall_mapper(self, archtype: QL_ARCH):
         qlos_path = f'.os.{self.type.name.lower()}.map_syscall'
         qlos_func = 'get_syscall_mapper'
 
         func = ql_get_module_function(qlos_path, qlos_func)
 
@@ -187,15 +281,15 @@
         return (self.euid == 0) and (self.egid == 0)
 
     @QlOs.root.setter
     def root(self, enabled: bool) -> None:
         self.euid = 0 if enabled else self.uid
         self.egid = 0 if enabled else self.gid
 
-    def set_syscall(self, target: Union[int, str], handler: Callable, intercept: QL_INTERCEPT=QL_INTERCEPT.CALL):
+    def set_syscall(self, target: Union[int, str], handler: Callable, intercept: QL_INTERCEPT = QL_INTERCEPT.CALL):
         """Either hook or replace a system call with a custom one.
 
         Args:
             target: either syscall name or number. a name may be used only if target syscall is implemented
             handler: function to call
             intercept:
                 `QL_INTERCEPT.CALL` : run handler instead of the existing target implementation
@@ -265,22 +359,22 @@
             # skip first arg (always 'ql') and filter out python special args (*args and **kwargs)
             param_names = [info.name for info in param_names[1:] if info.kind == Parameter.POSITIONAL_OR_KEYWORD]
 
             # read parameter values
             params = [self.__syscall_cc.getRawParam(i) for i in range(len(param_names))]
 
             try:
-        		# if set, fire up the on-enter hook and let it override original args set
+                # if set, fire up the on-enter hook and let it override original args set
                 if onenter_hook:
                     overrides = onenter_hook(self.ql, *params)
 
                     if overrides is not None:
                         _, params = overrides
 
-        		# perform syscall
+                # perform syscall
                 retval = syscall_hook(self.ql, *params)
 
                 # if set, fire up the on-exit hook and let it override the return value
                 if onexit_hook:
                     override = onexit_hook(self.ql, *params, retval)
 
                     if override is not None:
@@ -294,15 +388,15 @@
                 raise
 
             except Exception as e:
                 self.ql.log.exception(f'Syscall ERROR: {syscall_name} DEBUG: {e}')
                 raise e
 
             # print out log entry
-            syscall_basename = syscall_name[len(SYSCALL_PREF) if syscall_name.startswith(SYSCALL_PREF) else 0:] 
+            syscall_basename = syscall_name[len(SYSCALL_PREF) if syscall_name.startswith(SYSCALL_PREF) else 0:]
 
             args = []
 
             for name, value in zip(param_names, params):
                 # cut the first part of the arg if it is of form fstatat64_fd
                 if name.startswith(f'{syscall_basename}_'):
                     name = name.partition('_')[-1]
@@ -345,7 +439,15 @@
 
     def set_syscall_return(self, retval: int):
         self.__syscall_cc.setReturnValue(retval)
 
     @property
     def fd(self):
         return self._fd
+
+    @property
+    def shm(self):
+        return self._shm
+
+    @property
+    def msq(self):
+        return self._msq
```

### Comparing `qiling-1.4.5/qiling/os/posix/stat.py` & `qiling-1.4.6/qiling/os/posix/stat.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/os/posix/structs.py` & `qiling-1.4.6/qiling/os/posix/structs.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/os/posix/syscall/__init__.py` & `qiling-1.4.6/qiling/os/posix/syscall/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,28 +2,31 @@
 #
 # Cross Platform and Multi Architecture Advanced Binary Emulation Framework
 #
 from .fcntl import *
 from .futex import *
 from .ioctl import *
 from .mman import *
+from .msg import *
 from .net import *
 from .personality import *
 from .poll import *
 from .prctl import *
 from .ptrace import *
 from .random import *
 from .resource import *
 from .sched import *
 from .select import *
 from .sendfile import *
+from .shm import *
 from .signal import *
 from .socket import *
 from .stat import *
 from .sysctl import *
+from .syscall import *
 from .sysinfo import *
 from .time import *
 from .types import *
 from .uio import *
 from .unistd import *
 from .utsname import *
 from .wait import *
```

### Comparing `qiling-1.4.5/qiling/os/posix/syscall/fcntl.py` & `qiling-1.4.6/qiling/os/posix/syscall/fcntl.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,153 +1,129 @@
 #!/usr/bin/env python3
 #
 # Cross Platform and Multi Architecture Advanced Binary Emulation Framework
 #
 
 import os
-from pathlib import Path
 
 from qiling import Qiling
 from qiling.const import QL_OS, QL_ARCH
 from qiling.exception import QlSyscallError
 from qiling.os.posix.const import *
 from qiling.os.posix.const_mapping import ql_open_flag_mapping
 from qiling.os.posix.filestruct import ql_socket
 
-def ql_syscall_open(ql: Qiling, filename: int, flags: int, mode: int):
-    path = ql.os.utils.read_cstring(filename)
-    real_path = ql.os.path.transform_to_real_path(path)
-    relative_path = ql.os.path.transform_to_relative_path(path)
+from .unistd import virtual_abspath_at, get_opened_fd
+
 
+def __do_open(ql: Qiling, absvpath: str, flags: int, mode: int) -> int:
     flags &= 0xffffffff
     mode &= 0xffffffff
 
+    # look for the next available fd slot
     idx = next((i for i in range(NR_OPEN) if ql.os.fd[i] is None), -1)
 
     if idx == -1:
-        regreturn = -EMFILE
-    else:
-        try:
-            if ql.arch.type == QL_ARCH.ARM and ql.os.type != QL_OS.QNX:
-                mode = 0
+        return -EMFILE
 
-            flags = ql_open_flag_mapping(ql, flags)
-            ql.os.fd[idx] = ql.os.fs_mapper.open_ql_file(path, flags, mode)
-            regreturn = idx
-        except QlSyscallError as e:
-            regreturn = - e.errno
+    if ql.arch.type is QL_ARCH.ARM and ql.os.type is not QL_OS.QNX:
+        mode = 0
 
+    # translate emulated os open flags into host os open flags
+    flags = ql_open_flag_mapping(ql, flags)
 
-    ql.log.debug("open(%s, 0o%o) = %d" % (relative_path, mode, regreturn))
+    try:
+        ql.os.fd[idx] = ql.os.fs_mapper.open_ql_file(absvpath, flags, mode)
+    except QlSyscallError:
+        return -1
 
-    if regreturn >= 0 and regreturn != 2:
-        ql.log.debug(f'File found: {real_path:s}')
-    else:
-        ql.log.debug(f'File not found {real_path:s}')
+    return idx
 
-    return regreturn
 
-def ql_syscall_creat(ql: Qiling, filename: int, mode: int):
-    flags = posix_open_flags["O_WRONLY"] | posix_open_flags["O_CREAT"] | posix_open_flags["O_TRUNC"]
+def ql_syscall_open(ql: Qiling, filename: int, flags: int, mode: int):
+    vpath = ql.os.utils.read_cstring(filename)
+    absvpath = ql.os.path.virtual_abspath(vpath)
 
-    path = ql.os.utils.read_cstring(filename)
-    real_path = ql.os.path.transform_to_real_path(path)
-    relative_path = ql.os.path.transform_to_relative_path(path)
+    regreturn = __do_open(ql, absvpath, flags, mode)
 
-    flags &= 0xffffffff
-    mode &= 0xffffffff
+    ql.log.debug(f'open("{absvpath}", {flags:#x}, 0{mode:o}) = {regreturn}')
 
-    idx = next((i for i in range(NR_OPEN) if ql.os.fd[i] is None), -1)
+    return regreturn
 
-    if idx == -1:
-        regreturn = -ENOMEM 
-    else:
-        try:
-            if ql.arch.type == QL_ARCH.ARM:
-                mode = 0
 
-            flags = ql_open_flag_mapping(ql, flags)
-            ql.os.fd[idx] = ql.os.fs_mapper.open_ql_file(path, flags, mode)
-            regreturn = idx
-        except QlSyscallError as e:
-            regreturn = -e.errno
+def ql_syscall_openat(ql: Qiling, fd: int, path: int, flags: int, mode: int):
+    vpath = ql.os.utils.read_cstring(path)
+    absvpath = virtual_abspath_at(ql, vpath, fd)
 
-    ql.log.debug("creat(%s, 0o%o) = %d" % (relative_path, mode, regreturn))
+    regreturn = -1 if absvpath is None else __do_open(ql, absvpath, flags, mode)
 
-    if regreturn >= 0 and regreturn != 2:
-        ql.log.debug(f'File found: {real_path:s}')
-    else:
-        ql.log.debug(f'File not found {real_path:s}')
+    ql.log.debug(f'openat({fd:d}, "{vpath}", {flags:#x}, 0{mode:o}) = {regreturn:d}')
 
     return regreturn
 
-def ql_syscall_openat(ql: Qiling, fd: int, path: int, flags: int, mode: int):
-    file_path = ql.os.utils.read_cstring(path)
-    # real_path = ql.os.path.transform_to_real_path(path)
-    # relative_path = ql.os.path.transform_to_relative_path(path)
 
-    flags &= 0xffffffff
+def ql_syscall_creat(ql: Qiling, filename: int, mode: int):
+    vpath = ql.os.utils.read_cstring(filename)
+
+    # FIXME: this is broken
+    flags = posix_open_flags["O_WRONLY"] | posix_open_flags["O_CREAT"] | posix_open_flags["O_TRUNC"]
     mode &= 0xffffffff
 
     idx = next((i for i in range(NR_OPEN) if ql.os.fd[i] is None), -1)
 
     if idx == -1:
-        regreturn = -EMFILE
+        regreturn = -ENOMEM
     else:
-        try:
-            if ql.arch.type == QL_ARCH.ARM:
-                mode = 0
+        if ql.arch.type == QL_ARCH.ARM:
+            mode = 0
 
+        try:
             flags = ql_open_flag_mapping(ql, flags)
-            fd = ql.unpacks(ql.pack(fd))
+            ql.os.fd[idx] = ql.os.fs_mapper.open_ql_file(vpath, flags, mode)
+        except QlSyscallError as e:
+            regreturn = -e.errno
+        else:
+            regreturn = idx
 
-            if 0 <= fd < NR_OPEN:
-                fobj = ql.os.fd[fd]
-                # ql_file object or QlFsMappedObject
-                if hasattr(fobj, "fileno") and hasattr(fobj, "name"):
-                    if not Path.is_absolute(Path(file_path)):
-                        file_path = Path(fobj.name) / Path(file_path)
+    hpath = ql.os.path.virtual_to_host_path(vpath)
+    absvpath = ql.os.path.virtual_abspath(vpath)
 
-            ql.os.fd[idx] = ql.os.fs_mapper.open_ql_file(file_path, flags, mode)
+    ql.log.debug(f'creat("{absvpath}", {mode:#o}) = {regreturn}')
 
-            regreturn = idx
-        except QlSyscallError as e:
-            regreturn = -e.errno
-            
-    ql.log.debug(f'openat(fd = {fd:d}, path = {file_path}, mode = {mode:#o}) = {regreturn:d}')
+    if regreturn >= 0 and regreturn != 2:
+        ql.log.debug(f'File found: {hpath:s}')
+    else:
+        ql.log.debug(f'File not found {hpath:s}')
 
     return regreturn
 
 
 def ql_syscall_fcntl(ql: Qiling, fd: int, cmd: int, arg: int):
-    if fd not in range(NR_OPEN):
-        return -EBADF
-
-    f = ql.os.fd[fd]
+    f = get_opened_fd(ql.os, fd)
 
     if f is None:
-        return -EBADF
+        return -1
 
     if cmd == F_DUPFD:
         if arg not in range(NR_OPEN):
             regreturn = -EINVAL
 
         for idx in range(arg, len(ql.os.fd)):
             if ql.os.fd[idx] is None:
                 ql.os.fd[idx] = f.dup()
                 regreturn = idx
                 break
         else:
             regreturn = -EMFILE
 
     elif cmd == F_GETFD:
-        regreturn = getattr(f, "close_on_exec", 0)
+        regreturn = int(getattr(f, "close_on_exec", False))
 
     elif cmd == F_SETFD:
-        f.close_on_exec = 1 if arg & FD_CLOEXEC else 0
+        f.close_on_exec = bool(arg & FD_CLOEXEC)
         regreturn = 0
 
     elif cmd == F_GETFL:
         regreturn = f.fcntl(cmd, arg)
 
     elif cmd == F_SETFL:
         flags = ql_open_flag_mapping(ql, arg)
@@ -205,32 +181,40 @@
 def ql_syscall_flock(ql: Qiling, fd: int, operation: int):
     # Should always return 0, we don't need a actual file lock
 
     return 0
 
 
 def ql_syscall_rename(ql: Qiling, oldname_buf: int, newname_buf: int):
-    """
-    rename(const char *oldpath, const char *newpath)
-    description: change the name or location of a file
-    ret value: On success, zero is returned. On error, -1 is returned
-    """
-    regreturn = 0  # default value is success
-    oldpath = ql.os.utils.read_cstring(oldname_buf)
-    newpath = ql.os.utils.read_cstring(newname_buf)
-
-    ql.log.debug(f"rename() path: {oldpath} -> {newpath}")
-
-    old_realpath = ql.os.path.transform_to_real_path(oldpath)
-    new_realpath = ql.os.path.transform_to_real_path(newpath)
-
-    if old_realpath == new_realpath:
-        # do nothing, just return success
-        return regreturn
+    old_vpath = ql.os.utils.read_cstring(oldname_buf)
+    new_vpath = ql.os.utils.read_cstring(newname_buf)
 
-    try:
-        os.rename(old_realpath, new_realpath)
-    except OSError:
-        ql.log.exception(f"rename(): {newpath} exists!")
-        regreturn = -1
+    old_absvpath = ql.os.path.virtual_abspath(old_vpath)
+
+    # if has a mapping, rename the mapped vpath
+    if ql.os.fs_mapper.has_mapping(old_absvpath):
+        try:
+            ql.os.fs_mapper.rename_mapping(old_vpath, new_vpath)
+        except KeyError:
+            regreturn = -1
+        else:
+            regreturn = 0
+
+    # otherwise, rename the actual files
+    else:
+        old_hpath = ql.os.path.virtual_to_host_path(old_vpath)
+        new_hpath = ql.os.path.virtual_to_host_path(new_vpath)
+
+        # if source and target paths are identical, do nothing
+        if old_hpath == new_hpath:
+            return 0
+
+        try:
+            os.rename(old_hpath, new_hpath)
+        except OSError:
+            regreturn = -1
+        else:
+            regreturn = 0
 
-    return regreturn
+    ql.log.debug(f'rename("{old_vpath}", "{new_vpath}") = {regreturn}')
+
+    return regreturn
```

### Comparing `qiling-1.4.5/qiling/os/posix/syscall/futex.py` & `qiling-1.4.6/qiling/os/posix/syscall/futex.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/os/posix/syscall/ioctl.py` & `qiling-1.4.6/qiling/os/posix/syscall/ioctl.py`

 * *Files 3% similar despite different names*

```diff
@@ -57,18 +57,18 @@
         if allowed:
             if _cmd == TCGETS:
                 return 0, 0, 0, 0
 
             elif _cmd == TIOCGWINSZ:
                 # struct winsize
                 # {
-                #   unsigned short ws_row;	/* rows, in characters */
-                #   unsigned short ws_col;	/* columns, in characters */
-                #   unsigned short ws_xpixel;	/* horizontal size, pixels */
-                #   unsigned short ws_ypixel;	/* vertical size, pixels */
+                #   unsigned short ws_row;    /* rows, in characters */
+                #   unsigned short ws_col;    /* columns, in characters */
+                #   unsigned short ws_xpixel;    /* horizontal size, pixels */
+                #   unsigned short ws_ypixel;    /* vertical size, pixels */
                 # };
                 return 1000, 360, 1000, 1000
 
             elif _cmd == TIOCSWINSZ:
                 # Ignore it
                 return None
```

### Comparing `qiling-1.4.5/qiling/os/posix/syscall/mman.py` & `qiling-1.4.6/qiling/os/posix/syscall/mman.py`

 * *Files 8% similar despite different names*

```diff
@@ -221,37 +221,7 @@
 
 
 def ql_syscall_mmap2(ql: Qiling, addr: int, length: int, prot: int, flags: int, fd: int, pgoffset: int):
     if ql.os.type != QL_OS.QNX:
         pgoffset *= ql.mem.pagesize
 
     return syscall_mmap_impl(ql, addr, length, prot, flags, fd, pgoffset, 2)
-
-
-def ql_syscall_shmget(ql: Qiling, key: int, size: int, shmflg: int):
-    if shmflg & IPC_CREAT:
-        if shmflg & IPC_EXCL:
-            if key in ql.os._shms:
-                return EEXIST
-        else:
-            #addr = ql.mem.map_anywhere(size)
-            ql.os._shms[key] = (key, size)
-            return key
-    else:
-        if key not in ql.os._shms:
-            return ENOENT
-
-
-def ql_syscall_shmat(ql: Qiling, shmid: int, shmaddr: int, shmflg: int):
-    # shmid == key
-    # dummy implementation
-    if shmid not in ql.os._shms:
-        return EINVAL
-
-    key, size = ql.os._shms[shmid]
-
-    if shmaddr == 0:
-        addr = ql.mem.map_anywhere(size)
-    else:
-        addr = ql.mem.map(shmaddr, size, info="[shm]")
-
-    return addr
```

### Comparing `qiling-1.4.5/qiling/os/posix/syscall/net.py` & `qiling-1.4.6/qiling/os/posix/syscall/net.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/os/posix/syscall/poll.py` & `qiling-1.4.6/qiling/os/posix/syscall/poll.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/os/posix/syscall/resource.py` & `qiling-1.4.6/qiling/os/posix/syscall/resource.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/os/posix/syscall/sched.py` & `qiling-1.4.6/qiling/os/posix/syscall/sched.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/os/posix/syscall/select.py` & `qiling-1.4.6/qiling/os/posix/syscall/select.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/os/posix/syscall/sendfile.py` & `qiling-1.4.6/qiling/os/posix/syscall/sendfile.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/os/posix/syscall/signal.py` & `qiling-1.4.6/qiling/os/posix/syscall/signal.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/os/posix/syscall/socket.py` & `qiling-1.4.6/qiling/os/posix/syscall/socket.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,18 +23,18 @@
 def inet_aton(ipaddr: str) -> int:
     # ipdata = bytes(int(a, 0) for a in ipaddr.split('.', 4))
     ipdata = ipaddress.IPv4Address(ipaddr).packed
 
     return int.from_bytes(ipdata, byteorder='big')
 
 
-def inet6_aton(ipaddr: str) -> int:
-    ipdata = ipaddress.IPv6Address(ipaddr).packed
+def inet6_aton(ipaddr: str) -> Tuple[int, ...]:
+    abytes = ipaddress.IPv6Address(ipaddr).packed
 
-    return int.from_bytes(ipdata, byteorder='big')
+    return tuple(abytes)
 
 
 def inet_htoa(ql: Qiling, addr: int) -> str:
     abytes = ql.pack32(addr)
 
     return ipaddress.IPv4Address(abytes).compressed
 
@@ -48,14 +48,18 @@
 def inet6_htoa(ql: Qiling, addr: bytes) -> str:
     # TODO: swap addr bytes order according to ql.arch.endian?
 
     return ipaddress.IPv6Address(addr).compressed
 
 
 def inet6_ntoa(addr: bytes) -> str:
+    # if addr arg is not strictly a bytes object, convert it to bytes
+    if not isinstance(addr, bytes):
+        addr = bytes(addr)
+
     return ipaddress.IPv6Address(addr).compressed
 
 
 def ntohs(ql: Qiling, nval: int) -> int:
     ebdata = nval.to_bytes(length=2, byteorder='big')
 
     return ql.unpack16(ebdata)
@@ -256,21 +260,21 @@
         port = ntohs(ql, sockaddr_obj.sin_port)
         host = inet_htoa(ql, sockaddr_obj.sin_addr.s_addr)
 
         ql.log.debug(f'Connecting to {host}:{port}')
         dest = (host, port)
 
     elif sock.family == AF_INET6 and ql.os.ipv6:
-        sockaddr_in6 = make_sockaddr_in(abits, endian)
+        sockaddr_in6 = make_sockaddr_in6(abits, endian)
         sockaddr_obj = sockaddr_in6.from_buffer(data)
 
-        port = ntohs(ql, sockaddr_obj.sin_port)
+        port = ntohs(ql, sockaddr_obj.sin6_port)
         host = inet6_htoa(ql, sockaddr_obj.sin6_addr.s6_addr)
 
-        ql.log.debug(f'Conecting to {host}:{port}')
+        ql.log.debug(f'Connecting to {host}:{port}')
         dest = (host, port)
 
     if dest is not None:
         try:
             sock.connect(dest)
         except (ConnectionError, FileNotFoundError):
             regreturn = -1
@@ -405,18 +409,18 @@
         if not ql.os.root and port <= 1024:
             port = port + 8000
 
         ql.log.debug(f'Binding socket to {host}:{port}')
         dest = (host, port)
 
     elif sa_family == AF_INET6 and ql.os.ipv6:
-        sockaddr_in6 = make_sockaddr_in(abits, endian)
+        sockaddr_in6 = make_sockaddr_in6(abits, endian)
         sockaddr_obj = sockaddr_in6.from_buffer(data)
 
-        port = ntohs(ql, sockaddr_obj.sin_port)
+        port = ntohs(ql, sockaddr_obj.sin6_port)
         host = inet6_ntoa(sockaddr_obj.sin6_addr.s6_addr)
 
         if ql.os.bindtolocalhost:
             host = '::1'
 
         if not ql.os.root and port <= 1024:
             port = port + 8000
@@ -875,18 +879,18 @@
         port = ntohs(ql, sockaddr_obj.sin_port)
         host = inet_ntoa(sockaddr_obj.sin_addr.s_addr)
 
         ql.log.debug(f'Sending {len(tmp_buf):d} bytes to {host}:{port}')
         dest = (host, port)
 
     elif sa_family == AF_INET6 and ql.os.ipv6:
-        sockaddr_in6 = make_sockaddr_in(abits, endian)
+        sockaddr_in6 = make_sockaddr_in6(abits, endian)
         sockaddr_obj = sockaddr_in6.from_buffer(data)
 
-        port = ntohs(ql, sockaddr_obj.sin_port)
+        port = ntohs(ql, sockaddr_obj.sin6_port)
         host = inet6_ntoa(sockaddr_obj.sin6_addr.s6_addr)
 
         ql.log.debug(f'Sending to {host}:{port}')
         dest = (host, port)
 
     if dest is not None:
         try:
```

### Comparing `qiling-1.4.5/qiling/os/posix/syscall/stat.py` & `qiling-1.4.6/qiling/os/posix/syscall/stat.py`

 * *Files 17% similar despite different names*

```diff
@@ -13,50 +13,50 @@
 from qiling.os.posix.const import NR_OPEN, EBADF, ENOENT, AT_FDCWD, AT_EMPTY_PATH
 from qiling.os.posix.stat import Stat, Lstat
 
 # Caveat: Never use types like ctypes.c_long whose size differs across platforms.
 
 # /sys/sys/stat.h
 # struct stat {
-# 	dev_t     st_dev;		/* inode's device */                        uint64_t
-# 	ino_t	  st_ino;		/* inode's number */                        uint64_t
-# 	nlink_t	  st_nlink;		/* number of hard links */                  uint64_t
-# 	mode_t	  st_mode;		/* inode protection mode */                 uint16_t
-# 	__int16_t st_padding0;                                              int16_t
-# 	uid_t	  st_uid;		/* user ID of the file's owner */           uint32_t
-# 	gid_t	  st_gid;		/* group ID of the file's group */          uint32_t
-# 	__int32_t st_padding1;                                              int32_t
-# 	dev_t     st_rdev;		/* device type */                           uint64_t
-# #ifdef	__STAT_TIME_T_EXT
-# 	__int32_t st_atim_ext;
+#     dev_t     st_dev;        /* inode's device */                        uint64_t
+#     ino_t      st_ino;        /* inode's number */                        uint64_t
+#     nlink_t      st_nlink;        /* number of hard links */                  uint64_t
+#     mode_t      st_mode;        /* inode protection mode */                 uint16_t
+#     __int16_t st_padding0;                                              int16_t
+#     uid_t      st_uid;        /* user ID of the file's owner */           uint32_t
+#     gid_t      st_gid;        /* group ID of the file's group */          uint32_t
+#     __int32_t st_padding1;                                              int32_t
+#     dev_t     st_rdev;        /* device type */                           uint64_t
+# #ifdef    __STAT_TIME_T_EXT
+#     __int32_t st_atim_ext;
 # #endif
-# 	struct	timespec st_atim;	/* time of last access */               uint64_t * 2      
-# #ifdef	__STAT_TIME_T_EXT
-# 	__int32_t st_mtim_ext;
+#     struct    timespec st_atim;    /* time of last access */               uint64_t * 2      
+# #ifdef    __STAT_TIME_T_EXT
+#     __int32_t st_mtim_ext;
 # #endif
-# 	struct	timespec st_mtim;	/* time of last data modification */    uint64_t * 2
-# #ifdef	__STAT_TIME_T_EXT
-# 	__int32_t st_ctim_ext;
+#     struct    timespec st_mtim;    /* time of last data modification */    uint64_t * 2
+# #ifdef    __STAT_TIME_T_EXT
+#     __int32_t st_ctim_ext;
 # #endif
-# 	struct	timespec st_ctim;	/* time of last file status change */   uint64_t * 2
-# #ifdef	__STAT_TIME_T_EXT
-# 	__int32_t st_btim_ext;
+#     struct    timespec st_ctim;    /* time of last file status change */   uint64_t * 2
+# #ifdef    __STAT_TIME_T_EXT
+#     __int32_t st_btim_ext;
 # #endif
-# 	struct	timespec st_birthtim;	/* time of file creation */         uint64_t * 2
-# 	off_t	  st_size;		/* file size, in bytes */                   int64_t
-# 	blkcnt_t st_blocks;		/* blocks allocated for file */             int64_t
-# 	blksize_t st_blksize;		/* optimal blocksize for I/O */         int32_t
-# 	fflags_t  st_flags;		/* user defined flags for file */           uint32_t
-# 	__uint64_t st_gen;		/* file generation number */                uint64_t
-# 	__uint64_t st_spare[10];                                            uint64_t * 10
+#     struct    timespec st_birthtim;    /* time of file creation */         uint64_t * 2
+#     off_t      st_size;        /* file size, in bytes */                   int64_t
+#     blkcnt_t st_blocks;        /* blocks allocated for file */             int64_t
+#     blksize_t st_blksize;        /* optimal blocksize for I/O */         int32_t
+#     fflags_t  st_flags;        /* user defined flags for file */           uint32_t
+#     __uint64_t st_gen;        /* file generation number */                uint64_t
+#     __uint64_t st_spare[10];                                            uint64_t * 10
 # };
 #
 # struct timespec {
-# 	time_t	tv_sec;		/* seconds */                                   uint64_t
-# 	long	tv_nsec;	/* and nanoseconds */                           uint64_t (LP64 data model)
+#     time_t    tv_sec;        /* seconds */                                   uint64_t
+#     long    tv_nsec;    /* and nanoseconds */                           uint64_t (LP64 data model)
 # };
 #
 #
 # Assume no EXT.
 class FreeBSDX86Stat(ctypes.Structure):
     _fields_ = [
         ("st_dev", ctypes.c_uint64),
@@ -126,29 +126,29 @@
 # #define __DARWIN_STRUCT_STAT64_TIMES \
 # struct timespec st_atimespec;           /* time of last access */ \
 # struct timespec st_mtimespec;           /* time of last data modification */ \
 # struct timespec st_ctimespec;           /* time of last status change */ \
 # struct timespec st_birthtimespec;       /* time of file creation(birth) */
 #
 # #define __DARWIN_STRUCT_STAT64 { \
-# 	dev_t		st_dev;                 /* [XSI] ID of device containing file */ \      int32_t
-# 	mode_t		st_mode;                /* [XSI] Mode of file (see below) */ \          uint16_t
-# 	nlink_t		st_nlink;               /* [XSI] Number of hard links */ \              uint16_t      
-# 	__darwin_ino64_t st_ino;                /* [XSI] File serial number */ \            uint64_t
-# 	uid_t		st_uid;                 /* [XSI] User ID of the file */ \               uint32_t
-# 	gid_t		st_gid;                 /* [XSI] Group ID of the file */ \              uint32_t
-# 	dev_t		st_rdev;                /* [XSI] Device ID */ \                         int32_t
-# 	__DARWIN_STRUCT_STAT64_TIMES \                                                      uint64_t (long) * 8
-# 	off_t		st_size;                /* [XSI] file size, in bytes */ \               int64_t
-# 	blkcnt_t	st_blocks;              /* [XSI] blocks allocated for file */ \         int64_t
-# 	blksize_t	st_blksize;             /* [XSI] optimal blocksize for I/O */ \         int32_t
-# 	__uint32_t	st_flags;               /* user defined flags for file */ \             uint32_t
-# 	__uint32_t	st_gen;                 /* file generation number */ \                  uint32_t
-# 	__int32_t	st_lspare;              /* RESERVED: DO NOT USE! */ \                   int32_t
-# 	__int64_t	st_qspare[2];           /* RESERVED: DO NOT USE! */ \                   int64_t * 2
+#     dev_t        st_dev;                 /* [XSI] ID of device containing file */ \      int32_t
+#     mode_t        st_mode;                /* [XSI] Mode of file (see below) */ \          uint16_t
+#     nlink_t        st_nlink;               /* [XSI] Number of hard links */ \              uint16_t      
+#     __darwin_ino64_t st_ino;                /* [XSI] File serial number */ \            uint64_t
+#     uid_t        st_uid;                 /* [XSI] User ID of the file */ \               uint32_t
+#     gid_t        st_gid;                 /* [XSI] Group ID of the file */ \              uint32_t
+#     dev_t        st_rdev;                /* [XSI] Device ID */ \                         int32_t
+#     __DARWIN_STRUCT_STAT64_TIMES \                                                      uint64_t (long) * 8
+#     off_t        st_size;                /* [XSI] file size, in bytes */ \               int64_t
+#     blkcnt_t    st_blocks;              /* [XSI] blocks allocated for file */ \         int64_t
+#     blksize_t    st_blksize;             /* [XSI] optimal blocksize for I/O */ \         int32_t
+#     __uint32_t    st_flags;               /* user defined flags for file */ \             uint32_t
+#     __uint32_t    st_gen;                 /* file generation number */ \                  uint32_t
+#     __int32_t    st_lspare;              /* RESERVED: DO NOT USE! */ \                   int32_t
+#     __int64_t    st_qspare[2];           /* RESERVED: DO NOT USE! */ \                   int64_t * 2
 # }
 # /*
 #  * [XSI] This structure is used as the second parameter to the fstat(),
 #  * lstat(), and stat() functions.
 #  */
 # #if __DARWIN_64_BIT_INO_T
 
@@ -184,92 +184,92 @@
 # They are the same in source code.
 MacOSStat64 = MacOSStat
 
 # https://elixir.bootlin.com/linux/latest/source/arch/mips/include/uapi/asm/stat.h#L19
 #
 # #if (_MIPS_SIM == _MIPS_SIM_ABI32) || (_MIPS_SIM == _MIPS_SIM_NABI32)
 # struct stat {
-# 	unsigned	st_dev;                                                             uint32_t
-# 	long		st_pad1[3];		/* Reserved for network id */                       int32_t
-# 	ino_t		st_ino;                                                             uint32_t (unsinged long)
-# 	mode_t		st_mode;                                                            uint32_t (unsinged int)
-# 	__u32		st_nlink;                                                           uint32_t
-# 	uid_t		st_uid;                                                             uint32_t (unsigned int)
-# 	gid_t		st_gid;                                                             uint32_t (unsigned int)
-# 	unsigned	st_rdev;                                                            uint32_t
-# 	long		st_pad2[2];                                                         uint32_t * 2
-# 	long		st_size;                                                            uint32_t
-# 	long		st_pad3;                                                            uint32_t
-# 	/*
-# 	 * Actually this should be timestruc_t st_atime, st_mtime and st_ctime
-# 	 * but we don't have it under Linux.
-# 	 */
-# 	long		st_atime;                                                           uint32_t
-# 	long		st_atime_nsec;                                                      uint32_t
-# 	long		st_mtime;                                                           uint32_t
-# 	long		st_mtime_nsec;                                                      uint32_t
-# 	long		st_ctime;                                                           uint32_t
-# 	long		st_ctime_nsec;                                                      uint32_t
-# 	long		st_blksize;                                                         uint32_t
-# 	long		st_blocks;                                                          uint32_t
-# 	long		st_pad4[14];                                                        uint32_t * 4
+#     unsigned    st_dev;                                                             uint32_t
+#     long        st_pad1[3];        /* Reserved for network id */                       int32_t
+#     ino_t        st_ino;                                                             uint32_t (unsinged long)
+#     mode_t        st_mode;                                                            uint32_t (unsinged int)
+#     __u32        st_nlink;                                                           uint32_t
+#     uid_t        st_uid;                                                             uint32_t (unsigned int)
+#     gid_t        st_gid;                                                             uint32_t (unsigned int)
+#     unsigned    st_rdev;                                                            uint32_t
+#     long        st_pad2[2];                                                         uint32_t * 2
+#     long        st_size;                                                            uint32_t
+#     long        st_pad3;                                                            uint32_t
+#     /*
+#      * Actually this should be timestruc_t st_atime, st_mtime and st_ctime
+#      * but we don't have it under Linux.
+#      */
+#     long        st_atime;                                                           uint32_t
+#     long        st_atime_nsec;                                                      uint32_t
+#     long        st_mtime;                                                           uint32_t
+#     long        st_mtime_nsec;                                                      uint32_t
+#     long        st_ctime;                                                           uint32_t
+#     long        st_ctime_nsec;                                                      uint32_t
+#     long        st_blksize;                                                         uint32_t
+#     long        st_blocks;                                                          uint32_t
+#     long        st_pad4[14];                                                        uint32_t * 4
 # };
 #
 # struct stat64 {
-# 	unsigned long	st_dev;                                                         uint32_t
-# 	unsigned long	st_pad0[3];	/* Reserved for st_dev expansion  */                uint32_t * 3
-# 	unsigned long long	st_ino;                                                     uint64_t
-# 	mode_t		st_mode;                                                            uint32_t
-# 	__u32		st_nlink;                                                           uint32_t
-# 	uid_t		st_uid;                                                             uint32_t
-# 	gid_t		st_gid;                                                             uint32_t
-# 	unsigned long	st_rdev;                                                        uint32_t
-# 	unsigned long	st_pad1[3];	/* Reserved for st_rdev expansion  */               uint32_t * 3
-# 	long long	st_size;                                                            uint64_t
-# 	/*
-# 	 * Actually this should be timestruc_t st_atime, st_mtime and st_ctime
-# 	 * but we don't have it under Linux.
-# 	 */
-# 	long		st_atime;                                                           int32_t
-# 	unsigned long	st_atime_nsec;	/* Reserved for st_atime expansion  */          uint32_t
-# 	long		st_mtime;                                                           int32_t
-# 	unsigned long	st_mtime_nsec;	/* Reserved for st_mtime expansion  */          uint32_t
-# 	long		st_ctime;                                                           int32_t
-# 	unsigned long	st_ctime_nsec;	/* Reserved for st_ctime expansion  */          uint32_t
-# 	unsigned long	st_blksize;                                                     uint32_t
-# 	unsigned long	st_pad2;                                                        uint32_t
-# 	long long	st_blocks;                                                          int64_t
+#     unsigned long    st_dev;                                                         uint32_t
+#     unsigned long    st_pad0[3];    /* Reserved for st_dev expansion  */                uint32_t * 3
+#     unsigned long long    st_ino;                                                     uint64_t
+#     mode_t        st_mode;                                                            uint32_t
+#     __u32        st_nlink;                                                           uint32_t
+#     uid_t        st_uid;                                                             uint32_t
+#     gid_t        st_gid;                                                             uint32_t
+#     unsigned long    st_rdev;                                                        uint32_t
+#     unsigned long    st_pad1[3];    /* Reserved for st_rdev expansion  */               uint32_t * 3
+#     long long    st_size;                                                            uint64_t
+#     /*
+#      * Actually this should be timestruc_t st_atime, st_mtime and st_ctime
+#      * but we don't have it under Linux.
+#      */
+#     long        st_atime;                                                           int32_t
+#     unsigned long    st_atime_nsec;    /* Reserved for st_atime expansion  */          uint32_t
+#     long        st_mtime;                                                           int32_t
+#     unsigned long    st_mtime_nsec;    /* Reserved for st_mtime expansion  */          uint32_t
+#     long        st_ctime;                                                           int32_t
+#     unsigned long    st_ctime_nsec;    /* Reserved for st_ctime expansion  */          uint32_t
+#     unsigned long    st_blksize;                                                     uint32_t
+#     unsigned long    st_pad2;                                                        uint32_t
+#     long long    st_blocks;                                                          int64_t
 # };
 # #endif /* _MIPS_SIM == _MIPS_SIM_ABI32 */
 # #if _MIPS_SIM == _MIPS_SIM_ABI64
 # /* The memory layout is the same as of struct stat64 of the 32-bit kernel.  */
 # struct stat {
-# 	unsigned int		st_dev;                                                     uint32_t
-# 	unsigned int		st_pad0[3]; /* Reserved for st_dev expansion */             uint32_t * 3
-# 	unsigned long		st_ino;                                                     uint64_t
-# 	mode_t			st_mode;                                                        uint32_t
-# 	__u32			st_nlink;                                                       uint32_t
-# 	uid_t			st_uid;                                                         uint32_t
-# 	gid_t			st_gid;                                                         uint32_t
-# 	unsigned int		st_rdev;                                                    uint32_t
-# 	unsigned int		st_pad1[3]; /* Reserved for st_rdev expansion */            uint32_t * 3
-# 	long			st_size;                                                        uint64_t
-# 	/*
-# 	 * Actually this should be timestruc_t st_atime, st_mtime and st_ctime
-# 	 * but we don't have it under Linux.
-# 	 */
-# 	unsigned int		st_atime;                                                   uint32_t
-# 	unsigned int		st_atime_nsec;                                              uint32_t
-# 	unsigned int		st_mtime;                                                   uint32_t
-# 	unsigned int		st_mtime_nsec;                                              uint32_t
-# 	unsigned int		st_ctime;                                                   uint32_t
-# 	unsigned int		st_ctime_nsec;                                              uint32_t
-# 	unsigned int		st_blksize;                                                 uint32_t
-# 	unsigned int		st_pad2;                                                    uint32_t
-# 	unsigned long		st_blocks;                                                  uint64_t
+#     unsigned int        st_dev;                                                     uint32_t
+#     unsigned int        st_pad0[3]; /* Reserved for st_dev expansion */             uint32_t * 3
+#     unsigned long        st_ino;                                                     uint64_t
+#     mode_t            st_mode;                                                        uint32_t
+#     __u32            st_nlink;                                                       uint32_t
+#     uid_t            st_uid;                                                         uint32_t
+#     gid_t            st_gid;                                                         uint32_t
+#     unsigned int        st_rdev;                                                    uint32_t
+#     unsigned int        st_pad1[3]; /* Reserved for st_rdev expansion */            uint32_t * 3
+#     long            st_size;                                                        uint64_t
+#     /*
+#      * Actually this should be timestruc_t st_atime, st_mtime and st_ctime
+#      * but we don't have it under Linux.
+#      */
+#     unsigned int        st_atime;                                                   uint32_t
+#     unsigned int        st_atime_nsec;                                              uint32_t
+#     unsigned int        st_mtime;                                                   uint32_t
+#     unsigned int        st_mtime_nsec;                                              uint32_t
+#     unsigned int        st_ctime;                                                   uint32_t
+#     unsigned int        st_ctime_nsec;                                              uint32_t
+#     unsigned int        st_blksize;                                                 uint32_t
+#     unsigned int        st_pad2;                                                    uint32_t
+#     unsigned long        st_blocks;                                                  uint64_t
 # };
 
 class LinuxMips32Stat(ctypes.Structure):
     _fields_ = [
         ("st_dev", ctypes.c_uint32),
         ("st_pad1", ctypes.c_int32 * 3),
         ("st_ino", ctypes.c_uint32),
@@ -395,75 +395,75 @@
 
     _pack_ = 4
 
 # https://elixir.bootlin.com/linux/latest/source/arch/x86/include/uapi/asm/stat.h#L10
 #
 # #ifdef __i386__
 # struct stat {
-# 	unsigned long  st_dev;                                                      uint32_t
-# 	unsigned long  st_ino;                                                      uint32_t
-# 	unsigned short st_mode;                                                     uint16_t
-# 	unsigned short st_nlink;                                                    uint16_t
-# 	unsigned short st_uid;                                                      uint16_t
-# 	unsigned short st_gid;                                                      uint16_t
-# 	unsigned long  st_rdev;                                                     uint32_t
-# 	unsigned long  st_size;                                                     uint32_t
-# 	unsigned long  st_blksize;                                                  uint32_t
-# 	unsigned long  st_blocks;                                                   uint32_t
-# 	unsigned long  st_atime;                                                    uint32_t
-# 	unsigned long  st_atime_nsec;                                               uint32_t
-# 	unsigned long  st_mtime;                                                    uint32_t
-# 	unsigned long  st_mtime_nsec;                                               uint32_t
-# 	unsigned long  st_ctime;                                                    uint32_t
-# 	unsigned long  st_ctime_nsec;                                               uint32_t
-# 	unsigned long  __unused4;                                                   uint32_t
-# 	unsigned long  __unused5;                                                   uint32_t
+#     unsigned long  st_dev;                                                      uint32_t
+#     unsigned long  st_ino;                                                      uint32_t
+#     unsigned short st_mode;                                                     uint16_t
+#     unsigned short st_nlink;                                                    uint16_t
+#     unsigned short st_uid;                                                      uint16_t
+#     unsigned short st_gid;                                                      uint16_t
+#     unsigned long  st_rdev;                                                     uint32_t
+#     unsigned long  st_size;                                                     uint32_t
+#     unsigned long  st_blksize;                                                  uint32_t
+#     unsigned long  st_blocks;                                                   uint32_t
+#     unsigned long  st_atime;                                                    uint32_t
+#     unsigned long  st_atime_nsec;                                               uint32_t
+#     unsigned long  st_mtime;                                                    uint32_t
+#     unsigned long  st_mtime_nsec;                                               uint32_t
+#     unsigned long  st_ctime;                                                    uint32_t
+#     unsigned long  st_ctime_nsec;                                               uint32_t
+#     unsigned long  __unused4;                                                   uint32_t
+#     unsigned long  __unused5;                                                   uint32_t
 # };
 # struct stat64 {
-# 	unsigned long long	st_dev;                                                 uint64_t
-# 	unsigned char	__pad0[4];                                                  uint8_t * 4
-# 	unsigned long	__st_ino;                                                   uint32_t
-# 	unsigned int	st_mode;                                                    uint32_t
-# 	unsigned int	st_nlink;                                                   uint32_t
-# 	unsigned long	st_uid;                                                     uint32_t
-# 	unsigned long	st_gid;                                                     uint32_t
-# 	unsigned long long	st_rdev;                                                uint64_t
-# 	unsigned char	__pad3[4];                                                  uint8_t * 4
-# 	long long	st_size;                                                        int64_t
-# 	unsigned long	st_blksize;                                                 uint32_t
-# 	/* Number 512-byte blocks allocated. */
-# 	unsigned long long	st_blocks;                                              uint64_t
-# 	unsigned long	st_atime;                                                   uint32_t
-# 	unsigned long	st_atime_nsec;                                              uint32_t
-# 	unsigned long	st_mtime;                                                   uint32_t
-# 	unsigned int	st_mtime_nsec;                                              uint32_t
-# 	unsigned long	st_ctime;                                                   uint32_t
-# 	unsigned long	st_ctime_nsec;                                              uint32_t
-# 	unsigned long long	st_ino;                                                 uint64_t
+#     unsigned long long    st_dev;                                                 uint64_t
+#     unsigned char    __pad0[4];                                                  uint8_t * 4
+#     unsigned long    __st_ino;                                                   uint32_t
+#     unsigned int    st_mode;                                                    uint32_t
+#     unsigned int    st_nlink;                                                   uint32_t
+#     unsigned long    st_uid;                                                     uint32_t
+#     unsigned long    st_gid;                                                     uint32_t
+#     unsigned long long    st_rdev;                                                uint64_t
+#     unsigned char    __pad3[4];                                                  uint8_t * 4
+#     long long    st_size;                                                        int64_t
+#     unsigned long    st_blksize;                                                 uint32_t
+#     /* Number 512-byte blocks allocated. */
+#     unsigned long long    st_blocks;                                              uint64_t
+#     unsigned long    st_atime;                                                   uint32_t
+#     unsigned long    st_atime_nsec;                                              uint32_t
+#     unsigned long    st_mtime;                                                   uint32_t
+#     unsigned int    st_mtime_nsec;                                              uint32_t
+#     unsigned long    st_ctime;                                                   uint32_t
+#     unsigned long    st_ctime_nsec;                                              uint32_t
+#     unsigned long long    st_ino;                                                 uint64_t
 # };
 # #else /* __i386__ */
 # struct stat {
-# 	__kernel_ulong_t	st_dev;                                                 uint64_t
-# 	__kernel_ulong_t	st_ino;                                                 uint64_t
-# 	__kernel_ulong_t	st_nlink;                                               uint64_t
-# 	unsigned int		st_mode;                                                uint32_t
-# 	unsigned int		st_uid;                                                 uint32_t
-# 	unsigned int		st_gid;                                                 uint32_t
-# 	unsigned int		__pad0;                                                 uint32_t
-# 	__kernel_ulong_t	st_rdev;                                                uint64_t
-# 	__kernel_long_t		st_size;                                                int64_t
-# 	__kernel_long_t		st_blksize;                                             int64_t
-# 	__kernel_long_t		st_blocks;	/* Number 512-byte blocks allocated. */     int64_t
-# 	__kernel_ulong_t	st_atime;                                               uint64_t
-# 	__kernel_ulong_t	st_atime_nsec;                                          uint64_t
-# 	__kernel_ulong_t	st_mtime;                                               uint64_t
-# 	__kernel_ulong_t	st_mtime_nsec;                                          uint64_t
-# 	__kernel_ulong_t	st_ctime;                                               uint64_t
-# 	__kernel_ulong_t	st_ctime_nsec;                                          uint64_t
-# 	__kernel_long_t		__unused[3];                                            int64_t
+#     __kernel_ulong_t    st_dev;                                                 uint64_t
+#     __kernel_ulong_t    st_ino;                                                 uint64_t
+#     __kernel_ulong_t    st_nlink;                                               uint64_t
+#     unsigned int        st_mode;                                                uint32_t
+#     unsigned int        st_uid;                                                 uint32_t
+#     unsigned int        st_gid;                                                 uint32_t
+#     unsigned int        __pad0;                                                 uint32_t
+#     __kernel_ulong_t    st_rdev;                                                uint64_t
+#     __kernel_long_t        st_size;                                                int64_t
+#     __kernel_long_t        st_blksize;                                             int64_t
+#     __kernel_long_t        st_blocks;    /* Number 512-byte blocks allocated. */     int64_t
+#     __kernel_ulong_t    st_atime;                                               uint64_t
+#     __kernel_ulong_t    st_atime_nsec;                                          uint64_t
+#     __kernel_ulong_t    st_mtime;                                               uint64_t
+#     __kernel_ulong_t    st_mtime_nsec;                                          uint64_t
+#     __kernel_ulong_t    st_ctime;                                               uint64_t
+#     __kernel_ulong_t    st_ctime_nsec;                                          uint64_t
+#     __kernel_long_t        __unused[3];                                            int64_t
 # };
 # #endif
 
 class LinuxX86Stat(ctypes.Structure):
     _fields_ = [
         ("st_dev", ctypes.c_uint32),
         ("st_ino", ctypes.c_uint32),
@@ -536,90 +536,90 @@
 
     _pack_ = 4
 
 # https://elixir.bootlin.com/linux/latest/source/arch/arm/include/uapi/asm/stat.h#L21
 #
 # struct stat {
 # #if defined(__ARMEB__)
-# 	unsigned short st_dev;                                                          uint16_t
-# 	unsigned short __pad1;                                                          uint16_t
+#     unsigned short st_dev;                                                          uint16_t
+#     unsigned short __pad1;                                                          uint16_t
 # #else
-# 	unsigned long  st_dev;                                                          uint32_t
+#     unsigned long  st_dev;                                                          uint32_t
 # #endif
-# 	unsigned long  st_ino;                                                          uint32_t
-# 	unsigned short st_mode;                                                         uint16_t
-# 	unsigned short st_nlink;                                                        uint16_t
-# 	unsigned short st_uid;                                                          uint16_t
-# 	unsigned short st_gid;                                                          uint16_t
+#     unsigned long  st_ino;                                                          uint32_t
+#     unsigned short st_mode;                                                         uint16_t
+#     unsigned short st_nlink;                                                        uint16_t
+#     unsigned short st_uid;                                                          uint16_t
+#     unsigned short st_gid;                                                          uint16_t
 # #if defined(__ARMEB__)
-# 	unsigned short st_rdev;                                                         uint16_t
-# 	unsigned short __pad2;                                                          uint16_t
+#     unsigned short st_rdev;                                                         uint16_t
+#     unsigned short __pad2;                                                          uint16_t
 # #else
-# 	unsigned long  st_rdev;                                                         uint32_t
+#     unsigned long  st_rdev;                                                         uint32_t
 # #endif
-# 	unsigned long  st_size;                                                         uint32_t
-# 	unsigned long  st_blksize;                                                      uint32_t
-# 	unsigned long  st_blocks;                                                       uint32_t
-# 	unsigned long  st_atime;                                                        uint32_t
-# 	unsigned long  st_atime_nsec;                                                   uint32_t
-# 	unsigned long  st_mtime;                                                        uint32_t
-# 	unsigned long  st_mtime_nsec;                                                   uint32_t
-# 	unsigned long  st_ctime;                                                        uint32_t
-# 	unsigned long  st_ctime_nsec;                                                   uint32_t
-# 	unsigned long  __unused4;                                                       uint32_t
-# 	unsigned long  __unused5;                                                       uint32_t
+#     unsigned long  st_size;                                                         uint32_t
+#     unsigned long  st_blksize;                                                      uint32_t
+#     unsigned long  st_blocks;                                                       uint32_t
+#     unsigned long  st_atime;                                                        uint32_t
+#     unsigned long  st_atime_nsec;                                                   uint32_t
+#     unsigned long  st_mtime;                                                        uint32_t
+#     unsigned long  st_mtime_nsec;                                                   uint32_t
+#     unsigned long  st_ctime;                                                        uint32_t
+#     unsigned long  st_ctime_nsec;                                                   uint32_t
+#     unsigned long  __unused4;                                                       uint32_t
+#     unsigned long  __unused5;                                                       uint32_t
 # };
 
 # struct stat64 {
-# 	unsigned long long	st_dev;                                                     uint64_t
-# 	unsigned char   __pad0[4];                                                      uint8_t * 4
-# #define STAT64_HAS_BROKEN_ST_INO	1
-# 	unsigned long	__st_ino;                                                       uint32_t
-# 	unsigned int	st_mode;                                                        uint32_t
-# 	unsigned int	st_nlink;                                                       uint32_t
-# 	unsigned long	st_uid;                                                         uint32_t
-# 	unsigned long	st_gid;                                                         uint32_t
-# 	unsigned long long	st_rdev;                                                    uint64_t
-# 	unsigned char   __pad3[4];                                                      uint8_t * 4
-# 	long long	st_size;                                                            int64_t
-# 	unsigned long	st_blksize;                                                     uint32_t
-# 	unsigned long long st_blocks;	/* Number 512-byte blocks allocated. */         uint64_t
-# 	unsigned long	st_atime;                                                       uint32_t
-# 	unsigned long	st_atime_nsec;                                                  uint32_t
-# 	unsigned long	st_mtime;                                                       uint32_t
-# 	unsigned long	st_mtime_nsec;                                                  uint32_t
-# 	unsigned long	st_ctime;                                                       uint32_t
-# 	unsigned long	st_ctime_nsec;                                                  uint32_t
-# 	unsigned long long	st_ino;                                                     uint64_t
+#     unsigned long long    st_dev;                                                     uint64_t
+#     unsigned char   __pad0[4];                                                      uint8_t * 4
+# #define STAT64_HAS_BROKEN_ST_INO    1
+#     unsigned long    __st_ino;                                                       uint32_t
+#     unsigned int    st_mode;                                                        uint32_t
+#     unsigned int    st_nlink;                                                       uint32_t
+#     unsigned long    st_uid;                                                         uint32_t
+#     unsigned long    st_gid;                                                         uint32_t
+#     unsigned long long    st_rdev;                                                    uint64_t
+#     unsigned char   __pad3[4];                                                      uint8_t * 4
+#     long long    st_size;                                                            int64_t
+#     unsigned long    st_blksize;                                                     uint32_t
+#     unsigned long long st_blocks;    /* Number 512-byte blocks allocated. */         uint64_t
+#     unsigned long    st_atime;                                                       uint32_t
+#     unsigned long    st_atime_nsec;                                                  uint32_t
+#     unsigned long    st_mtime;                                                       uint32_t
+#     unsigned long    st_mtime_nsec;                                                  uint32_t
+#     unsigned long    st_ctime;                                                       uint32_t
+#     unsigned long    st_ctime_nsec;                                                  uint32_t
+#     unsigned long long    st_ino;                                                     uint64_t
 # };
 
 # ARM64 stat is different!
 # https://elixir.bootlin.com/linux/v4.20.17/source/arch/arm64/include/asm/stat.h
 # The stat.h above includes https://elixir.bootlin.com/linux/v4.20.17/source/arch/arm64/include/uapi/asm/stat.h
 # struct stat {
-# 	unsigned long	st_dev;		/* Device.  */                                      uint64_t
-# 	unsigned long	st_ino;		/* File serial number.  */                          uint64_t
-# 	unsigned int	st_mode;	/* File mode.  */                                   uint32_t
-# 	unsigned int	st_nlink;	/* Link count.  */                                  uint32_t
-# 	unsigned int	st_uid;		/* User ID of the file's owner.  */                 uint32_t
-# 	unsigned int	st_gid;		/* Group ID of the file's group. */                 uint32_t
-# 	unsigned long	st_rdev;	/* Device number, if device.  */                    uint64_t
-# 	unsigned long	__pad1;                                                         uint64_t
-# 	long		st_size;	/* Size of file, in bytes.  */                          int64_t
-# 	int		st_blksize;	/* Optimal block size for I/O.  */                          int32_t
-# 	int		__pad2;                                                                 int32_t
-# 	long		st_blocks;	/* Number 512-byte blocks allocated. */                 int64_t
-# 	long		st_atime;	/* Time of last access.  */                             int64_t
-# 	unsigned long	st_atime_nsec;                                                  uint64_t
-# 	long		st_mtime;	/* Time of last modification.  */                       int64_t
-# 	unsigned long	st_mtime_nsec;                                                  uint64_t
-# 	long		st_ctime;	/* Time of last status change.  */                      int64_t
-# 	unsigned long	st_ctime_nsec;                                                  uint64_t
-# 	unsigned int	__unused4;                                                      uint32_t
-# 	unsigned int	__unused5;                                                      uint32_t
+#     unsigned long    st_dev;        /* Device.  */                                      uint64_t
+#     unsigned long    st_ino;        /* File serial number.  */                          uint64_t
+#     unsigned int    st_mode;    /* File mode.  */                                   uint32_t
+#     unsigned int    st_nlink;    /* Link count.  */                                  uint32_t
+#     unsigned int    st_uid;        /* User ID of the file's owner.  */                 uint32_t
+#     unsigned int    st_gid;        /* Group ID of the file's group. */                 uint32_t
+#     unsigned long    st_rdev;    /* Device number, if device.  */                    uint64_t
+#     unsigned long    __pad1;                                                         uint64_t
+#     long        st_size;    /* Size of file, in bytes.  */                          int64_t
+#     int        st_blksize;    /* Optimal block size for I/O.  */                          int32_t
+#     int        __pad2;                                                                 int32_t
+#     long        st_blocks;    /* Number 512-byte blocks allocated. */                 int64_t
+#     long        st_atime;    /* Time of last access.  */                             int64_t
+#     unsigned long    st_atime_nsec;                                                  uint64_t
+#     long        st_mtime;    /* Time of last modification.  */                       int64_t
+#     unsigned long    st_mtime_nsec;                                                  uint64_t
+#     long        st_ctime;    /* Time of last status change.  */                      int64_t
+#     unsigned long    st_ctime_nsec;                                                  uint64_t
+#     unsigned int    __unused4;                                                      uint32_t
+#     unsigned int    __unused5;                                                      uint32_t
 # };
 
 class LinuxARMStat(ctypes.Structure):
     _fields_ = [
         ("st_dev", ctypes.c_uint32),
         ("st_ino", ctypes.c_uint32),
         ("st_mode", ctypes.c_uint16),
@@ -767,34 +767,34 @@
         ("__unused5", ctypes.c_uint32)
     ]
 
     _pack_ = 8
 
 # Srouce: https://github.com/riscv-collab/riscv-gnu-toolchain/blob/master/linux-headers/include/asm-generic/stat.h
 # struct stat {
-# 	unsigned long	st_dev;		/* Device.  */
-# 	unsigned long	st_ino;		/* File serial number.  */
-# 	unsigned int	st_mode;	/* File mode.  */
-# 	unsigned int	st_nlink;	/* Link count.  */
-# 	unsigned int	st_uid;		/* User ID of the file's owner.  */
-# 	unsigned int	st_gid;		/* Group ID of the file's group. */
-# 	unsigned long	st_rdev;	/* Device number, if device.  */
-# 	unsigned long	__pad1;
-# 	long		st_size;	/* Size of file, in bytes.  */
-# 	int		st_blksize;	/* Optimal block size for I/O.  */
-# 	int		__pad2;
-# 	long		st_blocks;	/* Number 512-byte blocks allocated. */
-# 	long		st_atime;	/* Time of last access.  */
-# 	unsigned long	st_atime_nsec;
-# 	long		st_mtime;	/* Time of last modification.  */
-# 	unsigned long	st_mtime_nsec;
-# 	long		st_ctime;	/* Time of last status change.  */
-# 	unsigned long	st_ctime_nsec;
-# 	unsigned int	__unused4;
-# 	unsigned int	__unused5;
+#     unsigned long    st_dev;        /* Device.  */
+#     unsigned long    st_ino;        /* File serial number.  */
+#     unsigned int    st_mode;    /* File mode.  */
+#     unsigned int    st_nlink;    /* Link count.  */
+#     unsigned int    st_uid;        /* User ID of the file's owner.  */
+#     unsigned int    st_gid;        /* Group ID of the file's group. */
+#     unsigned long    st_rdev;    /* Device number, if device.  */
+#     unsigned long    __pad1;
+#     long        st_size;    /* Size of file, in bytes.  */
+#     int        st_blksize;    /* Optimal block size for I/O.  */
+#     int        __pad2;
+#     long        st_blocks;    /* Number 512-byte blocks allocated. */
+#     long        st_atime;    /* Time of last access.  */
+#     unsigned long    st_atime_nsec;
+#     long        st_mtime;    /* Time of last modification.  */
+#     unsigned long    st_mtime_nsec;
+#     long        st_ctime;    /* Time of last status change.  */
+#     unsigned long    st_ctime_nsec;
+#     unsigned int    __unused4;
+#     unsigned int    __unused5;
 # };
 
 class LinuxRISCVStat(ctypes.Structure):
     _fields_ = [
         ("st_dev", ctypes.c_uint64),
         ("st_ino", ctypes.c_uint64),
         ("st_mode", ctypes.c_uint32),
@@ -817,39 +817,39 @@
         ("__unused5", ctypes.c_uint32),
     ]
 
     _pack_ = 8
 
 # Srouce: https://elixir.bootlin.com/linux/latest/source/arch/powerpc/include/uapi/asm/stat.h#L30
 # struct stat {
-# 	unsigned long	st_dev;
-# 	ino_t		st_ino;
+#     unsigned long    st_dev;
+#     ino_t        st_ino;
 # #ifdef __powerpc64__
-# 	unsigned long	st_nlink;
-# 	mode_t		st_mode;
+#     unsigned long    st_nlink;
+#     mode_t        st_mode;
 # #else
-# 	mode_t		st_mode;
-# 	unsigned short	st_nlink;
+#     mode_t        st_mode;
+#     unsigned short    st_nlink;
 # #endif
-# 	uid_t		st_uid;
-# 	gid_t		st_gid;
-# 	unsigned long	st_rdev;
-# 	long		st_size;
-# 	unsigned long	st_blksize;
-# 	unsigned long	st_blocks;
-# 	unsigned long	st_atime;
-# 	unsigned long	st_atime_nsec;
-# 	unsigned long	st_mtime;
-# 	unsigned long	st_mtime_nsec;
-# 	unsigned long	st_ctime;
-# 	unsigned long	st_ctime_nsec;
-# 	unsigned long	__unused4;
-# 	unsigned long	__unused5;
+#     uid_t        st_uid;
+#     gid_t        st_gid;
+#     unsigned long    st_rdev;
+#     long        st_size;
+#     unsigned long    st_blksize;
+#     unsigned long    st_blocks;
+#     unsigned long    st_atime;
+#     unsigned long    st_atime_nsec;
+#     unsigned long    st_mtime;
+#     unsigned long    st_mtime_nsec;
+#     unsigned long    st_ctime;
+#     unsigned long    st_ctime_nsec;
+#     unsigned long    __unused4;
+#     unsigned long    __unused5;
 # #ifdef __powerpc64__
-# 	unsigned long	__unused6;
+#     unsigned long    __unused6;
 # #endif
 # };
 
 class LinuxPPCStat(ctypes.BigEndianStructure):
     _fields_ = [
         ("st_dev", ctypes.c_uint32),
         ("st_ino", ctypes.c_uint32),
@@ -871,33 +871,33 @@
         ("__unused5", ctypes.c_uint32)
     ]
 
     _pack_ = 8
 
 # Srouce: https://elixir.bootlin.com/linux/latest/source/arch/powerpc/include/uapi/asm/stat.h#L60
 # struct stat64 {
-# 	unsigned long long st_dev;		/* Device.  */
-# 	unsigned long long st_ino;		/* File serial number.  */
-# 	unsigned int	st_mode;	/* File mode.  */
-# 	unsigned int	st_nlink;	/* Link count.  */
-# 	unsigned int	st_uid;		/* User ID of the file's owner.  */
-# 	unsigned int	st_gid;		/* Group ID of the file's group. */
-# 	unsigned long long st_rdev;	/* Device number, if device.  */
-# 	unsigned short	__pad2;
-# 	long long	st_size;	/* Size of file, in bytes.  */
-# 	int		st_blksize;	/* Optimal block size for I/O.  */
-# 	long long	st_blocks;	/* Number 512-byte blocks allocated. */
-# 	int		st_atime;	/* Time of last access.  */
-# 	unsigned int	st_atime_nsec;
-# 	int		st_mtime;	/* Time of last modification.  */
-# 	unsigned int	st_mtime_nsec;
-# 	int		st_ctime;	/* Time of last status change.  */
-# 	unsigned int	st_ctime_nsec;
-# 	unsigned int	__unused4;
-# 	unsigned int	__unused5;
+#     unsigned long long st_dev;        /* Device.  */
+#     unsigned long long st_ino;        /* File serial number.  */
+#     unsigned int    st_mode;    /* File mode.  */
+#     unsigned int    st_nlink;    /* Link count.  */
+#     unsigned int    st_uid;        /* User ID of the file's owner.  */
+#     unsigned int    st_gid;        /* Group ID of the file's group. */
+#     unsigned long long st_rdev;    /* Device number, if device.  */
+#     unsigned short    __pad2;
+#     long long    st_size;    /* Size of file, in bytes.  */
+#     int        st_blksize;    /* Optimal block size for I/O.  */
+#     long long    st_blocks;    /* Number 512-byte blocks allocated. */
+#     int        st_atime;    /* Time of last access.  */
+#     unsigned int    st_atime_nsec;
+#     int        st_mtime;    /* Time of last modification.  */
+#     unsigned int    st_mtime_nsec;
+#     int        st_ctime;    /* Time of last status change.  */
+#     unsigned int    st_ctime_nsec;
+#     unsigned int    __unused4;
+#     unsigned int    __unused5;
 # };
 
 class LinuxPPCStat64(ctypes.BigEndianStructure):
     _fields_ = [
         ("st_dev", ctypes.c_uint64),
         ("st_ino", ctypes.c_uint64),
         ("st_mode", ctypes.c_uint32),
@@ -921,78 +921,78 @@
 
     _pack_ = 8
 
 # Source: openqnx lib/c/public/sys/stat.h
 #
 # struct stat {
 # #if _FILE_OFFSET_BITS - 0 == 64
-# 	ino_t			st_ino;			/* File serial number.					*/
-# 	off_t			st_size;
+#     ino_t            st_ino;            /* File serial number.                    */
+#     off_t            st_size;
 # #elif !defined(_FILE_OFFSET_BITS) || _FILE_OFFSET_BITS == 32
 # #if defined(__LITTLEENDIAN__)
-# 	ino_t			st_ino;			/* File serial number.					*/
-# 	ino_t			st_ino_hi;
-# 	off_t			st_size;
-# 	off_t			st_size_hi;
+#     ino_t            st_ino;            /* File serial number.                    */
+#     ino_t            st_ino_hi;
+#     off_t            st_size;
+#     off_t            st_size_hi;
 # #elif defined(__BIGENDIAN__)
-# 	ino_t			st_ino_hi;
-# 	ino_t			st_ino;			/* File serial number.					*/
-# 	off_t			st_size_hi;
-# 	off_t			st_size;
+#     ino_t            st_ino_hi;
+#     ino_t            st_ino;            /* File serial number.                    */
+#     off_t            st_size_hi;
+#     off_t            st_size;
 # #else
 #  #error endian not configured for system
 # #endif
 # #else
 #  #error _FILE_OFFSET_BITS value is unsupported
 # #endif
-# 	_CSTD dev_t		st_dev;			/* ID of device containing file.		*/
-# 	_CSTD dev_t		st_rdev;		/* Device ID, for inode that is device	*/
-# 	uid_t			st_uid;
-# 	gid_t			st_gid;
-# 	_CSTD time_t	st_mtime;		/* Time of last data modification		*/
-# 	_CSTD time_t	st_atime;		/* Time last accessed					*/
-# 	_CSTD time_t	st_ctime;		/* Time of last status change			*/
-# 	_CSTD mode_t	st_mode;		/* see below							*/
-# 	nlink_t			st_nlink;
-# 	blksize_t		st_blocksize;	/* Size of a block used by st_nblocks   */
-# 	_Int32t			st_nblocks;		/* Number of blocks st_blocksize blocks */
-# 	blksize_t		st_blksize;		/* Prefered I/O block size for object   */
+#     _CSTD dev_t        st_dev;            /* ID of device containing file.        */
+#     _CSTD dev_t        st_rdev;        /* Device ID, for inode that is device    */
+#     uid_t            st_uid;
+#     gid_t            st_gid;
+#     _CSTD time_t    st_mtime;        /* Time of last data modification        */
+#     _CSTD time_t    st_atime;        /* Time last accessed                    */
+#     _CSTD time_t    st_ctime;        /* Time of last status change            */
+#     _CSTD mode_t    st_mode;        /* see below                            */
+#     nlink_t            st_nlink;
+#     blksize_t        st_blocksize;    /* Size of a block used by st_nblocks   */
+#     _Int32t            st_nblocks;        /* Number of blocks st_blocksize blocks */
+#     blksize_t        st_blksize;        /* Prefered I/O block size for object   */
 # #if _FILE_OFFSET_BITS - 0 == 64
-# 	blkcnt_t		st_blocks;		/* Number of 512 byte blocks			*/
+#     blkcnt_t        st_blocks;        /* Number of 512 byte blocks            */
 # #elif !defined(_FILE_OFFSET_BITS) || _FILE_OFFSET_BITS == 32
 # #if defined(__LITTLEENDIAN__)
-# 	blkcnt_t		st_blocks;
-# 	blkcnt_t		st_blocks_hi;
+#     blkcnt_t        st_blocks;
+#     blkcnt_t        st_blocks_hi;
 # #elif defined(__BIGENDIAN__)
-# 	blkcnt_t		st_blocks_hi;
-# 	blkcnt_t		st_blocks;
+#     blkcnt_t        st_blocks_hi;
+#     blkcnt_t        st_blocks;
 # #else
 #  #error endian not configured for system
 # #endif
 # #else
 #  #error _FILE_OFFSET_BITS value is unsupported
 # #endif
 # };
 
 # struct stat64 {
-# 	ino64_t			st_ino;			/* File serial number.					*/
-# 	off64_t			st_size;
-# 	_CSTD dev_t		st_dev;			/* ID of device containing file.		*/
-# 	_CSTD dev_t		st_rdev;		/* Device ID, for inode that is device	*/
-# 	uid_t			st_uid;
-# 	gid_t			st_gid;
-# 	_CSTD time_t	st_mtime;		/* Time of last data modification		*/
-# 	_CSTD time_t	st_atime;		/* Time last accessed					*/
-# 	_CSTD time_t	st_ctime;		/* Time of last status change			*/
-# 	_CSTD mode_t	st_mode;		/* see below							*/
-# 	nlink_t			st_nlink;
-# 	blksize_t		st_blocksize;	/* Size of a block used by st_nblocks   */
-# 	_Int32t			st_nblocks;		/* Number of blocks st_blocksize blocks */
-# 	blksize_t		st_blksize;		/* Prefered I/O block size for object   */
-# 	blkcnt64_t		st_blocks;		/* Number of 512 byte blocks			*/
+#     ino64_t            st_ino;            /* File serial number.                    */
+#     off64_t            st_size;
+#     _CSTD dev_t        st_dev;            /* ID of device containing file.        */
+#     _CSTD dev_t        st_rdev;        /* Device ID, for inode that is device    */
+#     uid_t            st_uid;
+#     gid_t            st_gid;
+#     _CSTD time_t    st_mtime;        /* Time of last data modification        */
+#     _CSTD time_t    st_atime;        /* Time last accessed                    */
+#     _CSTD time_t    st_ctime;        /* Time of last status change            */
+#     _CSTD mode_t    st_mode;        /* see below                            */
+#     nlink_t            st_nlink;
+#     blksize_t        st_blocksize;    /* Size of a block used by st_nblocks   */
+#     _Int32t            st_nblocks;        /* Number of blocks st_blocksize blocks */
+#     blksize_t        st_blksize;        /* Prefered I/O block size for object   */
+#     blkcnt64_t        st_blocks;        /* Number of 512 byte blocks            */
 # };
 
 class QNXARMStat(ctypes.Structure):
     _fields_ = [
         ("st_ino", ctypes.c_uint32),
         ("st_ino_hi", ctypes.c_uint32), # this field must be zero
         ("st_size", ctypes.c_uint32),
@@ -1221,35 +1221,53 @@
         return None, ql.os.fd[dirfd].name
 
     if 0 < dirfd < NR_OPEN:
         return ql.os.fd[dirfd].fileno(), path
 
 
 def ql_syscall_chmod(ql: Qiling, filename: int, mode: int):
-    file_path = ql.os.utils.read_cstring(filename)
-    real_path = ql.os.path.transform_to_real_path(file_path)
+    vpath = ql.os.utils.read_cstring(filename)
+    hpath = ql.os.path.virtual_to_host_path(vpath)
+
+    if not ql.os.path.is_safe_host_path(hpath):
+        raise PermissionError(f'unsafe path: {hpath}')
+
     try:
-        os.chmod(real_path, mode)
-        regreturn = 0
-    except:
+        os.chmod(hpath, mode)
+    except OSError:
         regreturn = -1
-    ql.log.debug(f'chmod("{ql.os.utils.read_cstring(filename)}", {mode:d}) = 0')
+    else:
+        regreturn = 0
+
+    ql.log.debug(f'chmod("{vpath}", 0{mode:o}) = {regreturn}')
+
     return regreturn
 
+
 def ql_syscall_fchmod(ql: Qiling, fd: int, mode: int):
-    if fd not in range(NR_OPEN) or ql.os.fd[fd] is None:
-        return -EBADF
+    if fd not in range(NR_OPEN):
+        return -1
+
+    f = ql.os.fd[fd]
+
+    if f is None:
+        return -1
+
     try:
-        os.fchmod(ql.os.fd[fd].fileno(), mode)
-        regreturn = 0
-    except:
+        os.fchmod(f.fileno(), mode)
+    except OSError:
         regreturn = -1
-    ql.log.debug("fchmod(%d, %d) = %d" % (fd, mode, regreturn))
+    else:
+        regreturn = 0
+
+    ql.log.debug(f'fchmod({fd}, 0{mode:o}) = {regreturn}')
+
     return regreturn
 
+
 def ql_syscall_fstatat64(ql: Qiling, dirfd: int, path: int, buf_ptr: int, flags: int):
     dirfd, real_path = transform_path(ql, dirfd, path, flags)
 
     try:
         buf = pack_stat64_struct(ql, Stat(real_path, dirfd))
         ql.mem.write(buf_ptr, buf)
 
@@ -1472,40 +1490,53 @@
         regreturn = -1
 
     ql.log.debug("mknodat(%d, %s, 0%o, %d) = %d" % (dirfd, real_path, mode, dev, regreturn))
     return regreturn
 
 
 def ql_syscall_mkdir(ql: Qiling, pathname: int, mode: int):
-    file_path = ql.os.utils.read_cstring(pathname)
-    real_path = ql.os.path.transform_to_real_path(file_path)
-    regreturn = 0
+    vpath = ql.os.utils.read_cstring(pathname)
+    hpath = ql.os.path.virtual_to_host_path(vpath)
+
+    if not ql.os.path.is_safe_host_path(hpath):
+        raise PermissionError(f'unsafe path: {hpath}')
 
     try:
-        if not os.path.exists(real_path):
-            os.mkdir(real_path, mode)
-    except:
+        if not os.path.exists(hpath):
+            os.mkdir(hpath, mode)
+    except OSError:
         regreturn = -1
+    else:
+        regreturn = 0
+
+    ql.log.debug(f'mkdir("{vpath}", 0{mode:o}) = {regreturn}')
 
-    ql.log.debug("mkdir(%s, 0%o) = %d" % (real_path, mode, regreturn))
     return regreturn
 
+
 def ql_syscall_rmdir(ql: Qiling, pathname: int):
-    file_path = ql.os.utils.read_cstring(pathname)
-    real_path = ql.os.path.transform_to_real_path(file_path)
-    regreturn = 0
+    vpath = ql.os.utils.read_cstring(pathname)
+    hpath = ql.os.path.virtual_to_host_path(vpath)
+
+    if not ql.os.path.is_safe_host_path(hpath):
+        raise PermissionError(f'unsafe path: {hpath}')
 
     try:
-        if os.path.exists(real_path):
-            os.rmdir(real_path)
-    except:
+        if os.path.exists(hpath):
+            os.rmdir(hpath)
+    except OSError:
         regreturn = -1
+    else:
+        regreturn = 0
+
+    ql.log.debug(f'rmdir("{vpath}") = {regreturn}')
 
     return regreturn
 
+
 def ql_syscall_fstatfs(ql: Qiling, fd: int, buf: int):
     data = b"0" * (12 * 8)  # for now, just return 0s
     regreturn = 0
 
     try:
         ql.mem.write(buf, data)
     except:
```

### Comparing `qiling-1.4.5/qiling/os/posix/syscall/sysinfo.py` & `qiling-1.4.6/qiling/os/posix/syscall/sysinfo.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/os/posix/syscall/time.py` & `qiling-1.4.6/qiling/os/posix/syscall/time.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/os/posix/syscall/types.py` & `qiling-1.4.6/qiling/os/posix/syscall/types.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/os/posix/syscall/uio.py` & `qiling-1.4.6/qiling/os/posix/syscall/uio.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/os/posix/syscall/unistd.py` & `qiling-1.4.6/qiling/os/posix/syscall/unistd.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 #!/usr/bin/env python3
 #
 # Cross Platform and Multi Architecture Advanced Binary Emulation Framework
 #
 
+from __future__ import annotations
+
 import os
-import stat
 import itertools
 import pathlib
 
-from typing import Iterator
-from multiprocessing import Process
+from typing import TYPE_CHECKING, Iterator, Optional
 
 from qiling import Qiling
 from qiling.const import QL_ARCH, QL_OS
 from qiling.os.posix.filestruct import ql_pipe
 from qiling.os.posix.const import *
-from qiling.os.posix.stat import Stat
 from qiling.core_hooks import QlCoreHooks
 
+if TYPE_CHECKING:
+    from qiling.os.posix.posix import QlOsPosix
+
+
 def ql_syscall_exit(ql: Qiling, code: int):
-    if ql.os.child_processes == True:
+    if ql.os.child_processes:
         os._exit(0)
 
     if ql.multithread:
         def _sched_cb_exit(cur_thread):
             ql.log.debug(f"[Thread {cur_thread.get_id()}] Terminated")
             ql.os.thread_management.stop_thread(cur_thread)
             cur_thread.exit_code = code
@@ -33,15 +36,15 @@
         td.sched_cb = _sched_cb_exit
     else:
         ql.os.exit_code = code
         ql.os.stop()
 
 
 def ql_syscall_exit_group(ql: Qiling, code: int):
-    if ql.os.child_processes == True:
+    if ql.os.child_processes:
         os._exit(0)
 
     if ql.multithread:
         def _sched_cb_exit(cur_thread):
             ql.log.debug(f"[Thread {cur_thread.get_id()}] Terminated")
             ql.os.thread_management.stop_thread(cur_thread)
             cur_thread.exit_code = code
@@ -131,107 +134,171 @@
 def ql_syscall_setgroups(ql: Qiling, gidsetsize: int, grouplist: int):
     return 0
 
 
 def ql_syscall_setresuid(ql: Qiling):
     return 0
 
+
 def ql_syscall_setresgid(ql: Qiling):
     return 0
 
+
 def ql_syscall_capget(ql: Qiling, hdrp: int, datap: int):
     return 0
 
+
 def ql_syscall_capset(ql: Qiling, hdrp: int, datap: int):
     return 0
 
+
 def ql_syscall_kill(ql: Qiling, pid: int, sig: int):
     return 0
 
 
+def get_opened_fd(os: QlOsPosix, fd: int):
+    if fd not in range(NR_OPEN):
+        # TODO: set errno to EBADF
+        return None
+
+    f = os.fd[fd]
+
+    if f is None:
+        # TODO: set errno to EBADF
+        return None
+
+    return f
+
+
 def ql_syscall_fsync(ql: Qiling, fd: int):
-    try:
-        os.fsync(ql.os.fd[fd].fileno())
-        regreturn = 0
-    except:
+    f = get_opened_fd(ql.os, fd)
+
+    if f is None:
         regreturn = -1
-    ql.log.debug("fsync(%d) = %d" % (fd, regreturn))
+
+    else:
+        try:
+            os.fsync(f.fileno())
+        except OSError:
+            regreturn = -1
+        else:
+            regreturn = 0
+
+    ql.log.debug(f'fsync({fd:d}) = {regreturn}')
+
     return regreturn
 
 
 def ql_syscall_fdatasync(ql: Qiling, fd: int):
     try:
         os.fdatasync(ql.os.fd[fd].fileno())
-        regreturn = 0
-    except:
+    except OSError:
         regreturn = -1
-    ql.log.debug("fdatasync(%d) = %d" % (fd, regreturn))
+    else:
+        regreturn = 0
+
+    ql.log.debug(f'fdatasync({fd:d}) = {regreturn}')
+
     return regreturn
 
 
-def ql_syscall_faccessat(ql: Qiling, dfd: int, filename: int, mode: int):
-    access_path = ql.os.utils.read_cstring(filename)
-    real_path = ql.os.path.transform_to_real_path(access_path)
+def virtual_abspath_at(ql: Qiling, vpath: str, dirfd: int) -> Optional[str]:
+    if ql.os.path.is_virtual_abspath(vpath):
+        return vpath
 
-    if not os.path.exists(real_path):
-        regreturn = -1
-    else:
-        regreturn = 0
+    # <WORKAROUND>
+    def __as_signed(value: int, nbits: int) -> int:
+        msb = (1 << (nbits - 1))
+
+        return -(((value & msb) << 1) - value)
+
+    # syscall params are read as unsigned int by default. until we fix that
+    # broadly, this is a workaround to turn fd into a signed value
+    dirfd = __as_signed(dirfd, ql.arch.bits)
+    # </WORKAROUND>
+
+    if dirfd == AT_FDCWD:
+        basedir = ql.os.path.cwd
 
-    if regreturn == -1:
-        ql.log.debug(f'File not found or skipped: {access_path}')
     else:
-        ql.log.debug(f'File found: {access_path}')
+        f = get_opened_fd(ql.os, dirfd)
 
-    return regreturn
+        if f is None or not hasattr(f, 'name'):
+            # EBADF
+            return None
 
+        hpath = f.name
 
-def ql_syscall_lseek(ql: Qiling, fd: int, offset: int, origin: int):
-    if fd not in range(NR_OPEN):
-        return -EBADF
+        if not os.path.isdir(hpath):
+            # ENOTDIR
+            return None
 
-    f = ql.os.fd[fd]
+        basedir = ql.os.path.host_to_virtual_path(hpath)
 
-    if f is None:
-        return -EBADF
+    return str(ql.os.path.PureVirtualPath(basedir, vpath))
 
-    offset = ql.unpacks(ql.pack(offset))
 
-    try:
-        regreturn = f.seek(offset, origin)
-    except OSError:
+def ql_syscall_faccessat(ql: Qiling, dirfd: int, filename: int, mode: int):
+    vpath = ql.os.utils.read_cstring(filename)
+    vpath_at = virtual_abspath_at(ql, vpath, dirfd)
+
+    if vpath_at is None:
         regreturn = -1
 
-    # ql.log.debug("lseek(fd = %d, ofset = 0x%x, origin = 0x%x) = %d" % (fd, offset, origin, regreturn))
+    else:
+        hpath = ql.os.path.virtual_to_host_path(vpath_at)
+
+        if not ql.os.path.is_safe_host_path(hpath):
+            raise PermissionError(f'unsafe path: {hpath}')
+
+        regreturn = 0 if os.path.exists(hpath) else -1
+
+    ql.log.debug(f'faccessat({dirfd:d}, "{vpath}", {mode:d}) = {regreturn}')
 
     return regreturn
 
 
-def ql_syscall__llseek(ql: Qiling, fd: int, offset_high: int, offset_low: int, result: int, whence: int):
-    if fd not in range(NR_OPEN):
-        return -EBADF
+def ql_syscall_lseek(ql: Qiling, fd: int, offset: int, origin: int):
+    offset = ql.unpacks(ql.pack(offset))
 
-    f = ql.os.fd[fd]
+    f = get_opened_fd(ql.os, fd)
 
     if f is None:
-        return -EBADF
+        regreturn = -1
+
+    else:
+        try:
+            regreturn = f.seek(offset, origin)
+        except OSError:
+            regreturn = -1
 
+    ql.log.debug(f'lseek({fd:d}, {offset:#x}, {origin}) = {regreturn}')
+
+    return regreturn
+
+
+def ql_syscall__llseek(ql: Qiling, fd: int, offset_high: int, offset_low: int, result: int, whence: int):
     # treat offset as a signed value
     offset = ql.unpack64s(ql.pack64((offset_high << 32) | offset_low))
-    origin = whence
 
-    try:
-        ret = f.seek(offset, origin)
-    except OSError:
+    f = get_opened_fd(ql.os, fd)
+
+    if f is None:
         regreturn = -1
+
     else:
-        ql.mem.write_ptr(result, ret, 8)
-        regreturn = 0
+        try:
+            ret = f.seek(offset, whence)
+        except OSError:
+            regreturn = -1
+        else:
+            ql.mem.write_ptr(result, ret, 8)
+            regreturn = 0
 
-    # ql.log.debug("_llseek(%d, 0x%x, 0x%x, 0x%x) = %d" % (fd, offset_high, offset_low, origin, regreturn))
+    ql.log.debug(f'_llseek({fd:d}, {offset_high:#x}, {offset_low:#x}, {result:#x}, {whence}) = {regreturn}')
 
     return regreturn
 
 
 def ql_syscall_brk(ql: Qiling, inp: int):
     if inp:
         cur_brk_addr = ql.loader.brk_address
@@ -247,104 +314,94 @@
 
         ql.loader.brk_address = new_brk_addr
 
     return ql.loader.brk_address
 
 
 def ql_syscall_access(ql: Qiling, path: int, mode: int):
-    file_path = ql.os.utils.read_cstring(path)
-    real_path = ql.os.path.transform_to_real_path(file_path)
-    relative_path = ql.os.path.transform_to_relative_path(file_path)
+    vpath = ql.os.utils.read_cstring(path)
+    hpath = ql.os.path.virtual_to_host_path(vpath)
 
-    regreturn = 0 if os.path.exists(real_path) else -1
+    if not ql.os.path.is_safe_host_path(hpath):
+        raise PermissionError(f'unsafe path: {hpath}')
 
-    # ql.log.debug("access(%s, 0x%x) = %d " % (relative_path, access_mode, regreturn))
+    regreturn = 0 if os.path.exists(hpath) else -1
 
-    if regreturn == 0:
-        ql.log.debug(f'File found: {relative_path}')
-    else:
-        ql.log.debug(f'No such file or directory: {relative_path}')
+    ql.log.debug(f'access("{vpath}", 0{mode:o}) = {regreturn}')
 
     return regreturn
 
 
 def ql_syscall_close(ql: Qiling, fd: int):
-    if fd not in range(NR_OPEN):
-        return -1
-
-    f = ql.os.fd[fd]
+    f = get_opened_fd(ql.os, fd)
 
     if f is None:
-        return -1
+        regreturn = -1
 
-    f.close()
-    ql.os.fd[fd] = None
+    else:
+        f.close()
+        ql.os.fd[fd] = None
+        regreturn = 0
 
-    return 0
+    ql.log.debug(f'close({fd:d}) = {regreturn}')
 
+    return regreturn
 
-def ql_syscall_pread64(ql: Qiling, fd: int, buf: int, length: int, offt: int):
-    if fd not in range(NR_OPEN):
-        return -1
 
-    f = ql.os.fd[fd]
+def ql_syscall_pread64(ql: Qiling, fd: int, buf: int, length: int, offt: int):
+    f = get_opened_fd(ql.os, fd)
 
     if f is None:
-        return -1
+        regreturn = -1
 
-    # https://chromium.googlesource.com/linux-syscall-support/+/2c73abf02fd8af961e38024882b9ce0df6b4d19b
-    # https://chromiumcodereview.appspot.com/10910222
-    if ql.arch.type == QL_ARCH.MIPS:
-        offt = ql.mem.read_ptr(ql.arch.regs.arch_sp + 0x10, 8)
+    else:
+        # https://chromium.googlesource.com/linux-syscall-support/+/2c73abf02fd8af961e38024882b9ce0df6b4d19b
+        # https://chromiumcodereview.appspot.com/10910222
+        if ql.arch.type == QL_ARCH.MIPS:
+            offt = ql.mem.read_ptr(ql.arch.regs.arch_sp + 0x10, 8)
 
-    try:
-        pos = f.tell()
-        f.seek(offt)
+        try:
+            pos = f.tell()
+            f.seek(offt)
 
-        data = f.read(length)
-        f.seek(pos)
+            data = f.read(length)
+            f.seek(pos)
+        except OSError:
+            regreturn = -1
+        else:
+            ql.mem.write(buf, data)
 
-        ql.mem.write(buf, data)
-    except:
-        regreturn = -1
-    else:
-        regreturn = len(data)
+            regreturn = len(data)
 
     return regreturn
 
 
 def ql_syscall_read(ql: Qiling, fd, buf: int, length: int):
-    if fd not in range(NR_OPEN):
-        return -EBADF
-
-    f = ql.os.fd[fd]
+    f = get_opened_fd(ql.os, fd)
 
     if f is None:
-        return -EBADF
+        return -1
 
     try:
         data = f.read(length)
         ql.mem.write(buf, data)
     except:
         regreturn = -EBADF
     else:
         ql.log.debug(f'read() CONTENT: {data!r}')
         regreturn = len(data)
 
     return regreturn
 
 
 def ql_syscall_write(ql: Qiling, fd: int, buf: int, count: int):
-    if fd not in range(NR_OPEN):
-        return -EBADF
-
-    f = ql.os.fd[fd]
+    f = get_opened_fd(ql.os, fd)
 
     if f is None:
-        return -EBADF
+        return -1
 
     try:
         data = ql.mem.read(buf, count)
     except:
         regreturn = -1
     else:
         ql.log.debug(f'write() CONTENT: {bytes(data)}')
@@ -353,112 +410,119 @@
             f.write(data)
 
             regreturn = count
         else:
             ql.log.warning(f'write failed since fd {fd:d} does not have a write method')
             regreturn = -1
 
-
     return regreturn
 
 
-def ql_syscall_readlink(ql: Qiling, path_name: int, path_buff: int, path_buffsize: int):
-    pathname = ql.os.utils.read_cstring(path_name)
-    # pathname = str(pathname, 'utf-8', errors="ignore")
-    host_path = ql.os.path.virtual_to_host_path(pathname)
-    virt_path = ql.os.path.virtual_abspath(pathname)
-
-    # cover procfs psaudo files first
-    # TODO: /proc/self/root, /proc/self/cwd
-    if virt_path == r'/proc/self/exe':
-        p = ql.os.path.host_to_virtual_path(ql.path)
-        p = p.encode('utf-8')
+def __do_readlink(ql: Qiling, absvpath: str, outbuf: int) -> int:
+    target = None
 
-        ql.mem.write(path_buff, p + b'\x00')
-        regreturn = len(p)
+    # cover a few procfs pseudo files first
+    if absvpath == r'/proc/self/exe':
+        # note this would raise an exception if the binary is not under rootfs
+        target = ql.os.path.host_to_virtual_path(ql.path)
 
-    elif os.path.exists(host_path):
-        regreturn = 0
+    elif absvpath == r'/proc/self/cwd':
+        target = ql.os.path.cwd
+
+    elif absvpath == r'/proc/self/root':
+        target = ql.os.path.root
 
     else:
-        regreturn = -1
+        hpath = ql.os.path.virtual_to_host_path(absvpath)
 
-    ql.log.debug('readlink("%s", 0x%x, 0x%x) = %d' % (virt_path, path_buff, path_buffsize, regreturn))
+        if not ql.os.path.is_safe_host_path(hpath):
+            raise PermissionError(f'unsafe path: {hpath}')
 
-    return regreturn
+        # FIXME: we do not really know how to emulated links, so we do not read them
+        if os.path.exists(hpath):
+            target = ''
 
+    if target is None:
+        return -1
 
-def ql_syscall_getcwd(ql: Qiling, path_buff: int, path_buffsize: int):
-    localpath = ql.os.path.transform_to_relative_path('./')
-    localpath = bytes(localpath, 'utf-8') + b'\x00'
+    cstr = target.encode('utf-8')
+
+    if cstr:
+        ql.mem.write(outbuf, cstr + b'\x00')
+
+    return len(cstr)
 
-    ql.mem.write(path_buff, localpath)
-    regreturn = len(localpath)
 
-    pathname = ql.os.utils.read_cstring(path_buff)
-    # pathname = str(pathname, 'utf-8', errors="ignore")
+def ql_syscall_readlink(ql: Qiling, pathname: int, buf: int, bufsize: int):
+    vpath = ql.os.utils.read_cstring(pathname)
+    absvpath = ql.os.path.virtual_abspath(vpath)
 
-    ql.log.debug("getcwd(%s, 0x%x) = %d" % (pathname, path_buffsize, regreturn))
+    regreturn = __do_readlink(ql, absvpath, buf)
+
+    ql.log.debug(f'readlink("{vpath}", {buf:#x}, {bufsize:#x}) = {regreturn}')
 
     return regreturn
 
 
-def ql_syscall_chdir(ql: Qiling, path_name: int):
-    pathname = ql.os.utils.read_cstring(path_name)
-    host_path = ql.os.path.virtual_to_host_path(pathname)
-    virt_path = ql.os.path.virtual_abspath(pathname)
+def ql_syscall_readlinkat(ql: Qiling, dirfd: int, pathname: int, buf: int, bufsize: int):
+    vpath = ql.os.utils.read_cstring(pathname)
+    absvpath = virtual_abspath_at(ql, vpath, dirfd)
 
-    if os.path.exists(host_path) and os.path.isdir(host_path):
-        ql.os.path.cwd = virt_path
+    regreturn = -1 if absvpath is None else __do_readlink(ql, absvpath, buf)
 
-        regreturn = 0
-        ql.log.debug("chdir(%s) = %d"% (virt_path, regreturn))
-    else:
-        regreturn = -1
-        ql.log.warning("chdir(%s) = %d : not found" % (virt_path, regreturn))
+    ql.log.debug(f'readlinkat({dirfd:d}, "{vpath}", {buf:#x}, {bufsize:#x}) = {regreturn}')
 
     return regreturn
 
 
-def ql_syscall_readlinkat(ql: Qiling, dfd: int, path: int, buf: int, bufsize: int):
-    pathname = ql.os.utils.read_cstring(path)
-    # pathname = str(pathname, 'utf-8', errors="ignore")
-    host_path = ql.os.path.virtual_to_host_path(pathname)
-    virt_path = ql.os.path.virtual_abspath(pathname)
+def ql_syscall_getcwd(ql: Qiling, path_buff: int, path_buffsize: int):
+    cwd = ql.os.path.cwd
 
-    # cover procfs psaudo files first
-    # TODO: /proc/self/root, /proc/self/cwd
-    if virt_path == r'/proc/self/exe':
-        p = ql.os.path.host_to_virtual_path(ql.path)
-        p = p.encode('utf-8')
+    cwd_bytes = cwd.encode('utf-8') + b'\x00'
+    ql.mem.write(path_buff, cwd_bytes)
+    regreturn = len(cwd_bytes)
 
-        ql.mem.write(buf, p + b'\x00')
-        regreturn = len(p)
+    ql.log.debug(f'getcwd("{cwd}", {path_buffsize}) = {regreturn}')
+
+    return regreturn
 
-    elif os.path.exists(host_path):
-        regreturn = 0
 
+def ql_syscall_chdir(ql: Qiling, path_name: int):
+    vpath = ql.os.utils.read_cstring(path_name)
+    hpath = ql.os.path.virtual_to_host_path(vpath)
+
+    if not ql.os.path.is_safe_host_path(hpath):
+        raise PermissionError(f'unsafe path: {hpath}')
+
+    absvpath = ql.os.path.virtual_abspath(vpath)
+
+    if os.path.isdir(hpath):
+        ql.os.path.cwd = absvpath
+
+        regreturn = 0
     else:
         regreturn = -1
 
-    ql.log.debug('readlinkat(%d, "%s", 0x%x, 0x%x) = %d' % (dfd, virt_path, buf, bufsize, regreturn))
+    ql.log.debug(f'chdir("{absvpath}") = {regreturn}')
 
     return regreturn
 
 
 def ql_syscall_getpid(ql: Qiling):
     return 0x512
 
 
 def ql_syscall_getppid(ql: Qiling):
     return 0x1024
 
 
 def ql_syscall_vfork(ql: Qiling):
     if ql.host.os == QL_OS.WINDOWS:
+        from multiprocessing import Process
+
         try:
             pid = Process()
             pid = 0
         except:
             pid = -1
     else:
         pid = os.fork()
@@ -475,49 +539,61 @@
 
     return regreturn
 
 
 def ql_syscall_fork(ql: Qiling):
     return ql_syscall_vfork(ql)
 
+
 def ql_syscall_setsid(ql: Qiling):
     return os.getpid()
 
 
 def ql_syscall_execve(ql: Qiling, pathname: int, argv: int, envp: int):
-    file_path = ql.os.utils.read_cstring(pathname)
-    real_path = ql.os.path.transform_to_real_path(file_path)
+    vpath = ql.os.utils.read_cstring(pathname)
+    hpath = ql.os.path.virtual_to_host_path(vpath)
 
-    def __read_str_array(addr: int) -> Iterator[str]:
+    # is it safe to run?
+    if not ql.os.path.is_safe_host_path(hpath):
+        return -1   # EACCES
+
+    # is it a file? does it exist?
+    if not os.path.isfile(hpath):
+        return -1   # EACCES
+
+    def __read_ptr_array(addr: int) -> Iterator[int]:
         if addr:
             while True:
                 elem = ql.mem.read_ptr(addr)
 
                 if elem == 0:
                     break
 
-                yield ql.os.utils.read_cstring(elem)
+                yield elem
                 addr += ql.arch.pointersize
 
-    args = [s for s in __read_str_array(argv)]
+    def __read_str_array(addr: int) -> Iterator[str]:
+        yield from (ql.os.utils.read_cstring(ptr) for ptr in __read_ptr_array(addr))
+
+    args = list(__read_str_array(argv))
 
     env = {}
     for s in __read_str_array(envp):
         k, _, v = s.partition('=')
         env[k] = v
 
-    ql.emu_stop()
+    ql.stop()
+    ql.clear_ql_hooks()
+    ql.mem.unmap_all()
 
-    ql.log.debug(f'execve({file_path}, [{", ".join(args)}], [{", ".join(f"{k}={v}" for k, v in env.items())}])')
+    ql.log.debug(f'execve("{vpath}", [{", ".join(args)}], [{", ".join(f"{k}={v}" for k, v in env.items())}])')
 
     ql.loader.argv = args
     ql.loader.env = env
-    ql._argv = [real_path] + args
-    ql.mem.map_info = []
-    ql.clear_ql_hooks()
+    ql._argv = [hpath] + args
 
     # Clean debugger to prevent port conflicts
     # ql.debugger = None
 
     if ql.code:
         return
 
@@ -530,64 +606,94 @@
 
     if hasattr(ql.arch, 'msr'):
         ql.arch.msr.uc = uc
 
     QlCoreHooks.__init__(ql, uc)
 
     ql.os.load()
+
+    # close all open fd marked with 'close_on_exec'
+    for i in range(NR_OPEN):
+        f = ql.os.fd[i]
+
+        if f and getattr(f, 'close_on_exec', False) and not f.closed:
+            f.close()
+            ql.os.fd[i] = None
+
     ql.loader.run()
     ql.run()
 
 
 def ql_syscall_dup(ql: Qiling, oldfd: int):
-    if oldfd not in range(NR_OPEN):
-        return -EBADF
-
-    f = ql.os.fd[oldfd]
+    f = get_opened_fd(ql.os, oldfd)
 
     if f is None:
-        return -EBADF
+        return -1
 
-    idx = next((i for i in range(NR_OPEN) if ql.os.fd[i] is None), -1)
+    newfd = next((i for i in range(NR_OPEN) if ql.os.fd[i] is None), -1)
 
-    if idx == -1:
+    if newfd == -1:
         return -EMFILE
 
-    ql.os.fd[idx] = f.dup()
+    ql.os.fd[newfd] = f.dup()
 
-    return idx
+    ql.log.debug(f'dup({oldfd:d}) = {newfd:d}')
 
+    return newfd
 
-def ql_syscall_dup2(ql: Qiling, fd: int, newfd: int):
-    if fd not in range(NR_OPEN) or newfd not in range(NR_OPEN):
-        return -EBADF
 
-    f = ql.os.fd[fd]
+def ql_syscall_dup2(ql: Qiling, oldfd: int, newfd: int):
+    f = get_opened_fd(ql.os, oldfd)
 
     if f is None:
-        return -EBADF
+        return -1
+
+    if newfd not in range(NR_OPEN):
+        return -1
+
+    newslot = ql.os.fd[newfd]
+
+    if newslot is not None:
+        newslot.close()
 
     ql.os.fd[newfd] = f.dup()
 
+    ql.log.debug(f'dup2({oldfd:d}, {newfd:d}) = {newfd:d}')
+
     return newfd
 
 
-def ql_syscall_dup3(ql: Qiling, fd: int, newfd: int, flags: int):
-    if fd not in range(NR_OPEN) or newfd not in range(NR_OPEN):
-        return -1
+def ql_syscall_dup3(ql: Qiling, oldfd: int, newfd: int, flags: int):
+    O_CLOEXEC = 0o2000000
 
-    f = ql.os.fd[fd]
+    f = get_opened_fd(ql.os, oldfd)
 
     if f is None:
         return -1
 
-    ql.os.fd[newfd] = f.dup()
+    if newfd not in range(NR_OPEN):
+        return -1
+
+    newslot = ql.os.fd[newfd]
+
+    if newslot is not None:
+        newslot.close()
+
+    newf = f.dup()
+
+    if flags & O_CLOEXEC:
+        newf.close_on_exec = True
+
+    ql.os.fd[newfd] = newf
+
+    ql.log.debug(f'dup3({oldfd:d}, {newfd:d}, 0{flags:o}) = {newfd:d}')
 
     return newfd
 
+
 def ql_syscall_set_tid_address(ql: Qiling, tidptr: int):
     if ql.os.thread_management:
         regreturn = ql.os.thread_management.cur_thread.id
     else:
         regreturn = os.getpid()
 
     return regreturn
@@ -617,110 +723,115 @@
     return regreturn
 
 
 def ql_syscall_nice(ql: Qiling, inc: int):
     return 0
 
 
-def ql_syscall_truncate(ql: Qiling, path: int, length: int):
-    file_path = ql.os.utils.read_cstring(path)
-    real_path = ql.os.path.transform_to_real_path(file_path)
-    st_size = Stat(real_path).st_size
+def __do_truncate(ql: Qiling, hpath: str, length: int) -> int:
+    if not ql.os.path.is_safe_host_path(hpath):
+        raise PermissionError(f'unsafe path: {hpath}')
 
     try:
-        if st_size >= length:
-            os.truncate(real_path, length)
+        st_size = os.path.getsize(hpath)
 
-        else:
+        if st_size > length:
+            os.truncate(hpath, length)
+
+        elif st_size < length:
             padding = length - st_size
 
-            with open(real_path, 'a+b') as ofile:
+            with open(hpath, 'a+b') as ofile:
                 ofile.write(b'\x00' * padding)
-    except:
-        regreturn = -1
+    except OSError:
+        return -1
     else:
-        regreturn = 0
+        return 0
+
+
+def ql_syscall_truncate(ql: Qiling, path: int, length: int):
+    vpath = ql.os.utils.read_cstring(path)
+    hpath = ql.os.path.virtual_to_host_path(vpath)
+
+    regreturn = __do_truncate(ql, hpath, length)
 
-    ql.log.debug('truncate(%s, 0x%x) = %d' % (file_path, length, regreturn))
+    ql.log.debug(f'truncate("{vpath}", {length:#x}) = {regreturn}')
 
     return regreturn
 
 
 def ql_syscall_ftruncate(ql: Qiling, fd: int, length: int):
-    real_path = ql.os.fd[fd].name
-    st_size = Stat(real_path).st_size
+    f = get_opened_fd(ql.os, fd)
 
-    try:
-        if st_size >= length:
-            os.truncate(real_path, length)
+    regreturn = -1 if f is None else __do_truncate(ql, f.name, length)
 
-        else:
-            padding = length - st_size
+    ql.log.debug(f'ftruncate({fd}, {length:#x}) = {regreturn}')
 
-            with open(real_path, 'a+b') as ofile:
-                ofile.write(b'\x00' * padding)
-    except:
-        regreturn = -1
-    else:
-        regreturn = 0
+    return regreturn
 
-    ql.log.debug("ftruncate(%d, 0x%x) = %d" % (fd, length, regreturn))
 
-    return regreturn
+def __do_unlink(ql: Qiling, absvpath: str) -> int:
 
+    def __has_opened_fd(hpath: str) -> bool:
+        opened_fds = (ql.os.fd[i] for i in range(NR_OPEN) if ql.os.fd[i] is not None)
+        f = next((fd for fd in opened_fds if getattr(fd, 'name', '') == hpath), None)
 
-def ql_syscall_unlink(ql: Qiling, pathname: int):
-    file_path = ql.os.utils.read_cstring(pathname)
-    real_path = ql.os.path.transform_to_real_path(file_path)
+        return f is not None and f.closed
 
-    opened_fds = [getattr(ql.os.fd[i], 'name', None) for i in range(NR_OPEN) if ql.os.fd[i] is not None]
-    path = pathlib.Path(real_path)
+    hpath = ql.os.path.virtual_to_host_path(absvpath)
 
-    if any((real_path not in opened_fds, path.is_block_device(), path.is_fifo(), path.is_socket(), path.is_symlink())):
-        try:
-            os.unlink(real_path)
-        except FileNotFoundError:
-            ql.log.debug('No such file or directory')
-            regreturn = -1
-        except:
-            regreturn = -1
-        else:
-            regreturn = 0
+    if ql.os.fs_mapper.has_mapping(absvpath):
+        if __has_opened_fd(hpath):
+            return -1
+
+        ql.os.fs_mapper.remove_mapping(absvpath)
 
     else:
-        regreturn = -1
+        if not ql.os.path.is_safe_host_path(hpath):
+            raise PermissionError(f'unsafe path: {hpath}')
 
-    ql.log.debug("unlink(%s) = %d" % (file_path, regreturn))
+        # NOTE: no idea why these are always ok to remove
+        def __ok_to_remove(hpath: str) -> bool:
+            path = pathlib.Path(hpath)
 
-    return regreturn
+            return any((path.is_block_device(), path.is_fifo(), path.is_socket(), path.is_symlink()))
 
+        if __has_opened_fd(hpath) and not __ok_to_remove(hpath):
+            return -1
 
-def ql_syscall_unlinkat(ql: Qiling, fd: int, pathname: int):
-    file_path = ql.os.utils.read_cstring(pathname)
-    real_path = ql.os.path.transform_to_real_path(file_path)
+        try:
+            os.unlink(hpath)
+        except OSError:
+            return -1
 
-    try:
-        dir_fd = ql.os.fd[fd].fileno()
-    except:
-        dir_fd = None
+    return 0
 
-    try:
-        if dir_fd is None:
-            os.unlink(real_path)
-        else:
-            os.unlink(file_path, dir_fd=dir_fd)
-    except OSError as e:
-        regreturn = -e.errno
-    else:
-        regreturn = 0
 
-    ql.log.debug("unlinkat(fd = %d, path = '%s') = %d" % (fd, file_path, regreturn))
+def ql_syscall_unlink(ql: Qiling, pathname: int):
+    vpath = ql.os.utils.read_cstring(pathname)
+    absvpath = ql.os.path.virtual_abspath(vpath)
+
+    regreturn = __do_unlink(ql, absvpath)
+
+    ql.log.debug(f'unlink("{vpath}") = {regreturn}')
 
     return regreturn
 
+
+def ql_syscall_unlinkat(ql: Qiling, dirfd: int, pathname: int, flags: int):
+    vpath = ql.os.utils.read_cstring(pathname)
+    absvpath = virtual_abspath_at(ql, vpath, dirfd)
+
+    regreturn = -1 if absvpath is None else __do_unlink(ql, absvpath)
+
+    ql.log.debug(f'unlinkat({dirfd}, "{vpath}") = {regreturn}')
+
+    return regreturn
+
+
 # https://man7.org/linux/man-pages/man2/getdents.2.html
 #    struct linux_dirent {
 #        unsigned long  d_ino;     /* Inode number */
 #        unsigned long  d_off;     /* Offset to next linux_dirent */
 #        unsigned short d_reclen;  /* Length of this linux_dirent */
 #        char           d_name[];  /* Filename (null-terminated) */
 #                                  /* length is actually (d_reclen - 2 - offsetof(struct linux_dirent, d_name)) */
@@ -762,15 +873,15 @@
                 break
         else:
             t = 0x0 # DT_UNKNOWN
 
         return bytes([t])
 
     if ql.os.fd[fd].tell() == 0:
-        n = ql.arch.pointersize
+        n = 8 if is_64 else ql.arch.pointersize
         total_size = 0
         results = os.scandir(ql.os.fd[fd].name)
         _ent_count = 0
 
         for result in itertools.chain((pathlib.Path('.'), pathlib.Path('..')), results): # chain speical directories with the results
             d_ino = result.inode() if isinstance(result, os.DirEntry) else result.stat().st_ino
             d_off = 0
@@ -783,16 +894,16 @@
             try:
                 packed_d_ino = (ql.pack(d_ino), n)
             except:
                 packed_d_ino = (ql.pack64(d_ino), n)
 
             if is_64:
                 fields = (
-                    (ql.pack(d_ino), n),
-                    (ql.pack(d_off), n),
+                    (ql.pack64(d_ino), n),
+                    (ql.pack64(d_off), n),
                     (ql.pack16(d_reclen), 2),
                     (d_type, 1),
                     (d_name, len(d_name))
                 )
             else:
                 fields = (
                     packed_d_ino,
@@ -823,9 +934,10 @@
 
     return regreturn
 
 
 def ql_syscall_getdents(ql: Qiling, fd: int, dirp: int, count: int):
     return __getdents_common(ql, fd, dirp, count, is_64=False)
 
+
 def ql_syscall_getdents64(ql: Qiling, fd: int, dirp: int, count: int):
     return __getdents_common(ql, fd, dirp, count, is_64=True)
```

### Comparing `qiling-1.4.5/qiling/os/posix/syscall/utsname.py` & `qiling-1.4.6/qiling/os/posix/syscall/utsname.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/os/posix/syscall/wait.py` & `qiling-1.4.6/qiling/os/posix/syscall/wait.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/os/qnx/const.py` & `qiling-1.4.6/qiling/os/qnx/const.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/os/qnx/helpers.py` & `qiling-1.4.6/qiling/os/qnx/helpers.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/os/qnx/map_msgtype.py` & `qiling-1.4.6/qiling/os/qnx/map_msgtype.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/os/qnx/map_syscall.py` & `qiling-1.4.6/qiling/os/qnx/map_syscall.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/os/qnx/message.py` & `qiling-1.4.6/qiling/os/qnx/message.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/os/qnx/qnx.py` & `qiling-1.4.6/qiling/os/qnx/qnx.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 #!/usr/bin/env python3
-# 
+#
 # Cross Platform and Multi Architecture Advanced Binary Emulation Framework
 #
 
-import os
-
 from unicorn import UcError
 
 from qiling import Qiling
 from qiling.arch import arm_utils
 from qiling.os.posix.posix import QlOsPosix
 from qiling.os.qnx.const import NTO_SIDE_CHANNEL, SYSMGR_PID, SYSMGR_CHID, SYSMGR_COID
 from qiling.os.qnx.helpers import QnxConn
@@ -16,14 +14,15 @@
 
 from qiling.cc import QlCC, intel, arm, mips, riscv, ppc
 from qiling.const import QL_ARCH, QL_OS
 from qiling.os.fcall import QlFunctionCall
 from qiling.os.const import *
 from qiling.os.posix.posix import QlOsPosix
 
+
 class QlOsQnx(QlOsPosix):
     type = QL_OS.QNX
 
     def __init__(self, ql: Qiling):
         super(QlOsQnx, self).__init__(ql)
 
         self.ql = ql
@@ -41,17 +40,16 @@
 
         self.fcall = QlFunctionCall(ql, cc)
 
         self.thread_class = None
         self.futexm = None
         self.fh = None
         self.function_after_load_list = []
-        self.elf_mem_start = 0x0
         self.load()
-        
+
         # use counters to get free Ids
         self.channel_id = 1
         # TODO: replace 0x400 with NR_OPEN from Qiling 1.25
         self.connection_id_lo = 0x400 + 1
         self.connection_id_hi = NTO_SIDE_CHANNEL + 1
         # map Connection Id (coid) to Process Id (pid) and Channel Id (chid)
         self.connections = {}
@@ -71,45 +69,43 @@
             #self.thread_class = thread.QlLinuxARMThread
             arm_utils.init_linux_traps(self.ql, {
                 'memory_barrier': 0xffff0fa0,
                 'cmpxchg': 0xffff0fc0,
                 'get_tls': 0xffff0fe0
             })
 
-
     def hook_syscall(self, ql, intno):
         return self.load_syscall()
 
-
     def register_function_after_load(self, function):
         if function not in self.function_after_load_list:
             self.function_after_load_list.append(function)
 
-
     def run_function_after_load(self):
         for f in self.function_after_load_list:
             f()
 
-
     def run(self):
         if self.ql.exit_point is not None:
             self.exit_point = self.ql.exit_point
 
-        if  self.ql.entry_point is not None:
+        if self.ql.entry_point is not None:
             self.ql.loader.elf_entry = self.ql.entry_point
 
-        self.cpupage_addr        = int(self.ql.os.profile.get("OS32", "cpupage_address"), 16)
-        self.cpupage_tls_addr    = int(self.ql.os.profile.get("OS32", "cpupage_tls_address"), 16)
-        self.tls_data_addr       = int(self.ql.os.profile.get("OS32", "tls_data_address"), 16)
-        self.syspage_addr        = int(self.ql.os.profile.get("OS32", "syspage_address"), 16)
-        syspage_path             = os.path.join(self.ql.rootfs, "syspage.bin")
+        profile = self.ql.os.profile['OS32']
+
+        self.cpupage_addr     = profile.getint('cpupage_address')
+        self.cpupage_tls_addr = profile.getint('cpupage_tls_address')
+        self.tls_data_addr    = profile.getint('tls_data_address')
+        self.syspage_addr     = profile.getint('syspage_address')
 
         self.ql.mem.map(self.syspage_addr, 0x4000, info="[syspage_mem]")
-        
-        with open(syspage_path, "rb") as sp:
+        syspage_hpath = self.ql.os.path.virtual_to_host_path("/syspage.bin")
+
+        with open(syspage_hpath, "rb") as sp:
             self.ql.mem.write(self.syspage_addr, sp.read())
 
         # Address of struct _thread_local_storage for our thread
         self.ql.mem.write_ptr(self.cpupage_addr, self.cpupage_tls_addr, 4)
         tls = _thread_local_storage(self.ql, self.cpupage_tls_addr)
 
         # Fill TLS structure with proper values
```

### Comparing `qiling-1.4.5/qiling/os/qnx/structs.py` & `qiling-1.4.6/qiling/os/qnx/structs.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/os/qnx/syscall.py` & `qiling-1.4.6/qiling/os/qnx/syscall.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/os/stats.py` & `qiling-1.4.6/qiling/os/stats.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/os/struct.py` & `qiling-1.4.6/qiling/os/struct.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/os/thread.py` & `qiling-1.4.6/qiling/os/thread.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/os/uefi/const.py` & `qiling-1.4.6/qiling/os/uefi/const.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,45 +2,45 @@
 # 
 # Cross Platform and Multi Architecture Advanced Binary Emulation Framework
 #
 
 EFI_MAX_BIT = (1 << 63)
 EFI_SUCCESS = 0
 
-EFI_LOAD_ERROR				= EFI_MAX_BIT |  1
-EFI_INVALID_PARAMETER		= EFI_MAX_BIT |  2
-EFI_UNSUPPORTED				= EFI_MAX_BIT |  3
-EFI_BAD_BUFFER_SIZE			= EFI_MAX_BIT |  4
-EFI_BUFFER_TOO_SMALL		= EFI_MAX_BIT |  5
-EFI_NOT_READY				= EFI_MAX_BIT |  6
-EFI_DEVICE_ERROR			= EFI_MAX_BIT |  7
-EFI_WRITE_PROTECTED			= EFI_MAX_BIT |  8
-EFI_OUT_OF_RESOURCES		= EFI_MAX_BIT |  9
-EFI_VOLUME_CORRUPTED		= EFI_MAX_BIT | 10
-EFI_VOLUME_FULL				= EFI_MAX_BIT | 11
-EFI_NO_MEDIA				= EFI_MAX_BIT | 12
-EFI_MEDIA_CHANGED			= EFI_MAX_BIT | 13
-EFI_NOT_FOUND				= EFI_MAX_BIT | 14
-EFI_ACCESS_DENIED			= EFI_MAX_BIT | 15
-EFI_NO_RESPONSE				= EFI_MAX_BIT | 16
-EFI_NO_MAPPING				= EFI_MAX_BIT | 17
-EFI_TIMEOUT					= EFI_MAX_BIT | 18
-EFI_NOT_STARTED				= EFI_MAX_BIT | 19
-EFI_ALREADY_STARTED			= EFI_MAX_BIT | 20
-EFI_ABORTED					= EFI_MAX_BIT | 21
-EFI_ICMP_ERROR				= EFI_MAX_BIT | 22
-EFI_TFTP_ERROR				= EFI_MAX_BIT | 23
-EFI_PROTOCOL_ERROR			= EFI_MAX_BIT | 24
-EFI_INCOMPATIBLE_VERSION	= EFI_MAX_BIT | 25
-EFI_SECURITY_VIOLATION		= EFI_MAX_BIT | 26
-EFI_CRC_ERROR				= EFI_MAX_BIT | 27
-EFI_END_OF_MEDIA			= EFI_MAX_BIT | 28
-EFI_END_OF_FILE				= EFI_MAX_BIT | 31
-EFI_INVALID_LANGUAGE		= EFI_MAX_BIT | 32
+EFI_LOAD_ERROR                = EFI_MAX_BIT |  1
+EFI_INVALID_PARAMETER        = EFI_MAX_BIT |  2
+EFI_UNSUPPORTED                = EFI_MAX_BIT |  3
+EFI_BAD_BUFFER_SIZE            = EFI_MAX_BIT |  4
+EFI_BUFFER_TOO_SMALL        = EFI_MAX_BIT |  5
+EFI_NOT_READY                = EFI_MAX_BIT |  6
+EFI_DEVICE_ERROR            = EFI_MAX_BIT |  7
+EFI_WRITE_PROTECTED            = EFI_MAX_BIT |  8
+EFI_OUT_OF_RESOURCES        = EFI_MAX_BIT |  9
+EFI_VOLUME_CORRUPTED        = EFI_MAX_BIT | 10
+EFI_VOLUME_FULL                = EFI_MAX_BIT | 11
+EFI_NO_MEDIA                = EFI_MAX_BIT | 12
+EFI_MEDIA_CHANGED            = EFI_MAX_BIT | 13
+EFI_NOT_FOUND                = EFI_MAX_BIT | 14
+EFI_ACCESS_DENIED            = EFI_MAX_BIT | 15
+EFI_NO_RESPONSE                = EFI_MAX_BIT | 16
+EFI_NO_MAPPING                = EFI_MAX_BIT | 17
+EFI_TIMEOUT                    = EFI_MAX_BIT | 18
+EFI_NOT_STARTED                = EFI_MAX_BIT | 19
+EFI_ALREADY_STARTED            = EFI_MAX_BIT | 20
+EFI_ABORTED                    = EFI_MAX_BIT | 21
+EFI_ICMP_ERROR                = EFI_MAX_BIT | 22
+EFI_TFTP_ERROR                = EFI_MAX_BIT | 23
+EFI_PROTOCOL_ERROR            = EFI_MAX_BIT | 24
+EFI_INCOMPATIBLE_VERSION    = EFI_MAX_BIT | 25
+EFI_SECURITY_VIOLATION        = EFI_MAX_BIT | 26
+EFI_CRC_ERROR                = EFI_MAX_BIT | 27
+EFI_END_OF_MEDIA            = EFI_MAX_BIT | 28
+EFI_END_OF_FILE                = EFI_MAX_BIT | 31
+EFI_INVALID_LANGUAGE        = EFI_MAX_BIT | 32
 
-EFI_WARN_UNKNOWN_GLYPH		= EFI_MAX_BIT | 1
-EFI_WARN_DELETE_FAILURE		= EFI_MAX_BIT | 2
-EFI_WARN_WRITE_FAILURE		= EFI_MAX_BIT | 3
-EFI_WARN_BUFFER_TOO_SMALL	= EFI_MAX_BIT | 4
+EFI_WARN_UNKNOWN_GLYPH        = EFI_MAX_BIT | 1
+EFI_WARN_DELETE_FAILURE        = EFI_MAX_BIT | 2
+EFI_WARN_WRITE_FAILURE        = EFI_MAX_BIT | 3
+EFI_WARN_BUFFER_TOO_SMALL    = EFI_MAX_BIT | 4
 
 # @see: MdePkg\Include\Base.h
 EFI_ERROR = lambda status: (status & EFI_MAX_BIT) != 0
```

### Comparing `qiling-1.4.5/qiling/os/uefi/fncc.py` & `qiling-1.4.6/qiling/os/uefi/fncc.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/os/uefi/guids.csv` & `qiling-1.4.6/qiling/os/uefi/guids.csv`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/os/uefi/hob.py` & `qiling-1.4.6/qiling/os/uefi/hob.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,102 +4,102 @@
 #
 
 from qiling import Qiling
 from qiling.os.uefi.context import UefiContext
 from qiling.os.uefi.utils import GetEfiConfigurationTable, CompareGuid, str_to_guid
 from qiling.os.uefi.UefiBaseType import STRUCT, EFI_GUID, UINT32, UINT16
 
-EFI_HOB_TYPE_HANDOFF		 = 0x0001
-EFI_HOB_TYPE_GUID_EXTENSION	 = 0x0004
+EFI_HOB_TYPE_HANDOFF         = 0x0001
+EFI_HOB_TYPE_GUID_EXTENSION     = 0x0004
 EFI_HOB_TYPE_END_OF_HOB_LIST = 0xffff
 
 class EFI_HOB_GENERIC_HEADER(STRUCT):
-	_fields_ = [
-		('HobType',		UINT16),
-		('HobLength',	UINT16),
-		('Reserved',	UINT32)
-	]
+    _fields_ = [
+        ('HobType',        UINT16),
+        ('HobLength',    UINT16),
+        ('Reserved',    UINT32)
+    ]
 
 class EFI_HOB_GUID_TYPE(STRUCT):
-	_fields_ = [
-		('Header',	EFI_HOB_GENERIC_HEADER),
-		('Name',	EFI_GUID)
-	]
+    _fields_ = [
+        ('Header',    EFI_HOB_GENERIC_HEADER),
+        ('Name',    EFI_GUID)
+    ]
 
 def GetHobList(ql: Qiling, context: UefiContext) -> int:
-	"""Get HOB list location in memory (ostensibly set by PEI).
-	"""
+    """Get HOB list location in memory (ostensibly set by PEI).
+    """
 
-	hoblist_guid = ql.os.profile['HOB_LIST']['Guid']
-	hoblist_vend = GetEfiConfigurationTable(context, hoblist_guid)
+    hoblist_guid = ql.os.profile['HOB_LIST']['Guid']
+    hoblist_vend = GetEfiConfigurationTable(context, hoblist_guid)
 
-	assert hoblist_vend is not None, 'hob list guid not found'
+    assert hoblist_vend is not None, 'hob list guid not found'
 
-	return hoblist_vend
+    return hoblist_vend
 
 def CreateHob(ql: Qiling, context: UefiContext, hob) -> int:
-	"""Add a HOB to the end of the HOB list.
-	"""
+    """Add a HOB to the end of the HOB list.
+    """
 
-	hoblist = GetHobList(ql, context)
+    hoblist = GetHobList(ql, context)
 
-	# look for the list end marker; uefi codebase assumes there is
-	# always one
-	hoblist = GetNextHob(ql, EFI_HOB_TYPE_END_OF_HOB_LIST, hoblist)
-
-	# overwrite end marker with the hob
-	pHob = hoblist
-	hob.saveTo(ql, pHob)
-	hoblist += hob.sizeof()
-
-	# create a new end marker istead, following the hob
-	marker = EFI_HOB_GENERIC_HEADER()
-	marker.HobType = EFI_HOB_TYPE_END_OF_HOB_LIST
-	marker.HobLength = 0x0000
-	marker.Reserved = 0x00000000
-	marker.saveTo(ql, hoblist)
+    # look for the list end marker; uefi codebase assumes there is
+    # always one
+    hoblist = GetNextHob(ql, EFI_HOB_TYPE_END_OF_HOB_LIST, hoblist)
+
+    # overwrite end marker with the hob
+    pHob = hoblist
+    hob.saveTo(ql, pHob)
+    hoblist += hob.sizeof()
+
+    # create a new end marker istead, following the hob
+    marker = EFI_HOB_GENERIC_HEADER()
+    marker.HobType = EFI_HOB_TYPE_END_OF_HOB_LIST
+    marker.HobLength = 0x0000
+    marker.Reserved = 0x00000000
+    marker.saveTo(ql, hoblist)
 
-	# return the address the hob was written to; it might be useful
-	return pHob
+    # return the address the hob was written to; it might be useful
+    return pHob
 
 def GetNextHob(ql: Qiling, hobtype: int, hoblist: int) -> int:
-	"""Get next HOB on the list.
-	"""
+    """Get next HOB on the list.
+    """
 
-	hobaddr = hoblist
+    hobaddr = hoblist
 
-	while True:
-		header = EFI_HOB_GENERIC_HEADER.loadFrom(ql, hobaddr)
+    while True:
+        header = EFI_HOB_GENERIC_HEADER.loadFrom(ql, hobaddr)
 
-		# found the hob?
-		if header.HobType == hobtype:
-			break
+        # found the hob?
+        if header.HobType == hobtype:
+            break
 
-		# reached end of hob list?
-		if header.HobType == EFI_HOB_TYPE_END_OF_HOB_LIST:
-			return 0
+        # reached end of hob list?
+        if header.HobType == EFI_HOB_TYPE_END_OF_HOB_LIST:
+            return 0
 
-		hobaddr += header.HobLength
+        hobaddr += header.HobLength
 
-	return hobaddr
+    return hobaddr
 
 def GetNextGuidHob(ql: Qiling, guid: str, hoblist: int) -> int:
-	"""Find next HOB with the specified GUID.
-	"""
+    """Find next HOB with the specified GUID.
+    """
 
-	hobguid = str_to_guid(guid)
-	hobaddr = hoblist
+    hobguid = str_to_guid(guid)
+    hobaddr = hoblist
 
-	while True:
-		hobaddr = GetNextHob(ql, EFI_HOB_TYPE_GUID_EXTENSION, hobaddr)
+    while True:
+        hobaddr = GetNextHob(ql, EFI_HOB_TYPE_GUID_EXTENSION, hobaddr)
 
-		if not hobaddr:
-			return 0
+        if not hobaddr:
+            return 0
 
-		hob = EFI_HOB_GUID_TYPE.loadFrom(ql, hobaddr)
+        hob = EFI_HOB_GUID_TYPE.loadFrom(ql, hobaddr)
 
-		if CompareGuid(hob.Name, hobguid):
-			break
+        if CompareGuid(hob.Name, hobguid):
+            break
 
-		hobaddr += hob.Header.HobLength
+        hobaddr += hob.Header.HobLength
 
-	return hobaddr
+    return hobaddr
```

### Comparing `qiling-1.4.5/qiling/os/uefi/protocols/EfiSmmBase2Protocol.py` & `qiling-1.4.6/qiling/os/uefi/protocols/EfiSmmBase2Protocol.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,47 +11,47 @@
 from ..utils import *
 from ..ProcessorBind import *
 from ..UefiBaseType import *
 from ..smst import *
 
 # @see: MdePkg\Include\Protocol\SmmBase2.h
 class EFI_SMM_BASE2_PROTOCOL(STRUCT):
-	EFI_SMM_BASE2_PROTOCOL = STRUCT
+    EFI_SMM_BASE2_PROTOCOL = STRUCT
 
-	_fields_ = [
-		('InSmm',			FUNCPTR(EFI_STATUS, PTR(EFI_SMM_BASE2_PROTOCOL), PTR(BOOLEAN))),
-		('GetSmstLocation',	FUNCPTR(EFI_STATUS, PTR(EFI_SMM_BASE2_PROTOCOL), PTR(PTR(EFI_SMM_SYSTEM_TABLE2)))),
-	]
+    _fields_ = [
+        ('InSmm',            FUNCPTR(EFI_STATUS, PTR(EFI_SMM_BASE2_PROTOCOL), PTR(BOOLEAN))),
+        ('GetSmstLocation',    FUNCPTR(EFI_STATUS, PTR(EFI_SMM_BASE2_PROTOCOL), PTR(PTR(EFI_SMM_SYSTEM_TABLE2)))),
+    ]
 
 @dxeapi(params = {
-	"This"		: POINTER,
-	"InSmram"	: POINTER
+    "This"        : POINTER,
+    "InSmram"    : POINTER
 })
 def hook_InSmm(ql: Qiling, address: int, params):
-	ql.log.debug(f'InSmram = {ql.os.smm.active}')
+    ql.log.debug(f'InSmram = {ql.os.smm.active}')
 
-	write_int8(ql, params["InSmram"], int(ql.os.smm.active))
+    write_int8(ql, params["InSmram"], int(ql.os.smm.active))
 
-	return EFI_SUCCESS
+    return EFI_SUCCESS
 
 @dxeapi(params = {
-	"This"	: POINTER,
-	"Smst"	: POINTER
+    "This"    : POINTER,
+    "Smst"    : POINTER
 })
 def hook_GetSmstLocation(ql: Qiling, address: int, params):
-	Smst = params["Smst"]
+    Smst = params["Smst"]
 
-	if Smst == 0:
-		return EFI_INVALID_PARAMETER
+    if Smst == 0:
+        return EFI_INVALID_PARAMETER
 
-	write_int64(ql, Smst, ql.loader.gSmst)
+    write_int64(ql, Smst, ql.loader.gSmst)
 
-	return EFI_SUCCESS
+    return EFI_SUCCESS
 
 descriptor = {
-	"guid" : "f4ccbfb7-f6e0-47fd-9dd4-10a8f150c191",
-	"struct" : EFI_SMM_BASE2_PROTOCOL,
-	"fields" : (
-		("InSmm",			hook_InSmm),
-		("GetSmstLocation",	hook_GetSmstLocation)
-	)
+    "guid" : "f4ccbfb7-f6e0-47fd-9dd4-10a8f150c191",
+    "struct" : EFI_SMM_BASE2_PROTOCOL,
+    "fields" : (
+        ("InSmm",            hook_InSmm),
+        ("GetSmstLocation",    hook_GetSmstLocation)
+    )
 }
```

### Comparing `qiling-1.4.5/qiling/os/uefi/protocols/EfiSmmSwDispatch2Protocol.py` & `qiling-1.4.6/qiling/os/uefi/protocols/EfiSmmSwDispatch2Protocol.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,114 +10,114 @@
 from ..ProcessorBind import *
 from ..UefiBaseType import *
 from .. import utils
 
 MAXIMUM_SWI_VALUE = 0xff
 
 class EFI_SMM_SW_CONTEXT(STRUCT):
-	_pack_ = 8
+    _pack_ = 8
 
-	_fields_ = [
-		('SwSmiCpuIndex',	UINTN),	# index of the cpu which generated the swsmi
-		('CommandPort',		UINT8),	# port number used to trigger the swsmi
-		('DataPort',		UINT8)	# irrelevant
-	]
+    _fields_ = [
+        ('SwSmiCpuIndex',    UINTN),    # index of the cpu which generated the swsmi
+        ('CommandPort',        UINT8),    # port number used to trigger the swsmi
+        ('DataPort',        UINT8)    # irrelevant
+    ]
 
 # @file: MdePkg\Include\Protocol\SmmSwDispatch2.h
 class EFI_SMM_SW_REGISTER_CONTEXT(STRUCT):
-	_fields_ = [
-		('SwSmiInputValue', UINTN)
-	]
+    _fields_ = [
+        ('SwSmiInputValue', UINTN)
+    ]
 
 # @ file: MdePkg\Include\Pi\PiMmCis.h
 EFI_SMM_HANDLER_ENTRY_POINT2 = FUNCPTR(EFI_STATUS, EFI_HANDLE, PTR(VOID), PTR(VOID), PTR(UINTN))
 
 class EFI_SMM_SW_DISPATCH2_PROTOCOL(STRUCT):
-	EFI_SMM_SW_DISPATCH2_PROTOCOL = STRUCT
+    EFI_SMM_SW_DISPATCH2_PROTOCOL = STRUCT
 
-	_fields_ = [
-		('Register',		FUNCPTR(EFI_STATUS, PTR(EFI_SMM_SW_DISPATCH2_PROTOCOL), EFI_SMM_HANDLER_ENTRY_POINT2, PTR(EFI_SMM_SW_REGISTER_CONTEXT), PTR(EFI_HANDLE))),
-		('UnRegister',		FUNCPTR(EFI_STATUS, PTR(EFI_SMM_SW_DISPATCH2_PROTOCOL), EFI_HANDLE)),
-		('MaximumSwiValue',	UINTN)
-	]
+    _fields_ = [
+        ('Register',        FUNCPTR(EFI_STATUS, PTR(EFI_SMM_SW_DISPATCH2_PROTOCOL), EFI_SMM_HANDLER_ENTRY_POINT2, PTR(EFI_SMM_SW_REGISTER_CONTEXT), PTR(EFI_HANDLE))),
+        ('UnRegister',        FUNCPTR(EFI_STATUS, PTR(EFI_SMM_SW_DISPATCH2_PROTOCOL), EFI_HANDLE)),
+        ('MaximumSwiValue',    UINTN)
+    ]
 
 @dxeapi(params = {
-	"This"				: POINTER,	# PTR(EFI_SMM_SW_DISPATCH2_PROTOCOL)
-	"DispatchFunction"	: POINTER,	# EFI_SMM_HANDLER_ENTRY_POINT2
-	"RegisterContext"	: POINTER,	# PTR(EFI_SMM_SW_REGISTER_CONTEXT)
-	"DispatchHandle"	: POINTER	# PTR(EFI_HANDLE)
+    "This"                : POINTER,    # PTR(EFI_SMM_SW_DISPATCH2_PROTOCOL)
+    "DispatchFunction"    : POINTER,    # EFI_SMM_HANDLER_ENTRY_POINT2
+    "RegisterContext"    : POINTER,    # PTR(EFI_SMM_SW_REGISTER_CONTEXT)
+    "DispatchHandle"    : POINTER    # PTR(EFI_HANDLE)
 })
 def hook_Register(ql: Qiling, address: int, params):
-	DispatchFunction: int = params['DispatchFunction']
-	RegisterContext: int = params['RegisterContext']
-	DispatchHandle: int = params['DispatchHandle']
+    DispatchFunction: int = params['DispatchFunction']
+    RegisterContext: int = params['RegisterContext']
+    DispatchHandle: int = params['DispatchHandle']
 
-	if DispatchFunction == 0 or DispatchHandle == 0:
-		return EFI_INVALID_PARAMETER
+    if DispatchFunction == 0 or DispatchHandle == 0:
+        return EFI_INVALID_PARAMETER
 
-	handlers = ql.loader.smm_context.swsmi_handlers
+    handlers = ql.loader.smm_context.swsmi_handlers
 
-	SwRegisterContext = EFI_SMM_SW_REGISTER_CONTEXT.loadFrom(ql, RegisterContext)
-	idx = SwRegisterContext.SwSmiInputValue
+    SwRegisterContext = EFI_SMM_SW_REGISTER_CONTEXT.loadFrom(ql, RegisterContext)
+    idx = SwRegisterContext.SwSmiInputValue
 
-	# a value of -1 indicates that the swsmi index for this handler is flexible and
-	# should be assigned by the protocol
-	if idx == ((1 << ql.arch.bits) - 1):
-		idx = next((i for i in range(1, MAXIMUM_SWI_VALUE) if i not in handlers), None)
+    # a value of -1 indicates that the swsmi index for this handler is flexible and
+    # should be assigned by the protocol
+    if idx == ((1 << ql.arch.bits) - 1):
+        idx = next((i for i in range(1, MAXIMUM_SWI_VALUE) if i not in handlers), None)
 
-		if idx is None:
-			return EFI_OUT_OF_RESOURCES
+        if idx is None:
+            return EFI_OUT_OF_RESOURCES
 
-		SwRegisterContext.SwSmiInputValue = idx
-		SwRegisterContext.saveTo(ql, RegisterContext)
+        SwRegisterContext.SwSmiInputValue = idx
+        SwRegisterContext.saveTo(ql, RegisterContext)
 
-	else:
-		This = EFI_SMM_SW_DISPATCH2_PROTOCOL.loadFrom(ql, params['This'])
+    else:
+        This = EFI_SMM_SW_DISPATCH2_PROTOCOL.loadFrom(ql, params['This'])
 
-		if idx in handlers:
-			return EFI_INVALID_PARAMETER
+        if idx in handlers:
+            return EFI_INVALID_PARAMETER
 
-		if idx > This.MaximumSwiValue:
-			return EFI_INVALID_PARAMETER
+        if idx > This.MaximumSwiValue:
+            return EFI_INVALID_PARAMETER
 
-	# allocate handle and return it through out parameter
-	Handle = ql.loader.smm_context.heap.alloc(ql.arch.pointersize)
-	utils.write_int64(ql, DispatchHandle, Handle)
+    # allocate handle and return it through out parameter
+    Handle = ql.loader.smm_context.heap.alloc(ql.arch.pointersize)
+    utils.write_int64(ql, DispatchHandle, Handle)
 
-	args = {
-		'DispatchHandle'  : Handle,
-		'RegisterContext' : SwRegisterContext
-	}
+    args = {
+        'DispatchHandle'  : Handle,
+        'RegisterContext' : SwRegisterContext
+    }
 
-	handlers[idx] = (DispatchFunction, args)
+    handlers[idx] = (DispatchFunction, args)
 
-	return EFI_SUCCESS
+    return EFI_SUCCESS
 
 @dxeapi(params = {
-	"This"				: POINTER,
-	"DispatchHandle"	: POINTER
+    "This"                : POINTER,
+    "DispatchHandle"    : POINTER
 })
 def hook_UnRegister(ql: Qiling, address: int, params):
-	DispatchHandle: int = params['DispatchHandle']
+    DispatchHandle: int = params['DispatchHandle']
 
-	handlers = ql.loader.smm_context.swsmi_handlers
-	heap = ql.loader.smm_context.heap
+    handlers = ql.loader.smm_context.swsmi_handlers
+    heap = ql.loader.smm_context.heap
 
-	idx = next((idx for idx, (_, args) in handlers.items() if args['DispatchHandle'] == DispatchHandle), None)
+    idx = next((idx for idx, (_, args) in handlers.items() if args['DispatchHandle'] == DispatchHandle), None)
 
-	if idx is None:
-		return EFI_INVALID_PARAMETER
+    if idx is None:
+        return EFI_INVALID_PARAMETER
 
-	heap.free(DispatchHandle)
-	del handlers[idx]
+    heap.free(DispatchHandle)
+    del handlers[idx]
 
-	return EFI_SUCCESS
+    return EFI_SUCCESS
 
 descriptor = {
-	"guid" : "18a3c6dc-5eea-48c8-a1c1-b53389f98999",
-	"struct" : EFI_SMM_SW_DISPATCH2_PROTOCOL,
-	"fields" : (
-		("Register",		hook_Register),
-		("UnRegister",		hook_UnRegister),
-		('MaximumSwiValue',	MAXIMUM_SWI_VALUE)
-	)
+    "guid" : "18a3c6dc-5eea-48c8-a1c1-b53389f98999",
+    "struct" : EFI_SMM_SW_DISPATCH2_PROTOCOL,
+    "fields" : (
+        ("Register",        hook_Register),
+        ("UnRegister",        hook_UnRegister),
+        ('MaximumSwiValue',    MAXIMUM_SWI_VALUE)
+    )
 }
```

### Comparing `qiling-1.4.5/qiling/os/uefi/protocols/common.py` & `qiling-1.4.6/qiling/os/uefi/protocols/common.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,131 +4,131 @@
 #
 
 from qiling.os.uefi.const import EFI_SUCCESS, EFI_NOT_FOUND, EFI_UNSUPPORTED, EFI_BUFFER_TOO_SMALL, EFI_INVALID_PARAMETER
 from qiling.os.uefi.utils import read_int64, write_int64
 from qiling.os.uefi.UefiSpec import EFI_LOCATE_SEARCH_TYPE
 
 def LocateHandles(context, params):
-	SearchType = params["SearchType"]
-	Protocol = params["Protocol"]
+    SearchType = params["SearchType"]
+    Protocol = params["Protocol"]
 
-	# get all handles
-	if SearchType == EFI_LOCATE_SEARCH_TYPE.AllHandles:
-		handles = context.protocols.keys()
+    # get all handles
+    if SearchType == EFI_LOCATE_SEARCH_TYPE.AllHandles:
+        handles = context.protocols.keys()
 
-	# get all handles that support the specified protocol
-	elif SearchType == EFI_LOCATE_SEARCH_TYPE.ByProtocol:
-		handles = [handle for handle, guid_dic in context.protocols.items() if Protocol in guid_dic]
+    # get all handles that support the specified protocol
+    elif SearchType == EFI_LOCATE_SEARCH_TYPE.ByProtocol:
+        handles = [handle for handle, guid_dic in context.protocols.items() if Protocol in guid_dic]
 
-	else:
-		handles = []
+    else:
+        handles = []
 
-	return len(handles) * context.ql.arch.pointersize, handles
+    return len(handles) * context.ql.arch.pointersize, handles
 
 def InstallProtocolInterface(context, params):
-	handle = read_int64(context.ql, params["Handle"])
+    handle = read_int64(context.ql, params["Handle"])
 
-	if handle == 0:
-		handle = context.heap.alloc(1)
+    if handle == 0:
+        handle = context.heap.alloc(1)
 
-	dic = context.protocols.get(handle, {})
+    dic = context.protocols.get(handle, {})
 
-	dic[params["Protocol"]] = params["Interface"]
-	context.protocols[handle] = dic
+    dic[params["Protocol"]] = params["Interface"]
+    context.protocols[handle] = dic
 
-	write_int64(context.ql, params["Handle"], handle)
-	context.notify_protocol(params['Handle'], params['Protocol'], params['Interface'], True)
+    write_int64(context.ql, params["Handle"], handle)
+    context.notify_protocol(params['Handle'], params['Protocol'], params['Interface'], True)
 
-	return EFI_SUCCESS
+    return EFI_SUCCESS
 
 def ReinstallProtocolInterface(context, params):
-	handle = params["Handle"]
+    handle = params["Handle"]
 
-	if handle not in context.protocols:
-		return EFI_NOT_FOUND
+    if handle not in context.protocols:
+        return EFI_NOT_FOUND
 
-	dic = context.protocols[handle]
-	protocol = params["Protocol"]
+    dic = context.protocols[handle]
+    protocol = params["Protocol"]
 
-	if protocol not in dic:
-		return EFI_NOT_FOUND
+    if protocol not in dic:
+        return EFI_NOT_FOUND
 
-	dic[protocol] = params["NewInterface"]
+    dic[protocol] = params["NewInterface"]
 
-	return EFI_SUCCESS
+    return EFI_SUCCESS
 
 def UninstallProtocolInterface(context, params):
-	handle = params["Handle"]
+    handle = params["Handle"]
 
-	if handle not in context.protocols:
-		return EFI_NOT_FOUND
+    if handle not in context.protocols:
+        return EFI_NOT_FOUND
 
-	dic = context.protocols[handle]
-	protocol = params["Protocol"]
+    dic = context.protocols[handle]
+    protocol = params["Protocol"]
 
-	if protocol not in dic:
-		return EFI_NOT_FOUND
+    if protocol not in dic:
+        return EFI_NOT_FOUND
 
-	del dic[protocol]
+    del dic[protocol]
 
-	return EFI_SUCCESS
+    return EFI_SUCCESS
 
 def HandleProtocol(context, params):
-	handle = params["Handle"]
-	protocol = params["Protocol"]
-	interface = params['Interface']
+    handle = params["Handle"]
+    protocol = params["Protocol"]
+    interface = params['Interface']
 
-	if handle in context.protocols:
-		supported = context.protocols[handle]
+    if handle in context.protocols:
+        supported = context.protocols[handle]
 
-		if protocol in supported:
-			write_int64(context.ql, interface, supported[protocol])
+        if protocol in supported:
+            write_int64(context.ql, interface, supported[protocol])
 
-			return EFI_SUCCESS
+            return EFI_SUCCESS
 
-	return EFI_UNSUPPORTED
+    return EFI_UNSUPPORTED
 
 def LocateHandle(context, params):
-	buffer_size, handles = LocateHandles(context, params)
+    buffer_size, handles = LocateHandles(context, params)
 
-	if len(handles) == 0:
-		return EFI_NOT_FOUND
+    if len(handles) == 0:
+        return EFI_NOT_FOUND
 
-	ret = EFI_BUFFER_TOO_SMALL
+    ret = EFI_BUFFER_TOO_SMALL
 
-	if read_int64(context.ql, params["BufferSize"]) >= buffer_size:
-		ptr = params["Buffer"]
+    if read_int64(context.ql, params["BufferSize"]) >= buffer_size:
+        ptr = params["Buffer"]
 
-		for handle in handles:
-			write_int64(context.ql, ptr, handle)
-			ptr += context.ql.arch.pointersize
+        for handle in handles:
+            write_int64(context.ql, ptr, handle)
+            ptr += context.ql.arch.pointersize
 
-		ret = EFI_SUCCESS
+        ret = EFI_SUCCESS
 
-	write_int64(context.ql, params["BufferSize"], buffer_size)
+    write_int64(context.ql, params["BufferSize"], buffer_size)
 
-	return ret
+    return ret
 
 def LocateProtocol(context, params):
-	protocol = params['Protocol']
+    protocol = params['Protocol']
 
-	for handle, guid_dic in context.protocols.items():
-		if "Handle" in params and params["Handle"] != handle:
-			continue
-
-		if protocol in guid_dic:
-			# write protocol address to out variable Interface
-			write_int64(context.ql, params['Interface'], guid_dic[protocol])
-			return EFI_SUCCESS
+    for handle, guid_dic in context.protocols.items():
+        if "Handle" in params and params["Handle"] != handle:
+            continue
+
+        if protocol in guid_dic:
+            # write protocol address to out variable Interface
+            write_int64(context.ql, params['Interface'], guid_dic[protocol])
+            return EFI_SUCCESS
 
-	return EFI_NOT_FOUND
+    return EFI_NOT_FOUND
 
 def InstallConfigurationTable(context, params):
-	guid = params["Guid"]
-	table = params["Table"]
+    guid = params["Guid"]
+    table = params["Table"]
 
-	if not guid:
-		return EFI_INVALID_PARAMETER
+    if not guid:
+        return EFI_INVALID_PARAMETER
 
-	context.conftable.install(guid, table)
+    context.conftable.install(guid, table)
 
-	return EFI_SUCCESS
+    return EFI_SUCCESS
```

### Comparing `qiling-1.4.5/qiling/os/uefi/type32.py` & `qiling-1.4.6/qiling/os/uefi/type32.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/os/uefi/type64.py` & `qiling-1.4.6/qiling/os/uefi/type64.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/os/uefi/utils.py` & `qiling-1.4.6/qiling/os/uefi/utils.py`

 * *Files 27% similar despite different names*

```diff
@@ -9,181 +9,181 @@
 from typing import Optional, Mapping
 
 from qiling import Qiling
 from qiling.os.uefi.const import EFI_SUCCESS
 from qiling.os.uefi.UefiBaseType import EFI_GUID
 
 def signal_event(ql: Qiling, event_id: int) -> None:
-	event = ql.loader.events[event_id]
+    event = ql.loader.events[event_id]
 
-	if not event["Set"]:
-		event["Set"] = True
-		notify_func = event["NotifyFunction"]
-		callback_args = event["CallbackArgs"]
+    if not event["Set"]:
+        event["Set"] = True
+        notify_func = event["NotifyFunction"]
+        callback_args = event["CallbackArgs"]
 
-		ql.loader.notify_list.append((event_id, notify_func, callback_args))
+        ql.loader.notify_list.append((event_id, notify_func, callback_args))
 
 def execute_protocol_notifications(ql: Qiling, from_hook: bool = False) -> bool:
-	if not ql.loader.notify_list:
-		return False
+    if not ql.loader.notify_list:
+        return False
 
-	next_hook = ql.loader.context.heap.alloc(ql.arch.pointersize)
+    next_hook = ql.loader.context.heap.alloc(ql.arch.pointersize)
 
-	def __notify_next(ql: Qiling):
-		# discard previous callback's shadow space
-		ql.arch.regs.arch_sp += (4 * ql.arch.pointersize)
+    def __notify_next(ql: Qiling):
+        # discard previous callback's shadow space
+        ql.arch.regs.arch_sp += (4 * ql.arch.pointersize)
 
-		if ql.loader.notify_list:
-			event_id, notify_func, callback_args = ql.loader.notify_list.pop(0)
-			ql.log.info(f'Notify event: id = {event_id}, (*{notify_func:#x})({", ".join(f"{a:#x}" for a in callback_args)})')
+        if ql.loader.notify_list:
+            event_id, notify_func, callback_args = ql.loader.notify_list.pop(0)
+            ql.log.info(f'Notify event: id = {event_id}, (*{notify_func:#x})({", ".join(f"{a:#x}" for a in callback_args)})')
 
-			ql.loader.call_function(notify_func, callback_args, next_hook)
-		else:
-			ql.log.info(f'Notify event: done')
+            ql.loader.call_function(notify_func, callback_args, next_hook)
+        else:
+            ql.log.info(f'Notify event: done')
 
-			# the last item on the list has been notified; tear down this hook
-			ql.loader.context.heap.free(next_hook)
-			hret.remove()
+            # the last item on the list has been notified; tear down this hook
+            ql.loader.context.heap.free(next_hook)
+            hret.remove()
 
-			ql.arch.regs.rax = EFI_SUCCESS
-			ql.arch.regs.arch_pc = ql.stack_pop()
+            ql.arch.regs.rax = EFI_SUCCESS
+            ql.arch.regs.arch_pc = ql.stack_pop()
 
-	hret = ql.hook_address(__notify_next, next_hook)
+    hret = ql.hook_address(__notify_next, next_hook)
 
-	# __notify_next unwinds the previous callback shadow space allocated by call_function. however, on its first invocation
-	# there is no such shadow space. to maintain stack consistency we set here a bogus shadow space that may be discarded
-	# safely
-	ql.arch.regs.arch_sp -= (4 * ql.arch.pointersize)
+    # __notify_next unwinds the previous callback shadow space allocated by call_function. however, on its first invocation
+    # there is no such shadow space. to maintain stack consistency we set here a bogus shadow space that may be discarded
+    # safely
+    ql.arch.regs.arch_sp -= (4 * ql.arch.pointersize)
 
-	# To avoid having two versions of the code the first notify function will also be called from the __notify_next hook.
-	if from_hook:
-		ql.stack_push(next_hook)
-	else:
-		ql.stack_push(ql.loader.context.end_of_execution_ptr)
-		ql.arch.regs.arch_pc = next_hook
+    # To avoid having two versions of the code the first notify function will also be called from the __notify_next hook.
+    if from_hook:
+        ql.stack_push(next_hook)
+    else:
+        ql.stack_push(ql.loader.context.end_of_execution_ptr)
+        ql.arch.regs.arch_pc = next_hook
 
-	return True
+    return True
 
 def ptr_read8(ql: Qiling, addr: int) -> int:
-	"""Read BYTE data from a pointer
-	"""
+    """Read BYTE data from a pointer
+    """
 
-	return ql.mem.read_ptr(addr, 1)
+    return ql.mem.read_ptr(addr, 1)
 
 def ptr_write8(ql: Qiling, addr: int, val: int) -> None:
-	"""Write BYTE data to a pointer
-	"""
+    """Write BYTE data to a pointer
+    """
 
-	ql.mem.write_ptr(addr, val, 1)
+    ql.mem.write_ptr(addr, val, 1)
 
 def ptr_read16(ql: Qiling, addr: int) -> int:
-	"""Read WORD data from a pointer
-	"""
+    """Read WORD data from a pointer
+    """
 
-	return ql.mem.read_ptr(addr, 2)
+    return ql.mem.read_ptr(addr, 2)
 
 def ptr_write16(ql: Qiling, addr: int, val: int) -> None:
-	"""Write WORD data to a pointer
-	"""
+    """Write WORD data to a pointer
+    """
 
-	ql.mem.write_ptr(addr, val, 2)
+    ql.mem.write_ptr(addr, val, 2)
 
 def ptr_read32(ql: Qiling, addr: int) -> int:
-	"""Read DWORD data from a pointer
-	"""
+    """Read DWORD data from a pointer
+    """
 
-	return ql.mem.read_ptr(addr, 4)
+    return ql.mem.read_ptr(addr, 4)
 
 def ptr_write32(ql: Qiling, addr: int, val: int) -> None:
-	"""Write DWORD data to a pointer
-	"""
+    """Write DWORD data to a pointer
+    """
 
-	ql.mem.write_ptr(addr, val, 4)
+    ql.mem.write_ptr(addr, val, 4)
 
 def ptr_read64(ql: Qiling, addr: int) -> int:
-	"""Read QWORD data from a pointer
-	"""
+    """Read QWORD data from a pointer
+    """
 
-	return ql.mem.read_ptr(addr, 8)
+    return ql.mem.read_ptr(addr, 8)
 
 def ptr_write64(ql: Qiling, addr: int, val: int) -> None:
-	"""Write QWORD data to a pointer
-	"""
+    """Write QWORD data to a pointer
+    """
 
-	ql.mem.write_ptr(addr, val, 8)
+    ql.mem.write_ptr(addr, val, 8)
 
 # backward comptability
 read_int8   = ptr_read8
 write_int8  = ptr_write8
 read_int16  = ptr_read16
 write_int16 = ptr_write16
 read_int32  = ptr_read32
 write_int32 = ptr_write32
 read_int64  = ptr_read64
 write_int64 = ptr_write64
 
 def init_struct(ql: Qiling, base: int, descriptor: Mapping):
-	struct_class = descriptor['struct']
-	struct_fields = descriptor.get('fields', [])
+    struct_class = descriptor['struct']
+    struct_fields = descriptor.get('fields', [])
 
-	isntance = struct_class()
-	ql.log.info(f'Initializing {struct_class.__name__}')
+    isntance = struct_class()
+    ql.log.info(f'Initializing {struct_class.__name__}')
 
-	for name, value in struct_fields:
-		if value is not None:
-			# a method: hook this field
-			if callable(value):
-				p = base + struct_class.offsetof(name)
+    for name, value in struct_fields:
+        if value is not None:
+            # a method: hook this field
+            if callable(value):
+                p = base + struct_class.offsetof(name)
 
-				setattr(isntance, name, p)
-				ql.hook_address(value, p)
+                setattr(isntance, name, p)
+                ql.hook_address(value, p)
 
-				ql.log.info(f' | {name:36s} {p:#010x}')
+                ql.log.info(f' | {name:36s} {p:#010x}')
 
-			# a value: set it
-			else:
-				setattr(isntance, name, value)
+            # a value: set it
+            else:
+                setattr(isntance, name, value)
 
-	ql.log.info(f'')
+    ql.log.info(f'')
 
-	return isntance
+    return isntance
 
 def str_to_guid(guid: str) -> EFI_GUID:
-	"""Construct an EFI_GUID structure out of a plain GUID string.
-	"""
+    """Construct an EFI_GUID structure out of a plain GUID string.
+    """
 
-	buff = UUID(hex=guid).bytes_le
+    buff = UUID(hex=guid).bytes_le
 
-	return EFI_GUID.from_buffer_copy(buff)
+    return EFI_GUID.from_buffer_copy(buff)
 
 def CompareGuid(guid1: EFI_GUID, guid2: EFI_GUID) -> bool:
-	return bytes(guid1) == bytes(guid2)
+    return bytes(guid1) == bytes(guid2)
 
 def install_configuration_table(context, key: str, table: Optional[int]):
-	"""Create a new Configuration Table entry and add it to the list.
+    """Create a new Configuration Table entry and add it to the list.
 
-	Args:
-		ql    : Qiling instance
-		key   : profile section name that holds the entry data
-		table : address of configuration table data; if None, data will be read
-		        from profile section into memory
-	"""
-
-	cfgtable = context.ql.os.profile[key]
-	guid = cfgtable['Guid']
-
-	# if pointer to table data was not specified, load table data
-	# from profile and have table pointing to it
-	if table is None:
-		data = binascii.unhexlify(cfgtable['TableData'])
-		table = context.conf_table_data_next_ptr
+    Args:
+        ql    : Qiling instance
+        key   : profile section name that holds the entry data
+        table : address of configuration table data; if None, data will be read
+                from profile section into memory
+    """
+
+    cfgtable = context.ql.os.profile[key]
+    guid = cfgtable['Guid']
+
+    # if pointer to table data was not specified, load table data
+    # from profile and have table pointing to it
+    if table is None:
+        data = binascii.unhexlify(cfgtable['TableData'])
+        table = context.conf_table_data_next_ptr
 
-		context.ql.mem.write(table, data)
-		context.conf_table_data_next_ptr += len(data)
+        context.ql.mem.write(table, data)
+        context.conf_table_data_next_ptr += len(data)
 
-	context.conftable.install(guid, table)
+    context.conftable.install(guid, table)
 
 def GetEfiConfigurationTable(context, guid: str) -> Optional[int]:
-	"""Find a configuration table by its GUID.
-	"""
+    """Find a configuration table by its GUID.
+    """
 
-	return context.conftable.get_vendor_table(guid)
+    return context.conftable.get_vendor_table(guid)
```

### Comparing `qiling-1.4.5/qiling/os/utils.py` & `qiling-1.4.6/qiling/os/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #!/usr/bin/env python3
-# 
+#
 # Cross Platform and Multi Architecture Advanced Binary Emulation Framework
 #
 
 """
 This module is intended for general purpose functions that are only used in qiling.os
 """
 
@@ -12,50 +12,69 @@
 
 from qiling import Qiling
 from qiling.const import QL_VERBOSE
 
 # TODO: separate windows-specific implementation
 from qiling.os.windows.structs import make_unicode_string
 
-class QlOsUtils:
 
+class QlOsUtils:
     ELLIPSIS_PREF = r'__qlva_'
 
     def __init__(self, ql: Qiling):
         self.ql = ql
 
-    @staticmethod
-    def read_string(ql: Qiling, address: int, terminator: bytes) -> str:
-        result = bytearray()
+    def read_string(self, address: int, encoding: str, maxlen: int = 0) -> str:
+        """Read a null-terminated string from memory.
+
+        Args:
+            address : starting address
+            encoding: string encoding to use
+            maxlen  : limit number of characters to read before reaching null terminator,
+                      0 for unlimited length
+
+        Returns: decoded string
+        """
+
+        terminator = '\x00'.encode(encoding)
+
+        data = bytearray()
         charlen = len(terminator)
+        strlen = 0
 
-        char = ql.mem.read(address, charlen)
+        while True:
+            char = self.ql.mem.read(address, charlen)
 
-        while char != terminator:
-            address += charlen
-            result += char
-            char = ql.mem.read(address, charlen)
+            if char == terminator:
+                break
 
-        return result.decode(errors="ignore")
+            data += char
+            strlen += 1
 
-    def read_wstring(self, address: int) -> str:
-        s = QlOsUtils.read_string(self.ql, address, b'\x00\x00')
+            if strlen == maxlen:
+                break
+
+            address += charlen
 
-        # We need to remove \x00 inside the string. Compares do not work otherwise
-        s = s.replace("\x00", "")
+        s = data.decode(encoding, errors='backslashreplace')
         self.ql.os.stats.log_string(s)
 
         return s
 
-    def read_cstring(self, address: int) -> str:
-        s = QlOsUtils.read_string(self.ql, address, b'\x00')
+    def read_wstring(self, address: int, maxlen: int = 0) -> str:
+        """Read a null-terminated wide string from memory.
+        """
 
-        self.ql.os.stats.log_string(s)
+        return self.read_string(address, 'utf-16le', maxlen)
 
-        return s
+    def read_cstring(self, address: int, maxlen: int = 0) -> str:
+        """Read a null-terminated ASCII string from memory.
+        """
+
+        return self.read_string(address, 'latin1', maxlen)
 
     def read_guid(self, address: int) -> UUID:
         raw_guid = self.ql.mem.read(address, 16)
 
         return UUID(bytes_le=bytes(raw_guid))
 
     @staticmethod
```

### Comparing `qiling-1.4.5/qiling/os/windows/api.py` & `qiling-1.4.6/qiling/os/windows/api.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #!/usr/bin/env python3
-# 
+#
 # Cross Platform and Multi Architecture Advanced Binary Emulation Framework
 #
 
 from qiling.os.const import *
 
 # See: https://docs.microsoft.com/en-us/windows/win32/winprog/windows-data-types
 
@@ -52,29 +52,25 @@
 HMODULE                     = HANDLE
 HWND                        = HANDLE
 PSID                        = HANDLE
 SC_HANDLE                   = HANDLE
 
 LPCSTR                      = STRING
 LPOSVERSIONINFOA            = STRING
-PANSI_STRING                = STRING
-PCANSI_STRING               = STRING
 PCNZCH                      = STRING
 PCSTR                       = STRING
 PCSZ                        = STRING
 
 BSTR                        = WSTRING
 LPCTSTR                     = WSTRING
 LPCWSTR                     = WSTRING
 LPOSVERSIONINFOW            = WSTRING
 OLECHAR                     = WSTRING
 PCNZWCH                     = WSTRING
-PCUNICODE_STRING            = WSTRING
 PCWSTR                      = WSTRING
-PUNICODE_STRING             = WSTRING
 
 DLGPROC                     = POINTER
 DWORD_PTR                   = POINTER
 HDC                         = POINTER
 HGLOBAL                     = POINTER
 HHOOK                       = POINTER
 HINTERNET                   = POINTER
@@ -119,14 +115,18 @@
 LPWCH                       = POINTER
 LPWIN32_FIND_DATAA          = POINTER
 LPWORD                      = POINTER
 LPWSADATA                   = POINTER
 LPWSAPROTOCOL_INFOA         = POINTER
 LPWSTR                      = POINTER
 MSIHANDLE                   = POINTER
+PANSI_STRING                = POINTER
+PUNICODE_STRING             = POINTER
+PCANSI_STRING               = POINTER
+PCUNICODE_STRING            = POINTER
 PACCESS_STATE               = POINTER
 PBOOL                       = POINTER
 PBYTE                       = POINTER
 PCACTCTXW                   = POINTER
 PCLIENT_ID                  = POINTER
 PCONSOLE_SCREEN_BUFFER_INFO = POINTER
 PDEVICE_OBJECT              = POINTER
```

### Comparing `qiling-1.4.5/qiling/os/windows/clipboard.py` & `qiling-1.4.6/qiling/os/windows/clipboard.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/os/windows/const.py` & `qiling-1.4.6/qiling/os/windows/const.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #!/usr/bin/env python3
-# 
+#
 # Cross Platform and Multi Architecture Advanced Binary Emulation Framework
 #
 from Registry import Registry
 
 # ERRORS CODE
 # https://docs.microsoft.com/en-us/windows/win32/debug/system-error-codes--0-499-
 ERROR_SUCCESS = 0x0
@@ -31,14 +31,16 @@
 # https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-erref/596a1078-e883-4972-9bbc-49e60bebca55
 STATUS_SUCCESS = 0
 STATUS_UNSUCCESSFUL = 0xC0000001
 # ...
 STATUS_INFO_LENGTH_MISMATCH = 0xC0000004
 STATUS_INVALID_PARAMETER = 0xC000000D
 STATUS_INVALID_HANDLE = 0xC0000008
+STATUS_PROCEDURE_NOT_FOUND = 0xC000007A
+STATUS_DLL_NOT_FOUND = 0xC0000135
 STATUS_PORT_NOT_SET = 0xC0000353
 STATUS_NO_YIELD_PERFORMED = 0x40000024
 # ...
 
 INVALID_HANDLE_VALUE = -1
 
 STD_INPUT_HANDLE  = 0xfffffff6  # -10
```

### Comparing `qiling-1.4.5/qiling/os/windows/dlls/__init__.py` & `qiling-1.4.6/qiling/os/windows/dlls/__init__.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/os/windows/dlls/advapi32.py` & `qiling-1.4.6/qiling/os/windows/dlls/advapi32.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/os/windows/dlls/crypt32.py` & `qiling-1.4.6/qiling/os/windows/dlls/crypt32.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/os/windows/dlls/kernel32/__init__.py` & `qiling-1.4.6/qiling/os/windows/dlls/kernel32/__init__.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/os/windows/dlls/kernel32/consoleapi2.py` & `qiling-1.4.6/qiling/os/windows/dlls/kernel32/consoleapi2.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/os/windows/dlls/kernel32/debugapi.py` & `qiling-1.4.6/qiling/os/windows/dlls/kernel32/debugapi.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/os/windows/dlls/kernel32/errhandlingapi.py` & `qiling-1.4.6/qiling/os/windows/dlls/kernel32/errhandlingapi.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/os/windows/dlls/kernel32/fibersapi.py` & `qiling-1.4.6/qiling/os/windows/dlls/kernel32/fibersapi.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/os/windows/dlls/kernel32/fileapi.py` & `qiling-1.4.6/qiling/os/windows/dlls/kernel32/fileapi.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,29 +48,21 @@
 
     if not filename:
         return INVALID_HANDLE_VALUE
 
     if len(filename) >= MAX_PATH:
         return ERROR_INVALID_PARAMETER
 
-    host_path = ql.os.path.virtual_to_host_path(filename)
-
-    # Verify the directory is in ql.rootfs to ensure no path traversal has taken place
-    if not ql.os.path.is_safe_host_path(host_path):
-        ql.os.last_error = ERROR_FILE_NOT_FOUND
-
-        return INVALID_HANDLE_VALUE
-
     # Check if path exists
     filesize = 0
 
     try:
-        f = ql.os.fs_mapper.open(host_path, "r")
+        f = ql.os.fs_mapper.open(filename, "r")
 
-        filesize = os.path.getsize(host_path)
+        filesize = os.path.getsize(f.name)
     except FileNotFoundError:
         ql.os.last_error = ERROR_FILE_NOT_FOUND
 
         return INVALID_HANDLE_VALUE
 
     # Create a handle for the path
     new_handle = Handle(obj=f)
@@ -218,27 +210,114 @@
     return 1
 
 def _CreateFile(ql: Qiling, address: int, params):
     s_lpFileName = params["lpFileName"]
     dwDesiredAccess = params["dwDesiredAccess"]
     # dwShareMode = params["dwShareMode"]
     # lpSecurityAttributes = params["lpSecurityAttributes"]
-    # dwCreationDisposition = params["dwCreationDisposition"]
+    
+    # Handle Creation Disposition. I.e. how to respond
+    # when a file either exists or doesn't
+    # See https://learn.microsoft.com/en-us/windows/win32/api/fileapi/nf-fileapi-createfilea
+    dwCreationDisposition = params["dwCreationDisposition"]
+
     # dwFlagsAndAttributes = params["dwFlagsAndAttributes"]
     # hTemplateFile = params["hTemplateFile"]
 
     # access mask DesiredAccess
-    if dwDesiredAccess & GENERIC_WRITE:
-        mode = "wb"
-    else:
+    perm_write = dwDesiredAccess & GENERIC_WRITE
+    perm_read  = dwDesiredAccess & GENERIC_READ
+    
+    # TODO: unused
+    perm_exec = dwDesiredAccess & GENERIC_EXECUTE
+
+    # only open file if it exists. error otherwise
+    open_existing = (
+        (dwCreationDisposition == OPEN_EXISTING) or
+        (dwCreationDisposition == TRUNCATE_EXISTING ) 
+        )
+     
+    # check if the file exists 
+    # TODO: race condition if file is deleted/reated  
+    file_exists = ql.os.fs_mapper.file_exists(s_lpFileName)
+
+    if (open_existing and (not file_exists)):
+        # the CreationDisposition wants a file to exist
+        # it does not 
+        ql.os.last_error = ERROR_FILE_NOT_FOUND
+        return INVALID_HANDLE_VALUE
+
+    if ((dwCreationDisposition == CREATE_NEW ) and file_exists):
+        # only create a file if it does not exist. 
+        # if it does, error
+        ql.os.last_error = ERROR_FILE_EXISTS
+
+    truncate  = (dwCreationDisposition == CREATE_ALWAYS) or  (dwCreationDisposition == TRUNCATE_EXISTING)
+
+    # TODO: this function does not handle general access masks. 
+    # see https://learn.microsoft.com/en-us/windows/win32/secauthz/access-mask
+    # it is only able to handle Generic R/W
+
+    # read only 
+    if (perm_read) and ( not (perm_write)):
         mode = "rb"
 
+    # Write only
+    elif ( perm_write and (not perm_read)):
+        # TODO: fopen modes do not allow for write only access
+        # Likely need to use os.open instead. 
+
+        if (truncate and (not open_existing)) or (truncate and open_existing and file_exists):
+            # create a new file or truncate an existing one
+            mode = "wb"
+        else:   
+            ql.log.warn("_CreateFile has been called with Write only access. This is not currently supported and the handle is still allows for read access!")
+            # read/write, do not create. do not truncatd
+            mode = "rb+"
+    
+    elif perm_read and perm_write:
+        # Note that this ignores exec access mask 
+        mode = "rb+"
+
+    elif perm_exec:
+        # TODO: handle exec access mask
+        # it is only executable or has a non standard access mask
+        ql.log.warn("_CreateFile has been called with executable only access or with a non standard access mask. This is not currently supported and the handle is set to Read/Write")
+        mode = "rb+"        
+    else:
+        # This is probably an invalid access mask
+        ql.log.warn(f"Invalid access mask provided: {dwDesiredAccess}")
+        # TODO: add error code 
+        return INVALID_HANDLE_VALUE
+
     try:
+        # we should have exited by now if the file doesn't exist
+        if (not file_exists) and (mode != "wb"):
+            status = ql.os.fs_mapper.create_empty_file(s_lpFileName)
+            if not status:
+                # could not create a new file
+                # bail out.
+                # TODO: set last_error
+                ql.log.warn(f"_CreateFile could not create new file {s_lpFileName}")
+                return INVALID_HANDLE_VALUE    
+
         f = ql.os.fs_mapper.open(s_lpFileName, mode)
+        if truncate and mode != "wb":
+            # redundant if mode is wb
+            f.truncate(0)
+
+        if dwCreationDisposition == CREATE_ALWAYS:
+                # we overwrote the file.
+                ql.os.last_error = ERROR_ALREADY_EXISTS
+                
+        if dwCreationDisposition == OPEN_ALWAYS:
+            ql.os.last_error = ERROR_ALREADY_EXISTS
+            
     except FileNotFoundError:
+        # Creation disposition determines what happens when the file doesn't exist
         ql.os.last_error = ERROR_FILE_NOT_FOUND
         return INVALID_HANDLE_VALUE
 
     new_handle = Handle(obj=f)
     ql.os.handle_manager.append(new_handle)
 
     return new_handle.id
```

### Comparing `qiling-1.4.5/qiling/os/windows/dlls/kernel32/handleapi.py` & `qiling-1.4.6/qiling/os/windows/dlls/kernel32/handleapi.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/os/windows/dlls/kernel32/heapapi.py` & `qiling-1.4.6/qiling/os/windows/dlls/kernel32/heapapi.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/os/windows/dlls/kernel32/interlockedapi.py` & `qiling-1.4.6/qiling/os/windows/dlls/kernel32/interlockedapi.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/os/windows/dlls/kernel32/ioapiset.py` & `qiling-1.4.6/qiling/os/windows/dlls/kernel32/ioapiset.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/os/windows/dlls/kernel32/libloaderapi.py` & `qiling-1.4.6/qiling/os/windows/dlls/kernel32/libloaderapi.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,18 +140,14 @@
     # if lpProcName is a short integer, it is an ordinal. otherwise, that is a function name.
     if lpProcName > MAXUSHORT:
         procname = ql.os.utils.read_cstring(lpProcName)
 
         # let log output reflect a human-readable procname
         params["lpProcName"] = procname
 
-        # WORKAROUND for gandcrab
-        if procname == "RtlComputeCrc32":
-            return 0
-
         procname = procname.encode('latin1')
 
     else:
         ordinal = lpProcName
 
     # get dll name by handle (module base)
     dll_name = next((os.path.basename(image.path).casefold() for image in ql.loader.images if image.base == hModule), None)
```

### Comparing `qiling-1.4.5/qiling/os/windows/dlls/kernel32/memoryapi.py` & `qiling-1.4.6/qiling/os/windows/dlls/kernel32/memoryapi.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/os/windows/dlls/kernel32/processenv.py` & `qiling-1.4.6/qiling/os/windows/dlls/kernel32/processenv.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/os/windows/dlls/kernel32/processthreadsapi.py` & `qiling-1.4.6/qiling/os/windows/dlls/kernel32/processthreadsapi.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 #   UINT uExitCode
 # );
 @winsdkapi(cc=STDCALL, params={
     'uExitCode' : UINT
 })
 def hook_ExitProcess(ql: Qiling, address: int, params):
     ql.emu_stop()
-    ql.os.PE_RUN = False
 
 def _GetStartupInfo(ql: Qiling, address: int, params, *, wide: bool):
     lpStartupInfo = params['lpStartupInfo']
     sui_struct = make_startup_info(ql.arch.bits)
 
     enc = 'utf-16le' if wide else 'latin1'
     desktop_title = f'QilingDesktop\x00'.encode(enc)
@@ -234,15 +233,14 @@
 })
 def hook_TerminateProcess(ql: Qiling, address: int, params):
     # Samples will try to kill other process! We don't want to always stop!
     process = params["hProcess"]
 
     if process == ql.os.profile.getint("KERNEL", "pid"):  # or process == ql.os.image_address:
         ql.emu_stop()
-        ql.os.PE_RUN = False
 
     return 1
 
 # HANDLE GetCurrentThread();
 @winsdkapi(cc=STDCALL, params={})
 def hook_GetCurrentThread(ql: Qiling, address: int, params):
     return ql.os.thread_manager.cur_thread.id
```

### Comparing `qiling-1.4.5/qiling/os/windows/dlls/kernel32/profileapi.py` & `qiling-1.4.6/qiling/os/windows/dlls/kernel32/profileapi.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/os/windows/dlls/kernel32/psapi.py` & `qiling-1.4.6/qiling/os/windows/dlls/kernel32/psapi.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/os/windows/dlls/kernel32/stringapiset.py` & `qiling-1.4.6/qiling/os/windows/dlls/kernel32/stringapiset.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/os/windows/dlls/kernel32/synchapi.py` & `qiling-1.4.6/qiling/os/windows/dlls/kernel32/synchapi.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/os/windows/dlls/kernel32/sysinfoapi.py` & `qiling-1.4.6/qiling/os/windows/dlls/kernel32/sysinfoapi.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/os/windows/dlls/kernel32/timezoneapi.py` & `qiling-1.4.6/qiling/os/windows/dlls/kernel32/timezoneapi.py`

 * *Files 25% similar despite different names*

```diff
@@ -8,12 +8,12 @@
 from qiling.os.windows.const import *
 from qiling.os.windows.fncc import *
 
 # DWORD GetTimeZoneInformation(
 #   [out] LPTIME_ZONE_INFORMATION lpTimeZoneInformation
 # );
 @winsdkapi(cc=STDCALL, params={
-	'lpTimeZoneInformation' : LPTIME_ZONE_INFORMATION
+    'lpTimeZoneInformation' : LPTIME_ZONE_INFORMATION
 })
 def hook_GetTimeZoneInformation(ql: Qiling, address: int, params):
     # TODO: implement this later. fail for now
-	return TIME_ZONE_ID_INVALID
+    return TIME_ZONE_ID_INVALID
```

### Comparing `qiling-1.4.5/qiling/os/windows/dlls/kernel32/tlhelp32.py` & `qiling-1.4.6/qiling/os/windows/dlls/kernel32/tlhelp32.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/os/windows/dlls/kernel32/winbase.py` & `qiling-1.4.6/qiling/os/windows/dlls/kernel32/winbase.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,15 +154,14 @@
 #   int ExitCode
 # );
 @winsdkapi(cc=STDCALL, params={
     'ExitCode' : INT
 })
 def hook_FatalExit(ql: Qiling, address: int, params):
     ql.emu_stop()
-    ql.os.PE_RUN = False
 
 # PVOID EncodePointer(
 #  _In_ PVOID Ptr
 # );
 @winsdkapi(cc=STDCALL, params={
     'Ptr' : PVOID
 })
```

### Comparing `qiling-1.4.5/qiling/os/windows/dlls/kernel32/winnls.py` & `qiling-1.4.6/qiling/os/windows/dlls/kernel32/winnls.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/os/windows/dlls/kernel32/winnt.py` & `qiling-1.4.6/qiling/os/windows/dlls/kernel32/winnt.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/os/windows/dlls/kernel32/wow64apiset.py` & `qiling-1.4.6/qiling/os/windows/dlls/kernel32/wow64apiset.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/os/windows/dlls/msi.py` & `qiling-1.4.6/qiling/os/windows/dlls/msi.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/os/windows/dlls/msvcrt.py` & `qiling-1.4.6/qiling/os/windows/dlls/msvcrt.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #!/usr/bin/env python3
-# 
+#
 # Cross Platform and Multi Architecture Advanced Binary Emulation Framework
 #
 
 import time
 from typing import Sequence
 
 from qiling import Qiling
@@ -189,15 +189,14 @@
 #    int const status
 # );
 @winsdkapi(cc=CDECL, params={
     'status' : INT
 })
 def hook_exit(ql: Qiling, address: int, params):
     ql.emu_stop()
-    ql.os.PE_RUN = False
 
 # int __cdecl _initterm_e(
 #    PVFV *,
 #    PVFV *
 # );
 @winsdkapi(cc=CDECL, params={
     'pfbegin' : POINTER,
```

### Comparing `qiling-1.4.5/qiling/os/windows/dlls/ntdll.py` & `qiling-1.4.6/qiling/os/windows/dlls/ntdll.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #!/usr/bin/env python3
-# 
+#
 # Cross Platform and Multi Architecture Advanced Binary Emulation Framework
 #
 
 import os
 
 from qiling import Qiling
 from qiling.os.windows.api import *
@@ -11,14 +11,16 @@
 
 from qiling.const import QL_ARCH
 from qiling.exception import *
 from qiling.os.const import *
 from qiling.os.windows.const import *
 from qiling.os.windows.handle import *
 from qiling.os.windows import structs
+from qiling.os.windows import utils
+
 
 # void *memcpy(
 #    void *dest,
 #    const void *src,
 #    size_t count
 # );
 @winsdkapi(cc=CDECL, params={
@@ -64,15 +66,15 @@
             InheritedFromUniqueProcessId=kconf.getint('parent_pid')
         )
 
         res_data = bytes(pci_obj)
 
     else:
         # TODO: support more info class ("flag") values
-        ql.log.info(f'SetInformationProcess: no implementation for info class {flag:#04x}')
+        ql.log.info(f'QueryInformationProcess: no implementation for info class {flag:#04x}')
 
         return STATUS_UNSUCCESSFUL
 
     res_size = len(res_data)
 
     if obuf_len >= res_size:
         ql.mem.write(obuf_ptr, res_data)
@@ -314,58 +316,62 @@
 })
 def hook_NtSetInformationProcess(ql: Qiling, address: int, params):
     _SetInformationProcess(ql, address, params)
 
 def _SetInformationProcess(ql: Qiling, address: int, params):
     process = params["ProcessHandle"]
     flag = params["ProcessInformationClass"]
-    dst = params["ProcessInformation"]
-    dst_size = params["ProcessInformationLength"]
+    ibuf_ptr = params["ProcessInformation"]
+    ibuf_len = params["ProcessInformationLength"]
 
     if flag == ProcessDebugFlags:
-        value = b"\x01" * 0x4
+        flag_name = 'ProcessDebugFlags'
+        comment = ''
+        read_len = 4
 
     elif flag == ProcessDebugPort:
-        value = b"\x00" * 0x4
+        flag_name = 'ProcessDebugPort'
+        comment = ''
+        read_len = 4
 
     elif flag == ProcessDebugObjectHandle:
         return STATUS_PORT_NOT_SET
 
     elif flag == ProcessBreakOnTermination:
-            ql.log.debug("The target may be attempting modify a the 'critical' flag of the process")  
+        flag_name = 'ProcessBreakOnTermination'
+        comment = 'the critical flag of the process'
+        read_len = 1    # FIXME: is it really a single-byte data?
 
     elif flag == ProcessExecuteFlags:
-        ql.log.debug("The target may be attempting to modify DEP for the process")
-
-        if dst:
-            ql.mem.write_ptr(dst, 0, 1)
+        flag_name = 'ProcessExecuteFlags'
+        comment = 'DEP for the process'
+        read_len = 1
 
     elif flag == ProcessBasicInformation:
-        kconf = ql.os.profile['KERNEL']
-        pbi_struct = structs.make_process_basic_info(ql.arch.bits)
+        flag_name = 'ProcessBasicInformation'
+        comment = 'PEB debug flag for the process'
 
-        pci_obj = pbi_struct(
-            ExitStatus=0,
-            PebBaseAddress=ql.loader.TEB.PebAddress,
-            AffinityMask=0,
-            BasePriority=0,
-            UniqueProcessId=kconf.getint('pid'),
-            InheritedFromUniqueProcessId=kconf.getint('parent_pid')
-        )
-
-        ql.log.debug("The target may be attempting to modify the PEB debug flag")
-        value = bytes(pbi_obj)
+        pbi_struct = structs.make_process_basic_info(ql.arch.bits)
+        read_len = pbi_struct.sizeof()
 
     else:
         # TODO: support more info class ("flag") values
         ql.log.info(f'SetInformationProcess: no implementation for info class {flag:#04x}')
 
         return STATUS_UNSUCCESSFUL
 
-    # TODO: value is never used after assignment
+    if ibuf_len >= read_len:
+        data = (ql.mem.read_ptr if read_len in (1, 2, 4, 8) else ql.mem.read)(ibuf_ptr, read_len)
+
+        ql.log.debug(f'SetInformationProcess: {flag_name} was set to {data}')
+
+        if comment:
+            ql.log.debug(f'The target may be attempting modify {comment}')
+
+        # NOTE: we don't actually change anything
 
     return STATUS_SUCCESS
 
 # NTSYSAPI
 # NTSTATUS
 # NTAPI
 # NtYieldExecution(
@@ -393,24 +399,29 @@
     FunctionAddress = params['FunctionAddress']
 
     # Check if dll is loaded
     dll_name = next((os.path.basename(path).casefold() for base, _, path in ql.loader.images if base == ModuleHandle), None)
 
     if dll_name is None:
         ql.log.debug(f'Could not find specified handle {ModuleHandle} in loaded DLL')
-        return 0
+        return STATUS_DLL_NOT_FOUND
 
-    identifier = bytes(FunctionName, 'ascii') if FunctionName else Ordinal
+    identifier = utils.read_pansi_string(ql, FunctionName) if FunctionName else Ordinal
     iat = ql.loader.import_address_table[dll_name]
 
-    if identifier in iat:
-        ql.mem.write_ptr(FunctionAddress, iat[identifier])
-        return 0
+    if not identifier:
+        return STATUS_INVALID_PARAMETER
+
+    if identifier not in iat:
+        return STATUS_PROCEDURE_NOT_FOUND
+
+    ql.mem.write_ptr(FunctionAddress, iat[identifier])
+
+    return STATUS_SUCCESS
 
-    return 0xFFFFFFFF
 
 # NTSYSAPI PVOID RtlAllocateHeap(
 #  PVOID  HeapHandle,
 #  ULONG  Flags,
 #  SIZE_T Size
 # );
 @winsdkapi(cc=STDCALL, params={
```

### Comparing `qiling-1.4.5/qiling/os/windows/dlls/ntoskrnl.py` & `qiling-1.4.6/qiling/os/windows/dlls/ntoskrnl.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,17 +7,19 @@
 
 from qiling import Qiling
 from qiling.exception import QlErrorNotImplemented
 from qiling.os.windows.api import *
 from qiling.os.windows.const import *
 from qiling.os.windows.fncc import *
 from qiling.os.windows.structs import *
+from qiling.os.windows import utils
 from qiling.os.windows.wdk_const import DO_DEVICE_INITIALIZING, DO_EXCLUSIVE
 from qiling.utils import verify_ret
 
+
 # NTSYSAPI NTSTATUS RtlGetVersion(
 #   PRTL_OSVERSIONINFOW lpVersionInformation
 # );
 @winsdkapi(cc=CDECL, params={
     'lpVersionInformation' : PRTL_OSVERSIONINFOW
 })
 def hook_RtlGetVersion(ql: Qiling, address: int, params):
@@ -427,48 +429,54 @@
     'Tag' : ULONG
 })
 def hook_ExFreePoolWithTag(ql: Qiling, address: int, params):
     addr = params['P']
 
     ql.os.heap.free(addr)
 
-hook_only_routine_address = [b'IoCreateDeviceSecure']
+
+hook_only_routine_address = ['IoCreateDeviceSecure']
+
 
 # PVOID MmGetSystemRoutineAddress(
 #  PUNICODE_STRING SystemRoutineName
 # );
 @winsdkapi(cc=STDCALL, params={
     'SystemRoutineName' : PUNICODE_STRING
 })
 def hook_MmGetSystemRoutineAddress(ql: Qiling, address: int, params):
-    SystemRoutineName = bytes(params["SystemRoutineName"], 'ascii')
+    SystemRoutineName = params["SystemRoutineName"]
+
+    routine_name = SystemRoutineName and utils.read_punicode_string(ql, SystemRoutineName)
 
-    # check function name in import table
-    for dll_name in ('ntoskrnl.exe', 'ntkrnlpa.exe', 'hal.dll'):
-        if dll_name in ql.loader.import_address_table:
-            if SystemRoutineName in ql.loader.import_address_table[dll_name]:
-                return ql.loader.import_address_table[dll_name][SystemRoutineName]
-
-    # function not found!
-    # we check function name in `hook_only_routine_address`.
-    if SystemRoutineName in hook_only_routine_address:
-        index = hook_only_routine_address.index(SystemRoutineName)
-        # found!
+    if routine_name:
+        # check function name in import table
         for dll_name in ('ntoskrnl.exe', 'ntkrnlpa.exe', 'hal.dll'):
-            image = ql.loader.get_image_by_name(dll_name)
+            if dll_name in ql.loader.import_address_table:
+                if routine_name in ql.loader.import_address_table[dll_name]:
+                    return ql.loader.import_address_table[dll_name][routine_name]
+
+        # function not found!
+        # we check function name in `hook_only_routine_address`.
+        if routine_name in hook_only_routine_address:
+            index = hook_only_routine_address.index(routine_name)
+            # found!
+            for dll_name in ('ntoskrnl.exe', 'ntkrnlpa.exe', 'hal.dll'):
+                image = ql.loader.get_image_by_name(dll_name)
+
+                if image:
+                    # create fake address
+                    new_function_address = image.base + index + 1
+                    # update import address table
+                    ql.loader.import_symbols[new_function_address] = {
+                        'name': SystemRoutineName.encode(),
+                        'ordinal': -1
+                    }
+                    return new_function_address
 
-            if image:
-                # create fake address
-                new_function_address = image.base + index + 1
-                # update import address table
-                ql.loader.import_symbols[new_function_address] = {
-                    'name': SystemRoutineName,
-                    'ordinal': -1
-                }
-                return new_function_address
     return 0
 
 # int _wcsnicmp(
 #    const wchar_t *string1,
 #    const wchar_t *string2,
 #    size_t count
 # );
```

### Comparing `qiling-1.4.5/qiling/os/windows/dlls/ole32.py` & `qiling-1.4.6/qiling/os/windows/dlls/ole32.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/os/windows/dlls/oleaut32.py` & `qiling-1.4.6/qiling/os/windows/dlls/oleaut32.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/os/windows/dlls/shell32.py` & `qiling-1.4.6/qiling/os/windows/dlls/shell32.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/os/windows/dlls/shlwapi.py` & `qiling-1.4.6/qiling/os/windows/dlls/shlwapi.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/os/windows/dlls/user32.py` & `qiling-1.4.6/qiling/os/windows/dlls/user32.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,18 +92,18 @@
     'lpDialogFunc'   : DLGPROC,
     'dwInitParam'    : LPARAM
 })
 def hook_DialogBoxParamA(ql: Qiling, address: int, params):
     return 0
 
 # UINT GetDlgItemTextA(
-# 	HWND  hDlg,
-# 	int   nIDDlgItem,
-# 	LPSTR lpString,
-# 	int   cchMax
+#     HWND  hDlg,
+#     int   nIDDlgItem,
+#     LPSTR lpString,
+#     int   cchMax
 # );
 @winsdkapi(cc=STDCALL, params={
     'hDlg'       : HWND,
     'nIDDlgItem' : INT,
     'lpString'   : LPSTR,
     'cchMax'     : INT
 })
```

### Comparing `qiling-1.4.5/qiling/os/windows/dlls/wininet.py` & `qiling-1.4.6/qiling/os/windows/dlls/wininet.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/os/windows/dlls/wsock32.py` & `qiling-1.4.6/qiling/os/windows/dlls/wsock32.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/os/windows/dlls/wudplatform.py` & `qiling-1.4.6/qiling/os/windows/dlls/wudplatform.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/os/windows/fiber.py` & `qiling-1.4.6/qiling/os/windows/fiber.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/os/windows/fncc.py` & `qiling-1.4.6/qiling/os/windows/fncc.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/os/windows/handle.py` & `qiling-1.4.6/qiling/os/windows/handle.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/os/windows/registry.py` & `qiling-1.4.6/qiling/os/windows/registry.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/os/windows/structs.py` & `qiling-1.4.6/qiling/os/windows/structs.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,15 +112,15 @@
 
     # make sure mismatches in peb size are not overlooked
     assert PEB.sizeof() == expected_size
 
     return PEB
 
 
-# https://docs.microsoft.com/en-us/windows/win32/api/subauth/ns-subauth-unicode_string
+# https://learn.microsoft.com/en-us/windows/win32/api/ntdef/ns-ntdef-_unicode_string
 @lru_cache(maxsize=2)
 def make_unicode_string(archbits: int):
     """Generate a UNICODE_STRING structure class.
     """
 
     native_type = struct.get_native_type(archbits)
     Struct = struct.get_aligned_struct(archbits)
@@ -131,14 +131,18 @@
             ('MaximumLength', ctypes.c_uint16),
             ('Buffer',        native_type)
         )
 
     return UNICODE_STRING
 
 
+# https://learn.microsoft.com/en-us/windows/win32/api/ntdef/ns-ntdef-string
+make_ansi_string = make_unicode_string
+
+
 # https://docs.microsoft.com/en-us/windows-hardware/drivers/ddi/wdm/ns-wdm-_driver_object
 def make_driver_object(archbits: int):
     """Generate a DRIVER_OBJECT structure class.
     """
 
     native_type = struct.get_native_type(archbits)
     Struct = struct.get_aligned_struct(archbits)
@@ -979,15 +983,15 @@
             ('MappingInfoIndexNode', RTL_BALANCED_NODE),
             ('OriginalBase', native_type),
             ('LoadTime', LARGE_INTEGER),
             ('BaseNameHashValue', native_type),
             ('LoadReason', ctypes.c_uint32),
             ('ImplicitPathOptions', native_type),
             ('ReferenceCount', native_type),
-        	# 1607+
+            # 1607+
             ('DependentLoadFlags', native_type),
             # 1703+
             ('SigningLevel', ctypes.c_uint8)
         )
 
     return LdrDataTableEntry
```

### Comparing `qiling-1.4.5/qiling/os/windows/thread.py` & `qiling-1.4.6/qiling/os/windows/thread.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/os/windows/utils.py` & `qiling-1.4.6/qiling/os/windows/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 #!/usr/bin/env python3
 #
 # Cross Platform and Multi Architecture Advanced Binary Emulation Framework
 #
 
-from typing import Iterable, Tuple, TypeVar
+from typing import Iterable, Optional, Tuple, TypeVar
 
 from unicorn import UcError
 
 from qiling import Qiling
 from qiling.exception import QlErrorSyscallError
 from qiling.os.const import POINTER
 from qiling.os.windows.fncc import STDCALL
 from qiling.os.windows.wdk_const import *
 from qiling.os.windows.structs import *
 from qiling.utils import verify_ret
 
 Comparable = TypeVar('Comparable', str, int)
 
+
 # an alternative to Python2 cmp builtin which no longer exists in Python3
 def cmp(a: Comparable, b: Comparable) -> int:
     return (a > b) - (a < b)
 
 
 def has_lib_ext(name: str) -> bool:
     ext = name.lower().rpartition('.')[-1]
@@ -106,28 +107,29 @@
         (POINTER, ql.loader.driver_object.DeviceObject),
         (POINTER, irp_addr)
     ))
 
     ql.log.info(f'Executing from {major_func:#x}')
 
     try:
-        # now emulate 
+        # now emulate
         ql.run(major_func)
     except UcError as err:
         verify_ret(ql, err)
 
     # read updated IRP state before releasing resources
     with irp_struct.ref(ql.mem, irp_addr) as irp_obj:
         info = irp_obj.IoStatus.Information
 
     # free all allocated memory
     __free_all(allocations)
 
     return info
 
+
 # Emulate DeviceIoControl() of Windows
 # BOOL DeviceIoControl(
 #      HANDLE       hDevice,
 #      DWORD        dwIoControlCode,
 #      LPVOID       lpInBuffer,
 #      DWORD        nInBufferSize,
 #      LPVOID       lpOutBuffer,
@@ -260,7 +262,35 @@
         elif ctl_method == METHOD_NEITHER:
             output_data = ql.mem.read(output_buffer_addr, info)
 
     # now free all alloc memory
     __free_all(allocations)
 
     return status, info, output_data
+
+
+def read_pansi_string(ql: Qiling, ptr: int) -> Optional[str]:
+    """Read and decode the string referenced by a PANSI_STRING structure. It is
+    the caller responsibility to make sure the pointer to the structure is accesible.
+    """
+
+    astr_obj = make_ansi_string(ql.arch.bits).load_from(ql.mem, ptr)
+
+    if astr_obj.Buffer and astr_obj.Length:
+        return ql.os.utils.read_cstring(astr_obj.Buffer, maxlen=astr_obj.Length)
+
+    return None
+
+
+def read_punicode_string(ql: Qiling, ptr: int) -> Optional[str]:
+    """Read and decode the string referenced by a PUNICODE_STRING structure. It is
+    the caller responsibility to make sure the pointer to the structure is accesible.
+    """
+
+    ucstr_obj = make_unicode_string(ql.arch.bits).load_from(ql.mem, ptr)
+
+    if ucstr_obj.Buffer and ucstr_obj.Length:
+        assert ucstr_obj.Length % 2 == 0, f'wide string size is expected to be a multiplication of 2. got: {ucstr_obj.Length}'
+
+        return ql.os.utils.read_wstring(ucstr_obj.Buffer, maxlen=ucstr_obj.Length // 2)
+
+    return None
```

### Comparing `qiling-1.4.5/qiling/os/windows/wdk_const.py` & `qiling-1.4.6/qiling/os/windows/wdk_const.py`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/os/windows/windows.py` & `qiling-1.4.6/qiling/os/windows/windows.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 from . import thread
 from . import clipboard
 from . import fiber
 from . import registry
 
 import qiling.os.windows.dlls as api
 
+
 class QlOsWindows(QlOs):
     type = QL_OS.WINDOWS
 
     def __init__(self, ql: Qiling):
         super().__init__(ql)
 
         self.ql = ql
@@ -76,30 +77,28 @@
         username = self.profile.get('USER', 'username')
 
         self.windir = ntpath.join(sysdrv, windir)
         self.winsys = ntpath.join(sysdrv, windir, 'System32')
         self.userprofile = ntpath.join(sysdrv, 'Users', username)
         self.username = username
 
-        self.PE_RUN = False
         self.last_error = 0
 
         self.argv = self.ql.argv
         self.env = self.ql.env
         self.pid = self.profile.getint('KERNEL', 'pid')
 
         self.services = {}
         self.load()
 
         # only after handle manager has been set up we can assign the standard streams
         self.stdin  = self._stdin
         self.stdout = self._stdout
         self.stderr = self._stderr
 
-
     @QlOs.stdin.setter
     def stdin(self, stream: TextIO) -> None:
         self._stdin = stream
 
         handle = self.handle_manager.get(const.STD_INPUT_HANDLE)
         assert handle is not None
 
@@ -119,29 +118,27 @@
         self._stderr = stream
 
         handle = self.handle_manager.get(const.STD_ERROR_HANDLE)
         assert handle is not None
 
         handle.obj = stream
 
-
     def load(self):
-        self.setupGDT()
+        self.__setup_gdt()
         self.__setup_components()
 
         # hook win api
         self.ql.hook_code(self.hook_winapi)
 
-
-    def setupGDT(self):
+    def __setup_gdt(self):
         gdtm = GDTManager(self.ql)
 
         segm_class: Type[SegmentManager] = {
-            32 : SegmentManager86,
-            64 : SegmentManager64
+            32: SegmentManager86,
+            64: SegmentManager64
         }[self.ql.arch.bits]
 
         # setup gdt and segments selectors
         segm = segm_class(self.ql.arch, gdtm)
         segm.setup_cs_ds_ss_es(0, 4 << 30)
         segm.setup_fs(FS_SEGMENT_ADDR, FS_SEGMENT_SIZE)
         segm.setup_gs(GS_SEGMENT_ADDR, GS_SEGMENT_SIZE)
@@ -152,15 +149,14 @@
         self.ql.mem.map(FS_SEGMENT_ADDR, FS_SEGMENT_SIZE, info='[FS]')
 
         if not self.ql.mem.is_available(GS_SEGMENT_ADDR, GS_SEGMENT_SIZE):
             raise QlMemoryMappedError('cannot map GS segment, memory location is taken')
 
         self.ql.mem.map(GS_SEGMENT_ADDR, GS_SEGMENT_SIZE, info='[GS]')
 
-
     def __setup_components(self):
         reghive = self.path.transform_to_real_path(ntpath.join(self.windir, 'registry'))
 
         self.handle_manager = handle.HandleManager()
         self.registry_manager = registry.RegistryManager(self.ql, reghive)
         self.clipboard = clipboard.Clipboard(self)
         self.fiber_manager = fiber.FiberManager(self.ql)
@@ -198,27 +194,24 @@
                     raise QlErrorSyscallError("Windows API Implementation Error")
             else:
                 ql.log.warning(f'api {api_name} ({entry["dll"]}) is not implemented')
 
                 if ql.debug_stop:
                     raise QlErrorSyscallNotFound("Windows API implementation not found")
 
-
     def run(self):
         if self.ql.exit_point is not None:
             self.exit_point = self.ql.exit_point
 
-        if  self.ql.entry_point is not None:
+        if self.ql.entry_point is not None:
             self.ql.loader.entry_point = self.ql.entry_point
 
         entry_point = self.ql.loader.entry_point
         exit_point = (self.ql.loader.entry_point + len(self.ql.code)) if self.ql.code else self.exit_point
 
-        self.PE_RUN = True
-
         try:
             self.ql.emu_start(entry_point, exit_point, self.ql.timeout, self.ql.count)
         except UcError:
             self.emu_error()
             raise
 
         self.registry_manager.save()
```

### Comparing `qiling-1.4.5/qiling/profiles/linux.ql` & `qiling-1.4.6/qiling/profiles/linux.ql`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/profiles/macos.ql` & `qiling-1.4.6/qiling/profiles/macos.ql`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/profiles/qnx.ql` & `qiling-1.4.6/qiling/profiles/qnx.ql`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/profiles/uefi.ql` & `qiling-1.4.6/qiling/profiles/uefi.ql`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/profiles/windows.ql` & `qiling-1.4.6/qiling/profiles/windows.ql`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qiling/utils.py` & `qiling-1.4.6/qiling/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 #!/usr/bin/env python3
-# 
+#
 # Cross Platform and Multi Architecture Advanced Binary Emulation Framework
 #
 
 """
 This module is intended for general purpose functions that can be used
 thoughout the qiling framework
 """
 
-from functools import partial
-from pathlib import Path
-import importlib, inspect, os
+import importlib
+import inspect
+import os
 
+from functools import partial
 from configparser import ConfigParser
+from pathlib import Path
 from types import ModuleType
 from typing import TYPE_CHECKING, Any, Callable, Mapping, Optional, Tuple, TypeVar, Union
 
 from unicorn import UC_ERR_READ_UNMAPPED, UC_ERR_FETCH_UNMAPPED
 
 from qiling.exception import *
 from qiling.const import QL_ARCH, QL_ENDIAN, QL_OS, QL_DEBUGGER
@@ -34,76 +36,84 @@
 
 
 def __name_to_enum(name: str, mapping: Mapping[str, T], aliases: Mapping[str, str] = {}) -> Optional[T]:
     key = name.casefold()
 
     return mapping.get(aliases.get(key) or key)
 
+
 def os_convert(os: str) -> Optional[QL_OS]:
     alias_map = {
-        'darwin' : 'macos'
+        'darwin': 'macos'
     }
 
     return __name_to_enum(os, os_map, alias_map)
 
+
 def arch_convert(arch: str) -> Optional[QL_ARCH]:
     alias_map = {
-        'x86_64'  : 'x8664',
-        'riscv32' : 'riscv'
+        'x86_64':  'x8664',
+        'riscv32': 'riscv'
     }
 
     return __name_to_enum(arch, arch_map, alias_map)
 
+
 def debugger_convert(debugger: str) -> Optional[QL_DEBUGGER]:
     return __name_to_enum(debugger, debugger_map)
 
+
 def arch_os_convert(arch: QL_ARCH) -> Optional[QL_OS]:
     return arch_os_map.get(arch)
 
+
 def ql_get_module(module_name: str) -> ModuleType:
     try:
         module = importlib.import_module(module_name, 'qiling')
     except (ModuleNotFoundError, KeyError):
         raise QlErrorModuleNotFound(f'Unable to import module {module_name}')
 
     return module
 
+
 def ql_get_module_function(module_name: str, member_name: str):
     module = ql_get_module(module_name)
 
     try:
         member = getattr(module, member_name)
     except AttributeError:
         raise QlErrorModuleFunctionNotFound(f'Unable to import {member_name} from {module_name}')
 
     return member
 
+
 def __emu_env_from_pathname(path: str) -> Tuple[Optional[QL_ARCH], Optional[QL_OS], Optional[QL_ENDIAN]]:
     if os.path.isdir(path) and path.endswith('.kext'):
         return QL_ARCH.X8664, QL_OS.MACOS, QL_ENDIAN.EL
 
     if os.path.isfile(path):
         _, ext = os.path.splitext(path)
 
         if ext in ('.DOS_COM', '.DOS_MBR', '.DOS_EXE'):
             return QL_ARCH.A8086, QL_OS.DOS, QL_ENDIAN.EL
 
     return None, None, None
 
+
 def __emu_env_from_elf(path: str) -> Tuple[Optional[QL_ARCH], Optional[QL_OS], Optional[QL_ENDIAN]]:
     # instead of using full-blown elffile parsing, we perform a simple parsing to avoid
     # external dependencies for target systems that do not need them.
     #
     # see: https://refspecs.linuxfoundation.org/elf/gabi4+/ch4.eheader.html
 
     # ei_class
     ELFCLASS32 = 1    # 32-bit
     ELFCLASS64 = 2    # 64-bit
 
-    #ei_data
+    # ei_data
     ELFDATA2LSB = 1   # little-endian
     ELFDATA2MSB = 2   # big-endian
 
     # ei_osabi
     ELFOSABI_SYSV       = 0
     ELFOSABI_LINUX      = 3
     ELFOSABI_FREEBSD    = 9
@@ -117,16 +127,16 @@
     EM_ARM     = 40
     EM_X86_64  = 62
     EM_AARCH64 = 183
     EM_RISCV   = 243
     EM_PPC     = 20
 
     endianess = {
-        ELFDATA2LSB : (QL_ENDIAN.EL, 'little'),
-        ELFDATA2MSB : (QL_ENDIAN.EB, 'big')
+        ELFDATA2LSB: (QL_ENDIAN.EL, 'little'),
+        ELFDATA2MSB: (QL_ENDIAN.EB, 'big')
     }
 
     machines32 = {
         EM_386   : QL_ARCH.X86,
         EM_MIPS  : QL_ARCH.MIPS,
         EM_ARM   : QL_ARCH.ARM,
         EM_RISCV : QL_ARCH.RISCV,
@@ -136,16 +146,16 @@
     machines64 = {
         EM_X86_64  : QL_ARCH.X8664,
         EM_AARCH64 : QL_ARCH.ARM64,
         EM_RISCV   : QL_ARCH.RISCV64
     }
 
     classes = {
-        ELFCLASS32 : machines32,
-        ELFCLASS64 : machines64
+        ELFCLASS32: machines32,
+        ELFCLASS64: machines64
     }
 
     abis = {
         ELFOSABI_SYSV       : QL_OS.LINUX,
         ELFOSABI_LINUX      : QL_OS.LINUX,
         ELFOSABI_FREEBSD    : QL_OS.FREEBSD,
         ELFOSABI_ARM_AEABI  : QL_OS.LINUX,
@@ -188,14 +198,15 @@
                     ostype = abis[ei_osabi]
 
                     if blob and b'ldqnx.so' in blob:
                         ostype = QL_OS.QNX
 
     return archtype, ostype, archendian
 
+
 def __emu_env_from_macho(path: str) -> Tuple[Optional[QL_ARCH], Optional[QL_OS], Optional[QL_ENDIAN]]:
     macho_macos_sig64 = b'\xcf\xfa\xed\xfe'
     macho_macos_sig32 = b'\xce\xfa\xed\xfe'
     macho_macos_fat = b'\xca\xfe\xba\xbe'  # should be header for FAT
 
     arch = None
     ostype = None
@@ -216,14 +227,15 @@
 
         elif ident[4] == 0x0c and ident[7] == 0x01:  # ARM64
             endian = QL_ENDIAN.EL
             arch = QL_ARCH.ARM64
 
     return arch, ostype, endian
 
+
 def __emu_env_from_pe(path: str) -> Tuple[Optional[QL_ARCH], Optional[QL_OS], Optional[QL_ENDIAN]]:
     import pefile
 
     try:
         pe = pefile.PE(path, fast_load=True)
     except:
         return None, None, None
@@ -256,14 +268,15 @@
         else:
             ostype = QL_OS.WINDOWS
 
         archendian = QL_ENDIAN.EL
 
     return arch, ostype, archendian
 
+
 def ql_guess_emu_env(path: str) -> Tuple[Optional[QL_ARCH], Optional[QL_OS], Optional[QL_ENDIAN]]:
     guessing_methods = (
         __emu_env_from_pathname,
         __emu_env_from_elf,
         __emu_env_from_macho,
         __emu_env_from_pe
     )
@@ -274,17 +287,18 @@
         if None not in (arch, ostype, endian):
             break
     else:
         arch, ostype, endian = (None, ) * 3
 
     return arch, ostype, endian
 
+
 def select_loader(ostype: QL_OS, libcache: bool) -> QlClassInit['QlLoader']:
-    if ostype == QL_OS.WINDOWS:
-        kwargs = {'libcache' : libcache}
+    if ostype is QL_OS.WINDOWS:
+        kwargs = {'libcache': libcache}
 
     else:
         kwargs = {}
 
     module = {
         QL_OS.LINUX   : r'elf',
         QL_OS.FREEBSD : r'elf',
@@ -301,22 +315,24 @@
     qlloader_path = f'.loader.{module}'
     qlloader_class = f'QlLoader{module.upper()}'
 
     obj = ql_get_module_function(qlloader_path, qlloader_class)
 
     return partial(obj, **kwargs)
 
+
 def select_component(component_type: str, component_name: str, **kwargs) -> QlClassInit[Any]:
     component_path = f'.{component_type}.{component_name}'
     component_class = f'Ql{component_name.capitalize()}Manager'
 
     obj = ql_get_module_function(component_path, component_class)
 
     return partial(obj, **kwargs)
 
+
 def select_debugger(options: Union[str, bool]) -> Optional[QlClassInit['QlDebugger']]:
     if options is True:
         options = 'gdb'
 
     if type(options) is str:
         objname, *args = options.split(':')
         dbgtype = debugger_convert(objname)
@@ -349,22 +365,23 @@
 
         obj = ql_get_module_function(f'.debugger.{objname}.{objname}', f'Ql{str.capitalize(objname)}')
 
         return partial(obj, **kwargs)
 
     return None
 
+
 def select_arch(archtype: QL_ARCH, endian: QL_ENDIAN, thumb: bool) -> QlClassInit['QlArch']:
     # set endianess and thumb mode for arm-based archs
-    if archtype == QL_ARCH.ARM:
-        kwargs = {'endian' : endian, 'thumb' : thumb}
+    if archtype is QL_ARCH.ARM:
+        kwargs = {'endian': endian, 'thumb': thumb}
 
     # set endianess for mips arch
-    elif archtype == QL_ARCH.MIPS:
-        kwargs = {'endian' : endian}
+    elif archtype is QL_ARCH.MIPS:
+        kwargs = {'endian': endian}
 
     else:
         kwargs = {}
 
     module = {
         QL_ARCH.A8086    : r'x86',
         QL_ARCH.X86      : r'x86',
@@ -382,31 +399,33 @@
     qlarch_path = f'.arch.{module}'
     qlarch_class = f'QlArch{archtype.name.upper()}'
 
     obj = ql_get_module_function(qlarch_path, qlarch_class)
 
     return partial(obj, **kwargs)
 
+
 def select_os(ostype: QL_OS) -> QlClassInit['QlOs']:
     qlos_name = ostype.name
     qlos_path = f'.os.{qlos_name.lower()}.{qlos_name.lower()}'
     qlos_class = f'QlOs{qlos_name.capitalize()}'
 
     obj = ql_get_module_function(qlos_path, qlos_class)
 
     return partial(obj)
 
+
 def profile_setup(ostype: QL_OS, user_config: Optional[Union[str, dict]]):
     # mcu uses a yaml-based config
-    if ostype == QL_OS.MCU:
+    if ostype is QL_OS.MCU:
         import yaml
 
         if user_config:
             with open(user_config) as f:
-                config = yaml.load(f, Loader=yaml.Loader)
+                config = yaml.load(f, Loader=yaml.SafeLoader)
         else:
             config = {}
 
     else:
         # patch 'getint' to convert integers of all bases
         int_converter = partial(int, base=0)
         config = ConfigParser(converters={'int': int_converter})
@@ -419,17 +438,18 @@
 
         # user-specified profile adds or overrides existing setting
         if isinstance(user_config, dict):
             config.read_dict(user_config)
 
         elif user_config:
             config.read(user_config)
-        
+
     return config
 
+
 # verify if emulator returns properly
 def verify_ret(ql: 'Qiling', err):
     # init_sp location is not consistent; this is here to work around that
     if not hasattr(ql.os, 'init_sp'):
         ql.os.init_sp = ql.loader.init_sp
 
     ql.log.debug("Got exception %u: init SP = %x, current SP = %x, PC = %x" %(err.errno, ql.os.init_sp, ql.arch.regs.arch_sp, ql.arch.regs.arch_pc))
@@ -445,28 +465,29 @@
                 if ql.os.init_sp == ql.arch.regs.arch_sp - 8:
                     pass
                 else:
                     raise
 
         if ql.arch.type == QL_ARCH.X8664: # Win64
             if ql.os.init_sp == ql.arch.regs.arch_sp or ql.os.init_sp + 8 == ql.arch.regs.arch_sp or ql.os.init_sp + 0x10 == ql.arch.regs.arch_sp:  # FIXME
-                # 0x11626	 c3	  	ret
+                # 0x11626     c3          ret
                 # print("OK, stack balanced!")
                 pass
             else:
                 raise
         else:   # Win32
             if ql.os.init_sp + 12 == ql.arch.regs.arch_sp:   # 12 = 8 + 4
-                # 0x114dd	 c2 08 00	  	ret 	8
+                # 0x114dd     c2 08 00          ret     8
                 pass
             else:
                 raise
     else:
         raise
 
+
 __all__ = [
     'os_convert',
     'arch_convert',
     'debugger_convert',
     'arch_os_convert',
     'ql_get_module',
     'ql_get_module_function',
```

### Comparing `qiling-1.4.5/qiling.egg-info/PKG-INFO` & `qiling-1.4.6/qiling.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qiling
-Version: 1.4.5
+Version: 1.4.6
 Summary: Qiling is an advanced binary emulation framework that cross-platform-architecture
 Home-page: http://qiling.io
 Maintainer: KaiJern Lau (xwings)
 Maintainer-email: info@qiling.io
 License: GPLv2
 Keywords: qiling binary emulator framework malware analysis UEFI IoT
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `qiling-1.4.5/qiling.egg-info/SOURCES.txt` & `qiling-1.4.6/qiling.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 COPYING
 README.md
 qltool
+qltui.py
 setup.py
 qiling/__init__.py
 qiling/const.py
 qiling/core.py
 qiling/core_hooks.py
 qiling/core_hooks_types.py
 qiling/core_struct.py
@@ -268,14 +269,15 @@
 qiling/extensions/afl/afl.py
 qiling/extensions/coverage/__init__.py
 qiling/extensions/coverage/utils.py
 qiling/extensions/coverage/formats/__init__.py
 qiling/extensions/coverage/formats/base.py
 qiling/extensions/coverage/formats/drcov.py
 qiling/extensions/coverage/formats/drcov_exact.py
+qiling/extensions/coverage/formats/history.py
 qiling/extensions/idaplugin/__init__.py
 qiling/extensions/idaplugin/qilingida.py
 qiling/extensions/mcu/__init__.py
 qiling/extensions/mcu/atmel/__init__.py
 qiling/extensions/mcu/atmel/sam3x8e.py
 qiling/extensions/mcu/bes/__init__.py
 qiling/extensions/mcu/bes/bes2300.py
@@ -548,27 +550,30 @@
 qiling/os/posix/stat.py
 qiling/os/posix/structs.py
 qiling/os/posix/syscall/__init__.py
 qiling/os/posix/syscall/fcntl.py
 qiling/os/posix/syscall/futex.py
 qiling/os/posix/syscall/ioctl.py
 qiling/os/posix/syscall/mman.py
+qiling/os/posix/syscall/msg.py
 qiling/os/posix/syscall/net.py
 qiling/os/posix/syscall/personality.py
 qiling/os/posix/syscall/poll.py
 qiling/os/posix/syscall/prctl.py
 qiling/os/posix/syscall/ptrace.py
 qiling/os/posix/syscall/random.py
 qiling/os/posix/syscall/resource.py
 qiling/os/posix/syscall/sched.py
 qiling/os/posix/syscall/select.py
 qiling/os/posix/syscall/sendfile.py
+qiling/os/posix/syscall/shm.py
 qiling/os/posix/syscall/signal.py
 qiling/os/posix/syscall/socket.py
 qiling/os/posix/syscall/stat.py
+qiling/os/posix/syscall/syscall.py
 qiling/os/posix/syscall/sysctl.py
 qiling/os/posix/syscall/sysinfo.py
 qiling/os/posix/syscall/time.py
 qiling/os/posix/syscall/types.py
 qiling/os/posix/syscall/uio.py
 qiling/os/posix/syscall/unistd.py
 qiling/os/posix/syscall/utsname.py
```

### Comparing `qiling-1.4.5/qiling.egg-info/requires.txt` & `qiling-1.4.6/qiling.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `qiling-1.4.5/qltool` & `qiling-1.4.6/qltool`

 * *Files 3% similar despite different names*

```diff
@@ -1,84 +1,105 @@
 #!/usr/bin/env python3
-# 
+#
 # Cross Platform and Multi Architecture Advanced Binary Emulation Framework
 #
 
 import argparse
 import os
 import sys
 import ast
 import pickle
+
 from pprint import pprint
+from typing import TYPE_CHECKING, Mapping, Type
 
 from unicorn import __version__ as uc_ver
 from qiling import __version__ as ql_ver
 
 from qiling import Qiling
 from qiling.arch import utils as arch_utils
 from qiling.debugger.qdb import QlQdb
-from qiling.utils import arch_convert
 from qiling.const import QL_VERBOSE, QL_ENDIAN, os_map, arch_map, verbose_map
 from qiling.extensions.coverage import utils as cov_utils
 from qiling.extensions import report
 
+
+if TYPE_CHECKING:
+    from enum import Enum
+
+
 # read code from file
 def read_file(fname: str):
     with open(fname, "rb") as f:
         content = f.read()
 
     return content
 
+
 class __arg_env(argparse.Action):
-    def __call__(self, parser, namespace, values, option_string):
+    def __call__(self, parser, namespace, values: str, option_string):
         if os.path.exists(values):
             with open(values, 'rb') as f:
                 env = pickle.load(f)
         else:
             env = ast.literal_eval(values)
 
         setattr(namespace, self.dest, env or {})
 
-class __arg_verbose(argparse.Action):
-    def __call__(self, parser, namespace, values, option_string):
-        setattr(namespace, self.dest, verbose_map[values])
+
+def __make_enum_arg(enum_rmap: Mapping[str, 'Enum'], aliases: Mapping[str, str] = {}) -> Type[argparse.Action]:
+    class __enum_arg(argparse.Action):
+        def __call__(self, parser, namespace, values: str, option_string):
+            values = values.casefold()
+
+            if values in aliases:
+                values = aliases[values]
+
+            setattr(namespace, self.dest, enum_rmap[values])
+
+    return __enum_arg
+
+
+__arg_archtype = __make_enum_arg(arch_map, {'x86_64': 'x8664', 'riscv32': 'riscv'})
+__arg_ostype = __make_enum_arg(os_map, {'darwin': 'macos'})
+__arg_verbose = __make_enum_arg(verbose_map)
+
 
 def handle_code(options: argparse.Namespace):
     archendian = {
         'little': QL_ENDIAN.EL,
         'big'   : QL_ENDIAN.EB
     }[options.endian]
 
     if options.format == 'hex':
         if options.input is not None:
-            print ("Load HEX from ARGV")
+            print("Load HEX from ARGV")
             code = str(options.input).strip("\\\\x").split("x")
             code = "".join(code).strip()
-            code =  bytes.fromhex(code)
+            code = bytes.fromhex(code)
         elif options.filename is not None:
-            print ("Load HEX from FILE")
+            print("Load HEX from FILE")
             code = str(read_file(options.filename)).strip('b\'').strip('\\n')
             code = code.strip('x').split("\\\\x")
             code = "".join(code).strip()
             code = bytes.fromhex(code)
         else:
             print("ERROR: File not found")
             exit(1)
 
     elif options.format == 'asm':
-        print ("Load ASM from FILE")
+        print("Load ASM from FILE")
         assembly = read_file(options.filename)
-        archtype = arch_convert(options.arch)
 
-        assembler = arch_utils.assembler(archtype, archendian, options.thumb)
+        assembler = arch_utils.assembler(options.arch, archendian, options.thumb)
         code, _ = assembler.asm(assembly)
         code = bytes(code)
 
     elif options.format == 'bin':
-        print ("Load BIN from FILE")
+        print("Load BIN from FILE")
         if options.filename is not None:
             code = read_file(options.filename)
         else:
             print("ERROR: File not found")
             exit(1)
 
     ql = Qiling(
@@ -92,14 +113,15 @@
         filter=options.filter,
         endian=archendian,
         thumb=options.thumb,
     )
 
     return ql
 
+
 def handle_run(options: argparse.Namespace):
     effective_argv = []
 
     # with argv
     if options.filename is not None and options.run_args == []:
         effective_argv = [options.filename] + options.args
 
@@ -127,14 +149,15 @@
     # attach Qdb at entry point
     if options.qdb is True:
         QlQdb(ql, rr=options.rr).run()
         exit()
 
     return ql
 
+
 def handle_examples(parser: argparse.ArgumentParser):
     prog = os.path.basename(__file__)
 
     __ql_examples = f"""Examples:
 
     With code:
         {prog} code --os linux --arch arm --format hex -f examples/shellcodes/linarm32_tcp_reverse_shell.hex
@@ -164,14 +187,15 @@
     With binary file and json output:
         {prog} run -f examples/rootfs/x86_windows/bin/x86_hello.exe --rootfs examples/rootfs/x86_windows --no-console --json
 
 """
 
     parser.exit(0, __ql_examples)
 
+
 if __name__ == '__main__':
     parser = argparse.ArgumentParser()
     parser.add_argument('--version', action='version', version=f'qltool for Qiling {ql_ver}, using Unicorn {uc_ver}')
 
     commands = parser.add_subparsers(title='sub commands', description='select execution mode', dest='subcommand', required=True)
 
     # set "run" subcommand options
@@ -181,18 +205,18 @@
     run_parser.add_argument('--args', default=[], nargs=argparse.REMAINDER, dest="args", help="args")
     run_parser.add_argument('run_args', default=[], nargs=argparse.REMAINDER)
 
     # set "code" subcommand options
     code_parser = commands.add_parser('code', help='execute a shellcode')
     code_parser.add_argument('-f', '--filename', metavar="FILE", help="filename")
     code_parser.add_argument('-i', '--input', metavar="INPUT", dest="input", help='input hex value')
-    code_parser.add_argument('--arch', required=True, choices=arch_map)
+    code_parser.add_argument('--arch', required=True, choices=arch_map, action=__arg_archtype)
     code_parser.add_argument('--thumb', action='store_true', default=False, help='specify thumb mode for ARM')
     code_parser.add_argument('--endian', choices=('little', 'big'), default='little', help='specify endianess for bi-endian archs')
-    code_parser.add_argument('--os', required=True, choices=os_map)
+    code_parser.add_argument('--os', required=True, choices=os_map, action=__arg_ostype)
     code_parser.add_argument('--rootfs', default='.', help='emulated root filesystem, that is where all libraries reside')
     code_parser.add_argument('--format', choices=('asm', 'hex', 'bin'), default='bin', help='input file format')
 
     # set "examples" subcommand
     expl_parser = commands.add_parser('examples', help='show examples and exit', add_help=False)
 
     # set "qltui" subcommand
@@ -213,15 +237,15 @@
     comm_parser.add_argument('--profile', help="define a customized profile")
     comm_parser.add_argument('--no-console', action='store_false', dest='console', help='do not emit output to console')
     comm_parser.add_argument('-e', '--filter', metavar='REGEXP', default=None, help="apply a filtering regexp on log output")
     comm_parser.add_argument('--log-file', help="write log to a file")
     comm_parser.add_argument('--log-plain', action='store_true', help="do not use colors in log output")
     comm_parser.add_argument('--root', action='store_true', help='enable sudo required mode')
     comm_parser.add_argument('--debug-stop', action='store_true', help='stop running on error; requires verbose to be set to either "debug" or "dump"')
-    comm_parser.add_argument('-m', '--multithread',action='store_true', help='run in multithread mode')
+    comm_parser.add_argument('-m', '--multithread', action='store_true', help='run in multithread mode')
     comm_parser.add_argument('--timeout', type=int, default=0, help='set emulation timeout')
     comm_parser.add_argument('-c', '--coverage-file', default=None, help='code coverage file name')
     comm_parser.add_argument('--coverage-format', default='drcov', choices=cov_utils.factory.formats, help='code coverage file format')
     comm_parser.add_argument('--json', action='store_true', help='print a json report of the emulation')
     comm_parser.add_argument('--libcache', action='store_true', help='enable dll caching for windows')
     options = parser.parse_args()
```

### Comparing `qiling-1.4.5/setup.py` & `qiling-1.4.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 #!/usr/bin/env python3
 #
 # Python setup for Qiling framework
 
 from setuptools import setup, find_packages
 
 # NOTE: use "-dev" for dev branch
-#VERSION = "1.4.6" + "-dev"
-VERSION = "1.4.5"
+#VERSION = "1.4.7" + "-dev"
+VERSION = "1.4.6"
 
 requirements = [
     "capstone>=4.0.1",
     "unicorn>=2.0.1",
     "pefile>=2022.5.30",
     "python-registry>=1.3.1",
     "keystone-engine>=0.9.2",
@@ -86,15 +86,15 @@
         # that you indicate whether you support Python 2, Python 3 or both.
         'Programming Language :: Python :: 3',
     ],
 
     keywords='qiling binary emulator framework malware analysis UEFI IoT',
 
     packages=find_packages(),
-    scripts=['qltool'],
+    scripts=['qltool', 'qltui.py'],
     package_data={
         'qiling': ['profiles/*.ql'],
         'qiling.debugger.gdb': ['xml/*/*'],
         'qiling.os.uefi': ['guids.csv'],
         'qiling.arch.evm.analysis': ['signatures.json']
     },
     install_requires=requirements,
```

