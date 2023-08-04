# Comparing `tmp/balpy-0.0.0a82.tar.gz` & `tmp/balpy-0.0.0a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "balpy-0.0.0a82.tar", max compression
+gzip compressed data, was "/Users/gerg/Desktop/balancer/balpy/dist/tmpkori4w0v/balpy-0.0.0a9.tar", last modified: Fri Jul  2 20:52:15 2021, max compression
```

## Comparing `balpy-0.0.0a82.tar` & `balpy-0.0.0a9.tar`

### file list

```diff
@@ -1,290 +1,87 @@
--rw-r--r--   0        0        0    35148 2023-07-10 19:21:21.514399 balpy-0.0.0a82/LICENSE
--rw-r--r--   0        0        0       69 2023-07-10 19:21:21.514577 balpy-0.0.0a82/balpy/__init__.py
--rw-r--r--   0        0        0     5272 2023-07-10 19:21:21.523718 balpy-0.0.0a82/balpy/abi/ERC20.json
--rw-r--r--   0        0        0     3021 2023-07-10 19:21:21.523839 balpy-0.0.0a82/balpy/balancerErrors.py
--rw-r--r--   0        0        0     1837 2023-07-10 19:21:21.523945 balpy-0.0.0a82/balpy/balancerv2cad/.gitignore
--rw-r--r--   0        0        0    35149 2023-07-10 19:21:21.524026 balpy-0.0.0a82/balpy/balancerv2cad/LICENSE
--rw-r--r--   0        0        0     1601 2023-07-10 19:21:21.524111 balpy-0.0.0a82/balpy/balancerv2cad/README.md
--rw-r--r--   0        0        0     6175 2023-07-10 19:21:21.524220 balpy-0.0.0a82/balpy/balancerv2cad/notebooks/BalancerV2.ipynb
--rw-r--r--   0        0        0     5825 2023-07-10 19:21:21.524301 balpy-0.0.0a82/balpy/balancerv2cad/poetry.lock
--rw-r--r--   0        0        0      721 2023-07-10 19:21:21.524362 balpy-0.0.0a82/balpy/balancerv2cad/pyproject.toml
--rw-r--r--   0        0        0     1354 2023-07-10 19:21:21.524465 balpy-0.0.0a82/balpy/balancerv2cad/scripts/project_helper.py
--rw-r--r--   0        0        0      366 2023-07-10 19:21:21.524585 balpy-0.0.0a82/balpy/balancerv2cad/src/balancerv2cad/BalancerConstants.py
--rw-r--r--   0        0        0    17684 2023-07-10 19:21:21.524685 balpy-0.0.0a82/balpy/balancerv2cad/src/balancerv2cad/StableMath.py
--rw-r--r--   0        0        0     2220 2023-07-10 19:21:21.524761 balpy-0.0.0a82/balpy/balancerv2cad/src/balancerv2cad/StablePool.py
--rw-r--r--   0        0        0    12945 2023-07-10 19:21:21.524847 balpy-0.0.0a82/balpy/balancerv2cad/src/balancerv2cad/WeightedMath.py
--rw-r--r--   0        0        0     3595 2023-07-10 19:21:21.524917 balpy-0.0.0a82/balpy/balancerv2cad/src/balancerv2cad/WeightedPool.py
--rw-r--r--   0        0        0        0 2023-07-10 19:21:21.524945 balpy-0.0.0a82/balpy/balancerv2cad/src/balancerv2cad/__init__.py
--rw-r--r--   0        0        0        0 2023-07-10 19:21:21.525016 balpy-0.0.0a82/balpy/balancerv2cad/src/balancerv2cad/logger/__init__.py
--rw-r--r--   0        0        0     2731 2023-07-10 19:21:21.525095 balpy-0.0.0a82/balpy/balancerv2cad/src/balancerv2cad/logger/pkg_logger.py
--rw-r--r--   0        0        0     1068 2023-07-10 19:21:21.525160 balpy-0.0.0a82/balpy/balancerv2cad/src/balancerv2cad/main.py
--rw-r--r--   0        0        0      984 2023-07-10 19:21:21.525218 balpy-0.0.0a82/balpy/balancerv2cad/src/balancerv2cad/util.py
--rw-r--r--   0        0        0        0 2023-07-10 19:21:21.525271 balpy-0.0.0a82/balpy/balancerv2cad/tests/__init__.py
--rw-r--r--   0        0        0      862 2023-07-10 19:21:21.525337 balpy-0.0.0a82/balpy/balancerv2cad/tests/conftest.py
--rw-r--r--   0        0        0     8323 2023-07-10 19:21:21.525436 balpy-0.0.0a82/balpy/balancerv2cad/tests/unit-test/test_StableMath.py
--rw-r--r--   0        0        0     9042 2023-07-10 19:21:21.525508 balpy-0.0.0a82/balpy/balancerv2cad/tests/unit-test/test_WeightedMath.py
--rw-r--r--   0        0        0      391 2023-07-10 19:21:21.525566 balpy-0.0.0a82/balpy/balancerv2cad/tests/unit-test/test_kickstart.py
--rw-r--r--   0        0        0    94414 2023-07-10 20:27:40.769893 balpy-0.0.0a82/balpy/balpy.py
--rw-r--r--   0        0        0     6452 2023-07-10 19:21:21.526392 balpy-0.0.0a82/balpy/deployments/20210418-authorizer/abi/Authorizer.json
--rw-r--r--   0        0        0       95 2023-07-10 19:21:21.526495 balpy-0.0.0a82/balpy/deployments/20210418-authorizer/output/arbitrum.json
--rw-r--r--   0        0        0       64 2023-07-10 19:21:21.526548 balpy-0.0.0a82/balpy/deployments/20210418-authorizer/output/fantom.json
--rw-r--r--   0        0        0       64 2023-07-10 19:21:21.526600 balpy-0.0.0a82/balpy/deployments/20210418-authorizer/output/goerli.json
--rw-r--r--   0        0        0       64 2023-07-10 19:21:21.526651 balpy-0.0.0a82/balpy/deployments/20210418-authorizer/output/kovan.json
--rw-r--r--   0        0        0       64 2023-07-10 19:21:21.526704 balpy-0.0.0a82/balpy/deployments/20210418-authorizer/output/mainnet.json
--rw-r--r--   0        0        0       94 2023-07-10 19:21:21.526873 balpy-0.0.0a82/balpy/deployments/20210418-authorizer/output/optimism.json
--rw-r--r--   0        0        0       64 2023-07-10 19:21:21.526942 balpy-0.0.0a82/balpy/deployments/20210418-authorizer/output/polygon.json
--rw-r--r--   0        0        0       64 2023-07-10 19:21:21.527000 balpy-0.0.0a82/balpy/deployments/20210418-authorizer/output/rinkeby.json
--rw-r--r--   0        0        0       64 2023-07-10 19:21:21.527062 balpy-0.0.0a82/balpy/deployments/20210418-authorizer/output/ropsten.json
--rw-r--r--   0        0        0     3129 2023-07-10 19:21:21.527194 balpy-0.0.0a82/balpy/deployments/20210418-vault/abi/BalancerHelpers.json
--rw-r--r--   0        0        0    24952 2023-07-10 19:21:21.527268 balpy-0.0.0a82/balpy/deployments/20210418-vault/abi/Vault.json
--rw-r--r--   0        0        0      156 2023-07-10 19:21:21.527370 balpy-0.0.0a82/balpy/deployments/20210418-vault/output/arbitrum.json
--rw-r--r--   0        0        0      126 2023-07-10 19:21:21.527427 balpy-0.0.0a82/balpy/deployments/20210418-vault/output/fantom.json
--rw-r--r--   0        0        0      126 2023-07-10 19:21:21.527485 balpy-0.0.0a82/balpy/deployments/20210418-vault/output/goerli.json
--rw-r--r--   0        0        0      126 2023-07-10 19:21:21.527538 balpy-0.0.0a82/balpy/deployments/20210418-vault/output/kovan.json
--rw-r--r--   0        0        0      126 2023-07-10 19:21:21.527595 balpy-0.0.0a82/balpy/deployments/20210418-vault/output/mainnet.json
--rw-r--r--   0        0        0      156 2023-07-10 19:21:21.527654 balpy-0.0.0a82/balpy/deployments/20210418-vault/output/optimism.json
--rw-r--r--   0        0        0      156 2023-07-10 19:21:21.527707 balpy-0.0.0a82/balpy/deployments/20210418-vault/output/polygon.json
--rw-r--r--   0        0        0      126 2023-07-10 19:21:21.527760 balpy-0.0.0a82/balpy/deployments/20210418-vault/output/rinkeby.json
--rw-r--r--   0        0        0      126 2023-07-10 19:21:21.527814 balpy-0.0.0a82/balpy/deployments/20210418-vault/output/ropsten.json
--rw-r--r--   0        0        0    17557 2023-07-10 19:21:21.528000 balpy-0.0.0a82/balpy/deployments/20210418-weighted-pool/abi/WeightedPool.json
--rw-r--r--   0        0        0    22832 2023-07-10 19:21:21.528110 balpy-0.0.0a82/balpy/deployments/20210418-weighted-pool/abi/WeightedPool2Tokens.json
--rw-r--r--   0        0        0     2366 2023-07-10 19:21:21.528209 balpy-0.0.0a82/balpy/deployments/20210418-weighted-pool/abi/WeightedPool2TokensFactory.json
--rw-r--r--   0        0        0     2261 2023-07-10 19:21:21.528271 balpy-0.0.0a82/balpy/deployments/20210418-weighted-pool/abi/WeightedPoolFactory.json
--rw-r--r--   0        0        0      181 2023-07-10 19:21:21.528360 balpy-0.0.0a82/balpy/deployments/20210418-weighted-pool/output/arbitrum.json
--rw-r--r--   0        0        0      151 2023-07-10 19:21:21.528416 balpy-0.0.0a82/balpy/deployments/20210418-weighted-pool/output/fantom.json
--rw-r--r--   0        0        0      151 2023-07-10 19:21:21.528479 balpy-0.0.0a82/balpy/deployments/20210418-weighted-pool/output/goerli.json
--rw-r--r--   0        0        0      151 2023-07-10 19:21:21.528534 balpy-0.0.0a82/balpy/deployments/20210418-weighted-pool/output/kovan.json
--rw-r--r--   0        0        0      151 2023-07-10 19:21:21.528596 balpy-0.0.0a82/balpy/deployments/20210418-weighted-pool/output/mainnet.json
--rw-r--r--   0        0        0      181 2023-07-10 19:21:21.528698 balpy-0.0.0a82/balpy/deployments/20210418-weighted-pool/output/optimism.json
--rw-r--r--   0        0        0      151 2023-07-10 19:21:21.528801 balpy-0.0.0a82/balpy/deployments/20210418-weighted-pool/output/polygon.json
--rw-r--r--   0        0        0      151 2023-07-10 19:21:21.528906 balpy-0.0.0a82/balpy/deployments/20210418-weighted-pool/output/rinkeby.json
--rw-r--r--   0        0        0      151 2023-07-10 19:21:21.529043 balpy-0.0.0a82/balpy/deployments/20210418-weighted-pool/output/ropsten.json
--rw-r--r--   0        0        0    20951 2023-07-10 19:21:21.529274 balpy-0.0.0a82/balpy/deployments/20210624-stable-pool/abi/StablePool.json
--rw-r--r--   0        0        0     2272 2023-07-10 19:21:21.529375 balpy-0.0.0a82/balpy/deployments/20210624-stable-pool/abi/StablePoolFactory.json
--rw-r--r--   0        0        0      101 2023-07-10 19:21:21.529485 balpy-0.0.0a82/balpy/deployments/20210624-stable-pool/output/arbitrum.json
--rw-r--r--   0        0        0       71 2023-07-10 19:21:21.529542 balpy-0.0.0a82/balpy/deployments/20210624-stable-pool/output/fantom.json
--rw-r--r--   0        0        0      101 2023-07-10 19:21:21.529601 balpy-0.0.0a82/balpy/deployments/20210624-stable-pool/output/kovan.json
--rw-r--r--   0        0        0      101 2023-07-10 19:21:21.529659 balpy-0.0.0a82/balpy/deployments/20210624-stable-pool/output/mainnet.json
--rw-r--r--   0        0        0      101 2023-07-10 19:21:21.529737 balpy-0.0.0a82/balpy/deployments/20210624-stable-pool/output/optimism.json
--rw-r--r--   0        0        0      101 2023-07-10 19:21:21.529796 balpy-0.0.0a82/balpy/deployments/20210624-stable-pool/output/polygon.json
--rw-r--r--   0        0        0      101 2023-07-10 19:21:21.529851 balpy-0.0.0a82/balpy/deployments/20210624-stable-pool/output/rinkeby.json
--rw-r--r--   0        0        0    20592 2023-07-10 19:21:21.530033 balpy-0.0.0a82/balpy/deployments/20210721-liquidity-bootstrapping-pool/abi/LiquidityBootstrappingPool.json
--rw-r--r--   0        0        0     2958 2023-07-10 19:21:21.530111 balpy-0.0.0a82/balpy/deployments/20210721-liquidity-bootstrapping-pool/abi/LiquidityBootstrappingPoolFactory.json
--rw-r--r--   0        0        0      117 2023-07-10 19:21:21.530241 balpy-0.0.0a82/balpy/deployments/20210721-liquidity-bootstrapping-pool/output/arbitrum.json
--rw-r--r--   0        0        0       87 2023-07-10 19:21:21.530309 balpy-0.0.0a82/balpy/deployments/20210721-liquidity-bootstrapping-pool/output/fantom.json
--rw-r--r--   0        0        0      123 2023-07-10 19:21:21.530414 balpy-0.0.0a82/balpy/deployments/20210721-liquidity-bootstrapping-pool/output/goerli.json
--rw-r--r--   0        0        0      117 2023-07-10 19:21:21.530503 balpy-0.0.0a82/balpy/deployments/20210721-liquidity-bootstrapping-pool/output/kovan.json
--rw-r--r--   0        0        0      117 2023-07-10 19:21:21.530565 balpy-0.0.0a82/balpy/deployments/20210721-liquidity-bootstrapping-pool/output/mainnet.json
--rw-r--r--   0        0        0      117 2023-07-10 19:21:21.530620 balpy-0.0.0a82/balpy/deployments/20210721-liquidity-bootstrapping-pool/output/polygon.json
--rw-r--r--   0        0        0      117 2023-07-10 19:21:21.530698 balpy-0.0.0a82/balpy/deployments/20210721-liquidity-bootstrapping-pool/output/rinkeby.json
--rw-r--r--   0        0        0    29126 2023-07-10 19:21:21.530870 balpy-0.0.0a82/balpy/deployments/20210727-meta-stable-pool/abi/MetaStablePool.json
--rw-r--r--   0        0        0     3218 2023-07-10 19:21:21.530954 balpy-0.0.0a82/balpy/deployments/20210727-meta-stable-pool/abi/MetaStablePoolFactory.json
--rw-r--r--   0        0        0      171 2023-07-10 19:21:21.531087 balpy-0.0.0a82/balpy/deployments/20210727-meta-stable-pool/output/arbitrum.json
--rw-r--r--   0        0        0       75 2023-07-10 19:21:21.531162 balpy-0.0.0a82/balpy/deployments/20210727-meta-stable-pool/output/fantom.json
--rw-r--r--   0        0        0       76 2023-07-10 19:21:21.531223 balpy-0.0.0a82/balpy/deployments/20210727-meta-stable-pool/output/goerli.json
--rw-r--r--   0        0        0      171 2023-07-10 19:21:21.531298 balpy-0.0.0a82/balpy/deployments/20210727-meta-stable-pool/output/kovan.json
--rw-r--r--   0        0        0      171 2023-07-10 19:21:21.531390 balpy-0.0.0a82/balpy/deployments/20210727-meta-stable-pool/output/mainnet.json
--rw-r--r--   0        0        0      171 2023-07-10 19:21:21.531476 balpy-0.0.0a82/balpy/deployments/20210727-meta-stable-pool/output/optimism.json
--rw-r--r--   0        0        0      171 2023-07-10 19:21:21.531587 balpy-0.0.0a82/balpy/deployments/20210727-meta-stable-pool/output/polygon.json
--rw-r--r--   0        0        0      171 2023-07-10 19:21:21.531679 balpy-0.0.0a82/balpy/deployments/20210727-meta-stable-pool/output/rinkeby.json
--rw-r--r--   0        0        0     8837 2023-07-10 19:21:21.531847 balpy-0.0.0a82/balpy/deployments/20210811-ldo-merkle/abi/MerkleRedeem.json
--rw-r--r--   0        0        0       97 2023-07-10 19:21:21.531957 balpy-0.0.0a82/balpy/deployments/20210811-ldo-merkle/output/mainnet.json
--rw-r--r--   0        0        0     7542 2023-07-10 19:21:21.532118 balpy-0.0.0a82/balpy/deployments/20210812-lido-relayer/abi/LidoRelayer.json
--rw-r--r--   0        0        0       95 2023-07-10 19:21:21.532253 balpy-0.0.0a82/balpy/deployments/20210812-lido-relayer/output/kovan.json
--rw-r--r--   0        0        0       95 2023-07-10 19:21:21.532346 balpy-0.0.0a82/balpy/deployments/20210812-lido-relayer/output/mainnet.json
--rw-r--r--   0        0        0      669 2023-07-10 19:21:21.532500 balpy-0.0.0a82/balpy/deployments/20210812-wsteth-rate-provider/abi/WstETHRateProvider.json
--rw-r--r--   0        0        0      102 2023-07-10 19:21:21.532641 balpy-0.0.0a82/balpy/deployments/20210812-wsteth-rate-provider/output/kovan.json
--rw-r--r--   0        0        0      102 2023-07-10 19:21:21.532753 balpy-0.0.0a82/balpy/deployments/20210812-wsteth-rate-provider/output/mainnet.json
--rw-r--r--   0        0        0    23050 2023-07-10 19:21:21.532986 balpy-0.0.0a82/balpy/deployments/20210907-investment-pool/abi/InvestmentPool.json
--rw-r--r--   0        0        0     3083 2023-07-10 19:21:21.533079 balpy-0.0.0a82/balpy/deployments/20210907-investment-pool/abi/InvestmentPoolFactory.json
--rw-r--r--   0        0        0      105 2023-07-10 19:21:21.533216 balpy-0.0.0a82/balpy/deployments/20210907-investment-pool/output/arbitrum.json
--rw-r--r--   0        0        0      105 2023-07-10 19:21:21.533288 balpy-0.0.0a82/balpy/deployments/20210907-investment-pool/output/kovan.json
--rw-r--r--   0        0        0      105 2023-07-10 19:21:21.533353 balpy-0.0.0a82/balpy/deployments/20210907-investment-pool/output/mainnet.json
--rw-r--r--   0        0        0      105 2023-07-10 19:21:21.533435 balpy-0.0.0a82/balpy/deployments/20210907-investment-pool/output/polygon.json
--rw-r--r--   0        0        0      105 2023-07-10 19:21:21.533529 balpy-0.0.0a82/balpy/deployments/20210907-investment-pool/output/rinkeby.json
--rw-r--r--   0        0        0     8837 2023-07-10 19:21:21.533689 balpy-0.0.0a82/balpy/deployments/20210913-bal-arbitrum-merkle/abi/MerkleRedeem.json
--rw-r--r--   0        0        0       96 2023-07-10 19:21:21.533811 balpy-0.0.0a82/balpy/deployments/20210913-bal-arbitrum-merkle/output/arbitrum.json
--rw-r--r--   0        0        0     8837 2023-07-10 19:21:21.533988 balpy-0.0.0a82/balpy/deployments/20210928-mcb-arbitrum-merkle/abi/MerkleRedeem.json
--rw-r--r--   0        0        0       96 2023-07-10 19:21:21.534097 balpy-0.0.0a82/balpy/deployments/20210928-mcb-arbitrum-merkle/output/arbitrum.json
--rw-r--r--   0        0        0     9544 2023-07-10 19:21:21.534311 balpy-0.0.0a82/balpy/deployments/20211012-merkle-orchard/abi/MerkleOrchard.json
--rw-r--r--   0        0        0       97 2023-07-10 19:21:21.534440 balpy-0.0.0a82/balpy/deployments/20211012-merkle-orchard/output/arbitrum.json
--rw-r--r--   0        0        0       97 2023-07-10 19:21:21.534543 balpy-0.0.0a82/balpy/deployments/20211012-merkle-orchard/output/kovan.json
--rw-r--r--   0        0        0       97 2023-07-10 19:21:21.534605 balpy-0.0.0a82/balpy/deployments/20211012-merkle-orchard/output/mainnet.json
--rw-r--r--   0        0        0       97 2023-07-10 19:21:21.534664 balpy-0.0.0a82/balpy/deployments/20211012-merkle-orchard/output/polygon.json
--rw-r--r--   0        0        0       97 2023-07-10 19:21:21.534743 balpy-0.0.0a82/balpy/deployments/20211012-merkle-orchard/output/rinkeby.json
--rw-r--r--   0        0        0    20542 2023-07-10 19:21:21.535006 balpy-0.0.0a82/balpy/deployments/20211202-no-protocol-fee-lbp/abi/NoProtocolFeeLiquidityBootstrappingPool.json
--rw-r--r--   0        0        0     3748 2023-07-10 19:21:21.535126 balpy-0.0.0a82/balpy/deployments/20211202-no-protocol-fee-lbp/abi/NoProtocolFeeLiquidityBootstrappingPoolFactory.json
--rw-r--r--   0        0        0      130 2023-07-10 19:21:21.535263 balpy-0.0.0a82/balpy/deployments/20211202-no-protocol-fee-lbp/output/arbitrum.json
--rw-r--r--   0        0        0      130 2023-07-10 19:21:21.535369 balpy-0.0.0a82/balpy/deployments/20211202-no-protocol-fee-lbp/output/kovan.json
--rw-r--r--   0        0        0      130 2023-07-10 19:21:21.535427 balpy-0.0.0a82/balpy/deployments/20211202-no-protocol-fee-lbp/output/mainnet.json
--rw-r--r--   0        0        0      130 2023-07-10 19:21:21.535515 balpy-0.0.0a82/balpy/deployments/20211202-no-protocol-fee-lbp/output/optimism.json
--rw-r--r--   0        0        0      130 2023-07-10 19:21:21.535620 balpy-0.0.0a82/balpy/deployments/20211202-no-protocol-fee-lbp/output/polygon.json
--rw-r--r--   0        0        0      130 2023-07-10 19:21:21.535679 balpy-0.0.0a82/balpy/deployments/20211202-no-protocol-fee-lbp/output/rinkeby.json
--rw-r--r--   0        0        0     1190 2023-07-10 19:21:21.535858 balpy-0.0.0a82/balpy/deployments/20211203-batch-relayer/abi/BalancerRelayer.json
--rw-r--r--   0        0        0    16188 2023-07-10 19:21:21.535919 balpy-0.0.0a82/balpy/deployments/20211203-batch-relayer/abi/BatchRelayerLibrary.json
--rw-r--r--   0        0        0      170 2023-07-10 19:21:21.536005 balpy-0.0.0a82/balpy/deployments/20211203-batch-relayer/output/arbitrum.json
--rw-r--r--   0        0        0      170 2023-07-10 19:21:21.536085 balpy-0.0.0a82/balpy/deployments/20211203-batch-relayer/output/kovan.json
--rw-r--r--   0        0        0      170 2023-07-10 19:21:21.536163 balpy-0.0.0a82/balpy/deployments/20211203-batch-relayer/output/mainnet.json
--rw-r--r--   0        0        0      170 2023-07-10 19:21:21.536235 balpy-0.0.0a82/balpy/deployments/20211203-batch-relayer/output/polygon.json
--rw-r--r--   0        0        0      170 2023-07-10 19:21:21.536312 balpy-0.0.0a82/balpy/deployments/20211203-batch-relayer/output/rinkeby.json
--rw-r--r--   0        0        0    20638 2023-07-10 19:21:21.536541 balpy-0.0.0a82/balpy/deployments/20211208-aave-linear-pool/abi/AaveLinearPool.json
--rw-r--r--   0        0        0     2977 2023-07-10 19:21:21.536645 balpy-0.0.0a82/balpy/deployments/20211208-aave-linear-pool/abi/AaveLinearPoolFactory.json
--rw-r--r--   0        0        0      105 2023-07-10 19:21:21.536728 balpy-0.0.0a82/balpy/deployments/20211208-aave-linear-pool/output/arbitrum.json
--rw-r--r--   0        0        0      105 2023-07-10 19:21:21.536804 balpy-0.0.0a82/balpy/deployments/20211208-aave-linear-pool/output/kovan.json
--rw-r--r--   0        0        0      105 2023-07-10 19:21:21.536909 balpy-0.0.0a82/balpy/deployments/20211208-aave-linear-pool/output/mainnet.json
--rw-r--r--   0        0        0      105 2023-07-10 19:21:21.537006 balpy-0.0.0a82/balpy/deployments/20211208-aave-linear-pool/output/polygon.json
--rw-r--r--   0        0        0    27089 2023-07-10 19:21:21.537180 balpy-0.0.0a82/balpy/deployments/20211208-stable-phantom-pool/abi/StablePhantomPool.json
--rw-r--r--   0        0        0     3133 2023-07-10 19:21:21.537311 balpy-0.0.0a82/balpy/deployments/20211208-stable-phantom-pool/abi/StablePhantomPoolFactory.json
--rw-r--r--   0        0        0      108 2023-07-10 19:21:21.537446 balpy-0.0.0a82/balpy/deployments/20211208-stable-phantom-pool/output/arbitrum.json
--rw-r--r--   0        0        0       78 2023-07-10 19:21:21.537524 balpy-0.0.0a82/balpy/deployments/20211208-stable-phantom-pool/output/fantom.json
--rw-r--r--   0        0        0      108 2023-07-10 19:21:21.537577 balpy-0.0.0a82/balpy/deployments/20211208-stable-phantom-pool/output/kovan.json
--rw-r--r--   0        0        0      108 2023-07-10 19:21:21.537626 balpy-0.0.0a82/balpy/deployments/20211208-stable-phantom-pool/output/mainnet.json
--rw-r--r--   0        0        0      108 2023-07-10 19:21:21.537675 balpy-0.0.0a82/balpy/deployments/20211208-stable-phantom-pool/output/polygon.json
--rw-r--r--   0        0        0    20626 2023-07-10 19:21:21.537807 balpy-0.0.0a82/balpy/deployments/20220304-erc4626-linear-pool/abi/ERC4626LinearPool.json
--rw-r--r--   0        0        0     2977 2023-07-10 19:21:21.537878 balpy-0.0.0a82/balpy/deployments/20220304-erc4626-linear-pool/abi/ERC4626LinearPoolFactory.json
--rw-r--r--   0        0        0       78 2023-07-10 19:21:21.537963 balpy-0.0.0a82/balpy/deployments/20220304-erc4626-linear-pool/output/mainnet.json
--rw-r--r--   0        0        0      108 2023-07-10 19:21:21.538015 balpy-0.0.0a82/balpy/deployments/20220304-erc4626-linear-pool/output/polygon.json
--rw-r--r--   0        0        0     1190 2023-07-10 19:21:21.538130 balpy-0.0.0a82/balpy/deployments/20220318-batch-relayer-v2/abi/BalancerRelayer.json
--rw-r--r--   0        0        0    18945 2023-07-10 19:21:21.538196 balpy-0.0.0a82/balpy/deployments/20220318-batch-relayer-v2/abi/BatchRelayerLibrary.json
--rw-r--r--   0        0        0      170 2023-07-10 19:21:21.538285 balpy-0.0.0a82/balpy/deployments/20220318-batch-relayer-v2/output/polygon.json
--rw-r--r--   0        0        0     1459 2023-07-10 19:21:21.538411 balpy-0.0.0a82/balpy/deployments/20220325-authorizer-adaptor/abi/AuthorizerAdaptor.json
--rw-r--r--   0        0        0      101 2023-07-10 19:21:21.538497 balpy-0.0.0a82/balpy/deployments/20220325-authorizer-adaptor/output/arbitrum.json
--rw-r--r--   0        0        0      101 2023-07-10 19:21:21.538554 balpy-0.0.0a82/balpy/deployments/20220325-authorizer-adaptor/output/kovan.json
--rw-r--r--   0        0        0      101 2023-07-10 19:21:21.538608 balpy-0.0.0a82/balpy/deployments/20220325-authorizer-adaptor/output/mainnet.json
--rw-r--r--   0        0        0      101 2023-07-10 19:21:21.538662 balpy-0.0.0a82/balpy/deployments/20220325-authorizer-adaptor/output/optimism.json
--rw-r--r--   0        0        0      101 2023-07-10 19:21:21.538712 balpy-0.0.0a82/balpy/deployments/20220325-authorizer-adaptor/output/polygon.json
--rw-r--r--   0        0        0     3256 2023-07-10 19:21:21.538843 balpy-0.0.0a82/balpy/deployments/20220325-bal-token-holder-factory/abi/BALTokenHolder.json
--rw-r--r--   0        0        0     2441 2023-07-10 19:21:21.538901 balpy-0.0.0a82/balpy/deployments/20220325-bal-token-holder-factory/abi/BALTokenHolderFactory.json
--rw-r--r--   0        0        0      105 2023-07-10 19:21:21.538985 balpy-0.0.0a82/balpy/deployments/20220325-bal-token-holder-factory/output/kovan.json
--rw-r--r--   0        0        0      105 2023-07-10 19:21:21.539038 balpy-0.0.0a82/balpy/deployments/20220325-bal-token-holder-factory/output/mainnet.json
--rw-r--r--   0        0        0     7339 2023-07-10 19:21:21.539166 balpy-0.0.0a82/balpy/deployments/20220325-balancer-token-admin/abi/BalancerTokenAdmin.json
--rw-r--r--   0        0        0      102 2023-07-10 19:21:21.539249 balpy-0.0.0a82/balpy/deployments/20220325-balancer-token-admin/output/kovan.json
--rw-r--r--   0        0        0      102 2023-07-10 19:21:21.539308 balpy-0.0.0a82/balpy/deployments/20220325-balancer-token-admin/output/mainnet.json
--rw-r--r--   0        0        0     6093 2023-07-10 19:21:21.539468 balpy-0.0.0a82/balpy/deployments/20220325-gauge-adder/abi/GaugeAdder.json
--rw-r--r--   0        0        0       94 2023-07-10 19:21:21.539557 balpy-0.0.0a82/balpy/deployments/20220325-gauge-adder/output/kovan.json
--rw-r--r--   0        0        0       94 2023-07-10 19:21:21.539618 balpy-0.0.0a82/balpy/deployments/20220325-gauge-adder/output/mainnet.json
--rw-r--r--   0        0        0     7585 2023-07-10 19:21:21.539804 balpy-0.0.0a82/balpy/deployments/20220325-gauge-controller/abi/BalancerMinter.json
--rw-r--r--   0        0        0    13181 2023-07-10 19:21:21.539901 balpy-0.0.0a82/balpy/deployments/20220325-gauge-controller/abi/GaugeController.json
--rw-r--r--   0        0        0     9844 2023-07-10 19:21:21.539998 balpy-0.0.0a82/balpy/deployments/20220325-gauge-controller/abi/VotingEscrow.json
--rw-r--r--   0        0        0      229 2023-07-10 19:21:21.540322 balpy-0.0.0a82/balpy/deployments/20220325-gauge-controller/output/kovan.json
--rw-r--r--   0        0        0      229 2023-07-10 19:21:21.540387 balpy-0.0.0a82/balpy/deployments/20220325-gauge-controller/output/mainnet.json
--rw-r--r--   0        0        0     2402 2023-07-10 19:21:21.540611 balpy-0.0.0a82/balpy/deployments/20220325-mainnet-gauge-factory/abi/LiquidityGaugeFactory.json
--rw-r--r--   0        0        0    22312 2023-07-10 19:21:21.540722 balpy-0.0.0a82/balpy/deployments/20220325-mainnet-gauge-factory/abi/LiquidityGaugeV5.json
--rw-r--r--   0        0        0      173 2023-07-10 19:21:21.540848 balpy-0.0.0a82/balpy/deployments/20220325-mainnet-gauge-factory/output/kovan.json
--rw-r--r--   0        0        0      173 2023-07-10 19:21:21.540914 balpy-0.0.0a82/balpy/deployments/20220325-mainnet-gauge-factory/output/mainnet.json
--rw-r--r--   0        0        0     3125 2023-07-10 19:21:21.541136 balpy-0.0.0a82/balpy/deployments/20220325-single-recipient-gauge-factory/abi/SingleRecipientGauge.json
--rw-r--r--   0        0        0     2890 2023-07-10 19:21:21.541204 balpy-0.0.0a82/balpy/deployments/20220325-single-recipient-gauge-factory/abi/SingleRecipientGaugeFactory.json
--rw-r--r--   0        0        0      111 2023-07-10 19:21:21.541307 balpy-0.0.0a82/balpy/deployments/20220325-single-recipient-gauge-factory/output/kovan.json
--rw-r--r--   0        0        0      111 2023-07-10 19:21:21.541373 balpy-0.0.0a82/balpy/deployments/20220325-single-recipient-gauge-factory/output/mainnet.json
--rw-r--r--   0        0        0    12812 2023-07-10 19:21:21.541548 balpy-0.0.0a82/balpy/deployments/20220325-test-balancer-token/abi/TestBalancerToken.json
--rw-r--r--   0        0        0      101 2023-07-10 19:21:21.541661 balpy-0.0.0a82/balpy/deployments/20220325-test-balancer-token/output/kovan.json
--rw-r--r--   0        0        0    15900 2023-07-10 19:21:21.541931 balpy-0.0.0a82/balpy/deployments/20220325-ve-delegation/abi/VotingEscrowDelegation.json
--rw-r--r--   0        0        0     3109 2023-07-10 19:21:21.542030 balpy-0.0.0a82/balpy/deployments/20220325-ve-delegation/abi/VotingEscrowDelegationProxy.json
--rw-r--r--   0        0        0      185 2023-07-10 19:21:21.542182 balpy-0.0.0a82/balpy/deployments/20220325-ve-delegation/output/kovan.json
--rw-r--r--   0        0        0      185 2023-07-10 19:21:21.542245 balpy-0.0.0a82/balpy/deployments/20220325-ve-delegation/output/mainnet.json
--rw-r--r--   0        0        0     8430 2023-07-10 19:21:21.542411 balpy-0.0.0a82/balpy/deployments/20220325-veBAL-deployment-coordinator/abi/veBALDeploymentCoordinator.json
--rw-r--r--   0        0        0      110 2023-07-10 19:21:21.542502 balpy-0.0.0a82/balpy/deployments/20220325-veBAL-deployment-coordinator/output/kovan.json
--rw-r--r--   0        0        0      110 2023-07-10 19:21:21.542560 balpy-0.0.0a82/balpy/deployments/20220325-veBAL-deployment-coordinator/output/mainnet.json
--rw-r--r--   0        0        0     2808 2023-07-10 19:21:21.542746 balpy-0.0.0a82/balpy/deployments/20220413-arbitrum-root-gauge-factory/abi/ArbitrumRootGauge.json
--rw-r--r--   0        0        0     5030 2023-07-10 19:21:21.542817 balpy-0.0.0a82/balpy/deployments/20220413-arbitrum-root-gauge-factory/abi/ArbitrumRootGaugeFactory.json
--rw-r--r--   0        0        0      108 2023-07-10 19:21:21.542930 balpy-0.0.0a82/balpy/deployments/20220413-arbitrum-root-gauge-factory/output/mainnet.json
--rw-r--r--   0        0        0     4884 2023-07-10 19:21:21.543091 balpy-0.0.0a82/balpy/deployments/20220413-child-chain-gauge-factory/abi/ChildChainLiquidityGaugeFactory.json
--rw-r--r--   0        0        0     5740 2023-07-10 19:21:21.543169 balpy-0.0.0a82/balpy/deployments/20220413-child-chain-gauge-factory/abi/ChildChainStreamer.json
--rw-r--r--   0        0        0    17344 2023-07-10 19:21:21.543257 balpy-0.0.0a82/balpy/deployments/20220413-child-chain-gauge-factory/abi/RewardsOnlyGauge.json
--rw-r--r--   0        0        0      253 2023-07-10 19:21:21.543378 balpy-0.0.0a82/balpy/deployments/20220413-child-chain-gauge-factory/output/arbitrum.json
--rw-r--r--   0        0        0      253 2023-07-10 19:21:21.543445 balpy-0.0.0a82/balpy/deployments/20220413-child-chain-gauge-factory/output/kovan.json
--rw-r--r--   0        0        0      253 2023-07-10 19:21:21.543510 balpy-0.0.0a82/balpy/deployments/20220413-child-chain-gauge-factory/output/polygon.json
--rw-r--r--   0        0        0     3213 2023-07-10 19:21:21.543660 balpy-0.0.0a82/balpy/deployments/20220413-polygon-root-gauge-factory/abi/PolygonRootGauge.json
--rw-r--r--   0        0        0     2504 2023-07-10 19:21:21.543721 balpy-0.0.0a82/balpy/deployments/20220413-polygon-root-gauge-factory/abi/PolygonRootGaugeFactory.json
--rw-r--r--   0        0        0      107 2023-07-10 19:21:21.543817 balpy-0.0.0a82/balpy/deployments/20220413-polygon-root-gauge-factory/output/mainnet.json
--rw-r--r--   0        0        0     2950 2023-07-10 19:21:21.543974 balpy-0.0.0a82/balpy/deployments/20220415-veBAL-L2-gauge-setup-coordinator/abi/veBALL2GaugeSetupCoordinator.json
--rw-r--r--   0        0        0      112 2023-07-10 19:21:21.544077 balpy-0.0.0a82/balpy/deployments/20220415-veBAL-L2-gauge-setup-coordinator/output/mainnet.json
--rw-r--r--   0        0        0     2383 2023-07-10 19:21:21.544240 balpy-0.0.0a82/balpy/deployments/20220418-veBAL-gauge-fix-coordinator/abi/veBALGaugeFixCoordinator.json
--rw-r--r--   0        0        0      108 2023-07-10 19:21:21.544337 balpy-0.0.0a82/balpy/deployments/20220418-veBAL-gauge-fix-coordinator/output/mainnet.json
--rw-r--r--   0        0        0     7262 2023-07-10 19:21:21.544492 balpy-0.0.0a82/balpy/deployments/20220420-fee-distributor/abi/FeeDistributor.json
--rw-r--r--   0        0        0       98 2023-07-10 19:21:21.544598 balpy-0.0.0a82/balpy/deployments/20220420-fee-distributor/output/mainnet.json
--rw-r--r--   0        0        0     3086 2023-07-10 19:21:21.544750 balpy-0.0.0a82/balpy/deployments/20220420-smart-wallet-checker/abi/SmartWalletChecker.json
--rw-r--r--   0        0        0      102 2023-07-10 19:21:21.544855 balpy-0.0.0a82/balpy/deployments/20220420-smart-wallet-checker/output/mainnet.json
--rw-r--r--   0        0        0     2131 2023-07-10 19:21:21.544997 balpy-0.0.0a82/balpy/deployments/20220421-smart-wallet-checker-coordinator/abi/SmartWalletCheckerCoordinator.json
--rw-r--r--   0        0        0      113 2023-07-10 19:21:21.545087 balpy-0.0.0a82/balpy/deployments/20220421-smart-wallet-checker-coordinator/output/mainnet.json
--rw-r--r--   0        0        0     3224 2023-07-10 19:21:21.545219 balpy-0.0.0a82/balpy/deployments/20220422-distribution-scheduler/abi/DistributionScheduler.json
--rw-r--r--   0        0        0      105 2023-07-10 19:21:21.545326 balpy-0.0.0a82/balpy/deployments/20220422-distribution-scheduler/output/kovan.json
--rw-r--r--   0        0        0      105 2023-07-10 19:21:21.545393 balpy-0.0.0a82/balpy/deployments/20220422-distribution-scheduler/output/mainnet.json
--rw-r--r--   0        0        0    22333 2023-07-10 19:21:21.545574 balpy-0.0.0a82/balpy/deployments/20220609-stable-pool-v2/abi/StablePool.json
--rw-r--r--   0        0        0     3892 2023-07-10 19:21:21.545655 balpy-0.0.0a82/balpy/deployments/20220609-stable-pool-v2/abi/StablePoolFactory.json
--rw-r--r--   0        0        0      102 2023-07-10 19:21:21.545753 balpy-0.0.0a82/balpy/deployments/20220609-stable-pool-v2/output/arbitrum.json
--rw-r--r--   0        0        0      101 2023-07-10 19:21:21.545813 balpy-0.0.0a82/balpy/deployments/20220609-stable-pool-v2/output/kovan.json
--rw-r--r--   0        0        0      101 2023-07-10 19:21:21.545879 balpy-0.0.0a82/balpy/deployments/20220609-stable-pool-v2/output/mainnet.json
--rw-r--r--   0        0        0      101 2023-07-10 19:21:21.545939 balpy-0.0.0a82/balpy/deployments/20220609-stable-pool-v2/output/optimism.json
--rw-r--r--   0        0        0      101 2023-07-10 19:21:21.545999 balpy-0.0.0a82/balpy/deployments/20220609-stable-pool-v2/output/polygon.json
--rw-r--r--   0        0        0     4884 2023-07-10 19:21:21.546140 balpy-0.0.0a82/balpy/deployments/20220725-protocol-fee-percentages-provider/abi/ProtocolFeePercentagesProvider.json
--rw-r--r--   0        0        0      114 2023-07-10 19:21:21.546239 balpy-0.0.0a82/balpy/deployments/20220725-protocol-fee-percentages-provider/output/arbitrum.json
--rw-r--r--   0        0        0      114 2023-07-10 19:21:21.546298 balpy-0.0.0a82/balpy/deployments/20220725-protocol-fee-percentages-provider/output/goerli.json
--rw-r--r--   0        0        0      114 2023-07-10 19:21:21.546354 balpy-0.0.0a82/balpy/deployments/20220725-protocol-fee-percentages-provider/output/mainnet.json
--rw-r--r--   0        0        0      114 2023-07-10 19:21:21.546412 balpy-0.0.0a82/balpy/deployments/20220725-protocol-fee-percentages-provider/output/optimism.json
--rw-r--r--   0        0        0      114 2023-07-10 19:21:21.546467 balpy-0.0.0a82/balpy/deployments/20220725-protocol-fee-percentages-provider/output/polygon.json
--rw-r--r--   0        0        0    22764 2023-07-10 19:21:21.546598 balpy-0.0.0a82/balpy/deployments/20220817-aave-rebalanced-linear-pool/abi/AaveLinearPool.json
--rw-r--r--   0        0        0     4373 2023-07-10 19:21:21.546669 balpy-0.0.0a82/balpy/deployments/20220817-aave-rebalanced-linear-pool/abi/AaveLinearPoolFactory.json
--rw-r--r--   0        0        0     1376 2023-07-10 19:21:21.547014 balpy-0.0.0a82/balpy/deployments/20220817-aave-rebalanced-linear-pool/abi/AaveLinearPoolRebalancer.json
--rw-r--r--   0        0        0      105 2023-07-10 19:21:21.547125 balpy-0.0.0a82/balpy/deployments/20220817-aave-rebalanced-linear-pool/output/arbitrum.json
--rw-r--r--   0        0        0      105 2023-07-10 19:21:21.547184 balpy-0.0.0a82/balpy/deployments/20220817-aave-rebalanced-linear-pool/output/goerli.json
--rw-r--r--   0        0        0      105 2023-07-10 19:21:21.547369 balpy-0.0.0a82/balpy/deployments/20220817-aave-rebalanced-linear-pool/output/mainnet.json
--rw-r--r--   0        0        0      105 2023-07-10 19:21:21.547467 balpy-0.0.0a82/balpy/deployments/20220817-aave-rebalanced-linear-pool/output/optimism.json
--rw-r--r--   0        0        0      105 2023-07-10 19:21:21.547543 balpy-0.0.0a82/balpy/deployments/20220817-aave-rebalanced-linear-pool/output/polygon.json
--rw-r--r--   0        0        0    27639 2023-07-10 19:21:21.547751 balpy-0.0.0a82/balpy/deployments/20220906-composable-stable-pool/abi/ComposableStablePool.json
--rw-r--r--   0        0        0     4446 2023-07-10 19:21:21.547846 balpy-0.0.0a82/balpy/deployments/20220906-composable-stable-pool/abi/ComposableStablePoolFactory.json
--rw-r--r--   0        0        0      111 2023-07-10 19:21:21.547963 balpy-0.0.0a82/balpy/deployments/20220906-composable-stable-pool/output/arbitrum.json
--rw-r--r--   0        0        0      111 2023-07-10 19:21:21.548055 balpy-0.0.0a82/balpy/deployments/20220906-composable-stable-pool/output/goerli.json
--rw-r--r--   0        0        0      111 2023-07-10 19:21:21.548121 balpy-0.0.0a82/balpy/deployments/20220906-composable-stable-pool/output/mainnet.json
--rw-r--r--   0        0        0      111 2023-07-10 19:21:21.548186 balpy-0.0.0a82/balpy/deployments/20220906-composable-stable-pool/output/optimism.json
--rw-r--r--   0        0        0      111 2023-07-10 19:21:21.548255 balpy-0.0.0a82/balpy/deployments/20220906-composable-stable-pool/output/polygon.json
--rw-r--r--   0        0        0    22393 2023-07-10 19:21:21.548421 balpy-0.0.0a82/balpy/deployments/20220908-weighted-pool-v2/abi/WeightedPool.json
--rw-r--r--   0        0        0     4456 2023-07-10 19:21:21.548506 balpy-0.0.0a82/balpy/deployments/20220908-weighted-pool-v2/abi/WeightedPoolFactory.json
--rw-r--r--   0        0        0      103 2023-07-10 19:21:21.548623 balpy-0.0.0a82/balpy/deployments/20220908-weighted-pool-v2/output/arbitrum.json
--rw-r--r--   0        0        0      103 2023-07-10 19:21:21.548774 balpy-0.0.0a82/balpy/deployments/20220908-weighted-pool-v2/output/goerli.json
--rw-r--r--   0        0        0      103 2023-07-10 19:21:21.548852 balpy-0.0.0a82/balpy/deployments/20220908-weighted-pool-v2/output/mainnet.json
--rw-r--r--   0        0        0      103 2023-07-10 19:21:21.548919 balpy-0.0.0a82/balpy/deployments/20220908-weighted-pool-v2/output/optimism.json
--rw-r--r--   0        0        0      103 2023-07-10 19:21:21.548983 balpy-0.0.0a82/balpy/deployments/20220908-weighted-pool-v2/output/polygon.json
--rw-r--r--   0        0        0      562 2023-07-10 19:21:21.549132 balpy-0.0.0a82/balpy/deployments/20221021-managed-pool/abi/CircuitBreakerLib.json
--rw-r--r--   0        0        0    34468 2023-07-10 19:21:21.549232 balpy-0.0.0a82/balpy/deployments/20221021-managed-pool/abi/ManagedPool.json
--rw-r--r--   0        0        0     5521 2023-07-10 19:21:21.549304 balpy-0.0.0a82/balpy/deployments/20221021-managed-pool/abi/ManagedPoolFactory.json
--rw-r--r--   0        0        0      251 2023-07-10 19:21:21.549451 balpy-0.0.0a82/balpy/deployments/20221021-managed-pool/output/arbitrum.json
--rw-r--r--   0        0        0      251 2023-07-10 19:21:21.549535 balpy-0.0.0a82/balpy/deployments/20221021-managed-pool/output/goerli.json
--rw-r--r--   0        0        0      251 2023-07-10 19:21:21.549621 balpy-0.0.0a82/balpy/deployments/20221021-managed-pool/output/mainnet.json
--rw-r--r--   0        0        0      251 2023-07-10 19:21:21.549703 balpy-0.0.0a82/balpy/deployments/20221021-managed-pool/output/optimism.json
--rw-r--r--   0        0        0      251 2023-07-10 19:21:21.549780 balpy-0.0.0a82/balpy/deployments/20221021-managed-pool/output/polygon.json
--rw-r--r--   0        0        0    27985 2023-07-10 19:21:21.550035 balpy-0.0.0a82/balpy/deployments/20230206-composable-stable-pool-v3/abi/ComposableStablePool.json
--rw-r--r--   0        0        0     5400 2023-07-10 19:21:21.550127 balpy-0.0.0a82/balpy/deployments/20230206-composable-stable-pool-v3/abi/ComposableStablePoolFactory.json
--rw-r--r--   0        0        0      157 2023-07-10 19:21:21.550259 balpy-0.0.0a82/balpy/deployments/20230206-composable-stable-pool-v3/output/arbitrum.json
--rw-r--r--   0        0        0      157 2023-07-10 19:21:21.550336 balpy-0.0.0a82/balpy/deployments/20230206-composable-stable-pool-v3/output/bsc.json
--rw-r--r--   0        0        0      157 2023-07-10 19:21:21.550408 balpy-0.0.0a82/balpy/deployments/20230206-composable-stable-pool-v3/output/gnosis.json
--rw-r--r--   0        0        0      157 2023-07-10 19:21:21.550484 balpy-0.0.0a82/balpy/deployments/20230206-composable-stable-pool-v3/output/goerli.json
--rw-r--r--   0        0        0      157 2023-07-10 19:21:21.550559 balpy-0.0.0a82/balpy/deployments/20230206-composable-stable-pool-v3/output/mainnet.json
--rw-r--r--   0        0        0      157 2023-07-10 19:21:21.550630 balpy-0.0.0a82/balpy/deployments/20230206-composable-stable-pool-v3/output/optimism.json
--rw-r--r--   0        0        0      157 2023-07-10 19:21:21.550708 balpy-0.0.0a82/balpy/deployments/20230206-composable-stable-pool-v3/output/polygon.json
--rw-r--r--   0        0        0    24366 2023-07-10 19:21:21.550916 balpy-0.0.0a82/balpy/deployments/20230206-erc4626-linear-pool-v3/abi/ERC4626LinearPool.json
--rw-r--r--   0        0        0     6198 2023-07-10 19:21:21.551007 balpy-0.0.0a82/balpy/deployments/20230206-erc4626-linear-pool-v3/abi/ERC4626LinearPoolFactory.json
--rw-r--r--   0        0        0     1376 2023-07-10 19:21:21.551090 balpy-0.0.0a82/balpy/deployments/20230206-erc4626-linear-pool-v3/abi/ERC4626LinearPoolRebalancer.json
--rw-r--r--   0        0        0      223 2023-07-10 19:21:21.551208 balpy-0.0.0a82/balpy/deployments/20230206-erc4626-linear-pool-v3/output/arbitrum.json
--rw-r--r--   0        0        0      223 2023-07-10 19:21:21.551278 balpy-0.0.0a82/balpy/deployments/20230206-erc4626-linear-pool-v3/output/goerli.json
--rw-r--r--   0        0        0      149 2023-07-10 19:21:21.551334 balpy-0.0.0a82/balpy/deployments/20230206-erc4626-linear-pool-v3/output/mainnet.json
--rw-r--r--   0        0        0      223 2023-07-10 19:21:21.551385 balpy-0.0.0a82/balpy/deployments/20230206-erc4626-linear-pool-v3/output/optimism.json
--rw-r--r--   0        0        0      223 2023-07-10 19:21:21.551442 balpy-0.0.0a82/balpy/deployments/20230206-erc4626-linear-pool-v3/output/polygon.json
--rw-r--r--   0        0        0       78 2023-07-10 19:21:21.551495 balpy-0.0.0a82/balpy/deployments/20230206-erc4626-linear-pool-v3/output/test.json
--rw-r--r--   0        0        0    22718 2023-07-10 19:21:21.551653 balpy-0.0.0a82/balpy/deployments/20230206-weighted-pool-v3/abi/WeightedPool.json
--rw-r--r--   0        0        0     5125 2023-07-10 19:21:21.551727 balpy-0.0.0a82/balpy/deployments/20230206-weighted-pool-v3/abi/WeightedPoolFactory.json
--rw-r--r--   0        0        0      141 2023-07-10 19:21:21.551817 balpy-0.0.0a82/balpy/deployments/20230206-weighted-pool-v3/output/arbitrum.json
--rw-r--r--   0        0        0      141 2023-07-10 19:21:21.551873 balpy-0.0.0a82/balpy/deployments/20230206-weighted-pool-v3/output/bsc.json
--rw-r--r--   0        0        0      141 2023-07-10 19:21:21.551933 balpy-0.0.0a82/balpy/deployments/20230206-weighted-pool-v3/output/gnosis.json
--rw-r--r--   0        0        0      141 2023-07-10 19:21:21.551992 balpy-0.0.0a82/balpy/deployments/20230206-weighted-pool-v3/output/goerli.json
--rw-r--r--   0        0        0      141 2023-07-10 19:21:21.552052 balpy-0.0.0a82/balpy/deployments/20230206-weighted-pool-v3/output/mainnet.json
--rw-r--r--   0        0        0      141 2023-07-10 19:21:21.552119 balpy-0.0.0a82/balpy/deployments/20230206-weighted-pool-v3/output/optimism.json
--rw-r--r--   0        0        0      141 2023-07-10 19:21:21.552173 balpy-0.0.0a82/balpy/deployments/20230206-weighted-pool-v3/output/polygon.json
--rw-r--r--   0        0        0        0 2023-07-10 19:21:21.552235 balpy-0.0.0a82/balpy/enums/__init__.py
--rw-r--r--   0        0        0      361 2023-07-10 19:21:21.552306 balpy-0.0.0a82/balpy/enums/stablePoolJoinExitKind.py
--rw-r--r--   0        0        0      353 2023-07-10 19:21:21.552365 balpy-0.0.0a82/balpy/enums/weightedPoolJoinExitKind.py
--rw-r--r--   0        0        0       30 2023-07-10 19:21:21.552448 balpy-0.0.0a82/balpy/graph/__init__.py
--rw-r--r--   0        0        0     7869 2023-07-10 19:21:21.552533 balpy-0.0.0a82/balpy/graph/graph.py
--rw-r--r--   0        0        0      466 2023-07-10 20:30:05.157736 balpy-0.0.0a82/pyproject.toml
--rw-r--r--   0        0        0     6941 2023-07-10 20:30:27.737469 balpy-0.0.0a82/setup.py
--rw-r--r--   0        0        0      639 2023-07-10 20:30:27.737685 balpy-0.0.0a82/PKG-INFO
+drwxr-xr-x   0 gerg       (506) staff       (20)        0 2021-07-02 20:52:15.889461 balpy-0.0.0a9/
+-rw-r--r--   0 gerg       (506) staff       (20)    35148 2021-06-11 18:50:15.000000 balpy-0.0.0a9/LICENSE
+-rw-r--r--   0 gerg       (506) staff       (20)       54 2021-06-11 16:57:24.000000 balpy-0.0.0a9/MANIFEST.in
+-rw-r--r--   0 gerg       (506) staff       (20)     1791 2021-07-02 20:52:15.889700 balpy-0.0.0a9/PKG-INFO
+-rw-r--r--   0 gerg       (506) staff       (20)     1267 2021-06-18 14:54:53.000000 balpy-0.0.0a9/README.md
+drwxr-xr-x   0 gerg       (506) staff       (20)        0 2021-07-02 20:52:15.718829 balpy-0.0.0a9/balpy/
+-rw-r--r--   0 gerg       (506) staff       (20)       24 2021-06-09 23:53:58.000000 balpy-0.0.0a9/balpy/__init__.py
+drwxr-xr-x   0 gerg       (506) staff       (20)        0 2021-07-02 20:52:15.733117 balpy-0.0.0a9/balpy/abi/
+-rw-r--r--   0 gerg       (506) staff       (20)     3129 2021-05-28 17:03:32.000000 balpy-0.0.0a9/balpy/abi/BalancerHelpers.json
+-rw-r--r--   0 gerg       (506) staff       (20)     5265 2021-05-28 17:03:32.000000 balpy-0.0.0a9/balpy/abi/BalancerPoolToken.json
+-rw-r--r--   0 gerg       (506) staff       (20)      466 2021-05-28 17:03:32.000000 balpy-0.0.0a9/balpy/abi/BasePoolFactory.json
+-rw-r--r--   0 gerg       (506) staff       (20)     5272 2021-05-28 17:03:32.000000 balpy-0.0.0a9/balpy/abi/ERC20.json
+-rw-r--r--   0 gerg       (506) staff       (20)    25917 2021-05-28 17:03:32.000000 balpy-0.0.0a9/balpy/abi/ExchangeProxy.json
+-rw-r--r--   0 gerg       (506) staff       (20)      916 2021-05-28 17:03:32.000000 balpy-0.0.0a9/balpy/abi/Multicall.json
+-rw-r--r--   0 gerg       (506) staff       (20)    15112 2021-05-28 17:03:32.000000 balpy-0.0.0a9/balpy/abi/StablePool.json
+-rw-r--r--   0 gerg       (506) staff       (20)     1689 2021-05-28 17:03:32.000000 balpy-0.0.0a9/balpy/abi/StablePoolFactory.json
+-rw-r--r--   0 gerg       (506) staff       (20)    24945 2021-05-28 17:03:32.000000 balpy-0.0.0a9/balpy/abi/Vault.json
+-rw-r--r--   0 gerg       (506) staff       (20)    17544 2021-05-28 17:03:32.000000 balpy-0.0.0a9/balpy/abi/WeightedPool.json
+-rw-r--r--   0 gerg       (506) staff       (20)     1678 2021-05-28 17:03:32.000000 balpy-0.0.0a9/balpy/abi/WeightedPoolFactory.json
+-rw-r--r--   0 gerg       (506) staff       (20)      418 2021-05-28 17:03:32.000000 balpy-0.0.0a9/balpy/abi/Weth.json
+drwxr-xr-x   0 gerg       (506) staff       (20)        0 2021-07-02 20:52:15.714837 balpy-0.0.0a9/balpy/artifacts/
+drwxr-xr-x   0 gerg       (506) staff       (20)        0 2021-07-02 20:52:15.748751 balpy-0.0.0a9/balpy/artifacts/goerli/
+-rw-r--r--   0 gerg       (506) staff       (20)    72282 2021-05-28 17:03:35.000000 balpy-0.0.0a9/balpy/artifacts/goerli/Authorizer.json
+-rw-r--r--   0 gerg       (506) staff       (20)   236033 2021-05-28 17:03:35.000000 balpy-0.0.0a9/balpy/artifacts/goerli/BalancerHelpers.json
+-rw-r--r--   0 gerg       (506) staff       (20)    16269 2021-05-28 17:03:35.000000 balpy-0.0.0a9/balpy/artifacts/goerli/Multicall.json
+-rw-r--r--   0 gerg       (506) staff       (20)    93102 2021-05-28 17:03:35.000000 balpy-0.0.0a9/balpy/artifacts/goerli/TokenFactory.json
+-rw-r--r--   0 gerg       (506) staff       (20)   135105 2021-05-28 17:03:35.000000 balpy-0.0.0a9/balpy/artifacts/goerli/Vault.json
+-rw-r--r--   0 gerg       (506) staff       (20)    82570 2021-05-28 17:03:35.000000 balpy-0.0.0a9/balpy/artifacts/goerli/WETH.json
+-rw-rw-r--   0 gerg       (506) staff       (20)   101844 2021-06-16 19:59:47.000000 balpy-0.0.0a9/balpy/artifacts/goerli/WeightedPool2TokensFactory.json
+-rw-r--r--   0 gerg       (506) staff       (20)   102115 2021-05-28 17:03:35.000000 balpy-0.0.0a9/balpy/artifacts/goerli/WeightedPoolFactory.json
+drwxr-xr-x   0 gerg       (506) staff       (20)        0 2021-07-02 20:52:15.779188 balpy-0.0.0a9/balpy/artifacts/kovan/
+-rw-r--r--   0 gerg       (506) staff       (20)    72280 2021-05-28 17:03:34.000000 balpy-0.0.0a9/balpy/artifacts/kovan/Authorizer.json
+-rw-r--r--   0 gerg       (506) staff       (20)   236032 2021-05-28 17:03:35.000000 balpy-0.0.0a9/balpy/artifacts/kovan/BalancerHelpers.json
+-rw-r--r--   0 gerg       (506) staff       (20)    16268 2021-05-28 17:03:35.000000 balpy-0.0.0a9/balpy/artifacts/kovan/Multicall.json
+-rw-rw-r--   0 gerg       (506) staff       (20)    93591 2021-06-16 19:59:47.000000 balpy-0.0.0a9/balpy/artifacts/kovan/StablePoolFactory.json
+-rw-r--r--   0 gerg       (506) staff       (20)    93102 2021-05-28 17:03:35.000000 balpy-0.0.0a9/balpy/artifacts/kovan/TokenFactory.json
+-rw-r--r--   0 gerg       (506) staff       (20)   135104 2021-05-28 17:03:34.000000 balpy-0.0.0a9/balpy/artifacts/kovan/Vault.json
+-rw-r--r--   0 gerg       (506) staff       (20)    82568 2021-05-28 17:03:35.000000 balpy-0.0.0a9/balpy/artifacts/kovan/WETH.json
+-rw-rw-r--   0 gerg       (506) staff       (20)   101844 2021-06-16 19:59:47.000000 balpy-0.0.0a9/balpy/artifacts/kovan/WeightedPool2TokensFactory.json
+-rw-r--r--   0 gerg       (506) staff       (20)   102115 2021-05-28 17:03:35.000000 balpy-0.0.0a9/balpy/artifacts/kovan/WeightedPoolFactory.json
+drwxr-xr-x   0 gerg       (506) staff       (20)        0 2021-07-02 20:52:15.805989 balpy-0.0.0a9/balpy/artifacts/mainnet/
+-rw-r--r--   0 gerg       (506) staff       (20)    72284 2021-05-28 17:03:35.000000 balpy-0.0.0a9/balpy/artifacts/mainnet/Authorizer.json
+-rw-r--r--   0 gerg       (506) staff       (20)   236034 2021-05-28 17:03:35.000000 balpy-0.0.0a9/balpy/artifacts/mainnet/BalancerHelpers.json
+-rw-r--r--   0 gerg       (506) staff       (20)    16270 2021-05-28 17:03:35.000000 balpy-0.0.0a9/balpy/artifacts/mainnet/Multicall.json
+-rw-r--r--   0 gerg       (506) staff       (20)    93591 2021-06-18 14:32:48.000000 balpy-0.0.0a9/balpy/artifacts/mainnet/StablePoolFactory.json
+-rw-r--r--   0 gerg       (506) staff       (20)    93103 2021-05-28 17:03:35.000000 balpy-0.0.0a9/balpy/artifacts/mainnet/TokenFactory.json
+-rw-r--r--   0 gerg       (506) staff       (20)   135106 2021-05-28 17:03:35.000000 balpy-0.0.0a9/balpy/artifacts/mainnet/Vault.json
+-rw-r--r--   0 gerg       (506) staff       (20)    82568 2021-05-28 17:03:35.000000 balpy-0.0.0a9/balpy/artifacts/mainnet/WETH.json
+-rw-rw-r--   0 gerg       (506) staff       (20)   101846 2021-06-16 19:59:47.000000 balpy-0.0.0a9/balpy/artifacts/mainnet/WeightedPool2TokensFactory.json
+-rw-r--r--   0 gerg       (506) staff       (20)   102116 2021-05-28 17:03:35.000000 balpy-0.0.0a9/balpy/artifacts/mainnet/WeightedPoolFactory.json
+drwxr-xr-x   0 gerg       (506) staff       (20)        0 2021-07-02 20:52:15.838485 balpy-0.0.0a9/balpy/artifacts/polygon/
+-rw-r--r--   0 gerg       (506) staff       (20)    72284 2021-06-18 14:27:48.000000 balpy-0.0.0a9/balpy/artifacts/polygon/Authorizer.json
+-rw-r--r--   0 gerg       (506) staff       (20)   236034 2021-06-18 14:27:48.000000 balpy-0.0.0a9/balpy/artifacts/polygon/BalancerHelpers.json
+-rw-r--r--   0 gerg       (506) staff       (20)    16270 2021-06-18 14:27:48.000000 balpy-0.0.0a9/balpy/artifacts/polygon/Multicall.json
+-rw-r--r--   0 gerg       (506) staff       (20)    93591 2021-06-18 14:32:54.000000 balpy-0.0.0a9/balpy/artifacts/polygon/StablePoolFactory.json
+-rw-r--r--   0 gerg       (506) staff       (20)    93103 2021-06-18 14:27:48.000000 balpy-0.0.0a9/balpy/artifacts/polygon/TokenFactory.json
+-rw-r--r--   0 gerg       (506) staff       (20)   135106 2021-06-18 14:27:48.000000 balpy-0.0.0a9/balpy/artifacts/polygon/Vault.json
+-rw-r--r--   0 gerg       (506) staff       (20)    82568 2021-06-18 14:27:48.000000 balpy-0.0.0a9/balpy/artifacts/polygon/WETH.json
+-rw-r--r--   0 gerg       (506) staff       (20)   101846 2021-06-18 14:27:48.000000 balpy-0.0.0a9/balpy/artifacts/polygon/WeightedPool2TokensFactory.json
+-rw-r--r--   0 gerg       (506) staff       (20)   102116 2021-06-18 14:27:48.000000 balpy-0.0.0a9/balpy/artifacts/polygon/WeightedPoolFactory.json
+drwxr-xr-x   0 gerg       (506) staff       (20)        0 2021-07-02 20:52:15.862416 balpy-0.0.0a9/balpy/artifacts/rinkeby/
+-rw-r--r--   0 gerg       (506) staff       (20)    72282 2021-05-28 17:03:33.000000 balpy-0.0.0a9/balpy/artifacts/rinkeby/Authorizer.json
+-rw-r--r--   0 gerg       (506) staff       (20)   236032 2021-05-28 17:03:33.000000 balpy-0.0.0a9/balpy/artifacts/rinkeby/BalancerHelpers.json
+-rw-r--r--   0 gerg       (506) staff       (20)    16268 2021-05-28 17:03:33.000000 balpy-0.0.0a9/balpy/artifacts/rinkeby/Multicall.json
+-rw-r--r--   0 gerg       (506) staff       (20)    93101 2021-05-28 17:03:33.000000 balpy-0.0.0a9/balpy/artifacts/rinkeby/TokenFactory.json
+-rw-r--r--   0 gerg       (506) staff       (20)   135105 2021-05-28 17:03:33.000000 balpy-0.0.0a9/balpy/artifacts/rinkeby/Vault.json
+-rw-r--r--   0 gerg       (506) staff       (20)    82565 2021-05-28 17:03:33.000000 balpy-0.0.0a9/balpy/artifacts/rinkeby/WETH.json
+-rw-rw-r--   0 gerg       (506) staff       (20)   101844 2021-06-16 19:59:47.000000 balpy-0.0.0a9/balpy/artifacts/rinkeby/WeightedPool2TokensFactory.json
+-rw-r--r--   0 gerg       (506) staff       (20)   102115 2021-05-28 17:03:33.000000 balpy-0.0.0a9/balpy/artifacts/rinkeby/WeightedPoolFactory.json
+drwxr-xr-x   0 gerg       (506) staff       (20)        0 2021-07-02 20:52:15.887470 balpy-0.0.0a9/balpy/artifacts/ropsten/
+-rw-r--r--   0 gerg       (506) staff       (20)    72281 2021-05-28 17:03:33.000000 balpy-0.0.0a9/balpy/artifacts/ropsten/Authorizer.json
+-rw-r--r--   0 gerg       (506) staff       (20)   236032 2021-05-28 17:03:33.000000 balpy-0.0.0a9/balpy/artifacts/ropsten/BalancerHelpers.json
+-rw-r--r--   0 gerg       (506) staff       (20)    16269 2021-05-28 17:03:33.000000 balpy-0.0.0a9/balpy/artifacts/ropsten/Multicall.json
+-rw-r--r--   0 gerg       (506) staff       (20)    93102 2021-05-28 17:03:33.000000 balpy-0.0.0a9/balpy/artifacts/ropsten/TokenFactory.json
+-rw-r--r--   0 gerg       (506) staff       (20)   135104 2021-05-28 17:03:33.000000 balpy-0.0.0a9/balpy/artifacts/ropsten/Vault.json
+-rw-r--r--   0 gerg       (506) staff       (20)    82568 2021-05-28 17:03:33.000000 balpy-0.0.0a9/balpy/artifacts/ropsten/WETH.json
+-rw-rw-r--   0 gerg       (506) staff       (20)   101844 2021-06-16 19:59:47.000000 balpy-0.0.0a9/balpy/artifacts/ropsten/WeightedPool2TokensFactory.json
+-rw-r--r--   0 gerg       (506) staff       (20)   102115 2021-05-28 17:03:33.000000 balpy-0.0.0a9/balpy/artifacts/ropsten/WeightedPoolFactory.json
+-rw-r--r--   0 gerg       (506) staff       (20)    29444 2021-07-02 20:49:31.000000 balpy-0.0.0a9/balpy/balpy.py
+drwxr-xr-x   0 gerg       (506) staff       (20)        0 2021-07-02 20:52:15.722715 balpy-0.0.0a9/balpy.egg-info/
+-rw-r--r--   0 gerg       (506) staff       (20)     1791 2021-07-02 20:52:15.000000 balpy-0.0.0a9/balpy.egg-info/PKG-INFO
+-rw-r--r--   0 gerg       (506) staff       (20)     2719 2021-07-02 20:52:15.000000 balpy-0.0.0a9/balpy.egg-info/SOURCES.txt
+-rw-r--r--   0 gerg       (506) staff       (20)        1 2021-07-02 20:52:15.000000 balpy-0.0.0a9/balpy.egg-info/dependency_links.txt
+-rw-r--r--   0 gerg       (506) staff       (20)       45 2021-07-02 20:52:15.000000 balpy-0.0.0a9/balpy.egg-info/requires.txt
+-rw-r--r--   0 gerg       (506) staff       (20)        6 2021-07-02 20:52:15.000000 balpy-0.0.0a9/balpy.egg-info/top_level.txt
+-rw-r--r--   0 gerg       (506) staff       (20)      103 2021-06-10 14:59:49.000000 balpy-0.0.0a9/pyproject.toml
+-rw-r--r--   0 gerg       (506) staff       (20)      637 2021-07-02 20:52:15.891117 balpy-0.0.0a9/setup.cfg
```

### Comparing `balpy-0.0.0a82/LICENSE` & `balpy-0.0.0a9/LICENSE`

 * *Files identical despite different names*

### Comparing `balpy-0.0.0a82/balpy/abi/ERC20.json` & `balpy-0.0.0a9/balpy/abi/ERC20.json`

 * *Files identical despite different names*

### Comparing `balpy-0.0.0a82/balpy/deployments/20210418-authorizer/abi/Authorizer.json` & `balpy-0.0.0a9/balpy/abi/BalancerPoolToken.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6174836601307189%*

 * *Differences: {'0': "{'inputs': {1: {'internalType': 'string', 'name': 'tokenSymbol', 'type': 'string'}, insert: "*

 * *      "[(0, OrderedDict([('internalType', 'string'), ('name', 'tokenName'), ('type', "*

 * *      "'string')]))]}}",*

 * * '1': "{'inputs': {0: {'internalType': 'address', 'name': 'owner', 'type': 'address'}, 1: {'name': "*

 * *      "'spender'}, 2: {'indexed': False, 'internalType': 'uint256', 'name': 'value', 'type': "*

 * *      "'uint256'}}, 'name': 'Approval'}",*

 * * '10': "{'inputs': [], 'name': 'symbol', 'outputs': [OrderedD […]*

```diff
@@ -1,342 +1,288 @@
 [
     {
         "inputs": [
             {
-                "internalType": "address",
-                "name": "admin",
-                "type": "address"
+                "internalType": "string",
+                "name": "tokenName",
+                "type": "string"
+            },
+            {
+                "internalType": "string",
+                "name": "tokenSymbol",
+                "type": "string"
             }
         ],
         "stateMutability": "nonpayable",
         "type": "constructor"
     },
     {
         "anonymous": false,
         "inputs": [
             {
                 "indexed": true,
-                "internalType": "bytes32",
-                "name": "role",
-                "type": "bytes32"
+                "internalType": "address",
+                "name": "owner",
+                "type": "address"
             },
             {
                 "indexed": true,
-                "internalType": "bytes32",
-                "name": "previousAdminRole",
-                "type": "bytes32"
+                "internalType": "address",
+                "name": "spender",
+                "type": "address"
             },
             {
-                "indexed": true,
-                "internalType": "bytes32",
-                "name": "newAdminRole",
-                "type": "bytes32"
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "value",
+                "type": "uint256"
             }
         ],
-        "name": "RoleAdminChanged",
+        "name": "Approval",
         "type": "event"
     },
     {
         "anonymous": false,
         "inputs": [
             {
                 "indexed": true,
-                "internalType": "bytes32",
-                "name": "role",
-                "type": "bytes32"
-            },
-            {
-                "indexed": true,
                 "internalType": "address",
-                "name": "account",
+                "name": "from",
                 "type": "address"
             },
             {
                 "indexed": true,
                 "internalType": "address",
-                "name": "sender",
+                "name": "to",
                 "type": "address"
+            },
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "value",
+                "type": "uint256"
             }
         ],
-        "name": "RoleGranted",
+        "name": "Transfer",
         "type": "event"
     },
     {
-        "anonymous": false,
         "inputs": [
             {
-                "indexed": true,
-                "internalType": "bytes32",
-                "name": "role",
-                "type": "bytes32"
-            },
-            {
-                "indexed": true,
                 "internalType": "address",
-                "name": "account",
+                "name": "owner",
                 "type": "address"
             },
             {
-                "indexed": true,
                 "internalType": "address",
-                "name": "sender",
+                "name": "spender",
                 "type": "address"
             }
         ],
-        "name": "RoleRevoked",
-        "type": "event"
-    },
-    {
-        "inputs": [],
-        "name": "DEFAULT_ADMIN_ROLE",
+        "name": "allowance",
         "outputs": [
             {
-                "internalType": "bytes32",
+                "internalType": "uint256",
                 "name": "",
-                "type": "bytes32"
+                "type": "uint256"
             }
         ],
         "stateMutability": "view",
         "type": "function"
     },
     {
         "inputs": [
             {
-                "internalType": "bytes32",
-                "name": "actionId",
-                "type": "bytes32"
-            },
-            {
                 "internalType": "address",
-                "name": "account",
+                "name": "spender",
                 "type": "address"
             },
             {
-                "internalType": "address",
-                "name": "",
-                "type": "address"
+                "internalType": "uint256",
+                "name": "amount",
+                "type": "uint256"
             }
         ],
-        "name": "canPerform",
+        "name": "approve",
         "outputs": [
             {
                 "internalType": "bool",
                 "name": "",
                 "type": "bool"
             }
         ],
-        "stateMutability": "view",
+        "stateMutability": "nonpayable",
         "type": "function"
     },
     {
         "inputs": [
             {
-                "internalType": "bytes32",
-                "name": "role",
-                "type": "bytes32"
+                "internalType": "address",
+                "name": "account",
+                "type": "address"
             }
         ],
-        "name": "getRoleAdmin",
+        "name": "balanceOf",
         "outputs": [
             {
-                "internalType": "bytes32",
+                "internalType": "uint256",
                 "name": "",
-                "type": "bytes32"
+                "type": "uint256"
             }
         ],
         "stateMutability": "view",
         "type": "function"
     },
     {
+        "inputs": [],
+        "name": "decimals",
+        "outputs": [
+            {
+                "internalType": "uint8",
+                "name": "",
+                "type": "uint8"
+            }
+        ],
+        "stateMutability": "pure",
+        "type": "function"
+    },
+    {
         "inputs": [
             {
-                "internalType": "bytes32",
-                "name": "role",
-                "type": "bytes32"
+                "internalType": "address",
+                "name": "spender",
+                "type": "address"
             },
             {
                 "internalType": "uint256",
-                "name": "index",
+                "name": "amount",
                 "type": "uint256"
             }
         ],
-        "name": "getRoleMember",
+        "name": "decreaseApproval",
         "outputs": [
             {
-                "internalType": "address",
+                "internalType": "bool",
                 "name": "",
-                "type": "address"
+                "type": "bool"
             }
         ],
-        "stateMutability": "view",
+        "stateMutability": "nonpayable",
         "type": "function"
     },
     {
         "inputs": [
             {
-                "internalType": "bytes32",
-                "name": "role",
-                "type": "bytes32"
+                "internalType": "address",
+                "name": "spender",
+                "type": "address"
+            },
+            {
+                "internalType": "uint256",
+                "name": "amount",
+                "type": "uint256"
             }
         ],
-        "name": "getRoleMemberCount",
+        "name": "increaseApproval",
         "outputs": [
             {
-                "internalType": "uint256",
+                "internalType": "bool",
                 "name": "",
-                "type": "uint256"
+                "type": "bool"
             }
         ],
-        "stateMutability": "view",
+        "stateMutability": "nonpayable",
         "type": "function"
     },
     {
-        "inputs": [
-            {
-                "internalType": "bytes32",
-                "name": "role",
-                "type": "bytes32"
-            },
+        "inputs": [],
+        "name": "name",
+        "outputs": [
             {
-                "internalType": "address",
-                "name": "account",
-                "type": "address"
+                "internalType": "string",
+                "name": "",
+                "type": "string"
             }
         ],
-        "name": "grantRole",
-        "outputs": [],
-        "stateMutability": "nonpayable",
+        "stateMutability": "view",
         "type": "function"
     },
     {
-        "inputs": [
-            {
-                "internalType": "bytes32[]",
-                "name": "roles",
-                "type": "bytes32[]"
-            },
+        "inputs": [],
+        "name": "symbol",
+        "outputs": [
             {
-                "internalType": "address",
-                "name": "account",
-                "type": "address"
+                "internalType": "string",
+                "name": "",
+                "type": "string"
             }
         ],
-        "name": "grantRoles",
-        "outputs": [],
-        "stateMutability": "nonpayable",
+        "stateMutability": "view",
         "type": "function"
     },
     {
-        "inputs": [
-            {
-                "internalType": "bytes32[]",
-                "name": "roles",
-                "type": "bytes32[]"
-            },
+        "inputs": [],
+        "name": "totalSupply",
+        "outputs": [
             {
-                "internalType": "address[]",
-                "name": "accounts",
-                "type": "address[]"
+                "internalType": "uint256",
+                "name": "",
+                "type": "uint256"
             }
         ],
-        "name": "grantRolesToMany",
-        "outputs": [],
-        "stateMutability": "nonpayable",
+        "stateMutability": "view",
         "type": "function"
     },
     {
         "inputs": [
             {
-                "internalType": "bytes32",
-                "name": "role",
-                "type": "bytes32"
-            },
-            {
                 "internalType": "address",
-                "name": "account",
+                "name": "recipient",
                 "type": "address"
+            },
+            {
+                "internalType": "uint256",
+                "name": "amount",
+                "type": "uint256"
             }
         ],
-        "name": "hasRole",
+        "name": "transfer",
         "outputs": [
             {
                 "internalType": "bool",
                 "name": "",
                 "type": "bool"
             }
         ],
-        "stateMutability": "view",
+        "stateMutability": "nonpayable",
         "type": "function"
     },
     {
         "inputs": [
             {
-                "internalType": "bytes32",
-                "name": "role",
-                "type": "bytes32"
-            },
-            {
                 "internalType": "address",
-                "name": "account",
+                "name": "sender",
                 "type": "address"
-            }
-        ],
-        "name": "renounceRole",
-        "outputs": [],
-        "stateMutability": "nonpayable",
-        "type": "function"
-    },
-    {
-        "inputs": [
-            {
-                "internalType": "bytes32",
-                "name": "role",
-                "type": "bytes32"
             },
             {
                 "internalType": "address",
-                "name": "account",
+                "name": "recipient",
                 "type": "address"
-            }
-        ],
-        "name": "revokeRole",
-        "outputs": [],
-        "stateMutability": "nonpayable",
-        "type": "function"
-    },
-    {
-        "inputs": [
-            {
-                "internalType": "bytes32[]",
-                "name": "roles",
-                "type": "bytes32[]"
             },
             {
-                "internalType": "address",
-                "name": "account",
-                "type": "address"
+                "internalType": "uint256",
+                "name": "amount",
+                "type": "uint256"
             }
         ],
-        "name": "revokeRoles",
-        "outputs": [],
-        "stateMutability": "nonpayable",
-        "type": "function"
-    },
-    {
-        "inputs": [
-            {
-                "internalType": "bytes32[]",
-                "name": "roles",
-                "type": "bytes32[]"
-            },
+        "name": "transferFrom",
+        "outputs": [
             {
-                "internalType": "address[]",
-                "name": "accounts",
-                "type": "address[]"
+                "internalType": "bool",
+                "name": "",
+                "type": "bool"
             }
         ],
-        "name": "revokeRolesFromMany",
-        "outputs": [],
         "stateMutability": "nonpayable",
         "type": "function"
     }
 ]
```

### Comparing `balpy-0.0.0a82/balpy/deployments/20210418-vault/abi/BalancerHelpers.json` & `balpy-0.0.0a9/balpy/abi/BalancerHelpers.json`

 * *Files identical despite different names*

### Comparing `balpy-0.0.0a82/balpy/deployments/20210418-vault/abi/Vault.json` & `balpy-0.0.0a9/balpy/abi/Vault.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9974999999999999%*

 * *Differences: {'32': "{'stateMutability': 'view'}"}*

```diff
@@ -986,15 +986,15 @@
         "outputs": [
             {
                 "internalType": "int256[]",
                 "name": "",
                 "type": "int256[]"
             }
         ],
-        "stateMutability": "nonpayable",
+        "stateMutability": "view",
         "type": "function"
     },
     {
         "inputs": [
             {
                 "internalType": "enum IVault.PoolSpecialization",
                 "name": "specialization",
```

### Comparing `balpy-0.0.0a82/balpy/deployments/20210418-weighted-pool/abi/WeightedPool.json` & `balpy-0.0.0a9/balpy/abi/WeightedPool.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9945945945945945%*

 * *Differences: {'29': "{'stateMutability': 'view'}", '30': "{'stateMutability': 'view'}"}*

```diff
@@ -732,15 +732,15 @@
             },
             {
                 "internalType": "uint256[]",
                 "name": "amountsOut",
                 "type": "uint256[]"
             }
         ],
-        "stateMutability": "nonpayable",
+        "stateMutability": "view",
         "type": "function"
     },
     {
         "inputs": [
             {
                 "internalType": "bytes32",
                 "name": "poolId",
@@ -786,15 +786,15 @@
             },
             {
                 "internalType": "uint256[]",
                 "name": "amountsIn",
                 "type": "uint256[]"
             }
         ],
-        "stateMutability": "nonpayable",
+        "stateMutability": "view",
         "type": "function"
     },
     {
         "inputs": [
             {
                 "internalType": "bool",
                 "name": "paused",
```

### Comparing `balpy-0.0.0a82/balpy/deployments/20210418-weighted-pool/abi/WeightedPool2Tokens.json` & `balpy-0.0.0a9/balpy/abi/StablePool.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6200217103749711%*

 * *Differences: {'0': "{'inputs': {7: {'internalType': 'uint256', 'name': 'emergencyPeriodCheckExtension', 'type': "*

 * *      "'uint256', delete: ['components']}, insert: [(0, OrderedDict([('internalType', 'contract "*

 * *      "IVault'), ('name', 'vault'), ('type', 'address')])), (1, OrderedDict([('internalType', "*

 * *      "'string'), ('name', 'name'), ('type', 'string')])), (2, OrderedDict([('internalType', "*

 * *      "'string'), ('name', 'symbol'), ('type', 'string')])), (3, OrderedDict([('internalType', "*

 * *      "'contract IERC20[] […]*

```diff
@@ -1,76 +1,49 @@
 [
     {
         "inputs": [
             {
-                "components": [
-                    {
-                        "internalType": "contract IVault",
-                        "name": "vault",
-                        "type": "address"
-                    },
-                    {
-                        "internalType": "string",
-                        "name": "name",
-                        "type": "string"
-                    },
-                    {
-                        "internalType": "string",
-                        "name": "symbol",
-                        "type": "string"
-                    },
-                    {
-                        "internalType": "contract IERC20",
-                        "name": "token0",
-                        "type": "address"
-                    },
-                    {
-                        "internalType": "contract IERC20",
-                        "name": "token1",
-                        "type": "address"
-                    },
-                    {
-                        "internalType": "uint256",
-                        "name": "normalizedWeight0",
-                        "type": "uint256"
-                    },
-                    {
-                        "internalType": "uint256",
-                        "name": "normalizedWeight1",
-                        "type": "uint256"
-                    },
-                    {
-                        "internalType": "uint256",
-                        "name": "swapFeePercentage",
-                        "type": "uint256"
-                    },
-                    {
-                        "internalType": "uint256",
-                        "name": "pauseWindowDuration",
-                        "type": "uint256"
-                    },
-                    {
-                        "internalType": "uint256",
-                        "name": "bufferPeriodDuration",
-                        "type": "uint256"
-                    },
-                    {
-                        "internalType": "bool",
-                        "name": "oracleEnabled",
-                        "type": "bool"
-                    },
-                    {
-                        "internalType": "address",
-                        "name": "owner",
-                        "type": "address"
-                    }
-                ],
-                "internalType": "struct WeightedPool2Tokens.NewPoolParams",
-                "name": "params",
-                "type": "tuple"
+                "internalType": "contract IVault",
+                "name": "vault",
+                "type": "address"
+            },
+            {
+                "internalType": "string",
+                "name": "name",
+                "type": "string"
+            },
+            {
+                "internalType": "string",
+                "name": "symbol",
+                "type": "string"
+            },
+            {
+                "internalType": "contract IERC20[]",
+                "name": "tokens",
+                "type": "address[]"
+            },
+            {
+                "internalType": "uint256",
+                "name": "amplificationParameter",
+                "type": "uint256"
+            },
+            {
+                "internalType": "uint256",
+                "name": "swapFee",
+                "type": "uint256"
+            },
+            {
+                "internalType": "uint256",
+                "name": "emergencyPeriod",
+                "type": "uint256"
+            },
+            {
+                "internalType": "uint256",
+                "name": "emergencyPeriodCheckExtension",
+                "type": "uint256"
             }
         ],
         "stateMutability": "nonpayable",
         "type": "constructor"
     },
     {
         "anonymous": false,
@@ -99,45 +72,32 @@
     },
     {
         "anonymous": false,
         "inputs": [
             {
                 "indexed": false,
                 "internalType": "bool",
-                "name": "enabled",
-                "type": "bool"
-            }
-        ],
-        "name": "OracleEnabledChanged",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "bool",
-                "name": "paused",
+                "name": "active",
                 "type": "bool"
             }
         ],
-        "name": "PausedStateChanged",
+        "name": "EmergencyPeriodChanged",
         "type": "event"
     },
     {
         "anonymous": false,
         "inputs": [
             {
                 "indexed": false,
                 "internalType": "uint256",
-                "name": "swapFeePercentage",
+                "name": "swapFee",
                 "type": "uint256"
             }
         ],
-        "name": "SwapFeePercentageChanged",
+        "name": "SwapFeeChanged",
         "type": "event"
     },
     {
         "anonymous": false,
         "inputs": [
             {
                 "indexed": true,
@@ -158,27 +118,14 @@
                 "type": "uint256"
             }
         ],
         "name": "Transfer",
         "type": "event"
     },
     {
-        "inputs": [],
-        "name": "DOMAIN_SEPARATOR",
-        "outputs": [
-            {
-                "internalType": "bytes32",
-                "name": "",
-                "type": "bytes32"
-            }
-        ],
-        "stateMutability": "view",
-        "type": "function"
-    },
-    {
         "inputs": [
             {
                 "internalType": "address",
                 "name": "owner",
                 "type": "address"
             },
             {
@@ -276,221 +223,55 @@
             }
         ],
         "stateMutability": "nonpayable",
         "type": "function"
     },
     {
         "inputs": [],
-        "name": "enableOracle",
-        "outputs": [],
-        "stateMutability": "nonpayable",
-        "type": "function"
-    },
-    {
-        "inputs": [
-            {
-                "internalType": "bytes4",
-                "name": "selector",
-                "type": "bytes4"
-            }
-        ],
-        "name": "getActionId",
-        "outputs": [
-            {
-                "internalType": "bytes32",
-                "name": "",
-                "type": "bytes32"
-            }
-        ],
-        "stateMutability": "view",
-        "type": "function"
-    },
-    {
-        "inputs": [],
-        "name": "getAuthorizer",
-        "outputs": [
-            {
-                "internalType": "contract IAuthorizer",
-                "name": "",
-                "type": "address"
-            }
-        ],
-        "stateMutability": "view",
-        "type": "function"
-    },
-    {
-        "inputs": [],
-        "name": "getInvariant",
+        "name": "getAmplificationParameter",
         "outputs": [
             {
                 "internalType": "uint256",
                 "name": "",
                 "type": "uint256"
             }
         ],
         "stateMutability": "view",
         "type": "function"
     },
     {
         "inputs": [],
-        "name": "getLargestSafeQueryWindow",
-        "outputs": [
-            {
-                "internalType": "uint256",
-                "name": "",
-                "type": "uint256"
-            }
-        ],
-        "stateMutability": "pure",
-        "type": "function"
-    },
-    {
-        "inputs": [],
-        "name": "getLastInvariant",
-        "outputs": [
-            {
-                "internalType": "uint256",
-                "name": "",
-                "type": "uint256"
-            }
-        ],
-        "stateMutability": "view",
-        "type": "function"
-    },
-    {
-        "inputs": [
-            {
-                "internalType": "enum IPriceOracle.Variable",
-                "name": "variable",
-                "type": "uint8"
-            }
-        ],
-        "name": "getLatest",
-        "outputs": [
-            {
-                "internalType": "uint256",
-                "name": "",
-                "type": "uint256"
-            }
-        ],
-        "stateMutability": "view",
-        "type": "function"
-    },
-    {
-        "inputs": [],
-        "name": "getMiscData",
-        "outputs": [
-            {
-                "internalType": "int256",
-                "name": "logInvariant",
-                "type": "int256"
-            },
-            {
-                "internalType": "int256",
-                "name": "logTotalSupply",
-                "type": "int256"
-            },
-            {
-                "internalType": "uint256",
-                "name": "oracleSampleCreationTimestamp",
-                "type": "uint256"
-            },
-            {
-                "internalType": "uint256",
-                "name": "oracleIndex",
-                "type": "uint256"
-            },
-            {
-                "internalType": "bool",
-                "name": "oracleEnabled",
-                "type": "bool"
-            },
-            {
-                "internalType": "uint256",
-                "name": "swapFeePercentage",
-                "type": "uint256"
-            }
-        ],
-        "stateMutability": "view",
-        "type": "function"
-    },
-    {
-        "inputs": [],
-        "name": "getNormalizedWeights",
-        "outputs": [
-            {
-                "internalType": "uint256[]",
-                "name": "",
-                "type": "uint256[]"
-            }
-        ],
-        "stateMutability": "view",
-        "type": "function"
-    },
-    {
-        "inputs": [],
-        "name": "getOwner",
+        "name": "getAuthorizer",
         "outputs": [
             {
-                "internalType": "address",
+                "internalType": "contract IAuthorizer",
                 "name": "",
                 "type": "address"
             }
         ],
         "stateMutability": "view",
         "type": "function"
     },
     {
-        "inputs": [
-            {
-                "components": [
-                    {
-                        "internalType": "enum IPriceOracle.Variable",
-                        "name": "variable",
-                        "type": "uint8"
-                    },
-                    {
-                        "internalType": "uint256",
-                        "name": "ago",
-                        "type": "uint256"
-                    }
-                ],
-                "internalType": "struct IPriceOracle.OracleAccumulatorQuery[]",
-                "name": "queries",
-                "type": "tuple[]"
-            }
-        ],
-        "name": "getPastAccumulators",
-        "outputs": [
-            {
-                "internalType": "int256[]",
-                "name": "results",
-                "type": "int256[]"
-            }
-        ],
-        "stateMutability": "view",
-        "type": "function"
-    },
-    {
         "inputs": [],
-        "name": "getPausedState",
+        "name": "getEmergencyPeriod",
         "outputs": [
             {
                 "internalType": "bool",
-                "name": "paused",
+                "name": "active",
                 "type": "bool"
             },
             {
                 "internalType": "uint256",
-                "name": "pauseWindowEndTime",
+                "name": "endDate",
                 "type": "uint256"
             },
             {
                 "internalType": "uint256",
-                "name": "bufferPeriodEndTime",
+                "name": "checkEndDate",
                 "type": "uint256"
             }
         ],
         "stateMutability": "view",
         "type": "function"
     },
     {
@@ -516,125 +297,27 @@
                 "type": "uint256"
             }
         ],
         "stateMutability": "view",
         "type": "function"
     },
     {
-        "inputs": [
-            {
-                "internalType": "uint256",
-                "name": "index",
-                "type": "uint256"
-            }
-        ],
-        "name": "getSample",
-        "outputs": [
-            {
-                "internalType": "int256",
-                "name": "logPairPrice",
-                "type": "int256"
-            },
-            {
-                "internalType": "int256",
-                "name": "accLogPairPrice",
-                "type": "int256"
-            },
-            {
-                "internalType": "int256",
-                "name": "logBptPrice",
-                "type": "int256"
-            },
-            {
-                "internalType": "int256",
-                "name": "accLogBptPrice",
-                "type": "int256"
-            },
-            {
-                "internalType": "int256",
-                "name": "logInvariant",
-                "type": "int256"
-            },
-            {
-                "internalType": "int256",
-                "name": "accLogInvariant",
-                "type": "int256"
-            },
-            {
-                "internalType": "uint256",
-                "name": "timestamp",
-                "type": "uint256"
-            }
-        ],
-        "stateMutability": "view",
-        "type": "function"
-    },
-    {
         "inputs": [],
-        "name": "getSwapFeePercentage",
+        "name": "getSwapFee",
         "outputs": [
             {
                 "internalType": "uint256",
                 "name": "",
                 "type": "uint256"
             }
         ],
         "stateMutability": "view",
         "type": "function"
     },
     {
-        "inputs": [
-            {
-                "components": [
-                    {
-                        "internalType": "enum IPriceOracle.Variable",
-                        "name": "variable",
-                        "type": "uint8"
-                    },
-                    {
-                        "internalType": "uint256",
-                        "name": "secs",
-                        "type": "uint256"
-                    },
-                    {
-                        "internalType": "uint256",
-                        "name": "ago",
-                        "type": "uint256"
-                    }
-                ],
-                "internalType": "struct IPriceOracle.OracleAverageQuery[]",
-                "name": "queries",
-                "type": "tuple[]"
-            }
-        ],
-        "name": "getTimeWeightedAverage",
-        "outputs": [
-            {
-                "internalType": "uint256[]",
-                "name": "results",
-                "type": "uint256[]"
-            }
-        ],
-        "stateMutability": "view",
-        "type": "function"
-    },
-    {
-        "inputs": [],
-        "name": "getTotalSamples",
-        "outputs": [
-            {
-                "internalType": "uint256",
-                "name": "",
-                "type": "uint256"
-            }
-        ],
-        "stateMutability": "pure",
-        "type": "function"
-    },
-    {
         "inputs": [],
         "name": "getVault",
         "outputs": [
             {
                 "internalType": "contract IVault",
                 "name": "",
                 "type": "address"
@@ -679,33 +362,14 @@
         ],
         "stateMutability": "view",
         "type": "function"
     },
     {
         "inputs": [
             {
-                "internalType": "address",
-                "name": "owner",
-                "type": "address"
-            }
-        ],
-        "name": "nonces",
-        "outputs": [
-            {
-                "internalType": "uint256",
-                "name": "",
-                "type": "uint256"
-            }
-        ],
-        "stateMutability": "view",
-        "type": "function"
-    },
-    {
-        "inputs": [
-            {
                 "internalType": "bytes32",
                 "name": "poolId",
                 "type": "bytes32"
             },
             {
                 "internalType": "address",
                 "name": "sender",
@@ -714,20 +378,20 @@
             {
                 "internalType": "address",
                 "name": "recipient",
                 "type": "address"
             },
             {
                 "internalType": "uint256[]",
-                "name": "balances",
+                "name": "currentBalances",
                 "type": "uint256[]"
             },
             {
                 "internalType": "uint256",
-                "name": "lastChangeBlock",
+                "name": "latestBlockNumberUsed",
                 "type": "uint256"
             },
             {
                 "internalType": "uint256",
                 "name": "protocolSwapFeePercentage",
                 "type": "uint256"
             },
@@ -768,20 +432,20 @@
             {
                 "internalType": "address",
                 "name": "recipient",
                 "type": "address"
             },
             {
                 "internalType": "uint256[]",
-                "name": "balances",
+                "name": "currentBalances",
                 "type": "uint256[]"
             },
             {
                 "internalType": "uint256",
-                "name": "lastChangeBlock",
+                "name": "latestBlockNumberUsed",
                 "type": "uint256"
             },
             {
                 "internalType": "uint256",
                 "name": "protocolSwapFeePercentage",
                 "type": "uint256"
             },
@@ -791,20 +455,20 @@
                 "type": "bytes"
             }
         ],
         "name": "onJoinPool",
         "outputs": [
             {
                 "internalType": "uint256[]",
-                "name": "amountsIn",
+                "name": "",
                 "type": "uint256[]"
             },
             {
                 "internalType": "uint256[]",
-                "name": "dueProtocolFeeAmounts",
+                "name": "",
                 "type": "uint256[]"
             }
         ],
         "stateMutability": "nonpayable",
         "type": "function"
     },
     {
@@ -834,15 +498,15 @@
                     {
                         "internalType": "bytes32",
                         "name": "poolId",
                         "type": "bytes32"
                     },
                     {
                         "internalType": "uint256",
-                        "name": "lastChangeBlock",
+                        "name": "latestBlockNumberUsed",
                         "type": "uint256"
                     },
                     {
                         "internalType": "address",
                         "name": "from",
                         "type": "address"
                     },
@@ -854,80 +518,42 @@
                     {
                         "internalType": "bytes",
                         "name": "userData",
                         "type": "bytes"
                     }
                 ],
                 "internalType": "struct IPoolSwapStructs.SwapRequest",
-                "name": "request",
+                "name": "swapRequest",
                 "type": "tuple"
             },
             {
+                "internalType": "uint256[]",
+                "name": "balances",
+                "type": "uint256[]"
+            },
+            {
                 "internalType": "uint256",
-                "name": "balanceTokenIn",
+                "name": "indexIn",
                 "type": "uint256"
             },
             {
                 "internalType": "uint256",
-                "name": "balanceTokenOut",
+                "name": "indexOut",
                 "type": "uint256"
             }
         ],
         "name": "onSwap",
         "outputs": [
             {
                 "internalType": "uint256",
                 "name": "",
                 "type": "uint256"
             }
         ],
-        "stateMutability": "nonpayable",
-        "type": "function"
-    },
-    {
-        "inputs": [
-            {
-                "internalType": "address",
-                "name": "owner",
-                "type": "address"
-            },
-            {
-                "internalType": "address",
-                "name": "spender",
-                "type": "address"
-            },
-            {
-                "internalType": "uint256",
-                "name": "value",
-                "type": "uint256"
-            },
-            {
-                "internalType": "uint256",
-                "name": "deadline",
-                "type": "uint256"
-            },
-            {
-                "internalType": "uint8",
-                "name": "v",
-                "type": "uint8"
-            },
-            {
-                "internalType": "bytes32",
-                "name": "r",
-                "type": "bytes32"
-            },
-            {
-                "internalType": "bytes32",
-                "name": "s",
-                "type": "bytes32"
-            }
-        ],
-        "name": "permit",
-        "outputs": [],
-        "stateMutability": "nonpayable",
+        "stateMutability": "view",
         "type": "function"
     },
     {
         "inputs": [
             {
                 "internalType": "bytes32",
                 "name": "poolId",
@@ -941,20 +567,20 @@
             {
                 "internalType": "address",
                 "name": "recipient",
                 "type": "address"
             },
             {
                 "internalType": "uint256[]",
-                "name": "balances",
+                "name": "currentBalances",
                 "type": "uint256[]"
             },
             {
                 "internalType": "uint256",
-                "name": "lastChangeBlock",
+                "name": "latestBlockNumberUsed",
                 "type": "uint256"
             },
             {
                 "internalType": "uint256",
                 "name": "protocolSwapFeePercentage",
                 "type": "uint256"
             },
@@ -973,15 +599,15 @@
             },
             {
                 "internalType": "uint256[]",
                 "name": "amountsOut",
                 "type": "uint256[]"
             }
         ],
-        "stateMutability": "nonpayable",
+        "stateMutability": "view",
         "type": "function"
     },
     {
         "inputs": [
             {
                 "internalType": "bytes32",
                 "name": "poolId",
@@ -995,20 +621,20 @@
             {
                 "internalType": "address",
                 "name": "recipient",
                 "type": "address"
             },
             {
                 "internalType": "uint256[]",
-                "name": "balances",
+                "name": "currentBalances",
                 "type": "uint256[]"
             },
             {
                 "internalType": "uint256",
-                "name": "lastChangeBlock",
+                "name": "latestBlockNumberUsed",
                 "type": "uint256"
             },
             {
                 "internalType": "uint256",
                 "name": "protocolSwapFeePercentage",
                 "type": "uint256"
             },
@@ -1027,39 +653,39 @@
             },
             {
                 "internalType": "uint256[]",
                 "name": "amountsIn",
                 "type": "uint256[]"
             }
         ],
-        "stateMutability": "nonpayable",
+        "stateMutability": "view",
         "type": "function"
     },
     {
         "inputs": [
             {
                 "internalType": "bool",
-                "name": "paused",
+                "name": "active",
                 "type": "bool"
             }
         ],
-        "name": "setPaused",
+        "name": "setEmergencyPeriod",
         "outputs": [],
         "stateMutability": "nonpayable",
         "type": "function"
     },
     {
         "inputs": [
             {
                 "internalType": "uint256",
-                "name": "swapFeePercentage",
+                "name": "swapFee",
                 "type": "uint256"
             }
         ],
-        "name": "setSwapFeePercentage",
+        "name": "setSwapFee",
         "outputs": [],
         "stateMutability": "nonpayable",
         "type": "function"
     },
     {
         "inputs": [],
         "name": "symbol",
```

### Comparing `balpy-0.0.0a82/balpy/deployments/20210418-weighted-pool/abi/WeightedPool2TokensFactory.json` & `balpy-0.0.0a9/balpy/abi/WeightedPoolFactory.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6217592592592592%*

 * *Differences: {'0': "{'inputs': {0: {'name': '_vault'}}}",*

 * * '1': "{'name': 'PoolRegistered'}",*

 * * '2': "{'inputs': {4: {'name': 'swapFee'}, 5: {'internalType': 'uint256', 'name': "*

 * *      "'emergencyPeriod', 'type': 'uint256'}, 6: {'internalType': 'uint256', 'name': "*

 * *      "'emergencyPeriodCheckExtension', 'type': 'uint256'}}}",*

 * * '3': "{'name': 'vault'}",*

 * * 'delete': '[5, 3]'}*

```diff
@@ -1,13 +1,13 @@
 [
     {
         "inputs": [
             {
                 "internalType": "contract IVault",
-                "name": "vault",
+                "name": "_vault",
                 "type": "address"
             }
         ],
         "stateMutability": "nonpayable",
         "type": "constructor"
     },
     {
@@ -16,15 +16,15 @@
             {
                 "indexed": true,
                 "internalType": "address",
                 "name": "pool",
                 "type": "address"
             }
         ],
-        "name": "PoolCreated",
+        "name": "PoolRegistered",
         "type": "event"
     },
     {
         "inputs": [
             {
                 "internalType": "string",
                 "name": "name",
@@ -43,26 +43,26 @@
             {
                 "internalType": "uint256[]",
                 "name": "weights",
                 "type": "uint256[]"
             },
             {
                 "internalType": "uint256",
-                "name": "swapFeePercentage",
+                "name": "swapFee",
                 "type": "uint256"
             },
             {
-                "internalType": "bool",
-                "name": "oracleEnabled",
-                "type": "bool"
+                "internalType": "uint256",
+                "name": "emergencyPeriod",
+                "type": "uint256"
             },
             {
-                "internalType": "address",
-                "name": "owner",
-                "type": "address"
+                "internalType": "uint256",
+                "name": "emergencyPeriodCheckExtension",
+                "type": "uint256"
             }
         ],
         "name": "create",
         "outputs": [
             {
                 "internalType": "address",
                 "name": "",
@@ -70,56 +70,19 @@
             }
         ],
         "stateMutability": "nonpayable",
         "type": "function"
     },
     {
         "inputs": [],
-        "name": "getPauseConfiguration",
-        "outputs": [
-            {
-                "internalType": "uint256",
-                "name": "pauseWindowDuration",
-                "type": "uint256"
-            },
-            {
-                "internalType": "uint256",
-                "name": "bufferPeriodDuration",
-                "type": "uint256"
-            }
-        ],
-        "stateMutability": "view",
-        "type": "function"
-    },
-    {
-        "inputs": [],
-        "name": "getVault",
+        "name": "vault",
         "outputs": [
             {
                 "internalType": "contract IVault",
                 "name": "",
                 "type": "address"
             }
         ],
         "stateMutability": "view",
         "type": "function"
-    },
-    {
-        "inputs": [
-            {
-                "internalType": "address",
-                "name": "pool",
-                "type": "address"
-            }
-        ],
-        "name": "isPoolFromFactory",
-        "outputs": [
-            {
-                "internalType": "bool",
-                "name": "",
-                "type": "bool"
-            }
-        ],
-        "stateMutability": "view",
-        "type": "function"
     }
 ]
```

### Comparing `balpy-0.0.0a82/balpy/deployments/20210418-weighted-pool/abi/WeightedPoolFactory.json` & `balpy-0.0.0a9/balpy/abi/StablePoolFactory.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6193783068783069%*

 * *Differences: {'0': "{'inputs': {0: {'name': '_vault'}}}",*

 * * '1': "{'name': 'PoolRegistered'}",*

 * * '2': "{'inputs': {4: {'internalType': 'uint256', 'name': 'swapFee', 'type': 'uint256'}, 5: "*

 * *      "{'name': 'emergencyPeriod'}, 6: {'internalType': 'uint256', 'name': "*

 * *      "'emergencyPeriodCheckExtension', 'type': 'uint256'}, insert: [(3, "*

 * *      "OrderedDict([('internalType', 'uint256'), ('name', 'amplificationParameter'), ('type', "*

 * *      "'uint256')]))]}}",*

 * * '3': "{'name': 'vault'}",*

 * * 'delete': '[5, 3]'}*

```diff
@@ -1,13 +1,13 @@
 [
     {
         "inputs": [
             {
                 "internalType": "contract IVault",
-                "name": "vault",
+                "name": "_vault",
                 "type": "address"
             }
         ],
         "stateMutability": "nonpayable",
         "type": "constructor"
     },
     {
@@ -16,15 +16,15 @@
             {
                 "indexed": true,
                 "internalType": "address",
                 "name": "pool",
                 "type": "address"
             }
         ],
-        "name": "PoolCreated",
+        "name": "PoolRegistered",
         "type": "event"
     },
     {
         "inputs": [
             {
                 "internalType": "string",
                 "name": "name",
@@ -37,84 +37,52 @@
             },
             {
                 "internalType": "contract IERC20[]",
                 "name": "tokens",
                 "type": "address[]"
             },
             {
-                "internalType": "uint256[]",
-                "name": "weights",
-                "type": "uint256[]"
+                "internalType": "uint256",
+                "name": "amplificationParameter",
+                "type": "uint256"
             },
             {
                 "internalType": "uint256",
-                "name": "swapFeePercentage",
+                "name": "swapFee",
                 "type": "uint256"
             },
             {
-                "internalType": "address",
-                "name": "owner",
-                "type": "address"
-            }
-        ],
-        "name": "create",
-        "outputs": [
-            {
-                "internalType": "address",
-                "name": "",
-                "type": "address"
-            }
-        ],
-        "stateMutability": "nonpayable",
-        "type": "function"
-    },
-    {
-        "inputs": [],
-        "name": "getPauseConfiguration",
-        "outputs": [
-            {
                 "internalType": "uint256",
-                "name": "pauseWindowDuration",
+                "name": "emergencyPeriod",
                 "type": "uint256"
             },
             {
                 "internalType": "uint256",
-                "name": "bufferPeriodDuration",
+                "name": "emergencyPeriodCheckExtension",
                 "type": "uint256"
             }
         ],
-        "stateMutability": "view",
-        "type": "function"
-    },
-    {
-        "inputs": [],
-        "name": "getVault",
+        "name": "create",
         "outputs": [
             {
-                "internalType": "contract IVault",
+                "internalType": "address",
                 "name": "",
                 "type": "address"
             }
         ],
-        "stateMutability": "view",
+        "stateMutability": "nonpayable",
         "type": "function"
     },
     {
-        "inputs": [
-            {
-                "internalType": "address",
-                "name": "pool",
-                "type": "address"
-            }
-        ],
-        "name": "isPoolFromFactory",
+        "inputs": [],
+        "name": "vault",
         "outputs": [
             {
-                "internalType": "bool",
+                "internalType": "contract IVault",
                 "name": "",
-                "type": "bool"
+                "type": "address"
             }
         ],
         "stateMutability": "view",
         "type": "function"
     }
 ]
```

### Comparing `balpy-0.0.0a82/balpy/deployments/20210624-stable-pool/abi/StablePool.json` & `balpy-0.0.0a9/balpy/abi/ExchangeProxy.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.2694042318824548%*

 * *Differences: {'0': "{'inputs': {0: {'name': '_weth'}, delete: [7, 6, 5, 4, 3, 2, 1, 0]}, 'payable': False}",*

 * * '1': "{'inputs': {0: {'name': 'previousOwner'}, 1: {'name': 'newOwner'}, delete: [2]}, 'name': "*

 * *      "'OwnershipTransferred'}",*

 * * '10': "{'name': 'isOwner', 'outputs': {0: {'internalType': 'bool', 'type': 'bool'}}, 'constant': "*

 * *       "True, 'payable': False}",*

 * * '11': "{'inputs': [OrderedDict([('components', [OrderedDict([('internalType', 'address'), "*

 * *       "('name', 'pool'), ('type', 'address')]), OrderedDi […]*

```diff
@@ -1,1053 +1,868 @@
 [
     {
         "inputs": [
             {
-                "internalType": "contract IVault",
-                "name": "vault",
-                "type": "address"
-            },
-            {
-                "internalType": "string",
-                "name": "name",
-                "type": "string"
-            },
-            {
-                "internalType": "string",
-                "name": "symbol",
-                "type": "string"
-            },
-            {
-                "internalType": "contract IERC20[]",
-                "name": "tokens",
-                "type": "address[]"
-            },
-            {
-                "internalType": "uint256",
-                "name": "amplificationParameter",
-                "type": "uint256"
-            },
-            {
-                "internalType": "uint256",
-                "name": "swapFeePercentage",
-                "type": "uint256"
-            },
-            {
-                "internalType": "uint256",
-                "name": "pauseWindowDuration",
-                "type": "uint256"
-            },
-            {
-                "internalType": "uint256",
-                "name": "bufferPeriodDuration",
-                "type": "uint256"
-            },
-            {
                 "internalType": "address",
-                "name": "owner",
+                "name": "_weth",
                 "type": "address"
             }
         ],
+        "payable": false,
         "stateMutability": "nonpayable",
         "type": "constructor"
     },
     {
         "anonymous": false,
         "inputs": [
             {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "startValue",
-                "type": "uint256"
-            },
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "endValue",
-                "type": "uint256"
-            },
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "startTime",
-                "type": "uint256"
-            },
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "endTime",
-                "type": "uint256"
-            }
-        ],
-        "name": "AmpUpdateStarted",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "currentValue",
-                "type": "uint256"
-            }
-        ],
-        "name": "AmpUpdateStopped",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
                 "indexed": true,
                 "internalType": "address",
-                "name": "owner",
+                "name": "previousOwner",
                 "type": "address"
             },
             {
                 "indexed": true,
                 "internalType": "address",
-                "name": "spender",
+                "name": "newOwner",
                 "type": "address"
-            },
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "value",
-                "type": "uint256"
             }
         ],
-        "name": "Approval",
+        "name": "OwnershipTransferred",
         "type": "event"
     },
     {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "bool",
-                "name": "paused",
-                "type": "bool"
-            }
-        ],
-        "name": "PausedStateChanged",
-        "type": "event"
+        "payable": true,
+        "stateMutability": "payable",
+        "type": "fallback"
     },
     {
-        "anonymous": false,
+        "constant": false,
         "inputs": [
             {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "swapFeePercentage",
-                "type": "uint256"
-            }
-        ],
-        "name": "SwapFeePercentageChanged",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
+                "components": [
+                    {
+                        "internalType": "address",
+                        "name": "pool",
+                        "type": "address"
+                    },
+                    {
+                        "internalType": "address",
+                        "name": "tokenIn",
+                        "type": "address"
+                    },
+                    {
+                        "internalType": "address",
+                        "name": "tokenOut",
+                        "type": "address"
+                    },
+                    {
+                        "internalType": "uint256",
+                        "name": "swapAmount",
+                        "type": "uint256"
+                    },
+                    {
+                        "internalType": "uint256",
+                        "name": "limitReturnAmount",
+                        "type": "uint256"
+                    },
+                    {
+                        "internalType": "uint256",
+                        "name": "maxPrice",
+                        "type": "uint256"
+                    }
+                ],
+                "internalType": "struct ExchangeProxy.Swap[]",
+                "name": "swaps",
+                "type": "tuple[]"
+            },
             {
-                "indexed": true,
-                "internalType": "address",
-                "name": "from",
+                "internalType": "contract TokenInterface",
+                "name": "tokenIn",
                 "type": "address"
             },
             {
-                "indexed": true,
-                "internalType": "address",
-                "name": "to",
+                "internalType": "contract TokenInterface",
+                "name": "tokenOut",
                 "type": "address"
             },
             {
-                "indexed": false,
                 "internalType": "uint256",
-                "name": "value",
+                "name": "totalAmountIn",
                 "type": "uint256"
-            }
-        ],
-        "name": "Transfer",
-        "type": "event"
-    },
-    {
-        "inputs": [],
-        "name": "DOMAIN_SEPARATOR",
-        "outputs": [
-            {
-                "internalType": "bytes32",
-                "name": "",
-                "type": "bytes32"
-            }
-        ],
-        "stateMutability": "view",
-        "type": "function"
-    },
-    {
-        "inputs": [
-            {
-                "internalType": "address",
-                "name": "owner",
-                "type": "address"
             },
             {
-                "internalType": "address",
-                "name": "spender",
-                "type": "address"
+                "internalType": "uint256",
+                "name": "minTotalAmountOut",
+                "type": "uint256"
             }
         ],
-        "name": "allowance",
+        "name": "batchSwapExactIn",
         "outputs": [
             {
                 "internalType": "uint256",
-                "name": "",
+                "name": "totalAmountOut",
                 "type": "uint256"
             }
         ],
-        "stateMutability": "view",
+        "payable": true,
+        "stateMutability": "payable",
         "type": "function"
     },
     {
+        "constant": false,
         "inputs": [
             {
-                "internalType": "address",
-                "name": "spender",
-                "type": "address"
+                "components": [
+                    {
+                        "internalType": "address",
+                        "name": "pool",
+                        "type": "address"
+                    },
+                    {
+                        "internalType": "address",
+                        "name": "tokenIn",
+                        "type": "address"
+                    },
+                    {
+                        "internalType": "address",
+                        "name": "tokenOut",
+                        "type": "address"
+                    },
+                    {
+                        "internalType": "uint256",
+                        "name": "swapAmount",
+                        "type": "uint256"
+                    },
+                    {
+                        "internalType": "uint256",
+                        "name": "limitReturnAmount",
+                        "type": "uint256"
+                    },
+                    {
+                        "internalType": "uint256",
+                        "name": "maxPrice",
+                        "type": "uint256"
+                    }
+                ],
+                "internalType": "struct ExchangeProxy.Swap[]",
+                "name": "swaps",
+                "type": "tuple[]"
             },
             {
-                "internalType": "uint256",
-                "name": "amount",
-                "type": "uint256"
-            }
-        ],
-        "name": "approve",
-        "outputs": [
-            {
-                "internalType": "bool",
-                "name": "",
-                "type": "bool"
-            }
-        ],
-        "stateMutability": "nonpayable",
-        "type": "function"
-    },
-    {
-        "inputs": [
-            {
-                "internalType": "address",
-                "name": "account",
+                "internalType": "contract TokenInterface",
+                "name": "tokenIn",
                 "type": "address"
-            }
-        ],
-        "name": "balanceOf",
-        "outputs": [
-            {
-                "internalType": "uint256",
-                "name": "",
-                "type": "uint256"
-            }
-        ],
-        "stateMutability": "view",
-        "type": "function"
-    },
-    {
-        "inputs": [],
-        "name": "decimals",
-        "outputs": [
-            {
-                "internalType": "uint8",
-                "name": "",
-                "type": "uint8"
-            }
-        ],
-        "stateMutability": "view",
-        "type": "function"
-    },
-    {
-        "inputs": [
+            },
             {
-                "internalType": "address",
-                "name": "spender",
+                "internalType": "contract TokenInterface",
+                "name": "tokenOut",
                 "type": "address"
             },
             {
                 "internalType": "uint256",
-                "name": "amount",
+                "name": "maxTotalAmountIn",
                 "type": "uint256"
             }
         ],
-        "name": "decreaseAllowance",
+        "name": "batchSwapExactOut",
         "outputs": [
             {
-                "internalType": "bool",
-                "name": "",
-                "type": "bool"
+                "internalType": "uint256",
+                "name": "totalAmountIn",
+                "type": "uint256"
             }
         ],
-        "stateMutability": "nonpayable",
+        "payable": true,
+        "stateMutability": "payable",
         "type": "function"
     },
     {
+        "constant": true,
         "inputs": [
             {
-                "internalType": "bytes4",
-                "name": "selector",
-                "type": "bytes4"
-            }
-        ],
-        "name": "getActionId",
-        "outputs": [
-            {
-                "internalType": "bytes32",
-                "name": "",
-                "type": "bytes32"
-            }
-        ],
-        "stateMutability": "view",
-        "type": "function"
-    },
-    {
-        "inputs": [],
-        "name": "getAmplificationParameter",
-        "outputs": [
-            {
-                "internalType": "uint256",
-                "name": "value",
-                "type": "uint256"
-            },
-            {
-                "internalType": "bool",
-                "name": "isUpdating",
-                "type": "bool"
+                "internalType": "uint256[]",
+                "name": "bestInputAmounts",
+                "type": "uint256[]"
             },
             {
                 "internalType": "uint256",
-                "name": "precision",
+                "name": "swapAmount",
                 "type": "uint256"
             }
         ],
-        "stateMutability": "view",
-        "type": "function"
-    },
-    {
-        "inputs": [],
-        "name": "getAuthorizer",
-        "outputs": [
-            {
-                "internalType": "contract IAuthorizer",
-                "name": "",
-                "type": "address"
-            }
-        ],
-        "stateMutability": "view",
-        "type": "function"
-    },
-    {
-        "inputs": [],
-        "name": "getOwner",
+        "name": "calcDust",
         "outputs": [
             {
-                "internalType": "address",
+                "internalType": "uint256[]",
                 "name": "",
-                "type": "address"
+                "type": "uint256[]"
             }
         ],
-        "stateMutability": "view",
+        "payable": false,
+        "stateMutability": "pure",
         "type": "function"
     },
     {
-        "inputs": [],
-        "name": "getPausedState",
-        "outputs": [
-            {
-                "internalType": "bool",
-                "name": "paused",
-                "type": "bool"
-            },
+        "constant": true,
+        "inputs": [
             {
                 "internalType": "uint256",
-                "name": "pauseWindowEndTime",
+                "name": "tokenWeightIn",
                 "type": "uint256"
             },
             {
                 "internalType": "uint256",
-                "name": "bufferPeriodEndTime",
+                "name": "tokenBalanceOut",
                 "type": "uint256"
-            }
-        ],
-        "stateMutability": "view",
-        "type": "function"
-    },
-    {
-        "inputs": [],
-        "name": "getPoolId",
-        "outputs": [
-            {
-                "internalType": "bytes32",
-                "name": "",
-                "type": "bytes32"
-            }
-        ],
-        "stateMutability": "view",
-        "type": "function"
-    },
-    {
-        "inputs": [],
-        "name": "getRate",
-        "outputs": [
+            },
             {
                 "internalType": "uint256",
-                "name": "",
+                "name": "tokenWeightOut",
                 "type": "uint256"
             }
         ],
-        "stateMutability": "view",
-        "type": "function"
-    },
-    {
-        "inputs": [],
-        "name": "getSwapFeePercentage",
+        "name": "calcSlippageSlopeEffectivePrice",
         "outputs": [
             {
                 "internalType": "uint256",
-                "name": "",
+                "name": "slippageSlopeEffectivePrice",
                 "type": "uint256"
             }
         ],
-        "stateMutability": "view",
-        "type": "function"
-    },
-    {
-        "inputs": [],
-        "name": "getVault",
-        "outputs": [
-            {
-                "internalType": "contract IVault",
-                "name": "",
-                "type": "address"
-            }
-        ],
-        "stateMutability": "view",
+        "payable": false,
+        "stateMutability": "pure",
         "type": "function"
     },
     {
+        "constant": true,
         "inputs": [
             {
-                "internalType": "address",
-                "name": "spender",
-                "type": "address"
+                "internalType": "uint256[]",
+                "name": "bestInputAmounts",
+                "type": "uint256[]"
             },
             {
-                "internalType": "uint256",
-                "name": "addedValue",
-                "type": "uint256"
-            }
-        ],
-        "name": "increaseAllowance",
-        "outputs": [
-            {
-                "internalType": "bool",
-                "name": "",
-                "type": "bool"
+                "components": [
+                    {
+                        "internalType": "address",
+                        "name": "pool",
+                        "type": "address"
+                    },
+                    {
+                        "internalType": "uint256",
+                        "name": "tokenBalanceIn",
+                        "type": "uint256"
+                    },
+                    {
+                        "internalType": "uint256",
+                        "name": "tokenWeightIn",
+                        "type": "uint256"
+                    },
+                    {
+                        "internalType": "uint256",
+                        "name": "tokenBalanceOut",
+                        "type": "uint256"
+                    },
+                    {
+                        "internalType": "uint256",
+                        "name": "tokenWeightOut",
+                        "type": "uint256"
+                    },
+                    {
+                        "internalType": "uint256",
+                        "name": "swapFee",
+                        "type": "uint256"
+                    },
+                    {
+                        "internalType": "uint256",
+                        "name": "slippageSlopeEffectivePrice",
+                        "type": "uint256"
+                    }
+                ],
+                "internalType": "struct ExchangeProxy.Pool[]",
+                "name": "bestPools",
+                "type": "tuple[]"
             }
         ],
-        "stateMutability": "nonpayable",
-        "type": "function"
-    },
-    {
-        "inputs": [],
-        "name": "name",
+        "name": "calcTotalOutExactIn",
         "outputs": [
             {
-                "internalType": "string",
-                "name": "",
-                "type": "string"
+                "internalType": "uint256",
+                "name": "totalOutput",
+                "type": "uint256"
             }
         ],
-        "stateMutability": "view",
+        "payable": false,
+        "stateMutability": "pure",
         "type": "function"
     },
     {
+        "constant": true,
         "inputs": [
             {
-                "internalType": "address",
-                "name": "owner",
-                "type": "address"
+                "internalType": "uint256[]",
+                "name": "bestInputAmounts",
+                "type": "uint256[]"
+            },
+            {
+                "components": [
+                    {
+                        "internalType": "address",
+                        "name": "pool",
+                        "type": "address"
+                    },
+                    {
+                        "internalType": "uint256",
+                        "name": "tokenBalanceIn",
+                        "type": "uint256"
+                    },
+                    {
+                        "internalType": "uint256",
+                        "name": "tokenWeightIn",
+                        "type": "uint256"
+                    },
+                    {
+                        "internalType": "uint256",
+                        "name": "tokenBalanceOut",
+                        "type": "uint256"
+                    },
+                    {
+                        "internalType": "uint256",
+                        "name": "tokenWeightOut",
+                        "type": "uint256"
+                    },
+                    {
+                        "internalType": "uint256",
+                        "name": "swapFee",
+                        "type": "uint256"
+                    },
+                    {
+                        "internalType": "uint256",
+                        "name": "slippageSlopeEffectivePrice",
+                        "type": "uint256"
+                    }
+                ],
+                "internalType": "struct ExchangeProxy.Pool[]",
+                "name": "bestPools",
+                "type": "tuple[]"
             }
         ],
-        "name": "nonces",
+        "name": "calcTotalOutExactOut",
         "outputs": [
             {
                 "internalType": "uint256",
-                "name": "",
+                "name": "totalOutput",
                 "type": "uint256"
             }
         ],
-        "stateMutability": "view",
+        "payable": false,
+        "stateMutability": "pure",
         "type": "function"
     },
     {
+        "constant": true,
         "inputs": [
             {
-                "internalType": "bytes32",
-                "name": "poolId",
-                "type": "bytes32"
-            },
-            {
                 "internalType": "address",
-                "name": "sender",
+                "name": "tokenIn",
                 "type": "address"
             },
             {
                 "internalType": "address",
-                "name": "recipient",
+                "name": "tokenOut",
                 "type": "address"
             },
             {
-                "internalType": "uint256[]",
-                "name": "balances",
-                "type": "uint256[]"
-            },
-            {
-                "internalType": "uint256",
-                "name": "lastChangeBlock",
-                "type": "uint256"
-            },
-            {
-                "internalType": "uint256",
-                "name": "protocolSwapFeePercentage",
-                "type": "uint256"
-            },
-            {
-                "internalType": "bytes",
-                "name": "userData",
-                "type": "bytes"
+                "internalType": "address",
+                "name": "poolAddress",
+                "type": "address"
             }
         ],
-        "name": "onExitPool",
+        "name": "getPoolData",
         "outputs": [
             {
-                "internalType": "uint256[]",
-                "name": "",
-                "type": "uint256[]"
-            },
-            {
-                "internalType": "uint256[]",
+                "components": [
+                    {
+                        "internalType": "address",
+                        "name": "pool",
+                        "type": "address"
+                    },
+                    {
+                        "internalType": "uint256",
+                        "name": "tokenBalanceIn",
+                        "type": "uint256"
+                    },
+                    {
+                        "internalType": "uint256",
+                        "name": "tokenWeightIn",
+                        "type": "uint256"
+                    },
+                    {
+                        "internalType": "uint256",
+                        "name": "tokenBalanceOut",
+                        "type": "uint256"
+                    },
+                    {
+                        "internalType": "uint256",
+                        "name": "tokenWeightOut",
+                        "type": "uint256"
+                    },
+                    {
+                        "internalType": "uint256",
+                        "name": "swapFee",
+                        "type": "uint256"
+                    },
+                    {
+                        "internalType": "uint256",
+                        "name": "slippageSlopeEffectivePrice",
+                        "type": "uint256"
+                    }
+                ],
+                "internalType": "struct ExchangeProxy.Pool",
                 "name": "",
-                "type": "uint256[]"
+                "type": "tuple"
             }
         ],
-        "stateMutability": "nonpayable",
+        "payable": false,
+        "stateMutability": "view",
         "type": "function"
     },
     {
-        "inputs": [
-            {
-                "internalType": "bytes32",
-                "name": "poolId",
-                "type": "bytes32"
-            },
-            {
-                "internalType": "address",
-                "name": "sender",
-                "type": "address"
-            },
-            {
-                "internalType": "address",
-                "name": "recipient",
-                "type": "address"
-            },
-            {
-                "internalType": "uint256[]",
-                "name": "balances",
-                "type": "uint256[]"
-            },
-            {
-                "internalType": "uint256",
-                "name": "lastChangeBlock",
-                "type": "uint256"
-            },
-            {
-                "internalType": "uint256",
-                "name": "protocolSwapFeePercentage",
-                "type": "uint256"
-            },
-            {
-                "internalType": "bytes",
-                "name": "userData",
-                "type": "bytes"
-            }
-        ],
-        "name": "onJoinPool",
+        "constant": true,
+        "inputs": [],
+        "name": "isOwner",
         "outputs": [
             {
-                "internalType": "uint256[]",
-                "name": "",
-                "type": "uint256[]"
-            },
-            {
-                "internalType": "uint256[]",
+                "internalType": "bool",
                 "name": "",
-                "type": "uint256[]"
+                "type": "bool"
             }
         ],
-        "stateMutability": "nonpayable",
+        "payable": false,
+        "stateMutability": "view",
         "type": "function"
     },
     {
+        "constant": false,
         "inputs": [
             {
                 "components": [
                     {
-                        "internalType": "enum IVault.SwapKind",
-                        "name": "kind",
-                        "type": "uint8"
+                        "internalType": "address",
+                        "name": "pool",
+                        "type": "address"
                     },
                     {
-                        "internalType": "contract IERC20",
+                        "internalType": "address",
                         "name": "tokenIn",
                         "type": "address"
                     },
                     {
-                        "internalType": "contract IERC20",
+                        "internalType": "address",
                         "name": "tokenOut",
                         "type": "address"
                     },
                     {
                         "internalType": "uint256",
-                        "name": "amount",
+                        "name": "swapAmount",
                         "type": "uint256"
                     },
                     {
-                        "internalType": "bytes32",
-                        "name": "poolId",
-                        "type": "bytes32"
-                    },
-                    {
                         "internalType": "uint256",
-                        "name": "lastChangeBlock",
+                        "name": "limitReturnAmount",
                         "type": "uint256"
                     },
                     {
-                        "internalType": "address",
-                        "name": "from",
-                        "type": "address"
-                    },
-                    {
-                        "internalType": "address",
-                        "name": "to",
-                        "type": "address"
-                    },
-                    {
-                        "internalType": "bytes",
-                        "name": "userData",
-                        "type": "bytes"
+                        "internalType": "uint256",
+                        "name": "maxPrice",
+                        "type": "uint256"
                     }
                 ],
-                "internalType": "struct IPoolSwapStructs.SwapRequest",
-                "name": "swapRequest",
-                "type": "tuple"
+                "internalType": "struct ExchangeProxy.Swap[][]",
+                "name": "swapSequences",
+                "type": "tuple[][]"
             },
             {
-                "internalType": "uint256[]",
-                "name": "balances",
-                "type": "uint256[]"
+                "internalType": "contract TokenInterface",
+                "name": "tokenIn",
+                "type": "address"
+            },
+            {
+                "internalType": "contract TokenInterface",
+                "name": "tokenOut",
+                "type": "address"
             },
             {
                 "internalType": "uint256",
-                "name": "indexIn",
+                "name": "totalAmountIn",
                 "type": "uint256"
             },
             {
                 "internalType": "uint256",
-                "name": "indexOut",
+                "name": "minTotalAmountOut",
                 "type": "uint256"
             }
         ],
-        "name": "onSwap",
+        "name": "multihopBatchSwapExactIn",
         "outputs": [
             {
                 "internalType": "uint256",
-                "name": "",
+                "name": "totalAmountOut",
                 "type": "uint256"
             }
         ],
-        "stateMutability": "view",
+        "payable": true,
+        "stateMutability": "payable",
         "type": "function"
     },
     {
+        "constant": false,
         "inputs": [
             {
                 "components": [
                     {
-                        "internalType": "enum IVault.SwapKind",
-                        "name": "kind",
-                        "type": "uint8"
+                        "internalType": "address",
+                        "name": "pool",
+                        "type": "address"
                     },
                     {
-                        "internalType": "contract IERC20",
+                        "internalType": "address",
                         "name": "tokenIn",
                         "type": "address"
                     },
                     {
-                        "internalType": "contract IERC20",
+                        "internalType": "address",
                         "name": "tokenOut",
                         "type": "address"
                     },
                     {
                         "internalType": "uint256",
-                        "name": "amount",
+                        "name": "swapAmount",
                         "type": "uint256"
                     },
                     {
-                        "internalType": "bytes32",
-                        "name": "poolId",
-                        "type": "bytes32"
-                    },
-                    {
                         "internalType": "uint256",
-                        "name": "lastChangeBlock",
+                        "name": "limitReturnAmount",
                         "type": "uint256"
                     },
                     {
-                        "internalType": "address",
-                        "name": "from",
-                        "type": "address"
-                    },
-                    {
-                        "internalType": "address",
-                        "name": "to",
-                        "type": "address"
-                    },
-                    {
-                        "internalType": "bytes",
-                        "name": "userData",
-                        "type": "bytes"
+                        "internalType": "uint256",
+                        "name": "maxPrice",
+                        "type": "uint256"
                     }
                 ],
-                "internalType": "struct IPoolSwapStructs.SwapRequest",
-                "name": "request",
-                "type": "tuple"
+                "internalType": "struct ExchangeProxy.Swap[][]",
+                "name": "swapSequences",
+                "type": "tuple[][]"
             },
             {
-                "internalType": "uint256",
-                "name": "balanceTokenIn",
-                "type": "uint256"
+                "internalType": "contract TokenInterface",
+                "name": "tokenIn",
+                "type": "address"
+            },
+            {
+                "internalType": "contract TokenInterface",
+                "name": "tokenOut",
+                "type": "address"
             },
             {
                 "internalType": "uint256",
-                "name": "balanceTokenOut",
+                "name": "maxTotalAmountIn",
                 "type": "uint256"
             }
         ],
-        "name": "onSwap",
+        "name": "multihopBatchSwapExactOut",
         "outputs": [
             {
                 "internalType": "uint256",
-                "name": "",
+                "name": "totalAmountIn",
                 "type": "uint256"
             }
         ],
-        "stateMutability": "view",
+        "payable": true,
+        "stateMutability": "payable",
         "type": "function"
     },
     {
-        "inputs": [
+        "constant": true,
+        "inputs": [],
+        "name": "owner",
+        "outputs": [
             {
                 "internalType": "address",
-                "name": "owner",
+                "name": "",
                 "type": "address"
-            },
+            }
+        ],
+        "payable": false,
+        "stateMutability": "view",
+        "type": "function"
+    },
+    {
+        "constant": false,
+        "inputs": [],
+        "name": "renounceOwnership",
+        "outputs": [],
+        "payable": false,
+        "stateMutability": "nonpayable",
+        "type": "function"
+    },
+    {
+        "constant": false,
+        "inputs": [
             {
                 "internalType": "address",
-                "name": "spender",
+                "name": "_registry",
                 "type": "address"
-            },
-            {
-                "internalType": "uint256",
-                "name": "value",
-                "type": "uint256"
-            },
-            {
-                "internalType": "uint256",
-                "name": "deadline",
-                "type": "uint256"
-            },
-            {
-                "internalType": "uint8",
-                "name": "v",
-                "type": "uint8"
-            },
-            {
-                "internalType": "bytes32",
-                "name": "r",
-                "type": "bytes32"
-            },
-            {
-                "internalType": "bytes32",
-                "name": "s",
-                "type": "bytes32"
             }
         ],
-        "name": "permit",
+        "name": "setRegistry",
         "outputs": [],
+        "payable": false,
         "stateMutability": "nonpayable",
         "type": "function"
     },
     {
+        "constant": false,
         "inputs": [
             {
-                "internalType": "bytes32",
-                "name": "poolId",
-                "type": "bytes32"
-            },
-            {
-                "internalType": "address",
-                "name": "sender",
+                "internalType": "contract TokenInterface",
+                "name": "tokenIn",
                 "type": "address"
             },
             {
-                "internalType": "address",
-                "name": "recipient",
+                "internalType": "contract TokenInterface",
+                "name": "tokenOut",
                 "type": "address"
             },
             {
-                "internalType": "uint256[]",
-                "name": "balances",
-                "type": "uint256[]"
-            },
-            {
                 "internalType": "uint256",
-                "name": "lastChangeBlock",
+                "name": "totalAmountIn",
                 "type": "uint256"
             },
             {
                 "internalType": "uint256",
-                "name": "protocolSwapFeePercentage",
+                "name": "minTotalAmountOut",
                 "type": "uint256"
             },
             {
-                "internalType": "bytes",
-                "name": "userData",
-                "type": "bytes"
+                "internalType": "uint256",
+                "name": "nPools",
+                "type": "uint256"
             }
         ],
-        "name": "queryExit",
+        "name": "smartSwapExactIn",
         "outputs": [
             {
                 "internalType": "uint256",
-                "name": "bptIn",
+                "name": "totalAmountOut",
                 "type": "uint256"
-            },
-            {
-                "internalType": "uint256[]",
-                "name": "amountsOut",
-                "type": "uint256[]"
             }
         ],
-        "stateMutability": "nonpayable",
+        "payable": true,
+        "stateMutability": "payable",
         "type": "function"
     },
     {
+        "constant": false,
         "inputs": [
             {
-                "internalType": "bytes32",
-                "name": "poolId",
-                "type": "bytes32"
-            },
-            {
-                "internalType": "address",
-                "name": "sender",
+                "internalType": "contract TokenInterface",
+                "name": "tokenIn",
                 "type": "address"
             },
             {
-                "internalType": "address",
-                "name": "recipient",
+                "internalType": "contract TokenInterface",
+                "name": "tokenOut",
                 "type": "address"
             },
             {
-                "internalType": "uint256[]",
-                "name": "balances",
-                "type": "uint256[]"
-            },
-            {
                 "internalType": "uint256",
-                "name": "lastChangeBlock",
+                "name": "totalAmountOut",
                 "type": "uint256"
             },
             {
                 "internalType": "uint256",
-                "name": "protocolSwapFeePercentage",
+                "name": "maxTotalAmountIn",
                 "type": "uint256"
             },
             {
-                "internalType": "bytes",
-                "name": "userData",
-                "type": "bytes"
+                "internalType": "uint256",
+                "name": "nPools",
+                "type": "uint256"
             }
         ],
-        "name": "queryJoin",
+        "name": "smartSwapExactOut",
         "outputs": [
             {
                 "internalType": "uint256",
-                "name": "bptOut",
+                "name": "totalAmountIn",
                 "type": "uint256"
-            },
-            {
-                "internalType": "uint256[]",
-                "name": "amountsIn",
-                "type": "uint256[]"
             }
         ],
-        "stateMutability": "nonpayable",
+        "payable": true,
+        "stateMutability": "payable",
         "type": "function"
     },
     {
+        "constant": false,
         "inputs": [
             {
-                "internalType": "contract IERC20",
-                "name": "token",
+                "internalType": "address",
+                "name": "newOwner",
                 "type": "address"
-            },
-            {
-                "internalType": "bytes",
-                "name": "poolConfig",
-                "type": "bytes"
             }
         ],
-        "name": "setAssetManagerPoolConfig",
+        "name": "transferOwnership",
         "outputs": [],
+        "payable": false,
         "stateMutability": "nonpayable",
         "type": "function"
     },
     {
+        "constant": true,
         "inputs": [
             {
-                "internalType": "bool",
-                "name": "paused",
-                "type": "bool"
-            }
-        ],
-        "name": "setPaused",
-        "outputs": [],
-        "stateMutability": "nonpayable",
-        "type": "function"
-    },
-    {
-        "inputs": [
+                "internalType": "address",
+                "name": "tokenIn",
+                "type": "address"
+            },
             {
-                "internalType": "uint256",
-                "name": "swapFeePercentage",
-                "type": "uint256"
-            }
-        ],
-        "name": "setSwapFeePercentage",
-        "outputs": [],
-        "stateMutability": "nonpayable",
-        "type": "function"
-    },
-    {
-        "inputs": [
+                "internalType": "address",
+                "name": "tokenOut",
+                "type": "address"
+            },
             {
                 "internalType": "uint256",
-                "name": "rawEndValue",
+                "name": "swapAmount",
                 "type": "uint256"
             },
             {
                 "internalType": "uint256",
-                "name": "endTime",
+                "name": "nPools",
                 "type": "uint256"
             }
         ],
-        "name": "startAmplificationParameterUpdate",
-        "outputs": [],
-        "stateMutability": "nonpayable",
-        "type": "function"
-    },
-    {
-        "inputs": [],
-        "name": "stopAmplificationParameterUpdate",
-        "outputs": [],
-        "stateMutability": "nonpayable",
-        "type": "function"
-    },
-    {
-        "inputs": [],
-        "name": "symbol",
+        "name": "viewSplitExactIn",
         "outputs": [
             {
-                "internalType": "string",
-                "name": "",
-                "type": "string"
-            }
-        ],
-        "stateMutability": "view",
-        "type": "function"
-    },
-    {
-        "inputs": [],
-        "name": "totalSupply",
-        "outputs": [
+                "components": [
+                    {
+                        "internalType": "address",
+                        "name": "pool",
+                        "type": "address"
+                    },
+                    {
+                        "internalType": "address",
+                        "name": "tokenIn",
+                        "type": "address"
+                    },
+                    {
+                        "internalType": "address",
+                        "name": "tokenOut",
+                        "type": "address"
+                    },
+                    {
+                        "internalType": "uint256",
+                        "name": "swapAmount",
+                        "type": "uint256"
+                    },
+                    {
+                        "internalType": "uint256",
+                        "name": "limitReturnAmount",
+                        "type": "uint256"
+                    },
+                    {
+                        "internalType": "uint256",
+                        "name": "maxPrice",
+                        "type": "uint256"
+                    }
+                ],
+                "internalType": "struct ExchangeProxy.Swap[]",
+                "name": "swaps",
+                "type": "tuple[]"
+            },
             {
                 "internalType": "uint256",
-                "name": "",
+                "name": "totalOutput",
                 "type": "uint256"
             }
         ],
+        "payable": false,
         "stateMutability": "view",
         "type": "function"
     },
     {
+        "constant": true,
         "inputs": [
             {
                 "internalType": "address",
-                "name": "recipient",
+                "name": "tokenIn",
                 "type": "address"
             },
             {
-                "internalType": "uint256",
-                "name": "amount",
-                "type": "uint256"
-            }
-        ],
-        "name": "transfer",
-        "outputs": [
-            {
-                "internalType": "bool",
-                "name": "",
-                "type": "bool"
-            }
-        ],
-        "stateMutability": "nonpayable",
-        "type": "function"
-    },
-    {
-        "inputs": [
-            {
                 "internalType": "address",
-                "name": "sender",
+                "name": "tokenOut",
                 "type": "address"
             },
             {
-                "internalType": "address",
-                "name": "recipient",
-                "type": "address"
+                "internalType": "uint256",
+                "name": "swapAmount",
+                "type": "uint256"
             },
             {
                 "internalType": "uint256",
-                "name": "amount",
+                "name": "nPools",
                 "type": "uint256"
             }
         ],
-        "name": "transferFrom",
+        "name": "viewSplitExactOut",
         "outputs": [
             {
-                "internalType": "bool",
-                "name": "",
-                "type": "bool"
+                "components": [
+                    {
+                        "internalType": "address",
+                        "name": "pool",
+                        "type": "address"
+                    },
+                    {
+                        "internalType": "address",
+                        "name": "tokenIn",
+                        "type": "address"
+                    },
+                    {
+                        "internalType": "address",
+                        "name": "tokenOut",
+                        "type": "address"
+                    },
+                    {
+                        "internalType": "uint256",
+                        "name": "swapAmount",
+                        "type": "uint256"
+                    },
+                    {
+                        "internalType": "uint256",
+                        "name": "limitReturnAmount",
+                        "type": "uint256"
+                    },
+                    {
+                        "internalType": "uint256",
+                        "name": "maxPrice",
+                        "type": "uint256"
+                    }
+                ],
+                "internalType": "struct ExchangeProxy.Swap[]",
+                "name": "swaps",
+                "type": "tuple[]"
+            },
+            {
+                "internalType": "uint256",
+                "name": "totalOutput",
+                "type": "uint256"
             }
         ],
-        "stateMutability": "nonpayable",
+        "payable": false,
+        "stateMutability": "view",
         "type": "function"
     }
 ]
```

### Comparing `balpy-0.0.0a82/balpy/deployments/20210624-stable-pool/abi/StablePoolFactory.json` & `balpy-0.0.0a9/balpy/abi/Multicall.json`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.18154761904761907%*

 * *Differences: {'0': "{'inputs': [OrderedDict([('components', [OrderedDict([('name', 'target'), ('type', "*

 * *      "'address')]), OrderedDict([('name', 'callData'), ('type', 'bytes')])]), ('name', 'calls'), "*

 * *      "('type', 'tuple[]')])], 'name': 'aggregate', 'outputs': {0: {'name': 'blockNumber', delete: "*

 * *      "['internalType']}, 1: {'name': 'returnData', 'type': 'bytes[]', delete: ['internalType']}}, "*

 * *      "'constant': True, 'payable': False}",*

 * * '1': "{'inputs': {0: {'name': 'addr', delete: ['internalType']}}, 'name' […]*

```diff
@@ -1,120 +1,54 @@
 [
     {
+        "constant": true,
         "inputs": [
             {
-                "internalType": "contract IVault",
-                "name": "vault",
-                "type": "address"
-            }
-        ],
-        "stateMutability": "nonpayable",
-        "type": "constructor"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": true,
-                "internalType": "address",
-                "name": "pool",
-                "type": "address"
-            }
-        ],
-        "name": "PoolCreated",
-        "type": "event"
-    },
-    {
-        "inputs": [
-            {
-                "internalType": "string",
-                "name": "name",
-                "type": "string"
-            },
-            {
-                "internalType": "string",
-                "name": "symbol",
-                "type": "string"
-            },
-            {
-                "internalType": "contract IERC20[]",
-                "name": "tokens",
-                "type": "address[]"
-            },
-            {
-                "internalType": "uint256",
-                "name": "amplificationParameter",
-                "type": "uint256"
-            },
-            {
-                "internalType": "uint256",
-                "name": "swapFeePercentage",
-                "type": "uint256"
-            },
-            {
-                "internalType": "address",
-                "name": "owner",
-                "type": "address"
-            }
-        ],
-        "name": "create",
-        "outputs": [
-            {
-                "internalType": "address",
-                "name": "",
-                "type": "address"
+                "components": [
+                    {
+                        "name": "target",
+                        "type": "address"
+                    },
+                    {
+                        "name": "callData",
+                        "type": "bytes"
+                    }
+                ],
+                "name": "calls",
+                "type": "tuple[]"
             }
         ],
-        "stateMutability": "nonpayable",
-        "type": "function"
-    },
-    {
-        "inputs": [],
-        "name": "getPauseConfiguration",
+        "name": "aggregate",
         "outputs": [
             {
-                "internalType": "uint256",
-                "name": "pauseWindowDuration",
+                "name": "blockNumber",
                 "type": "uint256"
             },
             {
-                "internalType": "uint256",
-                "name": "bufferPeriodDuration",
-                "type": "uint256"
-            }
-        ],
-        "stateMutability": "view",
-        "type": "function"
-    },
-    {
-        "inputs": [],
-        "name": "getVault",
-        "outputs": [
-            {
-                "internalType": "contract IVault",
-                "name": "",
-                "type": "address"
+                "name": "returnData",
+                "type": "bytes[]"
             }
         ],
+        "payable": false,
         "stateMutability": "view",
         "type": "function"
     },
     {
+        "constant": true,
         "inputs": [
             {
-                "internalType": "address",
-                "name": "pool",
+                "name": "addr",
                 "type": "address"
             }
         ],
-        "name": "isPoolFromFactory",
+        "name": "getEthBalance",
         "outputs": [
             {
-                "internalType": "bool",
-                "name": "",
-                "type": "bool"
+                "name": "balance",
+                "type": "uint256"
             }
         ],
+        "payable": false,
         "stateMutability": "view",
         "type": "function"
     }
 ]
```

