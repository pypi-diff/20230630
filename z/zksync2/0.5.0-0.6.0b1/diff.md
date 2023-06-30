# Comparing `tmp/zksync2-0.5.0.tar.gz` & `tmp/zksync2-0.6.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zksync2-0.5.0.tar", last modified: Fri May 26 13:16:39 2023, max compression
+gzip compressed data, was "zksync2-0.6.0b1.tar", last modified: Fri Jun 30 00:43:28 2023, max compression
```

## Comparing `zksync2-0.5.0.tar` & `zksync2-0.6.0b1.tar`

### file list

```diff
@@ -1,121 +1,134 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:16:39.838590 zksync2-0.5.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:16:39.802590 zksync2-0.5.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:16:39.810590 zksync2-0.5.0/.github/workflows/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1162 2023-05-26 13:16:23.000000 zksync2-0.5.0/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-05-26 13:16:23.000000 zksync2-0.5.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-26 13:16:23.000000 zksync2-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    16281 2023-05-26 13:16:39.838590 zksync2-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15696 2023-05-26 13:16:23.000000 zksync2-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:16:39.814590 zksync2-0.5.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-05-26 13:16:23.000000 zksync2-0.5.0/examples/01_deposit.py
--rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-05-26 13:16:23.000000 zksync2-0.5.0/examples/02_transfer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3971 2023-05-26 13:16:23.000000 zksync2-0.5.0/examples/03_transfer_erc20_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-05-26 13:16:23.000000 zksync2-0.5.0/examples/04_deploy_create.py
--rw-r--r--   0 runner    (1001) docker     (123)     6980 2023-05-26 13:16:23.000000 zksync2-0.5.0/examples/05_deploy_create_with_constructor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-05-26 13:16:23.000000 zksync2-0.5.0/examples/06_deploy_create_with_deps.py
--rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-05-26 13:16:23.000000 zksync2-0.5.0/examples/07_deploy_create2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4802 2023-05-26 13:16:23.000000 zksync2-0.5.0/examples/08_deploy_create2_deps.py
--rw-r--r--   0 runner    (1001) docker     (123)     3818 2023-05-26 13:16:23.000000 zksync2-0.5.0/examples/09_withdrawal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-05-26 13:16:23.000000 zksync2-0.5.0/examples/10_finalize_withdrawal.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-26 13:16:23.000000 zksync2-0.5.0/examples/11_check_balance.py
--rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-05-26 13:16:23.000000 zksync2-0.5.0/examples/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:16:39.806590 zksync2-0.5.0/examples/solidity/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:16:39.814590 zksync2-0.5.0/examples/solidity/demo/
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-26 13:16:23.000000 zksync2-0.5.0/examples/solidity/demo/Demo.sol
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-26 13:16:23.000000 zksync2-0.5.0/examples/solidity/demo/Foo.sol
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:16:39.814590 zksync2-0.5.0/examples/solidity/demo/build/
--rw-r--r--   0 runner    (1001) docker     (123)    11955 2023-05-26 13:16:23.000000 zksync2-0.5.0/examples/solidity/demo/build/combined.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:16:39.814590 zksync2-0.5.0/examples/solidity/incrementer/
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-26 13:16:23.000000 zksync2-0.5.0/examples/solidity/incrementer/Incrementer.sol
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:16:39.814590 zksync2-0.5.0/examples/solidity/incrementer/build/
--rw-r--r--   0 runner    (1001) docker     (123)     3977 2023-05-26 13:16:23.000000 zksync2-0.5.0/examples/solidity/incrementer/build/combined.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:16:39.818590 zksync2-0.5.0/examples/solidity/storage/
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-26 13:16:23.000000 zksync2-0.5.0/examples/solidity/storage/Storage.sol
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:16:39.818590 zksync2-0.5.0/examples/solidity/storage/build/
--rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-05-26 13:16:23.000000 zksync2-0.5.0/examples/solidity/storage/build/combined.json
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-26 13:16:23.000000 zksync2-0.5.0/examples/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-26 13:16:23.000000 zksync2-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-26 13:16:23.000000 zksync2-0.5.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-26 13:16:39.838590 zksync2-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-26 13:16:23.000000 zksync2-0.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:16:39.818590 zksync2-0.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 13:16:23.000000 zksync2-0.5.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:16:39.818590 zksync2-0.5.0/tests/contracts/
--rw-r--r--   0 runner    (1001) docker     (123)     9467 2023-05-26 13:16:23.000000 zksync2-0.5.0/tests/contracts/Counter.json
--rw-r--r--   0 runner    (1001) docker     (123)   103076 2023-05-26 13:16:23.000000 zksync2-0.5.0/tests/contracts/CustomAccount.json
--rw-r--r--   0 runner    (1001) docker     (123)    48494 2023-05-26 13:16:23.000000 zksync2-0.5.0/tests/contracts/CustomPaymaster.json
--rw-r--r--   0 runner    (1001) docker     (123)     8303 2023-05-26 13:16:23.000000 zksync2-0.5.0/tests/contracts/Foo.json
--rw-r--r--   0 runner    (1001) docker     (123)    15075 2023-05-26 13:16:23.000000 zksync2-0.5.0/tests/contracts/Import.json
--rw-r--r--   0 runner    (1001) docker     (123)     6733 2023-05-26 13:16:23.000000 zksync2-0.5.0/tests/contracts/SimpleConstructor.json
--rw-r--r--   0 runner    (1001) docker     (123)    50646 2023-05-26 13:16:23.000000 zksync2-0.5.0/tests/contracts/SomeERC20.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 13:16:23.000000 zksync2-0.5.0/tests/contracts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-26 13:16:23.000000 zksync2-0.5.0/tests/contracts/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:16:39.822590 zksync2-0.5.0/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 13:16:23.000000 zksync2-0.5.0/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-26 13:16:23.000000 zksync2-0.5.0/tests/integration/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3563 2023-05-26 13:16:23.000000 zksync2-0.5.0/tests/integration/test_deposit.py
--rw-r--r--   0 runner    (1001) docker     (123)     9344 2023-05-26 13:16:23.000000 zksync2-0.5.0/tests/integration/test_paymaster.py
--rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-05-26 13:16:23.000000 zksync2-0.5.0/tests/integration/test_transfer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-05-26 13:16:23.000000 zksync2-0.5.0/tests/integration/test_withdraw.py
--rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-05-26 13:16:23.000000 zksync2-0.5.0/tests/integration/test_zksync_contract.py
--rw-r--r--   0 runner    (1001) docker     (123)    42460 2023-05-26 13:16:23.000000 zksync2-0.5.0/tests/integration/test_zksync_web3.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:16:39.822590 zksync2-0.5.0/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 13:16:23.000000 zksync2-0.5.0/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-26 13:16:23.000000 zksync2-0.5.0/tests/unit/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-05-26 13:16:23.000000 zksync2-0.5.0/tests/unit/test_contract_deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4308 2023-05-26 13:16:23.000000 zksync2-0.5.0/tests/unit/test_eip712.py
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-05-26 13:16:23.000000 zksync2-0.5.0/tests/unit/test_eth_signer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-05-26 13:16:23.000000 zksync2-0.5.0/tests/unit/test_transaction712.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:16:39.822590 zksync2-0.5.0/zksync2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 13:16:23.000000 zksync2-0.5.0/zksync2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:16:39.826590 zksync2-0.5.0/zksync2/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 13:16:23.000000 zksync2-0.5.0/zksync2/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-05-26 13:16:23.000000 zksync2-0.5.0/zksync2/core/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-05-26 13:16:23.000000 zksync2-0.5.0/zksync2/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:16:39.830590 zksync2-0.5.0/zksync2/manage_contracts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 13:16:23.000000 zksync2-0.5.0/zksync2/manage_contracts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:16:39.834590 zksync2-0.5.0/zksync2/manage_contracts/contract_abi/
--rw-r--r--   0 runner    (1001) docker     (123)     8609 2023-05-26 13:16:23.000000 zksync2-0.5.0/zksync2/manage_contracts/contract_abi/ContractDeployer.json
--rw-r--r--   0 runner    (1001) docker     (123)     4508 2023-05-26 13:16:23.000000 zksync2-0.5.0/zksync2/manage_contracts/contract_abi/IERC20.json
--rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-05-26 13:16:23.000000 zksync2-0.5.0/zksync2/manage_contracts/contract_abi/IEthToken.json
--rw-r--r--   0 runner    (1001) docker     (123)     5320 2023-05-26 13:16:23.000000 zksync2-0.5.0/zksync2/manage_contracts/contract_abi/IL1Bridge.json
--rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-05-26 13:16:23.000000 zksync2-0.5.0/zksync2/manage_contracts/contract_abi/IL2Bridge.json
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-05-26 13:16:23.000000 zksync2-0.5.0/zksync2/manage_contracts/contract_abi/INonceHolder.json
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-26 13:16:23.000000 zksync2-0.5.0/zksync2/manage_contracts/contract_abi/IPaymasterFlow.json
--rw-r--r--   0 runner    (1001) docker     (123)    49698 2023-05-26 13:16:23.000000 zksync2-0.5.0/zksync2/manage_contracts/contract_abi/IZkSync.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 13:16:23.000000 zksync2-0.5.0/zksync2/manage_contracts/contract_abi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-05-26 13:16:23.000000 zksync2-0.5.0/zksync2/manage_contracts/contract_encoder_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6301 2023-05-26 13:16:23.000000 zksync2-0.5.0/zksync2/manage_contracts/contract_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-26 13:16:23.000000 zksync2-0.5.0/zksync2/manage_contracts/deploy_addresses.py
--rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-05-26 13:16:23.000000 zksync2-0.5.0/zksync2/manage_contracts/erc20_contract.py
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-05-26 13:16:23.000000 zksync2-0.5.0/zksync2/manage_contracts/eth_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     5304 2023-05-26 13:16:23.000000 zksync2-0.5.0/zksync2/manage_contracts/l1_bridge.py
--rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-05-26 13:16:23.000000 zksync2-0.5.0/zksync2/manage_contracts/l2_bridge.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-05-26 13:16:23.000000 zksync2-0.5.0/zksync2/manage_contracts/nonce_holder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-05-26 13:16:23.000000 zksync2-0.5.0/zksync2/manage_contracts/paymaster_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-05-26 13:16:23.000000 zksync2-0.5.0/zksync2/manage_contracts/precompute_contract_deployer.py
--rw-r--r--   0 runner    (1001) docker     (123)    14931 2023-05-26 13:16:23.000000 zksync2-0.5.0/zksync2/manage_contracts/zksync_contract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:16:39.834590 zksync2-0.5.0/zksync2/module/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 13:16:23.000000 zksync2-0.5.0/zksync2/module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-26 13:16:23.000000 zksync2-0.5.0/zksync2/module/middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-26 13:16:23.000000 zksync2-0.5.0/zksync2/module/module_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-05-26 13:16:23.000000 zksync2-0.5.0/zksync2/module/request_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-26 13:16:23.000000 zksync2-0.5.0/zksync2/module/response_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    14805 2023-05-26 13:16:23.000000 zksync2-0.5.0/zksync2/module/zksync_module.py
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-26 13:16:23.000000 zksync2-0.5.0/zksync2/module/zksync_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:16:39.834590 zksync2-0.5.0/zksync2/provider/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 13:16:23.000000 zksync2-0.5.0/zksync2/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13070 2023-05-26 13:16:23.000000 zksync2-0.5.0/zksync2/provider/eth_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:16:39.834590 zksync2-0.5.0/zksync2/signer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 13:16:23.000000 zksync2-0.5.0/zksync2/signer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-05-26 13:16:23.000000 zksync2-0.5.0/zksync2/signer/eth_signer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:16:39.838590 zksync2-0.5.0/zksync2/transaction/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 13:16:23.000000 zksync2-0.5.0/zksync2/transaction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6274 2023-05-26 13:16:23.000000 zksync2-0.5.0/zksync2/transaction/transaction712.py
--rw-r--r--   0 runner    (1001) docker     (123)     7845 2023-05-26 13:16:23.000000 zksync2-0.5.0/zksync2/transaction/transaction_builders.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:16:39.826590 zksync2-0.5.0/zksync2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16281 2023-05-26 13:16:39.000000 zksync2-0.5.0/zksync2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-05-26 13:16:39.000000 zksync2-0.5.0/zksync2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 13:16:39.000000 zksync2-0.5.0/zksync2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-26 13:16:39.000000 zksync2-0.5.0/zksync2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-26 13:16:39.000000 zksync2-0.5.0/zksync2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:43:28.903181 zksync2-0.6.0b1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:43:28.887180 zksync2-0.6.0b1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:43:28.891181 zksync2-0.6.0b1/.github/workflows/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1162 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    16283 2023-06-30 00:43:28.903181 zksync2-0.6.0b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15696 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:43:28.891181 zksync2-0.6.0b1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/examples/01_deposit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4162 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/examples/02_transfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/examples/03_transfer_erc20_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/examples/04_deploy_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6901 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/examples/05_deploy_create_with_constructor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/examples/06_deploy_create_with_deps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/examples/07_deploy_create2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4802 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/examples/08_deploy_create2_deps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3818 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/examples/09_withdrawal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/examples/10_finalize_withdrawal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/examples/11_check_balance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5305 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/examples/12_deploy_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4700 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/examples/13_deploy_account_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5369 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/examples/14_deploy_account_create2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6980 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/examples/15_use_paymaster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/examples/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:43:28.887180 zksync2-0.6.0b1/examples/solidity/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:43:28.891181 zksync2-0.6.0b1/examples/solidity/custom_paymaster/
+-rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/examples/solidity/custom_paymaster/Paymaster.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/examples/solidity/custom_paymaster/Token.sol
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:43:28.891181 zksync2-0.6.0b1/examples/solidity/custom_paymaster/build/
+-rw-r--r--   0 runner    (1001) docker     (123)    42342 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/examples/solidity/custom_paymaster/build/Paymaster.json
+-rw-r--r--   0 runner    (1001) docker     (123)    65416 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/examples/solidity/custom_paymaster/build/Token.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:43:28.891181 zksync2-0.6.0b1/examples/solidity/demo/
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/examples/solidity/demo/Demo.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/examples/solidity/demo/Foo.sol
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:43:28.895181 zksync2-0.6.0b1/examples/solidity/demo/build/
+-rw-r--r--   0 runner    (1001) docker     (123)    11955 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/examples/solidity/demo/build/combined.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:43:28.895181 zksync2-0.6.0b1/examples/solidity/incrementer/
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/examples/solidity/incrementer/Incrementer.sol
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:43:28.895181 zksync2-0.6.0b1/examples/solidity/incrementer/build/
+-rw-r--r--   0 runner    (1001) docker     (123)     3977 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/examples/solidity/incrementer/build/combined.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:43:28.895181 zksync2-0.6.0b1/examples/solidity/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/examples/solidity/storage/Storage.sol
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:43:28.895181 zksync2-0.6.0b1/examples/solidity/storage/build/
+-rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/examples/solidity/storage/build/combined.json
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/examples/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-30 00:43:28.907182 zksync2-0.6.0b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:43:28.895181 zksync2-0.6.0b1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:43:28.895181 zksync2-0.6.0b1/tests/contracts/
+-rw-r--r--   0 runner    (1001) docker     (123)     9467 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/tests/contracts/Counter.json
+-rw-r--r--   0 runner    (1001) docker     (123)   103076 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/tests/contracts/CustomAccount.json
+-rw-r--r--   0 runner    (1001) docker     (123)    48494 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/tests/contracts/CustomPaymaster.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8303 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/tests/contracts/Foo.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15075 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/tests/contracts/Import.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6733 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/tests/contracts/SimpleConstructor.json
+-rw-r--r--   0 runner    (1001) docker     (123)    50646 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/tests/contracts/SomeERC20.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/tests/contracts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/tests/contracts/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:43:28.895181 zksync2-0.6.0b1/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/tests/integration/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3563 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/tests/integration/test_deposit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9344 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/tests/integration/test_paymaster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/tests/integration/test_transfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/tests/integration/test_withdraw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/tests/integration/test_zksync_contract.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42460 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/tests/integration/test_zksync_web3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:43:28.899181 zksync2-0.6.0b1/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/tests/unit/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/tests/unit/test_contract_deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4308 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/tests/unit/test_eip712.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/tests/unit/test_eth_signer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/tests/unit/test_transaction712.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:43:28.899181 zksync2-0.6.0b1/zksync2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/zksync2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:43:28.899181 zksync2-0.6.0b1/zksync2/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/zksync2/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/zksync2/core/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/zksync2/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:43:28.899181 zksync2-0.6.0b1/zksync2/manage_contracts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/zksync2/manage_contracts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:43:28.903181 zksync2-0.6.0b1/zksync2/manage_contracts/contract_abi/
+-rw-r--r--   0 runner    (1001) docker     (123)     9537 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/zksync2/manage_contracts/contract_abi/ContractDeployer.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6220 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/zksync2/manage_contracts/contract_abi/IAllowList.json
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/zksync2/manage_contracts/contract_abi/IERC1271.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4508 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/zksync2/manage_contracts/contract_abi/IERC20.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/zksync2/manage_contracts/contract_abi/IEthToken.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5847 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/zksync2/manage_contracts/contract_abi/IL1Bridge.json
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/zksync2/manage_contracts/contract_abi/IL1Messenger.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/zksync2/manage_contracts/contract_abi/IL2Bridge.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/zksync2/manage_contracts/contract_abi/INonceHolder.json
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/zksync2/manage_contracts/contract_abi/IPaymasterFlow.json
+-rw-r--r--   0 runner    (1001) docker     (123)    49698 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/zksync2/manage_contracts/contract_abi/IZkSync.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/zksync2/manage_contracts/contract_abi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/zksync2/manage_contracts/contract_encoder_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6301 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/zksync2/manage_contracts/contract_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/zksync2/manage_contracts/deploy_addresses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/zksync2/manage_contracts/erc20_contract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/zksync2/manage_contracts/eth_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5304 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/zksync2/manage_contracts/l1_bridge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/zksync2/manage_contracts/l2_bridge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/zksync2/manage_contracts/nonce_holder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/zksync2/manage_contracts/paymaster_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/zksync2/manage_contracts/precompute_contract_deployer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14931 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/zksync2/manage_contracts/zksync_contract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:43:28.903181 zksync2-0.6.0b1/zksync2/module/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/zksync2/module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/zksync2/module/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/zksync2/module/module_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/zksync2/module/request_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/zksync2/module/response_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14805 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/zksync2/module/zksync_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/zksync2/module/zksync_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:43:28.903181 zksync2-0.6.0b1/zksync2/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/zksync2/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13089 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/zksync2/provider/eth_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:43:28.903181 zksync2-0.6.0b1/zksync2/signer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/zksync2/signer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/zksync2/signer/eth_signer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:43:28.903181 zksync2-0.6.0b1/zksync2/transaction/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/zksync2/transaction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6274 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/zksync2/transaction/transaction712.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11491 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/zksync2/transaction/transaction_builders.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:43:28.899181 zksync2-0.6.0b1/zksync2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16283 2023-06-30 00:43:28.000000 zksync2-0.6.0b1/zksync2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-06-30 00:43:28.000000 zksync2-0.6.0b1/zksync2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 00:43:28.000000 zksync2-0.6.0b1/zksync2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-30 00:43:28.000000 zksync2-0.6.0b1/zksync2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-30 00:43:28.000000 zksync2-0.6.0b1/zksync2.egg-info/top_level.txt
```

### Comparing `zksync2-0.5.0/.github/workflows/release.yaml` & `zksync2-0.6.0b1/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `zksync2-0.5.0/.gitignore` & `zksync2-0.6.0b1/.gitignore`

 * *Files identical despite different names*

### Comparing `zksync2-0.5.0/PKG-INFO` & `zksync2-0.6.0b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zksync2
-Version: 0.5.0
+Version: 0.6.0b1
 Summary: zkSync2 python client sdk
 Home-page: https://zksync.io
 Author: Danijel Radakovic
 Author-email: Danijel Radakovic <danijel@txfusion.io>
 License: MIT
 Project-URL: Homepage, https://github.com/zksync-sdk/zksync2-python
 Project-URL: Bug Tracker, https://github.com/zksync-sdk/zksync2-python/issues
```

### Comparing `zksync2-0.5.0/README.md` & `zksync2-0.6.0b1/README.md`

 * *Files identical despite different names*

### Comparing `zksync2-0.5.0/examples/01_deposit.py` & `zksync2-0.6.0b1/examples/01_deposit.py`

 * *Files identical despite different names*

### Comparing `zksync2-0.5.0/examples/02_transfer.py` & `zksync2-0.6.0b1/examples/02_transfer.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
     :param address:
       Desired ETH address that you want to transfer to.
 
     :param amount:
       Desired ETH amount that you want to transfer.
 
     :return:
-      The transaction hash of the deposit transaction.
+      The transaction hash of the transfer transaction.
 
     """
 
     # Get chain id of zkSync network
     chain_id = zk_web3.zksync.chain_id
 
     # Signer is used to generate signature of provided transaction
```

### Comparing `zksync2-0.5.0/examples/04_deploy_create.py` & `zksync2-0.6.0b1/examples/04_deploy_create.py`

 * *Files identical despite different names*

### Comparing `zksync2-0.5.0/examples/05_deploy_create_with_constructor.py` & `zksync2-0.6.0b1/examples/05_deploy_create_with_constructor.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,16 +49,15 @@
 
     # Get nonce of ETH address on zkSync network
     nonce = zk_web3.zksync.get_transaction_count(
         account.address, EthBlockParams.PENDING.value
     )
 
     # Get deployment nonce
-    nonce_holder = NonceHolder(zk_web3, account)
-    deployment_nonce = nonce_holder.get_deployment_nonce(account.address)
+    deployment_nonce = NonceHolder(zk_web3, account).get_deployment_nonce(account.address)
 
     # Precompute the address of smart contract
     # Use this if there is a case where contract address should be known before deployment
     deployer = PrecomputeContractDeployer(zk_web3)
     precomputed_address = deployer.compute_l2_create_address(account.address, deployment_nonce)
 
     # Get contract ABI and bytecode information
@@ -72,15 +71,14 @@
 
     # Create deployment contract transaction
     create_contract = TxCreateContract(
         web3=zk_web3,
         chain_id=chain_id,
         nonce=nonce,
         from_=account.address,
-        gas_limit=0,  # UNKNOWN AT THIS STATE,
         gas_price=gas_price,
         bytecode=incrementer_contract.bytecode,
         call_data=encoded_constructor,
     )
 
     # ZkSync transaction gas estimation
     estimate_gas = zk_web3.zksync.eth_estimate_gas(create_contract.tx)
@@ -101,15 +99,15 @@
     # Wait for deployment contract transaction to be included in a block
     tx_receipt = zk_web3.zksync.wait_for_transaction_receipt(
         tx_hash, timeout=240, poll_latency=0.5
     )
 
     print(f"Tx status: {tx_receipt['status']}")
     contract_address = tx_receipt["contractAddress"]
-    print(f"contract address: {contract_address}")
+    print(f"Contract address: {contract_address}")
 
     # Check does precompute address match with deployed address
     if precomputed_address.lower() != contract_address.lower():
         raise RuntimeError("Precomputed contract address does now match with deployed contract address")
 
     return contract_address
```

### Comparing `zksync2-0.5.0/examples/06_deploy_create_with_deps.py` & `zksync2-0.6.0b1/examples/06_deploy_create_with_deps.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,15 +62,14 @@
     gas_price = zk_web3.zksync.gas_price
 
     # Create deployment contract transaction
     create_contract = TxCreateContract(web3=zk_web3,
                                        chain_id=chain_id,
                                        nonce=nonce,
                                        from_=account.address,
-                                       gas_limit=0,
                                        gas_price=gas_price,
                                        bytecode=demo_contract.bytecode,
                                        deps=[foo_contract.bytecode])
 
     # ZkSync transaction gas estimation
     estimate_gas = zk_web3.zksync.eth_estimate_gas(create_contract.tx)
     print(f"Fee for transaction is: {Web3.from_wei(estimate_gas * gas_price, 'ether')} ETH")
@@ -90,15 +89,15 @@
     # Wait for deployment contract transaction to be included in a block
     tx_receipt = zk_web3.zksync.wait_for_transaction_receipt(
         tx_hash, timeout=240, poll_latency=0.5
     )
 
     print(f"Tx status: {tx_receipt['status']}")
     contract_address = tx_receipt["contractAddress"]
-    print(f"contract address: {contract_address}")
+    print(f"Contract address: {contract_address}")
 
     # Check does precompute address match with deployed address
     if precomputed_address.lower() != contract_address.lower():
         raise RuntimeError("Precomputed contract address does now match with deployed contract address")
 
 
 if __name__ == "__main__":
```

### Comparing `zksync2-0.5.0/examples/07_deploy_create2.py` & `zksync2-0.6.0b1/examples/07_deploy_create2.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,15 +96,15 @@
     # Wait for deployment contract transaction to be included in a block
     tx_receipt = zk_web3.zksync.wait_for_transaction_receipt(
         tx_hash, timeout=240, poll_latency=0.5
     )
 
     print(f"Tx status: {tx_receipt['status']}")
     contract_address = tx_receipt["contractAddress"]
-    print(f"contract address: {contract_address}")
+    print(f"Contract address: {contract_address}")
 
     # Check does precompute address match with deployed address
     if precomputed_address.lower() != contract_address.lower():
         raise RuntimeError("Precomputed contract address does now match with deployed contract address")
 
     return contract_address
```

### Comparing `zksync2-0.5.0/examples/08_deploy_create2_deps.py` & `zksync2-0.6.0b1/examples/08_deploy_create2_deps.py`

 * *Files 0% similar despite different names*

```diff
@@ -96,15 +96,15 @@
     # Wait for deployment contract transaction to be included in a block
     tx_receipt = zk_web3.zksync.wait_for_transaction_receipt(
         tx_hash, timeout=240, poll_latency=0.5
     )
 
     print(f"Tx status: {tx_receipt['status']}")
     contract_address = tx_receipt["contractAddress"]
-    print(f"contract address: {contract_address}")
+    print(f"Contract address: {contract_address}")
 
     # Check does precompute address match with deployed address
     if precomputed_address.lower() != contract_address.lower():
         raise RuntimeError("Precomputed contract address does now match with deployed contract address")
 
     return contract_address
```

### Comparing `zksync2-0.5.0/examples/09_withdrawal.py` & `zksync2-0.6.0b1/examples/09_withdrawal.py`

 * *Files identical despite different names*

### Comparing `zksync2-0.5.0/examples/10_finalize_withdrawal.py` & `zksync2-0.6.0b1/examples/10_finalize_withdrawal.py`

 * *Files identical despite different names*

### Comparing `zksync2-0.5.0/examples/11_check_balance.py` & `zksync2-0.6.0b1/examples/11_check_balance.py`

 * *Files identical despite different names*

### Comparing `zksync2-0.5.0/examples/README.md` & `zksync2-0.6.0b1/examples/README.md`

 * *Files identical despite different names*

### Comparing `zksync2-0.5.0/examples/solidity/demo/build/combined.json` & `zksync2-0.6.0b1/examples/solidity/demo/build/combined.json`

 * *Files identical despite different names*

### Comparing `zksync2-0.5.0/examples/solidity/incrementer/build/combined.json` & `zksync2-0.6.0b1/examples/solidity/incrementer/build/combined.json`

 * *Files identical despite different names*

### Comparing `zksync2-0.5.0/examples/solidity/storage/build/combined.json` & `zksync2-0.6.0b1/examples/solidity/storage/build/combined.json`

 * *Files identical despite different names*

### Comparing `zksync2-0.5.0/pyproject.toml` & `zksync2-0.6.0b1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "zksync2"
-version = "0.5.0"
+version = "0.6.0-beta.1"
 authors = [
   { name="Danijel Radakovic", email="danijel@txfusion.io" },
 ]
 description = "zkSync2 python client sdk"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `zksync2-0.5.0/setup.cfg` & `zksync2-0.6.0b1/setup.cfg`

 * *Files identical despite different names*

### Comparing `zksync2-0.5.0/tests/contracts/Counter.json` & `zksync2-0.6.0b1/tests/contracts/Counter.json`

 * *Files identical despite different names*

### Comparing `zksync2-0.5.0/tests/contracts/CustomAccount.json` & `zksync2-0.6.0b1/tests/contracts/CustomAccount.json`

 * *Files identical despite different names*

### Comparing `zksync2-0.5.0/tests/contracts/CustomPaymaster.json` & `zksync2-0.6.0b1/tests/contracts/CustomPaymaster.json`

 * *Files identical despite different names*

### Comparing `zksync2-0.5.0/tests/contracts/Foo.json` & `zksync2-0.6.0b1/tests/contracts/Foo.json`

 * *Files identical despite different names*

### Comparing `zksync2-0.5.0/tests/contracts/Import.json` & `zksync2-0.6.0b1/tests/contracts/Import.json`

 * *Files identical despite different names*

### Comparing `zksync2-0.5.0/tests/contracts/SimpleConstructor.json` & `zksync2-0.6.0b1/tests/contracts/SimpleConstructor.json`

 * *Files identical despite different names*

### Comparing `zksync2-0.5.0/tests/contracts/SomeERC20.json` & `zksync2-0.6.0b1/tests/contracts/SomeERC20.json`

 * *Files identical despite different names*

### Comparing `zksync2-0.5.0/tests/integration/test_config.py` & `zksync2-0.6.0b1/tests/integration/test_config.py`

 * *Files identical despite different names*

### Comparing `zksync2-0.5.0/tests/integration/test_deposit.py` & `zksync2-0.6.0b1/tests/integration/test_deposit.py`

 * *Files identical despite different names*

### Comparing `zksync2-0.5.0/tests/integration/test_paymaster.py` & `zksync2-0.6.0b1/tests/integration/test_paymaster.py`

 * *Files identical despite different names*

### Comparing `zksync2-0.5.0/tests/integration/test_transfer.py` & `zksync2-0.6.0b1/tests/integration/test_transfer.py`

 * *Files identical despite different names*

### Comparing `zksync2-0.5.0/tests/integration/test_withdraw.py` & `zksync2-0.6.0b1/tests/integration/test_withdraw.py`

 * *Files identical despite different names*

### Comparing `zksync2-0.5.0/tests/integration/test_zksync_contract.py` & `zksync2-0.6.0b1/tests/integration/test_zksync_contract.py`

 * *Files identical despite different names*

### Comparing `zksync2-0.5.0/tests/integration/test_zksync_web3.py` & `zksync2-0.6.0b1/tests/integration/test_zksync_web3.py`

 * *Files identical despite different names*

### Comparing `zksync2-0.5.0/tests/unit/test_config.py` & `zksync2-0.6.0b1/tests/unit/test_config.py`

 * *Files identical despite different names*

### Comparing `zksync2-0.5.0/tests/unit/test_contract_deploy.py` & `zksync2-0.6.0b1/tests/unit/test_contract_deploy.py`

 * *Files identical despite different names*

### Comparing `zksync2-0.5.0/tests/unit/test_eip712.py` & `zksync2-0.6.0b1/tests/unit/test_eip712.py`

 * *Files identical despite different names*

### Comparing `zksync2-0.5.0/tests/unit/test_eth_signer.py` & `zksync2-0.6.0b1/tests/unit/test_eth_signer.py`

 * *Files identical despite different names*

### Comparing `zksync2-0.5.0/tests/unit/test_transaction712.py` & `zksync2-0.6.0b1/tests/unit/test_transaction712.py`

 * *Files identical despite different names*

### Comparing `zksync2-0.5.0/zksync2/core/types.py` & `zksync2-0.6.0b1/zksync2/core/types.py`

 * *Files 3% similar despite different names*

```diff
@@ -83,7 +83,12 @@
     sources: Dict[str, ContractSourceDebugInfo]
 
 
 @dataclass
 class PaymasterParams(dict):
     paymaster: HexStr
     paymaster_input: bytes
+
+
+class AccountAbstractionVersion(Enum):
+    NONE = 0
+    VERSION_1 = 1
```

### Comparing `zksync2-0.5.0/zksync2/core/utils.py` & `zksync2-0.6.0b1/zksync2/core/utils.py`

 * *Files identical despite different names*

### Comparing `zksync2-0.5.0/zksync2/manage_contracts/contract_abi/ContractDeployer.json` & `zksync2-0.6.0b1/zksync2/manage_contracts/contract_abi/ContractDeployer.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9298148148148149%*

 * *Differences: {"'abi'": "{3: {'inputs': {0: {'name': '_salt'}}}, 12: {'stateMutability': 'view'}, insert: [(0, "*

 * *          "OrderedDict([('anonymous', False), ('inputs', [OrderedDict([('indexed', True), "*

 * *          "('internalType', 'address'), ('name', 'accountAddress'), ('type', 'address')]), "*

 * *          "OrderedDict([('indexed', False), ('internalType', 'enum "*

 * *          "IContractDeployer.AccountNonceOrdering'), ('name', 'nonceOrdering'), ('type', "*

 * *          "'uint8')])]), ('name', 'AccountNonceOrderingUpdated'), (' […]*

```diff
@@ -2,14 +2,52 @@
     "abi": [
         {
             "anonymous": false,
             "inputs": [
                 {
                     "indexed": true,
                     "internalType": "address",
+                    "name": "accountAddress",
+                    "type": "address"
+                },
+                {
+                    "indexed": false,
+                    "internalType": "enum IContractDeployer.AccountNonceOrdering",
+                    "name": "nonceOrdering",
+                    "type": "uint8"
+                }
+            ],
+            "name": "AccountNonceOrderingUpdated",
+            "type": "event"
+        },
+        {
+            "anonymous": false,
+            "inputs": [
+                {
+                    "indexed": true,
+                    "internalType": "address",
+                    "name": "accountAddress",
+                    "type": "address"
+                },
+                {
+                    "indexed": false,
+                    "internalType": "enum IContractDeployer.AccountAbstractionVersion",
+                    "name": "aaVersion",
+                    "type": "uint8"
+                }
+            ],
+            "name": "AccountVersionUpdated",
+            "type": "event"
+        },
+        {
+            "anonymous": false,
+            "inputs": [
+                {
+                    "indexed": true,
+                    "internalType": "address",
                     "name": "deployerAddress",
                     "type": "address"
                 },
                 {
                     "indexed": true,
                     "internalType": "bytes32",
                     "name": "bytecodeHash",
@@ -25,15 +63,15 @@
             "name": "ContractDeployed",
             "type": "event"
         },
         {
             "inputs": [
                 {
                     "internalType": "bytes32",
-                    "name": "",
+                    "name": "_salt",
                     "type": "bytes32"
                 },
                 {
                     "internalType": "bytes32",
                     "name": "_bytecodeHash",
                     "type": "bytes32"
                 },
@@ -337,15 +375,15 @@
             "outputs": [
                 {
                     "internalType": "address",
                     "name": "newAddress",
                     "type": "address"
                 }
             ],
-            "stateMutability": "pure",
+            "stateMutability": "view",
             "type": "function"
         },
         {
             "inputs": [
                 {
                     "internalType": "enum IContractDeployer.AccountAbstractionVersion",
                     "name": "_version",
```

### Comparing `zksync2-0.5.0/zksync2/manage_contracts/contract_abi/IERC20.json` & `zksync2-0.6.0b1/zksync2/manage_contracts/contract_abi/IERC20.json`

 * *Files identical despite different names*

### Comparing `zksync2-0.5.0/zksync2/manage_contracts/contract_abi/IEthToken.json` & `zksync2-0.6.0b1/zksync2/manage_contracts/contract_abi/IEthToken.json`

 * *Files identical despite different names*

### Comparing `zksync2-0.5.0/zksync2/manage_contracts/contract_abi/IL1Bridge.json` & `zksync2-0.6.0b1/zksync2/manage_contracts/contract_abi/IL1Bridge.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9419560185185185%*

 * *Differences: {"'abi'": "{1: {'inputs': {3: {'indexed': False}, insert: [(0, OrderedDict([('indexed', True), "*

 * *          "('internalType', 'bytes32'), ('name', 'l2DepositTxHash'), ('type', 'bytes32')]))]}}, 4: "*

 * *          "{'inputs': {insert: [(5, OrderedDict([('internalType', 'address'), ('name', "*

 * *          "'_refundRecipient'), ('type', 'address')]))]}}, insert: [(7, OrderedDict([('inputs', "*

 * *          "[]), ('name', 'l2Bridge'), ('outputs', [OrderedDict([('internalType', 'address'), "*

 * *          "('name', ''), ('type' […]*

```diff
@@ -26,26 +26,32 @@
             "type": "event"
         },
         {
             "anonymous": false,
             "inputs": [
                 {
                     "indexed": true,
+                    "internalType": "bytes32",
+                    "name": "l2DepositTxHash",
+                    "type": "bytes32"
+                },
+                {
+                    "indexed": true,
                     "internalType": "address",
                     "name": "from",
                     "type": "address"
                 },
                 {
                     "indexed": true,
                     "internalType": "address",
                     "name": "to",
                     "type": "address"
                 },
                 {
-                    "indexed": true,
+                    "indexed": false,
                     "internalType": "address",
                     "name": "l1Token",
                     "type": "address"
                 },
                 {
                     "indexed": false,
                     "internalType": "uint256",
@@ -146,14 +152,19 @@
                     "name": "_l2TxGasLimit",
                     "type": "uint256"
                 },
                 {
                     "internalType": "uint256",
                     "name": "_l2TxGasPerPubdataByte",
                     "type": "uint256"
+                },
+                {
+                    "internalType": "address",
+                    "name": "_refundRecipient",
+                    "type": "address"
                 }
             ],
             "name": "deposit",
             "outputs": [
                 {
                     "internalType": "bytes32",
                     "name": "txHash",
@@ -217,14 +228,27 @@
                     "type": "bool"
                 }
             ],
             "stateMutability": "view",
             "type": "function"
         },
         {
+            "inputs": [],
+            "name": "l2Bridge",
+            "outputs": [
+                {
+                    "internalType": "address",
+                    "name": "",
+                    "type": "address"
+                }
+            ],
+            "stateMutability": "view",
+            "type": "function"
+        },
+        {
             "inputs": [
                 {
                     "internalType": "address",
                     "name": "_l1Token",
                     "type": "address"
                 }
             ],
```

### Comparing `zksync2-0.5.0/zksync2/manage_contracts/contract_abi/IL2Bridge.json` & `zksync2-0.6.0b1/zksync2/manage_contracts/contract_abi/IL2Bridge.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9928571428571429%*

 * *Differences: {"'abi'": "{2: {'stateMutability': 'payable'}}"}*

```diff
@@ -88,15 +88,15 @@
                     "internalType": "bytes",
                     "name": "_data",
                     "type": "bytes"
                 }
             ],
             "name": "finalizeDeposit",
             "outputs": [],
-            "stateMutability": "nonpayable",
+            "stateMutability": "payable",
             "type": "function"
         },
         {
             "inputs": [],
             "name": "l1Bridge",
             "outputs": [
                 {
```

### Comparing `zksync2-0.5.0/zksync2/manage_contracts/contract_abi/INonceHolder.json` & `zksync2-0.6.0b1/zksync2/manage_contracts/contract_abi/INonceHolder.json`

 * *Files identical despite different names*

### Comparing `zksync2-0.5.0/zksync2/manage_contracts/contract_abi/IPaymasterFlow.json` & `zksync2-0.6.0b1/zksync2/manage_contracts/contract_abi/IPaymasterFlow.json`

 * *Files identical despite different names*

### Comparing `zksync2-0.5.0/zksync2/manage_contracts/contract_abi/IZkSync.json` & `zksync2-0.6.0b1/zksync2/manage_contracts/contract_abi/IZkSync.json`

 * *Files identical despite different names*

### Comparing `zksync2-0.5.0/zksync2/manage_contracts/contract_encoder_base.py` & `zksync2-0.6.0b1/zksync2/manage_contracts/contract_encoder_base.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,33 @@
 import json
+from enum import Enum
 from pathlib import Path
 from typing import Any, Optional
 from eth_typing import HexStr
 from eth_utils import remove_0x_prefix
 from web3 import Web3
 from web3._utils.abi import get_constructor_abi, merge_args_and_kwargs
 from web3._utils.contracts import encode_abi
 
 
+class JsonConfiguration(Enum):
+    COMBINED = "combined"
+    STANDARD = "standard"
+
+
 class BaseContractEncoder:
 
     @classmethod
-    def from_json(cls, web3: Web3, compiled_contract: Path):
+    def from_json(cls, web3: Web3, compiled_contract: Path, conf_type: JsonConfiguration = JsonConfiguration.COMBINED):
         with compiled_contract.open(mode='r') as json_f:
             data = json.load(json_f)
-            return cls(web3, abi=data["abi"])
+            if conf_type == JsonConfiguration.COMBINED:
+                return [cls(web3, abi=v["abi"], bytecode=v["bin"]) for k, v in data["contracts"].items()]
+            else:
+                return cls(web3, abi=data["abi"], bytecode=data["bytecode"])
 
     def __init__(self, web3: Web3, abi, bytecode: Optional[bytes] = None):
         self.web3 = web3
         self.abi = abi
         if bytecode is None:
             self.instance_contract = self.web3.eth.contract(abi=self.abi)
         else:
@@ -30,22 +39,14 @@
     @property
     def contract(self):
         return self.instance_contract
 
 
 class ContractEncoder(BaseContractEncoder):
 
-    @classmethod
-    def from_json(cls, web3: Web3, compiled_contract: Path):
-        with compiled_contract.open(mode='r') as json_f:
-            data = json.load(json_f)
-            # bytecode = bytes.fromhex(remove_0x_prefix(data["bytecode"]))
-            # return cls(web3, abi=data["abi"], bytecode=bytecode)
-            return [cls(web3, abi=v["abi"], bytecode=v["bin"]) for k, v in data["contracts"].items()]
-
     def __init__(self, web3: Web3, abi, bytecode):
         super(ContractEncoder, self).__init__(web3, abi, bytecode)
 
     def encode_constructor(self, *args: Any, **kwargs: Any) -> bytes:
         constructor_abi = get_constructor_abi(self.abi)
 
         if constructor_abi:
```

### Comparing `zksync2-0.5.0/zksync2/manage_contracts/contract_factory.py` & `zksync2-0.6.0b1/zksync2/manage_contracts/contract_factory.py`

 * *Files identical despite different names*

### Comparing `zksync2-0.5.0/zksync2/manage_contracts/erc20_contract.py` & `zksync2-0.6.0b1/zksync2/manage_contracts/erc20_contract.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from web3.types import TxReceipt
 from zksync2.manage_contracts.contract_encoder_base import BaseContractEncoder
 from zksync2.manage_contracts import contract_abi
 
 erc_20_abi_cache = None
 
 
-def _erc_20_abi_default():
+def get_erc20_abi():
     global erc_20_abi_cache
 
     if erc_20_abi_cache is None:
         with pkg_resources.path(contract_abi, "IERC20.json") as p:
             with p.open(mode='r') as json_file:
                 data = json.load(json_file)
                 erc_20_abi_cache = data['abi']
@@ -29,15 +29,15 @@
 
     def __init__(self, web3: Module,
                  contract_address: HexStr,
                  account: BaseAccount):
         check_sum_address = Web3.to_checksum_address(contract_address)
         self.contract_address = check_sum_address
         self.module = web3
-        self.contract = self.module.contract(self.contract_address, abi=_erc_20_abi_default())
+        self.contract = self.module.contract(self.contract_address, abi=get_erc20_abi())
         self.account = account
 
     def _nonce(self) -> int:
         return self.module.get_transaction_count(self.account.address)
 
     def approve(self,
                 zksync_address: HexStr,
@@ -81,9 +81,9 @@
             })
 
 
 class ERC20Encoder(BaseContractEncoder):
 
     def __init__(self, web3: Web3, abi: Optional[dict] = None):
         if abi is None:
-            abi = _erc_20_abi_default()
+            abi = get_erc20_abi()
         super(ERC20Encoder, self).__init__(web3, abi)
```

### Comparing `zksync2-0.5.0/zksync2/manage_contracts/eth_token.py` & `zksync2-0.6.0b1/zksync2/manage_contracts/eth_token.py`

 * *Files identical despite different names*

### Comparing `zksync2-0.5.0/zksync2/manage_contracts/l1_bridge.py` & `zksync2-0.6.0b1/zksync2/manage_contracts/l1_bridge.py`

 * *Files identical despite different names*

### Comparing `zksync2-0.5.0/zksync2/manage_contracts/l2_bridge.py` & `zksync2-0.6.0b1/zksync2/manage_contracts/l2_bridge.py`

 * *Files identical despite different names*

### Comparing `zksync2-0.5.0/zksync2/manage_contracts/nonce_holder.py` & `zksync2-0.6.0b1/zksync2/manage_contracts/nonce_holder.py`

 * *Files identical despite different names*

### Comparing `zksync2-0.5.0/zksync2/manage_contracts/paymaster_utils.py` & `zksync2-0.6.0b1/zksync2/manage_contracts/paymaster_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,11 +21,11 @@
 
 class PaymasterFlowEncoder(BaseContractEncoder):
 
     def __init__(self, web3: Web3):
         super(PaymasterFlowEncoder, self).__init__(web3, abi=_paymaster_flow_abi_default())
 
     def encode_approval_based(self, address: HexStr, min_allowance: int, inner_input: bytes) -> HexStr:
-        return self.encode_method(fn_name="approvalBased", args=[address, min_allowance, inner_input])
+        return self.encode_method(fn_name="approvalBased", args=(address, min_allowance, inner_input))
 
     def encode_general(self, inputs: bytes) -> HexStr:
-        return self.encode_method(fn_name="general", args=[inputs])
+        return self.encode_method(fn_name="general", args=tuple([inputs]))
```

### Comparing `zksync2-0.5.0/zksync2/manage_contracts/precompute_contract_deployer.py` & `zksync2-0.6.0b1/zksync2/manage_contracts/precompute_contract_deployer.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import importlib.resources as pkg_resources
-from eth_typing import HexStr
-from web3 import Web3
-from typing import Optional
 import json
+from typing import Optional
 
+from eth_typing import HexStr
+from eth_utils.crypto import keccak
+from web3 import Web3
 from web3.logs import DISCARD
 from web3.types import Nonce, TxReceipt
-from eth_utils.crypto import keccak
-from zksync2.manage_contracts import contract_abi
+
+from zksync2.core.types import AccountAbstractionVersion
 from zksync2.core.utils import pad_front_bytes, to_bytes, int_to_bytes, hash_byte_code
+from zksync2.manage_contracts import contract_abi
 from zksync2.manage_contracts.contract_encoder_base import BaseContractEncoder
 
 icontract_deployer_abi_cache = None
 
 
 def _icontract_deployer_abi_default():
     global icontract_deployer_abi_cache
@@ -25,14 +27,16 @@
     return icontract_deployer_abi_cache
 
 
 class PrecomputeContractDeployer:
     DEFAULT_SALT = b'\0' * 32
     CREATE_FUNC = "create"
     CREATE2_FUNC = "create2"
+    CREATE_ACCOUNT_FUNC = "createAccount"
+    CREATE2_ACCOUNT_FUNC = "create2Account"
     MAX_BYTE_CODE_LENGTH = 2 ** 16
     EMPTY_BYTES = b''
 
     CREATE_PREFIX = keccak(text="zksyncCreate")
     CREATE2_PREFIX = keccak(text="zksyncCreate2")
 
     def __init__(self, web3: Web3, abi: Optional[dict] = None):
@@ -54,27 +58,52 @@
             raise OverflowError("Salt data must be 32 length")
 
         bytecode_hash = hash_byte_code(bytecode)
         args = salt, bytecode_hash, call_data
 
         return self.contract_encoder.encode_method(fn_name=self.CREATE2_FUNC, args=args)
 
-    def encode_create(self, bytecode: bytes, call_data: Optional[bytes] = None, salt_data: Optional[bytes] = None):
-        if salt_data is None:
-            salt_data = self.DEFAULT_SALT
+    def encode_create(self, bytecode: bytes, call_data: Optional[bytes] = None) -> HexStr:
         if call_data is None:
             call_data = self.EMPTY_BYTES
 
-        if len(salt_data) != 32:
+        bytecode_hash = hash_byte_code(bytecode)
+        args = self.DEFAULT_SALT, bytecode_hash, call_data
+
+        return self.contract_encoder.encode_method(fn_name=self.CREATE_FUNC, args=args)
+
+    def encode_create2_account(self, bytecode: bytes,
+                               call_data: Optional[bytes] = None,
+                               salt: Optional[bytes] = None,
+                               version: AccountAbstractionVersion = AccountAbstractionVersion.VERSION_1
+                               ) -> HexStr:
+        if salt is None:
+            salt = self.DEFAULT_SALT
+        if call_data is None:
+            call_data = self.EMPTY_BYTES
+
+        if len(salt) != 32:
             raise OverflowError("Salt data must be 32 length")
 
         bytecode_hash = hash_byte_code(bytecode)
-        args = salt_data, bytecode_hash, call_data
+        args = salt, bytecode_hash, call_data, version.value
 
-        return self.contract_encoder.encode_method(fn_name=self.CREATE_FUNC, args=args)
+        return self.contract_encoder.encode_method(fn_name=self.CREATE2_ACCOUNT_FUNC, args=args)
+
+    def encode_create_account(self, bytecode: bytes,
+                              call_data: Optional[bytes] = None,
+                              version: AccountAbstractionVersion = AccountAbstractionVersion.VERSION_1
+                              ) -> HexStr:
+        if call_data is None:
+            call_data = self.EMPTY_BYTES
+
+        bytecode_hash = hash_byte_code(bytecode)
+        args = self.DEFAULT_SALT, bytecode_hash, call_data, version.value
+
+        return self.contract_encoder.encode_method(fn_name=self.CREATE_ACCOUNT_FUNC, args=args)
 
     def compute_l2_create_address(self, sender: HexStr, nonce: Nonce) -> HexStr:
         sender_bytes = to_bytes(sender)
         sender_bytes = pad_front_bytes(sender_bytes, 32)
         nonce = int_to_bytes(nonce)
         nonce_bytes = pad_front_bytes(nonce, 32)
         result = self.CREATE_PREFIX + sender_bytes + nonce_bytes
@@ -83,15 +112,15 @@
         address = "0x" + address.hex()
         return HexStr(Web3.to_checksum_address(address))
 
     def compute_l2_create2_address(self,
                                    sender: HexStr,
                                    bytecode: bytes,
                                    constructor: bytes,
-                                   salt: bytes):
+                                   salt: bytes) -> HexStr:
         if len(salt) != 32:
             raise OverflowError("Salt data must be 32 length")
 
         sender_bytes = to_bytes(sender)
         sender_bytes = pad_front_bytes(sender_bytes, 32)
         bytecode_hash = hash_byte_code(bytecode)
         ctor_hash = keccak(constructor)
@@ -102,8 +131,7 @@
         return HexStr(Web3.to_checksum_address(address))
 
     def extract_contract_address(self, receipt: TxReceipt) -> HexStr:
         result = self.contract_encoder.contract.events.ContractDeployed().process_receipt(receipt, errors=DISCARD)
         entry = result[1]["args"]
         addr = entry["contractAddress"]
         return addr
-
```

### Comparing `zksync2-0.5.0/zksync2/manage_contracts/zksync_contract.py` & `zksync2-0.6.0b1/zksync2/manage_contracts/zksync_contract.py`

 * *Files identical despite different names*

### Comparing `zksync2-0.5.0/zksync2/module/middleware.py` & `zksync2-0.6.0b1/zksync2/module/middleware.py`

 * *Files identical despite different names*

### Comparing `zksync2-0.5.0/zksync2/module/module_builder.py` & `zksync2-0.6.0b1/zksync2/module/module_builder.py`

 * *Files identical despite different names*

### Comparing `zksync2-0.5.0/zksync2/module/request_types.py` & `zksync2-0.6.0b1/zksync2/module/request_types.py`

 * *Files identical despite different names*

### Comparing `zksync2-0.5.0/zksync2/module/response_types.py` & `zksync2-0.6.0b1/zksync2/module/response_types.py`

 * *Files identical despite different names*

### Comparing `zksync2-0.5.0/zksync2/module/zksync_module.py` & `zksync2-0.6.0b1/zksync2/module/zksync_module.py`

 * *Files identical despite different names*

### Comparing `zksync2-0.5.0/zksync2/module/zksync_provider.py` & `zksync2-0.6.0b1/zksync2/module/zksync_provider.py`

 * *Files identical despite different names*

### Comparing `zksync2-0.5.0/zksync2/provider/eth_provider.py` & `zksync2-0.6.0b1/zksync2/provider/eth_provider.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,20 +70,20 @@
     def l2_token_address(self, token: Token):
         if token.is_eth():
             return token.l1_address
         else:
             return self.l1_bridge.l2_token_address(token.l1_address)
 
     def get_base_cost(self,
-                      gas_limit: int,
+                      l2_gas_limit: int,
                       gas_per_pubdata_byte: int = DEPOSIT_GAS_PER_PUBDATA_LIMIT,
                       gas_price: int = None):
         if gas_price is None:
             gas_price = self._eth_web3.eth.gas_price
-        return self.main_contract.l2_tx_base_cost(gas_price, gas_limit, gas_per_pubdata_byte)
+        return self.main_contract.l2_tx_base_cost(gas_price, l2_gas_limit, gas_per_pubdata_byte)
 
     def approve_erc20(self,
                       token: Token,
                       amount: int,
                       bridge_address: HexStr = None,
                       gas_limit: int = None) -> TxReceipt:
         if token.is_eth():
@@ -102,15 +102,15 @@
     def deposit(self,
                 token: Token,
                 amount: int,
                 to: HexStr = None,
                 operator_tip: int = 0,
                 bridge_address: HexStr = None,
                 approve_erc20: bool = False,
-                l2_gas_limit: int = RECOMMENDED_DEPOSIT_L2_GAS_LIMIT,
+                l2_gas_limit: int = RecommendedGasLimit.DEPOSIT.value,
                 gas_per_pubdata_byte: int = DEPOSIT_GAS_PER_PUBDATA_LIMIT,
                 gas_price: int = None,
                 gas_limit: int = None
                 ):
         bridge_contract = self.l1_bridge
         if bridge_address is not None:
             bridge_contract = L1Bridge(bridge_address,
@@ -123,15 +123,15 @@
         if gas_price is None:
             gas_price = self._eth_web3.eth.gas_price
         if gas_limit is None:
             gas_limit = RecommendedGasLimit.DEPOSIT.value
 
         base_cost = self.get_base_cost(gas_price=gas_price,
                                        gas_per_pubdata_byte=gas_per_pubdata_byte,
-                                       gas_limit=gas_limit)
+                                       l2_gas_limit=l2_gas_limit)
 
         if token.is_eth():
             value = base_cost + operator_tip + amount
             return self.request_execute(
                 contract_address=to,
                 call_data=HexStr("0x"),
                 l2_gas_limit=l2_gas_limit,
@@ -174,15 +174,15 @@
         if refund_recipient is None:
             refund_recipient = self.address
         if gas_price is None:
             gas_price = self._eth_web3.eth.gas_price
 
         base_cost = self.get_base_cost(gas_price=gas_price,
                                        gas_per_pubdata_byte=gas_per_pubdata_byte,
-                                       gas_limit=gas_limit)
+                                       l2_gas_limit=l2_gas_limit)
         value = base_cost + operator_tip + l2_value
         check_base_cost(base_cost, value)
 
         call_data = to_bytes(call_data)
 
         tx_receipt = self.main_contract.request_l2_transaction(contract_l2=contract_address,
                                                                l2_value=l2_value,
```

### Comparing `zksync2-0.5.0/zksync2/signer/eth_signer.py` & `zksync2-0.6.0b1/zksync2/signer/eth_signer.py`

 * *Files identical despite different names*

### Comparing `zksync2-0.5.0/zksync2/transaction/transaction712.py` & `zksync2-0.6.0b1/zksync2/transaction/transaction712.py`

 * *Files identical despite different names*

### Comparing `zksync2-0.5.0/zksync2/transaction/transaction_builders.py` & `zksync2-0.6.0b1/zksync2/transaction/transaction_builders.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 from abc import ABC
 from typing import Optional, List
+
 from eth_account.signers.base import BaseAccount
 from eth_typing import HexStr
 from web3 import Web3
 from web3.types import Nonce
+
 from zksync2.core.types import Token, BridgeAddresses, L2_ETH_TOKEN_ADDRESS
-from zksync2.manage_contracts.precompute_contract_deployer import PrecomputeContractDeployer
 from zksync2.manage_contracts.deploy_addresses import ZkSyncAddresses
 from zksync2.manage_contracts.eth_token import EthToken
 from zksync2.manage_contracts.l2_bridge import L2Bridge
-from zksync2.transaction.transaction712 import Transaction712
+from zksync2.manage_contracts.precompute_contract_deployer import PrecomputeContractDeployer
 from zksync2.module.request_types import EIP712Meta, TransactionType, Transaction as ZkTx
+from zksync2.transaction.transaction712 import Transaction712
 
 
 class TxBase(ABC):
 
     def __init__(self, trans: ZkTx):
         self.tx_: ZkTx = trans
 
@@ -42,52 +44,55 @@
                  nonce: int,
                  from_: HexStr,
                  to: HexStr,
                  value: int = 0,
                  data: HexStr = HexStr("0x"),
                  gas_limit: int = 0,
                  gas_price: int = 0,
-                 max_priority_fee_per_gas=100000000):
-        default_meta = EIP712Meta()
+                 max_priority_fee_per_gas=100_000_000,
+                 paymaster_params=None,
+                 custom_signature=None):
+        eip712_meta = EIP712Meta(gas_per_pub_data=EIP712Meta.GAS_PER_PUB_DATA_DEFAULT,
+                                 custom_signature=custom_signature,
+                                 factory_deps=None,
+                                 paymaster_params=paymaster_params)
+
         super(TxFunctionCall, self).__init__(
             trans={
                 "chain_id": chain_id,
                 "nonce": nonce,
                 "from": from_,
                 "to": to,
                 "gas": gas_limit,
                 "gasPrice": gas_price,
                 "maxPriorityFeePerGas": max_priority_fee_per_gas,
                 "value": value,
                 "data": data,
                 "transactionType": TransactionType.EIP_712_TX_TYPE.value,
-                "eip712Meta": default_meta
+                "eip712Meta": eip712_meta
             })
 
 
 class TxCreateContract(TxBase, ABC):
 
     def __init__(self,
                  web3: Web3,
                  chain_id: int,
                  nonce: int,
                  from_: HexStr,
-                 gas_limit: int,
-                 gas_price: int,
                  bytecode: bytes,
+                 gas_price: int,
+                 gas_limit: int = 0,
                  deps: List[bytes] = None,
                  call_data: Optional[bytes] = None,
                  value: int = 0,
-                 max_priority_fee_per_gas=100000000,
-                 salt: Optional[bytes] = None):
-
+                 max_priority_fee_per_gas=100_000_000
+                 ):
         contract_deployer = PrecomputeContractDeployer(web3)
-        generated_call_data = contract_deployer.encode_create(bytecode=bytecode,
-                                                              call_data=call_data,
-                                                              salt_data=salt)
+        generated_call_data = contract_deployer.encode_create(bytecode=bytecode, call_data=call_data)
         factory_deps = []
         if deps is not None:
             for dep in deps:
                 factory_deps.append(dep)
         factory_deps.append(bytecode)
         eip712_meta = EIP712Meta(gas_per_pub_data=EIP712Meta.GAS_PER_PUB_DATA_DEFAULT,
                                  custom_signature=None,
@@ -118,15 +123,15 @@
                  from_: HexStr,
                  gas_limit: int,
                  gas_price: int,
                  bytecode: bytes,
                  deps: List[bytes] = None,
                  call_data: Optional[bytes] = None,
                  value: int = 0,
-                 max_priority_fee_per_gas=100000000,
+                 max_priority_fee_per_gas=100_000_000,
                  salt: Optional[bytes] = None
                  ):
         contract_deployer = PrecomputeContractDeployer(web3)
         generated_call_data = contract_deployer.encode_create2(bytecode=bytecode,
                                                                call_data=call_data,
                                                                salt=salt)
         factory_deps = []
@@ -143,14 +148,101 @@
             "chain_id": chain_id,
             "nonce": nonce,
             "from": from_,
             "to": Web3.to_checksum_address(ZkSyncAddresses.CONTRACT_DEPLOYER_ADDRESS.value),
             "gas": gas_limit,
             "gasPrice": gas_price,
             "maxPriorityFeePerGas": max_priority_fee_per_gas,
+            "value": value,
+            "data": HexStr(generated_call_data),
+            "transactionType": TransactionType.EIP_712_TX_TYPE.value,
+            "eip712Meta": eip712_meta
+        })
+
+
+class TxCreateAccount(TxBase, ABC):
+
+    def __init__(self,
+                 web3: Web3,
+                 chain_id: int,
+                 nonce: int,
+                 from_: HexStr,
+                 bytecode: bytes,
+                 gas_price: int,
+                 gas_limit: int = 0,
+                 deps: List[bytes] = None,
+                 call_data: Optional[bytes] = None,
+                 value: int = 0,
+                 max_priority_fee_per_gas=100_000_000
+                 ):
+        contract_deployer = PrecomputeContractDeployer(web3)
+        generated_call_data = contract_deployer.encode_create_account(bytecode=bytecode, call_data=call_data)
+        factory_deps = []
+        if deps is not None:
+            for dep in deps:
+                factory_deps.append(dep)
+        factory_deps.append(bytecode)
+        eip712_meta = EIP712Meta(gas_per_pub_data=EIP712Meta.GAS_PER_PUB_DATA_DEFAULT,
+                                 custom_signature=None,
+                                 factory_deps=factory_deps,
+                                 paymaster_params=None)
+
+        super(TxCreateAccount, self).__init__(trans={
+            "chain_id": chain_id,
+            "nonce": nonce,
+            "from": from_,
+            "to": Web3.to_checksum_address(ZkSyncAddresses.CONTRACT_DEPLOYER_ADDRESS.value),
+            "gas": gas_limit,
+            "gasPrice": gas_price,
+            "maxPriorityFeePerGas": max_priority_fee_per_gas,
+            "value": value,
+            "data": HexStr(generated_call_data),
+            "transactionType": TransactionType.EIP_712_TX_TYPE.value,
+            "eip712Meta": eip712_meta
+        })
+
+
+class TxCreate2Account(TxBase, ABC):
+
+    def __init__(self,
+                 web3: Web3,
+                 chain_id: int,
+                 nonce: int,
+                 from_: HexStr,
+                 gas_limit: int,
+                 gas_price: int,
+                 bytecode: bytes,
+                 deps: List[bytes] = None,
+                 call_data: Optional[bytes] = None,
+                 value: int = 0,
+                 max_priority_fee_per_gas=100_000_000,
+                 salt: Optional[bytes] = None
+                 ):
+        contract_deployer = PrecomputeContractDeployer(web3)
+        generated_call_data = contract_deployer.encode_create2_account(bytecode=bytecode,
+                                                                       call_data=call_data,
+                                                                       salt=salt)
+        factory_deps = []
+        if deps is not None:
+            for dep in deps:
+                factory_deps.append(dep)
+        factory_deps.append(bytecode)
+
+        eip712_meta = EIP712Meta(gas_per_pub_data=EIP712Meta.GAS_PER_PUB_DATA_DEFAULT,
+                                 custom_signature=None,
+                                 factory_deps=factory_deps,
+                                 paymaster_params=None)
+        super(TxCreate2Account, self).__init__(trans={
+            "chain_id": chain_id,
+            "nonce": nonce,
+            "from": from_,
+            "to": Web3.to_checksum_address(ZkSyncAddresses.CONTRACT_DEPLOYER_ADDRESS.value),
+            "gas": gas_limit,
+            "gasPrice": gas_price,
+            "maxPriorityFeePerGas": max_priority_fee_per_gas,
             "value": value,
             "data": HexStr(generated_call_data),
             "transactionType": TransactionType.EIP_712_TX_TYPE.value,
             "eip712Meta": eip712_meta
         })
```

### Comparing `zksync2-0.5.0/zksync2.egg-info/PKG-INFO` & `zksync2-0.6.0b1/zksync2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zksync2
-Version: 0.5.0
+Version: 0.6.0b1
 Summary: zkSync2 python client sdk
 Home-page: https://zksync.io
 Author: Danijel Radakovic
 Author-email: Danijel Radakovic <danijel@txfusion.io>
 License: MIT
 Project-URL: Homepage, https://github.com/zksync-sdk/zksync2-python
 Project-URL: Bug Tracker, https://github.com/zksync-sdk/zksync2-python/issues
```

### Comparing `zksync2-0.5.0/zksync2.egg-info/SOURCES.txt` & `zksync2-0.6.0b1/zksync2.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -13,16 +13,24 @@
 examples/05_deploy_create_with_constructor.py
 examples/06_deploy_create_with_deps.py
 examples/07_deploy_create2.py
 examples/08_deploy_create2_deps.py
 examples/09_withdrawal.py
 examples/10_finalize_withdrawal.py
 examples/11_check_balance.py
+examples/12_deploy_token.py
+examples/13_deploy_account_create.py
+examples/14_deploy_account_create2.py
+examples/15_use_paymaster.py
 examples/README.md
 examples/utils.py
+examples/solidity/custom_paymaster/Paymaster.sol
+examples/solidity/custom_paymaster/Token.sol
+examples/solidity/custom_paymaster/build/Paymaster.json
+examples/solidity/custom_paymaster/build/Token.json
 examples/solidity/demo/Demo.sol
 examples/solidity/demo/Foo.sol
 examples/solidity/demo/build/combined.json
 examples/solidity/incrementer/Incrementer.sol
 examples/solidity/incrementer/build/combined.json
 examples/solidity/storage/Storage.sol
 examples/solidity/storage/build/combined.json
@@ -68,17 +76,20 @@
 zksync2/manage_contracts/l1_bridge.py
 zksync2/manage_contracts/l2_bridge.py
 zksync2/manage_contracts/nonce_holder.py
 zksync2/manage_contracts/paymaster_utils.py
 zksync2/manage_contracts/precompute_contract_deployer.py
 zksync2/manage_contracts/zksync_contract.py
 zksync2/manage_contracts/contract_abi/ContractDeployer.json
+zksync2/manage_contracts/contract_abi/IAllowList.json
+zksync2/manage_contracts/contract_abi/IERC1271.json
 zksync2/manage_contracts/contract_abi/IERC20.json
 zksync2/manage_contracts/contract_abi/IEthToken.json
 zksync2/manage_contracts/contract_abi/IL1Bridge.json
+zksync2/manage_contracts/contract_abi/IL1Messenger.json
 zksync2/manage_contracts/contract_abi/IL2Bridge.json
 zksync2/manage_contracts/contract_abi/INonceHolder.json
 zksync2/manage_contracts/contract_abi/IPaymasterFlow.json
 zksync2/manage_contracts/contract_abi/IZkSync.json
 zksync2/manage_contracts/contract_abi/__init__.py
 zksync2/module/__init__.py
 zksync2/module/middleware.py
```

