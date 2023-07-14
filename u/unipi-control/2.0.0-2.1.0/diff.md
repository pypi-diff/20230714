# Comparing `tmp/unipi-control-2.0.0.tar.gz` & `tmp/unipi-control-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unipi-control-2.0.0.tar", last modified: Fri Jun 23 16:29:54 2023, max compression
+gzip compressed data, was "unipi-control-2.1.0.tar", last modified: Fri Jul 14 07:41:06 2023, max compression
```

## Comparing `unipi-control-2.0.0.tar` & `unipi-control-2.1.0.tar`

### file list

```diff
@@ -1,162 +1,163 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:29:54.758712 unipi-control-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-23 16:29:38.000000 unipi-control-2.0.0/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:29:54.726712 unipi-control-2.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:29:54.734712 unipi-control-2.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-06-23 16:29:38.000000 unipi-control-2.0.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-23 16:29:38.000000 unipi-control-2.0.0/.github/workflows/parameters.json
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-23 16:29:38.000000 unipi-control-2.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-06-23 16:29:38.000000 unipi-control-2.0.0/.yamllint.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-06-23 16:29:38.000000 unipi-control-2.0.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-23 16:29:38.000000 unipi-control-2.0.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-23 16:29:38.000000 unipi-control-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-06-23 16:29:54.758712 unipi-control-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-06-23 16:29:38.000000 unipi-control-2.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-06-23 16:29:38.000000 unipi-control-2.0.0/coverage.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:29:54.734712 unipi-control-2.0.0/data/
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-23 16:29:38.000000 unipi-control-2.0.0/data/Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:29:54.726712 unipi-control-2.0.0/data/extras/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:29:54.726712 unipi-control-2.0.0/data/extras/homeassistant/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:29:54.726712 unipi-control-2.0.0/data/extras/homeassistant/blueprints/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:29:54.726712 unipi-control-2.0.0/data/extras/homeassistant/blueprints/automation/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:29:54.734712 unipi-control-2.0.0/data/extras/homeassistant/blueprints/automation/cover/
--rw-r--r--   0 runner    (1001) docker     (123)     6745 2023-06-23 16:29:38.000000 unipi-control-2.0.0/data/extras/homeassistant/blueprints/automation/cover/control.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1686 2023-06-23 16:29:38.000000 unipi-control-2.0.0/data/extras/homeassistant/blueprints/automation/cover/simple_cover_control.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:29:54.726712 unipi-control-2.0.0/data/opkg/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:29:54.734712 unipi-control-2.0.0/data/opkg/control/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-23 16:29:38.000000 unipi-control-2.0.0/data/opkg/control/control
--rwxr-xr-x   0 runner    (1001) docker     (123)      121 2023-06-23 16:29:38.000000 unipi-control-2.0.0/data/opkg/control/postinst
--rwxr-xr-x   0 runner    (1001) docker     (123)      121 2023-06-23 16:29:38.000000 unipi-control-2.0.0/data/opkg/control/prerm
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:29:54.726712 unipi-control-2.0.0/data/opkg/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:29:54.726712 unipi-control-2.0.0/data/opkg/data/usr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:29:54.730712 unipi-control-2.0.0/data/opkg/data/usr/local/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:29:54.730712 unipi-control-2.0.0/data/opkg/data/usr/local/etc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:29:54.734712 unipi-control-2.0.0/data/opkg/data/usr/local/etc/unipi/
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-06-23 16:29:38.000000 unipi-control-2.0.0/data/opkg/data/usr/local/etc/unipi/control.yaml.example
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:29:54.730712 unipi-control-2.0.0/data/opkg/data/usr/local/etc/unipi/hardware/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:29:54.738712 unipi-control-2.0.0/data/opkg/data/usr/local/etc/unipi/hardware/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)     4691 2023-06-23 16:29:38.000000 unipi-control-2.0.0/data/opkg/data/usr/local/etc/unipi/hardware/extensions/Eastron_SDM120M.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-23 16:29:38.000000 unipi-control-2.0.0/data/opkg/data/usr/local/etc/unipi/hardware/extensions/xS11.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:29:54.742712 unipi-control-2.0.0/data/opkg/data/usr/local/etc/unipi/hardware/neuron/
--rwxr-xr-x   0 runner    (1001) docker     (123)      796 2023-06-23 16:29:38.000000 unipi-control-2.0.0/data/opkg/data/usr/local/etc/unipi/hardware/neuron/L203.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-06-23 16:29:38.000000 unipi-control-2.0.0/data/opkg/data/usr/local/etc/unipi/hardware/neuron/L207.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-06-23 16:29:38.000000 unipi-control-2.0.0/data/opkg/data/usr/local/etc/unipi/hardware/neuron/L523.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-06-23 16:29:38.000000 unipi-control-2.0.0/data/opkg/data/usr/local/etc/unipi/hardware/neuron/L527.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-06-23 16:29:38.000000 unipi-control-2.0.0/data/opkg/data/usr/local/etc/unipi/hardware/neuron/L533.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-06-23 16:29:38.000000 unipi-control-2.0.0/data/opkg/data/usr/local/etc/unipi/hardware/neuron/M103.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-06-23 16:29:38.000000 unipi-control-2.0.0/data/opkg/data/usr/local/etc/unipi/hardware/neuron/M203.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-06-23 16:29:38.000000 unipi-control-2.0.0/data/opkg/data/usr/local/etc/unipi/hardware/neuron/M207.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-06-23 16:29:38.000000 unipi-control-2.0.0/data/opkg/data/usr/local/etc/unipi/hardware/neuron/M267.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-06-23 16:29:38.000000 unipi-control-2.0.0/data/opkg/data/usr/local/etc/unipi/hardware/neuron/M523.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-06-23 16:29:38.000000 unipi-control-2.0.0/data/opkg/data/usr/local/etc/unipi/hardware/neuron/M527.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-06-23 16:29:38.000000 unipi-control-2.0.0/data/opkg/data/usr/local/etc/unipi/hardware/neuron/M567.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-06-23 16:29:38.000000 unipi-control-2.0.0/data/opkg/data/usr/local/etc/unipi/hardware/neuron/S103-G.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-06-23 16:29:38.000000 unipi-control-2.0.0/data/opkg/data/usr/local/etc/unipi/hardware/neuron/S103.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-06-23 16:29:38.000000 unipi-control-2.0.0/data/opkg/data/usr/local/etc/unipi/hardware/neuron/S107.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-06-23 16:29:38.000000 unipi-control-2.0.0/data/opkg/data/usr/local/etc/unipi/hardware/neuron/S117.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-06-23 16:29:38.000000 unipi-control-2.0.0/data/opkg/data/usr/local/etc/unipi/hardware/neuron/S167.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-23 16:29:38.000000 unipi-control-2.0.0/data/opkg/data/usr/local/etc/unipi/hardware/neuron/S207.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:29:54.730712 unipi-control-2.0.0/data/opkg/data/usr/local/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:29:54.730712 unipi-control-2.0.0/data/opkg/data/usr/local/lib/systemd/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:29:54.742712 unipi-control-2.0.0/data/opkg/data/usr/local/lib/systemd/system/
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-06-23 16:29:38.000000 unipi-control-2.0.0/data/opkg/data/usr/local/lib/systemd/system/unipi-control.service
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:29:54.742712 unipi-control-2.0.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-06-23 16:29:38.000000 unipi-control-2.0.0/docs/commands.md
--rw-r--r--   0 runner    (1001) docker     (123)     9612 2023-06-23 16:29:38.000000 unipi-control-2.0.0/docs/configuration.md
--rw-r--r--   0 runner    (1001) docker     (123)     4676 2023-06-23 16:29:38.000000 unipi-control-2.0.0/docs/mqtt-topics.md
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-06-23 16:29:38.000000 unipi-control-2.0.0/docs/supported-hardware.md
--rw-r--r--   0 runner    (1001) docker     (123)     5438 2023-06-23 16:29:38.000000 unipi-control-2.0.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:29:54.742712 unipi-control-2.0.0/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)      600 2023-06-23 16:29:38.000000 unipi-control-2.0.0/scripts/entry.sh
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 16:29:54.758712 unipi-control-2.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:29:54.742712 unipi-control-2.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 16:29:38.000000 unipi-control-2.0.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8578 2023-06-23 16:29:38.000000 unipi-control-2.0.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     9682 2023-06-23 16:29:38.000000 unipi-control-2.0.0/tests/conftest_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:29:54.742712 unipi-control-2.0.0/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 16:29:38.000000 unipi-control-2.0.0/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5476 2023-06-23 16:29:38.000000 unipi-control-2.0.0/tests/integration/test_unipi_control.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:29:54.742712 unipi-control-2.0.0/tests/integration/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 16:29:38.000000 unipi-control-2.0.0/tests/integration/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4007 2023-06-23 16:29:38.000000 unipi-control-2.0.0/tests/integration/tools/test_config_backup.py
--rw-r--r--   0 runner    (1001) docker     (123)     5321 2023-06-23 16:29:38.000000 unipi-control-2.0.0/tests/integration/tools/test_config_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4615 2023-06-23 16:29:38.000000 unipi-control-2.0.0/tests/integration/tools/test_config_converter_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-23 16:29:38.000000 unipi-control-2.0.0/tests/integration/tools/test_model_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:29:54.746712 unipi-control-2.0.0/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 16:29:38.000000 unipi-control-2.0.0/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:29:54.746712 unipi-control-2.0.0/tests/unit/integrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 16:29:38.000000 unipi-control-2.0.0/tests/unit/integrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27427 2023-06-23 16:29:38.000000 unipi-control-2.0.0/tests/unit/integrations/test_covers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:29:54.746712 unipi-control-2.0.0/tests/unit/mqtt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 16:29:38.000000 unipi-control-2.0.0/tests/unit/mqtt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:29:54.746712 unipi-control-2.0.0/tests/unit/mqtt/discovery/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 16:29:38.000000 unipi-control-2.0.0/tests/unit/mqtt/discovery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26484 2023-06-23 16:29:38.000000 unipi-control-2.0.0/tests/unit/mqtt/discovery/test_binary_sensors.py
--rw-r--r--   0 runner    (1001) docker     (123)    21612 2023-06-23 16:29:38.000000 unipi-control-2.0.0/tests/unit/mqtt/discovery/test_binary_sensors_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     7493 2023-06-23 16:29:38.000000 unipi-control-2.0.0/tests/unit/mqtt/discovery/test_covers.py
--rw-r--r--   0 runner    (1001) docker     (123)    24229 2023-06-23 16:29:38.000000 unipi-control-2.0.0/tests/unit/mqtt/discovery/test_sensors.py
--rw-r--r--   0 runner    (1001) docker     (123)    19936 2023-06-23 16:29:38.000000 unipi-control-2.0.0/tests/unit/mqtt/discovery/test_sensors_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    22820 2023-06-23 16:29:38.000000 unipi-control-2.0.0/tests/unit/mqtt/discovery/test_switches.py
--rw-r--r--   0 runner    (1001) docker     (123)    20762 2023-06-23 16:29:38.000000 unipi-control-2.0.0/tests/unit/mqtt/discovery/test_switches_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:29:54.746712 unipi-control-2.0.0/tests/unit/mqtt/integrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 16:29:38.000000 unipi-control-2.0.0/tests/unit/mqtt/integrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14324 2023-06-23 16:29:38.000000 unipi-control-2.0.0/tests/unit/mqtt/integrations/test_covers.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-23 16:29:38.000000 unipi-control-2.0.0/tests/unit/mqtt/integrations/test_covers_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     6576 2023-06-23 16:29:38.000000 unipi-control-2.0.0/tests/unit/mqtt/test_features.py
--rw-r--r--   0 runner    (1001) docker     (123)    18507 2023-06-23 16:29:38.000000 unipi-control-2.0.0/tests/unit/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6906 2023-06-23 16:29:38.000000 unipi-control-2.0.0/tests/unit/test_config_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5995 2023-06-23 16:29:38.000000 unipi-control-2.0.0/tests/unit/test_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-06-23 16:29:38.000000 unipi-control-2.0.0/tests/unit/test_modbus.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-06-23 16:29:38.000000 unipi-control-2.0.0/tests/unit/test_neuron.py
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-23 16:29:38.000000 unipi-control-2.0.0/tests/unit/test_unipi_control.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:29:54.750712 unipi-control-2.0.0/unipi_control/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-23 16:29:38.000000 unipi-control-2.0.0/unipi_control/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23952 2023-06-23 16:29:38.000000 unipi-control-2.0.0/unipi_control/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:29:54.750712 unipi-control-2.0.0/unipi_control/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 16:29:38.000000 unipi-control-2.0.0/unipi_control/extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-06-23 16:29:38.000000 unipi-control-2.0.0/unipi_control/extensions/eastron.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:29:54.750712 unipi-control-2.0.0/unipi_control/features/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 16:29:38.000000 unipi-control-2.0.0/unipi_control/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6029 2023-06-23 16:29:38.000000 unipi-control-2.0.0/unipi_control/features/extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3727 2023-06-23 16:29:38.000000 unipi-control-2.0.0/unipi_control/features/map.py
--rw-r--r--   0 runner    (1001) docker     (123)     7084 2023-06-23 16:29:38.000000 unipi-control-2.0.0/unipi_control/features/neuron.py
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-06-23 16:29:38.000000 unipi-control-2.0.0/unipi_control/features/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:29:54.754712 unipi-control-2.0.0/unipi_control/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 16:29:38.000000 unipi-control-2.0.0/unipi_control/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-06-23 16:29:38.000000 unipi-control-2.0.0/unipi_control/helpers/argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-23 16:29:38.000000 unipi-control-2.0.0/unipi_control/helpers/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-06-23 16:29:38.000000 unipi-control-2.0.0/unipi_control/helpers/log.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-06-23 16:29:38.000000 unipi-control-2.0.0/unipi_control/helpers/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-06-23 16:29:38.000000 unipi-control-2.0.0/unipi_control/helpers/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-06-23 16:29:38.000000 unipi-control-2.0.0/unipi_control/helpers/yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:29:54.754712 unipi-control-2.0.0/unipi_control/integrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 16:29:38.000000 unipi-control-2.0.0/unipi_control/integrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25661 2023-06-23 16:29:38.000000 unipi-control-2.0.0/unipi_control/integrations/covers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-06-23 16:29:38.000000 unipi-control-2.0.0/unipi_control/modbus.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:29:54.754712 unipi-control-2.0.0/unipi_control/mqtt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 16:29:38.000000 unipi-control-2.0.0/unipi_control/mqtt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:29:54.754712 unipi-control-2.0.0/unipi_control/mqtt/discovery/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 16:29:38.000000 unipi-control-2.0.0/unipi_control/mqtt/discovery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-06-23 16:29:38.000000 unipi-control-2.0.0/unipi_control/mqtt/discovery/binary_sensors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-06-23 16:29:38.000000 unipi-control-2.0.0/unipi_control/mqtt/discovery/covers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-06-23 16:29:38.000000 unipi-control-2.0.0/unipi_control/mqtt/discovery/mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-06-23 16:29:38.000000 unipi-control-2.0.0/unipi_control/mqtt/discovery/sensors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3792 2023-06-23 16:29:38.000000 unipi-control-2.0.0/unipi_control/mqtt/discovery/switches.py
--rw-r--r--   0 runner    (1001) docker     (123)     4452 2023-06-23 16:29:38.000000 unipi-control-2.0.0/unipi_control/mqtt/features.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:29:54.754712 unipi-control-2.0.0/unipi_control/mqtt/integrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 16:29:38.000000 unipi-control-2.0.0/unipi_control/mqtt/integrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8484 2023-06-23 16:29:38.000000 unipi-control-2.0.0/unipi_control/mqtt/integrations/covers.py
--rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-06-23 16:29:38.000000 unipi-control-2.0.0/unipi_control/neuron.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:29:54.758712 unipi-control-2.0.0/unipi_control/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 16:29:38.000000 unipi-control-2.0.0/unipi_control/tools/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3200 2023-06-23 16:29:38.000000 unipi-control-2.0.0/unipi_control/tools/config_backup.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5207 2023-06-23 16:29:38.000000 unipi-control-2.0.0/unipi_control/tools/config_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-06-23 16:29:38.000000 unipi-control-2.0.0/unipi_control/tools/model_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     9553 2023-06-23 16:29:38.000000 unipi-control-2.0.0/unipi_control/unipi_control.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-23 16:29:54.000000 unipi-control-2.0.0/unipi_control/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:29:54.750712 unipi-control-2.0.0/unipi_control.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-06-23 16:29:54.000000 unipi-control-2.0.0/unipi_control.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4515 2023-06-23 16:29:54.000000 unipi-control-2.0.0/unipi_control.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 16:29:54.000000 unipi-control-2.0.0/unipi_control.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-23 16:29:54.000000 unipi-control-2.0.0/unipi_control.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-23 16:29:54.000000 unipi-control-2.0.0/unipi_control.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-23 16:29:54.000000 unipi-control-2.0.0/unipi_control.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:41:06.871073 unipi-control-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-14 07:40:40.000000 unipi-control-2.1.0/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:41:06.855072 unipi-control-2.1.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-14 07:40:40.000000 unipi-control-2.1.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:41:06.855072 unipi-control-2.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     4461 2023-07-14 07:40:40.000000 unipi-control-2.1.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-14 07:40:40.000000 unipi-control-2.1.0/.github/workflows/parameters.json
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-07-14 07:40:40.000000 unipi-control-2.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-07-14 07:40:40.000000 unipi-control-2.1.0/.yamllint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-07-14 07:40:40.000000 unipi-control-2.1.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-14 07:40:40.000000 unipi-control-2.1.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-14 07:40:40.000000 unipi-control-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4916 2023-07-14 07:41:06.867072 unipi-control-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-07-14 07:40:40.000000 unipi-control-2.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-07-14 07:40:40.000000 unipi-control-2.1.0/coverage.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:41:06.855072 unipi-control-2.1.0/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-14 07:40:40.000000 unipi-control-2.1.0/data/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:41:06.851072 unipi-control-2.1.0/data/extras/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:41:06.851072 unipi-control-2.1.0/data/extras/homeassistant/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:41:06.851072 unipi-control-2.1.0/data/extras/homeassistant/blueprints/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:41:06.851072 unipi-control-2.1.0/data/extras/homeassistant/blueprints/automation/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:41:06.855072 unipi-control-2.1.0/data/extras/homeassistant/blueprints/automation/cover/
+-rw-r--r--   0 runner    (1001) docker     (123)     6745 2023-07-14 07:40:40.000000 unipi-control-2.1.0/data/extras/homeassistant/blueprints/automation/cover/control.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1686 2023-07-14 07:40:40.000000 unipi-control-2.1.0/data/extras/homeassistant/blueprints/automation/cover/simple_cover_control.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:41:06.855072 unipi-control-2.1.0/data/opkg/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:41:06.859072 unipi-control-2.1.0/data/opkg/control/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-14 07:40:40.000000 unipi-control-2.1.0/data/opkg/control/control
+-rwxr-xr-x   0 runner    (1001) docker     (123)      121 2023-07-14 07:40:40.000000 unipi-control-2.1.0/data/opkg/control/postinst
+-rwxr-xr-x   0 runner    (1001) docker     (123)      121 2023-07-14 07:40:40.000000 unipi-control-2.1.0/data/opkg/control/prerm
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:41:06.855072 unipi-control-2.1.0/data/opkg/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:41:06.855072 unipi-control-2.1.0/data/opkg/data/usr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:41:06.855072 unipi-control-2.1.0/data/opkg/data/usr/local/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:41:06.855072 unipi-control-2.1.0/data/opkg/data/usr/local/etc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:41:06.859072 unipi-control-2.1.0/data/opkg/data/usr/local/etc/unipi/
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-07-14 07:40:40.000000 unipi-control-2.1.0/data/opkg/data/usr/local/etc/unipi/control.yaml.example
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:41:06.855072 unipi-control-2.1.0/data/opkg/data/usr/local/etc/unipi/hardware/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:41:06.859072 unipi-control-2.1.0/data/opkg/data/usr/local/etc/unipi/hardware/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)     4691 2023-07-14 07:40:40.000000 unipi-control-2.1.0/data/opkg/data/usr/local/etc/unipi/hardware/extensions/Eastron_SDM120M.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-14 07:40:40.000000 unipi-control-2.1.0/data/opkg/data/usr/local/etc/unipi/hardware/extensions/xS11.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:41:06.859072 unipi-control-2.1.0/data/opkg/data/usr/local/etc/unipi/hardware/neuron/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      796 2023-07-14 07:40:40.000000 unipi-control-2.1.0/data/opkg/data/usr/local/etc/unipi/hardware/neuron/L203.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-07-14 07:40:40.000000 unipi-control-2.1.0/data/opkg/data/usr/local/etc/unipi/hardware/neuron/L207.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-07-14 07:40:40.000000 unipi-control-2.1.0/data/opkg/data/usr/local/etc/unipi/hardware/neuron/L523.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-07-14 07:40:40.000000 unipi-control-2.1.0/data/opkg/data/usr/local/etc/unipi/hardware/neuron/L527.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-07-14 07:40:40.000000 unipi-control-2.1.0/data/opkg/data/usr/local/etc/unipi/hardware/neuron/L533.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-07-14 07:40:40.000000 unipi-control-2.1.0/data/opkg/data/usr/local/etc/unipi/hardware/neuron/M103.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-07-14 07:40:40.000000 unipi-control-2.1.0/data/opkg/data/usr/local/etc/unipi/hardware/neuron/M203.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-07-14 07:40:40.000000 unipi-control-2.1.0/data/opkg/data/usr/local/etc/unipi/hardware/neuron/M207.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-07-14 07:40:40.000000 unipi-control-2.1.0/data/opkg/data/usr/local/etc/unipi/hardware/neuron/M267.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-14 07:40:40.000000 unipi-control-2.1.0/data/opkg/data/usr/local/etc/unipi/hardware/neuron/M523.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-14 07:40:40.000000 unipi-control-2.1.0/data/opkg/data/usr/local/etc/unipi/hardware/neuron/M527.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-14 07:40:40.000000 unipi-control-2.1.0/data/opkg/data/usr/local/etc/unipi/hardware/neuron/M567.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-07-14 07:40:40.000000 unipi-control-2.1.0/data/opkg/data/usr/local/etc/unipi/hardware/neuron/S103-G.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-07-14 07:40:40.000000 unipi-control-2.1.0/data/opkg/data/usr/local/etc/unipi/hardware/neuron/S103.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-07-14 07:40:40.000000 unipi-control-2.1.0/data/opkg/data/usr/local/etc/unipi/hardware/neuron/S107.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-07-14 07:40:40.000000 unipi-control-2.1.0/data/opkg/data/usr/local/etc/unipi/hardware/neuron/S117.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-07-14 07:40:40.000000 unipi-control-2.1.0/data/opkg/data/usr/local/etc/unipi/hardware/neuron/S167.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-14 07:40:40.000000 unipi-control-2.1.0/data/opkg/data/usr/local/etc/unipi/hardware/neuron/S207.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:41:06.855072 unipi-control-2.1.0/data/opkg/data/usr/local/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:41:06.855072 unipi-control-2.1.0/data/opkg/data/usr/local/lib/systemd/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:41:06.859072 unipi-control-2.1.0/data/opkg/data/usr/local/lib/systemd/system/
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-14 07:40:40.000000 unipi-control-2.1.0/data/opkg/data/usr/local/lib/systemd/system/unipi-control.service
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:41:06.859072 unipi-control-2.1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-07-14 07:40:40.000000 unipi-control-2.1.0/docs/commands.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10560 2023-07-14 07:40:40.000000 unipi-control-2.1.0/docs/configuration.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-07-14 07:40:40.000000 unipi-control-2.1.0/docs/mqtt-topics.md
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-07-14 07:40:40.000000 unipi-control-2.1.0/docs/supported-hardware.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5694 2023-07-14 07:40:40.000000 unipi-control-2.1.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:41:06.859072 unipi-control-2.1.0/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      600 2023-07-14 07:40:40.000000 unipi-control-2.1.0/scripts/entry.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 07:41:06.871073 unipi-control-2.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:41:06.859072 unipi-control-2.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 07:40:40.000000 unipi-control-2.1.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8705 2023-07-14 07:40:40.000000 unipi-control-2.1.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10010 2023-07-14 07:40:40.000000 unipi-control-2.1.0/tests/conftest_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:41:06.859072 unipi-control-2.1.0/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 07:40:40.000000 unipi-control-2.1.0/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5485 2023-07-14 07:40:40.000000 unipi-control-2.1.0/tests/integration/test_unipi_control.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:41:06.863072 unipi-control-2.1.0/tests/integration/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 07:40:40.000000 unipi-control-2.1.0/tests/integration/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4019 2023-07-14 07:40:40.000000 unipi-control-2.1.0/tests/integration/tools/test_config_backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5469 2023-07-14 07:40:40.000000 unipi-control-2.1.0/tests/integration/tools/test_config_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4615 2023-07-14 07:40:40.000000 unipi-control-2.1.0/tests/integration/tools/test_config_converter_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-07-14 07:40:40.000000 unipi-control-2.1.0/tests/integration/tools/test_model_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:41:06.863072 unipi-control-2.1.0/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 07:40:40.000000 unipi-control-2.1.0/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:41:06.863072 unipi-control-2.1.0/tests/unit/integrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 07:40:40.000000 unipi-control-2.1.0/tests/unit/integrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27427 2023-07-14 07:40:40.000000 unipi-control-2.1.0/tests/unit/integrations/test_covers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:41:06.863072 unipi-control-2.1.0/tests/unit/mqtt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 07:40:40.000000 unipi-control-2.1.0/tests/unit/mqtt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:41:06.863072 unipi-control-2.1.0/tests/unit/mqtt/discovery/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 07:40:40.000000 unipi-control-2.1.0/tests/unit/mqtt/discovery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26479 2023-07-14 07:40:40.000000 unipi-control-2.1.0/tests/unit/mqtt/discovery/test_binary_sensors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21612 2023-07-14 07:40:40.000000 unipi-control-2.1.0/tests/unit/mqtt/discovery/test_binary_sensors_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7488 2023-07-14 07:40:40.000000 unipi-control-2.1.0/tests/unit/mqtt/discovery/test_covers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24224 2023-07-14 07:40:40.000000 unipi-control-2.1.0/tests/unit/mqtt/discovery/test_sensors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19936 2023-07-14 07:40:40.000000 unipi-control-2.1.0/tests/unit/mqtt/discovery/test_sensors_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22815 2023-07-14 07:40:40.000000 unipi-control-2.1.0/tests/unit/mqtt/discovery/test_switches.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20762 2023-07-14 07:40:40.000000 unipi-control-2.1.0/tests/unit/mqtt/discovery/test_switches_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:41:06.863072 unipi-control-2.1.0/tests/unit/mqtt/integrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 07:40:40.000000 unipi-control-2.1.0/tests/unit/mqtt/integrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14319 2023-07-14 07:40:40.000000 unipi-control-2.1.0/tests/unit/mqtt/integrations/test_covers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-14 07:40:40.000000 unipi-control-2.1.0/tests/unit/mqtt/integrations/test_covers_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6571 2023-07-14 07:40:40.000000 unipi-control-2.1.0/tests/unit/mqtt/test_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19772 2023-07-14 07:40:40.000000 unipi-control-2.1.0/tests/unit/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7041 2023-07-14 07:40:40.000000 unipi-control-2.1.0/tests/unit/test_config_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5995 2023-07-14 07:40:40.000000 unipi-control-2.1.0/tests/unit/test_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-07-14 07:40:40.000000 unipi-control-2.1.0/tests/unit/test_modbus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-07-14 07:40:40.000000 unipi-control-2.1.0/tests/unit/test_neuron.py
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-14 07:40:40.000000 unipi-control-2.1.0/tests/unit/test_unipi_control.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:41:06.863072 unipi-control-2.1.0/unipi_control/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-14 07:40:40.000000 unipi-control-2.1.0/unipi_control/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24282 2023-07-14 07:40:40.000000 unipi-control-2.1.0/unipi_control/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:41:06.867072 unipi-control-2.1.0/unipi_control/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 07:40:40.000000 unipi-control-2.1.0/unipi_control/extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-07-14 07:40:40.000000 unipi-control-2.1.0/unipi_control/extensions/eastron.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:41:06.867072 unipi-control-2.1.0/unipi_control/features/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 07:40:40.000000 unipi-control-2.1.0/unipi_control/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6029 2023-07-14 07:40:40.000000 unipi-control-2.1.0/unipi_control/features/extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3727 2023-07-14 07:40:40.000000 unipi-control-2.1.0/unipi_control/features/map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7084 2023-07-14 07:40:40.000000 unipi-control-2.1.0/unipi_control/features/neuron.py
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-07-14 07:40:40.000000 unipi-control-2.1.0/unipi_control/features/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:41:06.867072 unipi-control-2.1.0/unipi_control/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 07:40:40.000000 unipi-control-2.1.0/unipi_control/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-07-14 07:40:40.000000 unipi-control-2.1.0/unipi_control/helpers/argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-14 07:40:40.000000 unipi-control-2.1.0/unipi_control/helpers/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-07-14 07:40:40.000000 unipi-control-2.1.0/unipi_control/helpers/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-07-14 07:40:40.000000 unipi-control-2.1.0/unipi_control/helpers/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-07-14 07:40:40.000000 unipi-control-2.1.0/unipi_control/helpers/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-07-14 07:40:40.000000 unipi-control-2.1.0/unipi_control/helpers/yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:41:06.867072 unipi-control-2.1.0/unipi_control/integrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 07:40:40.000000 unipi-control-2.1.0/unipi_control/integrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25665 2023-07-14 07:40:40.000000 unipi-control-2.1.0/unipi_control/integrations/covers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4526 2023-07-14 07:40:40.000000 unipi-control-2.1.0/unipi_control/modbus.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:41:06.867072 unipi-control-2.1.0/unipi_control/mqtt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 07:40:40.000000 unipi-control-2.1.0/unipi_control/mqtt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:41:06.867072 unipi-control-2.1.0/unipi_control/mqtt/discovery/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 07:40:40.000000 unipi-control-2.1.0/unipi_control/mqtt/discovery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-07-14 07:40:40.000000 unipi-control-2.1.0/unipi_control/mqtt/discovery/binary_sensors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-07-14 07:40:40.000000 unipi-control-2.1.0/unipi_control/mqtt/discovery/covers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-07-14 07:40:40.000000 unipi-control-2.1.0/unipi_control/mqtt/discovery/mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-07-14 07:40:40.000000 unipi-control-2.1.0/unipi_control/mqtt/discovery/sensors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-07-14 07:40:40.000000 unipi-control-2.1.0/unipi_control/mqtt/discovery/switches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4447 2023-07-14 07:40:40.000000 unipi-control-2.1.0/unipi_control/mqtt/features.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:41:06.867072 unipi-control-2.1.0/unipi_control/mqtt/integrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 07:40:40.000000 unipi-control-2.1.0/unipi_control/mqtt/integrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8479 2023-07-14 07:40:40.000000 unipi-control-2.1.0/unipi_control/mqtt/integrations/covers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-07-14 07:40:40.000000 unipi-control-2.1.0/unipi_control/neuron.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:41:06.867072 unipi-control-2.1.0/unipi_control/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 07:40:40.000000 unipi-control-2.1.0/unipi_control/tools/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3214 2023-07-14 07:40:40.000000 unipi-control-2.1.0/unipi_control/tools/config_backup.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5217 2023-07-14 07:40:40.000000 unipi-control-2.1.0/unipi_control/tools/config_converter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2230 2023-07-14 07:40:40.000000 unipi-control-2.1.0/unipi_control/tools/model_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9563 2023-07-14 07:40:40.000000 unipi-control-2.1.0/unipi_control/unipi_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-14 07:41:06.000000 unipi-control-2.1.0/unipi_control/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:41:06.867072 unipi-control-2.1.0/unipi_control.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4916 2023-07-14 07:41:06.000000 unipi-control-2.1.0/unipi_control.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4538 2023-07-14 07:41:06.000000 unipi-control-2.1.0/unipi_control.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 07:41:06.000000 unipi-control-2.1.0/unipi_control.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-14 07:41:06.000000 unipi-control-2.1.0/unipi_control.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-14 07:41:06.000000 unipi-control-2.1.0/unipi_control.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-14 07:41:06.000000 unipi-control-2.1.0/unipi_control.egg-info/top_level.txt
```

### Comparing `unipi-control-2.0.0/.github/workflows/ci.yml` & `unipi-control-2.1.0/.github/workflows/ci.yml`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 name: CI
 
 on:
   workflow_dispatch:
+    inputs:
+      build-python-package:
+        description: Build python package
+        type: boolean
   pull_request:
   push:
+    branches:
+      - main
     tags:
       - v*
 
 jobs:
   parameters:
     name: Parameters
     uses: superbox-dev/python-package-workflows/.github/workflows/parameters.yml@main
@@ -47,29 +53,37 @@
       - parameters
     with:
       latest-python-version: ${{ needs.parameters.outputs.latest-python-version }}
 
   build-python-package:
     name: Build python package
     if: |
-      contains(fromJSON('["tag", "branch"]'), github.ref_type)
+      github.ref_type == 'tag'
+      || (
+        github.ref_type == 'branch'
+        && inputs.build-python-package
+      )
       && !endsWith(github.ref_name, '/merge')
     uses: superbox-dev/python-package-workflows/.github/workflows/build-python-package.yml@main
     needs:
       - parameters
       - unit-testing
       - code-analyse
     with:
       latest-python-version: ${{ needs.parameters.outputs.latest-python-version }}
       package-version: ${{ needs.parameters.outputs.package-version }}
 
   build-binary-files:
     name: Build binary files
     if: |
-      contains(fromJSON('["tag", "branch"]'), github.ref_type)
+      github.ref_type == 'tag'
+      || (
+        github.ref_type == 'branch'
+        && inputs.build-python-package
+      )
       && !endsWith(github.ref_name, '/merge')
     uses: superbox-dev/python-package-workflows/.github/workflows/build-binary-files.yml@main
     needs:
       - parameters
       - unit-testing
       - code-analyse
     with:
@@ -116,12 +130,13 @@
       ftp-publish-path: ${{ vars.FTP_PUBLISH_PATH }}
       is-dev-version: ${{ needs.parameters.outputs.is-dev-version }}
     secrets:
       FTP_PASSWORD: ${{ secrets.FILES_SUPERBOX_ONE_FTP_PASSWORD }}
 
   publish-on-pypi:
     name: Publish
+    if: github.ref_type == 'tag'
     needs:
       - release
     uses: superbox-dev/python-package-workflows/.github/workflows/publish-on-pypi.yml@main
     secrets:
       PYPI_API_TOKEN: ${{ secrets.PYPI_API_TOKEN }}
```

### Comparing `unipi-control-2.0.0/.yamllint.yml` & `unipi-control-2.1.0/.yamllint.yml`

 * *Files identical despite different names*

### Comparing `unipi-control-2.0.0/CHANGELOG.md` & `unipi-control-2.1.0/CHANGELOG.md`

 * *Files 16% similar despite different names*

```diff
@@ -3,14 +3,32 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [2.1.0] - 2023-07-14
+
+### Added
+
+- Added `advanced` section in `control.yaml` with the option `persistent_tmp_dir`.
+- Added documentation in [configuration.md](docs/configuration.md) for the `advanced` section.
+
+### Changed
+
+- Bump pymodbus to version 3.3.2
+- Bump ayncio-mqtt to version 1.0.0 (the package name changed to aiomqtt)
+
+## Fixed
+
+- Fixed crashing Unipi Control service after reinstall/update `unipi-modbus-tools` OPKG package.
+- Added `Restart=on-failure` for systemd service, in the OPKG package, to prevent unwanted crashes.
+- Repair the OPKG package for the Unipi Control OS. Added the missing control files to the package. 
+
 ## [2.0.0] - 2023-06-23
 
 ### Added
 
 - This CHANGELOG.md
 - Added the developer guide to [CONTRIBUTING.md](CONTRIBUTING.md)
 - Added `setuptools_scm` for automatic versioning.
```

### Comparing `unipi-control-2.0.0/CONTRIBUTING.md` & `unipi-control-2.1.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `unipi-control-2.0.0/LICENSE` & `unipi-control-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `unipi-control-2.0.0/PKG-INFO` & `unipi-control-2.1.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unipi-control
-Version: 2.0.0
+Version: 2.1.0
 Summary: Control Unipi I/O directly with MQTT commands.
 Author-email: Michael Hacker <mh@superbox.one>
 Maintainer-email: Michael Hacker <mh@superbox.one>
 License: Apache-2.0 license
 Project-URL: Source code, https://github.com/superbox-dev/unipi-control
 Project-URL: Issue tracker, https://github.com/superbox-dev/unipi-control/issues
 Keywords: mqtt,modbus,unipi
@@ -24,27 +24,41 @@
 Provides-Extra: build
 Provides-Extra: audit
 Provides-Extra: format
 Provides-Extra: lint
 Provides-Extra: tests
 License-File: LICENSE
 
-[![license-url](https://img.shields.io/badge/license-Apache%202-yellowgreen)](https://opensource.org/license/apache-2-0/)
 ![coverage-badge](https://raw.githubusercontent.com/superbox-dev/unipi-control/main/coverage.svg)
+[![CI](https://github.com/superbox-dev/unipi-control/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/superbox-dev/unipi-control/actions/workflows/ci.yml)
 ![Python 3.8](https://img.shields.io/badge/python-3.8-blue.svg)
 ![Python 3.9](https://img.shields.io/badge/python-3.9-blue.svg)
 ![Python 3.10](https://img.shields.io/badge/python-3.10-blue.svg)
 ![Python 3.11](https://img.shields.io/badge/python-3.11-blue.svg)
+![Python 3.11](https://img.shields.io/badge/python-3.11-blue.svg)
+
+[![license-url](https://img.shields.io/badge/license-Apache%202-yellowgreen)](https://opensource.org/license/apache-2-0/)
+![PyPi downloads](https://img.shields.io/pypi/dm/unipi-control)
+![Typing: strict](https://img.shields.io/badge/typing-strict-green.svg)
+![Code style: black](https://img.shields.io/badge/code%20style-black-black)
+![Code style: Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)
 
 <!-- pitch start -->
 # Unipi Control
 
 Unipi Control use Modbus for fast access to the I/O and provide MQTT topics for reading and writing the circuits. Optionally you can enable the Home Assistant MQTT discovery for binary sensors, sensors, switches and covers.
 <!-- pitch end -->
 
+---
+
+For more information please read the documentation at:
+[docs.superbox.one](https://docs.superbox.one)
+
+---
+
 <!-- quickstart start -->
 ## Getting started
 
 ### Recommended installation (only for Unipi Neuron)
 
 We have a ready to use SD card image called [Unipi Control OS](https://github.com/superbox-dev/unipi-control-os).
 
@@ -69,15 +83,15 @@
 
 Install `unipi-control` with pip:
 
 ```bash
 pip install unipi-control
 ```
 
-Copy the [config files](data/opkg/data/local/etc/unipi) to `/etc/unipi` and configurate the `/etc/unipi/control.yaml`.
+Copy the [config files](https://github.com/superbox-dev/unipi-control/data/opkg/data/local/etc/unipi) to `/etc/unipi` and configurate the `/etc/unipi/control.yaml`.
 
 Create the systemd service `/etc/systemd/system/unipi-control.service` with following content:
 
 ```ini
 [Unit]
 Description=Unipi Control
 After=multi-user.target
@@ -94,15 +108,15 @@
 Enable and start the systemd service:
 
 ```bash
 systemctl --system daemon-reload
 systemctl enable unipi-control.service
 systemctl start unipi-control.service
 ```
-<!-- quickstart start -->
+<!-- quickstart end -->
 
 ## Changelog
 
 The changelog lives in the [CHANGELOG.md](CHANGELOG.md) document. The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/).
 
 ## Contributing
```

### Comparing `unipi-control-2.0.0/README.md` & `unipi-control-2.1.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,34 @@
-[![license-url](https://img.shields.io/badge/license-Apache%202-yellowgreen)](https://opensource.org/license/apache-2-0/)
 ![coverage-badge](https://raw.githubusercontent.com/superbox-dev/unipi-control/main/coverage.svg)
+[![CI](https://github.com/superbox-dev/unipi-control/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/superbox-dev/unipi-control/actions/workflows/ci.yml)
 ![Python 3.8](https://img.shields.io/badge/python-3.8-blue.svg)
 ![Python 3.9](https://img.shields.io/badge/python-3.9-blue.svg)
 ![Python 3.10](https://img.shields.io/badge/python-3.10-blue.svg)
 ![Python 3.11](https://img.shields.io/badge/python-3.11-blue.svg)
+![Python 3.11](https://img.shields.io/badge/python-3.11-blue.svg)
+
+[![license-url](https://img.shields.io/badge/license-Apache%202-yellowgreen)](https://opensource.org/license/apache-2-0/)
+![PyPi downloads](https://img.shields.io/pypi/dm/unipi-control)
+![Typing: strict](https://img.shields.io/badge/typing-strict-green.svg)
+![Code style: black](https://img.shields.io/badge/code%20style-black-black)
+![Code style: Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)
 
 <!-- pitch start -->
 # Unipi Control
 
 Unipi Control use Modbus for fast access to the I/O and provide MQTT topics for reading and writing the circuits. Optionally you can enable the Home Assistant MQTT discovery for binary sensors, sensors, switches and covers.
 <!-- pitch end -->
 
+---
+
+For more information please read the documentation at:
+[docs.superbox.one](https://docs.superbox.one)
+
+---
+
 <!-- quickstart start -->
 ## Getting started
 
 ### Recommended installation (only for Unipi Neuron)
 
 We have a ready to use SD card image called [Unipi Control OS](https://github.com/superbox-dev/unipi-control-os).
 
@@ -39,15 +53,15 @@
 
 Install `unipi-control` with pip:
 
 ```bash
 pip install unipi-control
 ```
 
-Copy the [config files](data/opkg/data/local/etc/unipi) to `/etc/unipi` and configurate the `/etc/unipi/control.yaml`.
+Copy the [config files](https://github.com/superbox-dev/unipi-control/data/opkg/data/local/etc/unipi) to `/etc/unipi` and configurate the `/etc/unipi/control.yaml`.
 
 Create the systemd service `/etc/systemd/system/unipi-control.service` with following content:
 
 ```ini
 [Unit]
 Description=Unipi Control
 After=multi-user.target
@@ -64,15 +78,15 @@
 Enable and start the systemd service:
 
 ```bash
 systemctl --system daemon-reload
 systemctl enable unipi-control.service
 systemctl start unipi-control.service
 ```
-<!-- quickstart start -->
+<!-- quickstart end -->
 
 ## Changelog
 
 The changelog lives in the [CHANGELOG.md](CHANGELOG.md) document. The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/).
 
 ## Contributing
```

### Comparing `unipi-control-2.0.0/coverage.svg` & `unipi-control-2.1.0/coverage.svg`

 * *Files identical despite different names*

### Comparing `unipi-control-2.0.0/data/extras/homeassistant/blueprints/automation/cover/control.yaml` & `unipi-control-2.1.0/data/extras/homeassistant/blueprints/automation/cover/control.yaml`

 * *Files identical despite different names*

### Comparing `unipi-control-2.0.0/data/extras/homeassistant/blueprints/automation/cover/simple_cover_control.yaml` & `unipi-control-2.1.0/data/extras/homeassistant/blueprints/automation/cover/simple_cover_control.yaml`

 * *Files identical despite different names*

### Comparing `unipi-control-2.0.0/data/opkg/data/usr/local/etc/unipi/control.yaml.example` & `unipi-control-2.1.0/data/opkg/data/usr/local/etc/unipi/control.yaml.example`

 * *Files identical despite different names*

### Comparing `unipi-control-2.0.0/data/opkg/data/usr/local/etc/unipi/hardware/extensions/Eastron_SDM120M.yaml` & `unipi-control-2.1.0/data/opkg/data/usr/local/etc/unipi/hardware/extensions/Eastron_SDM120M.yaml`

 * *Files identical despite different names*

### Comparing `unipi-control-2.0.0/data/opkg/data/usr/local/etc/unipi/hardware/neuron/L203.yaml` & `unipi-control-2.1.0/data/opkg/data/usr/local/etc/unipi/hardware/neuron/L203.yaml`

 * *Files identical despite different names*

### Comparing `unipi-control-2.0.0/data/opkg/data/usr/local/etc/unipi/hardware/neuron/L207.yaml` & `unipi-control-2.1.0/data/opkg/data/usr/local/etc/unipi/hardware/neuron/L207.yaml`

 * *Files identical despite different names*

### Comparing `unipi-control-2.0.0/data/opkg/data/usr/local/etc/unipi/hardware/neuron/L523.yaml` & `unipi-control-2.1.0/data/opkg/data/usr/local/etc/unipi/hardware/neuron/L523.yaml`

 * *Files identical despite different names*

### Comparing `unipi-control-2.0.0/data/opkg/data/usr/local/etc/unipi/hardware/neuron/L527.yaml` & `unipi-control-2.1.0/data/opkg/data/usr/local/etc/unipi/hardware/neuron/L527.yaml`

 * *Files identical despite different names*

### Comparing `unipi-control-2.0.0/data/opkg/data/usr/local/etc/unipi/hardware/neuron/L533.yaml` & `unipi-control-2.1.0/data/opkg/data/usr/local/etc/unipi/hardware/neuron/L533.yaml`

 * *Files identical despite different names*

### Comparing `unipi-control-2.0.0/data/opkg/data/usr/local/etc/unipi/hardware/neuron/M103.yaml` & `unipi-control-2.1.0/data/opkg/data/usr/local/etc/unipi/hardware/neuron/M103.yaml`

 * *Files identical despite different names*

### Comparing `unipi-control-2.0.0/data/opkg/data/usr/local/etc/unipi/hardware/neuron/M203.yaml` & `unipi-control-2.1.0/data/opkg/data/usr/local/etc/unipi/hardware/neuron/M203.yaml`

 * *Files identical despite different names*

### Comparing `unipi-control-2.0.0/data/opkg/data/usr/local/etc/unipi/hardware/neuron/M207.yaml` & `unipi-control-2.1.0/data/opkg/data/usr/local/etc/unipi/hardware/neuron/M207.yaml`

 * *Files identical despite different names*

### Comparing `unipi-control-2.0.0/data/opkg/data/usr/local/etc/unipi/hardware/neuron/M267.yaml` & `unipi-control-2.1.0/data/opkg/data/usr/local/etc/unipi/hardware/neuron/M267.yaml`

 * *Files identical despite different names*

### Comparing `unipi-control-2.0.0/data/opkg/data/usr/local/etc/unipi/hardware/neuron/M523.yaml` & `unipi-control-2.1.0/data/opkg/data/usr/local/etc/unipi/hardware/neuron/M523.yaml`

 * *Files identical despite different names*

### Comparing `unipi-control-2.0.0/data/opkg/data/usr/local/etc/unipi/hardware/neuron/M527.yaml` & `unipi-control-2.1.0/data/opkg/data/usr/local/etc/unipi/hardware/neuron/M527.yaml`

 * *Files identical despite different names*

### Comparing `unipi-control-2.0.0/data/opkg/data/usr/local/etc/unipi/hardware/neuron/M567.yaml` & `unipi-control-2.1.0/data/opkg/data/usr/local/etc/unipi/hardware/neuron/M567.yaml`

 * *Files identical despite different names*

### Comparing `unipi-control-2.0.0/docs/commands.md` & `unipi-control-2.1.0/docs/commands.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # Commands
 
+<!-- content start -->
 ## unipi-control
 
 **Usage:**
 
 ````bash
 unipi-control [--log {systemd,stdout,file}] [--config CONFIG]
 ````
@@ -45,7 +46,9 @@
 | Argument   | Description                                                                |          |
 |------------|----------------------------------------------------------------------------|----------|
 | `input`    | path to the evok YAML file                                                 | required |
 | `output`   | path to save the converted YAML file                                       | required |
 | `--force`  | overwrite output YAML file if already exists                               |          |
 | `--log`    | set log handler to file or systemd (choices: `systemd`, `stdout` or `file` |          |
 | `-v`       | verbose mode: multiple -v options increase the verbosity (maximum: 4)      |          |
+
+<!-- content end -->
```

### Comparing `unipi-control-2.0.0/docs/configuration.md` & `unipi-control-2.1.0/docs/configuration.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # Configuration
 
+<!-- content start -->
 This are the configuration settings for the `/etc/unipi/control.yaml`.
 
 ## Device
 
 | Key    | Value                                                                                                                                                               |
 |--------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | `name` | The device name for the subscribe and publish topics. Default is the hostname. This name must be unique. This is important if multiple Unipi devices are available. |
@@ -138,18 +139,35 @@
 ```
 
 ### Calibration
 
 The covers save its cover and tilt position in a temporary file each time a stop command is executed. If the Unipi Control is interrupted, and a command (open/closing) is currently being executed, or the system is restarted, the calibration mode is enabled.
 When the Unipi Control starts in calibration mode, the cover fully open and disable calibration mode. This is required for the correct cover and tilt position.
 
+> Cover calibration mode is disabled when `persistent_tmp_dir` is enabled! To manualy reset the covers you must delete all files under `/var/tmp/unipi`.
+
+## Advanced
+
+| Key                  | Value                                                                                                                                                                                               |
+|----------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| `persistent_tmp_dir` | Enable persistent temporary directory. All temporary files are written to `/var/tmp/unipi` instead of `/tmp/unipi`. Default is `false`. If this is enabled then cover calibration mode is disabled! |
+
+```yaml
+# control.yaml
+advanced:
+  persistent_tmp_dir: True
+```
+
+
 ## Logging
 
 | Key     | Value                                                                  |
 |---------|------------------------------------------------------------------------|
 | `level` | Set level to `debug`, `info`, `warning` or `error`. Default is `info`. |
 
 ```yaml
 # control.yaml
 logging:
   level: info
 ```
+
+<!-- content end -->
```

### Comparing `unipi-control-2.0.0/docs/mqtt-topics.md` & `unipi-control-2.1.0/docs/mqtt-topics.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # MQTT topics
 
+<!-- content start -->
 Available MQTT topics:
 
 ## Features
 
 ### Unipi Neuron
 
 | Topic                                         | Response/Request | Description                                                                                          |
@@ -47,7 +48,9 @@
 |--------------------------------------------------------|-----------------------------------------------------|----------------------------------------------------------------------|
 | `[device_name]/[object_id]/cover/[device_class]/state` | `open`, `opening`, `closing`, `closed` or `stopped` | Get the cover state.                                                 |
 | `[device_name]/[object_id]/cover/[device_class]/set`          | `OPEN`, `CLOSE` or `STOP`                    | Send a string to control the cover.                                  |
 | `[device_name]/[object_id]/cover/[device_class]/position`     | `0` to `100`                                 | Get the cover position. `100` is fully open and `0` is fully closed. |
 | `[device_name]/[object_id]/cover/[device_class]/position/set` | `0` to `100`                                 | Send an integer to set the cover position.                           |
 | `[device_name]/[object_id]/cover/[device_class]/tilt`         | `0` to `100`                                 | Get the tilt position. `100` is fully open and `0` is fully closed.  |
 | `[device_name]/[object_id]/cover/[device_class]/tilt/set`     | `0` to `100`                                 | Send an integer to set the cover position.                           |
+
+<!-- content end -->
```

### Comparing `unipi-control-2.0.0/docs/supported-hardware.md` & `unipi-control-2.1.0/docs/supported-hardware.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # Supported hardware
 
+<!-- content start -->
 > If you have an Unipi device, that is not supported, then contact us and [create a issue](https://github.com/superbox-dev/unipi-control/issues).
 
 ## Tested devices
 
 * Unipi Neuron
   * L203
 * External Modbus RTU devices
@@ -27,7 +28,9 @@
   * Patron M527
   * Patron M567
   * Patron S207
   * Patron L207
   * Patron L527
 
 If you tried an untested Unipi device then please let us know the result to update this page.
+
+<!-- content end -->
```

### Comparing `unipi-control-2.0.0/pyproject.toml` & `unipi-control-2.1.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -25,17 +25,17 @@
     "Programming Language :: Python :: 3 :: Only",
     "Operating System :: POSIX :: Linux",
     "Topic :: System :: Networking",
     "Topic :: Utilities",
 ]
 requires-python = ">= 3.8"
 dependencies = [
-    "asyncio-mqtt==0.16.1",
-    "pymodbus[serial]==3.2.2",
-    "pyyaml~=6.0"
+    "aiomqtt==1.0.0",
+    "pymodbus[serial]==3.3.2",
+    "pyyaml==6.0"
 ]
 dynamic = ["version"]
 
 [project.scripts]
 unipi-control = "unipi_control.unipi_control:main"
 unipi-config-backup = "unipi_control.tools.config_backup:main"
 unipi-config-converter = "unipi_control.tools.config_converter:main"
@@ -44,33 +44,37 @@
 [project.urls]
 "Source code" = "https://github.com/superbox-dev/unipi-control"
 "Issue tracker" = "https://github.com/superbox-dev/unipi-control/issues"
 
 [project.optional-dependencies]
 build = [
     "setuptools>=65.5.1",
-    "build"
+    "build==0.10.0",
+]
+audit = [
+    "pip-audit==2.6.0",
+]
+format = [
+    "black==23.3.0",
 ]
-audit = ["pip-audit"]
-format = ["black"]
 lint = [
-    "mypy",
-    "pylint",
-    "ruff",
-    "types-PyYAML",
-    "yamllint",
+    "mypy==1.4.1",
+    "pylint==2.17.4",
+    "ruff==0.0.277",
+    "types-PyYAML==6.0.12.10",
+    "yamllint==1.32.0",
 ]
 tests = [
-    "coverage",
-    "coverage-badge",
-    "pytest",
-    "pytest-asyncio",
-    "pytest-cov",
-    "pytest-mock",
-    "pytest-xdist[psutil]",
+    "coverage==7.2.7",
+    "coverage-badge==1.1.0",
+    "pytest==7.4.0",
+    "pytest-asyncio==0.21.0",
+    "pytest-cov==4.1.0",
+    "pytest-mock==3.11.1",
+    "pytest-xdist[psutil]==3.3.1",
 ]
 
 [tool.setuptools]
 packages = ["unipi_control"]
 
 [tool.setuptools_scm]
 write_to = "unipi_control/version.py"
@@ -84,28 +88,29 @@
 python_version = "3.10"
 ignore_missing_imports = true
 disallow_any_generics = false # python 3.8 compatibility
 junit_xml = "reports/mypy.xml"
 
 [tool.pylint.master]
 disable = [
-    "C0114", # missing-module-docstring
-    "C0115", # missing-class-docstring
-    "C0116", # missing-function-docstring
-    "C0411", # wrong-import-order
-    "E0401", # import-error
-    "R0801", # duplicate-code
-    "R0902", # too-many-instance-attributes
-    "R0903", # too-few-public-methods
-    "R0913", # too-many-arguments
-    "R2044", # empty-comment
-    "R6003", # consider-alternative-union-syntax (python 3.8 compatibility)
-    "W0212", # protected-access (ruff lint this)
-    "W6001", # deprecated-typing-alias (python 3.8 compatibility)
-    "W0613" # unused-argument (ruff lint this)
+    "C0103",  # invalid-name
+    "C0114",  # missing-module-docstring
+    "C0115",  # missing-class-docstring
+    "C0116",  # missing-function-docstring
+    "C0411",  # wrong-import-order
+    "E0401",  # import-error
+    "R0801",  # duplicate-code
+    "R0902",  # too-many-instance-attributes
+    "R0903",  # too-few-public-methods
+    "R0913",  # too-many-arguments
+    "R2044",  # empty-comment
+    "R6003",  # consider-alternative-union-syntax (python 3.8 compatibility)
+    "W0212",  # protected-access (ruff lint this)
+    "W6001",  # deprecated-typing-alias (python 3.8 compatibility)
+    "W0613"   # unused-argument (ruff lint this)
 ]
 notes = ["FIXME"]
 ignore-patterns = ["version.py"]
 
 load-plugins = [
     "pylint.extensions.bad_builtin",
     "pylint.extensions.check_elif",
@@ -137,49 +142,50 @@
 max-line-length = 120
 
 [tool.ruff]
 target-version = "py310"
 line-length = 120
 select = ["ALL"]
 ignore = [
-    "ANN101", # missing-type-self
-    "ANN002", # missing-type-args
-    "ANN003", # missing-type-kwargs
-    "COM", # trailing-comma
-    "D101", # undocumented-public-class
-    "D104", # undocumented-public-package
-    "D105", # undocumented-magic-method
-    "D107", # undocumented-public-init
-    "D203", # one-blank-line-before-class
-    "D213", # multi-line-summary-second-line
-    "ERA001", # commented-out-code
-    "FA100", # missing-future-annotations-import
-    "FBT", # boolean-trap
-    "S101", # assert-used
-    "T201", # print
+    "ANN101",  # missing-type-self
+    "ANN002",  # missing-type-args
+    "ANN003",  # missing-type-kwargs
+    "COM",     # trailing-comma
+    "D101",    # undocumented-public-class
+    "D104",    # undocumented-public-package
+    "D105",    # undocumented-magic-method
+    "D107",    # undocumented-public-init
+    "D203",    # one-blank-line-before-class
+    "D213",    # multi-line-summary-second-line
+    "ERA001",  # commented-out-code
+    "FA100",   # missing-future-annotations-import
+    "FBT",     # boolean-trap
+    "S101",    # assert-used
+    "S108",    # hardcoded-temp-file
+    "T201",    # print
     "PLR0913", # too-many-arguments
     "PLR2004", # magic-value-comparison
-    "I001", # unsorted-imports
-    "UP006", # non-pep585-annotation (python 3.8 compatibility)
-    "UP007", # non-pep604-annotation (python 3.8 compatibility)
-    "UP035", # deprecated-import (python 3.8 compatibility)
-    "UP038", # non-pep604-isinstance (python 3.8 compatibility)
+    "I001",    # unsorted-imports
+    "UP006",   # non-pep585-annotation (python 3.8 compatibility)
+    "UP007",   # non-pep604-annotation (python 3.8 compatibility)
+    "UP035",   # deprecated-import (python 3.8 compatibility)
+    "UP038",   # non-pep604-isinstance (python 3.8 compatibility)
 ]
 
 [tool.pytest.ini_options]
 log_cli = true
 log_cli_level = "DEBUG"
 log_cli_format = "%(levelname)-8s | %(asctime)s: %(message)s"
 # https://docs.pytest.org/en/latest/reference/reference.html#ini-options-ref
 addopts = "--color=yes --exitfirst --failed-first --strict-config --strict-markers --junitxml=reports/pytest.xml"
 
 [tool.coverage.run] # https://coverage.readthedocs.io/en/latest/config.html#run
 branch = false
 
 [tool.coverage.report] # https://coverage.readthedocs.io/en/latest/config.html#report
-fail_under = 80
+fail_under = 95
 show_missing = true
 skip_covered = true
 exclude_also = [
     "if TYPE_CHECKING:",
     "@(abc\\.)?abstractmethod",
 ]
```

### Comparing `unipi-control-2.0.0/scripts/entry.sh` & `unipi-control-2.1.0/scripts/entry.sh`

 * *Files identical despite different names*

### Comparing `unipi-control-2.0.0/tests/conftest.py` & `unipi-control-2.1.0/tests/conftest.py`

 * *Files 8% similar despite different names*

```diff
@@ -53,67 +53,72 @@
     loop.run_until_complete(group)
 
     loop.close()
 
 
 class ConfigLoader:
     def __init__(self, temp: Path) -> None:
-        self.temp: Path = temp
-        self.config_file_path: Path = self.temp / "control.yaml"
+        self.tmp_dir: Path = temp
+        self.config_file: Path = self.tmp_dir / "control.yaml"
 
-        hardware_data_path: Path = self.temp / "hardware/neuron"
-        hardware_data_path.mkdir(parents=True)
-        self.hardware_data_file_path = hardware_data_path / "MOCKED_MODEL.yaml"
-
-        extension_hardware_data_path: Path = self.temp / "hardware/extensions"
-        extension_hardware_data_path.mkdir(parents=True)
-        self.extension_hardware_data_file_path = extension_hardware_data_path / "MOCKED_EASTRON.yaml"
+        hardware_data_dir: Path = self.tmp_dir / "hardware/neuron"
+        hardware_data_dir.mkdir(parents=True)
+        self.hardware_data_file = hardware_data_dir / "MOCKED_MODEL.yaml"
+
+        extension_hardware_data_dir: Path = self.tmp_dir / "hardware/extensions"
+        extension_hardware_data_dir.mkdir(parents=True)
+        self.extension_hardware_data_file = extension_hardware_data_dir / "MOCKED_EASTRON.yaml"
 
-        self.temp_path: Path = self.temp / "unipi"
-        self.temp_path.mkdir(parents=True)
+        self.unipi_tmp_dir: Path = self.tmp_dir / "unipi"
+        self.unipi_tmp_dir.mkdir(parents=True)
 
     def write_config(self, content: str) -> None:
         """Write config yaml file to temporary directory.
 
         Parameters
         ----------
         content: str
             Content for the config yaml file
         """
-        with self.config_file_path.open("w", encoding="utf-8") as _file:
+        with self.config_file.open("w", encoding="utf-8") as _file:
             _file.write(content)
 
     def write_hardware_data(self, content: str) -> None:
         """Write hardware yaml file to temporary directory.
 
         Parameters
         ----------
         content: str
             Content for the hardware yaml file
         """
-        with self.hardware_data_file_path.open("w", encoding="utf-8") as _file:
+        with self.hardware_data_file.open("w", encoding="utf-8") as _file:
             _file.write(content)
 
     def write_extension_hardware_data(self, content: str) -> None:
         """Write extension hardware yaml file to temporary directory.
 
         Parameters
         ----------
         content: str
             Content for extension the hardware yaml file
         """
-        with self.extension_hardware_data_file_path.open("w", encoding="utf-8") as _file:
+        with self.extension_hardware_data_file.open("w", encoding="utf-8") as _file:
             _file.write(content)
 
-    def get_config(self, config_base_path: Optional[Path] = None) -> Config:
+    def get_config(self, config_base_dir: Optional[Path] = None, set_unipi_tmp_dir: bool = True) -> Config:
         """Get the config dataclass."""
-        if not config_base_path:
-            config_base_path = self.temp
+        if not config_base_dir:
+            config_base_dir = self.tmp_dir
 
-        return Config(config_base_path=config_base_path, temp_path=self.temp_path)
+        config: Dict[str, Any] = {"config_base_dir": config_base_dir}
+
+        if set_unipi_tmp_dir:
+            config["unipi_tmp_dir"] = self.unipi_tmp_dir
+
+        return Config(**config)
 
 
 @pytest.fixture(name="config_loader")
 def create_config(request: SubRequest, tmp_path: Path) -> ConfigLoader:
     """Create config yaml file in temporary directory.
 
     Parameters
```

### Comparing `unipi-control-2.0.0/tests/conftest_data.py` & `unipi-control-2.1.0/tests/conftest_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,14 +79,34 @@
     device_class: roller_shutter
     cover_up: ro_3_03
     cover_down: ro_3_04
 logging:
   level: debug
 """
 
+CONFIG_CONTENT_WITH_PERSISTENT_TMP_DIR: Final[
+    str
+] = """device_info:
+  name: MOCKED UNIPI
+advanced:
+  persistent_tmp_dir: True
+logging:
+  level: debug
+"""
+
+CONFIG_CONTENT_WITHOUT_PERSISTENT_TMP_DIR: Final[
+    str
+] = """device_info:
+  name: MOCKED UNIPI
+advanced:
+  persistent_tmp_dir: False
+logging:
+  level: debug
+"""
+
 HARDWARE_DATA_CONTENT: Final[
     str
 ] = """modbus_register_blocks:
     # DI 1.x / DO 1.x
   - start_reg: 0
     count: 2
     # LED 1.x
```

### Comparing `unipi-control-2.0.0/tests/integration/test_unipi_control.py` & `unipi-control-2.1.0/tests/integration/test_unipi_control.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,15 +25,15 @@
             (CONFIG_CONTENT, HARDWARE_DATA_CONTENT, EXTENSION_HARDWARE_DATA_CONTENT),
         ],
         indirect=["config_loader"],
     )
     def test_hardware_is_not_supported(self, config_loader: ConfigLoader, caplog: LogCaptureFixture) -> None:
         """Test for hardware is not supported."""
         with pytest.raises(SystemExit) as error:
-            main(["-c", config_loader.temp.as_posix()])
+            main(["-c", config_loader.tmp_dir.as_posix()])
 
         logs: List[str] = [record.getMessage() for record in caplog.records]
 
         assert "[CONFIG] Hardware is not supported!" in logs
         assert error.value.code == 1
 
     @pytest.mark.parametrize(
@@ -65,15 +65,15 @@
         mock_modbus_tcp: AsyncMock = mocker.patch("unipi_control.unipi_control.AsyncModbusTcpClient", autospec=True)
         mock_modbus_client_tcp: AsyncMock = mocker.patch.object(ModbusClient, "tcp", new_callable=AsyncMock)
         mock_modbus_client_tcp.params.host = "MOCKED_MODBUS_HOST"
         mock_modbus_client_tcp.params.port = "502"
         mock_modbus_client_tcp.connected = False
 
         with pytest.raises(SystemExit) as error:
-            main(["-c", config_loader.temp.as_posix()])
+            main(["-c", config_loader.tmp_dir.as_posix()])
 
         logs: List[str] = [record.getMessage() for record in caplog.records]
 
         assert mock_modbus_tcp.mock_calls == [
             call(host="localhost", timeout=0.5, retries=3, retry_on_empty=True),
         ]
 
@@ -116,15 +116,15 @@
             "unipi_control.unipi_control.AsyncModbusSerialClient", autospec=True
         )
         mock_modbus_client_serial: AsyncMock = mocker.patch.object(ModbusClient, "serial", new_callable=AsyncMock)
         mock_modbus_client_serial.params.port = "/dev/MOCKED"
         mock_modbus_client_serial.connected = False
 
         with pytest.raises(SystemExit) as error:
-            main(["-c", config_loader.temp.as_posix()])
+            main(["-c", config_loader.tmp_dir.as_posix()])
 
         logs: List[str] = [record.getMessage() for record in caplog.records]
 
         assert mock_modbus_tcp.mock_calls == [
             call(host="localhost", timeout=0.5, retries=3, retry_on_empty=True),
         ]
```

### Comparing `unipi-control-2.0.0/tests/integration/tools/test_config_backup.py` & `unipi-control-2.1.0/tests/integration/tools/test_config_backup.py`

 * *Files 14% similar despite different names*

```diff
@@ -24,21 +24,21 @@
         [
             (CONFIG_CONTENT, HARDWARE_DATA_CONTENT, EXTENSION_HARDWARE_DATA_CONTENT),
         ],
         indirect=["config_loader"],
     )
     def test_unipi_config_backup(self, config_loader: ConfigLoader, caplog: LogCaptureFixture) -> None:
         """Test for config backup."""
-        backup_path: Path = config_loader.temp_path / "backup"
-        backup_path.mkdir()
+        backup_dir: Path = config_loader.unipi_tmp_dir / "backup"
+        backup_dir.mkdir()
 
-        main([backup_path.as_posix(), "-c", config_loader.temp.as_posix()])
+        main([backup_dir.as_posix(), "-c", config_loader.tmp_dir.as_posix()])
 
         logs: List[str] = [record.getMessage() for record in caplog.records]
-        files: List[Path] = list(backup_path.glob("*.tar.gz"))
+        files: List[Path] = list(backup_dir.glob("*.tar.gz"))
 
         assert len(logs) == 1
         assert len(files) == 1
         assert re.match(r"^.*/config-\d{4}-\d{2}-\d{2}-\d{6}\.tar\.gz$", files[0].as_posix())
         assert ".tar.gz created!" in logs[0]
 
 
@@ -49,15 +49,15 @@
             (CONFIG_CONTENT, HARDWARE_DATA_CONTENT, EXTENSION_HARDWARE_DATA_CONTENT),
         ],
         indirect=["config_loader"],
     )
     def test_cli_output_directory_not_exists(self, config_loader: ConfigLoader, caplog: LogCaptureFixture) -> None:
         """Test for missing output directory."""
         with pytest.raises(SystemExit) as error:
-            main([(config_loader.temp_path / "not_exists").as_posix(), "-c", config_loader.temp.as_posix()])
+            main([(config_loader.unipi_tmp_dir / "not_exists").as_posix(), "-c", config_loader.tmp_dir.as_posix()])
 
         logs: List[str] = [record.getMessage() for record in caplog.records]
 
         assert len(logs) == 1
         assert "OUTPUT directory not exists!" in logs
         assert error.value.code == 1
 
@@ -67,15 +67,15 @@
             (CONFIG_CONTENT, HARDWARE_DATA_CONTENT, EXTENSION_HARDWARE_DATA_CONTENT),
         ],
         indirect=["config_loader"],
     )
     def test_cli_output_is_not_a_directory(self, config_loader: ConfigLoader, caplog: LogCaptureFixture) -> None:
         """Test for output is not a directory."""
         with pytest.raises(SystemExit) as error:
-            main([config_loader.config_file_path.as_posix(), "-c", config_loader.temp.as_posix()])
+            main([config_loader.config_file.as_posix(), "-c", config_loader.tmp_dir.as_posix()])
 
         logs: List[str] = [record.getMessage() for record in caplog.records]
 
         assert len(logs) == 1
         assert "OUTPUT is a file not a directory!" in logs
         assert error.value.code == 1
 
@@ -91,17 +91,17 @@
     ) -> None:
         """Test for tarfile error."""
         mock_tar_add = MagicMock()
         mock_tar_add.side_effect = OSError("MOCKED", "MOCKED", "MOCKED")
         mock_tarfile_open = mocker.patch.object(tarfile, "open")
         mock_tarfile_open.return_value.__enter__.return_value.add = mock_tar_add
 
-        backup_path: Path = config_loader.temp_path / "backup"
-        backup_path.mkdir()
+        backup_dir: Path = config_loader.unipi_tmp_dir / "backup"
+        backup_dir.mkdir()
 
         with pytest.raises(SystemExit) as error:
-            main([backup_path.as_posix(), "-c", config_loader.temp.as_posix()])
+            main([backup_dir.as_posix(), "-c", config_loader.tmp_dir.as_posix()])
 
         logs: List[str] = [record.getMessage() for record in caplog.records]
 
         assert "MOCKED: 'MOCKED'" in logs
         assert error.value.code == 1
```

### Comparing `unipi-control-2.0.0/tests/integration/tools/test_config_converter.py` & `unipi-control-2.1.0/tests/integration/tools/test_config_converter.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,98 +10,106 @@
     EVOK_MODEL_CONTENT,
     CONVERTED_MODEL_CONTENT,
     INVALID_EVOK_MODEL_CONTENT,
 )
 from unipi_control.tools.config_converter import main
 
 
-@pytest.fixture(name="evok_hardware_yaml")
-def create_evok_hardware_yaml(request: SubRequest, tmp_path: Path) -> Path:
+@pytest.fixture(name="evok_hardware_yaml_file")
+def create_evok_hardware_yaml_file(request: SubRequest, tmp_path: Path) -> Path:
     """Create evok hardware yaml file in temporary directory."""
-    evok_hardware_path: Path = tmp_path / "evok"
-    evok_hardware_path.mkdir()
-    evok_hardware_yaml: Path = evok_hardware_path / "MOCKED_MODEL.yaml"
-    evok_hardware_yaml.write_text(request.param)
+    evok_hardware_dir: Path = tmp_path / "evok"
+    evok_hardware_dir.mkdir()
+    evok_hardware_yaml_file: Path = evok_hardware_dir / "MOCKED_MODEL.yaml"
+    evok_hardware_yaml_file.write_text(request.param)
 
-    return evok_hardware_yaml
+    return evok_hardware_yaml_file
 
 
 class TestHappyPathUnipiConfigConverter:
-    @pytest.mark.parametrize("evok_hardware_yaml", [EVOK_MODEL_CONTENT], indirect=["evok_hardware_yaml"])
-    def test_unipi_config_converter(self, evok_hardware_yaml: Path, caplog: LogCaptureFixture) -> None:
+    @pytest.mark.parametrize("evok_hardware_yaml_file", [EVOK_MODEL_CONTENT], indirect=["evok_hardware_yaml_file"])
+    def test_unipi_config_converter(self, evok_hardware_yaml_file: Path, caplog: LogCaptureFixture) -> None:
         """Test content output of converted yaml file."""
-        hardware_data_file_path = evok_hardware_yaml.parent.parent / "MOCKED_MODEL.yaml"
-        main([evok_hardware_yaml.as_posix(), hardware_data_file_path.parent.as_posix()])
+        hardware_data_file = evok_hardware_yaml_file.parent.parent / "MOCKED_MODEL.yaml"
+        main([evok_hardware_yaml_file.as_posix(), hardware_data_file.parent.as_posix()])
 
         logs: List[str] = [record.getMessage() for record in caplog.records]
 
-        assert f"YAML file written to: {hardware_data_file_path.as_posix()}" in logs
-        assert hardware_data_file_path.read_text() == CONVERTED_MODEL_CONTENT
+        assert f"YAML file written to: {hardware_data_file.as_posix()}" in logs
+        assert hardware_data_file.read_text() == CONVERTED_MODEL_CONTENT
 
 
 class TestUnappyPathUnipiConfigConverter:
-    @pytest.mark.parametrize("evok_hardware_yaml", [INVALID_EVOK_MODEL_CONTENT], indirect=["evok_hardware_yaml"])
-    def test_invalid_input_yaml_file(self, evok_hardware_yaml: Path, caplog: LogCaptureFixture) -> None:
+    @pytest.mark.parametrize(
+        "evok_hardware_yaml_file", [INVALID_EVOK_MODEL_CONTENT], indirect=["evok_hardware_yaml_file"]
+    )
+    def test_invalid_input_yaml_file(self, evok_hardware_yaml_file: Path, caplog: LogCaptureFixture) -> None:
         """Test that input yaml file raises UnexpectedError for invalid yaml file."""
-        hardware_data_file_path = evok_hardware_yaml.parent.parent / "MOCKED_MODEL.yaml"
+        hardware_data_file = evok_hardware_yaml_file.parent.parent / "MOCKED_MODEL.yaml"
 
         with pytest.raises(SystemExit) as error:
-            main([evok_hardware_yaml.as_posix(), hardware_data_file_path.parent.as_posix()])
+            main([evok_hardware_yaml_file.as_posix(), hardware_data_file.parent.as_posix()])
 
         logs: List[str] = [record.getMessage() for record in caplog.records]
 
         assert "INPUT is not a valid YAML file!" in logs
         assert error.value.code == 1
 
-    @pytest.mark.parametrize("evok_hardware_yaml", [EVOK_MODEL_CONTENT], indirect=["evok_hardware_yaml"])
-    def test_output_yaml_file_already_exists(self, evok_hardware_yaml: Path, caplog: LogCaptureFixture) -> None:
+    @pytest.mark.parametrize("evok_hardware_yaml_file", [EVOK_MODEL_CONTENT], indirect=["evok_hardware_yaml_file"])
+    def test_output_yaml_file_already_exists(self, evok_hardware_yaml_file: Path, caplog: LogCaptureFixture) -> None:
         """Test that output yaml file raises UnexpectedError if file already exists."""
-        hardware_data_file_path = evok_hardware_yaml.parent.parent / "MOCKED_MODEL.yaml"
-        hardware_data_file_path.write_text(CONVERTED_MODEL_CONTENT)
+        hardware_data_file = evok_hardware_yaml_file.parent.parent / "MOCKED_MODEL.yaml"
+        hardware_data_file.write_text(CONVERTED_MODEL_CONTENT)
 
         with pytest.raises(SystemExit) as error:
-            main([evok_hardware_yaml.as_posix(), hardware_data_file_path.parent.as_posix()])
+            main([evok_hardware_yaml_file.as_posix(), hardware_data_file.parent.as_posix()])
 
         logs: List[str] = [record.getMessage() for record in caplog.records]
 
         assert "OUTPUT YAML file already exists!" in logs
         assert error.value.code == 1
 
-    @pytest.mark.parametrize("evok_hardware_yaml", [INVALID_EVOK_MODEL_CONTENT], indirect=["evok_hardware_yaml"])
-    def test_input_is_not_a_file(self, evok_hardware_yaml: Path, caplog: LogCaptureFixture) -> None:
+    @pytest.mark.parametrize(
+        "evok_hardware_yaml_file", [INVALID_EVOK_MODEL_CONTENT], indirect=["evok_hardware_yaml_file"]
+    )
+    def test_input_is_not_a_file(self, evok_hardware_yaml_file: Path, caplog: LogCaptureFixture) -> None:
         """Test that input yaml file raises UnexpectedError if input is not a file."""
-        hardware_data_file_path = evok_hardware_yaml.parent.parent / "MOCKED_MODEL.yaml"
+        hardware_data_file = evok_hardware_yaml_file.parent.parent / "MOCKED_MODEL.yaml"
 
         with pytest.raises(SystemExit) as error:
-            main([evok_hardware_yaml.parent.as_posix(), hardware_data_file_path.parent.as_posix()])
+            main([evok_hardware_yaml_file.parent.as_posix(), hardware_data_file.parent.as_posix()])
 
         logs: List[str] = [record.getMessage() for record in caplog.records]
 
         assert "INPUT is not a file!" in logs
         assert error.value.code == 1
 
-    @pytest.mark.parametrize("evok_hardware_yaml", [INVALID_EVOK_MODEL_CONTENT], indirect=["evok_hardware_yaml"])
-    def test_output_is_a_file(self, evok_hardware_yaml: Path, caplog: LogCaptureFixture) -> None:
+    @pytest.mark.parametrize(
+        "evok_hardware_yaml_file", [INVALID_EVOK_MODEL_CONTENT], indirect=["evok_hardware_yaml_file"]
+    )
+    def test_output_is_a_file(self, evok_hardware_yaml_file: Path, caplog: LogCaptureFixture) -> None:
         """Test that output yaml directory raises UnexpectedError if output is a file."""
-        hardware_data_file_path = evok_hardware_yaml.parent.parent / "MOCKED_MODEL.yaml"
-        hardware_data_file_path.write_text(CONVERTED_MODEL_CONTENT)
+        hardware_data_file = evok_hardware_yaml_file.parent.parent / "MOCKED_MODEL.yaml"
+        hardware_data_file.write_text(CONVERTED_MODEL_CONTENT)
 
         with pytest.raises(SystemExit) as error:
-            main([evok_hardware_yaml.as_posix(), hardware_data_file_path.as_posix()])
+            main([evok_hardware_yaml_file.as_posix(), hardware_data_file.as_posix()])
 
         logs: List[str] = [record.getMessage() for record in caplog.records]
 
         assert "OUTPUT is a file not a directory!" in logs
         assert error.value.code == 1
 
-    @pytest.mark.parametrize("evok_hardware_yaml", [INVALID_EVOK_MODEL_CONTENT], indirect=["evok_hardware_yaml"])
-    def test_output_directory_not_exists(self, evok_hardware_yaml: Path, caplog: LogCaptureFixture) -> None:
+    @pytest.mark.parametrize(
+        "evok_hardware_yaml_file", [INVALID_EVOK_MODEL_CONTENT], indirect=["evok_hardware_yaml_file"]
+    )
+    def test_output_directory_not_exists(self, evok_hardware_yaml_file: Path, caplog: LogCaptureFixture) -> None:
         """Test that output yaml directory raises UnexpectedError if not exists."""
-        hardware_data_file_path = evok_hardware_yaml.parent.parent / "NOT_EXISTS"
+        hardware_data_file = evok_hardware_yaml_file.parent.parent / "NOT_EXISTS"
 
         with pytest.raises(SystemExit) as error:
-            main([evok_hardware_yaml.as_posix(), hardware_data_file_path.as_posix()])
+            main([evok_hardware_yaml_file.as_posix(), hardware_data_file.as_posix()])
 
         logs: List[str] = [record.getMessage() for record in caplog.records]
 
         assert "OUTPUT directory not exists!" in logs
         assert error.value.code == 1
```

### Comparing `unipi-control-2.0.0/tests/integration/tools/test_config_converter_data.py` & `unipi-control-2.1.0/tests/integration/tools/test_config_converter_data.py`

 * *Files identical despite different names*

### Comparing `unipi-control-2.0.0/tests/unit/integrations/test_covers.py` & `unipi-control-2.1.0/tests/unit/integrations/test_covers.py`

 * *Files identical despite different names*

### Comparing `unipi-control-2.0.0/tests/unit/mqtt/discovery/test_binary_sensors.py` & `unipi-control-2.1.0/tests/unit/mqtt/discovery/test_binary_sensors.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from typing import List
 from typing import Set
 from typing import Union
 from unittest.mock import AsyncMock
 
 import pytest
 from _pytest.logging import LogCaptureFixture  # pylint: disable=import-private-name
-from asyncio_mqtt import Client
+from aiomqtt import Client
 
 from tests.conftest_data import CONFIG_CONTENT
 from tests.conftest_data import EXTENSION_HARDWARE_DATA_CONTENT
 from tests.conftest_data import HARDWARE_DATA_CONTENT
 from tests.unit.mqtt.discovery.test_binary_sensors_data import discovery_message_expected
 from unipi_control.features.neuron import DigitalInput
 from unipi_control.features.neuron import DigitalOutput
```

### Comparing `unipi-control-2.0.0/tests/unit/mqtt/discovery/test_binary_sensors_data.py` & `unipi-control-2.1.0/tests/unit/mqtt/discovery/test_binary_sensors_data.py`

 * *Files identical despite different names*

### Comparing `unipi-control-2.0.0/tests/unit/mqtt/discovery/test_covers.py` & `unipi-control-2.1.0/tests/unit/mqtt/discovery/test_covers.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from typing import Dict
 from typing import List
 from typing import Set
 from unittest.mock import AsyncMock
 
 import pytest
 from _pytest.logging import LogCaptureFixture  # pylint: disable=import-private-name
-from asyncio_mqtt import Client
+from aiomqtt import Client
 
 from tests.conftest_data import CONFIG_CONTENT
 from tests.conftest_data import EXTENSION_HARDWARE_DATA_CONTENT
 from tests.conftest_data import HARDWARE_DATA_CONTENT
 from unipi_control.config import DEVICE_CLASSES
 from unipi_control.integrations.covers import CoverMap
 from unipi_control.mqtt.discovery.covers import HassCoversMqttPlugin
```

### Comparing `unipi-control-2.0.0/tests/unit/mqtt/discovery/test_sensors.py` & `unipi-control-2.1.0/tests/unit/mqtt/discovery/test_sensors.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from typing import List
 from typing import Set
 from typing import Union
 from unittest.mock import AsyncMock
 
 import pytest
 from _pytest.logging import LogCaptureFixture  # pylint: disable=import-private-name
-from asyncio_mqtt import Client
+from aiomqtt import Client
 
 from tests.conftest_data import CONFIG_CONTENT
 from tests.conftest_data import EXTENSION_HARDWARE_DATA_CONTENT
 from tests.conftest_data import HARDWARE_DATA_CONTENT
 from tests.unit.mqtt.discovery.test_sensors_data import discovery_message_expected
 from unipi_control.features.extensions import EastronMeter
 from unipi_control.mqtt.discovery.sensors import HassSensorsDiscovery
```

### Comparing `unipi-control-2.0.0/tests/unit/mqtt/discovery/test_sensors_data.py` & `unipi-control-2.1.0/tests/unit/mqtt/discovery/test_sensors_data.py`

 * *Files identical despite different names*

### Comparing `unipi-control-2.0.0/tests/unit/mqtt/discovery/test_switches.py` & `unipi-control-2.1.0/tests/unit/mqtt/discovery/test_switches.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from typing import List
 from typing import Set
 from typing import Union
 from unittest.mock import AsyncMock
 
 import pytest
 from _pytest.logging import LogCaptureFixture  # pylint: disable=import-private-name
-from asyncio_mqtt import Client
+from aiomqtt import Client
 
 from tests.conftest_data import CONFIG_CONTENT
 from tests.conftest_data import EXTENSION_HARDWARE_DATA_CONTENT
 from tests.conftest_data import HARDWARE_DATA_CONTENT
 from tests.unit.mqtt.discovery.test_switches_data import discovery_message_expected
 from unipi_control.features.neuron import DigitalInput
 from unipi_control.features.neuron import DigitalOutput
```

### Comparing `unipi-control-2.0.0/tests/unit/mqtt/discovery/test_switches_data.py` & `unipi-control-2.1.0/tests/unit/mqtt/discovery/test_switches_data.py`

 * *Files identical despite different names*

### Comparing `unipi-control-2.0.0/tests/unit/mqtt/integrations/test_covers.py` & `unipi-control-2.1.0/tests/unit/mqtt/integrations/test_covers.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from typing import List
 from typing import Set
 from unittest.mock import AsyncMock
 from unittest.mock import PropertyMock
 
 import pytest
 from _pytest.logging import LogCaptureFixture  # pylint: disable=import-private-name
-from asyncio_mqtt import Client
+from aiomqtt import Client
 from pytest_mock import MockerFixture
 
 from tests.conftest import MockMQTTMessages
 from tests.conftest_data import EXTENSION_HARDWARE_DATA_CONTENT
 from tests.conftest_data import HARDWARE_DATA_CONTENT
 from tests.unit.mqtt.integrations.test_covers_data import CONFIG_CONTENT
 from unipi_control.integrations.covers import Cover
```

### Comparing `unipi-control-2.0.0/tests/unit/mqtt/integrations/test_covers_data.py` & `unipi-control-2.1.0/tests/unit/mqtt/integrations/test_covers_data.py`

 * *Files identical despite different names*

### Comparing `unipi-control-2.0.0/tests/unit/mqtt/test_features.py` & `unipi-control-2.1.0/tests/unit/mqtt/test_features.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from unittest.mock import AsyncMock
 from unittest.mock import MagicMock
 from unittest.mock import PropertyMock
 from unittest.mock import call
 
 import pytest
 from _pytest.logging import LogCaptureFixture  # pylint: disable=import-private-name
-from asyncio_mqtt import Client
+from aiomqtt import Client
 from pytest_mock import MockerFixture
 
 from tests.conftest import MockMQTTMessages
 from tests.conftest_data import CONFIG_CONTENT
 from tests.conftest_data import EXTENSION_HARDWARE_DATA_CONTENT
 from tests.conftest_data import HARDWARE_DATA_CONTENT
 from unipi_control.mqtt.features import MeterFeaturesMqttPlugin
```

### Comparing `unipi-control-2.0.0/tests/unit/test_config.py` & `unipi-control-2.1.0/tests/unit/test_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 """Unit test for configurations."""
 import logging
 import re
+from pathlib import Path
 from typing import Dict
 from typing import List
 from typing import NamedTuple
 from typing import Optional
 from unittest.mock import PropertyMock
 
 import pytest
 from _pytest.capture import CaptureFixture  # pylint: disable=import-private-name
 from _pytest.logging import LogCaptureFixture  # pylint: disable=import-private-name
 from pytest_mock import MockerFixture
 
 from tests.conftest import ConfigLoader
 from tests.conftest import MockHardwareInfo
 from tests.conftest_data import CONFIG_CONTENT
+from tests.conftest_data import CONFIG_CONTENT_WITHOUT_PERSISTENT_TMP_DIR
+from tests.conftest_data import CONFIG_CONTENT_WITH_PERSISTENT_TMP_DIR
 from tests.conftest_data import EXTENSION_HARDWARE_DATA_CONTENT
 from tests.conftest_data import HARDWARE_DATA_CONTENT
 from tests.unit.test_config_data import CONFIG_DUPLICATE_COVERS_CIRCUITS
 from tests.unit.test_config_data import CONFIG_DUPLICATE_COVER_ID
 from tests.unit.test_config_data import CONFIG_DUPLICATE_MODBUS_UNIT
 from tests.unit.test_config_data import CONFIG_DUPLICATE_OBJECT_ID
 from tests.unit.test_config_data import CONFIG_INVALID
@@ -29,14 +32,15 @@
 from tests.unit.test_config_data import CONFIG_INVALID_FEATURE_ID
 from tests.unit.test_config_data import CONFIG_INVALID_FEATURE_TYPE
 from tests.unit.test_config_data import CONFIG_INVALID_HOMEASSISTANT_DISCOVERY_PREFIX
 from tests.unit.test_config_data import CONFIG_INVALID_LOG_LEVEL
 from tests.unit.test_config_data import CONFIG_INVALID_MODBUS_BAUD_RATE
 from tests.unit.test_config_data import CONFIG_INVALID_MODBUS_PARITY
 from tests.unit.test_config_data import CONFIG_INVALID_MQTT_PORT_TYPE
+from tests.unit.test_config_data import CONFIG_INVALID_PERSISTENT_TMP_DIR
 from tests.unit.test_config_data import CONFIG_LOGGING_LEVEL_ERROR
 from tests.unit.test_config_data import CONFIG_LOGGING_LEVEL_INFO
 from tests.unit.test_config_data import CONFIG_MISSING_COVER_KEY
 from tests.unit.test_config_data import CONFIG_MISSING_DEVICE_NAME
 from tests.unit.test_config_data import EXTENSION_HARDWARE_DATA_INVALID_KEY
 from tests.unit.test_config_data import EXTENSION_HARDWARE_DATA_IS_INVALID_YAML
 from tests.unit.test_config_data import EXTENSION_HARDWARE_DATA_IS_LIST
@@ -208,14 +212,36 @@
 
         neuron: Neuron = Neuron(config=config, modbus_client=modbus_client)
         await neuron.init()
 
         logs: List[str] = [record.getMessage() for record in caplog.records]
         assert "[CONFIG] 2 hardware definition(s) found." in logs
 
+    @pytest.mark.asyncio()
+    @pytest.mark.parametrize(
+        ("config_loader", "expected"),
+        [
+            (
+                (CONFIG_CONTENT_WITH_PERSISTENT_TMP_DIR, HARDWARE_DATA_CONTENT, EXTENSION_HARDWARE_DATA_CONTENT),
+                "/var/tmp/unipi",
+            ),
+            (
+                (CONFIG_CONTENT_WITHOUT_PERSISTENT_TMP_DIR, HARDWARE_DATA_CONTENT, EXTENSION_HARDWARE_DATA_CONTENT),
+                "/tmp/unipi",
+            ),
+        ],
+        indirect=["config_loader"],
+    )
+    def test_unipi_tmp_dir(self, config_loader: ConfigLoader, expected: str) -> None:
+        """Test persistent temporary directory."""
+        config: Config = config_loader.get_config(set_unipi_tmp_dir=False)
+        config.logging.init()
+
+        assert config.unipi_tmp_dir == Path(expected)
+
 
 class TestUnhappyPathConfig:
     @pytest.mark.parametrize(
         ("config_loader", "expected"),
         [
             (
                 (CONFIG_INVALID_DEVICE_NAME, HARDWARE_DATA_CONTENT, EXTENSION_HARDWARE_DATA_CONTENT),
@@ -301,14 +327,18 @@
                 (CONFIG_DUPLICATE_MODBUS_UNIT, HARDWARE_DATA_CONTENT, EXTENSION_HARDWARE_DATA_CONTENT),
                 "[MODBUS] Duplicate modbus unit '1' found in 'units'!",
             ),
             (
                 (CONFIG_MISSING_DEVICE_NAME, HARDWARE_DATA_CONTENT, EXTENSION_HARDWARE_DATA_CONTENT),
                 "[MODBUS] Device name for unit '1' is missing!",
             ),
+            (
+                (CONFIG_INVALID_PERSISTENT_TMP_DIR, HARDWARE_DATA_CONTENT, EXTENSION_HARDWARE_DATA_CONTENT),
+                "Expected persistent_tmp_dir to be <class 'bool'>, got 'invalid'",
+            ),
         ],
         indirect=["config_loader"],
     )
     def test_validation(self, config_loader: ConfigLoader, expected: str) -> None:
         """Test yaml config raises ConfigError when validation failed."""
         with pytest.raises(ConfigError) as error:
             config_loader.get_config()
@@ -339,15 +369,15 @@
     ) -> None:
         """Test invalid neuron hardware definition."""
         config: Config = config_loader.get_config()
 
         with pytest.raises(ConfigError) as error:
             Neuron(config=config, modbus_client=modbus_client)
 
-        assert str(error.value) == f"[CONFIG] Definition is invalid: {config_loader.hardware_data_file_path}{expected}"
+        assert str(error.value) == f"[CONFIG] Definition is invalid: {config_loader.hardware_data_file}{expected}"
 
     @pytest.mark.parametrize(
         ("config_loader", "expected"),
         [
             (
                 (CONFIG_CONTENT, HARDWARE_DATA_CONTENT, EXTENSION_HARDWARE_DATA_INVALID_KEY),
                 "\nKeyError: 'modbus_register_blocks'",
@@ -371,15 +401,15 @@
         config: Config = config_loader.get_config()
 
         with pytest.raises(ConfigError) as error:
             Neuron(config=config, modbus_client=modbus_client)
 
         assert (
             str(error.value)
-            == f"[CONFIG] Definition is invalid: {config_loader.extension_hardware_data_file_path}{expected}"
+            == f"[CONFIG] Definition is invalid: {config_loader.extension_hardware_data_file}{expected}"
         )
 
     @pytest.mark.parametrize(
         ("config_loader", "hardware_info", "expected"),
         [
             (
                 (CONFIG_CONTENT, HARDWARE_DATA_CONTENT, EXTENSION_HARDWARE_DATA_CONTENT),
```

### Comparing `unipi-control-2.0.0/tests/unit/test_config_data.py` & `unipi-control-2.1.0/tests/unit/test_config_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -262,14 +262,21 @@
   baud_rate: 2400
   units:
     - unit: 1
       identifier: Eastron_SDM120M
 logging:
   level: debug"""
 
+CONFIG_INVALID_PERSISTENT_TMP_DIR: Final[
+    str
+] = """device_info:
+  name: MOCKED UNIPI
+advanced:
+  persistent_tmp_dir: invalid
+"""
 
 HARDWARE_DATA_INVALID_KEY: Final[
     str
 ] = """modbus_register_block:
     # DI 1.x / DO 1.x
   - start_reg: 0
     count: 2
```

### Comparing `unipi-control-2.0.0/tests/unit/test_features.py` & `unipi-control-2.1.0/tests/unit/test_features.py`

 * *Files identical despite different names*

### Comparing `unipi-control-2.0.0/tests/unit/test_modbus.py` & `unipi-control-2.1.0/tests/unit/test_modbus.py`

 * *Files identical despite different names*

### Comparing `unipi-control-2.0.0/tests/unit/test_neuron.py` & `unipi-control-2.1.0/tests/unit/test_neuron.py`

 * *Files identical despite different names*

### Comparing `unipi-control-2.0.0/unipi_control/config.py` & `unipi-control-2.1.0/unipi_control/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,42 +7,41 @@
 import struct
 import typing
 from dataclasses import dataclass
 from dataclasses import field
 from dataclasses import is_dataclass
 from functools import cached_property
 from pathlib import Path
-from tempfile import gettempdir
 from typing import Any
 from typing import Dict
 from typing import Final
 from typing import Iterator
 from typing import List
 from typing import Mapping
 from typing import NamedTuple
 from typing import Optional
 from typing import Tuple
 from typing import Type
 from typing import Union
 
-from asyncio_mqtt.client import MQTT_LOGGER
+from aiomqtt.client import MQTT_LOGGER
 
 from unipi_control.helpers.exception import ConfigError
 from unipi_control.helpers.exception import YamlError
 from unipi_control.helpers.log import LOG_FORMAT
 from unipi_control.helpers.log import LOG_LEVEL
 from unipi_control.helpers.log import LOG_NAME
 from unipi_control.helpers.log import SIMPLE_LOG_FORMAT
 from unipi_control.helpers.log import SystemdHandler
 from unipi_control.helpers.typing import HardwareDefinition
 from unipi_control.helpers.yaml import yaml_loader_safe
 
 UNIPI_LOGGER: logging.Logger = logging.getLogger(LOG_NAME)
 
-DEFAULT_CONFIG_PATH: Final[Path] = Path("/etc/unipi")
+DEFAULT_CONFIG_DIR: Final[Path] = Path("/etc/unipi")
 DEVICE_CLASSES: Final[List[str]] = ["blind", "roller_shutter", "garage_door"]
 
 MODBUS_BAUD_RATES: Final[List[int]] = [2400, 4800, 9600, 19200, 38400, 57600, 115200]
 MODBUS_PARITY: Final[List[str]] = ["E", "O", "N"]
 
 
 class LogPrefix:
@@ -129,25 +128,25 @@
                             _value = self._update_field_with_dataclass(value, name=_field.name, field_type=_field.type)
                             break
 
                     setattr(self, key, _value)
 
         self.validate()
 
-    def update_from_yaml_file(self, config_path: Path) -> None:
+    def update_from_yaml_file(self, config_file: Path) -> None:
         """Update and validate config data class with settings from a YAML file.
 
         Parameters
         ----------
-        config_path: Path
+        config_file: Path
             Path to the YAML file.
         """
-        if config_path.is_file() and config_path.exists():
+        if config_file.is_file() and config_file.exists():
             try:
-                yaml_data: Dict[str, Any] = yaml_loader_safe(config_path)
+                yaml_data: Dict[str, Any] = yaml_loader_safe(config_file)
             except YamlError as error:
                 raise ConfigError(error) from error
 
             if isinstance(yaml_data, dict):
                 self.update(yaml_data)
 
     def validate(self) -> None:
@@ -340,14 +339,19 @@
             )
             raise ConfigError(exception_message)
 
         return value
 
 
 @dataclass
+class AdvancedConfig(ConfigLoaderMixin):
+    persistent_tmp_dir: bool = False
+
+
+@dataclass
 class LoggingConfig(ConfigLoaderMixin):
     level: str = field(default="error")
 
     @property
     def verbose(self) -> int:
         """Get logging verbose level as integer."""
         return list(LOG_LEVEL).index(self.level)
@@ -415,27 +419,31 @@
 class Config(ConfigLoaderMixin):  # pylint: disable=too-many-instance-attributes
     device_info: DeviceInfo = field(default_factory=DeviceInfo)
     mqtt: MqttConfig = field(default_factory=MqttConfig)
     modbus: ModbusConfig = field(default_factory=ModbusConfig)
     homeassistant: HomeAssistantConfig = field(default_factory=HomeAssistantConfig)
     features: Dict[str, FeatureConfig] = field(init=False, default_factory=dict)
     covers: List[CoverConfig] = field(init=False, default_factory=list)
+    advanced: AdvancedConfig = field(default_factory=AdvancedConfig)
     logging: LoggingConfig = field(default_factory=LoggingConfig)
-    config_base_path: Path = field(default=DEFAULT_CONFIG_PATH)
-    temp_path: Path = field(default=Path(gettempdir()) / "unipi")
-    sys_bus: Path = field(default=Path("/sys/bus/i2c/devices"))
+    config_base_dir: Path = field(default=DEFAULT_CONFIG_DIR)
+    unipi_tmp_dir: Path = field(default=Path("/tmp/unipi"))
+    sys_bus_dir: Path = field(default=Path("/sys/bus/i2c/devices"))
 
     @cached_property
-    def hardware_path(self) -> Path:
+    def hardware_dir(self) -> Path:
         """Return hardware path to neuron devices and extensions."""
-        return self.config_base_path / "hardware"
+        return self.config_base_dir / "hardware"
 
     def __post_init__(self) -> None:
-        self.temp_path.mkdir(exist_ok=True)
-        self.update_from_yaml_file(config_path=self.config_base_path / "control.yaml")
+        self.unipi_tmp_dir.mkdir(exist_ok=True)
+        self.update_from_yaml_file(config_file=self.config_base_dir / "control.yaml")
+
+        if self.advanced.persistent_tmp_dir:
+            self.unipi_tmp_dir = Path("/var/tmp/unipi")
 
         self._validate_feature_object_ids()
         self._validate_covers_circuits()
         self._validate_cover_ids()
 
     def _validate_feature_object_ids(self) -> None:
         object_ids: List[str] = []
@@ -484,61 +492,61 @@
                 raise ConfigError(msg)
 
             object_ids.append(cover.object_id)
 
 
 @dataclass
 class HardwareInfo:
-    sys_bus: Path
+    sys_bus_dir: Path
     name: str = field(default="unknown")
     model: str = field(default="unknown", init=False)
     version: str = field(default="unknown", init=False)
     serial: str = field(default="unknown", init=False)
 
     def __post_init__(self) -> None:  # pragma: no cover
         # Can't unit testing the hardware info.
         # This code only works on the real hardware!
-        unipi_1: Path = self.sys_bus / "1-0050/eeprom"
-        unipi_patron: Path = self.sys_bus / "2-0057/eeprom"
-        unipi_neuron_1: Path = self.sys_bus / "1-0057/eeprom"
-        unipi_neuron_0: Path = self.sys_bus / "0-0057/eeprom"
+        unipi_1_file: Path = self.sys_bus_dir / "1-0050/eeprom"
+        unipi_patron_file: Path = self.sys_bus_dir / "2-0057/eeprom"
+        unipi_neuron_1_file: Path = self.sys_bus_dir / "1-0057/eeprom"
+        unipi_neuron_0_file: Path = self.sys_bus_dir / "0-0057/eeprom"
 
-        if unipi_1.is_file():
-            with unipi_1.open("rb") as _file:
+        if unipi_1_file.is_file():
+            with unipi_1_file.open("rb") as _file:
                 ee_bytes = _file.read(256)
 
                 if ee_bytes[226] == 1 and ee_bytes[227] == 1:
                     self.name = "Unipi"
                     self.version = "1.1"
                 elif ee_bytes[226] == 11 and ee_bytes[227] == 1:
                     self.name = "Unipi Lite"
                     self.version = "1.1"
                 else:
                     self.name = "Unipi"
                     self.version = "1.0"
 
                 self.serial = struct.unpack("i", ee_bytes[228:232])[0]
-        elif unipi_patron.is_file():
-            with unipi_patron.open("rb") as _file:
+        elif unipi_patron_file.is_file():
+            with unipi_patron_file.open("rb") as _file:
                 ee_bytes = _file.read(128)
 
                 self.name = "Unipi Patron"
                 self.model = f"{ee_bytes[106:110].decode()}"
                 self.version = f"{ee_bytes[99]}.{ee_bytes[98]}"
                 self.serial = struct.unpack("i", ee_bytes[100:104])[0]
-        elif unipi_neuron_1.is_file():
-            with unipi_neuron_1.open("rb") as _file:
+        elif unipi_neuron_1_file.is_file():
+            with unipi_neuron_1_file.open("rb") as _file:
                 ee_bytes = _file.read(128)
 
                 self.name = "Unipi Neuron"
                 self.model = f"{ee_bytes[106:110].decode()}"
                 self.version = f"{ee_bytes[99]}.{ee_bytes[98]}"
                 self.serial = struct.unpack("i", ee_bytes[100:104])[0]
-        elif unipi_neuron_0.is_file():
-            with unipi_neuron_0.open("rb") as _file:
+        elif unipi_neuron_0_file.is_file():
+            with unipi_neuron_0_file.open("rb") as _file:
                 ee_bytes = _file.read(128)
 
                 self.name = "Unipi Neuron"
                 self.model = f"{ee_bytes[106:110].decode()}"
                 self.version = f"{ee_bytes[99]}.{ee_bytes[98]}"
                 self.serial = struct.unpack("i", ee_bytes[100:104])[0]
 
@@ -549,15 +557,15 @@
 
 
 class HardwareMap(Mapping[str, HardwareDefinition]):
     def __init__(self, config: Config) -> None:
         self.config = config
 
         self.data: Dict[str, HardwareDefinition] = {}
-        self.info: HardwareInfo = HardwareInfo(sys_bus=config.sys_bus)
+        self.info: HardwareInfo = HardwareInfo(sys_bus_dir=config.sys_bus_dir)
 
         if self.info.model == "unknown":
             msg = "Hardware is not supported!"
             raise ConfigError(msg)
 
         self._read_neuron_definition()
         self._read_extension_definitions()
@@ -569,15 +577,15 @@
     def __iter__(self) -> Iterator[str]:
         return iter(self.data)
 
     def __len__(self) -> int:
         return len(self.data)
 
     def _read_neuron_definition(self) -> None:
-        definition_file: Path = Path(f"{self.config.hardware_path}/neuron/{self.info.model}.yaml")
+        definition_file: Path = Path(f"{self.config.hardware_dir}/neuron/{self.info.model}.yaml")
 
         if definition_file.is_file():
             try:
                 yaml_content: Dict[str, Any] = yaml_loader_safe(definition_file)
 
                 self.data["neuron"] = HardwareDefinition(
                     unit=0,
@@ -600,15 +608,15 @@
                 msg = f"{LogPrefix.CONFIG} Definition is invalid: {definition_file}\n{error}"
                 raise ConfigError(msg) from error
         else:
             msg = "No valid YAML definition found for this device!"
             raise ConfigError(msg)
 
     def _read_extension_definitions(self) -> None:
-        for definition_file in Path(f"{self.config.hardware_path}/extensions").glob("*.yaml"):
+        for definition_file in Path(f"{self.config.hardware_dir}/extensions").glob("*.yaml"):
             try:
                 yaml_content: Dict[str, Any] = yaml_loader_safe(definition_file)
 
                 units: Iterator[ModbusUnitConfig] = self.config.modbus.get_units_by_identifier(
                     identifier=definition_file.stem
                 )
 
@@ -621,15 +629,15 @@
                         manufacturer=yaml_content["manufacturer"],
                         model=yaml_content["model"],
                         modbus_register_blocks=yaml_content["modbus_register_blocks"],
                         modbus_features=yaml_content["modbus_features"],
                     )
 
                 UNIPI_LOGGER.debug("%s Definition loaded: %s", LogPrefix.CONFIG, definition_file)
-            except KeyError as error:
+            except KeyError as error:  # ruff: noqa: PERF203
                 msg = f"{LogPrefix.CONFIG} Definition is invalid: {definition_file}\nKeyError: {error}"
                 raise ConfigError(msg) from error
             except TypeError as error:
                 msg = f"{LogPrefix.CONFIG} Definition is invalid: {definition_file}"
                 raise ConfigError(msg) from error
             except YamlError as error:
                 msg = f"{LogPrefix.CONFIG} Definition is invalid: {definition_file}\n{error}"
```

### Comparing `unipi-control-2.0.0/unipi_control/extensions/eastron.py` & `unipi-control-2.1.0/unipi_control/extensions/eastron.py`

 * *Files identical despite different names*

### Comparing `unipi-control-2.0.0/unipi_control/features/extensions.py` & `unipi-control-2.1.0/unipi_control/features/extensions.py`

 * *Files identical despite different names*

### Comparing `unipi-control-2.0.0/unipi_control/features/map.py` & `unipi-control-2.1.0/unipi_control/features/map.py`

 * *Files identical despite different names*

### Comparing `unipi-control-2.0.0/unipi_control/features/neuron.py` & `unipi-control-2.1.0/unipi_control/features/neuron.py`

 * *Files identical despite different names*

### Comparing `unipi-control-2.0.0/unipi_control/features/utils.py` & `unipi-control-2.1.0/unipi_control/features/utils.py`

 * *Files identical despite different names*

### Comparing `unipi-control-2.0.0/unipi_control/helpers/argparse.py` & `unipi-control-2.1.0/unipi_control/helpers/argparse.py`

 * *Files identical despite different names*

### Comparing `unipi-control-2.0.0/unipi_control/helpers/log.py` & `unipi-control-2.1.0/unipi_control/helpers/log.py`

 * *Files identical despite different names*

### Comparing `unipi-control-2.0.0/unipi_control/helpers/text.py` & `unipi-control-2.1.0/unipi_control/helpers/text.py`

 * *Files identical despite different names*

### Comparing `unipi-control-2.0.0/unipi_control/helpers/typing.py` & `unipi-control-2.1.0/unipi_control/helpers/typing.py`

 * *Files identical despite different names*

### Comparing `unipi-control-2.0.0/unipi_control/helpers/yaml.py` & `unipi-control-2.1.0/unipi_control/helpers/yaml.py`

 * *Files identical despite different names*

### Comparing `unipi-control-2.0.0/unipi_control/integrations/covers.py` & `unipi-control-2.1.0/unipi_control/integrations/covers.py`

 * *Files 1% similar despite different names*

```diff
@@ -247,15 +247,15 @@
         """Path to temporary cover file.
 
         Returns
         -------
         Path:
             Path to temporary cover file.
         """
-        return self.config.temp_path / self.topic.replace("/", "__")
+        return self.config.unipi_tmp_dir / self.topic.replace("/", "__")
 
     @property
     def is_opening(self) -> bool:
         """Check if cover is opening.
 
         Returns
         -------
```

### Comparing `unipi-control-2.0.0/unipi_control/modbus.py` & `unipi-control-2.1.0/unipi_control/modbus.py`

 * *Files 5% similar despite different names*

```diff
@@ -83,15 +83,15 @@
 
         if scan_type == "tcp":
             response = await check_modbus_call(self.modbus_client.tcp.read_input_registers, data)
         elif scan_type == "serial":
             response = await check_modbus_call(self.modbus_client.serial.read_input_registers, data)
 
         if response:
-            register = response.registers  # type: ignore[attr-defined]
+            register: List[int] = response.registers
             for index in range(data["count"]):
                 self.data[definition.unit][data["address"] + index] = register[index]
 
     async def scan(self, scan_type: str, hardware_types: List[str]) -> None:
         """Read modbus register blocks and cache the response."""
         for definition in self.hardware.get_definition_by_hardware_types(hardware_types):
             if not self.data.get(definition.unit):
```

### Comparing `unipi-control-2.0.0/unipi_control/mqtt/discovery/binary_sensors.py` & `unipi-control-2.1.0/unipi_control/mqtt/discovery/binary_sensors.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from asyncio import Task
 from typing import Any, ClassVar
 from typing import Dict
 from typing import List
 from typing import Set
 from typing import Tuple
 
-from asyncio_mqtt import Client
+from aiomqtt import Client
 
 from unipi_control.config import UNIPI_LOGGER
 from unipi_control.features.neuron import DigitalInput
 from unipi_control.features.utils import FeatureState
 from unipi_control.helpers.log import LOG_MQTT_PUBLISH
 from unipi_control.mqtt.discovery.mixin import HassDiscoveryMixin
 from unipi_control.neuron import Neuron
```

### Comparing `unipi-control-2.0.0/unipi_control/mqtt/discovery/covers.py` & `unipi-control-2.1.0/unipi_control/mqtt/discovery/covers.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from asyncio import Task
 from typing import Any
 from typing import Dict
 from typing import Optional
 from typing import Set
 from typing import Tuple
 
-from asyncio_mqtt import Client
+from aiomqtt import Client
 
 from unipi_control.config import Config
 from unipi_control.config import DEVICE_CLASSES
 from unipi_control.config import HardwareMap
 from unipi_control.config import UNIPI_LOGGER
 from unipi_control.helpers.log import LOG_MQTT_PUBLISH
 from unipi_control.integrations.covers import Cover
```

### Comparing `unipi-control-2.0.0/unipi_control/mqtt/discovery/mixin.py` & `unipi-control-2.1.0/unipi_control/mqtt/discovery/mixin.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Helpers for MQTT subscribe and publish."""
 
 from typing import Optional, TYPE_CHECKING
 from typing import Union
 
-from asyncio_mqtt import Client
+from aiomqtt import Client
 
 from unipi_control.features.extensions import EastronMeter
 from unipi_control.features.neuron import NeuronFeature
 from unipi_control.neuron import Neuron
 
 if TYPE_CHECKING:
     from unipi_control.config import Config
```

### Comparing `unipi-control-2.0.0/unipi_control/mqtt/discovery/sensors.py` & `unipi-control-2.1.0/unipi_control/mqtt/discovery/sensors.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from typing import Any, ClassVar
 from typing import Dict
 from typing import List
 from typing import Set
 from typing import Tuple
 from typing import Union
 
-from asyncio_mqtt import Client
+from aiomqtt import Client
 
 from unipi_control.config import UNIPI_LOGGER
 from unipi_control.features.extensions import EastronMeter
 from unipi_control.helpers.log import LOG_MQTT_PUBLISH
 from unipi_control.mqtt.discovery.mixin import HassDiscoveryMixin
 from unipi_control.neuron import Neuron
```

### Comparing `unipi-control-2.0.0/unipi_control/mqtt/discovery/switches.py` & `unipi-control-2.1.0/unipi_control/mqtt/discovery/switches.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from typing import Any, ClassVar
 from typing import Dict
 from typing import List
 from typing import Set
 from typing import Tuple
 from typing import Union
 
-from asyncio_mqtt import Client
+from aiomqtt import Client
 
 from unipi_control.config import UNIPI_LOGGER
 from unipi_control.features.neuron import DigitalOutput
 from unipi_control.features.neuron import Relay
 from unipi_control.features.utils import FeatureState
 from unipi_control.helpers.log import LOG_MQTT_PUBLISH
 from unipi_control.mqtt.discovery.mixin import HassDiscoveryMixin
```

### Comparing `unipi-control-2.0.0/unipi_control/mqtt/features.py` & `unipi-control-2.1.0/unipi_control/mqtt/features.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from contextlib import AsyncExitStack
 from typing import Any, ClassVar
 from typing import AsyncIterable
 from typing import List
 from typing import Set
 from typing import Union
 
-from asyncio_mqtt import Client
+from aiomqtt import Client
 
 from unipi_control.config import HardwareType
 from unipi_control.config import UNIPI_LOGGER
 from unipi_control.features.neuron import DigitalOutput
 from unipi_control.features.neuron import Relay
 from unipi_control.helpers.log import LOG_MQTT_PUBLISH
 from unipi_control.helpers.log import LOG_MQTT_SUBSCRIBE
```

### Comparing `unipi-control-2.0.0/unipi_control/mqtt/integrations/covers.py` & `unipi-control-2.1.0/unipi_control/mqtt/integrations/covers.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from typing import Dict
 from typing import List
 from typing import NamedTuple
 from typing import Optional
 from typing import Set
 from typing import Union
 
-from asyncio_mqtt import Client
+from aiomqtt import Client
 
 from unipi_control.config import DEVICE_CLASSES
 from unipi_control.config import LogPrefix
 from unipi_control.config import UNIPI_LOGGER
 from unipi_control.helpers.log import LOG_MQTT_PUBLISH
 from unipi_control.helpers.log import LOG_MQTT_SUBSCRIBE
 from unipi_control.helpers.log import LOG_MQTT_SUBSCRIBE_TOPIC
```

### Comparing `unipi-control-2.0.0/unipi_control/neuron.py` & `unipi-control-2.1.0/unipi_control/neuron.py`

 * *Files identical despite different names*

### Comparing `unipi-control-2.0.0/unipi_control/tools/config_backup.py` & `unipi-control-2.1.0/unipi_control/tools/config_backup.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,46 +8,46 @@
 from datetime import timezone
 from pathlib import Path
 from typing import List
 from typing import Optional
 
 from unipi_control import __version__  # type: ignore[attr-defined]
 from unipi_control.config import Config
-from unipi_control.config import DEFAULT_CONFIG_PATH
+from unipi_control.config import DEFAULT_CONFIG_DIR
 from unipi_control.config import LoggingConfig
 from unipi_control.config import UNIPI_LOGGER
 from unipi_control.helpers.argparse import init_argparse
 from unipi_control.helpers.exception import UnexpectedError
 from unipi_control.helpers.log import SIMPLE_LOG_FORMAT
 
 
 class UnipiConfigBackup:
     def __init__(self, config: Config) -> None:
         self.config: Config = config
 
-    def backup(self, target: Path) -> None:
+    def backup(self, target_dir: Path) -> None:
         """Backup configuration file."""
         exception_message: Optional[str] = None
 
-        if target.is_file():
+        if target_dir.is_file():
             exception_message = "OUTPUT is a file not a directory!"
-        elif not target.is_dir():
+        elif not target_dir.is_dir():
             exception_message = "OUTPUT directory not exists!"
 
         if exception_message:
             raise UnexpectedError(exception_message)
 
         datetime_now = datetime.now(tz=timezone.utc)
         tar_filename: str = f"config-{datetime_now.date()}-{datetime_now.strftime('%H%M%S')}.tar.gz"
-        tar_file: Path = target / tar_filename
+        tar_file: Path = target_dir / tar_filename
         tar_file.unlink(missing_ok=True)
 
         try:
             with tarfile.open(tar_file, "x:gz") as tar:
-                tar.add(self.config.config_base_path / "control.yaml", arcname=self.config.config_base_path)
+                tar.add(self.config.config_base_dir / "control.yaml", arcname=self.config.config_base_dir)
         except OSError as error:
             exception_message = f"{error.strerror}: '{error.filename}'"
             raise UnexpectedError(exception_message) from error
 
         UNIPI_LOGGER.info("%s created!", tar_file.as_posix())
 
 
@@ -65,32 +65,32 @@
     """
     parser: argparse.ArgumentParser = init_argparse(description="Backup Unipi Control configuration")
     parser.add_argument("output", help="path to save the backup file")
     parser.add_argument(
         "-c",
         "--config",
         action="store",
-        default=DEFAULT_CONFIG_PATH,
-        help=f"path to the configuration (default: {DEFAULT_CONFIG_PATH})",
+        default=DEFAULT_CONFIG_DIR,
+        help=f"path to the configuration (default: {DEFAULT_CONFIG_DIR})",
     )
     parser.add_argument("--version", action="version", version=f"%(prog)s {__version__}")
 
     return parser.parse_args(args)
 
 
 def main(argv: Optional[List[str]] = None) -> None:
     """Entrypoint for Unipi Config Converter."""
     if argv is None:
         argv = sys.argv[1:]
 
     try:
         args: argparse.Namespace = parse_args(argv)
 
-        config: Config = Config(logging=LoggingConfig(level="info"), config_base_path=Path(args.config))
+        config: Config = Config(logging=LoggingConfig(level="info"), config_base_dir=Path(args.config))
         config.logging.init(log=args.log, verbose=args.verbose, fmt=SIMPLE_LOG_FORMAT)
 
-        UnipiConfigBackup(config=config).backup(target=Path(args.output))
+        UnipiConfigBackup(config=config).backup(target_dir=Path(args.output))
     except UnexpectedError as error:
         UNIPI_LOGGER.critical(error)
         sys.exit(1)
     except KeyboardInterrupt:
         ...
```

### Comparing `unipi-control-2.0.0/unipi_control/tools/config_converter.py` & `unipi-control-2.1.0/unipi_control/tools/config_converter.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,16 +27,16 @@
 
 
 class UnipiConfigConverter:
     def __init__(self, force: bool) -> None:
         self.force: bool = force
 
     @staticmethod
-    def _read_source_yaml(source: Path) -> Dict[str, Any]:
-        source_yaml: Dict[str, Any] = yaml_loader_safe(source)
+    def _read_source_yaml(source_file: Path) -> Dict[str, Any]:
+        source_yaml: Dict[str, Any] = yaml_loader_safe(source_file)
 
         if isinstance(source_yaml, dict):
             return source_yaml
 
         exception_message: str = "INPUT is not a valid YAML file!"
         raise UnexpectedError(exception_message)
```

### Comparing `unipi-control-2.0.0/unipi_control/tools/model_info.py` & `unipi-control-2.1.0/unipi_control/tools/model_info.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,58 +1,59 @@
+#!/usr/bin/env python3
 """Read model informations from /sys path."""
 
 import struct
 from pathlib import Path
 
 
 def main() -> None:
     """Tiny script to detect the Unipi Neuron model."""
-    unipi_1: Path = Path("/sys/bus/i2c/devices/1-0050/eeprom")
-    unipi_patron: Path = Path("/sys/bus/i2c/devices/2-0057/eeprom")
-    unipi_neuron_1: Path = Path("/sys/bus/i2c/devices/1-0057/eeprom")
-    unipi_neuron_0: Path = Path("/sys/bus/i2c/devices/0-0057/eeprom")
+    unipi_1_file: Path = Path("/sys/bus/i2c/devices/1-0050/eeprom")
+    unipi_patron_file: Path = Path("/sys/bus/i2c/devices/2-0057/eeprom")
+    unipi_neuron_1_file: Path = Path("/sys/bus/i2c/devices/1-0057/eeprom")
+    unipi_neuron_0_file: Path = Path("/sys/bus/i2c/devices/0-0057/eeprom")
 
     name: str = "unknown"
     model: str = "unknown"
     version: str = "unknown"
     serial: str = "unknown"
 
-    if unipi_1.is_file():
-        with unipi_1.open("rb") as _file:
+    if unipi_1_file.is_file():
+        with unipi_1_file.open("rb") as _file:
             ee_bytes = _file.read(256)
 
             if ee_bytes[226] == 1 and ee_bytes[227] == 1:
                 name = "Unipi"
                 version = "1.1"
             elif ee_bytes[226] == 11 and ee_bytes[227] == 1:
                 name = "Unipi Lite"
                 version = "1.1"
             else:
                 name = "Unipi"
                 version = "1.0"
 
             serial = struct.unpack("i", ee_bytes[228:232])[0]
-    elif unipi_neuron_1.is_file():
-        with unipi_neuron_1.open("rb") as _file:
+    elif unipi_neuron_1_file.is_file():
+        with unipi_neuron_1_file.open("rb") as _file:
             ee_bytes = _file.read(128)
 
             name = "Unipi Neuron"
             model = f"{ee_bytes[106:110].decode()}"
             version = f"{ee_bytes[99]}.{ee_bytes[98]}"
             serial = struct.unpack("i", ee_bytes[100:104])[0]
-    elif unipi_patron.is_file():
-        with unipi_patron.open("rb") as _file:
+    elif unipi_patron_file.is_file():
+        with unipi_patron_file.open("rb") as _file:
             ee_bytes = _file.read(128)
 
             name = "Unipi Patron"
             model = f"{ee_bytes[106:110].decode()}"
             version = f"{ee_bytes[99]}.{ee_bytes[98]}"
             serial = struct.unpack("i", ee_bytes[100:104])[0]
-    elif unipi_neuron_0.is_file():
-        with unipi_neuron_0.open("rb") as _file:
+    elif unipi_neuron_0_file.is_file():
+        with unipi_neuron_0_file.open("rb") as _file:
             ee_bytes = _file.read(128)
 
             name = "Unipi Neuron"
             model = f"{ee_bytes[106:110].decode()}"
             version = f"{ee_bytes[99]}.{ee_bytes[98]}"
             serial = struct.unpack("i", ee_bytes[100:104])[0]
```

### Comparing `unipi-control-2.0.0/unipi_control/unipi_control.py` & `unipi-control-2.1.0/unipi_control/unipi_control.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,21 +10,21 @@
 from typing import Awaitable
 from typing import Callable
 from typing import List
 from typing import NoReturn
 from typing import Optional
 from typing import Set
 
-from asyncio_mqtt import Client
-from asyncio_mqtt import MqttError
+from aiomqtt import Client
+from aiomqtt import MqttError
 from pymodbus.client.serial import AsyncModbusSerialClient
 from pymodbus.client.tcp import AsyncModbusTcpClient
 
 from unipi_control.config import Config
-from unipi_control.config import DEFAULT_CONFIG_PATH
+from unipi_control.config import DEFAULT_CONFIG_DIR
 from unipi_control.config import LogPrefix
 from unipi_control.config import MqttConfig
 from unipi_control.config import UNIPI_LOGGER
 from unipi_control.helpers.argparse import init_argparse
 from unipi_control.helpers.exception import ConfigError
 from unipi_control.helpers.exception import UnexpectedError
 from unipi_control.helpers.text import slugify
@@ -73,23 +73,23 @@
             await HassSensorsMqttPlugin(self.neuron, mqtt_client).init_tasks(tasks)
             await HassSwitchesMqttPlugin(self.neuron, mqtt_client).init_tasks(tasks)
 
         await asyncio.gather(*tasks)
 
     @staticmethod
     async def _cancel_tasks(tasks: Set[Task]) -> None:
-        for task in tasks:
-            if task.done():
-                continue
+        try:
+            for task in tasks:
+                if task.done():
+                    continue
 
-            try:
                 task.cancel()
                 await task
-            except asyncio.CancelledError:
-                ...
+        except asyncio.CancelledError:
+            ...
 
     async def _modbus_connect(self) -> None:
         await self.modbus_client.tcp.connect()  # type: ignore[no-untyped-call]
 
         if self.modbus_client.tcp.connected:
             UNIPI_LOGGER.info(
                 "%s TCP client connected to %s:%s",
@@ -157,15 +157,15 @@
                     retry_reconnect = 0
 
                     UNIPI_LOGGER.info(
                         "%s Connected to broker at '%s:%s'", LogPrefix.MQTT, mqtt_config.host, mqtt_config.port
                     )
 
                     await callback(stack, mqtt_client)
-            except MqttError as error:
+            except MqttError as error:  # ruff: noqa: PERF203
                 UNIPI_LOGGER.error(
                     "%s Error '%s'. Connecting attempt #%s. Reconnecting in %s seconds.",
                     LogPrefix.MQTT,
                     error,
                     retry_reconnect + 1,
                     reconnect_interval,
                 )
@@ -202,17 +202,18 @@
     Argparse namespace
     """
     parser: argparse.ArgumentParser = init_argparse(description="Control Unipi I/O with MQTT commands")
     parser.add_argument(
         "-c",
         "--config",
         action="store",
-        default=DEFAULT_CONFIG_PATH,
-        help=f"path to the configuration (default: {DEFAULT_CONFIG_PATH})",
+        default=DEFAULT_CONFIG_DIR,
+        help=f"path to the configuration (default: {DEFAULT_CONFIG_DIR})",
     )
+
     parser.add_argument("--version", action="version", version=f"%(prog)s {__version__}")
 
     return parser.parse_args(args)
 
 
 def main(argv: Optional[List[str]] = None) -> None:
     """Entrypoint for Unipi Control."""
@@ -220,15 +221,15 @@
         argv = sys.argv[1:]
 
     unipi_control: Optional[UnipiControl] = None
 
     try:
         args: argparse.Namespace = parse_args(argv)
 
-        config: Config = Config(config_base_path=Path(args.config))
+        config: Config = Config(config_base_dir=Path(args.config))
         config.logging.init(log=args.log, verbose=args.verbose)
 
         unipi_control = UnipiControl(
             config=config,
             modbus_client=ModbusClient(
                 tcp=AsyncModbusTcpClient(
                     host="localhost",
```

### Comparing `unipi-control-2.0.0/unipi_control.egg-info/PKG-INFO` & `unipi-control-2.1.0/unipi_control.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unipi-control
-Version: 2.0.0
+Version: 2.1.0
 Summary: Control Unipi I/O directly with MQTT commands.
 Author-email: Michael Hacker <mh@superbox.one>
 Maintainer-email: Michael Hacker <mh@superbox.one>
 License: Apache-2.0 license
 Project-URL: Source code, https://github.com/superbox-dev/unipi-control
 Project-URL: Issue tracker, https://github.com/superbox-dev/unipi-control/issues
 Keywords: mqtt,modbus,unipi
@@ -24,27 +24,41 @@
 Provides-Extra: build
 Provides-Extra: audit
 Provides-Extra: format
 Provides-Extra: lint
 Provides-Extra: tests
 License-File: LICENSE
 
-[![license-url](https://img.shields.io/badge/license-Apache%202-yellowgreen)](https://opensource.org/license/apache-2-0/)
 ![coverage-badge](https://raw.githubusercontent.com/superbox-dev/unipi-control/main/coverage.svg)
+[![CI](https://github.com/superbox-dev/unipi-control/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/superbox-dev/unipi-control/actions/workflows/ci.yml)
 ![Python 3.8](https://img.shields.io/badge/python-3.8-blue.svg)
 ![Python 3.9](https://img.shields.io/badge/python-3.9-blue.svg)
 ![Python 3.10](https://img.shields.io/badge/python-3.10-blue.svg)
 ![Python 3.11](https://img.shields.io/badge/python-3.11-blue.svg)
+![Python 3.11](https://img.shields.io/badge/python-3.11-blue.svg)
+
+[![license-url](https://img.shields.io/badge/license-Apache%202-yellowgreen)](https://opensource.org/license/apache-2-0/)
+![PyPi downloads](https://img.shields.io/pypi/dm/unipi-control)
+![Typing: strict](https://img.shields.io/badge/typing-strict-green.svg)
+![Code style: black](https://img.shields.io/badge/code%20style-black-black)
+![Code style: Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)
 
 <!-- pitch start -->
 # Unipi Control
 
 Unipi Control use Modbus for fast access to the I/O and provide MQTT topics for reading and writing the circuits. Optionally you can enable the Home Assistant MQTT discovery for binary sensors, sensors, switches and covers.
 <!-- pitch end -->
 
+---
+
+For more information please read the documentation at:
+[docs.superbox.one](https://docs.superbox.one)
+
+---
+
 <!-- quickstart start -->
 ## Getting started
 
 ### Recommended installation (only for Unipi Neuron)
 
 We have a ready to use SD card image called [Unipi Control OS](https://github.com/superbox-dev/unipi-control-os).
 
@@ -69,15 +83,15 @@
 
 Install `unipi-control` with pip:
 
 ```bash
 pip install unipi-control
 ```
 
-Copy the [config files](data/opkg/data/local/etc/unipi) to `/etc/unipi` and configurate the `/etc/unipi/control.yaml`.
+Copy the [config files](https://github.com/superbox-dev/unipi-control/data/opkg/data/local/etc/unipi) to `/etc/unipi` and configurate the `/etc/unipi/control.yaml`.
 
 Create the systemd service `/etc/systemd/system/unipi-control.service` with following content:
 
 ```ini
 [Unit]
 Description=Unipi Control
 After=multi-user.target
@@ -94,15 +108,15 @@
 Enable and start the systemd service:
 
 ```bash
 systemctl --system daemon-reload
 systemctl enable unipi-control.service
 systemctl start unipi-control.service
 ```
-<!-- quickstart start -->
+<!-- quickstart end -->
 
 ## Changelog
 
 The changelog lives in the [CHANGELOG.md](CHANGELOG.md) document. The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/).
 
 ## Contributing
```

### Comparing `unipi-control-2.0.0/unipi_control.egg-info/SOURCES.txt` & `unipi-control-2.1.0/unipi_control.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 .yamllint.yml
 CHANGELOG.md
 CONTRIBUTING.md
 LICENSE
 README.md
 coverage.svg
 pyproject.toml
+.github/dependabot.yml
 .github/workflows/ci.yml
 .github/workflows/parameters.json
 data/Dockerfile
 data/extras/homeassistant/blueprints/automation/cover/control.yaml
 data/extras/homeassistant/blueprints/automation/cover/simple_cover_control.yaml
 data/opkg/control/control
 data/opkg/control/postinst
```

