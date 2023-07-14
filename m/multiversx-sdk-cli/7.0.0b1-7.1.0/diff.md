# Comparing `tmp/multiversx_sdk_cli-7.0.0b1.tar.gz` & `tmp/multiversx_sdk_cli-7.1.0.tar.gz`

## Comparing `multiversx_sdk_cli-7.0.0b1.tar` & `multiversx_sdk_cli-7.1.0.tar`

### file list

```diff
@@ -1,115 +1,115 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/__init__.py
--rw-r--r--   0        0        0     6432 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/accounts.py
--rw-r--r--   0        0        0     4010 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/cli.py
--rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/cli_accounts.py
--rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/cli_block.py
--rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/cli_config.py
--rw-r--r--   0        0        0    19784 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/cli_contracts.py
--rw-r--r--   0        0        0     3656 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/cli_data.py
--rw-r--r--   0        0        0    12580 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/cli_delegation.py
--rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/cli_deps.py
--rw-r--r--   0        0        0     5193 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/cli_dns.py
--rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/cli_ledger.py
--rw-r--r--   0        0        0     5875 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/cli_localnet.py
--rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/cli_network.py
--rw-r--r--   0        0        0     4126 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/cli_output.py
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/cli_password.py
--rw-r--r--   0        0        0    11873 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/cli_shared.py
--rw-r--r--   0        0        0     5242 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/cli_transactions.py
--rw-r--r--   0        0        0     8304 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/cli_validators.py
--rw-r--r--   0        0        0     9978 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/cli_wallet.py
--rw-r--r--   0        0        0     9707 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/config.py
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/constants.py
--rw-r--r--   0        0        0     5147 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/contract_verification.py
--rw-r--r--   0        0        0    10194 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/contracts.py
--rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/cosign_transaction.py
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/diskcache.py
--rw-r--r--   0        0        0     3394 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/dns.py
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/docker.py
--rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/downloader.py
--rw-r--r--   0        0        0     4881 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/errors.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/guards.py
--rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/interfaces.py
--rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/myprocess.py
--rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/simulation.py
--rw-r--r--   0        0        0    11018 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/transactions.py
--rw-r--r--   0        0        0     7223 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/utils.py
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/ux.py
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/version.py
--rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/workstation.py
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/.vscode/settings.json
--rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/delegation/__init__.py
--rw-r--r--   0        0        0     6511 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/delegation/staking_provider.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/dependencies/__init__.py
--rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/dependencies/install.py
--rw-r--r--   0        0        0    16479 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/dependencies/modules.py
--rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/dependencies/resolution.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/ledger/__init__.py
--rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/ledger/config.py
--rw-r--r--   0        0        0     5275 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/ledger/ledger_app_handler.py
--rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/ledger/ledger_functions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/localnet/__init__.py
--rw-r--r--   0        0        0     2375 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/localnet/config_default.py
--rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/localnet/config_general.py
--rw-r--r--   0        0        0     2060 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/localnet/config_networking.py
--rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/localnet/config_part.py
--rw-r--r--   0        0        0     6263 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/localnet/config_root.py
--rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/localnet/config_sharding.py
--rw-r--r--   0        0        0     6509 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/localnet/config_software.py
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/localnet/constants.py
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/localnet/genesis.py
--rw-r--r--   0        0        0     2510 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/localnet/genesis_json.py
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/localnet/genesis_smart_contracts_json.py
--rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/localnet/libraries.py
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/localnet/node.py
--rw-r--r--   0        0        0     2965 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/localnet/node_config_toml.py
--rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/localnet/nodes_setup_json.py
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/localnet/p2p_toml.py
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/localnet/seednode_p2pKey.pem
--rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/localnet/step_build_software.py
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/localnet/step_clean.py
--rw-r--r--   0        0        0     7724 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/localnet/step_config.py
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/localnet/step_new.py
--rw-r--r--   0        0        0     2268 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/localnet/step_prerequisites.py
--rw-r--r--   0        0        0     5745 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/localnet/step_start.py
--rw-r--r--   0        0        0     2811 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/localnet/wallets.py
--rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/projects/__init__.py
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/projects/constants.py
--rw-r--r--   0        0        0     3066 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/projects/core.py
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/projects/interfaces.py
--rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/projects/migrations.py
--rw-r--r--   0        0        0     7073 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/projects/project_base.py
--rw-r--r--   0        0        0     4616 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/projects/project_clang.py
--rw-r--r--   0        0        0     3419 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/projects/project_cpp.py
--rw-r--r--   0        0        0     9460 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/projects/project_rust.py
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/projects/project_sol.py
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/projects/shared.py
--rw-r--r--   0        0        0     8982 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/projects/templates.py
--rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/projects/templates_config.py
--rw-r--r--   0        0        0     2554 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/projects/templates_repository.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/projects/report/__init__.py
--rw-r--r--   0        0        0     2317 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/projects/report/do_report.py
--rw-r--r--   0        0        0     3903 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/projects/report/report_creator.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/projects/report/data/__init__.py
--rw-r--r--   0        0        0     2008 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/projects/report/data/common.py
--rw-r--r--   0        0        0     3986 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/projects/report/data/extracted_feature.py
--rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/projects/report/data/folder_report.py
--rw-r--r--   0        0        0     2542 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/projects/report/data/project_report.py
--rw-r--r--   0        0        0     4094 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/projects/report/data/report.py
--rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/projects/report/data/wasm_report.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/projects/report/features/__init__.py
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/projects/report/features/features.py
--rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/projects/report/features/report_option.py
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/projects/report/features/size.py
--rw-r--r--   0        0        0     2122 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/projects/report/features/twiggy_paths_check.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/projects/report/format/__init__.py
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/projects/report/format/change_type.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/projects/report/format/format_options.py
--rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/validators/__init__.py
--rw-r--r--   0        0        0     7082 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/validators/core.py
--rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/validators/validators_file.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/.gitignore
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/LICENSE
--rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/README.md
--rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/pyproject.toml
--rw-r--r--   0        0        0     2157 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.0.0b1/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/__init__.py
+-rw-r--r--   0        0        0     6432 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/accounts.py
+-rw-r--r--   0        0        0     4010 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/cli.py
+-rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/cli_accounts.py
+-rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/cli_block.py
+-rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/cli_config.py
+-rw-r--r--   0        0        0    19784 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/cli_contracts.py
+-rw-r--r--   0        0        0     3656 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/cli_data.py
+-rw-r--r--   0        0        0    12580 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/cli_delegation.py
+-rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/cli_deps.py
+-rw-r--r--   0        0        0     5193 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/cli_dns.py
+-rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/cli_ledger.py
+-rw-r--r--   0        0        0     5875 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/cli_localnet.py
+-rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/cli_network.py
+-rw-r--r--   0        0        0     4126 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/cli_output.py
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/cli_password.py
+-rw-r--r--   0        0        0    11873 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/cli_shared.py
+-rw-r--r--   0        0        0     5242 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/cli_transactions.py
+-rw-r--r--   0        0        0     8304 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/cli_validators.py
+-rw-r--r--   0        0        0     9978 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/cli_wallet.py
+-rw-r--r--   0        0        0     9707 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/config.py
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/constants.py
+-rw-r--r--   0        0        0     5147 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/contract_verification.py
+-rw-r--r--   0        0        0    10194 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/contracts.py
+-rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/cosign_transaction.py
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/diskcache.py
+-rw-r--r--   0        0        0     3394 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/dns.py
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/docker.py
+-rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/downloader.py
+-rw-r--r--   0        0        0     4881 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/errors.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/guards.py
+-rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/interfaces.py
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/myprocess.py
+-rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/simulation.py
+-rw-r--r--   0        0        0    11148 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/transactions.py
+-rw-r--r--   0        0        0     7223 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/utils.py
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/ux.py
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/version.py
+-rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/workstation.py
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/.vscode/settings.json
+-rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/delegation/__init__.py
+-rw-r--r--   0        0        0     6511 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/delegation/staking_provider.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/dependencies/__init__.py
+-rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/dependencies/install.py
+-rw-r--r--   0        0        0    16658 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/dependencies/modules.py
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/dependencies/resolution.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/ledger/__init__.py
+-rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/ledger/config.py
+-rw-r--r--   0        0        0     5275 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/ledger/ledger_app_handler.py
+-rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/ledger/ledger_functions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/localnet/__init__.py
+-rw-r--r--   0        0        0     2375 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/localnet/config_default.py
+-rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/localnet/config_general.py
+-rw-r--r--   0        0        0     2060 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/localnet/config_networking.py
+-rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/localnet/config_part.py
+-rw-r--r--   0        0        0     6263 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/localnet/config_root.py
+-rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/localnet/config_sharding.py
+-rw-r--r--   0        0        0     6509 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/localnet/config_software.py
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/localnet/constants.py
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/localnet/genesis.py
+-rw-r--r--   0        0        0     2510 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/localnet/genesis_json.py
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/localnet/genesis_smart_contracts_json.py
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/localnet/libraries.py
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/localnet/node.py
+-rw-r--r--   0        0        0     2965 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/localnet/node_config_toml.py
+-rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/localnet/nodes_setup_json.py
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/localnet/p2p_toml.py
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/localnet/seednode_p2pKey.pem
+-rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/localnet/step_build_software.py
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/localnet/step_clean.py
+-rw-r--r--   0        0        0     7724 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/localnet/step_config.py
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/localnet/step_new.py
+-rw-r--r--   0        0        0     2268 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/localnet/step_prerequisites.py
+-rw-r--r--   0        0        0     5745 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/localnet/step_start.py
+-rw-r--r--   0        0        0     2811 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/localnet/wallets.py
+-rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/projects/__init__.py
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/projects/constants.py
+-rw-r--r--   0        0        0     3066 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/projects/core.py
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/projects/interfaces.py
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/projects/migrations.py
+-rw-r--r--   0        0        0     7073 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/projects/project_base.py
+-rw-r--r--   0        0        0     4616 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/projects/project_clang.py
+-rw-r--r--   0        0        0     3419 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/projects/project_cpp.py
+-rw-r--r--   0        0        0     9460 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/projects/project_rust.py
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/projects/project_sol.py
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/projects/shared.py
+-rw-r--r--   0        0        0     8982 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/projects/templates.py
+-rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/projects/templates_config.py
+-rw-r--r--   0        0        0     2554 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/projects/templates_repository.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/projects/report/__init__.py
+-rw-r--r--   0        0        0     2317 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/projects/report/do_report.py
+-rw-r--r--   0        0        0     3903 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/projects/report/report_creator.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/projects/report/data/__init__.py
+-rw-r--r--   0        0        0     2008 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/projects/report/data/common.py
+-rw-r--r--   0        0        0     3986 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/projects/report/data/extracted_feature.py
+-rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/projects/report/data/folder_report.py
+-rw-r--r--   0        0        0     2542 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/projects/report/data/project_report.py
+-rw-r--r--   0        0        0     4094 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/projects/report/data/report.py
+-rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/projects/report/data/wasm_report.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/projects/report/features/__init__.py
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/projects/report/features/features.py
+-rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/projects/report/features/report_option.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/projects/report/features/size.py
+-rw-r--r--   0        0        0     2122 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/projects/report/features/twiggy_paths_check.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/projects/report/format/__init__.py
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/projects/report/format/change_type.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/projects/report/format/format_options.py
+-rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/validators/__init__.py
+-rw-r--r--   0        0        0     7082 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/validators/core.py
+-rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/validators/validators_file.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/.gitignore
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/LICENSE
+-rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/README.md
+-rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 multiversx_sdk_cli-7.1.0/PKG-INFO
```

### Comparing `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/accounts.py` & `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/accounts.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/cli.py` & `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/cli.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/cli_accounts.py` & `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/cli_accounts.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/cli_block.py` & `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/cli_block.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/cli_config.py` & `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/cli_config.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/cli_contracts.py` & `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/cli_contracts.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/cli_data.py` & `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/cli_data.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/cli_delegation.py` & `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/cli_delegation.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/cli_deps.py` & `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/cli_deps.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/cli_dns.py` & `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/cli_dns.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/cli_ledger.py` & `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/cli_ledger.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/cli_localnet.py` & `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/cli_localnet.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/cli_network.py` & `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/cli_network.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/cli_output.py` & `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/cli_output.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/cli_shared.py` & `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/cli_shared.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/cli_transactions.py` & `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/cli_transactions.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/cli_validators.py` & `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/cli_validators.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/cli_wallet.py` & `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/cli_wallet.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/config.py` & `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/config.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/contract_verification.py` & `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/contract_verification.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/contracts.py` & `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/contracts.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/cosign_transaction.py` & `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/cosign_transaction.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/diskcache.py` & `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/diskcache.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/dns.py` & `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/dns.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/docker.py` & `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/docker.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/downloader.py` & `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/downloader.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/errors.py` & `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/errors.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/guards.py` & `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/guards.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/interfaces.py` & `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/interfaces.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/myprocess.py` & `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/myprocess.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/simulation.py` & `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/simulation.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/transactions.py` & `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/transactions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,42 @@
 import base64
 import json
 import logging
 import time
 from collections import OrderedDict
-from typing import Any, Dict, List, Protocol, Sequence, TextIO, Tuple
+from typing import Any, Dict, List, Optional, Protocol, Sequence, TextIO, Tuple
 
 from multiversx_sdk_cli import config, errors, utils
 from multiversx_sdk_cli.accounts import Account, Address, LedgerAccount
-from multiversx_sdk_cli.cli_password import load_password, load_guardian_password
+from multiversx_sdk_cli.cli_password import (load_guardian_password,
+                                             load_password)
+from multiversx_sdk_cli.cosign_transaction import cosign_transaction
 from multiversx_sdk_cli.errors import NoWalletProvided
 from multiversx_sdk_cli.interfaces import ITransaction
-from multiversx_sdk_cli.cosign_transaction import cosign_transaction
 from multiversx_sdk_cli.ledger.ledger_functions import do_get_ledger_address
 
 logger = logging.getLogger("transactions")
 
 
 class ITransactionOnNetwork(Protocol):
     hash: str
-    is_completed: bool
+    is_completed: Optional[bool]
 
     def to_dictionary(self) -> Dict[str, Any]:
         ...
 
 
 class INetworkProvider(Protocol):
     def send_transaction(self, transaction: ITransaction) -> str:
         ...
 
     def send_transactions(self, transactions: Sequence[ITransaction]) -> Tuple[int, str]:
         ...
 
-    def get_transaction(self, tx_hash: str) -> ITransactionOnNetwork:
+    def get_transaction(self, tx_hash: str, with_process_status: Optional[bool]) -> ITransactionOnNetwork:
         ...
 
 
 class Transaction(ITransaction):
     def __init__(self):
         self.hash: str = ""
         self.nonce = 0
@@ -143,15 +144,15 @@
 
         tx_hash = proxy.send_transaction(payload)
         num_periods_to_wait = int(num_seconds_timeout / AWAIT_TRANSACTION_PERIOD)
 
         for _ in range(0, num_periods_to_wait):
             time.sleep(AWAIT_TRANSACTION_PERIOD)
 
-            tx = proxy.get_transaction(tx_hash)
+            tx = proxy.get_transaction(tx_hash, with_process_status=True)
             if tx.is_completed:
                 return tx
             else:
                 logger.info("Transaction not yet done.")
 
         raise errors.KnownError("Took too long to get transaction.")
```

### Comparing `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/utils.py` & `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/utils.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/version.py` & `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/version.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/workstation.py` & `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/workstation.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/delegation/__init__.py` & `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/delegation/__init__.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/delegation/staking_provider.py` & `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/delegation/staking_provider.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/dependencies/install.py` & `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/dependencies/install.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/dependencies/modules.py` & `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/dependencies/modules.py`

 * *Files 4% similar despite different names*

```diff
@@ -266,15 +266,19 @@
         if tag:
             toolchain = tag
         else:
             toolchain = "nightly"
 
         args = [str(installer_path), "--verbose", "--default-toolchain", toolchain, "--profile",
                 "minimal", "--target", "wasm32-unknown-unknown", "--no-modify-path", "-y"]
-        myprocess.run_process(args, env=self.get_env_for_install())
+        output = myprocess.run_process(args, env=self.get_env_for_install())
+
+        if output:
+            sc_meta_args = ["cargo", "install", "multiversx-sc-meta"]
+            myprocess.run_process(sc_meta_args, env=self.get_env_for_install())
 
     def _get_installer_url(self) -> str:
         if workstation.is_windows():
             return "https://win.rustup.rs"
         return "https://sh.rustup.rs"
 
     def _get_installer_path(self) -> Path:
```

### Comparing `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/ledger/config.py` & `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/ledger/config.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/ledger/ledger_app_handler.py` & `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/ledger/ledger_app_handler.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/ledger/ledger_functions.py` & `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/ledger/ledger_functions.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/localnet/config_default.py` & `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/localnet/config_default.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/localnet/config_general.py` & `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/localnet/config_general.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/localnet/config_networking.py` & `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/localnet/config_networking.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/localnet/config_part.py` & `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/localnet/config_part.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/localnet/config_root.py` & `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/localnet/config_root.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/localnet/config_sharding.py` & `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/localnet/config_sharding.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/localnet/config_software.py` & `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/localnet/config_software.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/localnet/genesis.py` & `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/localnet/genesis.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/localnet/genesis_json.py` & `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/localnet/genesis_json.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/localnet/libraries.py` & `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/localnet/libraries.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/localnet/node.py` & `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/localnet/node.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/localnet/node_config_toml.py` & `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/localnet/node_config_toml.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/localnet/nodes_setup_json.py` & `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/localnet/nodes_setup_json.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/localnet/p2p_toml.py` & `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/localnet/p2p_toml.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/localnet/step_build_software.py` & `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/localnet/step_build_software.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/localnet/step_config.py` & `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/localnet/step_config.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/localnet/step_prerequisites.py` & `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/localnet/step_prerequisites.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/localnet/step_start.py` & `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/localnet/step_start.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/localnet/wallets.py` & `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/localnet/wallets.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/projects/__init__.py` & `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/projects/__init__.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/projects/core.py` & `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/projects/core.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/projects/migrations.py` & `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/projects/migrations.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/projects/project_base.py` & `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/projects/project_base.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/projects/project_clang.py` & `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/projects/project_clang.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/projects/project_cpp.py` & `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/projects/project_cpp.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/projects/project_rust.py` & `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/projects/project_rust.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/projects/shared.py` & `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/projects/shared.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/projects/templates.py` & `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/projects/templates.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/projects/templates_config.py` & `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/projects/templates_config.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/projects/templates_repository.py` & `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/projects/templates_repository.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/projects/report/do_report.py` & `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/projects/report/do_report.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/projects/report/report_creator.py` & `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/projects/report/report_creator.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/projects/report/data/common.py` & `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/projects/report/data/common.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/projects/report/data/extracted_feature.py` & `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/projects/report/data/extracted_feature.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/projects/report/data/folder_report.py` & `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/projects/report/data/folder_report.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/projects/report/data/project_report.py` & `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/projects/report/data/project_report.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/projects/report/data/report.py` & `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/projects/report/data/report.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/projects/report/data/wasm_report.py` & `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/projects/report/data/wasm_report.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/projects/report/features/report_option.py` & `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/projects/report/features/report_option.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/projects/report/features/twiggy_paths_check.py` & `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/projects/report/features/twiggy_paths_check.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/projects/report/format/change_type.py` & `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/projects/report/format/change_type.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/validators/__init__.py` & `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/validators/__init__.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/validators/core.py` & `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/validators/core.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b1/multiversx_sdk_cli/validators/validators_file.py` & `multiversx_sdk_cli-7.1.0/multiversx_sdk_cli/validators/validators_file.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b1/LICENSE` & `multiversx_sdk_cli-7.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b1/README.md` & `multiversx_sdk_cli-7.1.0/README.md`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_cli-7.0.0b1/pyproject.toml` & `multiversx_sdk_cli-7.1.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "multiversx-sdk-cli"
-version = "7.0.0b1"
+version = "7.1.0"
 authors = [
   { name="MultiversX" },
 ]
 license = "MIT"
 description = "MultiversX Smart Contracts Tools"
 readme = "README.md"
 requires-python = ">=3.8"
@@ -22,17 +22,17 @@
   "toml>=0.10.2",
   "requests",
   "prettytable",
   "ledgercomm[hid]",
   "semver",
   "requests-cache",
   "rich==13.3.4",
-  "multiversx-sdk-network-providers==0.6.*",
-  "multiversx-sdk-wallet==0.7.*",
-  "multiversx-sdk-core>=0.4.1"
+  "multiversx-sdk-network-providers>=0.11.0",
+  "multiversx-sdk-wallet>=0.7.0",
+  "multiversx-sdk-core>=0.5.0"
 ]
 
 [tool.hatch.build]
 include = [
   "multiversx_sdk_cli/**"
 ]
 exclude = [
```

### Comparing `multiversx_sdk_cli-7.0.0b1/PKG-INFO` & `multiversx_sdk_cli-7.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: multiversx-sdk-cli
-Version: 7.0.0b1
+Version: 7.1.0
 Summary: MultiversX Smart Contracts Tools
 Project-URL: Homepage, https://github.com/multiversx/mx-sdk-py-cli
 Author: MultiversX
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Requires-Dist: ledgercomm[hid]
-Requires-Dist: multiversx-sdk-core>=0.4.1
-Requires-Dist: multiversx-sdk-network-providers==0.6.*
-Requires-Dist: multiversx-sdk-wallet==0.7.*
+Requires-Dist: multiversx-sdk-core>=0.5.0
+Requires-Dist: multiversx-sdk-network-providers>=0.11.0
+Requires-Dist: multiversx-sdk-wallet>=0.7.0
 Requires-Dist: prettytable
 Requires-Dist: requests
 Requires-Dist: requests-cache
 Requires-Dist: rich==13.3.4
 Requires-Dist: semver
 Requires-Dist: toml>=0.10.2
 Description-Content-Type: text/markdown
```

