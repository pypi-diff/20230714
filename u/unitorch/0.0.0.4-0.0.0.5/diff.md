# Comparing `tmp/unitorch-0.0.0.4.tar.gz` & `tmp/unitorch-0.0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unitorch-0.0.0.4.tar", last modified: Tue Jul  4 07:55:37 2023, max compression
+gzip compressed data, was "unitorch-0.0.0.5.tar", last modified: Fri Jul 14 20:43:03 2023, max compression
```

## Comparing `unitorch-0.0.0.4.tar` & `unitorch-0.0.0.5.tar`

### file list

```diff
@@ -1,471 +1,491 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.693682 unitorch-0.0.0.4/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.569682 unitorch-0.0.0.4/.pytest_cache/
--rw-r--r--   0 root         (0) root         (0)      302 2023-07-04 07:55:29.000000 unitorch-0.0.0.4/.pytest_cache/README.md
--rw-r--r--   0 root         (0) root         (0)     1085 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)      131 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     8991 2023-07-04 07:55:37.693682 unitorch-0.0.0.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7956 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.569682 unitorch-0.0.0.4/benchmarks/
--rw-r--r--   0 root         (0) root         (0)       87 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/benchmarks/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.553682 unitorch-0.0.0.4/docs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.569682 unitorch-0.0.0.4/docs/search/
--rw-r--r--   0 root         (0) root         (0)  1019279 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/docs/search/search_index.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.573682 unitorch-0.0.0.4/examples/
--rw-r--r--   0 root         (0) root         (0)     2311 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/examples/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.557682 unitorch-0.0.0.4/examples/configs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.573682 unitorch-0.0.0.4/examples/configs/caption/
--rw-r--r--   0 root         (0) root         (0)     1788 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/examples/configs/caption/blip.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.577682 unitorch-0.0.0.4/examples/configs/classification/
--rw-r--r--   0 root         (0) root         (0)     1545 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/examples/configs/classification/bert.ini
--rw-r--r--   0 root         (0) root         (0)     1700 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/examples/configs/classification/clip.ini
--rw-r--r--   0 root         (0) root         (0)     1688 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/examples/configs/classification/image_clip.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.577682 unitorch-0.0.0.4/examples/configs/classification/lora/
--rw-r--r--   0 root         (0) root         (0)     1639 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/examples/configs/classification/lora/bloom.ini
--rw-r--r--   0 root         (0) root         (0)     1588 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/examples/configs/classification/lora/bloom_ds.ini
--rw-r--r--   0 root         (0) root         (0)     1857 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/examples/configs/classification/lora/llama.ini
--rw-r--r--   0 root         (0) root         (0)     1806 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/examples/configs/classification/lora/llama_ds.ini
--rw-r--r--   0 root         (0) root         (0)     1556 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/examples/configs/classification/roberta.ini
--rw-r--r--   0 root         (0) root         (0)     1673 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/examples/configs/classification/swin.ini
--rw-r--r--   0 root         (0) root         (0)     1636 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/examples/configs/classification/text_clip.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.577682 unitorch-0.0.0.4/examples/configs/diffusion/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.577682 unitorch-0.0.0.4/examples/configs/diffusion/controlnet/
--rw-r--r--   0 root         (0) root         (0)     1925 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/examples/configs/diffusion/controlnet/canny.ini
--rw-r--r--   0 root         (0) root         (0)     1751 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/examples/configs/diffusion/stable-v1.5.ini
--rw-r--r--   0 root         (0) root         (0)     1751 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/examples/configs/diffusion/stable-v2.1.ini
--rw-r--r--   0 root         (0) root         (0)     1747 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/examples/configs/diffusion/stable-v2.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.581682 unitorch-0.0.0.4/examples/configs/generation/
--rw-r--r--   0 root         (0) root         (0)     1607 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/examples/configs/generation/bart.ini
--rw-r--r--   0 root         (0) root         (0)     1650 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/examples/configs/generation/bloom.ini
--rw-r--r--   0 root         (0) root         (0)     1666 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/examples/configs/generation/chatglm.ini
--rw-r--r--   0 root         (0) root         (0)     1646 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/examples/configs/generation/llama.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.581682 unitorch-0.0.0.4/examples/configs/generation/lora/
--rw-r--r--   0 root         (0) root         (0)     1589 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/examples/configs/generation/lora/bloom.ini
--rw-r--r--   0 root         (0) root         (0)     1537 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/examples/configs/generation/lora/bloom_ds.ini
--rw-r--r--   0 root         (0) root         (0)     1585 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/examples/configs/generation/lora/llama.ini
--rw-r--r--   0 root         (0) root         (0)     1533 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/examples/configs/generation/lora/llama_ds.ini
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/examples/configs/generation/mbart.ini
--rw-r--r--   0 root         (0) root         (0)     1597 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/examples/configs/generation/mt5.ini
--rw-r--r--   0 root         (0) root         (0)     1655 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/examples/configs/generation/pegasus.ini
--rw-r--r--   0 root         (0) root         (0)     1587 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/examples/configs/generation/t5.ini
--rw-r--r--   0 root         (0) root         (0)     1647 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/examples/configs/generation/xpegasus.ini
--rw-r--r--   0 root         (0) root         (0)     1745 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/examples/configs/generation/xprophetnet.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.581682 unitorch-0.0.0.4/examples/configs/pretrain/
--rw-r--r--   0 root         (0) root         (0)     1266 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/examples/configs/pretrain/clip.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.557682 unitorch-0.0.0.4/examples/configs/services/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.585682 unitorch-0.0.0.4/examples/configs/services/zip_image/
--rw-r--r--   0 root         (0) root         (0)      148 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/examples/configs/services/zip_image/config.ini
--rw-r--r--   0 root         (0) root         (0)      240 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/examples/configs/services/zip_image/config_v2.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.557682 unitorch-0.0.0.4/examples/hub/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.585682 unitorch-0.0.0.4/examples/hub/caption/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/examples/hub/caption/blip.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.585682 unitorch-0.0.0.4/examples/hub/classification/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/examples/hub/classification/bert.ini
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/examples/hub/classification/clip.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.585682 unitorch-0.0.0.4/examples/hub/generation/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/examples/hub/generation/bart.ini
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/examples/hub/generation/llama.ini
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/examples/hub/generation/xpegasus.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.585682 unitorch-0.0.0.4/notebooks/
--rw-r--r--   0 root         (0) root         (0)      131 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/notebooks/README.md
--rw-r--r--   0 root         (0) root         (0)     1790 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      131 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-04 07:55:37.693682 unitorch-0.0.0.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1527 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.557682 unitorch-0.0.0.4/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.585682 unitorch-0.0.0.4/src/unitorch/
--rw-r--r--   0 root         (0) root         (0)     2670 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.589682 unitorch-0.0.0.4/src/unitorch/cli/
--rw-r--r--   0 root         (0) root         (0)     6024 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.589682 unitorch-0.0.0.4/src/unitorch/cli/console/
--rw-r--r--   0 root         (0) root         (0)       65 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/console/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2092 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/console/eval.py
--rw-r--r--   0 root         (0) root         (0)     2095 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/console/infer.py
--rw-r--r--   0 root         (0) root         (0)     2172 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/console/script.py
--rw-r--r--   0 root         (0) root         (0)     4683 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/console/service.py
--rw-r--r--   0 root         (0) root         (0)     2095 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/console/train.py
--rw-r--r--   0 root         (0) root         (0)     4397 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/core.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.589682 unitorch-0.0.0.4/src/unitorch/cli/datasets/
--rw-r--r--   0 root         (0) root         (0)       98 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/datasets/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12406 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/datasets/hf.py
--rw-r--r--   0 root         (0) root         (0)     2613 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/decorators.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.589682 unitorch-0.0.0.4/src/unitorch/cli/loss/
--rw-r--r--   0 root         (0) root         (0)     4063 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/loss/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2857 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/loss/ranking.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.597682 unitorch-0.0.0.4/src/unitorch/cli/models/
--rw-r--r--   0 root         (0) root         (0)     2865 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.597682 unitorch-0.0.0.4/src/unitorch/cli/models/bart/
--rw-r--r--   0 root         (0) root         (0)     1378 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/bart/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6981 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/bart/modeling.py
--rw-r--r--   0 root         (0) root         (0)     6140 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/bart/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.597682 unitorch-0.0.0.4/src/unitorch/cli/models/beit/
--rw-r--r--   0 root         (0) root         (0)     1390 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/beit/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3142 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/beit/modeling.py
--rw-r--r--   0 root         (0) root         (0)     2535 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/beit/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.597682 unitorch-0.0.0.4/src/unitorch/cli/models/bert/
--rw-r--r--   0 root         (0) root         (0)     1177 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/bert/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3903 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/bert/modeling.py
--rw-r--r--   0 root         (0) root         (0)     6128 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/bert/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.601682 unitorch-0.0.0.4/src/unitorch/cli/models/blip/
--rw-r--r--   0 root         (0) root         (0)     2196 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/blip/__init__.py
--rw-r--r--   0 root         (0) root         (0)    22703 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/blip/modeling.py
--rw-r--r--   0 root         (0) root         (0)     7788 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/blip/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.601682 unitorch-0.0.0.4/src/unitorch/cli/models/bloom/
--rw-r--r--   0 root         (0) root         (0)     2570 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/bloom/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13026 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/bloom/modeling.py
--rw-r--r--   0 root         (0) root         (0)     8321 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/bloom/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.601682 unitorch-0.0.0.4/src/unitorch/cli/models/chatglm/
--rw-r--r--   0 root         (0) root         (0)     1201 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/chatglm/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13764 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/chatglm/modeling.py
--rw-r--r--   0 root         (0) root         (0)     8833 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/chatglm/processing.py
--rw-r--r--   0 root         (0) root         (0)     9143 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/classification_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.605682 unitorch-0.0.0.4/src/unitorch/cli/models/clip/
--rw-r--r--   0 root         (0) root         (0)     2514 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/clip/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16125 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/clip/modeling.py
--rw-r--r--   0 root         (0) root         (0)     5565 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/clip/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.605682 unitorch-0.0.0.4/src/unitorch/cli/models/deberta/
--rw-r--r--   0 root         (0) root         (0)     4492 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/deberta/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4077 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/deberta/modeling.py
--rw-r--r--   0 root         (0) root         (0)     4021 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/deberta/modeling_v2.py
--rw-r--r--   0 root         (0) root         (0)     3801 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/deberta/processing.py
--rw-r--r--   0 root         (0) root         (0)     3434 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/deberta/processing_v2.py
--rw-r--r--   0 root         (0) root         (0)     2545 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/detection_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.609682 unitorch-0.0.0.4/src/unitorch/cli/models/diffusers/
--rw-r--r--   0 root         (0) root         (0)     2453 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/diffusers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7480 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/diffusers/modeling_controlnet.py
--rw-r--r--   0 root         (0) root         (0)     9444 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/diffusers/modeling_stable.py
--rw-r--r--   0 root         (0) root         (0)     3879 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/diffusers/processing_controlnet.py
--rw-r--r--   0 root         (0) root         (0)     3838 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/diffusers/processing_stable.py
--rw-r--r--   0 root         (0) root         (0)     3126 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/diffusion_utils.py
--rw-r--r--   0 root         (0) root         (0)     2961 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/generation_utils.py
--rw-r--r--   0 root         (0) root         (0)     5092 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/image_utils.py
--rw-r--r--   0 root         (0) root         (0)     4297 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/label_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.609682 unitorch-0.0.0.4/src/unitorch/cli/models/llama/
--rw-r--r--   0 root         (0) root         (0)     2253 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/llama/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14017 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/llama/modeling.py
--rw-r--r--   0 root         (0) root         (0)     8206 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/llama/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.609682 unitorch-0.0.0.4/src/unitorch/cli/models/mbart/
--rw-r--r--   0 root         (0) root         (0)      887 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/mbart/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7602 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/mbart/modeling.py
--rw-r--r--   0 root         (0) root         (0)     5826 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/mbart/processing.py
--rw-r--r--   0 root         (0) root         (0)    15281 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/modeling_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.609682 unitorch-0.0.0.4/src/unitorch/cli/models/mt5/
--rw-r--r--   0 root         (0) root         (0)     1381 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/mt5/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7125 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/mt5/modeling.py
--rw-r--r--   0 root         (0) root         (0)     5815 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/mt5/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.609682 unitorch-0.0.0.4/src/unitorch/cli/models/peft/
--rw-r--r--   0 root         (0) root         (0)      524 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/peft/__init__.py
--rw-r--r--   0 root         (0) root         (0)    30502 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/peft/modeling_bloom.py
--rw-r--r--   0 root         (0) root         (0)    30560 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/peft/modeling_llama.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.613682 unitorch-0.0.0.4/src/unitorch/cli/models/pegasus/
--rw-r--r--   0 root         (0) root         (0)     1213 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/pegasus/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7233 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/pegasus/modeling.py
--rw-r--r--   0 root         (0) root         (0)     5885 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/pegasus/processing.py
--rw-r--r--   0 root         (0) root         (0)     2834 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/processing_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.613682 unitorch-0.0.0.4/src/unitorch/cli/models/prophetnet/
--rw-r--r--   0 root         (0) root         (0)      162 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/prophetnet/__init__.py
--rw-r--r--   0 root         (0) root         (0)       65 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/prophetnet/modeling.py
--rw-r--r--   0 root         (0) root         (0)       65 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/prophetnet/processing.py
--rw-r--r--   0 root         (0) root         (0)      650 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/random_utils.py
--rw-r--r--   0 root         (0) root         (0)      535 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/ranking_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.613682 unitorch-0.0.0.4/src/unitorch/cli/models/roberta/
--rw-r--r--   0 root         (0) root         (0)     1347 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/roberta/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3967 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/roberta/modeling.py
--rw-r--r--   0 root         (0) root         (0)     3766 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/roberta/processing.py
--rw-r--r--   0 root         (0) root         (0)     2462 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/segmentation_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.617682 unitorch-0.0.0.4/src/unitorch/cli/models/swin/
--rw-r--r--   0 root         (0) root         (0)     3032 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/swin/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3225 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/swin/modeling.py
--rw-r--r--   0 root         (0) root         (0)     2564 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/swin/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.617682 unitorch-0.0.0.4/src/unitorch/cli/models/t5/
--rw-r--r--   0 root         (0) root         (0)     1282 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/t5/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7144 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/t5/modeling.py
--rw-r--r--   0 root         (0) root         (0)     5811 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/t5/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.617682 unitorch-0.0.0.4/src/unitorch/cli/models/visualbert/
--rw-r--r--   0 root         (0) root         (0)     1310 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/visualbert/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8538 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/visualbert/modeling.py
--rw-r--r--   0 root         (0) root         (0)     6306 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/visualbert/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.617682 unitorch-0.0.0.4/src/unitorch/cli/models/vit/
--rw-r--r--   0 root         (0) root         (0)     4602 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/vit/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3191 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/vit/modeling.py
--rw-r--r--   0 root         (0) root         (0)     2583 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/vit/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.621682 unitorch-0.0.0.4/src/unitorch/cli/models/xlm_roberta/
--rw-r--r--   0 root         (0) root         (0)     2314 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/xlm_roberta/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7533 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/xlm_roberta/modeling.py
--rw-r--r--   0 root         (0) root         (0)     3408 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/xlm_roberta/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.621682 unitorch-0.0.0.4/src/unitorch/cli/models/xpegasus/
--rw-r--r--   0 root         (0) root         (0)     1189 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/xpegasus/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7237 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/xpegasus/modeling.py
--rw-r--r--   0 root         (0) root         (0)     5953 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/xpegasus/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.621682 unitorch-0.0.0.4/src/unitorch/cli/models/xprophetnet/
--rw-r--r--   0 root         (0) root         (0)     1034 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/xprophetnet/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7811 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/xprophetnet/modeling.py
--rw-r--r--   0 root         (0) root         (0)     5952 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/models/xprophetnet/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.621682 unitorch-0.0.0.4/src/unitorch/cli/optim/
--rw-r--r--   0 root         (0) root         (0)     1628 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/optim/__init__.py
--rw-r--r--   0 root         (0) root         (0)      744 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/optim/lion.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.621682 unitorch-0.0.0.4/src/unitorch/cli/rl/
--rw-r--r--   0 root         (0) root         (0)       65 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/rl/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.625682 unitorch-0.0.0.4/src/unitorch/cli/scheduler/
--rw-r--r--   0 root         (0) root         (0)      141 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/scheduler/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3084 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/scheduler/warmup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.625682 unitorch-0.0.0.4/src/unitorch/cli/score/
--rw-r--r--   0 root         (0) root         (0)    14139 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/score/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.625682 unitorch-0.0.0.4/src/unitorch/cli/scripts/
--rw-r--r--   0 root         (0) root         (0)      158 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/scripts/README.md
--rw-r--r--   0 root         (0) root         (0)      213 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/scripts/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.625682 unitorch-0.0.0.4/src/unitorch/cli/services/
--rw-r--r--   0 root         (0) root         (0)      257 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/services/__init__.py
--rw-r--r--   0 root         (0) root         (0)      223 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/services/readme.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.625682 unitorch-0.0.0.4/src/unitorch/cli/services/zip_image/
--rw-r--r--   0 root         (0) root         (0)      113 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/services/zip_image/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4866 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/services/zip_image/service.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.625682 unitorch-0.0.0.4/src/unitorch/cli/tasks/
--rw-r--r--   0 root         (0) root         (0)      458 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/tasks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    26512 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/tasks/deepspeed.py
--rw-r--r--   0 root         (0) root         (0)    31576 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/tasks/supervised.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.629682 unitorch-0.0.0.4/src/unitorch/cli/utils/
--rw-r--r--   0 root         (0) root         (0)       65 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/utils/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.629682 unitorch-0.0.0.4/src/unitorch/cli/writer/
--rw-r--r--   0 root         (0) root         (0)    10544 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/cli/writer/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.629682 unitorch-0.0.0.4/src/unitorch/datasets/
--rw-r--r--   0 root         (0) root         (0)      130 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/datasets/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6832 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/datasets/hf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.629682 unitorch-0.0.0.4/src/unitorch/loss/
--rw-r--r--   0 root         (0) root         (0)     4712 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/loss/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1559 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/loss/prophetnet.py
--rw-r--r--   0 root         (0) root         (0)     8411 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/loss/ranking.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.629682 unitorch-0.0.0.4/src/unitorch/models/
--rw-r--r--   0 root         (0) root         (0)     7474 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.633682 unitorch-0.0.0.4/src/unitorch/models/bart/
--rw-r--r--   0 root         (0) root         (0)      204 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/bart/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13676 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/bart/modeling.py
--rw-r--r--   0 root         (0) root         (0)     1996 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/bart/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.633682 unitorch-0.0.0.4/src/unitorch/models/beit/
--rw-r--r--   0 root         (0) root         (0)      202 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/beit/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1540 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/beit/modeling.py
--rw-r--r--   0 root         (0) root         (0)      960 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/beit/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.633682 unitorch-0.0.0.4/src/unitorch/models/bert/
--rw-r--r--   0 root         (0) root         (0)      208 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/bert/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2446 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/bert/modeling.py
--rw-r--r--   0 root         (0) root         (0)     8355 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/bert/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.637682 unitorch-0.0.0.4/src/unitorch/models/blip/
--rw-r--r--   0 root         (0) root         (0)      306 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/blip/__init__.py
--rw-r--r--   0 root         (0) root         (0)    30316 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/blip/modeling.py
--rw-r--r--   0 root         (0) root         (0)     7700 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/blip/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.637682 unitorch-0.0.0.4/src/unitorch/models/bloom/
--rw-r--r--   0 root         (0) root         (0)      247 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/bloom/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10867 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/bloom/modeling.py
--rw-r--r--   0 root         (0) root         (0)     9140 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/bloom/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.641682 unitorch-0.0.0.4/src/unitorch/models/chatglm/
--rw-r--r--   0 root         (0) root         (0)      259 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/chatglm/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4201 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/chatglm/configuration_chatglm.py
--rw-r--r--   0 root         (0) root         (0)    11157 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/chatglm/modeling.py
--rw-r--r--   0 root         (0) root         (0)    55823 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/chatglm/modeling_chatglm.py
--rw-r--r--   0 root         (0) root         (0)    11091 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/chatglm/processing.py
--rw-r--r--   0 root         (0) root         (0)    15625 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/chatglm/quantization.py
--rw-r--r--   0 root         (0) root         (0)    16827 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/chatglm/tokenization_chatglm.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.641682 unitorch-0.0.0.4/src/unitorch/models/clip/
--rw-r--r--   0 root         (0) root         (0)      281 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/clip/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15100 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/clip/modeling.py
--rw-r--r--   0 root         (0) root         (0)     4393 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/clip/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.641682 unitorch-0.0.0.4/src/unitorch/models/deberta/
--rw-r--r--   0 root         (0) root         (0)      424 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/deberta/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4503 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/deberta/modeling.py
--rw-r--r--   0 root         (0) root         (0)     2568 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/deberta/modeling_v2.py
--rw-r--r--   0 root         (0) root         (0)     1744 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/deberta/processing.py
--rw-r--r--   0 root         (0) root         (0)     1603 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/deberta/processing_v2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.645682 unitorch-0.0.0.4/src/unitorch/models/diffusers/
--rw-r--r--   0 root         (0) root         (0)      548 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/diffusers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6076 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/diffusers/modeling_controlnet.py
--rw-r--r--   0 root         (0) root         (0)     8201 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/diffusers/modeling_stable.py
--rw-r--r--   0 root         (0) root         (0)     3313 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/diffusers/processing_controlnet.py
--rw-r--r--   0 root         (0) root         (0)     3029 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/diffusers/processing_stable.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.645682 unitorch-0.0.0.4/src/unitorch/models/llama/
--rw-r--r--   0 root         (0) root         (0)      247 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/llama/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11334 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/llama/modeling.py
--rw-r--r--   0 root         (0) root         (0)     8976 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/llama/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.649682 unitorch-0.0.0.4/src/unitorch/models/mbart/
--rw-r--r--   0 root         (0) root         (0)      188 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/mbart/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13928 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/mbart/modeling.py
--rw-r--r--   0 root         (0) root         (0)     2163 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/mbart/processing.py
--rw-r--r--   0 root         (0) root         (0)     2140 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/modeling_ema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.649682 unitorch-0.0.0.4/src/unitorch/models/mt5/
--rw-r--r--   0 root         (0) root         (0)      180 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/mt5/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14219 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/mt5/modeling.py
--rw-r--r--   0 root         (0) root         (0)     2272 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/mt5/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.649682 unitorch-0.0.0.4/src/unitorch/models/peft/
--rw-r--r--   0 root         (0) root         (0)     5424 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/peft/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9891 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/peft/modeling_bloom_adalora.py
--rw-r--r--   0 root         (0) root         (0)     9487 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/peft/modeling_bloom_lora.py
--rw-r--r--   0 root         (0) root         (0)    10082 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/peft/modeling_llama_adalora.py
--rw-r--r--   0 root         (0) root         (0)     9266 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/peft/modeling_llama_lora.py
--rw-r--r--   0 root         (0) root         (0)       65 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/peft/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.653682 unitorch-0.0.0.4/src/unitorch/models/pegasus/
--rw-r--r--   0 root         (0) root         (0)      196 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/pegasus/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13604 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/pegasus/modeling.py
--rw-r--r--   0 root         (0) root         (0)     2307 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/pegasus/processing.py
--rw-r--r--   0 root         (0) root         (0)    13125 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/processing_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.653682 unitorch-0.0.0.4/src/unitorch/models/prophetnet/
--rw-r--r--   0 root         (0) root         (0)      179 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/prophetnet/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7435 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/prophetnet/modeling.py
--rw-r--r--   0 root         (0) root         (0)     2095 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/prophetnet/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.653682 unitorch-0.0.0.4/src/unitorch/models/roberta/
--rw-r--r--   0 root         (0) root         (0)      218 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/roberta/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4281 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/roberta/modeling.py
--rw-r--r--   0 root         (0) root         (0)     1992 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/roberta/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.653682 unitorch-0.0.0.4/src/unitorch/models/swin/
--rw-r--r--   0 root         (0) root         (0)      193 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/swin/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1534 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/swin/modeling.py
--rw-r--r--   0 root         (0) root         (0)      998 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/swin/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.657682 unitorch-0.0.0.4/src/unitorch/models/t5/
--rw-r--r--   0 root         (0) root         (0)      194 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/t5/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13285 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/t5/modeling.py
--rw-r--r--   0 root         (0) root         (0)     1924 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/t5/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.657682 unitorch-0.0.0.4/src/unitorch/models/visualbert/
--rw-r--r--   0 root         (0) root         (0)      248 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/visualbert/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6710 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/visualbert/modeling.py
--rw-r--r--   0 root         (0) root         (0)     2132 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/visualbert/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.657682 unitorch-0.0.0.4/src/unitorch/models/vit/
--rw-r--r--   0 root         (0) root         (0)      189 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/vit/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1571 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/vit/modeling.py
--rw-r--r--   0 root         (0) root         (0)     1026 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/vit/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.657682 unitorch-0.0.0.4/src/unitorch/models/xlm_roberta/
--rw-r--r--   0 root         (0) root         (0)      323 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/xlm_roberta/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7381 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/xlm_roberta/modeling.py
--rw-r--r--   0 root         (0) root         (0)     1576 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/xlm_roberta/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.661682 unitorch-0.0.0.4/src/unitorch/models/xpegasus/
--rw-r--r--   0 root         (0) root         (0)      237 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/xpegasus/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13710 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/xpegasus/modeling.py
--rw-r--r--   0 root         (0) root         (0)     1464 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/xpegasus/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.661682 unitorch-0.0.0.4/src/unitorch/models/xprophetnet/
--rw-r--r--   0 root         (0) root         (0)      212 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/xprophetnet/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13514 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/xprophetnet/modeling.py
--rw-r--r--   0 root         (0) root         (0)     1335 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/models/xprophetnet/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.661682 unitorch-0.0.0.4/src/unitorch/modules/
--rw-r--r--   0 root         (0) root         (0)      133 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/modules/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2453 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/modules/classifier.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.665682 unitorch-0.0.0.4/src/unitorch/modules/replace/
--rw-r--r--   0 root         (0) root         (0)      199 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/modules/replace/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14643 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/modules/replace/beam_search_v2.py
--rw-r--r--   0 root         (0) root         (0)     2092 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/modules/replace/datasets_v2.py
--rw-r--r--   0 root         (0) root         (0)     4158 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/modules/replace/hf_hub_v2.py
--rw-r--r--   0 root         (0) root         (0)     2053 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/modules/timm.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.665682 unitorch-0.0.0.4/src/unitorch/ops/
--rw-r--r--   0 root         (0) root         (0)      105 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/ops/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16794 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/ops/dyhead.py
--rw-r--r--   0 root         (0) root         (0)     1347 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/ops/ngram_repeat_block.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.665682 unitorch-0.0.0.4/src/unitorch/optim/
--rw-r--r--   0 root         (0) root         (0)      203 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/optim/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3201 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/optim/lion.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.665682 unitorch-0.0.0.4/src/unitorch/rl/
--rw-r--r--   0 root         (0) root         (0)       65 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/rl/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.665682 unitorch-0.0.0.4/src/unitorch/rl/utils/
--rw-r--r--   0 root         (0) root         (0)       65 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/rl/utils/buffer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.665682 unitorch-0.0.0.4/src/unitorch/scheduler/
--rw-r--r--   0 root         (0) root         (0)      149 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/scheduler/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1635 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/scheduler/warmup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.669682 unitorch-0.0.0.4/src/unitorch/score/
--rw-r--r--   0 root         (0) root         (0)     1892 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/score/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4297 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/score/bleu.py
--rw-r--r--   0 root         (0) root         (0)     7852 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/score/map.py
--rw-r--r--   0 root         (0) root         (0)    13291 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/score/rouge.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.669682 unitorch-0.0.0.4/src/unitorch/tasks/
--rw-r--r--   0 root         (0) root         (0)       65 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/tasks/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.669682 unitorch-0.0.0.4/src/unitorch/utils/
--rw-r--r--   0 root         (0) root         (0)    13636 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2236 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/utils/decorators.py
--rw-r--r--   0 root         (0) root         (0)     2597 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/utils/functional.py
--rw-r--r--   0 root         (0) root         (0)     1240 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/utils/image_utils.py
--rw-r--r--   0 root         (0) root         (0)     2319 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/utils/import_utils.py
--rw-r--r--   0 root         (0) root         (0)     2639 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/utils/io.py
--rw-r--r--   0 root         (0) root         (0)     5027 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/utils/palette.py
--rw-r--r--   0 root         (0) root         (0)     3851 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/src/unitorch/utils/torch_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.585682 unitorch-0.0.0.4/src/unitorch.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8991 2023-07-04 07:55:37.000000 unitorch-0.0.0.4/src/unitorch.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    13037 2023-07-04 07:55:37.000000 unitorch-0.0.0.4/src/unitorch.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-04 07:55:37.000000 unitorch-0.0.0.4/src/unitorch.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      287 2023-07-04 07:55:37.000000 unitorch-0.0.0.4/src/unitorch.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      356 2023-07-04 07:55:37.000000 unitorch-0.0.0.4/src/unitorch.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-07-04 07:55:37.000000 unitorch-0.0.0.4/src/unitorch.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.673682 unitorch-0.0.0.4/wiki/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.673682 unitorch-0.0.0.4/wiki/benchmarks/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/benchmarks/index.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.673682 unitorch-0.0.0.4/wiki/cli/
--rw-r--r--   0 root         (0) root         (0)      504 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/cli/ast.md
--rw-r--r--   0 root         (0) root         (0)      173 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/cli/csv.md
--rw-r--r--   0 root         (0) root         (0)      414 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/cli/datatypes.md
--rw-r--r--   0 root         (0) root         (0)      197 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/cli/deepspeed.md
--rw-r--r--   0 root         (0) root         (0)      181 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/cli/jsonl.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.681682 unitorch-0.0.0.4/wiki/cli/models/
--rw-r--r--   0 root         (0) root         (0)      348 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/cli/models/bart.md
--rw-r--r--   0 root         (0) root         (0)      379 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/cli/models/beit.md
--rw-r--r--   0 root         (0) root         (0)      364 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/cli/models/bert.md
--rw-r--r--   0 root         (0) root         (0)     1113 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/cli/models/blip.md
--rw-r--r--   0 root         (0) root         (0)      719 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/cli/models/bloom.md
--rw-r--r--   0 root         (0) root         (0)      761 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/cli/models/chatglm.md
--rw-r--r--   0 root         (0) root         (0)      939 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/cli/models/clip.md
--rw-r--r--   0 root         (0) root         (0)      783 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/cli/models/deberta.md
--rw-r--r--   0 root         (0) root         (0)      353 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/cli/models/diffusers.md
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/cli/models/index.md
--rw-r--r--   0 root         (0) root         (0)      719 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/cli/models/llama.md
--rw-r--r--   0 root         (0) root         (0)      359 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/cli/models/mbart.md
--rw-r--r--   0 root         (0) root         (0)      337 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/cli/models/mt5.md
--rw-r--r--   0 root         (0) root         (0)     1712 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/cli/models/peft.md
--rw-r--r--   0 root         (0) root         (0)      381 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/cli/models/pegasus.md
--rw-r--r--   0 root         (0) root         (0)       36 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/cli/models/prophetnet.md
--rw-r--r--   0 root         (0) root         (0)      398 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/cli/models/roberta.md
--rw-r--r--   0 root         (0) root         (0)      379 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/cli/models/swin.md
--rw-r--r--   0 root         (0) root         (0)      326 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/cli/models/t5.md
--rw-r--r--   0 root         (0) root         (0)      623 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/cli/models/visualbert.md
--rw-r--r--   0 root         (0) root         (0)      368 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/cli/models/vit.md
--rw-r--r--   0 root         (0) root         (0)      664 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/cli/models/xlm_roberta.md
--rw-r--r--   0 root         (0) root         (0)      392 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/cli/models/xpegasus.md
--rw-r--r--   0 root         (0) root         (0)      425 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/cli/models/xprophetnet.md
--rw-r--r--   0 root         (0) root         (0)      189 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/cli/parquet.md
--rw-r--r--   0 root         (0) root         (0)      851 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/cli/postprocess.md
--rw-r--r--   0 root         (0) root         (0)      146 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/cli/preprocess.md
--rw-r--r--   0 root         (0) root         (0)      192 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/cli/supervised.md
--rw-r--r--   0 root         (0) root         (0)     4600 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/configuration.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.569682 unitorch-0.0.0.4/wiki/examples/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.681682 unitorch-0.0.0.4/wiki/examples/caption/
--rw-r--r--   0 root         (0) root         (0)     4659 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/examples/caption/blip.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.685682 unitorch-0.0.0.4/wiki/examples/classification/
--rw-r--r--   0 root         (0) root         (0)     4208 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/examples/classification/clip.md
--rw-r--r--   0 root         (0) root         (0)     4130 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/examples/classification/roberta.md
--rw-r--r--   0 root         (0) root         (0)     4525 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/examples/classification/swin.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.685682 unitorch-0.0.0.4/wiki/examples/diffusion/
--rw-r--r--   0 root         (0) root         (0)       32 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/examples/diffusion/controlnet.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.685682 unitorch-0.0.0.4/wiki/examples/generation/
--rw-r--r--   0 root         (0) root         (0)     4145 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/examples/generation/bart.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.685682 unitorch-0.0.0.4/wiki/examples/service/
--rw-r--r--   0 root         (0) root         (0)     1602 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/examples/service/zip_image.md
--rw-r--r--   0 root         (0) root         (0)     1346 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/index.md
--rw-r--r--   0 root         (0) root         (0)      890 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/installation.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.685682 unitorch-0.0.0.4/wiki/labs/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/labs/index.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-04 07:55:37.693682 unitorch-0.0.0.4/wiki/models/
--rw-r--r--   0 root         (0) root         (0)      147 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/models/bart.md
--rw-r--r--   0 root         (0) root         (0)      165 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/models/beit.md
--rw-r--r--   0 root         (0) root         (0)      155 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/models/bert.md
--rw-r--r--   0 root         (0) root         (0)      453 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/models/blip.md
--rw-r--r--   0 root         (0) root         (0)      296 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/models/bloom.md
--rw-r--r--   0 root         (0) root         (0)      322 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/models/chatglm.md
--rw-r--r--   0 root         (0) root         (0)      383 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/models/clip.md
--rw-r--r--   0 root         (0) root         (0)      402 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/models/deberta.md
--rw-r--r--   0 root         (0) root         (0)      152 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/models/diffusers.md
--rw-r--r--   0 root         (0) root         (0)      450 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/models/index.md
--rw-r--r--   0 root         (0) root         (0)      296 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/models/llama.md
--rw-r--r--   0 root         (0) root         (0)      154 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/models/mbart.md
--rw-r--r--   0 root         (0) root         (0)      140 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/models/mt5.md
--rw-r--r--   0 root         (0) root         (0)      695 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/models/peft.md
--rw-r--r--   0 root         (0) root         (0)      168 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/models/pegasus.md
--rw-r--r--   0 root         (0) root         (0)      107 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/models/prophetnet.md
--rw-r--r--   0 root         (0) root         (0)      243 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/models/roberta.md
--rw-r--r--   0 root         (0) root         (0)      165 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/models/swin.md
--rw-r--r--   0 root         (0) root         (0)      133 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/models/t5.md
--rw-r--r--   0 root         (0) root         (0)      277 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/models/visualbert.md
--rw-r--r--   0 root         (0) root         (0)      158 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/models/vit.md
--rw-r--r--   0 root         (0) root         (0)      375 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/models/xlm_roberta.md
--rw-r--r--   0 root         (0) root         (0)      175 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/models/xpegasus.md
--rw-r--r--   0 root         (0) root         (0)      196 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/models/xprophetnet.md
--rw-r--r--   0 root         (0) root         (0)     4524 2023-07-04 07:47:14.000000 unitorch-0.0.0.4/wiki/overview.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.757856 unitorch-0.0.0.5/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.549856 unitorch-0.0.0.5/.pytest_cache/
+-rw-r--r--   0 root         (0) root         (0)      302 2023-07-14 20:42:54.000000 unitorch-0.0.0.5/.pytest_cache/README.md
+-rw-r--r--   0 root         (0) root         (0)     1085 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      131 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     9246 2023-07-14 20:43:03.757856 unitorch-0.0.0.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8187 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.549856 unitorch-0.0.0.5/benchmarks/
+-rw-r--r--   0 root         (0) root         (0)       87 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/benchmarks/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.525856 unitorch-0.0.0.5/docs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.549856 unitorch-0.0.0.5/docs/search/
+-rw-r--r--   0 root         (0) root         (0)  1081944 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/docs/search/search_index.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.553856 unitorch-0.0.0.5/examples/
+-rw-r--r--   0 root         (0) root         (0)     2311 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/examples/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.529856 unitorch-0.0.0.5/examples/configs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.557856 unitorch-0.0.0.5/examples/configs/caption/
+-rw-r--r--   0 root         (0) root         (0)     1788 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/examples/configs/caption/blip.ini
+-rw-r--r--   0 root         (0) root         (0)     2556 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/examples/configs/caption/minigpt4.ini
+-rw-r--r--   0 root         (0) root         (0)     2692 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/examples/configs/caption/minigpt4_ds.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.561856 unitorch-0.0.0.5/examples/configs/classification/
+-rw-r--r--   0 root         (0) root         (0)     1545 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/examples/configs/classification/bert.ini
+-rw-r--r--   0 root         (0) root         (0)     1700 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/examples/configs/classification/clip.ini
+-rw-r--r--   0 root         (0) root         (0)     1688 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/examples/configs/classification/image_clip.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.561856 unitorch-0.0.0.5/examples/configs/classification/lora/
+-rw-r--r--   0 root         (0) root         (0)     1639 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/examples/configs/classification/lora/bloom.ini
+-rw-r--r--   0 root         (0) root         (0)     1615 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/examples/configs/classification/lora/bloom_ds.ini
+-rw-r--r--   0 root         (0) root         (0)     1857 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/examples/configs/classification/lora/llama.ini
+-rw-r--r--   0 root         (0) root         (0)     1810 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/examples/configs/classification/lora/llama_ds.ini
+-rw-r--r--   0 root         (0) root         (0)     1556 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/examples/configs/classification/roberta.ini
+-rw-r--r--   0 root         (0) root         (0)     1673 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/examples/configs/classification/swin.ini
+-rw-r--r--   0 root         (0) root         (0)     1636 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/examples/configs/classification/text_clip.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.561856 unitorch-0.0.0.5/examples/configs/deepspeed/
+-rw-r--r--   0 root         (0) root         (0)      500 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/examples/configs/deepspeed/adamw.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.565856 unitorch-0.0.0.5/examples/configs/diffusion/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.565856 unitorch-0.0.0.5/examples/configs/diffusion/controlnet/
+-rw-r--r--   0 root         (0) root         (0)     1925 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/examples/configs/diffusion/controlnet/canny.ini
+-rw-r--r--   0 root         (0) root         (0)     1751 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/examples/configs/diffusion/stable-v1.5.ini
+-rw-r--r--   0 root         (0) root         (0)     1751 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/examples/configs/diffusion/stable-v2.1.ini
+-rw-r--r--   0 root         (0) root         (0)     1747 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/examples/configs/diffusion/stable-v2.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.569856 unitorch-0.0.0.5/examples/configs/generation/
+-rw-r--r--   0 root         (0) root         (0)     1607 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/examples/configs/generation/bart.ini
+-rw-r--r--   0 root         (0) root         (0)     1651 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/examples/configs/generation/bloom.ini
+-rw-r--r--   0 root         (0) root         (0)     1667 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/examples/configs/generation/chatglm.ini
+-rw-r--r--   0 root         (0) root         (0)     1647 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/examples/configs/generation/llama.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.577856 unitorch-0.0.0.5/examples/configs/generation/lora/
+-rw-r--r--   0 root         (0) root         (0)     1608 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/examples/configs/generation/lora/bloom.ini
+-rw-r--r--   0 root         (0) root         (0)     1582 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/examples/configs/generation/lora/bloom_ds.ini
+-rw-r--r--   0 root         (0) root         (0)     1604 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/examples/configs/generation/lora/llama.ini
+-rw-r--r--   0 root         (0) root         (0)     1578 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/examples/configs/generation/lora/llama_ds.ini
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/examples/configs/generation/mbart.ini
+-rw-r--r--   0 root         (0) root         (0)     1597 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/examples/configs/generation/mt5.ini
+-rw-r--r--   0 root         (0) root         (0)     1655 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/examples/configs/generation/pegasus.ini
+-rw-r--r--   0 root         (0) root         (0)     1587 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/examples/configs/generation/t5.ini
+-rw-r--r--   0 root         (0) root         (0)     1647 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/examples/configs/generation/xpegasus.ini
+-rw-r--r--   0 root         (0) root         (0)     1745 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/examples/configs/generation/xprophetnet.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.577856 unitorch-0.0.0.5/examples/configs/pretrain/
+-rw-r--r--   0 root         (0) root         (0)     1266 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/examples/configs/pretrain/clip.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.529856 unitorch-0.0.0.5/examples/configs/services/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.577856 unitorch-0.0.0.5/examples/configs/services/zip_image/
+-rw-r--r--   0 root         (0) root         (0)      148 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/examples/configs/services/zip_image/config.ini
+-rw-r--r--   0 root         (0) root         (0)      240 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/examples/configs/services/zip_image/config_v2.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.529856 unitorch-0.0.0.5/examples/hub/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.577856 unitorch-0.0.0.5/examples/hub/caption/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/examples/hub/caption/blip.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.577856 unitorch-0.0.0.5/examples/hub/classification/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/examples/hub/classification/bert.ini
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/examples/hub/classification/clip.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.581856 unitorch-0.0.0.5/examples/hub/generation/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/examples/hub/generation/bart.ini
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/examples/hub/generation/llama.ini
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/examples/hub/generation/xpegasus.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.581856 unitorch-0.0.0.5/notebooks/
+-rw-r--r--   0 root         (0) root         (0)      131 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/notebooks/README.md
+-rw-r--r--   0 root         (0) root         (0)     1879 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      131 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-14 20:43:03.757856 unitorch-0.0.0.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1527 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.529856 unitorch-0.0.0.5/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.581856 unitorch-0.0.0.5/src/unitorch/
+-rw-r--r--   0 root         (0) root         (0)     2670 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.581856 unitorch-0.0.0.5/src/unitorch/cli/
+-rw-r--r--   0 root         (0) root         (0)     6024 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.585856 unitorch-0.0.0.5/src/unitorch/cli/console/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/console/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2092 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/console/eval.py
+-rw-r--r--   0 root         (0) root         (0)      358 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/console/fastapi.py
+-rw-r--r--   0 root         (0) root         (0)     2072 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/console/infer.py
+-rw-r--r--   0 root         (0) root         (0)     2151 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/console/script.py
+-rw-r--r--   0 root         (0) root         (0)     4683 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/console/service.py
+-rw-r--r--   0 root         (0) root         (0)     2095 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/console/train.py
+-rw-r--r--   0 root         (0) root         (0)     4397 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/core.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.585856 unitorch-0.0.0.5/src/unitorch/cli/datasets/
+-rw-r--r--   0 root         (0) root         (0)       98 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/datasets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12406 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/datasets/hf.py
+-rw-r--r--   0 root         (0) root         (0)     2613 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/decorators.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.589856 unitorch-0.0.0.5/src/unitorch/cli/loss/
+-rw-r--r--   0 root         (0) root         (0)     4063 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/loss/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2857 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/loss/ranking.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.593856 unitorch-0.0.0.5/src/unitorch/cli/models/
+-rw-r--r--   0 root         (0) root         (0)     2901 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.597856 unitorch-0.0.0.5/src/unitorch/cli/models/bart/
+-rw-r--r--   0 root         (0) root         (0)     1378 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/bart/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       65 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/bart/fastapi.py
+-rw-r--r--   0 root         (0) root         (0)     7012 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/bart/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     6140 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/bart/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.597856 unitorch-0.0.0.5/src/unitorch/cli/models/beit/
+-rw-r--r--   0 root         (0) root         (0)     1390 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/beit/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3142 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/beit/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     2535 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/beit/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.597856 unitorch-0.0.0.5/src/unitorch/cli/models/bert/
+-rw-r--r--   0 root         (0) root         (0)     1177 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/bert/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3903 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/bert/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     6128 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/bert/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.601856 unitorch-0.0.0.5/src/unitorch/cli/models/blip/
+-rw-r--r--   0 root         (0) root         (0)     2196 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/blip/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    22734 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/blip/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     7788 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/blip/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.601856 unitorch-0.0.0.5/src/unitorch/cli/models/bloom/
+-rw-r--r--   0 root         (0) root         (0)     2570 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/bloom/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13074 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/bloom/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     8321 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/bloom/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.605856 unitorch-0.0.0.5/src/unitorch/cli/models/chatglm/
+-rw-r--r--   0 root         (0) root         (0)     1201 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/chatglm/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13812 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/chatglm/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     8833 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/chatglm/processing.py
+-rw-r--r--   0 root         (0) root         (0)     9143 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/classification_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.605856 unitorch-0.0.0.5/src/unitorch/cli/models/clip/
+-rw-r--r--   0 root         (0) root         (0)     2514 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/clip/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16125 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/clip/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     5565 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/clip/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.609856 unitorch-0.0.0.5/src/unitorch/cli/models/deberta/
+-rw-r--r--   0 root         (0) root         (0)     4492 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/deberta/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4077 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/deberta/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     4021 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/deberta/modeling_v2.py
+-rw-r--r--   0 root         (0) root         (0)     3801 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/deberta/processing.py
+-rw-r--r--   0 root         (0) root         (0)     3434 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/deberta/processing_v2.py
+-rw-r--r--   0 root         (0) root         (0)     2545 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/detection_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.609856 unitorch-0.0.0.5/src/unitorch/cli/models/diffusers/
+-rw-r--r--   0 root         (0) root         (0)     2453 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/diffusers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7500 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/diffusers/modeling_controlnet.py
+-rw-r--r--   0 root         (0) root         (0)     9444 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/diffusers/modeling_stable.py
+-rw-r--r--   0 root         (0) root         (0)     3879 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/diffusers/processing_controlnet.py
+-rw-r--r--   0 root         (0) root         (0)     3838 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/diffusers/processing_stable.py
+-rw-r--r--   0 root         (0) root         (0)     3126 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/diffusion_utils.py
+-rw-r--r--   0 root         (0) root         (0)     2961 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/generation_utils.py
+-rw-r--r--   0 root         (0) root         (0)     5092 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/image_utils.py
+-rw-r--r--   0 root         (0) root         (0)     4297 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/label_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.613856 unitorch-0.0.0.5/src/unitorch/cli/models/llama/
+-rw-r--r--   0 root         (0) root         (0)     3445 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/llama/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14065 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/llama/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     8206 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/llama/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.613856 unitorch-0.0.0.5/src/unitorch/cli/models/mbart/
+-rw-r--r--   0 root         (0) root         (0)      887 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/mbart/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7650 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/mbart/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     5826 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/mbart/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.617856 unitorch-0.0.0.5/src/unitorch/cli/models/minigpt4/
+-rw-r--r--   0 root         (0) root         (0)     2870 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/minigpt4/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10738 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/minigpt4/modeling.py
+-rw-r--r--   0 root         (0) root         (0)    10044 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/minigpt4/processing.py
+-rw-r--r--   0 root         (0) root         (0)    15281 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/modeling_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.617856 unitorch-0.0.0.5/src/unitorch/cli/models/mt5/
+-rw-r--r--   0 root         (0) root         (0)     1381 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/mt5/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7173 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/mt5/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     5815 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/mt5/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.617856 unitorch-0.0.0.5/src/unitorch/cli/models/peft/
+-rw-r--r--   0 root         (0) root         (0)      524 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/peft/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    30598 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/peft/modeling_bloom.py
+-rw-r--r--   0 root         (0) root         (0)    30656 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/peft/modeling_llama.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.621856 unitorch-0.0.0.5/src/unitorch/cli/models/pegasus/
+-rw-r--r--   0 root         (0) root         (0)     1213 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/pegasus/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7281 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/pegasus/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     5885 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/pegasus/processing.py
+-rw-r--r--   0 root         (0) root         (0)     2834 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/processing_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.621856 unitorch-0.0.0.5/src/unitorch/cli/models/prophetnet/
+-rw-r--r--   0 root         (0) root         (0)      162 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/prophetnet/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       65 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/prophetnet/modeling.py
+-rw-r--r--   0 root         (0) root         (0)       65 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/prophetnet/processing.py
+-rw-r--r--   0 root         (0) root         (0)      650 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/random_utils.py
+-rw-r--r--   0 root         (0) root         (0)      535 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/ranking_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.625856 unitorch-0.0.0.5/src/unitorch/cli/models/roberta/
+-rw-r--r--   0 root         (0) root         (0)     1347 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/roberta/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3967 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/roberta/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     3766 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/roberta/processing.py
+-rw-r--r--   0 root         (0) root         (0)     2462 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/segmentation_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.625856 unitorch-0.0.0.5/src/unitorch/cli/models/swin/
+-rw-r--r--   0 root         (0) root         (0)     3032 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/swin/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3225 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/swin/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     2564 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/swin/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.625856 unitorch-0.0.0.5/src/unitorch/cli/models/t5/
+-rw-r--r--   0 root         (0) root         (0)     1282 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/t5/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7192 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/t5/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     5811 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/t5/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.629856 unitorch-0.0.0.5/src/unitorch/cli/models/visualbert/
+-rw-r--r--   0 root         (0) root         (0)     1310 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/visualbert/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8538 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/visualbert/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     6306 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/visualbert/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.629856 unitorch-0.0.0.5/src/unitorch/cli/models/vit/
+-rw-r--r--   0 root         (0) root         (0)     4602 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/vit/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3191 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/vit/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     2583 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/vit/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.633856 unitorch-0.0.0.5/src/unitorch/cli/models/xlm_roberta/
+-rw-r--r--   0 root         (0) root         (0)     2314 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/xlm_roberta/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7533 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/xlm_roberta/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     3408 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/xlm_roberta/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.633856 unitorch-0.0.0.5/src/unitorch/cli/models/xpegasus/
+-rw-r--r--   0 root         (0) root         (0)     1189 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/xpegasus/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7286 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/xpegasus/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     5953 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/xpegasus/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.633856 unitorch-0.0.0.5/src/unitorch/cli/models/xprophetnet/
+-rw-r--r--   0 root         (0) root         (0)     1034 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/xprophetnet/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7842 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/xprophetnet/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     5952 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/xprophetnet/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.637856 unitorch-0.0.0.5/src/unitorch/cli/optim/
+-rw-r--r--   0 root         (0) root         (0)     1628 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/optim/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      744 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/optim/lion.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.637856 unitorch-0.0.0.5/src/unitorch/cli/rl/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/rl/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.637856 unitorch-0.0.0.5/src/unitorch/cli/scheduler/
+-rw-r--r--   0 root         (0) root         (0)      141 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/scheduler/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3084 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/scheduler/warmup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.637856 unitorch-0.0.0.5/src/unitorch/cli/score/
+-rw-r--r--   0 root         (0) root         (0)    14139 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/score/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.641856 unitorch-0.0.0.5/src/unitorch/cli/scripts/
+-rw-r--r--   0 root         (0) root         (0)      158 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/scripts/README.md
+-rw-r--r--   0 root         (0) root         (0)      213 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/scripts/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.641856 unitorch-0.0.0.5/src/unitorch/cli/services/
+-rw-r--r--   0 root         (0) root         (0)      257 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/services/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      223 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/services/readme.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.645856 unitorch-0.0.0.5/src/unitorch/cli/services/zip_image/
+-rw-r--r--   0 root         (0) root         (0)      113 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/services/zip_image/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4866 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/services/zip_image/service.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.645856 unitorch-0.0.0.5/src/unitorch/cli/tasks/
+-rw-r--r--   0 root         (0) root         (0)      457 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/tasks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    26512 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/tasks/deepspeed.py
+-rw-r--r--   0 root         (0) root         (0)    31622 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/tasks/supervised.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.645856 unitorch-0.0.0.5/src/unitorch/cli/utils/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/utils/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.645856 unitorch-0.0.0.5/src/unitorch/cli/writer/
+-rw-r--r--   0 root         (0) root         (0)    10544 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/writer/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.649856 unitorch-0.0.0.5/src/unitorch/datasets/
+-rw-r--r--   0 root         (0) root         (0)      130 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/datasets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6832 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/datasets/hf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.649856 unitorch-0.0.0.5/src/unitorch/loss/
+-rw-r--r--   0 root         (0) root         (0)     4712 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/loss/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1559 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/loss/prophetnet.py
+-rw-r--r--   0 root         (0) root         (0)     8411 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/loss/ranking.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.653856 unitorch-0.0.0.5/src/unitorch/models/
+-rw-r--r--   0 root         (0) root         (0)     7498 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.653856 unitorch-0.0.0.5/src/unitorch/models/bart/
+-rw-r--r--   0 root         (0) root         (0)      204 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/bart/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13719 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/bart/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     1996 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/bart/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.657856 unitorch-0.0.0.5/src/unitorch/models/beit/
+-rw-r--r--   0 root         (0) root         (0)      202 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/beit/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1540 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/beit/modeling.py
+-rw-r--r--   0 root         (0) root         (0)      960 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/beit/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.657856 unitorch-0.0.0.5/src/unitorch/models/bert/
+-rw-r--r--   0 root         (0) root         (0)      208 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/bert/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2446 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/bert/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     8355 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/bert/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.661856 unitorch-0.0.0.5/src/unitorch/models/blip/
+-rw-r--r--   0 root         (0) root         (0)      306 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/blip/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    30337 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/blip/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     7704 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/blip/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.661856 unitorch-0.0.0.5/src/unitorch/models/blip2/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/blip2/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      606 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/blip2/modeling.py
+-rw-r--r--   0 root         (0) root         (0)      663 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/blip2/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.665856 unitorch-0.0.0.5/src/unitorch/models/bloom/
+-rw-r--r--   0 root         (0) root         (0)      247 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/bloom/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10885 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/bloom/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     9108 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/bloom/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.669856 unitorch-0.0.0.5/src/unitorch/models/chatglm/
+-rw-r--r--   0 root         (0) root         (0)      259 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/chatglm/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4201 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/chatglm/configuration_chatglm.py
+-rw-r--r--   0 root         (0) root         (0)    11175 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/chatglm/modeling.py
+-rw-r--r--   0 root         (0) root         (0)    55823 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/chatglm/modeling_chatglm.py
+-rw-r--r--   0 root         (0) root         (0)    11091 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/chatglm/processing.py
+-rw-r--r--   0 root         (0) root         (0)    15625 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/chatglm/quantization.py
+-rw-r--r--   0 root         (0) root         (0)    16827 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/chatglm/tokenization_chatglm.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.673856 unitorch-0.0.0.5/src/unitorch/models/clip/
+-rw-r--r--   0 root         (0) root         (0)      281 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/clip/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15100 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/clip/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     4393 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/clip/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.673856 unitorch-0.0.0.5/src/unitorch/models/deberta/
+-rw-r--r--   0 root         (0) root         (0)      424 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/deberta/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4503 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/deberta/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     2568 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/deberta/modeling_v2.py
+-rw-r--r--   0 root         (0) root         (0)     1744 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/deberta/processing.py
+-rw-r--r--   0 root         (0) root         (0)     1603 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/deberta/processing_v2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.677856 unitorch-0.0.0.5/src/unitorch/models/diffusers/
+-rw-r--r--   0 root         (0) root         (0)      547 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/diffusers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6076 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/diffusers/modeling_controlnet.py
+-rw-r--r--   0 root         (0) root         (0)     8201 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/diffusers/modeling_stable.py
+-rw-r--r--   0 root         (0) root         (0)     3313 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/diffusers/processing_controlnet.py
+-rw-r--r--   0 root         (0) root         (0)     3029 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/diffusers/processing_stable.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.677856 unitorch-0.0.0.5/src/unitorch/models/llama/
+-rw-r--r--   0 root         (0) root         (0)      247 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/llama/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11394 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/llama/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     8944 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/llama/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.681856 unitorch-0.0.0.5/src/unitorch/models/mbart/
+-rw-r--r--   0 root         (0) root         (0)      188 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/mbart/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13976 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/mbart/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     2163 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/mbart/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.681856 unitorch-0.0.0.5/src/unitorch/models/minigpt4/
+-rw-r--r--   0 root         (0) root         (0)      258 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/minigpt4/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16994 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/minigpt4/modeling.py
+-rw-r--r--   0 root         (0) root         (0)    13727 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/minigpt4/processing.py
+-rw-r--r--   0 root         (0) root         (0)     2140 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/modeling_ema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.681856 unitorch-0.0.0.5/src/unitorch/models/mt5/
+-rw-r--r--   0 root         (0) root         (0)      180 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/mt5/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14250 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/mt5/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     2272 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/mt5/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.685856 unitorch-0.0.0.5/src/unitorch/models/peft/
+-rw-r--r--   0 root         (0) root         (0)     5424 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/peft/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9934 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/peft/modeling_bloom_adalora.py
+-rw-r--r--   0 root         (0) root         (0)     9530 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/peft/modeling_bloom_lora.py
+-rw-r--r--   0 root         (0) root         (0)    10125 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/peft/modeling_llama_adalora.py
+-rw-r--r--   0 root         (0) root         (0)     9309 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/peft/modeling_llama_lora.py
+-rw-r--r--   0 root         (0) root         (0)       65 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/peft/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.689856 unitorch-0.0.0.5/src/unitorch/models/pegasus/
+-rw-r--r--   0 root         (0) root         (0)      196 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/pegasus/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13652 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/pegasus/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     2307 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/pegasus/processing.py
+-rw-r--r--   0 root         (0) root         (0)    13125 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/processing_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.689856 unitorch-0.0.0.5/src/unitorch/models/prophetnet/
+-rw-r--r--   0 root         (0) root         (0)      179 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/prophetnet/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7435 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/prophetnet/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     2095 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/prophetnet/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.693856 unitorch-0.0.0.5/src/unitorch/models/roberta/
+-rw-r--r--   0 root         (0) root         (0)      218 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/roberta/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4281 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/roberta/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     1992 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/roberta/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.693856 unitorch-0.0.0.5/src/unitorch/models/swin/
+-rw-r--r--   0 root         (0) root         (0)      193 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/swin/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1534 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/swin/modeling.py
+-rw-r--r--   0 root         (0) root         (0)      998 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/swin/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.693856 unitorch-0.0.0.5/src/unitorch/models/t5/
+-rw-r--r--   0 root         (0) root         (0)      194 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/t5/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13316 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/t5/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     1924 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/t5/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.697856 unitorch-0.0.0.5/src/unitorch/models/visualbert/
+-rw-r--r--   0 root         (0) root         (0)      248 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/visualbert/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6710 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/visualbert/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     2132 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/visualbert/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.697856 unitorch-0.0.0.5/src/unitorch/models/vit/
+-rw-r--r--   0 root         (0) root         (0)      189 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/vit/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1571 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/vit/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     1026 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/vit/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.701856 unitorch-0.0.0.5/src/unitorch/models/xlm_roberta/
+-rw-r--r--   0 root         (0) root         (0)      323 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/xlm_roberta/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7381 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/xlm_roberta/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     1576 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/xlm_roberta/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.701856 unitorch-0.0.0.5/src/unitorch/models/xpegasus/
+-rw-r--r--   0 root         (0) root         (0)      237 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/xpegasus/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13741 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/xpegasus/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     1464 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/xpegasus/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.701856 unitorch-0.0.0.5/src/unitorch/models/xprophetnet/
+-rw-r--r--   0 root         (0) root         (0)      212 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/xprophetnet/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13545 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/xprophetnet/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     1335 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/xprophetnet/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.705856 unitorch-0.0.0.5/src/unitorch/modules/
+-rw-r--r--   0 root         (0) root         (0)      133 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/modules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2453 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/modules/classifier.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.705856 unitorch-0.0.0.5/src/unitorch/modules/replace/
+-rw-r--r--   0 root         (0) root         (0)      199 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/modules/replace/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14643 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/modules/replace/beam_search_v2.py
+-rw-r--r--   0 root         (0) root         (0)     2092 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/modules/replace/datasets_v2.py
+-rw-r--r--   0 root         (0) root         (0)     4158 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/modules/replace/hf_hub_v2.py
+-rw-r--r--   0 root         (0) root         (0)     2053 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/modules/timm.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.709856 unitorch-0.0.0.5/src/unitorch/ops/
+-rw-r--r--   0 root         (0) root         (0)      105 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/ops/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16794 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/ops/dyhead.py
+-rw-r--r--   0 root         (0) root         (0)     1347 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/ops/ngram_repeat_block.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.709856 unitorch-0.0.0.5/src/unitorch/optim/
+-rw-r--r--   0 root         (0) root         (0)      203 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/optim/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3201 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/optim/lion.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.709856 unitorch-0.0.0.5/src/unitorch/rl/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/rl/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.709856 unitorch-0.0.0.5/src/unitorch/rl/utils/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/rl/utils/buffer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.709856 unitorch-0.0.0.5/src/unitorch/scheduler/
+-rw-r--r--   0 root         (0) root         (0)      149 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/scheduler/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1635 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/scheduler/warmup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.713856 unitorch-0.0.0.5/src/unitorch/score/
+-rw-r--r--   0 root         (0) root         (0)     1892 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/score/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4297 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/score/bleu.py
+-rw-r--r--   0 root         (0) root         (0)     7852 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/score/map.py
+-rw-r--r--   0 root         (0) root         (0)    13291 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/score/rouge.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.713856 unitorch-0.0.0.5/src/unitorch/tasks/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/tasks/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.717856 unitorch-0.0.0.5/src/unitorch/utils/
+-rw-r--r--   0 root         (0) root         (0)    13662 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2236 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/utils/decorators.py
+-rw-r--r--   0 root         (0) root         (0)     2597 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/utils/functional.py
+-rw-r--r--   0 root         (0) root         (0)     1240 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/utils/image_utils.py
+-rw-r--r--   0 root         (0) root         (0)     2711 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/utils/import_utils.py
+-rw-r--r--   0 root         (0) root         (0)     2639 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/utils/io.py
+-rw-r--r--   0 root         (0) root         (0)     5027 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/utils/palette.py
+-rw-r--r--   0 root         (0) root         (0)     3851 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/utils/torch_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.581856 unitorch-0.0.0.5/src/unitorch.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     9246 2023-07-14 20:43:03.000000 unitorch-0.0.0.5/src/unitorch.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    13660 2023-07-14 20:43:03.000000 unitorch-0.0.0.5/src/unitorch.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-14 20:43:03.000000 unitorch-0.0.0.5/src/unitorch.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      344 2023-07-14 20:43:03.000000 unitorch-0.0.0.5/src/unitorch.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      383 2023-07-14 20:43:03.000000 unitorch-0.0.0.5/src/unitorch.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-07-14 20:43:03.000000 unitorch-0.0.0.5/src/unitorch.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.721855 unitorch-0.0.0.5/wiki/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.721855 unitorch-0.0.0.5/wiki/benchmarks/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/benchmarks/index.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.725856 unitorch-0.0.0.5/wiki/cli/
+-rw-r--r--   0 root         (0) root         (0)      504 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/cli/ast.md
+-rw-r--r--   0 root         (0) root         (0)      173 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/cli/csv.md
+-rw-r--r--   0 root         (0) root         (0)      414 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/cli/datatypes.md
+-rw-r--r--   0 root         (0) root         (0)      197 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/cli/deepspeed.md
+-rw-r--r--   0 root         (0) root         (0)      181 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/cli/jsonl.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.737856 unitorch-0.0.0.5/wiki/cli/models/
+-rw-r--r--   0 root         (0) root         (0)      348 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/cli/models/bart.md
+-rw-r--r--   0 root         (0) root         (0)      379 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/cli/models/beit.md
+-rw-r--r--   0 root         (0) root         (0)      364 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/cli/models/bert.md
+-rw-r--r--   0 root         (0) root         (0)     1113 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/cli/models/blip.md
+-rw-r--r--   0 root         (0) root         (0)      719 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/cli/models/bloom.md
+-rw-r--r--   0 root         (0) root         (0)      761 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/cli/models/chatglm.md
+-rw-r--r--   0 root         (0) root         (0)      939 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/cli/models/clip.md
+-rw-r--r--   0 root         (0) root         (0)      783 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/cli/models/deberta.md
+-rw-r--r--   0 root         (0) root         (0)      353 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/cli/models/diffusers.md
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/cli/models/index.md
+-rw-r--r--   0 root         (0) root         (0)      719 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/cli/models/llama.md
+-rw-r--r--   0 root         (0) root         (0)      359 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/cli/models/mbart.md
+-rw-r--r--   0 root         (0) root         (0)      227 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/cli/models/minigpt4.md
+-rw-r--r--   0 root         (0) root         (0)      337 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/cli/models/mt5.md
+-rw-r--r--   0 root         (0) root         (0)     1712 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/cli/models/peft.md
+-rw-r--r--   0 root         (0) root         (0)      381 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/cli/models/pegasus.md
+-rw-r--r--   0 root         (0) root         (0)       36 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/cli/models/prophetnet.md
+-rw-r--r--   0 root         (0) root         (0)      398 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/cli/models/roberta.md
+-rw-r--r--   0 root         (0) root         (0)      379 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/cli/models/swin.md
+-rw-r--r--   0 root         (0) root         (0)      326 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/cli/models/t5.md
+-rw-r--r--   0 root         (0) root         (0)      623 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/cli/models/visualbert.md
+-rw-r--r--   0 root         (0) root         (0)      368 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/cli/models/vit.md
+-rw-r--r--   0 root         (0) root         (0)      664 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/cli/models/xlm_roberta.md
+-rw-r--r--   0 root         (0) root         (0)      392 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/cli/models/xpegasus.md
+-rw-r--r--   0 root         (0) root         (0)      425 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/cli/models/xprophetnet.md
+-rw-r--r--   0 root         (0) root         (0)      189 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/cli/parquet.md
+-rw-r--r--   0 root         (0) root         (0)      851 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/cli/postprocess.md
+-rw-r--r--   0 root         (0) root         (0)      146 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/cli/preprocess.md
+-rw-r--r--   0 root         (0) root         (0)      192 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/cli/supervised.md
+-rw-r--r--   0 root         (0) root         (0)     4600 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/configuration.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.545856 unitorch-0.0.0.5/wiki/examples/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.737856 unitorch-0.0.0.5/wiki/examples/caption/
+-rw-r--r--   0 root         (0) root         (0)     4659 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/examples/caption/blip.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.741855 unitorch-0.0.0.5/wiki/examples/classification/
+-rw-r--r--   0 root         (0) root         (0)     4208 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/examples/classification/clip.md
+-rw-r--r--   0 root         (0) root         (0)     4130 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/examples/classification/roberta.md
+-rw-r--r--   0 root         (0) root         (0)     4525 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/examples/classification/swin.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.741855 unitorch-0.0.0.5/wiki/examples/diffusion/
+-rw-r--r--   0 root         (0) root         (0)       32 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/examples/diffusion/controlnet.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.741855 unitorch-0.0.0.5/wiki/examples/generation/
+-rw-r--r--   0 root         (0) root         (0)     4145 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/examples/generation/bart.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.741855 unitorch-0.0.0.5/wiki/examples/service/
+-rw-r--r--   0 root         (0) root         (0)     1602 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/examples/service/zip_image.md
+-rw-r--r--   0 root         (0) root         (0)     1346 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/index.md
+-rw-r--r--   0 root         (0) root         (0)      890 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/installation.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.741855 unitorch-0.0.0.5/wiki/labs/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/labs/index.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.753856 unitorch-0.0.0.5/wiki/models/
+-rw-r--r--   0 root         (0) root         (0)      147 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/models/bart.md
+-rw-r--r--   0 root         (0) root         (0)      165 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/models/beit.md
+-rw-r--r--   0 root         (0) root         (0)      155 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/models/bert.md
+-rw-r--r--   0 root         (0) root         (0)      453 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/models/blip.md
+-rw-r--r--   0 root         (0) root         (0)      296 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/models/bloom.md
+-rw-r--r--   0 root         (0) root         (0)      322 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/models/chatglm.md
+-rw-r--r--   0 root         (0) root         (0)      383 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/models/clip.md
+-rw-r--r--   0 root         (0) root         (0)      402 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/models/deberta.md
+-rw-r--r--   0 root         (0) root         (0)      152 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/models/diffusers.md
+-rw-r--r--   0 root         (0) root         (0)      450 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/models/index.md
+-rw-r--r--   0 root         (0) root         (0)      296 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/models/llama.md
+-rw-r--r--   0 root         (0) root         (0)      154 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/models/mbart.md
+-rw-r--r--   0 root         (0) root         (0)      297 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/models/minigpt4.md
+-rw-r--r--   0 root         (0) root         (0)      140 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/models/mt5.md
+-rw-r--r--   0 root         (0) root         (0)      695 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/models/peft.md
+-rw-r--r--   0 root         (0) root         (0)      168 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/models/pegasus.md
+-rw-r--r--   0 root         (0) root         (0)      107 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/models/prophetnet.md
+-rw-r--r--   0 root         (0) root         (0)      243 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/models/roberta.md
+-rw-r--r--   0 root         (0) root         (0)      165 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/models/swin.md
+-rw-r--r--   0 root         (0) root         (0)      133 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/models/t5.md
+-rw-r--r--   0 root         (0) root         (0)      277 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/models/visualbert.md
+-rw-r--r--   0 root         (0) root         (0)      158 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/models/vit.md
+-rw-r--r--   0 root         (0) root         (0)      375 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/models/xlm_roberta.md
+-rw-r--r--   0 root         (0) root         (0)      175 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/models/xpegasus.md
+-rw-r--r--   0 root         (0) root         (0)      196 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/models/xprophetnet.md
+-rw-r--r--   0 root         (0) root         (0)     4524 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/overview.md
```

### Comparing `unitorch-0.0.0.4/LICENSE` & `unitorch-0.0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/PKG-INFO` & `unitorch-0.0.0.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unitorch
-Version: 0.0.0.4
+Version: 0.0.0.5
 Summary: unitorch provides efficient implementation of popular unified NLU / NLG / CV / CTR / MM / RL models with PyTorch.
 Author-email: fuliucansheng <fuliucansheng@gmail.com>
 License: MIT
 Keywords: PyTorch
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
@@ -18,14 +18,15 @@
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: deepspeed
 Provides-Extra: diffusers
 Provides-Extra: accelerate
 Provides-Extra: chatglm
+Provides-Extra: fastapi
 Provides-Extra: all
 License-File: LICENSE
 
 <div align="Center"> 
 
 ![unitorch](unitorch.png)
 
@@ -48,14 +49,15 @@
  
 🔥 unitorch is a library that simplifies and accelerates the development of unified models for natural language understanding, natural language generation, computer vision, click-through rate prediction, multimodal learning and reinforcement learning. It is built on top of PyTorch and integrates seamlessly with popular frameworks such as transformers, peft, diffusers, and fastseq. With unitorch, you can use a single command line tool or a one-line code ` import unitorch` import to leverage the state-of-the-art models and datasets without sacrificing performance or accuracy.
 
 ------------------------------------
 
 # What's New Model
 
+* **MiniGPT-4** released with the paper [MiniGPT-4: Enhancing Vision-Language Understanding with Advanced Large Language Models](https://arxiv.org/abs/2304.10592) by Deyao Zhu, Jun Chen, Xiaoqian Shen, Xiang Li, Mohamed Elhoseiny.
 * **LLaMA** released with the paper [LLaMA: Open and Efficient Foundation Language Models](https://arxiv.org/abs/2302.13971) by Hugo Touvron, Thibaut Lavril, Gautier Izacard, Xavier Martinet, Marie-Anne Lachaux, Timothée Lacroix, Baptiste Rozière, Naman Goyal, Eric Hambro, Faisal Azhar, Aurelien Rodriguez, Armand Joulin, Edouard Grave, Guillaume Lample.
 * **BLOOM** released with the paper [BLOOM: A 176B-Parameter Open-Access Multilingual Language Model](https://arxiv.org/abs/2211.05100) by BigScience Workshop: Teven Le Scao, Angela Fan, Christopher Akiki, Ellie Pavlick, Suzana Ilić, Daniel Hesslow...
 * **PEGASUS-X** released with the paper [Investigating Efficiently Extending Transformers for Long Input Summarization](https://arxiv.org/abs/2208.04347) by Jason Phang, Yao Zhao, Peter J. Liu.
 * **BLIP** released with the paper [BLIP: Bootstrapping Language-Image Pre-training for Unified Vision-Language Understanding and Generation](https://arxiv.org/abs/2201.12086) by Junnan Li, Dongxu Li, Caiming Xiong, Steven Hoi.
 * **BEiT** released with the paper [BEiT: BERT Pre-Training of Image Transformers](https://arxiv.org/abs/2106.08254) by Hangbo Bao, Li Dong, Songhao Piao, Furu Wei.
 * **Swin Transformer** released with the paper [Swin Transformer: Hierarchical Vision Transformer using Shifted Windows](https://arxiv.org/abs/2103.14030) by Ze Liu, Yutong Lin, Yue Cao, Han Hu, Yixuan Wei, Zheng Zhang, Stephen Lin, Baining Guo.
 * **CLIP** released with the paper [Learning Transferable Visual Models From Natural Language Supervision](https://arxiv.org/abs/2103.00020) by Alec Radford, Jong Wook Kim, Chris Hallacy, Aditya Ramesh, Gabriel Goh, Sandhini Agarwal, Girish Sastry, Amanda Askell, Pamela Mishkin, Jack Clark, Gretchen Krueger, Ilya Sutskever.
```

### Comparing `unitorch-0.0.0.4/README.md` & `unitorch-0.0.0.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -21,14 +21,15 @@
  
 🔥 unitorch is a library that simplifies and accelerates the development of unified models for natural language understanding, natural language generation, computer vision, click-through rate prediction, multimodal learning and reinforcement learning. It is built on top of PyTorch and integrates seamlessly with popular frameworks such as transformers, peft, diffusers, and fastseq. With unitorch, you can use a single command line tool or a one-line code ` import unitorch` import to leverage the state-of-the-art models and datasets without sacrificing performance or accuracy.
 
 ------------------------------------
 
 # What's New Model
 
+* **MiniGPT-4** released with the paper [MiniGPT-4: Enhancing Vision-Language Understanding with Advanced Large Language Models](https://arxiv.org/abs/2304.10592) by Deyao Zhu, Jun Chen, Xiaoqian Shen, Xiang Li, Mohamed Elhoseiny.
 * **LLaMA** released with the paper [LLaMA: Open and Efficient Foundation Language Models](https://arxiv.org/abs/2302.13971) by Hugo Touvron, Thibaut Lavril, Gautier Izacard, Xavier Martinet, Marie-Anne Lachaux, Timothée Lacroix, Baptiste Rozière, Naman Goyal, Eric Hambro, Faisal Azhar, Aurelien Rodriguez, Armand Joulin, Edouard Grave, Guillaume Lample.
 * **BLOOM** released with the paper [BLOOM: A 176B-Parameter Open-Access Multilingual Language Model](https://arxiv.org/abs/2211.05100) by BigScience Workshop: Teven Le Scao, Angela Fan, Christopher Akiki, Ellie Pavlick, Suzana Ilić, Daniel Hesslow...
 * **PEGASUS-X** released with the paper [Investigating Efficiently Extending Transformers for Long Input Summarization](https://arxiv.org/abs/2208.04347) by Jason Phang, Yao Zhao, Peter J. Liu.
 * **BLIP** released with the paper [BLIP: Bootstrapping Language-Image Pre-training for Unified Vision-Language Understanding and Generation](https://arxiv.org/abs/2201.12086) by Junnan Li, Dongxu Li, Caiming Xiong, Steven Hoi.
 * **BEiT** released with the paper [BEiT: BERT Pre-Training of Image Transformers](https://arxiv.org/abs/2106.08254) by Hangbo Bao, Li Dong, Songhao Piao, Furu Wei.
 * **Swin Transformer** released with the paper [Swin Transformer: Hierarchical Vision Transformer using Shifted Windows](https://arxiv.org/abs/2103.14030) by Ze Liu, Yutong Lin, Yue Cao, Han Hu, Yixuan Wei, Zheng Zhang, Stephen Lin, Baining Guo.
 * **CLIP** released with the paper [Learning Transferable Visual Models From Natural Language Supervision](https://arxiv.org/abs/2103.00020) by Alec Radford, Jong Wook Kim, Chris Hallacy, Aditya Ramesh, Gabriel Goh, Sandhini Agarwal, Girish Sastry, Amanda Askell, Pamela Mishkin, Jack Clark, Gretchen Krueger, Ilya Sutskever.
```

### Comparing `unitorch-0.0.0.4/docs/search/search_index.json` & `unitorch-0.0.0.5/docs/search/search_index.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9886294261294261%*

 * *Differences: {"'docs'": "{53: {'text': '<pre><code>train(\\n    optim: str,\\n    loss_fn: str,\\n    score_fn: "*

 * *           'str,\\n    monitor_fns: Optional[Union[str, List[str]]] = None,\\n    scheduler: '*

 * *           'Optional[str] = None,\\n    from_ckpt_dir: Optional[str] = "./from_ckpt",\\n    '*

 * *           'to_ckpt_dir: Optional[str] = "./to_ckpt",\\n    train_batch_size: Optional[int] = '*

 * *           '128,\\n    dev_batch_size: Optional[int] = 128,\\n    pin_memory: Optional[bool] = '*

 * *           'True,\\n    num_w […]*

```diff
@@ -272,15 +272,15 @@
         {
             "location": "cli/supervised/#unitorch.cli.tasks.supervised.SupervisedTask.infer",
             "text": "<pre><code>infer(\n    postprocess_fn: str,\n    writer: str,\n    test_batch_size: Optional[int] = 128,\n    pin_memory: Optional[bool] = True,\n    num_workers: Optional[int] = 4,\n    max_size: Optional[int] = 10000,\n    from_ckpt_dir: Optional[str] = \"./from_ckpt\",\n    output_header: Optional[List] = None,\n    output_path: Optional[str] = \"./cache/predict.txt\",\n    postprocess_workers: Optional[int] = 2,\n    gpu_mode: Optional[bool] = False,\n)\n</code></pre> <p>Perform inference using the model.</p> <p>Parameters:</p> Name Type Description Default <code>postprocess_fn</code> <code>str</code> <p>The postprocessing function for inference.</p> required <code>writer</code> <code>str</code> <p>The writer to save the inference results.</p> required <code>test_batch_size</code> <code>optional</code> <p>The batch size for inference. Defaults to 128.</p> <code>128</code> <code>pin_memory</code> <code>optional</code> <p>Whether to pin memory during data loading. Defaults to True.</p> <code>True</code> <code>num_workers</code> <code>optional</code> <p>The number of worker processes for data loading. Defaults to 4.</p> <code>4</code> <code>max_size</code> <code>optional</code> <p>The maximum number of samples to process. Defaults to 10000.</p> <code>10000</code> <code>from_ckpt_dir</code> <code>optional</code> <p>The directory path to load checkpoints from. Defaults to \"./from_ckpt\".</p> <code>'./from_ckpt'</code> <code>output_header</code> <code>optional</code> <p>The header for the output file. Defaults to None.</p> <code>None</code> <code>output_path</code> <code>optional</code> <p>The path to save the output file. Defaults to \"./cache/predict.txt\".</p> <code>'./cache/predict.txt'</code> <code>postprocess_workers</code> <code>optional</code> <p>The number of worker processes for postprocessing. Defaults to 2.</p> <code>2</code> <code>gpu_mode</code> <code>optional</code> <p>Whether to make GPU active. Defaults to False.</p> <code>False</code> Source code in <code>src/unitorch/cli/tasks/supervised.py</code> <pre><code>@torch.no_grad()\n@add_default_section_for_function(\"core/task/supervised\")\ndef infer(\n    self,\n    postprocess_fn: str,\n    writer: str,\n    test_batch_size: Optional[int] = 128,\n    pin_memory: Optional[bool] = True,\n    num_workers: Optional[int] = 4,\n    max_size: Optional[int] = 10000,\n    from_ckpt_dir: Optional[str] = \"./from_ckpt\",\n    output_header: Optional[List] = None,\n    output_path: Optional[str] = \"./cache/predict.txt\",\n    postprocess_workers: Optional[int] = 2,\n    gpu_mode: Optional[bool] = False,\n):\n\"\"\"\n    Perform inference using the model.\n\n    Args:\n        postprocess_fn: The postprocessing function for inference.\n        writer: The writer to save the inference results.\n        test_batch_size (optional): The batch size for inference. Defaults to 128.\n        pin_memory (optional): Whether to pin memory during data loading. Defaults to True.\n        num_workers (optional): The number of worker processes for data loading. Defaults to 4.\n        max_size (optional): The maximum number of samples to process. Defaults to 10000.\n        from_ckpt_dir (optional): The directory path to load checkpoints from. Defaults to \"./from_ckpt\".\n        output_header (optional): The header for the output file. Defaults to None.\n        output_path (optional): The path to save the output file. Defaults to \"./cache/predict.txt\".\n        postprocess_workers (optional): The number of worker processes for postprocessing. Defaults to 2.\n        gpu_mode (optional): Whether to make GPU active. Defaults to False.\n    \"\"\"\n    assert self.n_gpu &lt;= 1\n    assert writer is not None\n\n    output_dir = os.path.dirname(output_path)\n    if not os.path.exists(output_dir):\n        os.makedirs(output_dir, exist_ok=True)\n\n    if postprocess_fn is not None:\n        postprocess_fn = init_registered_process(postprocess_fn, self.config)\n\n    if writer is not None:\n        writer = init_registered_module(\n            writer,\n            self.config,\n            registered_writer,\n            output_file=output_path,\n        )\n\n    skip_step = writer.skip_n_samples\n\n    if os.path.exists(from_ckpt_dir):\n        self.model.from_checkpoint(from_ckpt_dir)\n\n    if skip_step == 0:\n        sampler = SequentialSampler\n    else:\n        sampler = SequentialSkipSampler\n\n    if gpu_mode:\n        with ActiveGPUJob() as _:\n            dataset_test = self.datasets.get(\"test\")\n    else:\n        dataset_test = self.datasets.get(\"test\")\n\n    iter_test = DataLoader(\n        dataset_test,\n        sampler=sampler(dataset_test)\n        if not isinstance(dataset_test, Iterable)\n        else None,\n        batch_size=test_batch_size,\n        shuffle=False,\n        pin_memory=pin_memory,\n        num_workers=num_workers,\n        collate_fn=collate_fn,\n    )\n\n    if skip_step &gt; 0 and hasattr(dataset_test, \"set_skip_step\"):\n        dataset_test.set_skip_step(skip_step)\n\n    if skip_step &gt; 0 and hasattr(iter_test.sampler, \"set_skip_step\"):\n        iter_test.sampler.set_skip_step(skip_step)\n\n    if hasattr(dataset_test, \"dataset\"):\n        data_info = dataset_test.dataset\n        data_info = DatasetFeature(data_info)\n        iter_data = DataLoader(\n            deepcopy(data_info),\n            sampler=sampler(data_info)\n            if not isinstance(dataset_test, Iterable)\n            else None,\n            batch_size=test_batch_size,\n            shuffle=False,\n            pin_memory=pin_memory,\n            num_workers=num_workers,\n            collate_fn=None,\n        )\n    else:\n        iter_data = None\n\n    if skip_step &gt; 0 and hasattr(iter_data.sampler, \"set_skip_step\"):\n        iter_data.sampler.set_skip_step(skip_step)\n\n    self.model.eval()\n    start = time.time()\n\n    data_queue = Queue(maxsize=max_size)\n    msg_queue = Queue(maxsize=max_size)\n    postprocess_list = []\n    for _ in range(postprocess_workers):\n        p = PostProcess(\n            postprocess_fn,\n            data_queue,\n            msg_queue,\n        )\n        postprocess_list.append(p)\n        p.start()\n\n    io_process = IOProcess(msg_queue, writer=writer)\n    io_process.start()\n\n    if iter_data is None:\n        for step, (inputs, _) in enumerate(iter_test):\n            if torch.cuda.is_available():\n                inputs = inputs.cuda()\n            outputs = self.model(**inputs.dict())\n            outputs = outputs.cpu()\n            data_queue.put((step, outputs))\n    else:\n        for step, ((inputs, _), _infos) in enumerate(zip(iter_test, iter_data)):\n            if torch.cuda.is_available():\n                inputs = inputs.cuda()\n            outputs = self.model(**inputs.dict())\n            outputs = outputs.cpu()\n            if output_header is not None:\n                _infos = {k: _infos[k] for k in output_header if k in _infos}\n                outputs.from_pandas(pd.DataFrame(_infos))\n            data_queue.put((step, outputs))\n\n    data_queue.put((-1, GENERATE_FINISHED))\n    for p in postprocess_list:\n        p.join()\n\n    msg_queue.put((-1, GENERATE_FINISHED))\n    io_process.join()\n\n    end = time.time()\n    ms = (end - start) * 1000\n    logging.info(\n        \"{:.2f} ms, {:.1f} sample/s\".format(\n            ms,\n            ((len(dataset_test) - skip_step) / ms * 1000),\n        )\n    )\n</code></pre>",
             "title": "infer"
         },
         {
             "location": "cli/supervised/#unitorch.cli.tasks.supervised.SupervisedTask.train",
-            "text": "<pre><code>train(\n    optim: str,\n    loss_fn: str,\n    score_fn: str,\n    monitor_fns: Optional[Union[str, List[str]]] = None,\n    scheduler: Optional[str] = None,\n    from_ckpt_dir: Optional[str] = \"./from_ckpt\",\n    to_ckpt_dir: Optional[str] = \"./to_ckpt\",\n    train_batch_size: Optional[int] = 128,\n    dev_batch_size: Optional[int] = 128,\n    pin_memory: Optional[bool] = True,\n    num_workers: Optional[int] = 4,\n    save_optimizer: Optional[bool] = True,\n    save_scheduler: Optional[bool] = True,\n    log_freq: Optional[int] = 100,\n    ckpt_freq: Optional[int] = 10000,\n    grad_acc_step: Optional[int] = 1,\n    max_grad_norm: Optional[float] = 1.0,\n    num_training_samples: Optional[int] = 1000000000,\n    epochs: Optional[int] = 5,\n    use_ema: Optional[bool] = False,\n    ema_decay: Optional[float] = 0.9999,\n    ema_tau: Optional[int] = 2000,\n    use_amp: Optional[bool] = True,\n    gpu_mode: Optional[bool] = False,\n)\n</code></pre> <p>Train the model.</p> <p>Parameters:</p> Name Type Description Default <code>optim</code> <code>str</code> <p>The optimizer for training.</p> required <code>loss_fn</code> <code>str</code> <p>The loss function for training.</p> required <code>score_fn</code> <code>str</code> <p>The scoring function for evaluation.</p> required <code>monitor_fns</code> <code>optional</code> <p>The monitoring functions for evaluation. Defaults to None.</p> <code>None</code> <code>scheduler</code> <code>optional</code> <p>The scheduler for adjusting the learning rate. Defaults to None.</p> <code>None</code> <code>from_ckpt_dir</code> <code>optional</code> <p>The directory path to load checkpoints from. Defaults to \"./from_ckpt\".</p> <code>'./from_ckpt'</code> <code>to_ckpt_dir</code> <code>optional</code> <p>The directory path to save checkpoints to. Defaults to \"./to_ckpt\".</p> <code>'./to_ckpt'</code> <code>train_batch_size</code> <code>optional</code> <p>The batch size for training. Defaults to 128.</p> <code>128</code> <code>dev_batch_size</code> <code>optional</code> <p>The batch size for evaluation. Defaults to 128.</p> <code>128</code> <code>pin_memory</code> <code>optional</code> <p>Whether to pin memory during data loading. Defaults to True.</p> <code>True</code> <code>num_workers</code> <code>optional</code> <p>The number of worker processes for data loading. Defaults to 4.</p> <code>4</code> <code>save_optimizer</code> <code>optional</code> <p>Whether to save the optimizer. Defaults to True.</p> <code>True</code> <code>save_scheduler</code> <code>optional</code> <p>Whether to save the scheduler. Defaults to True.</p> <code>True</code> <code>log_freq</code> <code>optional</code> <p>The frequency of logging training information. Defaults to 100.</p> <code>100</code> <code>ckpt_freq</code> <code>optional</code> <p>The frequency of saving checkpoints. Defaults to 10000.</p> <code>10000</code> <code>grad_acc_step</code> <code>optional</code> <p>The number of gradient accumulation steps. Defaults to 1.</p> <code>1</code> <code>max_grad_norm</code> <code>optional</code> <p>The maximum gradient norm for gradient clipping. Defaults to 1.0.</p> <code>1.0</code> <code>num_training_samples</code> <code>optional</code> <p>The number of training samples. Defaults to 1000000000.</p> <code>1000000000</code> <code>epochs</code> <code>optional</code> <p>The number of training epochs. Defaults to 5.</p> <code>5</code> <code>use_ema</code> <code>optional</code> <p>Whether to use exponential moving average. Defaults to False.</p> <code>False</code> <code>ema_decay</code> <code>optional</code> <p>The decay rate for exponential moving average. Defaults to 0.9999.</p> <code>0.9999</code> <code>ema_tau</code> <code>optional</code> <p>The time constant for exponential moving average. Defaults to 2000.</p> <code>2000</code> <code>use_amp</code> <code>optional</code> <p>Whether to use automatic mixed precision. Defaults to True.</p> <code>True</code> <code>gpu_mode</code> <code>optional</code> <p>Whether to make GPU active. Defaults to False.</p> <code>False</code> Source code in <code>src/unitorch/cli/tasks/supervised.py</code> <pre><code>@add_default_section_for_function(\"core/task/supervised\")\ndef train(\n    self,\n    optim: str,\n    loss_fn: str,\n    score_fn: str,\n    monitor_fns: Optional[Union[str, List[str]]] = None,\n    scheduler: Optional[str] = None,\n    from_ckpt_dir: Optional[str] = \"./from_ckpt\",\n    to_ckpt_dir: Optional[str] = \"./to_ckpt\",\n    train_batch_size: Optional[int] = 128,\n    dev_batch_size: Optional[int] = 128,\n    pin_memory: Optional[bool] = True,\n    num_workers: Optional[int] = 4,\n    save_optimizer: Optional[bool] = True,\n    save_scheduler: Optional[bool] = True,\n    log_freq: Optional[int] = 100,\n    ckpt_freq: Optional[int] = 10000,\n    grad_acc_step: Optional[int] = 1,\n    max_grad_norm: Optional[float] = 1.0,\n    num_training_samples: Optional[int] = 1000000000,\n    epochs: Optional[int] = 5,\n    use_ema: Optional[bool] = False,\n    ema_decay: Optional[float] = 0.9999,\n    ema_tau: Optional[int] = 2000,\n    use_amp: Optional[bool] = True,\n    gpu_mode: Optional[bool] = False,\n):\n\"\"\"\n    Train the model.\n\n    Args:\n        optim: The optimizer for training.\n        loss_fn: The loss function for training.\n        score_fn: The scoring function for evaluation.\n        monitor_fns (optional): The monitoring functions for evaluation. Defaults to None.\n        scheduler (optional): The scheduler for adjusting the learning rate. Defaults to None.\n        from_ckpt_dir (optional): The directory path to load checkpoints from. Defaults to \"./from_ckpt\".\n        to_ckpt_dir (optional): The directory path to save checkpoints to. Defaults to \"./to_ckpt\".\n        train_batch_size (optional): The batch size for training. Defaults to 128.\n        dev_batch_size (optional): The batch size for evaluation. Defaults to 128.\n        pin_memory (optional): Whether to pin memory during data loading. Defaults to True.\n        num_workers (optional): The number of worker processes for data loading. Defaults to 4.\n        save_optimizer (optional): Whether to save the optimizer. Defaults to True.\n        save_scheduler (optional): Whether to save the scheduler. Defaults to True.\n        log_freq (optional): The frequency of logging training information. Defaults to 100.\n        ckpt_freq (optional): The frequency of saving checkpoints. Defaults to 10000.\n        grad_acc_step (optional): The number of gradient accumulation steps. Defaults to 1.\n        max_grad_norm (optional): The maximum gradient norm for gradient clipping. Defaults to 1.0.\n        num_training_samples (optional): The number of training samples. Defaults to 1000000000.\n        epochs (optional): The number of training epochs. Defaults to 5.\n        use_ema (optional): Whether to use exponential moving average. Defaults to False.\n        ema_decay (optional): The decay rate for exponential moving average. Defaults to 0.9999.\n        ema_tau (optional): The time constant for exponential moving average. Defaults to 2000.\n        use_amp (optional): Whether to use automatic mixed precision. Defaults to True.\n        gpu_mode (optional): Whether to make GPU active. Defaults to False.\n    \"\"\"\n    if not os.path.exists(to_ckpt_dir) and self.local_rank in [-1, 0]:\n        os.makedirs(to_ckpt_dir, exist_ok=True)\n\n    if loss_fn is not None:\n        loss_fn = init_registered_module(loss_fn, self.config, registered_loss)\n\n    if score_fn is not None:\n        score_fn = init_registered_module(score_fn, self.config, registered_score)\n\n    if monitor_fns is not None:\n        monitor_fns = [\n            init_registered_module(monitor_fn, self.config, registered_score)\n            for monitor_fn in monitor_fns\n            if monitor_fn in registered_score\n        ]\n\n    if optim is not None and self.model is not None:\n        optim = init_registered_module(\n            optim,\n            self.config,\n            registered_optim,\n            params=self.model.parameters(),\n        )\n\n    if os.path.exists(from_ckpt_dir):\n        self.model.from_checkpoint(from_ckpt_dir)\n        optim.from_checkpoint(from_ckpt_dir, weight_name=\"pytorch_optim.bin\",)\n\n    if os.path.exists(to_ckpt_dir):\n        self.model.from_checkpoint(\n            to_ckpt_dir,\n            weight_name=\"pytorch_model_latest.bin\",\n        )\n        optim.from_checkpoint(\n            to_ckpt_dir,\n            weight_name=\"pytorch_optim_latest.bin\",\n        )\n\n    info_path = os.path.join(to_ckpt_dir, \"info.json\")\n    if os.path.exists(info_path):\n        info = json.load(open(os.path.join(to_ckpt_dir, \"info.json\")))\n    else:\n        info = dict()\n\n    global_epoch = info.get(\"global_epoch\", 0)\n    global_step = info.get(\"global_step\", 0)\n    self.best_score = info.get(\"best_score\", self.best_score)\n\n    logging.info(f\"the best score is {self.best_score}\")\n\n    self.ema_model = None\n    if use_ema:\n        num_ema_steps = info.get(\"num_ema_steps\", 0)\n        self.ema_model = ExponentialMovingAverage(\n            self.model,\n            decay=ema_decay,\n            tau=ema_tau,\n            num_steps=num_ema_steps,\n        )\n        if os.path.exists(from_ckpt_dir):\n            self.ema_model.from_checkpoint(\n                from_ckpt_dir,\n                weight_name=\"pytorch_ema_model.bin\",\n            )\n        if os.path.exists(to_ckpt_dir):\n            self.ema_model.from_checkpoint(\n                to_ckpt_dir,\n                weight_name=\"pytorch_ema_model_latest.bin\",\n            )\n\n    for n, p in self.model.named_parameters():\n        logging.debug(\n            f\"{n}: trainable - {p.requires_grad} | tensor shape - {p.shape}\"\n        )\n\n    global_rank = -1\n    if self.n_gpu &gt; 1:\n        self.model = nn.parallel.DistributedDataParallel(\n            self.model,\n            device_ids=[self.local_rank],\n            output_device=self.local_rank,\n            find_unused_parameters=False,\n            broadcast_buffers=False,\n        )\n        global_rank = dist.get_rank()\n\n    train_sampler = DistributedSkipSampler if self.n_gpu &gt; 1 else RandomSkipSampler\n    dev_sampler = DistributedSampler if self.n_gpu &gt; 1 else SequentialSampler\n\n    if gpu_mode:\n        with ActiveGPUJob() as _:\n            dataset_train = self.datasets.get(\"train\")\n            dataset_dev = self.datasets.get(\"dev\")\n    else:\n        dataset_train = self.datasets.get(\"train\")\n        dataset_dev = self.datasets.get(\"dev\")\n\n    iter_train = DataLoader(\n        dataset_train,\n        sampler=train_sampler(dataset_train)\n        if not isinstance(dataset_train, Iterable)\n        else None,\n        batch_size=train_batch_size,\n        shuffle=False,\n        pin_memory=pin_memory,\n        num_workers=num_workers,\n        collate_fn=collate_fn,\n    )\n\n    iter_dev = DataLoader(\n        dataset_dev,\n        sampler=dev_sampler(dataset_dev)\n        if not isinstance(dataset_dev, Iterable)\n        else None,\n        batch_size=dev_batch_size,\n        shuffle=False,\n        pin_memory=pin_memory,\n        num_workers=num_workers,\n        collate_fn=collate_fn,\n    )\n\n    if scheduler is not None:\n        if not isinstance(dataset_train, Iterable):\n            num_training_steps = int(\n                epochs\n                * len(dataset_train)\n                // train_batch_size\n                // max(1, self.n_gpu)\n                // grad_acc_step\n            )\n        else:\n            num_training_steps = int(\n                epochs\n                * num_training_samples\n                // train_batch_size\n                // max(1, self.n_gpu)\n                // grad_acc_step\n            )\n\n        scheduler = init_registered_module(\n            scheduler,\n            self.config,\n            registered_scheduler,\n            optimizer=optim,\n            num_training_steps=num_training_steps,\n        )\n\n    if scheduler and os.path.exists(to_ckpt_dir):\n        scheduler.from_checkpoint(\n            to_ckpt_dir,\n            weight_name=\"pytorch_scheduler_latest.bin\",\n        )\n\n    if use_amp:\n        scaler = GradScaler()\n\n    log_loss = 0\n    dev_epoch = 0\n    for e in range(0, epochs):\n        torch.cuda.empty_cache()\n        if e &lt; global_epoch:\n            continue\n\n        if hasattr(dataset_train, \"set_epoch\"):\n            dataset_train.set_epoch(e)\n\n        if hasattr(dataset_train, \"set_skip_step\"):\n            dataset_train.set_skip_step(global_step * train_batch_size)\n\n        if hasattr(iter_train.sampler, \"set_epoch\"):\n            iter_train.sampler.set_epoch(e)\n\n        if hasattr(iter_train.sampler, \"set_skip_step\"):\n            iter_train.sampler.set_skip_step(global_step * train_batch_size)\n\n        self.model.train()\n        is_update_step = True\n        for step, (inputs, targets) in enumerate(iter_train):\n            step = step + global_step\n            is_update_step = False\n            if torch.cuda.is_available():\n                inputs = inputs.cuda()\n                targets = targets.cuda()\n\n            if is_torch2_available():\n                with torch.cuda.amp.autocast(\n                    enabled=True\n                ) as autocast, torch.backends.cuda.sdp_kernel(\n                    enable_flash=False\n                ) as disable:\n                    outputs = self.model(**inputs.dict())\n                    if isinstance(outputs, LossOutputs):\n                        loss = outputs.loss / grad_acc_step\n                    else:\n                        loss = (\n                            loss_fn(outputs=outputs, targets=targets)\n                            / grad_acc_step\n                        )\n            else:\n                with torch.cuda.amp.autocast(enabled=True) as autocast:\n                    outputs = self.model(**inputs.dict())\n                    if isinstance(outputs, LossOutputs):\n                        loss = outputs.loss / grad_acc_step\n                    else:\n                        loss = (\n                            loss_fn(outputs=outputs, targets=targets)\n                            / grad_acc_step\n                        )\n\n            nn.utils.clip_grad_norm_(self.model.parameters(), max_grad_norm)\n            if use_amp:\n                scaler.scale(loss).backward()\n            else:\n                loss.backward()\n            log_loss += loss.data * grad_acc_step\n            if (step + 1) % grad_acc_step == 0:\n                is_update_step = True\n                if use_amp:\n                    scaler.step(optim)\n                    scaler.update()\n                else:\n                    optim.step()\n                if scheduler is not None:\n                    scheduler.step()\n                optim.zero_grad()\n\n                if use_ema and self.ema_model is not None:\n                    self.ema_model.step(\n                        self.model.module if self.n_gpu &gt; 1 else self.model\n                    )\n\n            if (step + 1) % log_freq == 0 and global_rank in [-1, 0]:\n                logging.info(\n                    f\"epoch {e} step {step}: loss -- { log_loss / log_freq }\"\n                )\n                log_loss = 0\n\n            if (step + 1) % ckpt_freq == 0:\n                if hasattr(dataset_dev, \"set_epoch\"):\n                    dataset_dev.set_epoch(dev_epoch)\n\n                if hasattr(iter_dev.sampler, \"set_epoch\"):\n                    iter_dev.sampler.set_epoch(dev_epoch)\n\n                dev_epoch += 1\n                self.best_score = save_checkpoint(\n                    self.model.module if self.n_gpu &gt; 1 else self.model,\n                    to_ckpt_dir,\n                    iter_dev,\n                    score_fn,\n                    monitor_fns,\n                    optim=optim if save_optimizer else None,\n                    scheduler=scheduler if save_scheduler else None,\n                    ema_model=self.ema_model if use_ema else None,\n                    best_score=self.best_score,\n                    info_path=info_path,\n                    local_rank=self.local_rank,\n                    global_epoch=e,\n                    global_step=step + 1,\n                )\n\n        if not is_update_step:\n            scaler.step(optim)\n            scaler.update()\n            if scheduler is not None:\n                scheduler.step()\n            optim.zero_grad()\n\n            if use_ema and self.ema_model is not None:\n                self.ema_model.step(\n                    self.model.module if self.n_gpu &gt; 1 else self.model\n                )\n\n        log_loss = 0\n\n        if hasattr(dataset_dev, \"set_epoch\"):\n            dataset_dev.set_epoch(dev_epoch)\n\n        if hasattr(iter_dev.sampler, \"set_epoch\"):\n            iter_dev.sampler.set_epoch(dev_epoch)\n\n        dev_epoch += 1\n\n        global_step = 0\n        self.best_score = save_checkpoint(\n            self.model.module if self.n_gpu &gt; 1 else self.model,\n            to_ckpt_dir,\n            iter_dev,\n            score_fn,\n            monitor_fns,\n            optim=optim if save_optimizer else None,\n            scheduler=scheduler if save_scheduler else None,\n            ema_model=self.ema_model if use_ema else None,\n            best_score=self.best_score,\n            info_path=info_path,\n            local_rank=self.local_rank,\n            global_epoch=e,\n            global_step=0,\n        )\n</code></pre>",
+            "text": "<pre><code>train(\n    optim: str,\n    loss_fn: str,\n    score_fn: str,\n    monitor_fns: Optional[Union[str, List[str]]] = None,\n    scheduler: Optional[str] = None,\n    from_ckpt_dir: Optional[str] = \"./from_ckpt\",\n    to_ckpt_dir: Optional[str] = \"./to_ckpt\",\n    train_batch_size: Optional[int] = 128,\n    dev_batch_size: Optional[int] = 128,\n    pin_memory: Optional[bool] = True,\n    num_workers: Optional[int] = 4,\n    save_optimizer: Optional[bool] = True,\n    save_scheduler: Optional[bool] = True,\n    log_freq: Optional[int] = 100,\n    ckpt_freq: Optional[int] = 10000,\n    grad_acc_step: Optional[int] = 1,\n    max_grad_norm: Optional[float] = 1.0,\n    num_training_samples: Optional[int] = 1000000000,\n    epochs: Optional[int] = 5,\n    use_ema: Optional[bool] = False,\n    ema_decay: Optional[float] = 0.9999,\n    ema_tau: Optional[int] = 2000,\n    use_amp: Optional[bool] = True,\n    gpu_mode: Optional[bool] = False,\n)\n</code></pre> <p>Train the model.</p> <p>Parameters:</p> Name Type Description Default <code>optim</code> <code>str</code> <p>The optimizer for training.</p> required <code>loss_fn</code> <code>str</code> <p>The loss function for training.</p> required <code>score_fn</code> <code>str</code> <p>The scoring function for evaluation.</p> required <code>monitor_fns</code> <code>optional</code> <p>The monitoring functions for evaluation. Defaults to None.</p> <code>None</code> <code>scheduler</code> <code>optional</code> <p>The scheduler for adjusting the learning rate. Defaults to None.</p> <code>None</code> <code>from_ckpt_dir</code> <code>optional</code> <p>The directory path to load checkpoints from. Defaults to \"./from_ckpt\".</p> <code>'./from_ckpt'</code> <code>to_ckpt_dir</code> <code>optional</code> <p>The directory path to save checkpoints to. Defaults to \"./to_ckpt\".</p> <code>'./to_ckpt'</code> <code>train_batch_size</code> <code>optional</code> <p>The batch size for training. Defaults to 128.</p> <code>128</code> <code>dev_batch_size</code> <code>optional</code> <p>The batch size for evaluation. Defaults to 128.</p> <code>128</code> <code>pin_memory</code> <code>optional</code> <p>Whether to pin memory during data loading. Defaults to True.</p> <code>True</code> <code>num_workers</code> <code>optional</code> <p>The number of worker processes for data loading. Defaults to 4.</p> <code>4</code> <code>save_optimizer</code> <code>optional</code> <p>Whether to save the optimizer. Defaults to True.</p> <code>True</code> <code>save_scheduler</code> <code>optional</code> <p>Whether to save the scheduler. Defaults to True.</p> <code>True</code> <code>log_freq</code> <code>optional</code> <p>The frequency of logging training information. Defaults to 100.</p> <code>100</code> <code>ckpt_freq</code> <code>optional</code> <p>The frequency of saving checkpoints. Defaults to 10000.</p> <code>10000</code> <code>grad_acc_step</code> <code>optional</code> <p>The number of gradient accumulation steps. Defaults to 1.</p> <code>1</code> <code>max_grad_norm</code> <code>optional</code> <p>The maximum gradient norm for gradient clipping. Defaults to 1.0.</p> <code>1.0</code> <code>num_training_samples</code> <code>optional</code> <p>The number of training samples. Defaults to 1000000000.</p> <code>1000000000</code> <code>epochs</code> <code>optional</code> <p>The number of training epochs. Defaults to 5.</p> <code>5</code> <code>use_ema</code> <code>optional</code> <p>Whether to use exponential moving average. Defaults to False.</p> <code>False</code> <code>ema_decay</code> <code>optional</code> <p>The decay rate for exponential moving average. Defaults to 0.9999.</p> <code>0.9999</code> <code>ema_tau</code> <code>optional</code> <p>The time constant for exponential moving average. Defaults to 2000.</p> <code>2000</code> <code>use_amp</code> <code>optional</code> <p>Whether to use automatic mixed precision. Defaults to True.</p> <code>True</code> <code>gpu_mode</code> <code>optional</code> <p>Whether to make GPU active. Defaults to False.</p> <code>False</code> Source code in <code>src/unitorch/cli/tasks/supervised.py</code> <pre><code>@add_default_section_for_function(\"core/task/supervised\")\ndef train(\n    self,\n    optim: str,\n    loss_fn: str,\n    score_fn: str,\n    monitor_fns: Optional[Union[str, List[str]]] = None,\n    scheduler: Optional[str] = None,\n    from_ckpt_dir: Optional[str] = \"./from_ckpt\",\n    to_ckpt_dir: Optional[str] = \"./to_ckpt\",\n    train_batch_size: Optional[int] = 128,\n    dev_batch_size: Optional[int] = 128,\n    pin_memory: Optional[bool] = True,\n    num_workers: Optional[int] = 4,\n    save_optimizer: Optional[bool] = True,\n    save_scheduler: Optional[bool] = True,\n    log_freq: Optional[int] = 100,\n    ckpt_freq: Optional[int] = 10000,\n    grad_acc_step: Optional[int] = 1,\n    max_grad_norm: Optional[float] = 1.0,\n    num_training_samples: Optional[int] = 1000000000,\n    epochs: Optional[int] = 5,\n    use_ema: Optional[bool] = False,\n    ema_decay: Optional[float] = 0.9999,\n    ema_tau: Optional[int] = 2000,\n    use_amp: Optional[bool] = True,\n    gpu_mode: Optional[bool] = False,\n):\n\"\"\"\n    Train the model.\n\n    Args:\n        optim: The optimizer for training.\n        loss_fn: The loss function for training.\n        score_fn: The scoring function for evaluation.\n        monitor_fns (optional): The monitoring functions for evaluation. Defaults to None.\n        scheduler (optional): The scheduler for adjusting the learning rate. Defaults to None.\n        from_ckpt_dir (optional): The directory path to load checkpoints from. Defaults to \"./from_ckpt\".\n        to_ckpt_dir (optional): The directory path to save checkpoints to. Defaults to \"./to_ckpt\".\n        train_batch_size (optional): The batch size for training. Defaults to 128.\n        dev_batch_size (optional): The batch size for evaluation. Defaults to 128.\n        pin_memory (optional): Whether to pin memory during data loading. Defaults to True.\n        num_workers (optional): The number of worker processes for data loading. Defaults to 4.\n        save_optimizer (optional): Whether to save the optimizer. Defaults to True.\n        save_scheduler (optional): Whether to save the scheduler. Defaults to True.\n        log_freq (optional): The frequency of logging training information. Defaults to 100.\n        ckpt_freq (optional): The frequency of saving checkpoints. Defaults to 10000.\n        grad_acc_step (optional): The number of gradient accumulation steps. Defaults to 1.\n        max_grad_norm (optional): The maximum gradient norm for gradient clipping. Defaults to 1.0.\n        num_training_samples (optional): The number of training samples. Defaults to 1000000000.\n        epochs (optional): The number of training epochs. Defaults to 5.\n        use_ema (optional): Whether to use exponential moving average. Defaults to False.\n        ema_decay (optional): The decay rate for exponential moving average. Defaults to 0.9999.\n        ema_tau (optional): The time constant for exponential moving average. Defaults to 2000.\n        use_amp (optional): Whether to use automatic mixed precision. Defaults to True.\n        gpu_mode (optional): Whether to make GPU active. Defaults to False.\n    \"\"\"\n    if not os.path.exists(to_ckpt_dir) and self.local_rank in [-1, 0]:\n        os.makedirs(to_ckpt_dir, exist_ok=True)\n\n    if loss_fn is not None:\n        loss_fn = init_registered_module(loss_fn, self.config, registered_loss)\n\n    if score_fn is not None:\n        score_fn = init_registered_module(score_fn, self.config, registered_score)\n\n    if monitor_fns is not None:\n        monitor_fns = [\n            init_registered_module(monitor_fn, self.config, registered_score)\n            for monitor_fn in monitor_fns\n            if monitor_fn in registered_score\n        ]\n\n    if optim is not None and self.model is not None:\n        optim = init_registered_module(\n            optim,\n            self.config,\n            registered_optim,\n            params=self.model.parameters(),\n        )\n\n    if os.path.exists(from_ckpt_dir):\n        self.model.from_checkpoint(from_ckpt_dir)\n        optim.from_checkpoint(\n            from_ckpt_dir,\n            weight_name=\"pytorch_optim.bin\",\n        )\n\n    if os.path.exists(to_ckpt_dir):\n        self.model.from_checkpoint(\n            to_ckpt_dir,\n            weight_name=\"pytorch_model_latest.bin\",\n        )\n        optim.from_checkpoint(\n            to_ckpt_dir,\n            weight_name=\"pytorch_optim_latest.bin\",\n        )\n\n    info_path = os.path.join(to_ckpt_dir, \"info.json\")\n    if os.path.exists(info_path):\n        info = json.load(open(os.path.join(to_ckpt_dir, \"info.json\")))\n    else:\n        info = dict()\n\n    global_epoch = info.get(\"global_epoch\", 0)\n    global_step = info.get(\"global_step\", 0)\n    self.best_score = info.get(\"best_score\", self.best_score)\n\n    logging.info(f\"the best score is {self.best_score}\")\n\n    self.ema_model = None\n    if use_ema:\n        num_ema_steps = info.get(\"num_ema_steps\", 0)\n        self.ema_model = ExponentialMovingAverage(\n            self.model,\n            decay=ema_decay,\n            tau=ema_tau,\n            num_steps=num_ema_steps,\n        )\n        if os.path.exists(from_ckpt_dir):\n            self.ema_model.from_checkpoint(\n                from_ckpt_dir,\n                weight_name=\"pytorch_ema_model.bin\",\n            )\n        if os.path.exists(to_ckpt_dir):\n            self.ema_model.from_checkpoint(\n                to_ckpt_dir,\n                weight_name=\"pytorch_ema_model_latest.bin\",\n            )\n\n    for n, p in self.model.named_parameters():\n        logging.debug(\n            f\"{n}: trainable - {p.requires_grad} | tensor shape - {p.shape}\"\n        )\n\n    global_rank = -1\n    if self.n_gpu &gt; 1:\n        self.model = nn.parallel.DistributedDataParallel(\n            self.model,\n            device_ids=[self.local_rank],\n            output_device=self.local_rank,\n            find_unused_parameters=False,\n            broadcast_buffers=False,\n        )\n        global_rank = dist.get_rank()\n\n    train_sampler = DistributedSkipSampler if self.n_gpu &gt; 1 else RandomSkipSampler\n    dev_sampler = DistributedSampler if self.n_gpu &gt; 1 else SequentialSampler\n\n    if gpu_mode:\n        with ActiveGPUJob() as _:\n            dataset_train = self.datasets.get(\"train\")\n            dataset_dev = self.datasets.get(\"dev\")\n    else:\n        dataset_train = self.datasets.get(\"train\")\n        dataset_dev = self.datasets.get(\"dev\")\n\n    iter_train = DataLoader(\n        dataset_train,\n        sampler=train_sampler(dataset_train)\n        if not isinstance(dataset_train, Iterable)\n        else None,\n        batch_size=train_batch_size,\n        shuffle=False,\n        pin_memory=pin_memory,\n        num_workers=num_workers,\n        collate_fn=collate_fn,\n    )\n\n    iter_dev = DataLoader(\n        dataset_dev,\n        sampler=dev_sampler(dataset_dev)\n        if not isinstance(dataset_dev, Iterable)\n        else None,\n        batch_size=dev_batch_size,\n        shuffle=False,\n        pin_memory=pin_memory,\n        num_workers=num_workers,\n        collate_fn=collate_fn,\n    )\n\n    if scheduler is not None:\n        if not isinstance(dataset_train, Iterable):\n            num_training_steps = int(\n                epochs\n                * len(dataset_train)\n                // train_batch_size\n                // max(1, self.n_gpu)\n                // grad_acc_step\n            )\n        else:\n            num_training_steps = int(\n                epochs\n                * num_training_samples\n                // train_batch_size\n                // max(1, self.n_gpu)\n                // grad_acc_step\n            )\n\n        scheduler = init_registered_module(\n            scheduler,\n            self.config,\n            registered_scheduler,\n            optimizer=optim,\n            num_training_steps=num_training_steps,\n        )\n\n    if scheduler and os.path.exists(to_ckpt_dir):\n        scheduler.from_checkpoint(\n            to_ckpt_dir,\n            weight_name=\"pytorch_scheduler_latest.bin\",\n        )\n\n    if use_amp:\n        scaler = GradScaler()\n\n    log_loss = 0\n    dev_epoch = 0\n    for e in range(0, epochs):\n        torch.cuda.empty_cache()\n        if e &lt; global_epoch:\n            continue\n\n        if hasattr(dataset_train, \"set_epoch\"):\n            dataset_train.set_epoch(e)\n\n        if hasattr(dataset_train, \"set_skip_step\"):\n            dataset_train.set_skip_step(global_step * train_batch_size)\n\n        if hasattr(iter_train.sampler, \"set_epoch\"):\n            iter_train.sampler.set_epoch(e)\n\n        if hasattr(iter_train.sampler, \"set_skip_step\"):\n            iter_train.sampler.set_skip_step(global_step * train_batch_size)\n\n        self.model.train()\n        is_update_step = True\n        for step, (inputs, targets) in enumerate(iter_train):\n            step = step + global_step\n            is_update_step = False\n            if torch.cuda.is_available():\n                inputs = inputs.cuda()\n                targets = targets.cuda()\n\n            if is_torch2_available():\n                with torch.cuda.amp.autocast(\n                    enabled=True\n                ) as autocast, torch.backends.cuda.sdp_kernel(\n                    enable_flash=False\n                ) as disable:\n                    outputs = self.model(**inputs.dict())\n                    if isinstance(outputs, LossOutputs):\n                        loss = outputs.loss / grad_acc_step\n                    else:\n                        loss = (\n                            loss_fn(outputs=outputs, targets=targets)\n                            / grad_acc_step\n                        )\n            else:\n                with torch.cuda.amp.autocast(enabled=True) as autocast:\n                    outputs = self.model(**inputs.dict())\n                    if isinstance(outputs, LossOutputs):\n                        loss = outputs.loss / grad_acc_step\n                    else:\n                        loss = (\n                            loss_fn(outputs=outputs, targets=targets)\n                            / grad_acc_step\n                        )\n\n            nn.utils.clip_grad_norm_(self.model.parameters(), max_grad_norm)\n            if use_amp:\n                scaler.scale(loss).backward()\n            else:\n                loss.backward()\n            log_loss += loss.data * grad_acc_step\n            if (step + 1) % grad_acc_step == 0:\n                is_update_step = True\n                if use_amp:\n                    scaler.step(optim)\n                    scaler.update()\n                else:\n                    optim.step()\n                if scheduler is not None:\n                    scheduler.step()\n                optim.zero_grad()\n\n                if use_ema and self.ema_model is not None:\n                    self.ema_model.step(\n                        self.model.module if self.n_gpu &gt; 1 else self.model\n                    )\n\n            if (step + 1) % log_freq == 0 and global_rank in [-1, 0]:\n                logging.info(\n                    f\"epoch {e} step {step}: loss -- { log_loss / log_freq }\"\n                )\n                log_loss = 0\n\n            if (step + 1) % ckpt_freq == 0:\n                if hasattr(dataset_dev, \"set_epoch\"):\n                    dataset_dev.set_epoch(dev_epoch)\n\n                if hasattr(iter_dev.sampler, \"set_epoch\"):\n                    iter_dev.sampler.set_epoch(dev_epoch)\n\n                dev_epoch += 1\n                self.best_score = save_checkpoint(\n                    self.model.module if self.n_gpu &gt; 1 else self.model,\n                    to_ckpt_dir,\n                    iter_dev,\n                    score_fn,\n                    monitor_fns,\n                    optim=optim if save_optimizer else None,\n                    scheduler=scheduler if save_scheduler else None,\n                    ema_model=self.ema_model if use_ema else None,\n                    best_score=self.best_score,\n                    info_path=info_path,\n                    local_rank=self.local_rank,\n                    global_epoch=e,\n                    global_step=step + 1,\n                )\n\n        if not is_update_step:\n            scaler.step(optim)\n            scaler.update()\n            if scheduler is not None:\n                scheduler.step()\n            optim.zero_grad()\n\n            if use_ema and self.ema_model is not None:\n                self.ema_model.step(\n                    self.model.module if self.n_gpu &gt; 1 else self.model\n                )\n\n        log_loss = 0\n\n        if hasattr(dataset_dev, \"set_epoch\"):\n            dataset_dev.set_epoch(dev_epoch)\n\n        if hasattr(iter_dev.sampler, \"set_epoch\"):\n            iter_dev.sampler.set_epoch(dev_epoch)\n\n        dev_epoch += 1\n\n        global_step = 0\n        self.best_score = save_checkpoint(\n            self.model.module if self.n_gpu &gt; 1 else self.model,\n            to_ckpt_dir,\n            iter_dev,\n            score_fn,\n            monitor_fns,\n            optim=optim if save_optimizer else None,\n            scheduler=scheduler if save_scheduler else None,\n            ema_model=self.ema_model if use_ema else None,\n            best_score=self.best_score,\n            info_path=info_path,\n            local_rank=self.local_rank,\n            global_epoch=e,\n            global_step=0,\n        )\n</code></pre>",
             "title": "train"
         },
         {
             "location": "cli/models/bart/",
             "text": "",
             "title": "unitorch.cli.models.bart"
         },
@@ -307,15 +307,15 @@
         {
             "location": "cli/models/bart/#unitorch.cli.models.bart.modeling.BartForGeneration.from_core_configure",
             "text": "<pre><code>from_core_configure(config, **kwargs)\n</code></pre> <p>Create an instance of BartForGeneration from core configuration.</p> <p>Parameters:</p> Name Type Description Default <code>config</code> <p>The core configuration object.</p> required <code>**kwargs</code> <p>Additional keyword arguments.</p> <code>{}</code> <p>Returns:</p> Name Type Description <code>BartForGeneration</code> <p>The initialized BartForGeneration instance.</p> Source code in <code>src/unitorch/cli/models/bart/modeling.py</code> <pre><code>@classmethod\n@add_default_section_for_init(\"core/model/generation/bart\")\ndef from_core_configure(cls, config, **kwargs):\n\"\"\"\n    Create an instance of BartForGeneration from core configuration.\n\n    Args:\n        config: The core configuration object.\n        **kwargs: Additional keyword arguments.\n\n    Returns:\n        BartForGeneration: The initialized BartForGeneration instance.\n    \"\"\"\n    config.set_default_section(\"core/model/generation/bart\")\n    pretrained_name = config.getoption(\"pretrained_name\", \"default-bart\")\n    config_path = config.getoption(\"config_path\", None)\n    config_path = pop_value(\n        config_path,\n        nested_dict_value(pretrained_bart_infos, pretrained_name, \"config\"),\n    )\n\n    config_path = cached_path(config_path)\n    gradient_checkpointing = config.getoption(\"gradient_checkpointing\", False)\n\n    inst = cls(config_path, gradient_checkpointing)\n    pretrained_weight_path = config.getoption(\"pretrained_weight_path\", None)\n    weight_path = pop_value(\n        pretrained_weight_path,\n        nested_dict_value(pretrained_bart_infos, pretrained_name, \"weight\"),\n        check_none=False,\n    )\n    if weight_path is not None:\n        weight_path = cached_path(weight_path)\n        inst.from_pretrained(weight_path)\n\n    return inst\n</code></pre>",
             "title": "from_core_configure  <code>classmethod</code>"
         },
         {
             "location": "cli/models/bart/#unitorch.cli.models.bart.modeling.BartForGeneration.generate",
-            "text": "<pre><code>generate(\n    input_ids: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 2,\n    decoder_end_token_id: Optional[int] = 2,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n)\n</code></pre> <p>Generate sequences using the BartForGeneration model.</p> <p>Parameters:</p> Name Type Description Default <code>input_ids</code> <code>torch.Tensor</code> <p>Input IDs.</p> required <code>num_beams</code> <code>int</code> <p>Number of beams for beam search.</p> <code>5</code> <code>decoder_start_token_id</code> <code>int</code> <p>ID of the decoder start token.</p> <code>2</code> <code>decoder_end_token_id</code> <code>int</code> <p>ID of the decoder end token.</p> <code>2</code> <code>num_return_sequences</code> <code>int</code> <p>Number of generated sequences to return.</p> <code>1</code> <code>min_gen_seq_length</code> <code>int</code> <p>Minimum length of generated sequences.</p> <code>0</code> <code>max_gen_seq_length</code> <code>int</code> <p>Maximum length of generated sequences.</p> <code>48</code> <code>repetition_penalty</code> <code>float</code> <p>Repetition penalty.</p> <code>1.0</code> <code>no_repeat_ngram_size</code> <code>int</code> <p>Size of n-grams to avoid repeating.</p> <code>0</code> <code>early_stopping</code> <code>bool</code> <p>Whether to stop generation early.</p> <code>True</code> <code>length_penalty</code> <code>float</code> <p>Length penalty for generated sequences.</p> <code>1.0</code> <code>num_beam_groups</code> <code>int</code> <p>Number of groups for diverse beam search.</p> <code>1</code> <code>diversity_penalty</code> <code>float</code> <p>Diversity penalty for diverse beam search.</p> <code>0.0</code> <code>do_sample</code> <code>bool</code> <p>Whether to use sampling for generation.</p> <code>False</code> <code>temperature</code> <code>float</code> <p>Sampling temperature.</p> <code>1.0</code> <code>top_k</code> <code>int</code> <p>Top-k sampling parameter.</p> <code>50</code> <code>top_p</code> <code>float</code> <p>Top-p sampling parameter.</p> <code>1.0</code> <p>Returns:</p> Name Type Description <code>GenerationOutputs</code> <p>The generated sequences and their scores.</p> Source code in <code>src/unitorch/cli/models/bart/modeling.py</code> <pre><code>@add_default_section_for_function(\"core/model/generation/bart\")\n@torch.no_grad()\n@autocast()\ndef generate(\n    self,\n    input_ids: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 2,\n    decoder_end_token_id: Optional[int] = 2,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n):\n\"\"\"\n    Generate sequences using the BartForGeneration model.\n\n    Args:\n        input_ids (torch.Tensor): Input IDs.\n        num_beams (int, optional): Number of beams for beam search.\n        decoder_start_token_id (int, optional): ID of the decoder start token.\n        decoder_end_token_id (int, optional): ID of the decoder end token.\n        num_return_sequences (int, optional): Number of generated sequences to return.\n        min_gen_seq_length (int, optional): Minimum length of generated sequences.\n        max_gen_seq_length (int, optional): Maximum length of generated sequences.\n        repetition_penalty (float, optional): Repetition penalty.\n        no_repeat_ngram_size (int, optional): Size of n-grams to avoid repeating.\n        early_stopping (bool, optional): Whether to stop generation early.\n        length_penalty (float, optional): Length penalty for generated sequences.\n        num_beam_groups (int, optional): Number of groups for diverse beam search.\n        diversity_penalty (float, optional): Diversity penalty for diverse beam search.\n        do_sample (bool, optional): Whether to use sampling for generation.\n        temperature (float, optional): Sampling temperature.\n        top_k (int, optional): Top-k sampling parameter.\n        top_p (float, optional): Top-p sampling parameter.\n\n    Returns:\n        GenerationOutputs: The generated sequences and their scores.\n    \"\"\"\n    outputs = super().generate(\n        input_ids=input_ids,\n        num_beams=num_beams,\n        decoder_start_token_id=decoder_start_token_id,\n        decoder_end_token_id=decoder_end_token_id,\n        num_return_sequences=num_return_sequences,\n        min_gen_seq_length=min_gen_seq_length,\n        max_gen_seq_length=max_gen_seq_length,\n        repetition_penalty=repetition_penalty,\n        no_repeat_ngram_size=no_repeat_ngram_size,\n        early_stopping=early_stopping,\n        length_penalty=length_penalty,\n        num_beam_groups=num_beam_groups,\n        diversity_penalty=diversity_penalty,\n        do_sample=do_sample,\n        temperature=temperature,\n        top_k=top_k,\n        top_p=top_p,\n    )\n\n    return GenerationOutputs(\n        sequences=outputs.sequences,\n        sequences_scores=outputs.sequences_scores,\n    )\n</code></pre>",
+            "text": "<pre><code>generate(\n    input_ids: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 2,\n    decoder_end_token_id: Optional[\n        Union[int, List[int]]\n    ] = 2,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n)\n</code></pre> <p>Generate sequences using the BartForGeneration model.</p> <p>Parameters:</p> Name Type Description Default <code>input_ids</code> <code>torch.Tensor</code> <p>Input IDs.</p> required <code>num_beams</code> <code>int</code> <p>Number of beams for beam search.</p> <code>5</code> <code>decoder_start_token_id</code> <code>int</code> <p>ID of the decoder start token.</p> <code>2</code> <code>decoder_end_token_id</code> <code>int or List[int]</code> <p>ID of the decoder end token.</p> <code>2</code> <code>num_return_sequences</code> <code>int</code> <p>Number of generated sequences to return.</p> <code>1</code> <code>min_gen_seq_length</code> <code>int</code> <p>Minimum length of generated sequences.</p> <code>0</code> <code>max_gen_seq_length</code> <code>int</code> <p>Maximum length of generated sequences.</p> <code>48</code> <code>repetition_penalty</code> <code>float</code> <p>Repetition penalty.</p> <code>1.0</code> <code>no_repeat_ngram_size</code> <code>int</code> <p>Size of n-grams to avoid repeating.</p> <code>0</code> <code>early_stopping</code> <code>bool</code> <p>Whether to stop generation early.</p> <code>True</code> <code>length_penalty</code> <code>float</code> <p>Length penalty for generated sequences.</p> <code>1.0</code> <code>num_beam_groups</code> <code>int</code> <p>Number of groups for diverse beam search.</p> <code>1</code> <code>diversity_penalty</code> <code>float</code> <p>Diversity penalty for diverse beam search.</p> <code>0.0</code> <code>do_sample</code> <code>bool</code> <p>Whether to use sampling for generation.</p> <code>False</code> <code>temperature</code> <code>float</code> <p>Sampling temperature.</p> <code>1.0</code> <code>top_k</code> <code>int</code> <p>Top-k sampling parameter.</p> <code>50</code> <code>top_p</code> <code>float</code> <p>Top-p sampling parameter.</p> <code>1.0</code> <p>Returns:</p> Name Type Description <code>GenerationOutputs</code> <p>The generated sequences and their scores.</p> Source code in <code>src/unitorch/cli/models/bart/modeling.py</code> <pre><code>@add_default_section_for_function(\"core/model/generation/bart\")\n@torch.no_grad()\n@autocast()\ndef generate(\n    self,\n    input_ids: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 2,\n    decoder_end_token_id: Optional[Union[int, List[int]]] = 2,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n):\n\"\"\"\n    Generate sequences using the BartForGeneration model.\n\n    Args:\n        input_ids (torch.Tensor): Input IDs.\n        num_beams (int, optional): Number of beams for beam search.\n        decoder_start_token_id (int, optional): ID of the decoder start token.\n        decoder_end_token_id (int or List[int], optional): ID of the decoder end token.\n        num_return_sequences (int, optional): Number of generated sequences to return.\n        min_gen_seq_length (int, optional): Minimum length of generated sequences.\n        max_gen_seq_length (int, optional): Maximum length of generated sequences.\n        repetition_penalty (float, optional): Repetition penalty.\n        no_repeat_ngram_size (int, optional): Size of n-grams to avoid repeating.\n        early_stopping (bool, optional): Whether to stop generation early.\n        length_penalty (float, optional): Length penalty for generated sequences.\n        num_beam_groups (int, optional): Number of groups for diverse beam search.\n        diversity_penalty (float, optional): Diversity penalty for diverse beam search.\n        do_sample (bool, optional): Whether to use sampling for generation.\n        temperature (float, optional): Sampling temperature.\n        top_k (int, optional): Top-k sampling parameter.\n        top_p (float, optional): Top-p sampling parameter.\n\n    Returns:\n        GenerationOutputs: The generated sequences and their scores.\n    \"\"\"\n    outputs = super().generate(\n        input_ids=input_ids,\n        num_beams=num_beams,\n        decoder_start_token_id=decoder_start_token_id,\n        decoder_end_token_id=decoder_end_token_id,\n        num_return_sequences=num_return_sequences,\n        min_gen_seq_length=min_gen_seq_length,\n        max_gen_seq_length=max_gen_seq_length,\n        repetition_penalty=repetition_penalty,\n        no_repeat_ngram_size=no_repeat_ngram_size,\n        early_stopping=early_stopping,\n        length_penalty=length_penalty,\n        num_beam_groups=num_beam_groups,\n        diversity_penalty=diversity_penalty,\n        do_sample=do_sample,\n        temperature=temperature,\n        top_k=top_k,\n        top_p=top_p,\n    )\n\n    return GenerationOutputs(\n        sequences=outputs.sequences,\n        sequences_scores=outputs.sequences_scores,\n    )\n</code></pre>",
             "title": "generate"
         },
         {
             "location": "cli/models/beit/",
             "text": "",
             "title": "unitorch.cli.models.beit"
         },
@@ -462,15 +462,15 @@
         {
             "location": "cli/models/blip/#unitorch.cli.models.blip.modeling.BlipForImageCaption.from_core_configure",
             "text": "<pre><code>from_core_configure(config, **kwargs)\n</code></pre> <p>Create an instance of BlipForImageCaption from a core configuration.</p> <p>Parameters:</p> Name Type Description Default <code>config</code> <p>The core configuration.</p> required <code>**kwargs</code> <p>Additional keyword arguments.</p> <code>{}</code> <p>Returns:</p> Name Type Description <code>BlipForImageCaption</code> <p>An instance of BlipForImageCaption.</p> Source code in <code>src/unitorch/cli/models/blip/modeling.py</code> <pre><code>@classmethod\n@add_default_section_for_init(\"core/model/caption/blip\")\ndef from_core_configure(cls, config, **kwargs):\n\"\"\"\n    Create an instance of BlipForImageCaption from a core configuration.\n\n    Args:\n        config: The core configuration.\n        **kwargs: Additional keyword arguments.\n\n    Returns:\n        BlipForImageCaption: An instance of BlipForImageCaption.\n    \"\"\"\n    config.set_default_section(\"core/model/caption/blip\")\n    pretrained_name = config.getoption(\"pretrained_name\", \"default-blip\")\n    config_path = config.getoption(\"config_path\", None)\n    config_path = pop_value(\n        config_path,\n        nested_dict_value(pretrained_blip_infos, pretrained_name, \"config\"),\n    )\n\n    config_path = cached_path(config_path)\n    gradient_checkpointing = config.getoption(\"gradient_checkpointing\", False)\n\n    inst = cls(\n        config_path=config_path,\n        gradient_checkpointing=gradient_checkpointing,\n    )\n    pretrained_weight_path = config.getoption(\"pretrained_weight_path\", None)\n    weight_path = pop_value(\n        pretrained_weight_path,\n        nested_dict_value(pretrained_blip_infos, pretrained_name, \"weight\"),\n        check_none=False,\n    )\n    if weight_path is not None:\n        weight_path = cached_path(weight_path)\n        inst.from_pretrained(weight_path)\n\n    return inst\n</code></pre>",
             "title": "from_core_configure  <code>classmethod</code>"
         },
         {
             "location": "cli/models/blip/#unitorch.cli.models.blip.modeling.BlipForImageCaption.generate",
-            "text": "<pre><code>generate(\n    pixel_values: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 101,\n    decoder_end_token_id: Optional[int] = 102,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n)\n</code></pre> <p>Generate captions using the BlipForImageCaption model.</p> <p>Parameters:</p> Name Type Description Default <code>pixel_values</code> <code>torch.Tensor</code> <p>The pixel values of the images.</p> required <code>num_beams</code> <code>int</code> <p>The number of beams for beam search. Defaults to 5.</p> <code>5</code> <code>decoder_start_token_id</code> <code>int</code> <p>The start token ID for the decoder. Defaults to 30522.</p> <code>101</code> <code>decoder_end_token_id</code> <code>int</code> <p>The end token ID for the decoder. Defaults to 2.</p> <code>102</code> <code>num_return_sequences</code> <code>int</code> <p>The number of sequences to return. Defaults to 1.</p> <code>1</code> <code>min_gen_seq_length</code> <code>int</code> <p>The minimum length of generated sequences. Defaults to 0.</p> <code>0</code> <code>max_gen_seq_length</code> <code>int</code> <p>The maximum length of generated sequences. Defaults to 48.</p> <code>48</code> <code>repetition_penalty</code> <code>float</code> <p>The repetition penalty. Defaults to 1.0.</p> <code>1.0</code> <code>no_repeat_ngram_size</code> <code>int</code> <p>The size of n-grams to avoid repeating. Defaults to 0.</p> <code>0</code> <code>early_stopping</code> <code>bool</code> <p>Whether to perform early stopping. Defaults to True.</p> <code>True</code> <code>length_penalty</code> <code>float</code> <p>The length penalty. Defaults to 1.0.</p> <code>1.0</code> <code>num_beam_groups</code> <code>int</code> <p>The number of beam groups. Defaults to 1.</p> <code>1</code> <code>diversity_penalty</code> <code>float</code> <p>The diversity penalty. Defaults to 0.0.</p> <code>0.0</code> <code>do_sample</code> <code>bool</code> <p>Whether to use sampling for generation. Defaults to False.</p> <code>False</code> <code>temperature</code> <code>float</code> <p>The temperature value for sampling. Defaults to 1.0.</p> <code>1.0</code> <code>top_k</code> <code>int</code> <p>The top-k value for sampling. Defaults to 50.</p> <code>50</code> <code>top_p</code> <code>float</code> <p>The top-p value for sampling. Defaults to 1.0.</p> <code>1.0</code> <p>Returns:</p> Name Type Description <code>GenerationOutputs</code> <p>The generation outputs.</p> Source code in <code>src/unitorch/cli/models/blip/modeling.py</code> <pre><code>@torch.no_grad()\n@autocast()\ndef generate(\n    self,\n    pixel_values: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 101,\n    decoder_end_token_id: Optional[int] = 102,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n):\n\"\"\"\n    Generate captions using the BlipForImageCaption model.\n\n    Args:\n        pixel_values (torch.Tensor): The pixel values of the images.\n        num_beams (int, optional): The number of beams for beam search. Defaults to 5.\n        decoder_start_token_id (int, optional): The start token ID for the decoder. Defaults to 30522.\n        decoder_end_token_id (int, optional): The end token ID for the decoder. Defaults to 2.\n        num_return_sequences (int, optional): The number of sequences to return. Defaults to 1.\n        min_gen_seq_length (int, optional): The minimum length of generated sequences. Defaults to 0.\n        max_gen_seq_length (int, optional): The maximum length of generated sequences. Defaults to 48.\n        repetition_penalty (float, optional): The repetition penalty. Defaults to 1.0.\n        no_repeat_ngram_size (int, optional): The size of n-grams to avoid repeating. Defaults to 0.\n        early_stopping (bool, optional): Whether to perform early stopping. Defaults to True.\n        length_penalty (float, optional): The length penalty. Defaults to 1.0.\n        num_beam_groups (int, optional): The number of beam groups. Defaults to 1.\n        diversity_penalty (float, optional): The diversity penalty. Defaults to 0.0.\n        do_sample (bool, optional): Whether to use sampling for generation. Defaults to False.\n        temperature (float, optional): The temperature value for sampling. Defaults to 1.0.\n        top_k (int, optional): The top-k value for sampling. Defaults to 50.\n        top_p (float, optional): The top-p value for sampling. Defaults to 1.0.\n\n    Returns:\n        GenerationOutputs: The generation outputs.\n    \"\"\"\n    outputs = super().generate(\n        pixel_values=pixel_values,\n        num_beams=num_beams,\n        decoder_start_token_id=decoder_start_token_id,\n        decoder_end_token_id=decoder_end_token_id,\n        num_return_sequences=num_return_sequences,\n        min_gen_seq_length=min_gen_seq_length,\n        max_gen_seq_length=max_gen_seq_length,\n        repetition_penalty=repetition_penalty,\n        no_repeat_ngram_size=no_repeat_ngram_size,\n        early_stopping=early_stopping,\n        length_penalty=length_penalty,\n        num_beam_groups=num_beam_groups,\n        diversity_penalty=diversity_penalty,\n        do_sample=do_sample,\n        temperature=temperature,\n        top_k=top_k,\n        top_p=top_p,\n    )\n\n    return GenerationOutputs(\n        sequences=outputs.sequences,\n        sequences_scores=outputs.sequences_scores,\n    )\n</code></pre>",
+            "text": "<pre><code>generate(\n    pixel_values: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 101,\n    decoder_end_token_id: Optional[\n        Union[int, List[int]]\n    ] = 102,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n)\n</code></pre> <p>Generate captions using the BlipForImageCaption model.</p> <p>Parameters:</p> Name Type Description Default <code>pixel_values</code> <code>torch.Tensor</code> <p>The pixel values of the images.</p> required <code>num_beams</code> <code>int</code> <p>The number of beams for beam search. Defaults to 5.</p> <code>5</code> <code>decoder_start_token_id</code> <code>int</code> <p>The start token ID for the decoder. Defaults to 30522.</p> <code>101</code> <code>decoder_end_token_id</code> <code>int or List[int]</code> <p>The end token ID for the decoder. Defaults to 2.</p> <code>102</code> <code>num_return_sequences</code> <code>int</code> <p>The number of sequences to return. Defaults to 1.</p> <code>1</code> <code>min_gen_seq_length</code> <code>int</code> <p>The minimum length of generated sequences. Defaults to 0.</p> <code>0</code> <code>max_gen_seq_length</code> <code>int</code> <p>The maximum length of generated sequences. Defaults to 48.</p> <code>48</code> <code>repetition_penalty</code> <code>float</code> <p>The repetition penalty. Defaults to 1.0.</p> <code>1.0</code> <code>no_repeat_ngram_size</code> <code>int</code> <p>The size of n-grams to avoid repeating. Defaults to 0.</p> <code>0</code> <code>early_stopping</code> <code>bool</code> <p>Whether to perform early stopping. Defaults to True.</p> <code>True</code> <code>length_penalty</code> <code>float</code> <p>The length penalty. Defaults to 1.0.</p> <code>1.0</code> <code>num_beam_groups</code> <code>int</code> <p>The number of beam groups. Defaults to 1.</p> <code>1</code> <code>diversity_penalty</code> <code>float</code> <p>The diversity penalty. Defaults to 0.0.</p> <code>0.0</code> <code>do_sample</code> <code>bool</code> <p>Whether to use sampling for generation. Defaults to False.</p> <code>False</code> <code>temperature</code> <code>float</code> <p>The temperature value for sampling. Defaults to 1.0.</p> <code>1.0</code> <code>top_k</code> <code>int</code> <p>The top-k value for sampling. Defaults to 50.</p> <code>50</code> <code>top_p</code> <code>float</code> <p>The top-p value for sampling. Defaults to 1.0.</p> <code>1.0</code> <p>Returns:</p> Name Type Description <code>GenerationOutputs</code> <p>The generation outputs.</p> Source code in <code>src/unitorch/cli/models/blip/modeling.py</code> <pre><code>@torch.no_grad()\n@autocast()\ndef generate(\n    self,\n    pixel_values: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 101,\n    decoder_end_token_id: Optional[Union[int, List[int]]] = 102,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n):\n\"\"\"\n    Generate captions using the BlipForImageCaption model.\n\n    Args:\n        pixel_values (torch.Tensor): The pixel values of the images.\n        num_beams (int, optional): The number of beams for beam search. Defaults to 5.\n        decoder_start_token_id (int, optional): The start token ID for the decoder. Defaults to 30522.\n        decoder_end_token_id (int or List[int], optional): The end token ID for the decoder. Defaults to 2.\n        num_return_sequences (int, optional): The number of sequences to return. Defaults to 1.\n        min_gen_seq_length (int, optional): The minimum length of generated sequences. Defaults to 0.\n        max_gen_seq_length (int, optional): The maximum length of generated sequences. Defaults to 48.\n        repetition_penalty (float, optional): The repetition penalty. Defaults to 1.0.\n        no_repeat_ngram_size (int, optional): The size of n-grams to avoid repeating. Defaults to 0.\n        early_stopping (bool, optional): Whether to perform early stopping. Defaults to True.\n        length_penalty (float, optional): The length penalty. Defaults to 1.0.\n        num_beam_groups (int, optional): The number of beam groups. Defaults to 1.\n        diversity_penalty (float, optional): The diversity penalty. Defaults to 0.0.\n        do_sample (bool, optional): Whether to use sampling for generation. Defaults to False.\n        temperature (float, optional): The temperature value for sampling. Defaults to 1.0.\n        top_k (int, optional): The top-k value for sampling. Defaults to 50.\n        top_p (float, optional): The top-p value for sampling. Defaults to 1.0.\n\n    Returns:\n        GenerationOutputs: The generation outputs.\n    \"\"\"\n    outputs = super().generate(\n        pixel_values=pixel_values,\n        num_beams=num_beams,\n        decoder_start_token_id=decoder_start_token_id,\n        decoder_end_token_id=decoder_end_token_id,\n        num_return_sequences=num_return_sequences,\n        min_gen_seq_length=min_gen_seq_length,\n        max_gen_seq_length=max_gen_seq_length,\n        repetition_penalty=repetition_penalty,\n        no_repeat_ngram_size=no_repeat_ngram_size,\n        early_stopping=early_stopping,\n        length_penalty=length_penalty,\n        num_beam_groups=num_beam_groups,\n        diversity_penalty=diversity_penalty,\n        do_sample=do_sample,\n        temperature=temperature,\n        top_k=top_k,\n        top_p=top_p,\n    )\n\n    return GenerationOutputs(\n        sequences=outputs.sequences,\n        sequences_scores=outputs.sequences_scores,\n    )\n</code></pre>",
             "title": "generate"
         },
         {
             "location": "cli/models/bloom/",
             "text": "",
             "title": "unitorch.cli.models.bloom"
         },
@@ -527,15 +527,15 @@
         {
             "location": "cli/models/bloom/#unitorch.cli.models.bloom.modeling.BloomForGeneration.from_core_configure",
             "text": "<pre><code>from_core_configure(config, **kwargs)\n</code></pre> <p>Create an instance of BloomForGeneration from the core configuration.</p> <p>Parameters:</p> Name Type Description Default <code>config</code> <code>Config</code> <p>The core configuration object.</p> required <p>Returns:</p> Name Type Description <code>BloomForGeneration</code> <p>An instance of BloomForGeneration initialized with the provided configuration.</p> Source code in <code>src/unitorch/cli/models/bloom/modeling.py</code> <pre><code>@classmethod\n@add_default_section_for_init(\"core/model/generation/bloom\")\ndef from_core_configure(cls, config, **kwargs):\n\"\"\"\n    Create an instance of BloomForGeneration from the core configuration.\n\n    Args:\n        config (Config): The core configuration object.\n\n    Returns:\n        BloomForGeneration: An instance of BloomForGeneration initialized with the provided configuration.\n    \"\"\"\n    config.set_default_section(\"core/model/generation/bloom\")\n    pretrained_name = config.getoption(\"pretrained_name\", \"default-bloom\")\n    config_path = config.getoption(\"config_path\", None)\n    config_path = pop_value(\n        config_path,\n        nested_dict_value(pretrained_bloom_infos, pretrained_name, \"config\"),\n    )\n\n    config_path = cached_path(config_path)\n    gradient_checkpointing = config.getoption(\"gradient_checkpointing\", False)\n\n    inst = cls(config_path, gradient_checkpointing)\n    pretrained_weight_path = config.getoption(\"pretrained_weight_path\", None)\n    weight_path = pop_value(\n        pretrained_weight_path,\n        nested_dict_value(pretrained_bloom_infos, pretrained_name, \"weight\"),\n        check_none=False,\n    )\n\n    if weight_path is not None:\n        inst.from_pretrained(weight_path)\n\n    return inst\n</code></pre>",
             "title": "from_core_configure  <code>classmethod</code>"
         },
         {
             "location": "cli/models/bloom/#unitorch.cli.models.bloom.modeling.BloomForGeneration.generate",
-            "text": "<pre><code>generate(\n    input_ids: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 1,\n    decoder_end_token_id: Optional[int] = 2,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n)\n</code></pre> <p>Generate sequences using the Bloom model.</p> <p>Parameters:</p> Name Type Description Default <code>input_ids</code> <code>torch.Tensor</code> <p>Input token IDs.</p> required <code>num_beams</code> <code>int</code> <p>Number of beams for beam search. Defaults to 5.</p> <code>5</code> <code>decoder_start_token_id</code> <code>int</code> <p>Decoder start token ID. Defaults to 0.</p> <code>1</code> <code>decoder_end_token_id</code> <code>int</code> <p>Decoder end token ID. Defaults to 1.</p> <code>2</code> <code>num_return_sequences</code> <code>int</code> <p>Number of generated sequences to return. Defaults to 1.</p> <code>1</code> <code>min_gen_seq_length</code> <code>int</code> <p>Minimum generation sequence length. Defaults to 0.</p> <code>0</code> <code>max_gen_seq_length</code> <code>int</code> <p>Maximum generation sequence length. Defaults to 48.</p> <code>48</code> <code>repetition_penalty</code> <code>float</code> <p>Repetition penalty. Defaults to 1.0.</p> <code>1.0</code> <code>no_repeat_ngram_size</code> <code>int</code> <p>Size of n-grams to prevent repetition. Defaults to 0.</p> <code>0</code> <code>early_stopping</code> <code>bool</code> <p>Whether to perform early stopping. Defaults to True.</p> <code>True</code> <code>length_penalty</code> <code>float</code> <p>Length penalty. Defaults to 1.0.</p> <code>1.0</code> <code>num_beam_groups</code> <code>int</code> <p>Number of beam groups for diverse beam search. Defaults to 1.</p> <code>1</code> <code>diversity_penalty</code> <code>float</code> <p>Diversity penalty for diverse beam search. Defaults to 0.0.</p> <code>0.0</code> <code>do_sample</code> <code>bool</code> <p>Whether to use sampling for generation. Defaults to False.</p> <code>False</code> <code>temperature</code> <code>float</code> <p>Sampling temperature. Defaults to 1.0.</p> <code>1.0</code> <code>top_k</code> <code>int</code> <p>Top-k sampling parameter. Defaults to 50.</p> <code>50</code> <code>top_p</code> <code>float</code> <p>Top-p sampling parameter. Defaults to 1.0.</p> <code>1.0</code> <p>Returns:</p> Name Type Description <code>GenerationOutputs</code> <p>The generation outputs.</p> Source code in <code>src/unitorch/cli/models/bloom/modeling.py</code> <pre><code>@add_default_section_for_function(\"core/model/generation/bloom\")\n@torch.no_grad()\n@autocast()\ndef generate(\n    self,\n    input_ids: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 1,\n    decoder_end_token_id: Optional[int] = 2,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n):\n\"\"\"\n    Generate sequences using the Bloom model.\n\n    Args:\n        input_ids (torch.Tensor): Input token IDs.\n        num_beams (int, optional): Number of beams for beam search. Defaults to 5.\n        decoder_start_token_id (int, optional): Decoder start token ID. Defaults to 0.\n        decoder_end_token_id (int, optional): Decoder end token ID. Defaults to 1.\n        num_return_sequences (int, optional): Number of generated sequences to return. Defaults to 1.\n        min_gen_seq_length (int, optional): Minimum generation sequence length. Defaults to 0.\n        max_gen_seq_length (int, optional): Maximum generation sequence length. Defaults to 48.\n        repetition_penalty (float, optional): Repetition penalty. Defaults to 1.0.\n        no_repeat_ngram_size (int, optional): Size of n-grams to prevent repetition. Defaults to 0.\n        early_stopping (bool, optional): Whether to perform early stopping. Defaults to True.\n        length_penalty (float, optional): Length penalty. Defaults to 1.0.\n        num_beam_groups (int, optional): Number of beam groups for diverse beam search. Defaults to 1.\n        diversity_penalty (float, optional): Diversity penalty for diverse beam search. Defaults to 0.0.\n        do_sample (bool, optional): Whether to use sampling for generation. Defaults to False.\n        temperature (float, optional): Sampling temperature. Defaults to 1.0.\n        top_k (int, optional): Top-k sampling parameter. Defaults to 50.\n        top_p (float, optional): Top-p sampling parameter. Defaults to 1.0.\n\n    Returns:\n        GenerationOutputs: The generation outputs.\n    \"\"\"\n    outputs = super().generate(\n        input_ids,\n        num_beams=num_beams,\n        decoder_start_token_id=decoder_start_token_id,\n        decoder_end_token_id=decoder_end_token_id,\n        num_return_sequences=num_return_sequences,\n        min_gen_seq_length=min_gen_seq_length,\n        max_gen_seq_length=max_gen_seq_length,\n        repetition_penalty=repetition_penalty,\n        no_repeat_ngram_size=no_repeat_ngram_size,\n        early_stopping=early_stopping,\n        length_penalty=length_penalty,\n        num_beam_groups=num_beam_groups,\n        diversity_penalty=diversity_penalty,\n        do_sample=do_sample,\n        temperature=temperature,\n        top_k=top_k,\n        top_p=top_p,\n    )\n\n    return GenerationOutputs(\n        sequences=outputs.sequences,\n        sequences_scores=outputs.sequences_scores,\n    )\n</code></pre>",
+            "text": "<pre><code>generate(\n    input_ids: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 1,\n    decoder_end_token_id: Optional[\n        Union[int, List[int]]\n    ] = 2,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n)\n</code></pre> <p>Generate sequences using the Bloom model.</p> <p>Parameters:</p> Name Type Description Default <code>input_ids</code> <code>torch.Tensor</code> <p>Input token IDs.</p> required <code>num_beams</code> <code>int</code> <p>Number of beams for beam search. Defaults to 5.</p> <code>5</code> <code>decoder_start_token_id</code> <code>int</code> <p>Decoder start token ID. Defaults to 0.</p> <code>1</code> <code>decoder_end_token_id</code> <code>int or List[int]</code> <p>The ID(s) of the decoder end token(s). Defaults to 1.</p> <code>2</code> <code>num_return_sequences</code> <code>int</code> <p>Number of generated sequences to return. Defaults to 1.</p> <code>1</code> <code>min_gen_seq_length</code> <code>int</code> <p>Minimum generation sequence length. Defaults to 0.</p> <code>0</code> <code>max_gen_seq_length</code> <code>int</code> <p>Maximum generation sequence length. Defaults to 48.</p> <code>48</code> <code>repetition_penalty</code> <code>float</code> <p>Repetition penalty. Defaults to 1.0.</p> <code>1.0</code> <code>no_repeat_ngram_size</code> <code>int</code> <p>Size of n-grams to prevent repetition. Defaults to 0.</p> <code>0</code> <code>early_stopping</code> <code>bool</code> <p>Whether to perform early stopping. Defaults to True.</p> <code>True</code> <code>length_penalty</code> <code>float</code> <p>Length penalty. Defaults to 1.0.</p> <code>1.0</code> <code>num_beam_groups</code> <code>int</code> <p>Number of beam groups for diverse beam search. Defaults to 1.</p> <code>1</code> <code>diversity_penalty</code> <code>float</code> <p>Diversity penalty for diverse beam search. Defaults to 0.0.</p> <code>0.0</code> <code>do_sample</code> <code>bool</code> <p>Whether to use sampling for generation. Defaults to False.</p> <code>False</code> <code>temperature</code> <code>float</code> <p>Sampling temperature. Defaults to 1.0.</p> <code>1.0</code> <code>top_k</code> <code>int</code> <p>Top-k sampling parameter. Defaults to 50.</p> <code>50</code> <code>top_p</code> <code>float</code> <p>Top-p sampling parameter. Defaults to 1.0.</p> <code>1.0</code> <p>Returns:</p> Name Type Description <code>GenerationOutputs</code> <p>The generation outputs.</p> Source code in <code>src/unitorch/cli/models/bloom/modeling.py</code> <pre><code>@add_default_section_for_function(\"core/model/generation/bloom\")\n@torch.no_grad()\n@autocast()\ndef generate(\n    self,\n    input_ids: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 1,\n    decoder_end_token_id: Optional[Union[int, List[int]]] = 2,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n):\n\"\"\"\n    Generate sequences using the Bloom model.\n\n    Args:\n        input_ids (torch.Tensor): Input token IDs.\n        num_beams (int, optional): Number of beams for beam search. Defaults to 5.\n        decoder_start_token_id (int, optional): Decoder start token ID. Defaults to 0.\n        decoder_end_token_id (int or List[int], optional): The ID(s) of the decoder end token(s). Defaults to 1.\n        num_return_sequences (int, optional): Number of generated sequences to return. Defaults to 1.\n        min_gen_seq_length (int, optional): Minimum generation sequence length. Defaults to 0.\n        max_gen_seq_length (int, optional): Maximum generation sequence length. Defaults to 48.\n        repetition_penalty (float, optional): Repetition penalty. Defaults to 1.0.\n        no_repeat_ngram_size (int, optional): Size of n-grams to prevent repetition. Defaults to 0.\n        early_stopping (bool, optional): Whether to perform early stopping. Defaults to True.\n        length_penalty (float, optional): Length penalty. Defaults to 1.0.\n        num_beam_groups (int, optional): Number of beam groups for diverse beam search. Defaults to 1.\n        diversity_penalty (float, optional): Diversity penalty for diverse beam search. Defaults to 0.0.\n        do_sample (bool, optional): Whether to use sampling for generation. Defaults to False.\n        temperature (float, optional): Sampling temperature. Defaults to 1.0.\n        top_k (int, optional): Top-k sampling parameter. Defaults to 50.\n        top_p (float, optional): Top-p sampling parameter. Defaults to 1.0.\n\n    Returns:\n        GenerationOutputs: The generation outputs.\n    \"\"\"\n    outputs = super().generate(\n        input_ids,\n        num_beams=num_beams,\n        decoder_start_token_id=decoder_start_token_id,\n        decoder_end_token_id=decoder_end_token_id,\n        num_return_sequences=num_return_sequences,\n        min_gen_seq_length=min_gen_seq_length,\n        max_gen_seq_length=max_gen_seq_length,\n        repetition_penalty=repetition_penalty,\n        no_repeat_ngram_size=no_repeat_ngram_size,\n        early_stopping=early_stopping,\n        length_penalty=length_penalty,\n        num_beam_groups=num_beam_groups,\n        diversity_penalty=diversity_penalty,\n        do_sample=do_sample,\n        temperature=temperature,\n        top_k=top_k,\n        top_p=top_p,\n    )\n\n    return GenerationOutputs(\n        sequences=outputs.sequences,\n        sequences_scores=outputs.sequences_scores,\n    )\n</code></pre>",
             "title": "generate"
         },
         {
             "location": "cli/models/chatglm/",
             "text": "",
             "title": "unitorch.cli.models.chatglm"
         },
@@ -592,15 +592,15 @@
         {
             "location": "cli/models/chatglm/#unitorch.cli.models.chatglm.modeling.ChatGLMForGeneration.from_core_configure",
             "text": "<pre><code>from_core_configure(config, **kwargs)\n</code></pre> <p>Create an instance of ChatGLMForGeneration from the core configuration.</p> <p>Parameters:</p> Name Type Description Default <code>config</code> <code>Config</code> <p>The core configuration object.</p> required <p>Returns:</p> Name Type Description <code>ChatGLMForGeneration</code> <p>An instance of ChatGLMForGeneration initialized with the provided configuration.</p> Source code in <code>src/unitorch/cli/models/chatglm/modeling.py</code> <pre><code>@classmethod\n@add_default_section_for_init(\"core/model/generation/chatglm\")\ndef from_core_configure(cls, config, **kwargs):\n\"\"\"\n    Create an instance of ChatGLMForGeneration from the core configuration.\n\n    Args:\n        config (Config): The core configuration object.\n\n    Returns:\n        ChatGLMForGeneration: An instance of ChatGLMForGeneration initialized with the provided configuration.\n    \"\"\"\n    config.set_default_section(\"core/model/generation/chatglm\")\n    pretrained_name = config.getoption(\"pretrained_name\", \"default-chatglm\")\n    config_path = config.getoption(\"config_path\", None)\n    config_path = pop_value(\n        config_path,\n        nested_dict_value(pretrained_chatglm_infos, pretrained_name, \"config\"),\n    )\n\n    config_path = cached_path(config_path)\n    gradient_checkpointing = config.getoption(\"gradient_checkpointing\", False)\n\n    inst = cls(config_path, gradient_checkpointing)\n    pretrained_weight_path = config.getoption(\"pretrained_weight_path\", None)\n    weight_path = pop_value(\n        pretrained_weight_path,\n        nested_dict_value(pretrained_chatglm_infos, pretrained_name, \"weight\"),\n        check_none=False,\n    )\n    if weight_path is not None:\n        inst.from_pretrained(\n            weight_path=weight_path,\n        )\n\n    return inst\n</code></pre>",
             "title": "from_core_configure  <code>classmethod</code>"
         },
         {
             "location": "cli/models/chatglm/#unitorch.cli.models.chatglm.modeling.ChatGLMForGeneration.generate",
-            "text": "<pre><code>generate(\n    input_ids: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 2,\n    decoder_end_token_id: Optional[int] = 2,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n)\n</code></pre> <p>Generate sequences using the ChatGLM model.</p> <p>Parameters:</p> Name Type Description Default <code>input_ids</code> <code>torch.Tensor</code> <p>Input token IDs.</p> required <code>num_beams</code> <code>int</code> <p>Number of beams for beam search. Defaults to 5.</p> <code>5</code> <code>decoder_start_token_id</code> <code>int</code> <p>Decoder start token ID. Defaults to 0.</p> <code>2</code> <code>decoder_end_token_id</code> <code>int</code> <p>Decoder end token ID. Defaults to 1.</p> <code>2</code> <code>num_return_sequences</code> <code>int</code> <p>Number of generated sequences to return. Defaults to 1.</p> <code>1</code> <code>min_gen_seq_length</code> <code>int</code> <p>Minimum generation sequence length. Defaults to 0.</p> <code>0</code> <code>max_gen_seq_length</code> <code>int</code> <p>Maximum generation sequence length. Defaults to 48.</p> <code>48</code> <code>repetition_penalty</code> <code>float</code> <p>Repetition penalty. Defaults to 1.0.</p> <code>1.0</code> <code>no_repeat_ngram_size</code> <code>int</code> <p>Size of n-grams to prevent repetition. Defaults to 0.</p> <code>0</code> <code>early_stopping</code> <code>bool</code> <p>Whether to perform early stopping. Defaults to True.</p> <code>True</code> <code>length_penalty</code> <code>float</code> <p>Length penalty. Defaults to 1.0.</p> <code>1.0</code> <code>num_beam_groups</code> <code>int</code> <p>Number of beam groups for diverse beam search. Defaults to 1.</p> <code>1</code> <code>diversity_penalty</code> <code>float</code> <p>Diversity penalty for diverse beam search. Defaults to 0.0.</p> <code>0.0</code> <code>do_sample</code> <code>bool</code> <p>Whether to use sampling for generation. Defaults to False.</p> <code>False</code> <code>temperature</code> <code>float</code> <p>Sampling temperature. Defaults to 1.0.</p> <code>1.0</code> <code>top_k</code> <code>int</code> <p>Top-k sampling parameter. Defaults to 50.</p> <code>50</code> <code>top_p</code> <code>float</code> <p>Top-p sampling parameter. Defaults to 1.0.</p> <code>1.0</code> <p>Returns:</p> Name Type Description <code>GenerationOutputs</code> <p>The generation outputs.</p> Source code in <code>src/unitorch/cli/models/chatglm/modeling.py</code> <pre><code>@add_default_section_for_function(\"core/model/generation/chatglm\")\n@torch.no_grad()\n@autocast()\ndef generate(\n    self,\n    input_ids: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 2,\n    decoder_end_token_id: Optional[int] = 2,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n):\n\"\"\"\n    Generate sequences using the ChatGLM model.\n\n    Args:\n        input_ids (torch.Tensor): Input token IDs.\n        num_beams (int, optional): Number of beams for beam search. Defaults to 5.\n        decoder_start_token_id (int, optional): Decoder start token ID. Defaults to 0.\n        decoder_end_token_id (int, optional): Decoder end token ID. Defaults to 1.\n        num_return_sequences (int, optional): Number of generated sequences to return. Defaults to 1.\n        min_gen_seq_length (int, optional): Minimum generation sequence length. Defaults to 0.\n        max_gen_seq_length (int, optional): Maximum generation sequence length. Defaults to 48.\n        repetition_penalty (float, optional): Repetition penalty. Defaults to 1.0.\n        no_repeat_ngram_size (int, optional): Size of n-grams to prevent repetition. Defaults to 0.\n        early_stopping (bool, optional): Whether to perform early stopping. Defaults to True.\n        length_penalty (float, optional): Length penalty. Defaults to 1.0.\n        num_beam_groups (int, optional): Number of beam groups for diverse beam search. Defaults to 1.\n        diversity_penalty (float, optional): Diversity penalty for diverse beam search. Defaults to 0.0.\n        do_sample (bool, optional): Whether to use sampling for generation. Defaults to False.\n        temperature (float, optional): Sampling temperature. Defaults to 1.0.\n        top_k (int, optional): Top-k sampling parameter. Defaults to 50.\n        top_p (float, optional): Top-p sampling parameter. Defaults to 1.0.\n\n    Returns:\n        GenerationOutputs: The generation outputs.\n    \"\"\"\n    outputs = super().generate(\n        input_ids,\n        num_beams=num_beams,\n        decoder_start_token_id=decoder_start_token_id,\n        decoder_end_token_id=decoder_end_token_id,\n        num_return_sequences=num_return_sequences,\n        min_gen_seq_length=min_gen_seq_length,\n        max_gen_seq_length=max_gen_seq_length,\n        repetition_penalty=repetition_penalty,\n        no_repeat_ngram_size=no_repeat_ngram_size,\n        early_stopping=early_stopping,\n        length_penalty=length_penalty,\n        num_beam_groups=num_beam_groups,\n        diversity_penalty=diversity_penalty,\n        do_sample=do_sample,\n        temperature=temperature,\n        top_k=top_k,\n        top_p=top_p,\n    )\n\n    return GenerationOutputs(\n        sequences=outputs.sequences,\n        sequences_scores=outputs.sequences_scores,\n    )\n</code></pre>",
+            "text": "<pre><code>generate(\n    input_ids: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 2,\n    decoder_end_token_id: Optional[\n        Union[int, List[int]]\n    ] = 2,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n)\n</code></pre> <p>Generate sequences using the ChatGLM model.</p> <p>Parameters:</p> Name Type Description Default <code>input_ids</code> <code>torch.Tensor</code> <p>Input token IDs.</p> required <code>num_beams</code> <code>int</code> <p>Number of beams for beam search. Defaults to 5.</p> <code>5</code> <code>decoder_start_token_id</code> <code>int</code> <p>Decoder start token ID. Defaults to 0.</p> <code>2</code> <code>decoder_end_token_id</code> <code>int or List[int]</code> <p>The ID(s) of the decoder end token(s). Defaults to 1.</p> <code>2</code> <code>num_return_sequences</code> <code>int</code> <p>Number of generated sequences to return. Defaults to 1.</p> <code>1</code> <code>min_gen_seq_length</code> <code>int</code> <p>Minimum generation sequence length. Defaults to 0.</p> <code>0</code> <code>max_gen_seq_length</code> <code>int</code> <p>Maximum generation sequence length. Defaults to 48.</p> <code>48</code> <code>repetition_penalty</code> <code>float</code> <p>Repetition penalty. Defaults to 1.0.</p> <code>1.0</code> <code>no_repeat_ngram_size</code> <code>int</code> <p>Size of n-grams to prevent repetition. Defaults to 0.</p> <code>0</code> <code>early_stopping</code> <code>bool</code> <p>Whether to perform early stopping. Defaults to True.</p> <code>True</code> <code>length_penalty</code> <code>float</code> <p>Length penalty. Defaults to 1.0.</p> <code>1.0</code> <code>num_beam_groups</code> <code>int</code> <p>Number of beam groups for diverse beam search. Defaults to 1.</p> <code>1</code> <code>diversity_penalty</code> <code>float</code> <p>Diversity penalty for diverse beam search. Defaults to 0.0.</p> <code>0.0</code> <code>do_sample</code> <code>bool</code> <p>Whether to use sampling for generation. Defaults to False.</p> <code>False</code> <code>temperature</code> <code>float</code> <p>Sampling temperature. Defaults to 1.0.</p> <code>1.0</code> <code>top_k</code> <code>int</code> <p>Top-k sampling parameter. Defaults to 50.</p> <code>50</code> <code>top_p</code> <code>float</code> <p>Top-p sampling parameter. Defaults to 1.0.</p> <code>1.0</code> <p>Returns:</p> Name Type Description <code>GenerationOutputs</code> <p>The generation outputs.</p> Source code in <code>src/unitorch/cli/models/chatglm/modeling.py</code> <pre><code>@add_default_section_for_function(\"core/model/generation/chatglm\")\n@torch.no_grad()\n@autocast()\ndef generate(\n    self,\n    input_ids: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 2,\n    decoder_end_token_id: Optional[Union[int, List[int]]] = 2,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n):\n\"\"\"\n    Generate sequences using the ChatGLM model.\n\n    Args:\n        input_ids (torch.Tensor): Input token IDs.\n        num_beams (int, optional): Number of beams for beam search. Defaults to 5.\n        decoder_start_token_id (int, optional): Decoder start token ID. Defaults to 0.\n        decoder_end_token_id (int or List[int], optional): The ID(s) of the decoder end token(s). Defaults to 1.\n        num_return_sequences (int, optional): Number of generated sequences to return. Defaults to 1.\n        min_gen_seq_length (int, optional): Minimum generation sequence length. Defaults to 0.\n        max_gen_seq_length (int, optional): Maximum generation sequence length. Defaults to 48.\n        repetition_penalty (float, optional): Repetition penalty. Defaults to 1.0.\n        no_repeat_ngram_size (int, optional): Size of n-grams to prevent repetition. Defaults to 0.\n        early_stopping (bool, optional): Whether to perform early stopping. Defaults to True.\n        length_penalty (float, optional): Length penalty. Defaults to 1.0.\n        num_beam_groups (int, optional): Number of beam groups for diverse beam search. Defaults to 1.\n        diversity_penalty (float, optional): Diversity penalty for diverse beam search. Defaults to 0.0.\n        do_sample (bool, optional): Whether to use sampling for generation. Defaults to False.\n        temperature (float, optional): Sampling temperature. Defaults to 1.0.\n        top_k (int, optional): Top-k sampling parameter. Defaults to 50.\n        top_p (float, optional): Top-p sampling parameter. Defaults to 1.0.\n\n    Returns:\n        GenerationOutputs: The generation outputs.\n    \"\"\"\n    outputs = super().generate(\n        input_ids,\n        num_beams=num_beams,\n        decoder_start_token_id=decoder_start_token_id,\n        decoder_end_token_id=decoder_end_token_id,\n        num_return_sequences=num_return_sequences,\n        min_gen_seq_length=min_gen_seq_length,\n        max_gen_seq_length=max_gen_seq_length,\n        repetition_penalty=repetition_penalty,\n        no_repeat_ngram_size=no_repeat_ngram_size,\n        early_stopping=early_stopping,\n        length_penalty=length_penalty,\n        num_beam_groups=num_beam_groups,\n        diversity_penalty=diversity_penalty,\n        do_sample=do_sample,\n        temperature=temperature,\n        top_k=top_k,\n        top_p=top_p,\n    )\n\n    return GenerationOutputs(\n        sequences=outputs.sequences,\n        sequences_scores=outputs.sequences_scores,\n    )\n</code></pre>",
             "title": "generate"
         },
         {
             "location": "cli/models/clip/",
             "text": "",
             "title": "unitorch.cli.models.clip"
         },
@@ -757,15 +757,15 @@
         {
             "location": "cli/models/diffusers/#unitorch.cli.models.bart.modeling.BartForGeneration.from_core_configure",
             "text": "<pre><code>from_core_configure(config, **kwargs)\n</code></pre> <p>Create an instance of BartForGeneration from core configuration.</p> <p>Parameters:</p> Name Type Description Default <code>config</code> <p>The core configuration object.</p> required <code>**kwargs</code> <p>Additional keyword arguments.</p> <code>{}</code> <p>Returns:</p> Name Type Description <code>BartForGeneration</code> <p>The initialized BartForGeneration instance.</p> Source code in <code>src/unitorch/cli/models/bart/modeling.py</code> <pre><code>@classmethod\n@add_default_section_for_init(\"core/model/generation/bart\")\ndef from_core_configure(cls, config, **kwargs):\n\"\"\"\n    Create an instance of BartForGeneration from core configuration.\n\n    Args:\n        config: The core configuration object.\n        **kwargs: Additional keyword arguments.\n\n    Returns:\n        BartForGeneration: The initialized BartForGeneration instance.\n    \"\"\"\n    config.set_default_section(\"core/model/generation/bart\")\n    pretrained_name = config.getoption(\"pretrained_name\", \"default-bart\")\n    config_path = config.getoption(\"config_path\", None)\n    config_path = pop_value(\n        config_path,\n        nested_dict_value(pretrained_bart_infos, pretrained_name, \"config\"),\n    )\n\n    config_path = cached_path(config_path)\n    gradient_checkpointing = config.getoption(\"gradient_checkpointing\", False)\n\n    inst = cls(config_path, gradient_checkpointing)\n    pretrained_weight_path = config.getoption(\"pretrained_weight_path\", None)\n    weight_path = pop_value(\n        pretrained_weight_path,\n        nested_dict_value(pretrained_bart_infos, pretrained_name, \"weight\"),\n        check_none=False,\n    )\n    if weight_path is not None:\n        weight_path = cached_path(weight_path)\n        inst.from_pretrained(weight_path)\n\n    return inst\n</code></pre>",
             "title": "from_core_configure  <code>classmethod</code>"
         },
         {
             "location": "cli/models/diffusers/#unitorch.cli.models.bart.modeling.BartForGeneration.generate",
-            "text": "<pre><code>generate(\n    input_ids: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 2,\n    decoder_end_token_id: Optional[int] = 2,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n)\n</code></pre> <p>Generate sequences using the BartForGeneration model.</p> <p>Parameters:</p> Name Type Description Default <code>input_ids</code> <code>torch.Tensor</code> <p>Input IDs.</p> required <code>num_beams</code> <code>int</code> <p>Number of beams for beam search.</p> <code>5</code> <code>decoder_start_token_id</code> <code>int</code> <p>ID of the decoder start token.</p> <code>2</code> <code>decoder_end_token_id</code> <code>int</code> <p>ID of the decoder end token.</p> <code>2</code> <code>num_return_sequences</code> <code>int</code> <p>Number of generated sequences to return.</p> <code>1</code> <code>min_gen_seq_length</code> <code>int</code> <p>Minimum length of generated sequences.</p> <code>0</code> <code>max_gen_seq_length</code> <code>int</code> <p>Maximum length of generated sequences.</p> <code>48</code> <code>repetition_penalty</code> <code>float</code> <p>Repetition penalty.</p> <code>1.0</code> <code>no_repeat_ngram_size</code> <code>int</code> <p>Size of n-grams to avoid repeating.</p> <code>0</code> <code>early_stopping</code> <code>bool</code> <p>Whether to stop generation early.</p> <code>True</code> <code>length_penalty</code> <code>float</code> <p>Length penalty for generated sequences.</p> <code>1.0</code> <code>num_beam_groups</code> <code>int</code> <p>Number of groups for diverse beam search.</p> <code>1</code> <code>diversity_penalty</code> <code>float</code> <p>Diversity penalty for diverse beam search.</p> <code>0.0</code> <code>do_sample</code> <code>bool</code> <p>Whether to use sampling for generation.</p> <code>False</code> <code>temperature</code> <code>float</code> <p>Sampling temperature.</p> <code>1.0</code> <code>top_k</code> <code>int</code> <p>Top-k sampling parameter.</p> <code>50</code> <code>top_p</code> <code>float</code> <p>Top-p sampling parameter.</p> <code>1.0</code> <p>Returns:</p> Name Type Description <code>GenerationOutputs</code> <p>The generated sequences and their scores.</p> Source code in <code>src/unitorch/cli/models/bart/modeling.py</code> <pre><code>@add_default_section_for_function(\"core/model/generation/bart\")\n@torch.no_grad()\n@autocast()\ndef generate(\n    self,\n    input_ids: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 2,\n    decoder_end_token_id: Optional[int] = 2,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n):\n\"\"\"\n    Generate sequences using the BartForGeneration model.\n\n    Args:\n        input_ids (torch.Tensor): Input IDs.\n        num_beams (int, optional): Number of beams for beam search.\n        decoder_start_token_id (int, optional): ID of the decoder start token.\n        decoder_end_token_id (int, optional): ID of the decoder end token.\n        num_return_sequences (int, optional): Number of generated sequences to return.\n        min_gen_seq_length (int, optional): Minimum length of generated sequences.\n        max_gen_seq_length (int, optional): Maximum length of generated sequences.\n        repetition_penalty (float, optional): Repetition penalty.\n        no_repeat_ngram_size (int, optional): Size of n-grams to avoid repeating.\n        early_stopping (bool, optional): Whether to stop generation early.\n        length_penalty (float, optional): Length penalty for generated sequences.\n        num_beam_groups (int, optional): Number of groups for diverse beam search.\n        diversity_penalty (float, optional): Diversity penalty for diverse beam search.\n        do_sample (bool, optional): Whether to use sampling for generation.\n        temperature (float, optional): Sampling temperature.\n        top_k (int, optional): Top-k sampling parameter.\n        top_p (float, optional): Top-p sampling parameter.\n\n    Returns:\n        GenerationOutputs: The generated sequences and their scores.\n    \"\"\"\n    outputs = super().generate(\n        input_ids=input_ids,\n        num_beams=num_beams,\n        decoder_start_token_id=decoder_start_token_id,\n        decoder_end_token_id=decoder_end_token_id,\n        num_return_sequences=num_return_sequences,\n        min_gen_seq_length=min_gen_seq_length,\n        max_gen_seq_length=max_gen_seq_length,\n        repetition_penalty=repetition_penalty,\n        no_repeat_ngram_size=no_repeat_ngram_size,\n        early_stopping=early_stopping,\n        length_penalty=length_penalty,\n        num_beam_groups=num_beam_groups,\n        diversity_penalty=diversity_penalty,\n        do_sample=do_sample,\n        temperature=temperature,\n        top_k=top_k,\n        top_p=top_p,\n    )\n\n    return GenerationOutputs(\n        sequences=outputs.sequences,\n        sequences_scores=outputs.sequences_scores,\n    )\n</code></pre>",
+            "text": "<pre><code>generate(\n    input_ids: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 2,\n    decoder_end_token_id: Optional[\n        Union[int, List[int]]\n    ] = 2,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n)\n</code></pre> <p>Generate sequences using the BartForGeneration model.</p> <p>Parameters:</p> Name Type Description Default <code>input_ids</code> <code>torch.Tensor</code> <p>Input IDs.</p> required <code>num_beams</code> <code>int</code> <p>Number of beams for beam search.</p> <code>5</code> <code>decoder_start_token_id</code> <code>int</code> <p>ID of the decoder start token.</p> <code>2</code> <code>decoder_end_token_id</code> <code>int or List[int]</code> <p>ID of the decoder end token.</p> <code>2</code> <code>num_return_sequences</code> <code>int</code> <p>Number of generated sequences to return.</p> <code>1</code> <code>min_gen_seq_length</code> <code>int</code> <p>Minimum length of generated sequences.</p> <code>0</code> <code>max_gen_seq_length</code> <code>int</code> <p>Maximum length of generated sequences.</p> <code>48</code> <code>repetition_penalty</code> <code>float</code> <p>Repetition penalty.</p> <code>1.0</code> <code>no_repeat_ngram_size</code> <code>int</code> <p>Size of n-grams to avoid repeating.</p> <code>0</code> <code>early_stopping</code> <code>bool</code> <p>Whether to stop generation early.</p> <code>True</code> <code>length_penalty</code> <code>float</code> <p>Length penalty for generated sequences.</p> <code>1.0</code> <code>num_beam_groups</code> <code>int</code> <p>Number of groups for diverse beam search.</p> <code>1</code> <code>diversity_penalty</code> <code>float</code> <p>Diversity penalty for diverse beam search.</p> <code>0.0</code> <code>do_sample</code> <code>bool</code> <p>Whether to use sampling for generation.</p> <code>False</code> <code>temperature</code> <code>float</code> <p>Sampling temperature.</p> <code>1.0</code> <code>top_k</code> <code>int</code> <p>Top-k sampling parameter.</p> <code>50</code> <code>top_p</code> <code>float</code> <p>Top-p sampling parameter.</p> <code>1.0</code> <p>Returns:</p> Name Type Description <code>GenerationOutputs</code> <p>The generated sequences and their scores.</p> Source code in <code>src/unitorch/cli/models/bart/modeling.py</code> <pre><code>@add_default_section_for_function(\"core/model/generation/bart\")\n@torch.no_grad()\n@autocast()\ndef generate(\n    self,\n    input_ids: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 2,\n    decoder_end_token_id: Optional[Union[int, List[int]]] = 2,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n):\n\"\"\"\n    Generate sequences using the BartForGeneration model.\n\n    Args:\n        input_ids (torch.Tensor): Input IDs.\n        num_beams (int, optional): Number of beams for beam search.\n        decoder_start_token_id (int, optional): ID of the decoder start token.\n        decoder_end_token_id (int or List[int], optional): ID of the decoder end token.\n        num_return_sequences (int, optional): Number of generated sequences to return.\n        min_gen_seq_length (int, optional): Minimum length of generated sequences.\n        max_gen_seq_length (int, optional): Maximum length of generated sequences.\n        repetition_penalty (float, optional): Repetition penalty.\n        no_repeat_ngram_size (int, optional): Size of n-grams to avoid repeating.\n        early_stopping (bool, optional): Whether to stop generation early.\n        length_penalty (float, optional): Length penalty for generated sequences.\n        num_beam_groups (int, optional): Number of groups for diverse beam search.\n        diversity_penalty (float, optional): Diversity penalty for diverse beam search.\n        do_sample (bool, optional): Whether to use sampling for generation.\n        temperature (float, optional): Sampling temperature.\n        top_k (int, optional): Top-k sampling parameter.\n        top_p (float, optional): Top-p sampling parameter.\n\n    Returns:\n        GenerationOutputs: The generated sequences and their scores.\n    \"\"\"\n    outputs = super().generate(\n        input_ids=input_ids,\n        num_beams=num_beams,\n        decoder_start_token_id=decoder_start_token_id,\n        decoder_end_token_id=decoder_end_token_id,\n        num_return_sequences=num_return_sequences,\n        min_gen_seq_length=min_gen_seq_length,\n        max_gen_seq_length=max_gen_seq_length,\n        repetition_penalty=repetition_penalty,\n        no_repeat_ngram_size=no_repeat_ngram_size,\n        early_stopping=early_stopping,\n        length_penalty=length_penalty,\n        num_beam_groups=num_beam_groups,\n        diversity_penalty=diversity_penalty,\n        do_sample=do_sample,\n        temperature=temperature,\n        top_k=top_k,\n        top_p=top_p,\n    )\n\n    return GenerationOutputs(\n        sequences=outputs.sequences,\n        sequences_scores=outputs.sequences_scores,\n    )\n</code></pre>",
             "title": "generate"
         },
         {
             "location": "cli/models/llama/",
             "text": "",
             "title": "unitorch.cli.models.llama"
         },
@@ -822,15 +822,15 @@
         {
             "location": "cli/models/llama/#unitorch.cli.models.llama.modeling.LlamaForGeneration.from_core_configure",
             "text": "<pre><code>from_core_configure(config, **kwargs)\n</code></pre> <p>Create an instance of LlamaForGeneration from a core configuration.</p> <p>Parameters:</p> Name Type Description Default <code>config</code> <p>The core configuration.</p> required <code>**kwargs</code> <p>Additional keyword arguments.</p> <code>{}</code> <p>Returns:</p> Name Type Description <code>LlamaForGeneration</code> <p>An instance of LlamaForGeneration.</p> Source code in <code>src/unitorch/cli/models/llama/modeling.py</code> <pre><code>@classmethod\n@add_default_section_for_init(\"core/model/generation/llama\")\ndef from_core_configure(cls, config, **kwargs):\n\"\"\"\n    Create an instance of LlamaForGeneration from a core configuration.\n\n    Args:\n        config: The core configuration.\n        **kwargs: Additional keyword arguments.\n\n    Returns:\n        LlamaForGeneration: An instance of LlamaForGeneration.\n    \"\"\"\n    config.set_default_section(\"core/model/generation/llama\")\n    pretrained_name = config.getoption(\"pretrained_name\", \"default-llama\")\n    config_path = config.getoption(\"config_path\", None)\n    config_path = pop_value(\n        config_path,\n        nested_dict_value(pretrained_llama_infos, pretrained_name, \"config\"),\n    )\n\n    config_path = cached_path(config_path)\n    gradient_checkpointing = config.getoption(\"gradient_checkpointing\", False)\n\n    inst = cls(config_path, gradient_checkpointing)\n    pretrained_weight_path = config.getoption(\"pretrained_weight_path\", None)\n    weight_path = pop_value(\n        pretrained_weight_path,\n        nested_dict_value(pretrained_llama_infos, pretrained_name, \"weight\"),\n        check_none=False,\n    )\n\n    if weight_path is not None:\n        inst.from_pretrained(\n            weight_path=weight_path,\n        )\n\n    return inst\n</code></pre>",
             "title": "from_core_configure  <code>classmethod</code>"
         },
         {
             "location": "cli/models/llama/#unitorch.cli.models.llama.modeling.LlamaForGeneration.generate",
-            "text": "<pre><code>generate(\n    input_ids: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 1,\n    decoder_end_token_id: Optional[int] = 2,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n)\n</code></pre> <p>Generate sequences using the Llama model.</p> <p>Parameters:</p> Name Type Description Default <code>input_ids</code> <code>torch.Tensor</code> <p>Input token IDs.</p> required <code>num_beams</code> <code>int</code> <p>Number of beams for beam search. Defaults to 5.</p> <code>5</code> <code>decoder_start_token_id</code> <code>int</code> <p>Decoder start token ID. Defaults to 0.</p> <code>1</code> <code>decoder_end_token_id</code> <code>int</code> <p>Decoder end token ID. Defaults to 1.</p> <code>2</code> <code>num_return_sequences</code> <code>int</code> <p>Number of generated sequences to return. Defaults to 1.</p> <code>1</code> <code>min_gen_seq_length</code> <code>int</code> <p>Minimum generation sequence length. Defaults to 0.</p> <code>0</code> <code>max_gen_seq_length</code> <code>int</code> <p>Maximum generation sequence length. Defaults to 48.</p> <code>48</code> <code>repetition_penalty</code> <code>float</code> <p>Repetition penalty. Defaults to 1.0.</p> <code>1.0</code> <code>no_repeat_ngram_size</code> <code>int</code> <p>Size of n-grams to prevent repetition. Defaults to 0.</p> <code>0</code> <code>early_stopping</code> <code>bool</code> <p>Whether to perform early stopping. Defaults to True.</p> <code>True</code> <code>length_penalty</code> <code>float</code> <p>Length penalty. Defaults to 1.0.</p> <code>1.0</code> <code>num_beam_groups</code> <code>int</code> <p>Number of beam groups for diverse beam search. Defaults to 1.</p> <code>1</code> <code>diversity_penalty</code> <code>float</code> <p>Diversity penalty for diverse beam search. Defaults to 0.0.</p> <code>0.0</code> <code>do_sample</code> <code>bool</code> <p>Whether to use sampling for generation. Defaults to False.</p> <code>False</code> <code>temperature</code> <code>float</code> <p>Sampling temperature. Defaults to 1.0.</p> <code>1.0</code> <code>top_k</code> <code>int</code> <p>Top-k sampling parameter. Defaults to 50.</p> <code>50</code> <code>top_p</code> <code>float</code> <p>Top-p sampling parameter. Defaults to 1.0.</p> <code>1.0</code> <p>Returns:</p> Name Type Description <code>GenerationOutputs</code> <p>The generation outputs.</p> Source code in <code>src/unitorch/cli/models/llama/modeling.py</code> <pre><code>@add_default_section_for_function(\"core/model/generation/llama\")\n@torch.no_grad()\n@autocast()\ndef generate(\n    self,\n    input_ids: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 1,\n    decoder_end_token_id: Optional[int] = 2,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n):\n\"\"\"\n    Generate sequences using the Llama model.\n\n    Args:\n        input_ids (torch.Tensor): Input token IDs.\n        num_beams (int, optional): Number of beams for beam search. Defaults to 5.\n        decoder_start_token_id (int, optional): Decoder start token ID. Defaults to 0.\n        decoder_end_token_id (int, optional): Decoder end token ID. Defaults to 1.\n        num_return_sequences (int, optional): Number of generated sequences to return. Defaults to 1.\n        min_gen_seq_length (int, optional): Minimum generation sequence length. Defaults to 0.\n        max_gen_seq_length (int, optional): Maximum generation sequence length. Defaults to 48.\n        repetition_penalty (float, optional): Repetition penalty. Defaults to 1.0.\n        no_repeat_ngram_size (int, optional): Size of n-grams to prevent repetition. Defaults to 0.\n        early_stopping (bool, optional): Whether to perform early stopping. Defaults to True.\n        length_penalty (float, optional): Length penalty. Defaults to 1.0.\n        num_beam_groups (int, optional): Number of beam groups for diverse beam search. Defaults to 1.\n        diversity_penalty (float, optional): Diversity penalty for diverse beam search. Defaults to 0.0.\n        do_sample (bool, optional): Whether to use sampling for generation. Defaults to False.\n        temperature (float, optional): Sampling temperature. Defaults to 1.0.\n        top_k (int, optional): Top-k sampling parameter. Defaults to 50.\n        top_p (float, optional): Top-p sampling parameter. Defaults to 1.0.\n\n    Returns:\n        GenerationOutputs: The generation outputs.\n    \"\"\"\n    outputs = super().generate(\n        input_ids,\n        num_beams=num_beams,\n        decoder_start_token_id=decoder_start_token_id,\n        decoder_end_token_id=decoder_end_token_id,\n        num_return_sequences=num_return_sequences,\n        min_gen_seq_length=min_gen_seq_length,\n        max_gen_seq_length=max_gen_seq_length,\n        repetition_penalty=repetition_penalty,\n        no_repeat_ngram_size=no_repeat_ngram_size,\n        early_stopping=early_stopping,\n        length_penalty=length_penalty,\n        num_beam_groups=num_beam_groups,\n        diversity_penalty=diversity_penalty,\n        do_sample=do_sample,\n        temperature=temperature,\n        top_k=top_k,\n        top_p=top_p,\n    )\n\n    return GenerationOutputs(\n        sequences=outputs.sequences,\n        sequences_scores=outputs.sequences_scores,\n    )\n</code></pre>",
+            "text": "<pre><code>generate(\n    input_ids: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 1,\n    decoder_end_token_id: Optional[\n        Union[int, List[int]]\n    ] = 2,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n)\n</code></pre> <p>Generate sequences using the Llama model.</p> <p>Parameters:</p> Name Type Description Default <code>input_ids</code> <code>torch.Tensor</code> <p>Input token IDs.</p> required <code>num_beams</code> <code>int</code> <p>Number of beams for beam search. Defaults to 5.</p> <code>5</code> <code>decoder_start_token_id</code> <code>int</code> <p>Decoder start token ID. Defaults to 1.</p> <code>1</code> <code>decoder_end_token_id</code> <code>int or List[int]</code> <p>The ID(s) of the decoder end token(s). Defaults to 2.</p> <code>2</code> <code>num_return_sequences</code> <code>int</code> <p>Number of generated sequences to return. Defaults to 1.</p> <code>1</code> <code>min_gen_seq_length</code> <code>int</code> <p>Minimum generation sequence length. Defaults to 0.</p> <code>0</code> <code>max_gen_seq_length</code> <code>int</code> <p>Maximum generation sequence length. Defaults to 48.</p> <code>48</code> <code>repetition_penalty</code> <code>float</code> <p>Repetition penalty. Defaults to 1.0.</p> <code>1.0</code> <code>no_repeat_ngram_size</code> <code>int</code> <p>Size of n-grams to prevent repetition. Defaults to 0.</p> <code>0</code> <code>early_stopping</code> <code>bool</code> <p>Whether to perform early stopping. Defaults to True.</p> <code>True</code> <code>length_penalty</code> <code>float</code> <p>Length penalty. Defaults to 1.0.</p> <code>1.0</code> <code>num_beam_groups</code> <code>int</code> <p>Number of beam groups for diverse beam search. Defaults to 1.</p> <code>1</code> <code>diversity_penalty</code> <code>float</code> <p>Diversity penalty for diverse beam search. Defaults to 0.0.</p> <code>0.0</code> <code>do_sample</code> <code>bool</code> <p>Whether to use sampling for generation. Defaults to False.</p> <code>False</code> <code>temperature</code> <code>float</code> <p>Sampling temperature. Defaults to 1.0.</p> <code>1.0</code> <code>top_k</code> <code>int</code> <p>Top-k sampling parameter. Defaults to 50.</p> <code>50</code> <code>top_p</code> <code>float</code> <p>Top-p sampling parameter. Defaults to 1.0.</p> <code>1.0</code> <p>Returns:</p> Name Type Description <code>GenerationOutputs</code> <p>The generation outputs.</p> Source code in <code>src/unitorch/cli/models/llama/modeling.py</code> <pre><code>@add_default_section_for_function(\"core/model/generation/llama\")\n@torch.no_grad()\n@autocast()\ndef generate(\n    self,\n    input_ids: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 1,\n    decoder_end_token_id: Optional[Union[int, List[int]]] = 2,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n):\n\"\"\"\n    Generate sequences using the Llama model.\n\n    Args:\n        input_ids (torch.Tensor): Input token IDs.\n        num_beams (int, optional): Number of beams for beam search. Defaults to 5.\n        decoder_start_token_id (int, optional): Decoder start token ID. Defaults to 1.\n        decoder_end_token_id (int or List[int], optional): The ID(s) of the decoder end token(s). Defaults to 2.\n        num_return_sequences (int, optional): Number of generated sequences to return. Defaults to 1.\n        min_gen_seq_length (int, optional): Minimum generation sequence length. Defaults to 0.\n        max_gen_seq_length (int, optional): Maximum generation sequence length. Defaults to 48.\n        repetition_penalty (float, optional): Repetition penalty. Defaults to 1.0.\n        no_repeat_ngram_size (int, optional): Size of n-grams to prevent repetition. Defaults to 0.\n        early_stopping (bool, optional): Whether to perform early stopping. Defaults to True.\n        length_penalty (float, optional): Length penalty. Defaults to 1.0.\n        num_beam_groups (int, optional): Number of beam groups for diverse beam search. Defaults to 1.\n        diversity_penalty (float, optional): Diversity penalty for diverse beam search. Defaults to 0.0.\n        do_sample (bool, optional): Whether to use sampling for generation. Defaults to False.\n        temperature (float, optional): Sampling temperature. Defaults to 1.0.\n        top_k (int, optional): Top-k sampling parameter. Defaults to 50.\n        top_p (float, optional): Top-p sampling parameter. Defaults to 1.0.\n\n    Returns:\n        GenerationOutputs: The generation outputs.\n    \"\"\"\n    outputs = super().generate(\n        input_ids,\n        num_beams=num_beams,\n        decoder_start_token_id=decoder_start_token_id,\n        decoder_end_token_id=decoder_end_token_id,\n        num_return_sequences=num_return_sequences,\n        min_gen_seq_length=min_gen_seq_length,\n        max_gen_seq_length=max_gen_seq_length,\n        repetition_penalty=repetition_penalty,\n        no_repeat_ngram_size=no_repeat_ngram_size,\n        early_stopping=early_stopping,\n        length_penalty=length_penalty,\n        num_beam_groups=num_beam_groups,\n        diversity_penalty=diversity_penalty,\n        do_sample=do_sample,\n        temperature=temperature,\n        top_k=top_k,\n        top_p=top_p,\n    )\n\n    return GenerationOutputs(\n        sequences=outputs.sequences,\n        sequences_scores=outputs.sequences_scores,\n    )\n</code></pre>",
             "title": "generate"
         },
         {
             "location": "cli/models/mbart/",
             "text": "",
             "title": "unitorch.cli.models.mbart"
         },
@@ -857,15 +857,50 @@
         {
             "location": "cli/models/mbart/#unitorch.cli.models.mbart.modeling.MBartForGeneration.from_core_configure",
             "text": "<pre><code>from_core_configure(config, **kwargs)\n</code></pre> <p>Create an instance of MBartForGeneration from a core configuration.</p> <p>Parameters:</p> Name Type Description Default <code>config</code> <p>The core configuration.</p> required <code>**kwargs</code> <p>Additional keyword arguments.</p> <code>{}</code> <p>Returns:</p> Name Type Description <code>MBartForGeneration</code> <p>An instance of MBartForGeneration.</p> Source code in <code>src/unitorch/cli/models/mbart/modeling.py</code> <pre><code>@classmethod\n@add_default_section_for_init(\"core/model/generation/mbart\")\ndef from_core_configure(cls, config, **kwargs):\n\"\"\"\n    Create an instance of MBartForGeneration from a core configuration.\n\n    Args:\n        config: The core configuration.\n        **kwargs: Additional keyword arguments.\n\n    Returns:\n        MBartForGeneration: An instance of MBartForGeneration.\n    \"\"\"\n    config.set_default_section(\"core/model/generation/mbart\")\n    pretrained_name = config.getoption(\"pretrained_name\", \"default-mbart\")\n    config_path = config.getoption(\"config_path\", None)\n    config_path = pop_value(\n        config_path,\n        nested_dict_value(pretrained_mbart_infos, pretrained_name, \"config\"),\n    )\n\n    config_path = cached_path(config_path)\n    freeze_input_embedding = config.getoption(\"freeze_input_embedding\", True)\n    gradient_checkpointing = config.getoption(\"gradient_checkpointing\", False)\n\n    inst = cls(\n        config_path,\n        freeze_input_embedding=freeze_input_embedding,\n        gradient_checkpointing=gradient_checkpointing,\n    )\n    pretrained_weight_path = config.getoption(\"pretrained_weight_path\", None)\n    weight_path = pop_value(\n        pretrained_weight_path,\n        nested_dict_value(pretrained_mbart_infos, pretrained_name, \"weight\"),\n        check_none=False,\n    )\n    if weight_path is not None:\n        weight_path = cached_path(weight_path)\n        inst.from_pretrained(weight_path)\n\n    return inst\n</code></pre>",
             "title": "from_core_configure  <code>classmethod</code>"
         },
         {
             "location": "cli/models/mbart/#unitorch.cli.models.mbart.modeling.MBartForGeneration.generate",
-            "text": "<pre><code>generate(\n    input_ids: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 2,\n    decoder_end_token_id: Optional[int] = 2,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n)\n</code></pre> <p>Generate sequences using the MBart model.</p> <p>Parameters:</p> Name Type Description Default <code>input_ids</code> <code>torch.Tensor</code> <p>Input token IDs.</p> required <code>num_beams</code> <code>int</code> <p>Number of beams for beam search. Defaults to 5.</p> <code>5</code> <code>decoder_start_token_id</code> <code>int</code> <p>Decoder start token ID. Defaults to 0.</p> <code>2</code> <code>decoder_end_token_id</code> <code>int</code> <p>Decoder end token ID. Defaults to 1.</p> <code>2</code> <code>num_return_sequences</code> <code>int</code> <p>Number of generated sequences to return. Defaults to 1.</p> <code>1</code> <code>min_gen_seq_length</code> <code>int</code> <p>Minimum generation sequence length. Defaults to 0.</p> <code>0</code> <code>max_gen_seq_length</code> <code>int</code> <p>Maximum generation sequence length. Defaults to 48.</p> <code>48</code> <code>repetition_penalty</code> <code>float</code> <p>Repetition penalty. Defaults to 1.0.</p> <code>1.0</code> <code>no_repeat_ngram_size</code> <code>int</code> <p>Size of n-grams to prevent repetition. Defaults to 0.</p> <code>0</code> <code>early_stopping</code> <code>bool</code> <p>Whether to perform early stopping. Defaults to True.</p> <code>True</code> <code>length_penalty</code> <code>float</code> <p>Length penalty. Defaults to 1.0.</p> <code>1.0</code> <code>num_beam_groups</code> <code>int</code> <p>Number of beam groups for diverse beam search. Defaults to 1.</p> <code>1</code> <code>diversity_penalty</code> <code>float</code> <p>Diversity penalty for diverse beam search. Defaults to 0.0.</p> <code>0.0</code> <code>do_sample</code> <code>bool</code> <p>Whether to use sampling for generation. Defaults to False.</p> <code>False</code> <code>temperature</code> <code>float</code> <p>Sampling temperature. Defaults to 1.0.</p> <code>1.0</code> <code>top_k</code> <code>int</code> <p>Top-k sampling parameter. Defaults to 50.</p> <code>50</code> <code>top_p</code> <code>float</code> <p>Top-p sampling parameter. Defaults to 1.0.</p> <code>1.0</code> <p>Returns:</p> Name Type Description <code>GenerationOutputs</code> <p>The generation outputs.</p> Source code in <code>src/unitorch/cli/models/mbart/modeling.py</code> <pre><code>@add_default_section_for_function(\"core/model/generation/mbart\")\n@torch.no_grad()\n@autocast()\ndef generate(\n    self,\n    input_ids: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 2,\n    decoder_end_token_id: Optional[int] = 2,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n):\n\"\"\"\n    Generate sequences using the MBart model.\n\n    Args:\n        input_ids (torch.Tensor): Input token IDs.\n        num_beams (int, optional): Number of beams for beam search. Defaults to 5.\n        decoder_start_token_id (int, optional): Decoder start token ID. Defaults to 0.\n        decoder_end_token_id (int, optional): Decoder end token ID. Defaults to 1.\n        num_return_sequences (int, optional): Number of generated sequences to return. Defaults to 1.\n        min_gen_seq_length (int, optional): Minimum generation sequence length. Defaults to 0.\n        max_gen_seq_length (int, optional): Maximum generation sequence length. Defaults to 48.\n        repetition_penalty (float, optional): Repetition penalty. Defaults to 1.0.\n        no_repeat_ngram_size (int, optional): Size of n-grams to prevent repetition. Defaults to 0.\n        early_stopping (bool, optional): Whether to perform early stopping. Defaults to True.\n        length_penalty (float, optional): Length penalty. Defaults to 1.0.\n        num_beam_groups (int, optional): Number of beam groups for diverse beam search. Defaults to 1.\n        diversity_penalty (float, optional): Diversity penalty for diverse beam search. Defaults to 0.0.\n        do_sample (bool, optional): Whether to use sampling for generation. Defaults to False.\n        temperature (float, optional): Sampling temperature. Defaults to 1.0.\n        top_k (int, optional): Top-k sampling parameter. Defaults to 50.\n        top_p (float, optional): Top-p sampling parameter. Defaults to 1.0.\n\n    Returns:\n        GenerationOutputs: The generation outputs.\n    \"\"\"\n    outputs = super().generate(\n        input_ids,\n        num_beams=num_beams,\n        decoder_start_token_id=decoder_start_token_id,\n        decoder_end_token_id=decoder_end_token_id,\n        num_return_sequences=num_return_sequences,\n        min_gen_seq_length=min_gen_seq_length,\n        max_gen_seq_length=max_gen_seq_length,\n        repetition_penalty=repetition_penalty,\n        no_repeat_ngram_size=no_repeat_ngram_size,\n        early_stopping=early_stopping,\n        length_penalty=length_penalty,\n        num_beam_groups=num_beam_groups,\n        diversity_penalty=diversity_penalty,\n        do_sample=do_sample,\n        temperature=temperature,\n        top_k=top_k,\n        top_p=top_p,\n    )\n\n    return GenerationOutputs(\n        sequences=outputs.sequences,\n        sequences_scores=outputs.sequences_scores,\n    )\n</code></pre>",
+            "text": "<pre><code>generate(\n    input_ids: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 2,\n    decoder_end_token_id: Optional[\n        Union[int, List[int]]\n    ] = 2,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n)\n</code></pre> <p>Generate sequences using the MBart model.</p> <p>Parameters:</p> Name Type Description Default <code>input_ids</code> <code>torch.Tensor</code> <p>Input token IDs.</p> required <code>num_beams</code> <code>int</code> <p>Number of beams for beam search. Defaults to 5.</p> <code>5</code> <code>decoder_start_token_id</code> <code>int</code> <p>Decoder start token ID. Defaults to 0.</p> <code>2</code> <code>decoder_end_token_id</code> <code>int or List[int]</code> <p>The ID(s) of the decoder end token(s). Defaults to 1.</p> <code>2</code> <code>num_return_sequences</code> <code>int</code> <p>Number of generated sequences to return. Defaults to 1.</p> <code>1</code> <code>min_gen_seq_length</code> <code>int</code> <p>Minimum generation sequence length. Defaults to 0.</p> <code>0</code> <code>max_gen_seq_length</code> <code>int</code> <p>Maximum generation sequence length. Defaults to 48.</p> <code>48</code> <code>repetition_penalty</code> <code>float</code> <p>Repetition penalty. Defaults to 1.0.</p> <code>1.0</code> <code>no_repeat_ngram_size</code> <code>int</code> <p>Size of n-grams to prevent repetition. Defaults to 0.</p> <code>0</code> <code>early_stopping</code> <code>bool</code> <p>Whether to perform early stopping. Defaults to True.</p> <code>True</code> <code>length_penalty</code> <code>float</code> <p>Length penalty. Defaults to 1.0.</p> <code>1.0</code> <code>num_beam_groups</code> <code>int</code> <p>Number of beam groups for diverse beam search. Defaults to 1.</p> <code>1</code> <code>diversity_penalty</code> <code>float</code> <p>Diversity penalty for diverse beam search. Defaults to 0.0.</p> <code>0.0</code> <code>do_sample</code> <code>bool</code> <p>Whether to use sampling for generation. Defaults to False.</p> <code>False</code> <code>temperature</code> <code>float</code> <p>Sampling temperature. Defaults to 1.0.</p> <code>1.0</code> <code>top_k</code> <code>int</code> <p>Top-k sampling parameter. Defaults to 50.</p> <code>50</code> <code>top_p</code> <code>float</code> <p>Top-p sampling parameter. Defaults to 1.0.</p> <code>1.0</code> <p>Returns:</p> Name Type Description <code>GenerationOutputs</code> <p>The generation outputs.</p> Source code in <code>src/unitorch/cli/models/mbart/modeling.py</code> <pre><code>@add_default_section_for_function(\"core/model/generation/mbart\")\n@torch.no_grad()\n@autocast()\ndef generate(\n    self,\n    input_ids: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 2,\n    decoder_end_token_id: Optional[Union[int, List[int]]] = 2,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n):\n\"\"\"\n    Generate sequences using the MBart model.\n\n    Args:\n        input_ids (torch.Tensor): Input token IDs.\n        num_beams (int, optional): Number of beams for beam search. Defaults to 5.\n        decoder_start_token_id (int, optional): Decoder start token ID. Defaults to 0.\n        decoder_end_token_id (int or List[int], optional): The ID(s) of the decoder end token(s). Defaults to 1.\n        num_return_sequences (int, optional): Number of generated sequences to return. Defaults to 1.\n        min_gen_seq_length (int, optional): Minimum generation sequence length. Defaults to 0.\n        max_gen_seq_length (int, optional): Maximum generation sequence length. Defaults to 48.\n        repetition_penalty (float, optional): Repetition penalty. Defaults to 1.0.\n        no_repeat_ngram_size (int, optional): Size of n-grams to prevent repetition. Defaults to 0.\n        early_stopping (bool, optional): Whether to perform early stopping. Defaults to True.\n        length_penalty (float, optional): Length penalty. Defaults to 1.0.\n        num_beam_groups (int, optional): Number of beam groups for diverse beam search. Defaults to 1.\n        diversity_penalty (float, optional): Diversity penalty for diverse beam search. Defaults to 0.0.\n        do_sample (bool, optional): Whether to use sampling for generation. Defaults to False.\n        temperature (float, optional): Sampling temperature. Defaults to 1.0.\n        top_k (int, optional): Top-k sampling parameter. Defaults to 50.\n        top_p (float, optional): Top-p sampling parameter. Defaults to 1.0.\n\n    Returns:\n        GenerationOutputs: The generation outputs.\n    \"\"\"\n    outputs = super().generate(\n        input_ids,\n        num_beams=num_beams,\n        decoder_start_token_id=decoder_start_token_id,\n        decoder_end_token_id=decoder_end_token_id,\n        num_return_sequences=num_return_sequences,\n        min_gen_seq_length=min_gen_seq_length,\n        max_gen_seq_length=max_gen_seq_length,\n        repetition_penalty=repetition_penalty,\n        no_repeat_ngram_size=no_repeat_ngram_size,\n        early_stopping=early_stopping,\n        length_penalty=length_penalty,\n        num_beam_groups=num_beam_groups,\n        diversity_penalty=diversity_penalty,\n        do_sample=do_sample,\n        temperature=temperature,\n        top_k=top_k,\n        top_p=top_p,\n    )\n\n    return GenerationOutputs(\n        sequences=outputs.sequences,\n        sequences_scores=outputs.sequences_scores,\n    )\n</code></pre>",
+            "title": "generate"
+        },
+        {
+            "location": "cli/models/minigpt4/",
+            "text": "",
+            "title": "unitorch.cli.models.minigpt4"
+        },
+        {
+            "location": "cli/models/minigpt4/#minigpt4blip2llamaprocessor",
+            "text": "<p>         Bases: <code>_MiniGPT4Blip2LlamaProcessor</code></p> <p>MiniGPT4Blip2LlamaProcessor is a class for processing inputs and outputs of the MiniGPT4 model with Blip2 and Llama. It inherits from the _MiniGPT4Blip2LlamaProcessor class.</p> <p>Initializes a MiniGPT4Blip2LlamaProcessor instance.</p> <p>Parameters:</p> Name Type Description Default <code>vocab_path</code> <code>str</code> <p>The file path to the vocabulary.</p> required <code>vision_config_path</code> <code>str</code> <p>The file path to the vision configuration.</p> required <code>max_prefix_seq_length</code> <code>int</code> <p>The maximum length of the prefix sequence. Defaults to 32.</p> <code>32</code> <code>max_suffix_seq_length</code> <code>int</code> <p>The maximum length of the suffix sequence. Defaults to 128.</p> <code>128</code> <code>max_gen_seq_length</code> <code>int</code> <p>The maximum length of the generated sequence. Defaults to 128.</p> <code>128</code> Source code in <code>src/unitorch/cli/models/minigpt4/processing.py</code> <pre><code>def __init__(\n    self,\n    vocab_path: str,\n    vision_config_path: str,\n    max_prefix_seq_length: Optional[int] = 32,\n    max_suffix_seq_length: Optional[int] = 128,\n    max_gen_seq_length: Optional[int] = 128,\n):\n\"\"\"\n    Initializes a MiniGPT4Blip2LlamaProcessor instance.\n\n    Args:\n        vocab_path (str): The file path to the vocabulary.\n        vision_config_path (str): The file path to the vision configuration.\n        max_prefix_seq_length (int, optional): The maximum length of the prefix sequence. Defaults to 32.\n        max_suffix_seq_length (int, optional): The maximum length of the suffix sequence. Defaults to 128.\n        max_gen_seq_length (int, optional): The maximum length of the generated sequence. Defaults to 128.\n    \"\"\"\n    super().__init__(\n        vocab_file=vocab_path,\n        vision_config_path=vision_config_path,\n        max_prefix_seq_length=max_prefix_seq_length,\n        max_suffix_seq_length=max_suffix_seq_length,\n        max_gen_seq_length=max_gen_seq_length,\n    )\n</code></pre>",
+            "title": "MiniGPT4Blip2LlamaProcessor"
+        },
+        {
+            "location": "cli/models/minigpt4/#unitorch.cli.models.minigpt4.processing.MiniGPT4Blip2LlamaProcessor.from_core_configure",
+            "text": "<pre><code>from_core_configure(config, **kwargs)\n</code></pre> <p>Creates a MiniGPT4Blip2LlamaProcessor instance from a core configuration.</p> <p>Parameters:</p> Name Type Description Default <code>config</code> <p>The configuration object.</p> required <code>**kwargs</code> <p>Additional keyword arguments.</p> <code>{}</code> <p>Returns:</p> Name Type Description <code>dict</code> <p>The dictionary containing the processor configuration.</p> Source code in <code>src/unitorch/cli/models/minigpt4/processing.py</code> <pre><code>@classmethod\n@add_default_section_for_init(\"core/process/minigpt4\")\ndef from_core_configure(cls, config, **kwargs):\n\"\"\"\n    Creates a MiniGPT4Blip2LlamaProcessor instance from a core configuration.\n\n    Args:\n        config: The configuration object.\n        **kwargs: Additional keyword arguments.\n\n    Returns:\n        dict: The dictionary containing the processor configuration.\n    \"\"\"\n    config.set_default_section(\"core/process/minigpt4\")\n    pretrained_name = config.getoption(\"pretrained_name\", \"default-minigpt4\")\n    vocab_path = config.getoption(\"vocab_path\", None)\n    vocab_path = pop_value(\n        vocab_path,\n        nested_dict_value(pretrained_minigpt4_infos, pretrained_name, \"vocab\"),\n    )\n    vocab_path = cached_path(vocab_path)\n\n    vision_config_path = config.getoption(\"vision_config_path\", None)\n    vision_config_path = pop_value(\n        vision_config_path,\n        nested_dict_value(\n            pretrained_minigpt4_infos, pretrained_name, \"vision_config\"\n        ),\n    )\n    vision_config_path = cached_path(vision_config_path)\n\n    return {\n        \"vocab_path\": vocab_path,\n        \"vision_config_path\": vision_config_path,\n    }\n</code></pre>",
+            "title": "from_core_configure  <code>classmethod</code>"
+        },
+        {
+            "location": "cli/models/minigpt4/#minigpt4blip2llamaforgeneration",
+            "text": "<p>         Bases: <code>_MiniGPT4Blip2LlamaForGeneration</code></p> <p>MiniGPT4Blip2LlamaForGeneration is a class for generating sequences using the MiniGPT4 model with Blip2 and Llama. It inherits from the _MiniGPT4Blip2LlamaForGeneration class.</p> <p>Initializes a MiniGPT4Blip2LlamaForGeneration instance.</p> <p>Parameters:</p> Name Type Description Default <code>blip2_config_path</code> <code>str</code> <p>The file path to the Blip2 configuration.</p> required <code>llama_config_path</code> <code>str</code> <p>The file path to the Llama configuration.</p> required <code>pad_token_id</code> <code>int</code> <p>The ID of the padding token. Defaults to 0.</p> <code>0</code> <code>freeze_vision_model</code> <code>bool</code> <p>Whether to freeze the vision model. Defaults to True.</p> <code>True</code> <code>freeze_qformer_model</code> <code>bool</code> <p>Whether to freeze the query transformer model. Defaults to True.</p> <code>True</code> <code>freeze_llama_model</code> <code>bool</code> <p>Whether to freeze the Llama model. Defaults to True.</p> <code>True</code> <code>gradient_checkpointing</code> <code>bool</code> <p>Whether to use gradient checkpointing. Defaults to False.</p> <code>False</code> Source code in <code>src/unitorch/cli/models/minigpt4/modeling.py</code> <pre><code>def __init__(\n    self,\n    blip2_config_path: str,\n    llama_config_path: str,\n    pad_token_id: Optional[int] = 0,\n    freeze_vision_model: Optional[bool] = True,\n    freeze_qformer_model: Optional[bool] = True,\n    freeze_llama_model: Optional[bool] = True,\n    gradient_checkpointing: Optional[bool] = False,\n):\n\"\"\"\n    Initializes a MiniGPT4Blip2LlamaForGeneration instance.\n\n    Args:\n        blip2_config_path (str): The file path to the Blip2 configuration.\n        llama_config_path (str): The file path to the Llama configuration.\n        pad_token_id (int, optional): The ID of the padding token. Defaults to 0.\n        freeze_vision_model (bool, optional): Whether to freeze the vision model. Defaults to True.\n        freeze_qformer_model (bool, optional): Whether to freeze the query transformer model. Defaults to True.\n        freeze_llama_model (bool, optional): Whether to freeze the Llama model. Defaults to True.\n        gradient_checkpointing (bool, optional): Whether to use gradient checkpointing. Defaults to False.\n    \"\"\"\n    super().__init__(\n        blip2_config_path=blip2_config_path,\n        llama_config_path=llama_config_path,\n        pad_token_id=pad_token_id,\n        freeze_vision_model=freeze_vision_model,\n        freeze_qformer_model=freeze_qformer_model,\n        freeze_llama_model=freeze_llama_model,\n        gradient_checkpointing=gradient_checkpointing,\n    )\n</code></pre>",
+            "title": "MiniGPT4Blip2LlamaForGeneration"
+        },
+        {
+            "location": "cli/models/minigpt4/#unitorch.cli.models.minigpt4.modeling.MiniGPT4Blip2LlamaForGeneration.forward",
+            "text": "<pre><code>forward(\n    pixel_values: torch.Tensor,\n    prefix_input_ids: torch.Tensor,\n    suffix_input_ids: torch.Tensor,\n    decoder_input_ids: torch.Tensor,\n    prefix_attention_mask: Optional[torch.Tensor] = None,\n    suffix_attention_mask: Optional[torch.Tensor] = None,\n    decoder_attention_mask: Optional[torch.Tensor] = None,\n)\n</code></pre> <p>Performs a forward pass through the model.</p> <p>Parameters:</p> Name Type Description Default <code>pixel_values</code> <code>torch.Tensor</code> <p>The pixel values.</p> required <code>prefix_input_ids</code> <code>torch.Tensor</code> <p>The input IDs for the prefix tokens.</p> required <code>suffix_input_ids</code> <code>torch.Tensor</code> <p>The input IDs for the suffix tokens.</p> required <code>decoder_input_ids</code> <code>torch.Tensor</code> <p>The input IDs for the decoder tokens.</p> required <code>prefix_attention_mask</code> <code>torch.Tensor</code> <p>The attention mask for the prefix tokens. Defaults to None.</p> <code>None</code> <code>suffix_attention_mask</code> <code>torch.Tensor</code> <p>The attention mask for the suffix tokens. Defaults to None.</p> <code>None</code> <code>decoder_attention_mask</code> <code>torch.Tensor</code> <p>The attention mask for the decoder tokens. Defaults to None.</p> <code>None</code> <p>Returns:</p> Name Type Description <code>GenerationOutputs</code> <p>The generation outputs.</p> Source code in <code>src/unitorch/cli/models/minigpt4/modeling.py</code> <pre><code>@autocast()\ndef forward(\n    self,\n    pixel_values: torch.Tensor,\n    prefix_input_ids: torch.Tensor,\n    suffix_input_ids: torch.Tensor,\n    decoder_input_ids: torch.Tensor,\n    prefix_attention_mask: Optional[torch.Tensor] = None,\n    suffix_attention_mask: Optional[torch.Tensor] = None,\n    decoder_attention_mask: Optional[torch.Tensor] = None,\n):\n\"\"\"\n    Performs a forward pass through the model.\n\n    Args:\n        pixel_values (torch.Tensor): The pixel values.\n        prefix_input_ids (torch.Tensor): The input IDs for the prefix tokens.\n        suffix_input_ids (torch.Tensor): The input IDs for the suffix tokens.\n        decoder_input_ids (torch.Tensor): The input IDs for the decoder tokens.\n        prefix_attention_mask (torch.Tensor, optional): The attention mask for the prefix tokens.\n            Defaults to None.\n        suffix_attention_mask (torch.Tensor, optional): The attention mask for the suffix tokens.\n            Defaults to None.\n        decoder_attention_mask (torch.Tensor, optional): The attention mask for the decoder tokens.\n            Defaults to None.\n\n    Returns:\n        GenerationOutputs: The generation outputs.\n    \"\"\"\n    outputs = super().forward(\n        pixel_values=pixel_values,\n        prefix_input_ids=prefix_input_ids,\n        suffix_input_ids=suffix_input_ids,\n        decoder_input_ids=decoder_input_ids,\n        prefix_attention_mask=prefix_attention_mask,\n        suffix_attention_mask=suffix_attention_mask,\n        decoder_attention_mask=decoder_attention_mask,\n    )\n    return GenerationOutputs(sequences=outputs)\n</code></pre>",
+            "title": "forward"
+        },
+        {
+            "location": "cli/models/minigpt4/#unitorch.cli.models.minigpt4.modeling.MiniGPT4Blip2LlamaForGeneration.from_core_configure",
+            "text": "<pre><code>from_core_configure(config, **kwargs)\n</code></pre> <p>Creates a MiniGPT4Blip2LlamaForGeneration instance from a core configuration.</p> <p>Parameters:</p> Name Type Description Default <code>config</code> <p>The configuration object.</p> required <code>**kwargs</code> <p>Additional keyword arguments.</p> <code>{}</code> <p>Returns:</p> Name Type Description <code>MiniGPT4Blip2LlamaForGeneration</code> <p>The created instance.</p> Source code in <code>src/unitorch/cli/models/minigpt4/modeling.py</code> <pre><code>@classmethod\n@add_default_section_for_init(\"core/model/generation/minigpt4\")\ndef from_core_configure(cls, config, **kwargs):\n\"\"\"\n    Creates a MiniGPT4Blip2LlamaForGeneration instance from a core configuration.\n\n    Args:\n        config: The configuration object.\n        **kwargs: Additional keyword arguments.\n\n    Returns:\n        MiniGPT4Blip2LlamaForGeneration: The created instance.\n    \"\"\"\n    config.set_default_section(\"core/model/generation/minigpt4\")\n    pretrained_name = config.getoption(\"pretrained_name\", \"default-minigpt4\")\n\n    blip2_config_path = config.getoption(\"blip2_config_path\", None)\n    blip2_config_path = pop_value(\n        blip2_config_path,\n        nested_dict_value(\n            pretrained_minigpt4_infos, pretrained_name, \"blip2_config_path\"\n        ),\n    )\n    blip2_config_path = cached_path(blip2_config_path)\n\n    llama_config_path = config.getoption(\"llama_config_path\", None)\n    llama_config_path = pop_value(\n        llama_config_path,\n        nested_dict_value(\n            pretrained_minigpt4_infos, pretrained_name, \"llama_config_path\"\n        ),\n    )\n    llama_config_path = cached_path(llama_config_path)\n\n    freeze_vision_model = config.getoption(\"freeze_vision_model\", True)\n    freeze_qformer_model = config.getoption(\"freeze_qformer_model\", True)\n    freeze_llama_model = config.getoption(\"freeze_llama_model\", True)\n    gradient_checkpointing = config.getoption(\"gradient_checkpointing\", False)\n\n    inst = cls(\n        blip2_config_path,\n        llama_config_path,\n        freeze_vision_model=freeze_vision_model,\n        freeze_qformer_model=freeze_qformer_model,\n        freeze_llama_model=freeze_llama_model,\n        gradient_checkpointing=gradient_checkpointing,\n    )\n    pretrained_weight_path = config.getoption(\"pretrained_weight_path\", None)\n    weight_path = pop_value(\n        pretrained_weight_path,\n        nested_dict_value(pretrained_minigpt4_infos, pretrained_name, \"weight\"),\n        check_none=False,\n    )\n\n    if weight_path is not None:\n        inst.from_pretrained(\n            weight_path=weight_path,\n        )\n\n    return inst\n</code></pre>",
+            "title": "from_core_configure  <code>classmethod</code>"
+        },
+        {
+            "location": "cli/models/minigpt4/#unitorch.cli.models.minigpt4.modeling.MiniGPT4Blip2LlamaForGeneration.generate",
+            "text": "<pre><code>generate(\n    pixel_values: torch.Tensor,\n    prefix_input_ids: torch.Tensor,\n    suffix_input_ids: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 1,\n    decoder_end_token_id: Optional[\n        Union[int, List[int]]\n    ] = 2,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n)\n</code></pre> <p>Generates sequences using the model.</p> <p>Parameters:</p> Name Type Description Default <code>pixel_values</code> <code>torch.Tensor</code> <p>The pixel values.</p> required <code>prefix_input_ids</code> <code>torch.Tensor</code> <p>The input IDs for the prefix tokens.</p> required <code>suffix_input_ids</code> <code>torch.Tensor</code> <p>The input IDs for the suffix tokens.</p> required <code>num_beams</code> <code>int</code> <p>The number of beams for beam search. Defaults to 5.</p> <code>5</code> <code>decoder_start_token_id</code> <code>int</code> <p>The ID of the decoder start token. Defaults to 1.</p> <code>1</code> <code>decoder_end_token_id</code> <code>int or List[int]</code> <p>The ID(s) of the decoder end token(s). Defaults to 2.</p> <code>2</code> <code>num_return_sequences</code> <code>int</code> <p>The number of sequences to return. Defaults to 1.</p> <code>1</code> <code>min_gen_seq_length</code> <code>int</code> <p>The minimum generated sequence length. Defaults to 0.</p> <code>0</code> <code>max_gen_seq_length</code> <code>int</code> <p>The maximum generated sequence length. Defaults to 48.</p> <code>48</code> <code>repetition_penalty</code> <code>float</code> <p>The repetition penalty. Defaults to 1.0.</p> <code>1.0</code> <code>no_repeat_ngram_size</code> <code>int</code> <p>The size of the n-grams to avoid repeating. Defaults to 0.</p> <code>0</code> <code>early_stopping</code> <code>bool</code> <p>Whether to perform early stopping. Defaults to True.</p> <code>True</code> <code>length_penalty</code> <code>float</code> <p>The length penalty. Defaults to 1.0.</p> <code>1.0</code> <code>num_beam_groups</code> <code>int</code> <p>The number of beam groups for diverse beam search. Defaults to 1.</p> <code>1</code> <code>diversity_penalty</code> <code>float</code> <p>The diversity penalty for diverse beam search. Defaults to 0.0.</p> <code>0.0</code> <code>do_sample</code> <code>bool</code> <p>Whether to use sampling instead of beam search. Defaults to False.</p> <code>False</code> <code>temperature</code> <code>float</code> <p>The temperature value for sampling. Defaults to 1.0.</p> <code>1.0</code> <code>top_k</code> <code>int</code> <p>The value for top-k sampling. Defaults to 50.</p> <code>50</code> <code>top_p</code> <code>float</code> <p>The value for top-p (nucleus) sampling. Defaults to 1.0.</p> <code>1.0</code> <p>Returns:</p> Name Type Description <code>GenerationOutputs</code> <p>The generation outputs.</p> Source code in <code>src/unitorch/cli/models/minigpt4/modeling.py</code> <pre><code>@add_default_section_for_function(\"core/model/generation/minigpt4\")\n@torch.no_grad()\n@autocast()\ndef generate(\n    self,\n    pixel_values: torch.Tensor,\n    prefix_input_ids: torch.Tensor,\n    suffix_input_ids: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 1,\n    decoder_end_token_id: Optional[Union[int, List[int]]] = 2,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n):\n\"\"\"\n    Generates sequences using the model.\n\n    Args:\n        pixel_values (torch.Tensor): The pixel values.\n        prefix_input_ids (torch.Tensor): The input IDs for the prefix tokens.\n        suffix_input_ids (torch.Tensor): The input IDs for the suffix tokens.\n        num_beams (int, optional): The number of beams for beam search. Defaults to 5.\n        decoder_start_token_id (int, optional): The ID of the decoder start token. Defaults to 1.\n        decoder_end_token_id (int or List[int], optional): The ID(s) of the decoder end token(s).\n            Defaults to 2.\n        num_return_sequences (int, optional): The number of sequences to return. Defaults to 1.\n        min_gen_seq_length (int, optional): The minimum generated sequence length. Defaults to 0.\n        max_gen_seq_length (int, optional): The maximum generated sequence length. Defaults to 48.\n        repetition_penalty (float, optional): The repetition penalty. Defaults to 1.0.\n        no_repeat_ngram_size (int, optional): The size of the n-grams to avoid repeating. Defaults to 0.\n        early_stopping (bool, optional): Whether to perform early stopping. Defaults to True.\n        length_penalty (float, optional): The length penalty. Defaults to 1.0.\n        num_beam_groups (int, optional): The number of beam groups for diverse beam search.\n            Defaults to 1.\n        diversity_penalty (float, optional): The diversity penalty for diverse beam search. Defaults to 0.0.\n        do_sample (bool, optional): Whether to use sampling instead of beam search. Defaults to False.\n        temperature (float, optional): The temperature value for sampling. Defaults to 1.0.\n        top_k (int, optional): The value for top-k sampling. Defaults to 50.\n        top_p (float, optional): The value for top-p (nucleus) sampling. Defaults to 1.0.\n\n    Returns:\n        GenerationOutputs: The generation outputs.\n    \"\"\"\n    outputs = super().generate(\n        pixel_values=pixel_values,\n        prefix_input_ids=prefix_input_ids,\n        suffix_input_ids=suffix_input_ids,\n        num_beams=num_beams,\n        decoder_start_token_id=decoder_start_token_id,\n        decoder_end_token_id=decoder_end_token_id,\n        num_return_sequences=num_return_sequences,\n        min_gen_seq_length=min_gen_seq_length,\n        max_gen_seq_length=max_gen_seq_length,\n        repetition_penalty=repetition_penalty,\n        no_repeat_ngram_size=no_repeat_ngram_size,\n        early_stopping=early_stopping,\n        length_penalty=length_penalty,\n        num_beam_groups=num_beam_groups,\n        diversity_penalty=diversity_penalty,\n        do_sample=do_sample,\n        temperature=temperature,\n        top_k=top_k,\n        top_p=top_p,\n    )\n\n    return GenerationOutputs(\n        sequences=outputs.sequences,\n        sequences_scores=outputs.sequences_scores,\n    )\n</code></pre>",
             "title": "generate"
         },
         {
             "location": "cli/models/mt5/",
             "text": "",
             "title": "unitorch.cli.models.mt5"
         },
@@ -892,15 +927,15 @@
         {
             "location": "cli/models/mt5/#unitorch.cli.models.mt5.modeling.MT5ForGeneration.from_core_configure",
             "text": "<pre><code>from_core_configure(config, **kwargs)\n</code></pre> <p>Create an instance of MT5ForGeneration from a core configuration.</p> <p>Parameters:</p> Name Type Description Default <code>config</code> <p>The core configuration.</p> required <code>**kwargs</code> <p>Additional keyword arguments.</p> <code>{}</code> <p>Returns:</p> Name Type Description <code>MT5ForGeneration</code> <p>An instance of MT5ForGeneration.</p> Source code in <code>src/unitorch/cli/models/mt5/modeling.py</code> <pre><code>@classmethod\n@add_default_section_for_init(\"core/model/generation/mt5\")\ndef from_core_configure(cls, config, **kwargs):\n\"\"\"\n    Create an instance of MT5ForGeneration from a core configuration.\n\n    Args:\n        config: The core configuration.\n        **kwargs: Additional keyword arguments.\n\n    Returns:\n        MT5ForGeneration: An instance of MT5ForGeneration.\n    \"\"\"\n    config.set_default_section(\"core/model/generation/mt5\")\n    pretrained_name = config.getoption(\"pretrained_name\", \"default-mt5\")\n    config_path = config.getoption(\"config_path\", None)\n    config_path = pop_value(\n        config_path,\n        nested_dict_value(pretrained_mt5_infos, pretrained_name, \"config\"),\n    )\n\n    config_path = cached_path(config_path)\n    gradient_checkpointing = config.getoption(\"gradient_checkpointing\", False)\n\n    inst = cls(config_path, gradient_checkpointing)\n    pretrained_weight_path = config.getoption(\"pretrained_weight_path\", None)\n    weight_path = pop_value(\n        pretrained_weight_path,\n        nested_dict_value(pretrained_mt5_infos, pretrained_name, \"weight\"),\n        check_none=False,\n    )\n    if weight_path is not None:\n        weight_path = cached_path(weight_path)\n        inst.from_pretrained(weight_path)\n\n    return inst\n</code></pre>",
             "title": "from_core_configure  <code>classmethod</code>"
         },
         {
             "location": "cli/models/mt5/#unitorch.cli.models.mt5.modeling.MT5ForGeneration.generate",
-            "text": "<pre><code>generate(\n    input_ids: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 0,\n    decoder_end_token_id: Optional[int] = 1,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n)\n</code></pre> <p>Generate sequences using the MT5 model.</p> <p>Parameters:</p> Name Type Description Default <code>input_ids</code> <code>torch.Tensor</code> <p>Input token IDs.</p> required <code>num_beams</code> <code>int</code> <p>Number of beams for beam search. Defaults to 5.</p> <code>5</code> <code>decoder_start_token_id</code> <code>int</code> <p>Decoder start token ID. Defaults to 0.</p> <code>0</code> <code>decoder_end_token_id</code> <code>int</code> <p>Decoder end token ID. Defaults to 1.</p> <code>1</code> <code>num_return_sequences</code> <code>int</code> <p>Number of generated sequences to return. Defaults to 1.</p> <code>1</code> <code>min_gen_seq_length</code> <code>int</code> <p>Minimum generation sequence length. Defaults to 0.</p> <code>0</code> <code>max_gen_seq_length</code> <code>int</code> <p>Maximum generation sequence length. Defaults to 48.</p> <code>48</code> <code>repetition_penalty</code> <code>float</code> <p>Repetition penalty. Defaults to 1.0.</p> <code>1.0</code> <code>no_repeat_ngram_size</code> <code>int</code> <p>Size of n-grams to prevent repetition. Defaults to 0.</p> <code>0</code> <code>early_stopping</code> <code>bool</code> <p>Whether to perform early stopping. Defaults to True.</p> <code>True</code> <code>length_penalty</code> <code>float</code> <p>Length penalty. Defaults to 1.0.</p> <code>1.0</code> <code>num_beam_groups</code> <code>int</code> <p>Number of beam groups for diverse beam search. Defaults to 1.</p> <code>1</code> <code>diversity_penalty</code> <code>float</code> <p>Diversity penalty for diverse beam search. Defaults to 0.0.</p> <code>0.0</code> <code>do_sample</code> <code>bool</code> <p>Whether to use sampling for generation. Defaults to False.</p> <code>False</code> <code>temperature</code> <code>float</code> <p>Sampling temperature. Defaults to 1.0.</p> <code>1.0</code> <code>top_k</code> <code>int</code> <p>Top-k sampling parameter. Defaults to 50.</p> <code>50</code> <code>top_p</code> <code>float</code> <p>Top-p sampling parameter. Defaults to 1.0.</p> <code>1.0</code> <p>Returns:</p> Name Type Description <code>GenerationOutputs</code> <p>The generation outputs.</p> Source code in <code>src/unitorch/cli/models/mt5/modeling.py</code> <pre><code>@add_default_section_for_function(\"core/model/generation/mt5\")\n@torch.no_grad()\n@autocast()\ndef generate(\n    self,\n    input_ids: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 0,\n    decoder_end_token_id: Optional[int] = 1,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n):\n\"\"\"\n    Generate sequences using the MT5 model.\n\n    Args:\n        input_ids (torch.Tensor): Input token IDs.\n        num_beams (int, optional): Number of beams for beam search. Defaults to 5.\n        decoder_start_token_id (int, optional): Decoder start token ID. Defaults to 0.\n        decoder_end_token_id (int, optional): Decoder end token ID. Defaults to 1.\n        num_return_sequences (int, optional): Number of generated sequences to return. Defaults to 1.\n        min_gen_seq_length (int, optional): Minimum generation sequence length. Defaults to 0.\n        max_gen_seq_length (int, optional): Maximum generation sequence length. Defaults to 48.\n        repetition_penalty (float, optional): Repetition penalty. Defaults to 1.0.\n        no_repeat_ngram_size (int, optional): Size of n-grams to prevent repetition. Defaults to 0.\n        early_stopping (bool, optional): Whether to perform early stopping. Defaults to True.\n        length_penalty (float, optional): Length penalty. Defaults to 1.0.\n        num_beam_groups (int, optional): Number of beam groups for diverse beam search. Defaults to 1.\n        diversity_penalty (float, optional): Diversity penalty for diverse beam search. Defaults to 0.0.\n        do_sample (bool, optional): Whether to use sampling for generation. Defaults to False.\n        temperature (float, optional): Sampling temperature. Defaults to 1.0.\n        top_k (int, optional): Top-k sampling parameter. Defaults to 50.\n        top_p (float, optional): Top-p sampling parameter. Defaults to 1.0.\n\n    Returns:\n        GenerationOutputs: The generation outputs.\n    \"\"\"\n    outputs = super().generate(\n        input_ids,\n        num_beams=num_beams,\n        decoder_start_token_id=decoder_start_token_id,\n        decoder_end_token_id=decoder_end_token_id,\n        num_return_sequences=num_return_sequences,\n        min_gen_seq_length=min_gen_seq_length,\n        max_gen_seq_length=max_gen_seq_length,\n        repetition_penalty=repetition_penalty,\n        no_repeat_ngram_size=no_repeat_ngram_size,\n        early_stopping=early_stopping,\n        length_penalty=length_penalty,\n        num_beam_groups=num_beam_groups,\n        diversity_penalty=diversity_penalty,\n        do_sample=do_sample,\n        temperature=temperature,\n        top_k=top_k,\n        top_p=top_p,\n    )\n\n    return GenerationOutputs(\n        sequences=outputs.sequences,\n        sequences_scores=outputs.sequences_scores,\n    )\n</code></pre>",
+            "text": "<pre><code>generate(\n    input_ids: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 0,\n    decoder_end_token_id: Optional[\n        Union[int, List[int]]\n    ] = 1,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n)\n</code></pre> <p>Generate sequences using the MT5 model.</p> <p>Parameters:</p> Name Type Description Default <code>input_ids</code> <code>torch.Tensor</code> <p>Input token IDs.</p> required <code>num_beams</code> <code>int</code> <p>Number of beams for beam search. Defaults to 5.</p> <code>5</code> <code>decoder_start_token_id</code> <code>int</code> <p>Decoder start token ID. Defaults to 0.</p> <code>0</code> <code>decoder_end_token_id</code> <code>int or List[int]</code> <p>The ID(s) of the decoder end token(s). Defaults to 1.</p> <code>1</code> <code>num_return_sequences</code> <code>int</code> <p>Number of generated sequences to return. Defaults to 1.</p> <code>1</code> <code>min_gen_seq_length</code> <code>int</code> <p>Minimum generation sequence length. Defaults to 0.</p> <code>0</code> <code>max_gen_seq_length</code> <code>int</code> <p>Maximum generation sequence length. Defaults to 48.</p> <code>48</code> <code>repetition_penalty</code> <code>float</code> <p>Repetition penalty. Defaults to 1.0.</p> <code>1.0</code> <code>no_repeat_ngram_size</code> <code>int</code> <p>Size of n-grams to prevent repetition. Defaults to 0.</p> <code>0</code> <code>early_stopping</code> <code>bool</code> <p>Whether to perform early stopping. Defaults to True.</p> <code>True</code> <code>length_penalty</code> <code>float</code> <p>Length penalty. Defaults to 1.0.</p> <code>1.0</code> <code>num_beam_groups</code> <code>int</code> <p>Number of beam groups for diverse beam search. Defaults to 1.</p> <code>1</code> <code>diversity_penalty</code> <code>float</code> <p>Diversity penalty for diverse beam search. Defaults to 0.0.</p> <code>0.0</code> <code>do_sample</code> <code>bool</code> <p>Whether to use sampling for generation. Defaults to False.</p> <code>False</code> <code>temperature</code> <code>float</code> <p>Sampling temperature. Defaults to 1.0.</p> <code>1.0</code> <code>top_k</code> <code>int</code> <p>Top-k sampling parameter. Defaults to 50.</p> <code>50</code> <code>top_p</code> <code>float</code> <p>Top-p sampling parameter. Defaults to 1.0.</p> <code>1.0</code> <p>Returns:</p> Name Type Description <code>GenerationOutputs</code> <p>The generation outputs.</p> Source code in <code>src/unitorch/cli/models/mt5/modeling.py</code> <pre><code>@add_default_section_for_function(\"core/model/generation/mt5\")\n@torch.no_grad()\n@autocast()\ndef generate(\n    self,\n    input_ids: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 0,\n    decoder_end_token_id: Optional[Union[int, List[int]]] = 1,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n):\n\"\"\"\n    Generate sequences using the MT5 model.\n\n    Args:\n        input_ids (torch.Tensor): Input token IDs.\n        num_beams (int, optional): Number of beams for beam search. Defaults to 5.\n        decoder_start_token_id (int, optional): Decoder start token ID. Defaults to 0.\n        decoder_end_token_id (int or List[int], optional): The ID(s) of the decoder end token(s). Defaults to 1.\n        num_return_sequences (int, optional): Number of generated sequences to return. Defaults to 1.\n        min_gen_seq_length (int, optional): Minimum generation sequence length. Defaults to 0.\n        max_gen_seq_length (int, optional): Maximum generation sequence length. Defaults to 48.\n        repetition_penalty (float, optional): Repetition penalty. Defaults to 1.0.\n        no_repeat_ngram_size (int, optional): Size of n-grams to prevent repetition. Defaults to 0.\n        early_stopping (bool, optional): Whether to perform early stopping. Defaults to True.\n        length_penalty (float, optional): Length penalty. Defaults to 1.0.\n        num_beam_groups (int, optional): Number of beam groups for diverse beam search. Defaults to 1.\n        diversity_penalty (float, optional): Diversity penalty for diverse beam search. Defaults to 0.0.\n        do_sample (bool, optional): Whether to use sampling for generation. Defaults to False.\n        temperature (float, optional): Sampling temperature. Defaults to 1.0.\n        top_k (int, optional): Top-k sampling parameter. Defaults to 50.\n        top_p (float, optional): Top-p sampling parameter. Defaults to 1.0.\n\n    Returns:\n        GenerationOutputs: The generation outputs.\n    \"\"\"\n    outputs = super().generate(\n        input_ids,\n        num_beams=num_beams,\n        decoder_start_token_id=decoder_start_token_id,\n        decoder_end_token_id=decoder_end_token_id,\n        num_return_sequences=num_return_sequences,\n        min_gen_seq_length=min_gen_seq_length,\n        max_gen_seq_length=max_gen_seq_length,\n        repetition_penalty=repetition_penalty,\n        no_repeat_ngram_size=no_repeat_ngram_size,\n        early_stopping=early_stopping,\n        length_penalty=length_penalty,\n        num_beam_groups=num_beam_groups,\n        diversity_penalty=diversity_penalty,\n        do_sample=do_sample,\n        temperature=temperature,\n        top_k=top_k,\n        top_p=top_p,\n    )\n\n    return GenerationOutputs(\n        sequences=outputs.sequences,\n        sequences_scores=outputs.sequences_scores,\n    )\n</code></pre>",
             "title": "generate"
         },
         {
             "location": "cli/models/peft/",
             "text": "",
             "title": "unitorch.cli.models.peft"
         },
@@ -932,15 +967,15 @@
         {
             "location": "cli/models/peft/#unitorch.cli.models.peft.modeling_bloom.BloomAdaLoraForGeneration.from_core_configure",
             "text": "<pre><code>from_core_configure(config, **kwargs)\n</code></pre> <p>Create an instance of BloomAdaLoraForGeneration from a core configuration.</p> <p>Parameters:</p> Name Type Description Default <code>config</code> <p>The core configuration.</p> required <code>**kwargs</code> <p>Additional keyword arguments.</p> <code>{}</code> <p>Returns:</p> Name Type Description <code>BloomAdaLoraForGeneration</code> <p>The initialized BloomAdaLoraForGeneration instance.</p> Source code in <code>src/unitorch/cli/models/peft/modeling_bloom.py</code> <pre><code>@classmethod\n@add_default_section_for_init(\"core/model/generation/peft/adalora/bloom\")\ndef from_core_configure(cls, config, **kwargs):\n\"\"\"\n    Create an instance of BloomAdaLoraForGeneration from a core configuration.\n\n    Args:\n        config: The core configuration.\n        **kwargs: Additional keyword arguments.\n\n    Returns:\n        BloomAdaLoraForGeneration: The initialized BloomAdaLoraForGeneration instance.\n    \"\"\"\n    config.set_default_section(\"core/model/generation/peft/adalora/bloom\")\n    pretrained_name = config.getoption(\"pretrained_name\", \"default-bloom\")\n    config_path = config.getoption(\"config_path\", None)\n    config_path = pop_value(\n        config_path,\n        nested_dict_value(pretrained_bloom_infos, pretrained_name, \"config\"),\n    )\n    config_path = cached_path(config_path)\n\n    target_r = config.getoption(\"target_r\", 8)\n    init_r = config.getoption(\"init_r\", 12)\n    tinit = config.getoption(\"tinit\", 0)\n    tfinal = config.getoption(\"tfinal\", 0)\n    deltaT = config.getoption(\"deltaT\", 1)\n    beta1 = config.getoption(\"beta1\", 0.85)\n    beta2 = config.getoption(\"beta2\", 0.85)\n    orth_reg_weight = config.getoption(\"orth_reg_weight\", 0.5)\n    total_step = config.getoption(\"total_step\", None)\n    rank_pattern = config.getoption(\"rank_pattern\", None)\n\n    gradient_checkpointing = config.getoption(\"gradient_checkpointing\", False)\n\n    inst = cls(\n        config_path,\n        target_r=target_r,\n        init_r=init_r,\n        tinit=tinit,\n        tfinal=tfinal,\n        deltaT=deltaT,\n        beta1=beta1,\n        beta2=beta2,\n        orth_reg_weight=orth_reg_weight,\n        total_step=total_step,\n        rank_pattern=rank_pattern,\n        gradient_checkpointing=gradient_checkpointing,\n    )\n\n    weight_path = []\n    pretrained_weight_path = config.getoption(\"pretrained_weight_path\", None)\n    pretrained_weight_path = pop_value(\n        pretrained_weight_path,\n        nested_dict_value(pretrained_bloom_infos, pretrained_name, \"weight\"),\n        check_none=False,\n    )\n    if pretrained_weight_path is not None:\n        if isinstance(pretrained_weight_path, str):\n            weight_path.append(pretrained_weight_path)\n        elif isinstance(pretrained_weight_path, list):\n            weight_path.extend(pretrained_weight_path)\n\n    pretrained_adalora_weight_path = config.getoption(\n        \"pretrained_adalora_weight_path\", None\n    )\n    if pretrained_adalora_weight_path is not None:\n        weight_path.append(pretrained_adalora_weight_path)\n\n    if len(weight_path) &gt; 0:\n        inst.from_pretrained(\n            weight_path=weight_path,\n        )\n\n    return inst\n</code></pre>",
             "title": "from_core_configure  <code>classmethod</code>"
         },
         {
             "location": "cli/models/peft/#unitorch.cli.models.peft.modeling_bloom.BloomAdaLoraForGeneration.generate",
-            "text": "<pre><code>generate(\n    input_ids: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 1,\n    decoder_end_token_id: Optional[int] = 2,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n)\n</code></pre> <p>Generate sequences using the Bloom model.</p> <p>Parameters:</p> Name Type Description Default <code>input_ids</code> <code>torch.Tensor</code> <p>Input token IDs.</p> required <code>num_beams</code> <code>int</code> <p>Number of beams for beam search. Defaults to 5.</p> <code>5</code> <code>decoder_start_token_id</code> <code>int</code> <p>Decoder start token ID. Defaults to 0.</p> <code>1</code> <code>decoder_end_token_id</code> <code>int</code> <p>Decoder end token ID. Defaults to 1.</p> <code>2</code> <code>num_return_sequences</code> <code>int</code> <p>Number of generated sequences to return. Defaults to 1.</p> <code>1</code> <code>min_gen_seq_length</code> <code>int</code> <p>Minimum generation sequence length. Defaults to 0.</p> <code>0</code> <code>max_gen_seq_length</code> <code>int</code> <p>Maximum generation sequence length. Defaults to 48.</p> <code>48</code> <code>repetition_penalty</code> <code>float</code> <p>Repetition penalty. Defaults to 1.0.</p> <code>1.0</code> <code>no_repeat_ngram_size</code> <code>int</code> <p>Size of n-grams to prevent repetition. Defaults to 0.</p> <code>0</code> <code>early_stopping</code> <code>bool</code> <p>Whether to perform early stopping. Defaults to True.</p> <code>True</code> <code>length_penalty</code> <code>float</code> <p>Length penalty. Defaults to 1.0.</p> <code>1.0</code> <code>num_beam_groups</code> <code>int</code> <p>Number of beam groups for diverse beam search. Defaults to 1.</p> <code>1</code> <code>diversity_penalty</code> <code>float</code> <p>Diversity penalty for diverse beam search. Defaults to 0.0.</p> <code>0.0</code> <code>do_sample</code> <code>bool</code> <p>Whether to use sampling for generation. Defaults to False.</p> <code>False</code> <code>temperature</code> <code>float</code> <p>Sampling temperature. Defaults to 1.0.</p> <code>1.0</code> <code>top_k</code> <code>int</code> <p>Top-k sampling parameter. Defaults to 50.</p> <code>50</code> <code>top_p</code> <code>float</code> <p>Top-p sampling parameter. Defaults to 1.0.</p> <code>1.0</code> <p>Returns:</p> Name Type Description <code>GenerationOutputs</code> <p>The generation outputs.</p> Source code in <code>src/unitorch/cli/models/peft/modeling_bloom.py</code> <pre><code>@add_default_section_for_function(\"core/model/generation/peft/adalora/bloom\")\n@torch.no_grad()\n@autocast()\ndef generate(\n    self,\n    input_ids: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 1,\n    decoder_end_token_id: Optional[int] = 2,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n):\n\"\"\"\n    Generate sequences using the Bloom model.\n\n    Args:\n        input_ids (torch.Tensor): Input token IDs.\n        num_beams (int, optional): Number of beams for beam search. Defaults to 5.\n        decoder_start_token_id (int, optional): Decoder start token ID. Defaults to 0.\n        decoder_end_token_id (int, optional): Decoder end token ID. Defaults to 1.\n        num_return_sequences (int, optional): Number of generated sequences to return. Defaults to 1.\n        min_gen_seq_length (int, optional): Minimum generation sequence length. Defaults to 0.\n        max_gen_seq_length (int, optional): Maximum generation sequence length. Defaults to 48.\n        repetition_penalty (float, optional): Repetition penalty. Defaults to 1.0.\n        no_repeat_ngram_size (int, optional): Size of n-grams to prevent repetition. Defaults to 0.\n        early_stopping (bool, optional): Whether to perform early stopping. Defaults to True.\n        length_penalty (float, optional): Length penalty. Defaults to 1.0.\n        num_beam_groups (int, optional): Number of beam groups for diverse beam search. Defaults to 1.\n        diversity_penalty (float, optional): Diversity penalty for diverse beam search. Defaults to 0.0.\n        do_sample (bool, optional): Whether to use sampling for generation. Defaults to False.\n        temperature (float, optional): Sampling temperature. Defaults to 1.0.\n        top_k (int, optional): Top-k sampling parameter. Defaults to 50.\n        top_p (float, optional): Top-p sampling parameter. Defaults to 1.0.\n\n    Returns:\n        GenerationOutputs: The generation outputs.\n    \"\"\"\n    outputs = super().generate(\n        input_ids,\n        num_beams=num_beams,\n        decoder_start_token_id=decoder_start_token_id,\n        decoder_end_token_id=decoder_end_token_id,\n        num_return_sequences=num_return_sequences,\n        min_gen_seq_length=min_gen_seq_length,\n        max_gen_seq_length=max_gen_seq_length,\n        repetition_penalty=repetition_penalty,\n        no_repeat_ngram_size=no_repeat_ngram_size,\n        early_stopping=early_stopping,\n        length_penalty=length_penalty,\n        num_beam_groups=num_beam_groups,\n        diversity_penalty=diversity_penalty,\n        do_sample=do_sample,\n        temperature=temperature,\n        top_k=top_k,\n        top_p=top_p,\n    )\n\n    return GenerationOutputs(\n        sequences=outputs.sequences,\n        sequences_scores=outputs.sequences_scores,\n    )\n</code></pre>",
+            "text": "<pre><code>generate(\n    input_ids: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 1,\n    decoder_end_token_id: Optional[\n        Union[int, List[int]]\n    ] = 2,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n)\n</code></pre> <p>Generate sequences using the Bloom model.</p> <p>Parameters:</p> Name Type Description Default <code>input_ids</code> <code>torch.Tensor</code> <p>Input token IDs.</p> required <code>num_beams</code> <code>int</code> <p>Number of beams for beam search. Defaults to 5.</p> <code>5</code> <code>decoder_start_token_id</code> <code>int</code> <p>Decoder start token ID. Defaults to 0.</p> <code>1</code> <code>decoder_end_token_id</code> <code>int or List[int]</code> <p>The ID(s) of the decoder end token(s). Defaults to 1.</p> <code>2</code> <code>num_return_sequences</code> <code>int</code> <p>Number of generated sequences to return. Defaults to 1.</p> <code>1</code> <code>min_gen_seq_length</code> <code>int</code> <p>Minimum generation sequence length. Defaults to 0.</p> <code>0</code> <code>max_gen_seq_length</code> <code>int</code> <p>Maximum generation sequence length. Defaults to 48.</p> <code>48</code> <code>repetition_penalty</code> <code>float</code> <p>Repetition penalty. Defaults to 1.0.</p> <code>1.0</code> <code>no_repeat_ngram_size</code> <code>int</code> <p>Size of n-grams to prevent repetition. Defaults to 0.</p> <code>0</code> <code>early_stopping</code> <code>bool</code> <p>Whether to perform early stopping. Defaults to True.</p> <code>True</code> <code>length_penalty</code> <code>float</code> <p>Length penalty. Defaults to 1.0.</p> <code>1.0</code> <code>num_beam_groups</code> <code>int</code> <p>Number of beam groups for diverse beam search. Defaults to 1.</p> <code>1</code> <code>diversity_penalty</code> <code>float</code> <p>Diversity penalty for diverse beam search. Defaults to 0.0.</p> <code>0.0</code> <code>do_sample</code> <code>bool</code> <p>Whether to use sampling for generation. Defaults to False.</p> <code>False</code> <code>temperature</code> <code>float</code> <p>Sampling temperature. Defaults to 1.0.</p> <code>1.0</code> <code>top_k</code> <code>int</code> <p>Top-k sampling parameter. Defaults to 50.</p> <code>50</code> <code>top_p</code> <code>float</code> <p>Top-p sampling parameter. Defaults to 1.0.</p> <code>1.0</code> <p>Returns:</p> Name Type Description <code>GenerationOutputs</code> <p>The generation outputs.</p> Source code in <code>src/unitorch/cli/models/peft/modeling_bloom.py</code> <pre><code>@add_default_section_for_function(\"core/model/generation/peft/adalora/bloom\")\n@torch.no_grad()\n@autocast()\ndef generate(\n    self,\n    input_ids: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 1,\n    decoder_end_token_id: Optional[Union[int, List[int]]] = 2,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n):\n\"\"\"\n    Generate sequences using the Bloom model.\n\n    Args:\n        input_ids (torch.Tensor): Input token IDs.\n        num_beams (int, optional): Number of beams for beam search. Defaults to 5.\n        decoder_start_token_id (int, optional): Decoder start token ID. Defaults to 0.\n        decoder_end_token_id (int or List[int], optional): The ID(s) of the decoder end token(s). Defaults to 1.\n        num_return_sequences (int, optional): Number of generated sequences to return. Defaults to 1.\n        min_gen_seq_length (int, optional): Minimum generation sequence length. Defaults to 0.\n        max_gen_seq_length (int, optional): Maximum generation sequence length. Defaults to 48.\n        repetition_penalty (float, optional): Repetition penalty. Defaults to 1.0.\n        no_repeat_ngram_size (int, optional): Size of n-grams to prevent repetition. Defaults to 0.\n        early_stopping (bool, optional): Whether to perform early stopping. Defaults to True.\n        length_penalty (float, optional): Length penalty. Defaults to 1.0.\n        num_beam_groups (int, optional): Number of beam groups for diverse beam search. Defaults to 1.\n        diversity_penalty (float, optional): Diversity penalty for diverse beam search. Defaults to 0.0.\n        do_sample (bool, optional): Whether to use sampling for generation. Defaults to False.\n        temperature (float, optional): Sampling temperature. Defaults to 1.0.\n        top_k (int, optional): Top-k sampling parameter. Defaults to 50.\n        top_p (float, optional): Top-p sampling parameter. Defaults to 1.0.\n\n    Returns:\n        GenerationOutputs: The generation outputs.\n    \"\"\"\n    outputs = super().generate(\n        input_ids,\n        num_beams=num_beams,\n        decoder_start_token_id=decoder_start_token_id,\n        decoder_end_token_id=decoder_end_token_id,\n        num_return_sequences=num_return_sequences,\n        min_gen_seq_length=min_gen_seq_length,\n        max_gen_seq_length=max_gen_seq_length,\n        repetition_penalty=repetition_penalty,\n        no_repeat_ngram_size=no_repeat_ngram_size,\n        early_stopping=early_stopping,\n        length_penalty=length_penalty,\n        num_beam_groups=num_beam_groups,\n        diversity_penalty=diversity_penalty,\n        do_sample=do_sample,\n        temperature=temperature,\n        top_k=top_k,\n        top_p=top_p,\n    )\n\n    return GenerationOutputs(\n        sequences=outputs.sequences,\n        sequences_scores=outputs.sequences_scores,\n    )\n</code></pre>",
             "title": "generate"
         },
         {
             "location": "cli/models/peft/#bloomloraforclassification",
             "text": "<p>Tip</p> <p><code>classification/peft/lora/bloom</code> is the section for configuration of BloomLoraForClassification.</p> <p>         Bases: <code>_BloomLoraForClassification</code></p> <p>Initialize the BloomLoraForClassification model.</p> <p>Parameters:</p> Name Type Description Default <code>config_path</code> <code>str</code> <p>The path to the model configuration file.</p> required <code>lora_r</code> <code>int</code> <p>The number of Lora ranks. Defaults to 16.</p> <code>16</code> <code>lora_alpha</code> <code>int</code> <p>The Lora alpha value. Defaults to 32.</p> <code>32</code> <code>lora_dropout</code> <code>float</code> <p>The Lora dropout rate. Defaults to 0.05.</p> <code>0.05</code> <code>fan_in_fan_out</code> <code>bool</code> <p>Whether to use fan-in/fan-out weight initialization. Defaults to True.</p> <code>True</code> <code>target_modules</code> <code>Union[List[str], str]</code> <p>The target modules for Lora regularization. Defaults to [\"q_proj\", \"v_proj\"].</p> <code>['query_key_value']</code> <code>num_classes</code> <code>int</code> <p>The number of classes. Defaults to 1.</p> <code>1</code> <code>gradient_checkpointing</code> <code>bool</code> <p>Whether to use gradient checkpointing during training. Defaults to False.</p> <code>False</code> Source code in <code>src/unitorch/cli/models/peft/modeling_bloom.py</code> <pre><code>def __init__(\n    self,\n    config_path: str,\n    lora_r: Optional[int] = 16,\n    lora_alpha: Optional[int] = 32,\n    lora_dropout: Optional[float] = 0.05,\n    fan_in_fan_out: Optional[bool] = True,\n    target_modules: Optional[Union[List[str], str]] = [\"query_key_value\"],\n    num_classes: Optional[int] = 1,\n    gradient_checkpointing: Optional[bool] = False,\n):\n\"\"\"\n    Initialize the BloomLoraForClassification model.\n\n    Args:\n        config_path (str): The path to the model configuration file.\n        lora_r (int, optional): The number of Lora ranks. Defaults to 16.\n        lora_alpha (int, optional): The Lora alpha value. Defaults to 32.\n        lora_dropout (float, optional): The Lora dropout rate. Defaults to 0.05.\n        fan_in_fan_out (bool, optional): Whether to use fan-in/fan-out weight initialization. Defaults to True.\n        target_modules (Union[List[str], str], optional): The target modules for Lora regularization. Defaults to [\"q_proj\", \"v_proj\"].\n        num_classes (int, optional): The number of classes. Defaults to 1.\n        gradient_checkpointing (bool, optional): Whether to use gradient checkpointing during training. Defaults to False.\n    \"\"\"\n    super().__init__(\n        config_path=config_path,\n        lora_r=lora_r,\n        lora_alpha=lora_alpha,\n        lora_dropout=lora_dropout,\n        fan_in_fan_out=fan_in_fan_out,\n        target_modules=target_modules,\n        num_classes=num_classes,\n        gradient_checkpointing=gradient_checkpointing,\n    )\n</code></pre>",
             "title": "BloomLoraForClassification"
         },
@@ -967,15 +1002,15 @@
         {
             "location": "cli/models/peft/#unitorch.cli.models.peft.modeling_bloom.BloomLoraForGeneration.from_core_configure",
             "text": "<pre><code>from_core_configure(config, **kwargs)\n</code></pre> <p>Create an instance of BloomLoraForGeneration from a core configuration.</p> <p>Parameters:</p> Name Type Description Default <code>config</code> <p>The core configuration.</p> required <code>**kwargs</code> <p>Additional keyword arguments.</p> <code>{}</code> <p>Returns:</p> Name Type Description <code>BloomLoraForGeneration</code> <p>The initialized BloomLoraForGeneration instance.</p> Source code in <code>src/unitorch/cli/models/peft/modeling_bloom.py</code> <pre><code>@classmethod\n@add_default_section_for_init(\"core/model/generation/peft/lora/bloom\")\ndef from_core_configure(cls, config, **kwargs):\n\"\"\"\n    Create an instance of BloomLoraForGeneration from a core configuration.\n\n    Args:\n        config: The core configuration.\n        **kwargs: Additional keyword arguments.\n\n    Returns:\n        BloomLoraForGeneration: The initialized BloomLoraForGeneration instance.\n    \"\"\"\n    config.set_default_section(\"core/model/generation/peft/lora/bloom\")\n    pretrained_name = config.getoption(\"pretrained_name\", \"default-bloom\")\n    config_path = config.getoption(\"config_path\", None)\n    config_path = pop_value(\n        config_path,\n        nested_dict_value(pretrained_bloom_infos, pretrained_name, \"config\"),\n    )\n    config_path = cached_path(config_path)\n\n    lora_r = config.getoption(\"lora_r\", 16)\n    lora_alpha = config.getoption(\"lora_alpha\", 32)\n    lora_dropout = config.getoption(\"lora_dropout\", 0.05)\n    fan_in_fan_out = config.getoption(\"fan_in_fan_out\", True)\n    target_modules = config.getoption(\"target_modules\", [\"query_key_value\"])\n\n    gradient_checkpointing = config.getoption(\"gradient_checkpointing\", False)\n\n    inst = cls(\n        config_path,\n        lora_r=lora_r,\n        lora_alpha=lora_alpha,\n        lora_dropout=lora_dropout,\n        fan_in_fan_out=fan_in_fan_out,\n        target_modules=target_modules,\n        gradient_checkpointing=gradient_checkpointing,\n    )\n\n    weight_path = []\n    pretrained_weight_path = config.getoption(\"pretrained_weight_path\", None)\n    pretrained_weight_path = pop_value(\n        pretrained_weight_path,\n        nested_dict_value(pretrained_bloom_infos, pretrained_name, \"weight\"),\n        check_none=False,\n    )\n    if pretrained_weight_path is not None:\n        if isinstance(pretrained_weight_path, str):\n            weight_path.append(pretrained_weight_path)\n        elif isinstance(pretrained_weight_path, list):\n            weight_path.extend(pretrained_weight_path)\n\n    pretrained_lora_weight_path = config.getoption(\n        \"pretrained_lora_weight_path\", None\n    )\n    if pretrained_lora_weight_path is not None:\n        weight_path.append(pretrained_lora_weight_path)\n\n    if len(weight_path) &gt; 0:\n        inst.from_pretrained(\n            weight_path=weight_path,\n        )\n\n    return inst\n</code></pre>",
             "title": "from_core_configure  <code>classmethod</code>"
         },
         {
             "location": "cli/models/peft/#unitorch.cli.models.peft.modeling_bloom.BloomLoraForGeneration.generate",
-            "text": "<pre><code>generate(\n    input_ids: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 1,\n    decoder_end_token_id: Optional[int] = 2,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n)\n</code></pre> <p>Generate sequences using the Bloom model.</p> <p>Parameters:</p> Name Type Description Default <code>input_ids</code> <code>torch.Tensor</code> <p>Input token IDs.</p> required <code>num_beams</code> <code>int</code> <p>Number of beams for beam search. Defaults to 5.</p> <code>5</code> <code>decoder_start_token_id</code> <code>int</code> <p>Decoder start token ID. Defaults to 0.</p> <code>1</code> <code>decoder_end_token_id</code> <code>int</code> <p>Decoder end token ID. Defaults to 1.</p> <code>2</code> <code>num_return_sequences</code> <code>int</code> <p>Number of generated sequences to return. Defaults to 1.</p> <code>1</code> <code>min_gen_seq_length</code> <code>int</code> <p>Minimum generation sequence length. Defaults to 0.</p> <code>0</code> <code>max_gen_seq_length</code> <code>int</code> <p>Maximum generation sequence length. Defaults to 48.</p> <code>48</code> <code>repetition_penalty</code> <code>float</code> <p>Repetition penalty. Defaults to 1.0.</p> <code>1.0</code> <code>no_repeat_ngram_size</code> <code>int</code> <p>Size of n-grams to prevent repetition. Defaults to 0.</p> <code>0</code> <code>early_stopping</code> <code>bool</code> <p>Whether to perform early stopping. Defaults to True.</p> <code>True</code> <code>length_penalty</code> <code>float</code> <p>Length penalty. Defaults to 1.0.</p> <code>1.0</code> <code>num_beam_groups</code> <code>int</code> <p>Number of beam groups for diverse beam search. Defaults to 1.</p> <code>1</code> <code>diversity_penalty</code> <code>float</code> <p>Diversity penalty for diverse beam search. Defaults to 0.0.</p> <code>0.0</code> <code>do_sample</code> <code>bool</code> <p>Whether to use sampling for generation. Defaults to False.</p> <code>False</code> <code>temperature</code> <code>float</code> <p>Sampling temperature. Defaults to 1.0.</p> <code>1.0</code> <code>top_k</code> <code>int</code> <p>Top-k sampling parameter. Defaults to 50.</p> <code>50</code> <code>top_p</code> <code>float</code> <p>Top-p sampling parameter. Defaults to 1.0.</p> <code>1.0</code> <p>Returns:</p> Name Type Description <code>GenerationOutputs</code> <p>The generation outputs.</p> Source code in <code>src/unitorch/cli/models/peft/modeling_bloom.py</code> <pre><code>@add_default_section_for_function(\"core/model/generation/peft/lora/bloom\")\n@torch.no_grad()\n@autocast()\ndef generate(\n    self,\n    input_ids: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 1,\n    decoder_end_token_id: Optional[int] = 2,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n):\n\"\"\"\n    Generate sequences using the Bloom model.\n\n    Args:\n        input_ids (torch.Tensor): Input token IDs.\n        num_beams (int, optional): Number of beams for beam search. Defaults to 5.\n        decoder_start_token_id (int, optional): Decoder start token ID. Defaults to 0.\n        decoder_end_token_id (int, optional): Decoder end token ID. Defaults to 1.\n        num_return_sequences (int, optional): Number of generated sequences to return. Defaults to 1.\n        min_gen_seq_length (int, optional): Minimum generation sequence length. Defaults to 0.\n        max_gen_seq_length (int, optional): Maximum generation sequence length. Defaults to 48.\n        repetition_penalty (float, optional): Repetition penalty. Defaults to 1.0.\n        no_repeat_ngram_size (int, optional): Size of n-grams to prevent repetition. Defaults to 0.\n        early_stopping (bool, optional): Whether to perform early stopping. Defaults to True.\n        length_penalty (float, optional): Length penalty. Defaults to 1.0.\n        num_beam_groups (int, optional): Number of beam groups for diverse beam search. Defaults to 1.\n        diversity_penalty (float, optional): Diversity penalty for diverse beam search. Defaults to 0.0.\n        do_sample (bool, optional): Whether to use sampling for generation. Defaults to False.\n        temperature (float, optional): Sampling temperature. Defaults to 1.0.\n        top_k (int, optional): Top-k sampling parameter. Defaults to 50.\n        top_p (float, optional): Top-p sampling parameter. Defaults to 1.0.\n\n    Returns:\n        GenerationOutputs: The generation outputs.\n    \"\"\"\n    outputs = super().generate(\n        input_ids,\n        num_beams=num_beams,\n        decoder_start_token_id=decoder_start_token_id,\n        decoder_end_token_id=decoder_end_token_id,\n        num_return_sequences=num_return_sequences,\n        min_gen_seq_length=min_gen_seq_length,\n        max_gen_seq_length=max_gen_seq_length,\n        repetition_penalty=repetition_penalty,\n        no_repeat_ngram_size=no_repeat_ngram_size,\n        early_stopping=early_stopping,\n        length_penalty=length_penalty,\n        num_beam_groups=num_beam_groups,\n        diversity_penalty=diversity_penalty,\n        do_sample=do_sample,\n        temperature=temperature,\n        top_k=top_k,\n        top_p=top_p,\n    )\n\n    return GenerationOutputs(\n        sequences=outputs.sequences,\n        sequences_scores=outputs.sequences_scores,\n    )\n</code></pre>",
+            "text": "<pre><code>generate(\n    input_ids: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 1,\n    decoder_end_token_id: Optional[\n        Union[int, List[int]]\n    ] = 2,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n)\n</code></pre> <p>Generate sequences using the Bloom model.</p> <p>Parameters:</p> Name Type Description Default <code>input_ids</code> <code>torch.Tensor</code> <p>Input token IDs.</p> required <code>num_beams</code> <code>int</code> <p>Number of beams for beam search. Defaults to 5.</p> <code>5</code> <code>decoder_start_token_id</code> <code>int</code> <p>Decoder start token ID. Defaults to 0.</p> <code>1</code> <code>decoder_end_token_id</code> <code>int or List[int]</code> <p>The ID(s) of the decoder end token(s). Defaults to 1.</p> <code>2</code> <code>num_return_sequences</code> <code>int</code> <p>Number of generated sequences to return. Defaults to 1.</p> <code>1</code> <code>min_gen_seq_length</code> <code>int</code> <p>Minimum generation sequence length. Defaults to 0.</p> <code>0</code> <code>max_gen_seq_length</code> <code>int</code> <p>Maximum generation sequence length. Defaults to 48.</p> <code>48</code> <code>repetition_penalty</code> <code>float</code> <p>Repetition penalty. Defaults to 1.0.</p> <code>1.0</code> <code>no_repeat_ngram_size</code> <code>int</code> <p>Size of n-grams to prevent repetition. Defaults to 0.</p> <code>0</code> <code>early_stopping</code> <code>bool</code> <p>Whether to perform early stopping. Defaults to True.</p> <code>True</code> <code>length_penalty</code> <code>float</code> <p>Length penalty. Defaults to 1.0.</p> <code>1.0</code> <code>num_beam_groups</code> <code>int</code> <p>Number of beam groups for diverse beam search. Defaults to 1.</p> <code>1</code> <code>diversity_penalty</code> <code>float</code> <p>Diversity penalty for diverse beam search. Defaults to 0.0.</p> <code>0.0</code> <code>do_sample</code> <code>bool</code> <p>Whether to use sampling for generation. Defaults to False.</p> <code>False</code> <code>temperature</code> <code>float</code> <p>Sampling temperature. Defaults to 1.0.</p> <code>1.0</code> <code>top_k</code> <code>int</code> <p>Top-k sampling parameter. Defaults to 50.</p> <code>50</code> <code>top_p</code> <code>float</code> <p>Top-p sampling parameter. Defaults to 1.0.</p> <code>1.0</code> <p>Returns:</p> Name Type Description <code>GenerationOutputs</code> <p>The generation outputs.</p> Source code in <code>src/unitorch/cli/models/peft/modeling_bloom.py</code> <pre><code>@add_default_section_for_function(\"core/model/generation/peft/lora/bloom\")\n@torch.no_grad()\n@autocast()\ndef generate(\n    self,\n    input_ids: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 1,\n    decoder_end_token_id: Optional[Union[int, List[int]]] = 2,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n):\n\"\"\"\n    Generate sequences using the Bloom model.\n\n    Args:\n        input_ids (torch.Tensor): Input token IDs.\n        num_beams (int, optional): Number of beams for beam search. Defaults to 5.\n        decoder_start_token_id (int, optional): Decoder start token ID. Defaults to 0.\n        decoder_end_token_id (int or List[int], optional): The ID(s) of the decoder end token(s). Defaults to 1.\n        num_return_sequences (int, optional): Number of generated sequences to return. Defaults to 1.\n        min_gen_seq_length (int, optional): Minimum generation sequence length. Defaults to 0.\n        max_gen_seq_length (int, optional): Maximum generation sequence length. Defaults to 48.\n        repetition_penalty (float, optional): Repetition penalty. Defaults to 1.0.\n        no_repeat_ngram_size (int, optional): Size of n-grams to prevent repetition. Defaults to 0.\n        early_stopping (bool, optional): Whether to perform early stopping. Defaults to True.\n        length_penalty (float, optional): Length penalty. Defaults to 1.0.\n        num_beam_groups (int, optional): Number of beam groups for diverse beam search. Defaults to 1.\n        diversity_penalty (float, optional): Diversity penalty for diverse beam search. Defaults to 0.0.\n        do_sample (bool, optional): Whether to use sampling for generation. Defaults to False.\n        temperature (float, optional): Sampling temperature. Defaults to 1.0.\n        top_k (int, optional): Top-k sampling parameter. Defaults to 50.\n        top_p (float, optional): Top-p sampling parameter. Defaults to 1.0.\n\n    Returns:\n        GenerationOutputs: The generation outputs.\n    \"\"\"\n    outputs = super().generate(\n        input_ids,\n        num_beams=num_beams,\n        decoder_start_token_id=decoder_start_token_id,\n        decoder_end_token_id=decoder_end_token_id,\n        num_return_sequences=num_return_sequences,\n        min_gen_seq_length=min_gen_seq_length,\n        max_gen_seq_length=max_gen_seq_length,\n        repetition_penalty=repetition_penalty,\n        no_repeat_ngram_size=no_repeat_ngram_size,\n        early_stopping=early_stopping,\n        length_penalty=length_penalty,\n        num_beam_groups=num_beam_groups,\n        diversity_penalty=diversity_penalty,\n        do_sample=do_sample,\n        temperature=temperature,\n        top_k=top_k,\n        top_p=top_p,\n    )\n\n    return GenerationOutputs(\n        sequences=outputs.sequences,\n        sequences_scores=outputs.sequences_scores,\n    )\n</code></pre>",
             "title": "generate"
         },
         {
             "location": "cli/models/peft/#llamaadaloraforclassification",
             "text": "<p>Tip</p> <p><code>core/model/classification/peft/adalora/llama</code> is the section for configuration of LlamaAdaLoraForClassification.</p> <p>         Bases: <code>_LlamaAdaLoraForClassification</code></p> <p>LlamaAdaLora model for classification tasks.</p> <p>Initialize the LlamaAdaLoraForClassification model.</p> <p>Parameters:</p> Name Type Description Default <code>config_path</code> <code>str</code> <p>The path to the model configuration file.</p> required <code>target_r</code> <code>int</code> <p>The target rank. Defaults to 8.</p> <code>8</code> <code>init_r</code> <code>int</code> <p>The initial rank. Defaults to 12.</p> <code>12</code> <code>tinit</code> <code>int</code> <p>The initial temperature. Defaults to 0.</p> <code>0</code> <code>tfinal</code> <code>int</code> <p>The final temperature. Defaults to 0.</p> <code>0</code> <code>deltaT</code> <code>int</code> <p>The temperature change rate. Defaults to 1.</p> <code>1</code> <code>beta1</code> <code>float</code> <p>The value of beta1 for optimizer. Defaults to 0.85.</p> <code>0.85</code> <code>beta2</code> <code>float</code> <p>The value of beta2 for optimizer. Defaults to 0.85.</p> <code>0.85</code> <code>orth_reg_weight</code> <code>float</code> <p>The weight of the orthogonality regularization. Defaults to 0.5.</p> <code>0.5</code> <code>total_step</code> <code>int</code> <p>The total number of training steps. Defaults to None.</p> <code>None</code> <code>rank_pattern</code> <code>dict</code> <p>The rank pattern. Defaults to None.</p> <code>None</code> <code>num_classes</code> <code>int</code> <p>The number of classes. Defaults to 1.</p> <code>1</code> <code>gradient_checkpointing</code> <code>bool</code> <p>Whether to use gradient checkpointing during training. Defaults to False.</p> <code>False</code> Source code in <code>src/unitorch/cli/models/peft/modeling_llama.py</code> <pre><code>def __init__(\n    self,\n    config_path: str,\n    target_r: Optional[int] = 8,\n    init_r: Optional[int] = 12,\n    tinit: Optional[int] = 0,\n    tfinal: Optional[int] = 0,\n    deltaT: Optional[int] = 1,\n    beta1: Optional[float] = 0.85,\n    beta2: Optional[float] = 0.85,\n    orth_reg_weight: Optional[float] = 0.5,\n    total_step: Optional[int] = None,\n    rank_pattern: Optional[dict] = None,\n    num_classes: Optional[int] = 1,\n    gradient_checkpointing: Optional[bool] = False,\n):\n\"\"\"\n    Initialize the LlamaAdaLoraForClassification model.\n\n    Args:\n        config_path (str): The path to the model configuration file.\n        target_r (int, optional): The target rank. Defaults to 8.\n        init_r (int, optional): The initial rank. Defaults to 12.\n        tinit (int, optional): The initial temperature. Defaults to 0.\n        tfinal (int, optional): The final temperature. Defaults to 0.\n        deltaT (int, optional): The temperature change rate. Defaults to 1.\n        beta1 (float, optional): The value of beta1 for optimizer. Defaults to 0.85.\n        beta2 (float, optional): The value of beta2 for optimizer. Defaults to 0.85.\n        orth_reg_weight (float, optional): The weight of the orthogonality regularization. Defaults to 0.5.\n        total_step (int, optional): The total number of training steps. Defaults to None.\n        rank_pattern (dict, optional): The rank pattern. Defaults to None.\n        num_classes (int, optional): The number of classes. Defaults to 1.\n        gradient_checkpointing (bool, optional): Whether to use gradient checkpointing during training. Defaults to False.\n    \"\"\"\n    super().__init__(\n        config_path=config_path,\n        target_r=target_r,\n        init_r=init_r,\n        tinit=tinit,\n        tfinal=tfinal,\n        deltaT=deltaT,\n        beta1=beta1,\n        beta2=beta2,\n        orth_reg_weight=orth_reg_weight,\n        total_step=total_step,\n        rank_pattern=rank_pattern,\n        num_classes=num_classes,\n        gradient_checkpointing=gradient_checkpointing,\n    )\n</code></pre>",
             "title": "LlamaAdaLoraForClassification"
         },
@@ -1002,15 +1037,15 @@
         {
             "location": "cli/models/peft/#unitorch.cli.models.peft.modeling_llama.LlamaAdaLoraForGeneration.from_core_configure",
             "text": "<pre><code>from_core_configure(config, **kwargs)\n</code></pre> <p>Create an instance of LlamaAdaLoraForGeneration from a core configuration.</p> <p>Parameters:</p> Name Type Description Default <code>config</code> <p>The core configuration.</p> required <code>**kwargs</code> <p>Additional keyword arguments.</p> <code>{}</code> <p>Returns:</p> Name Type Description <code>LlamaAdaLoraForGeneration</code> <p>The initialized LlamaAdaLoraForGeneration instance.</p> Source code in <code>src/unitorch/cli/models/peft/modeling_llama.py</code> <pre><code>@classmethod\n@add_default_section_for_init(\"core/model/generation/peft/adalora/llama\")\ndef from_core_configure(cls, config, **kwargs):\n\"\"\"\n    Create an instance of LlamaAdaLoraForGeneration from a core configuration.\n\n    Args:\n        config: The core configuration.\n        **kwargs: Additional keyword arguments.\n\n    Returns:\n        LlamaAdaLoraForGeneration: The initialized LlamaAdaLoraForGeneration instance.\n    \"\"\"\n    config.set_default_section(\"core/model/generation/peft/adalora/llama\")\n    pretrained_name = config.getoption(\"pretrained_name\", \"default-llama\")\n    config_path = config.getoption(\"config_path\", None)\n    config_path = pop_value(\n        config_path,\n        nested_dict_value(pretrained_llama_infos, pretrained_name, \"config\"),\n    )\n    config_path = cached_path(config_path)\n\n    target_r = config.getoption(\"target_r\", 8)\n    init_r = config.getoption(\"init_r\", 12)\n    tinit = config.getoption(\"tinit\", 0)\n    tfinal = config.getoption(\"tfinal\", 0)\n    deltaT = config.getoption(\"deltaT\", 1)\n    beta1 = config.getoption(\"beta1\", 0.85)\n    beta2 = config.getoption(\"beta2\", 0.85)\n    orth_reg_weight = config.getoption(\"orth_reg_weight\", 0.5)\n    total_step = config.getoption(\"total_step\", None)\n    rank_pattern = config.getoption(\"rank_pattern\", None)\n\n    gradient_checkpointing = config.getoption(\"gradient_checkpointing\", False)\n\n    inst = cls(\n        config_path,\n        target_r=target_r,\n        init_r=init_r,\n        tinit=tinit,\n        tfinal=tfinal,\n        deltaT=deltaT,\n        beta1=beta1,\n        beta2=beta2,\n        orth_reg_weight=orth_reg_weight,\n        total_step=total_step,\n        rank_pattern=rank_pattern,\n        gradient_checkpointing=gradient_checkpointing,\n    )\n\n    weight_path = []\n    pretrained_weight_path = config.getoption(\"pretrained_weight_path\", None)\n    pretrained_weight_path = pop_value(\n        pretrained_weight_path,\n        nested_dict_value(pretrained_llama_infos, pretrained_name, \"weight\"),\n        check_none=False,\n    )\n    if pretrained_weight_path is not None:\n        if isinstance(pretrained_weight_path, str):\n            weight_path.append(pretrained_weight_path)\n        elif isinstance(pretrained_weight_path, list):\n            weight_path.extend(pretrained_weight_path)\n\n    pretrained_adalora_weight_path = config.getoption(\n        \"pretrained_adalora_weight_path\", None\n    )\n    if pretrained_adalora_weight_path is not None:\n        weight_path.append(pretrained_adalora_weight_path)\n\n    if len(weight_path) &gt; 0:\n        inst.from_pretrained(\n            weight_path=weight_path,\n        )\n\n    return inst\n</code></pre>",
             "title": "from_core_configure  <code>classmethod</code>"
         },
         {
             "location": "cli/models/peft/#unitorch.cli.models.peft.modeling_llama.LlamaAdaLoraForGeneration.generate",
-            "text": "<pre><code>generate(\n    input_ids: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 1,\n    decoder_end_token_id: Optional[int] = 2,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n)\n</code></pre> <p>Generate sequences using the Llama model.</p> <p>Parameters:</p> Name Type Description Default <code>input_ids</code> <code>torch.Tensor</code> <p>Input token IDs.</p> required <code>num_beams</code> <code>int</code> <p>Number of beams for beam search. Defaults to 5.</p> <code>5</code> <code>decoder_start_token_id</code> <code>int</code> <p>Decoder start token ID. Defaults to 0.</p> <code>1</code> <code>decoder_end_token_id</code> <code>int</code> <p>Decoder end token ID. Defaults to 1.</p> <code>2</code> <code>num_return_sequences</code> <code>int</code> <p>Number of generated sequences to return. Defaults to 1.</p> <code>1</code> <code>min_gen_seq_length</code> <code>int</code> <p>Minimum generation sequence length. Defaults to 0.</p> <code>0</code> <code>max_gen_seq_length</code> <code>int</code> <p>Maximum generation sequence length. Defaults to 48.</p> <code>48</code> <code>repetition_penalty</code> <code>float</code> <p>Repetition penalty. Defaults to 1.0.</p> <code>1.0</code> <code>no_repeat_ngram_size</code> <code>int</code> <p>Size of n-grams to prevent repetition. Defaults to 0.</p> <code>0</code> <code>early_stopping</code> <code>bool</code> <p>Whether to perform early stopping. Defaults to True.</p> <code>True</code> <code>length_penalty</code> <code>float</code> <p>Length penalty. Defaults to 1.0.</p> <code>1.0</code> <code>num_beam_groups</code> <code>int</code> <p>Number of beam groups for diverse beam search. Defaults to 1.</p> <code>1</code> <code>diversity_penalty</code> <code>float</code> <p>Diversity penalty for diverse beam search. Defaults to 0.0.</p> <code>0.0</code> <code>do_sample</code> <code>bool</code> <p>Whether to use sampling for generation. Defaults to False.</p> <code>False</code> <code>temperature</code> <code>float</code> <p>Sampling temperature. Defaults to 1.0.</p> <code>1.0</code> <code>top_k</code> <code>int</code> <p>Top-k sampling parameter. Defaults to 50.</p> <code>50</code> <code>top_p</code> <code>float</code> <p>Top-p sampling parameter. Defaults to 1.0.</p> <code>1.0</code> <p>Returns:</p> Name Type Description <code>GenerationOutputs</code> <p>The generation outputs.</p> Source code in <code>src/unitorch/cli/models/peft/modeling_llama.py</code> <pre><code>@add_default_section_for_function(\"core/model/generation/peft/adalora/llama\")\n@torch.no_grad()\n@autocast()\ndef generate(\n    self,\n    input_ids: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 1,\n    decoder_end_token_id: Optional[int] = 2,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n):\n\"\"\"\n    Generate sequences using the Llama model.\n\n    Args:\n        input_ids (torch.Tensor): Input token IDs.\n        num_beams (int, optional): Number of beams for beam search. Defaults to 5.\n        decoder_start_token_id (int, optional): Decoder start token ID. Defaults to 0.\n        decoder_end_token_id (int, optional): Decoder end token ID. Defaults to 1.\n        num_return_sequences (int, optional): Number of generated sequences to return. Defaults to 1.\n        min_gen_seq_length (int, optional): Minimum generation sequence length. Defaults to 0.\n        max_gen_seq_length (int, optional): Maximum generation sequence length. Defaults to 48.\n        repetition_penalty (float, optional): Repetition penalty. Defaults to 1.0.\n        no_repeat_ngram_size (int, optional): Size of n-grams to prevent repetition. Defaults to 0.\n        early_stopping (bool, optional): Whether to perform early stopping. Defaults to True.\n        length_penalty (float, optional): Length penalty. Defaults to 1.0.\n        num_beam_groups (int, optional): Number of beam groups for diverse beam search. Defaults to 1.\n        diversity_penalty (float, optional): Diversity penalty for diverse beam search. Defaults to 0.0.\n        do_sample (bool, optional): Whether to use sampling for generation. Defaults to False.\n        temperature (float, optional): Sampling temperature. Defaults to 1.0.\n        top_k (int, optional): Top-k sampling parameter. Defaults to 50.\n        top_p (float, optional): Top-p sampling parameter. Defaults to 1.0.\n\n    Returns:\n        GenerationOutputs: The generation outputs.\n    \"\"\"\n    outputs = super().generate(\n        input_ids,\n        num_beams=num_beams,\n        decoder_start_token_id=decoder_start_token_id,\n        decoder_end_token_id=decoder_end_token_id,\n        num_return_sequences=num_return_sequences,\n        min_gen_seq_length=min_gen_seq_length,\n        max_gen_seq_length=max_gen_seq_length,\n        repetition_penalty=repetition_penalty,\n        no_repeat_ngram_size=no_repeat_ngram_size,\n        early_stopping=early_stopping,\n        length_penalty=length_penalty,\n        num_beam_groups=num_beam_groups,\n        diversity_penalty=diversity_penalty,\n        do_sample=do_sample,\n        temperature=temperature,\n        top_k=top_k,\n        top_p=top_p,\n    )\n\n    return GenerationOutputs(\n        sequences=outputs.sequences,\n        sequences_scores=outputs.sequences_scores,\n    )\n</code></pre>",
+            "text": "<pre><code>generate(\n    input_ids: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 1,\n    decoder_end_token_id: Optional[\n        Union[int, List[int]]\n    ] = 2,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n)\n</code></pre> <p>Generate sequences using the Llama model.</p> <p>Parameters:</p> Name Type Description Default <code>input_ids</code> <code>torch.Tensor</code> <p>Input token IDs.</p> required <code>num_beams</code> <code>int</code> <p>Number of beams for beam search. Defaults to 5.</p> <code>5</code> <code>decoder_start_token_id</code> <code>int</code> <p>Decoder start token ID. Defaults to 0.</p> <code>1</code> <code>decoder_end_token_id</code> <code>int or List[int]</code> <p>The ID(s) of the decoder end token(s). Defaults to 1.</p> <code>2</code> <code>num_return_sequences</code> <code>int</code> <p>Number of generated sequences to return. Defaults to 1.</p> <code>1</code> <code>min_gen_seq_length</code> <code>int</code> <p>Minimum generation sequence length. Defaults to 0.</p> <code>0</code> <code>max_gen_seq_length</code> <code>int</code> <p>Maximum generation sequence length. Defaults to 48.</p> <code>48</code> <code>repetition_penalty</code> <code>float</code> <p>Repetition penalty. Defaults to 1.0.</p> <code>1.0</code> <code>no_repeat_ngram_size</code> <code>int</code> <p>Size of n-grams to prevent repetition. Defaults to 0.</p> <code>0</code> <code>early_stopping</code> <code>bool</code> <p>Whether to perform early stopping. Defaults to True.</p> <code>True</code> <code>length_penalty</code> <code>float</code> <p>Length penalty. Defaults to 1.0.</p> <code>1.0</code> <code>num_beam_groups</code> <code>int</code> <p>Number of beam groups for diverse beam search. Defaults to 1.</p> <code>1</code> <code>diversity_penalty</code> <code>float</code> <p>Diversity penalty for diverse beam search. Defaults to 0.0.</p> <code>0.0</code> <code>do_sample</code> <code>bool</code> <p>Whether to use sampling for generation. Defaults to False.</p> <code>False</code> <code>temperature</code> <code>float</code> <p>Sampling temperature. Defaults to 1.0.</p> <code>1.0</code> <code>top_k</code> <code>int</code> <p>Top-k sampling parameter. Defaults to 50.</p> <code>50</code> <code>top_p</code> <code>float</code> <p>Top-p sampling parameter. Defaults to 1.0.</p> <code>1.0</code> <p>Returns:</p> Name Type Description <code>GenerationOutputs</code> <p>The generation outputs.</p> Source code in <code>src/unitorch/cli/models/peft/modeling_llama.py</code> <pre><code>@add_default_section_for_function(\"core/model/generation/peft/adalora/llama\")\n@torch.no_grad()\n@autocast()\ndef generate(\n    self,\n    input_ids: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 1,\n    decoder_end_token_id: Optional[Union[int, List[int]]] = 2,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n):\n\"\"\"\n    Generate sequences using the Llama model.\n\n    Args:\n        input_ids (torch.Tensor): Input token IDs.\n        num_beams (int, optional): Number of beams for beam search. Defaults to 5.\n        decoder_start_token_id (int, optional): Decoder start token ID. Defaults to 0.\n        decoder_end_token_id (int or List[int], optional): The ID(s) of the decoder end token(s). Defaults to 1.\n        num_return_sequences (int, optional): Number of generated sequences to return. Defaults to 1.\n        min_gen_seq_length (int, optional): Minimum generation sequence length. Defaults to 0.\n        max_gen_seq_length (int, optional): Maximum generation sequence length. Defaults to 48.\n        repetition_penalty (float, optional): Repetition penalty. Defaults to 1.0.\n        no_repeat_ngram_size (int, optional): Size of n-grams to prevent repetition. Defaults to 0.\n        early_stopping (bool, optional): Whether to perform early stopping. Defaults to True.\n        length_penalty (float, optional): Length penalty. Defaults to 1.0.\n        num_beam_groups (int, optional): Number of beam groups for diverse beam search. Defaults to 1.\n        diversity_penalty (float, optional): Diversity penalty for diverse beam search. Defaults to 0.0.\n        do_sample (bool, optional): Whether to use sampling for generation. Defaults to False.\n        temperature (float, optional): Sampling temperature. Defaults to 1.0.\n        top_k (int, optional): Top-k sampling parameter. Defaults to 50.\n        top_p (float, optional): Top-p sampling parameter. Defaults to 1.0.\n\n    Returns:\n        GenerationOutputs: The generation outputs.\n    \"\"\"\n    outputs = super().generate(\n        input_ids,\n        num_beams=num_beams,\n        decoder_start_token_id=decoder_start_token_id,\n        decoder_end_token_id=decoder_end_token_id,\n        num_return_sequences=num_return_sequences,\n        min_gen_seq_length=min_gen_seq_length,\n        max_gen_seq_length=max_gen_seq_length,\n        repetition_penalty=repetition_penalty,\n        no_repeat_ngram_size=no_repeat_ngram_size,\n        early_stopping=early_stopping,\n        length_penalty=length_penalty,\n        num_beam_groups=num_beam_groups,\n        diversity_penalty=diversity_penalty,\n        do_sample=do_sample,\n        temperature=temperature,\n        top_k=top_k,\n        top_p=top_p,\n    )\n\n    return GenerationOutputs(\n        sequences=outputs.sequences,\n        sequences_scores=outputs.sequences_scores,\n    )\n</code></pre>",
             "title": "generate"
         },
         {
             "location": "cli/models/peft/#llamaloraforclassification",
             "text": "<p>Tip</p> <p><code>core/model/classification/peft/lora/llama</code> is the section for configuration of LlamaLoraForClassification.</p> <p>         Bases: <code>_LlamaLoraForClassification</code></p> <p>LlamaLora model for classification tasks.</p> <p>Initialize the LlamaLoraForClassification model.</p> <p>Parameters:</p> Name Type Description Default <code>config_path</code> <code>str</code> <p>The path to the model configuration file.</p> required <code>lora_r</code> <code>int</code> <p>The number of Lora ranks. Defaults to 16.</p> <code>16</code> <code>lora_alpha</code> <code>int</code> <p>The Lora alpha value. Defaults to 32.</p> <code>32</code> <code>lora_dropout</code> <code>float</code> <p>The Lora dropout rate. Defaults to 0.05.</p> <code>0.05</code> <code>fan_in_fan_out</code> <code>bool</code> <p>Whether to use fan-in/fan-out weight initialization. Defaults to True.</p> <code>True</code> <code>target_modules</code> <code>Union[List[str], str]</code> <p>The target modules for Lora regularization. Defaults to [\"q_proj\", \"v_proj\"].</p> <code>['q_proj', 'v_proj']</code> <code>num_classes</code> <code>int</code> <p>The number of classes. Defaults to 1.</p> <code>1</code> <code>gradient_checkpointing</code> <code>bool</code> <p>Whether to use gradient checkpointing during training. Defaults to False.</p> <code>False</code> Source code in <code>src/unitorch/cli/models/peft/modeling_llama.py</code> <pre><code>def __init__(\n    self,\n    config_path: str,\n    lora_r: Optional[int] = 16,\n    lora_alpha: Optional[int] = 32,\n    lora_dropout: Optional[float] = 0.05,\n    fan_in_fan_out: Optional[bool] = True,\n    target_modules: Optional[Union[List[str], str]] = [\"q_proj\", \"v_proj\"],\n    num_classes: Optional[int] = 1,\n    gradient_checkpointing: Optional[bool] = False,\n):\n\"\"\"\n    Initialize the LlamaLoraForClassification model.\n\n    Args:\n        config_path (str): The path to the model configuration file.\n        lora_r (int, optional): The number of Lora ranks. Defaults to 16.\n        lora_alpha (int, optional): The Lora alpha value. Defaults to 32.\n        lora_dropout (float, optional): The Lora dropout rate. Defaults to 0.05.\n        fan_in_fan_out (bool, optional): Whether to use fan-in/fan-out weight initialization. Defaults to True.\n        target_modules (Union[List[str], str], optional): The target modules for Lora regularization. Defaults to [\"q_proj\", \"v_proj\"].\n        num_classes (int, optional): The number of classes. Defaults to 1.\n        gradient_checkpointing (bool, optional): Whether to use gradient checkpointing during training. Defaults to False.\n    \"\"\"\n    super().__init__(\n        config_path=config_path,\n        lora_r=lora_r,\n        lora_alpha=lora_alpha,\n        lora_dropout=lora_dropout,\n        fan_in_fan_out=fan_in_fan_out,\n        target_modules=target_modules,\n        num_classes=num_classes,\n        gradient_checkpointing=gradient_checkpointing,\n    )\n</code></pre>",
             "title": "LlamaLoraForClassification"
         },
@@ -1037,15 +1072,15 @@
         {
             "location": "cli/models/peft/#unitorch.cli.models.peft.modeling_llama.LlamaLoraForGeneration.from_core_configure",
             "text": "<pre><code>from_core_configure(config, **kwargs)\n</code></pre> <p>Create an instance of LlamaLoraForGeneration from a core configuration.</p> <p>Parameters:</p> Name Type Description Default <code>config</code> <p>The core configuration.</p> required <code>**kwargs</code> <p>Additional keyword arguments.</p> <code>{}</code> <p>Returns:</p> Name Type Description <code>LlamaLoraForGeneration</code> <p>The initialized LlamaLoraForGeneration instance.</p> Source code in <code>src/unitorch/cli/models/peft/modeling_llama.py</code> <pre><code>@classmethod\n@add_default_section_for_init(\"core/model/generation/peft/lora/llama\")\ndef from_core_configure(cls, config, **kwargs):\n\"\"\"\n    Create an instance of LlamaLoraForGeneration from a core configuration.\n\n    Args:\n        config: The core configuration.\n        **kwargs: Additional keyword arguments.\n\n    Returns:\n        LlamaLoraForGeneration: The initialized LlamaLoraForGeneration instance.\n    \"\"\"\n    config.set_default_section(\"core/model/generation/peft/lora/llama\")\n    pretrained_name = config.getoption(\"pretrained_name\", \"default-llama\")\n    config_path = config.getoption(\"config_path\", None)\n    config_path = pop_value(\n        config_path,\n        nested_dict_value(pretrained_llama_infos, pretrained_name, \"config\"),\n    )\n    config_path = cached_path(config_path)\n\n    lora_r = config.getoption(\"lora_r\", 16)\n    lora_alpha = config.getoption(\"lora_alpha\", 32)\n    lora_dropout = config.getoption(\"lora_dropout\", 0.05)\n    fan_in_fan_out = config.getoption(\"fan_in_fan_out\", True)\n    target_modules = config.getoption(\"target_modules\", [\"q_proj\", \"v_proj\"])\n\n    gradient_checkpointing = config.getoption(\"gradient_checkpointing\", False)\n\n    inst = cls(\n        config_path,\n        lora_r=lora_r,\n        lora_alpha=lora_alpha,\n        lora_dropout=lora_dropout,\n        fan_in_fan_out=fan_in_fan_out,\n        target_modules=target_modules,\n        gradient_checkpointing=gradient_checkpointing,\n    )\n\n    weight_path = []\n    pretrained_weight_path = config.getoption(\"pretrained_weight_path\", None)\n    pretrained_weight_path = pop_value(\n        pretrained_weight_path,\n        nested_dict_value(pretrained_llama_infos, pretrained_name, \"weight\"),\n        check_none=False,\n    )\n    if pretrained_weight_path is not None:\n        if isinstance(pretrained_weight_path, str):\n            weight_path.append(pretrained_weight_path)\n        elif isinstance(pretrained_weight_path, list):\n            weight_path.extend(pretrained_weight_path)\n\n    pretrained_lora_weight_path = config.getoption(\n        \"pretrained_lora_weight_path\", None\n    )\n    if pretrained_lora_weight_path is not None:\n        weight_path.append(pretrained_lora_weight_path)\n\n    if len(weight_path) &gt; 0:\n        inst.from_pretrained(\n            weight_path=weight_path,\n        )\n\n    return inst\n</code></pre>",
             "title": "from_core_configure  <code>classmethod</code>"
         },
         {
             "location": "cli/models/peft/#unitorch.cli.models.peft.modeling_llama.LlamaLoraForGeneration.generate",
-            "text": "<pre><code>generate(\n    input_ids: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 1,\n    decoder_end_token_id: Optional[int] = 2,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n)\n</code></pre> <p>Generate sequences using the Llama model.</p> <p>Parameters:</p> Name Type Description Default <code>input_ids</code> <code>torch.Tensor</code> <p>Input token IDs.</p> required <code>num_beams</code> <code>int</code> <p>Number of beams for beam search. Defaults to 5.</p> <code>5</code> <code>decoder_start_token_id</code> <code>int</code> <p>Decoder start token ID. Defaults to 0.</p> <code>1</code> <code>decoder_end_token_id</code> <code>int</code> <p>Decoder end token ID. Defaults to 1.</p> <code>2</code> <code>num_return_sequences</code> <code>int</code> <p>Number of generated sequences to return. Defaults to 1.</p> <code>1</code> <code>min_gen_seq_length</code> <code>int</code> <p>Minimum generation sequence length. Defaults to 0.</p> <code>0</code> <code>max_gen_seq_length</code> <code>int</code> <p>Maximum generation sequence length. Defaults to 48.</p> <code>48</code> <code>repetition_penalty</code> <code>float</code> <p>Repetition penalty. Defaults to 1.0.</p> <code>1.0</code> <code>no_repeat_ngram_size</code> <code>int</code> <p>Size of n-grams to prevent repetition. Defaults to 0.</p> <code>0</code> <code>early_stopping</code> <code>bool</code> <p>Whether to perform early stopping. Defaults to True.</p> <code>True</code> <code>length_penalty</code> <code>float</code> <p>Length penalty. Defaults to 1.0.</p> <code>1.0</code> <code>num_beam_groups</code> <code>int</code> <p>Number of beam groups for diverse beam search. Defaults to 1.</p> <code>1</code> <code>diversity_penalty</code> <code>float</code> <p>Diversity penalty for diverse beam search. Defaults to 0.0.</p> <code>0.0</code> <code>do_sample</code> <code>bool</code> <p>Whether to use sampling for generation. Defaults to False.</p> <code>False</code> <code>temperature</code> <code>float</code> <p>Sampling temperature. Defaults to 1.0.</p> <code>1.0</code> <code>top_k</code> <code>int</code> <p>Top-k sampling parameter. Defaults to 50.</p> <code>50</code> <code>top_p</code> <code>float</code> <p>Top-p sampling parameter. Defaults to 1.0.</p> <code>1.0</code> <p>Returns:</p> Name Type Description <code>GenerationOutputs</code> <p>The generation outputs.</p> Source code in <code>src/unitorch/cli/models/peft/modeling_llama.py</code> <pre><code>@add_default_section_for_function(\"core/model/generation/peft/lora/llama\")\n@torch.no_grad()\n@autocast()\ndef generate(\n    self,\n    input_ids: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 1,\n    decoder_end_token_id: Optional[int] = 2,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n):\n\"\"\"\n    Generate sequences using the Llama model.\n\n    Args:\n        input_ids (torch.Tensor): Input token IDs.\n        num_beams (int, optional): Number of beams for beam search. Defaults to 5.\n        decoder_start_token_id (int, optional): Decoder start token ID. Defaults to 0.\n        decoder_end_token_id (int, optional): Decoder end token ID. Defaults to 1.\n        num_return_sequences (int, optional): Number of generated sequences to return. Defaults to 1.\n        min_gen_seq_length (int, optional): Minimum generation sequence length. Defaults to 0.\n        max_gen_seq_length (int, optional): Maximum generation sequence length. Defaults to 48.\n        repetition_penalty (float, optional): Repetition penalty. Defaults to 1.0.\n        no_repeat_ngram_size (int, optional): Size of n-grams to prevent repetition. Defaults to 0.\n        early_stopping (bool, optional): Whether to perform early stopping. Defaults to True.\n        length_penalty (float, optional): Length penalty. Defaults to 1.0.\n        num_beam_groups (int, optional): Number of beam groups for diverse beam search. Defaults to 1.\n        diversity_penalty (float, optional): Diversity penalty for diverse beam search. Defaults to 0.0.\n        do_sample (bool, optional): Whether to use sampling for generation. Defaults to False.\n        temperature (float, optional): Sampling temperature. Defaults to 1.0.\n        top_k (int, optional): Top-k sampling parameter. Defaults to 50.\n        top_p (float, optional): Top-p sampling parameter. Defaults to 1.0.\n\n    Returns:\n        GenerationOutputs: The generation outputs.\n    \"\"\"\n    outputs = super().generate(\n        input_ids,\n        num_beams=num_beams,\n        decoder_start_token_id=decoder_start_token_id,\n        decoder_end_token_id=decoder_end_token_id,\n        num_return_sequences=num_return_sequences,\n        min_gen_seq_length=min_gen_seq_length,\n        max_gen_seq_length=max_gen_seq_length,\n        repetition_penalty=repetition_penalty,\n        no_repeat_ngram_size=no_repeat_ngram_size,\n        early_stopping=early_stopping,\n        length_penalty=length_penalty,\n        num_beam_groups=num_beam_groups,\n        diversity_penalty=diversity_penalty,\n        do_sample=do_sample,\n        temperature=temperature,\n        top_k=top_k,\n        top_p=top_p,\n    )\n\n    return GenerationOutputs(\n        sequences=outputs.sequences,\n        sequences_scores=outputs.sequences_scores,\n    )\n</code></pre>",
+            "text": "<pre><code>generate(\n    input_ids: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 1,\n    decoder_end_token_id: Optional[\n        Union[int, List[int]]\n    ] = 2,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n)\n</code></pre> <p>Generate sequences using the Llama model.</p> <p>Parameters:</p> Name Type Description Default <code>input_ids</code> <code>torch.Tensor</code> <p>Input token IDs.</p> required <code>num_beams</code> <code>int</code> <p>Number of beams for beam search. Defaults to 5.</p> <code>5</code> <code>decoder_start_token_id</code> <code>int</code> <p>Decoder start token ID. Defaults to 0.</p> <code>1</code> <code>decoder_end_token_id</code> <code>int or List[int]</code> <p>The ID(s) of the decoder end token(s). Defaults to 1.</p> <code>2</code> <code>num_return_sequences</code> <code>int</code> <p>Number of generated sequences to return. Defaults to 1.</p> <code>1</code> <code>min_gen_seq_length</code> <code>int</code> <p>Minimum generation sequence length. Defaults to 0.</p> <code>0</code> <code>max_gen_seq_length</code> <code>int</code> <p>Maximum generation sequence length. Defaults to 48.</p> <code>48</code> <code>repetition_penalty</code> <code>float</code> <p>Repetition penalty. Defaults to 1.0.</p> <code>1.0</code> <code>no_repeat_ngram_size</code> <code>int</code> <p>Size of n-grams to prevent repetition. Defaults to 0.</p> <code>0</code> <code>early_stopping</code> <code>bool</code> <p>Whether to perform early stopping. Defaults to True.</p> <code>True</code> <code>length_penalty</code> <code>float</code> <p>Length penalty. Defaults to 1.0.</p> <code>1.0</code> <code>num_beam_groups</code> <code>int</code> <p>Number of beam groups for diverse beam search. Defaults to 1.</p> <code>1</code> <code>diversity_penalty</code> <code>float</code> <p>Diversity penalty for diverse beam search. Defaults to 0.0.</p> <code>0.0</code> <code>do_sample</code> <code>bool</code> <p>Whether to use sampling for generation. Defaults to False.</p> <code>False</code> <code>temperature</code> <code>float</code> <p>Sampling temperature. Defaults to 1.0.</p> <code>1.0</code> <code>top_k</code> <code>int</code> <p>Top-k sampling parameter. Defaults to 50.</p> <code>50</code> <code>top_p</code> <code>float</code> <p>Top-p sampling parameter. Defaults to 1.0.</p> <code>1.0</code> <p>Returns:</p> Name Type Description <code>GenerationOutputs</code> <p>The generation outputs.</p> Source code in <code>src/unitorch/cli/models/peft/modeling_llama.py</code> <pre><code>@add_default_section_for_function(\"core/model/generation/peft/lora/llama\")\n@torch.no_grad()\n@autocast()\ndef generate(\n    self,\n    input_ids: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 1,\n    decoder_end_token_id: Optional[Union[int, List[int]]] = 2,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n):\n\"\"\"\n    Generate sequences using the Llama model.\n\n    Args:\n        input_ids (torch.Tensor): Input token IDs.\n        num_beams (int, optional): Number of beams for beam search. Defaults to 5.\n        decoder_start_token_id (int, optional): Decoder start token ID. Defaults to 0.\n        decoder_end_token_id (int or List[int], optional): The ID(s) of the decoder end token(s). Defaults to 1.\n        num_return_sequences (int, optional): Number of generated sequences to return. Defaults to 1.\n        min_gen_seq_length (int, optional): Minimum generation sequence length. Defaults to 0.\n        max_gen_seq_length (int, optional): Maximum generation sequence length. Defaults to 48.\n        repetition_penalty (float, optional): Repetition penalty. Defaults to 1.0.\n        no_repeat_ngram_size (int, optional): Size of n-grams to prevent repetition. Defaults to 0.\n        early_stopping (bool, optional): Whether to perform early stopping. Defaults to True.\n        length_penalty (float, optional): Length penalty. Defaults to 1.0.\n        num_beam_groups (int, optional): Number of beam groups for diverse beam search. Defaults to 1.\n        diversity_penalty (float, optional): Diversity penalty for diverse beam search. Defaults to 0.0.\n        do_sample (bool, optional): Whether to use sampling for generation. Defaults to False.\n        temperature (float, optional): Sampling temperature. Defaults to 1.0.\n        top_k (int, optional): Top-k sampling parameter. Defaults to 50.\n        top_p (float, optional): Top-p sampling parameter. Defaults to 1.0.\n\n    Returns:\n        GenerationOutputs: The generation outputs.\n    \"\"\"\n    outputs = super().generate(\n        input_ids,\n        num_beams=num_beams,\n        decoder_start_token_id=decoder_start_token_id,\n        decoder_end_token_id=decoder_end_token_id,\n        num_return_sequences=num_return_sequences,\n        min_gen_seq_length=min_gen_seq_length,\n        max_gen_seq_length=max_gen_seq_length,\n        repetition_penalty=repetition_penalty,\n        no_repeat_ngram_size=no_repeat_ngram_size,\n        early_stopping=early_stopping,\n        length_penalty=length_penalty,\n        num_beam_groups=num_beam_groups,\n        diversity_penalty=diversity_penalty,\n        do_sample=do_sample,\n        temperature=temperature,\n        top_k=top_k,\n        top_p=top_p,\n    )\n\n    return GenerationOutputs(\n        sequences=outputs.sequences,\n        sequences_scores=outputs.sequences_scores,\n    )\n</code></pre>",
             "title": "generate"
         },
         {
             "location": "cli/models/pegasus/",
             "text": "",
             "title": "unitorch.cli.models.pegasus"
         },
@@ -1072,15 +1107,15 @@
         {
             "location": "cli/models/pegasus/#unitorch.cli.models.pegasus.modeling.PegasusForGeneration.from_core_configure",
             "text": "<pre><code>from_core_configure(config, **kwargs)\n</code></pre> <p>Create an instance of PegasusForGeneration from a core configuration.</p> <p>Parameters:</p> Name Type Description Default <code>config</code> <p>The core configuration.</p> required <code>**kwargs</code> <p>Additional keyword arguments.</p> <code>{}</code> <p>Returns:</p> Name Type Description <code>PegasusForGeneration</code> <p>The initialized PegasusForGeneration instance.</p> Source code in <code>src/unitorch/cli/models/pegasus/modeling.py</code> <pre><code>@classmethod\n@add_default_section_for_init(\"core/model/generation/pegasus\")\ndef from_core_configure(cls, config, **kwargs):\n\"\"\"\n    Create an instance of PegasusForGeneration from a core configuration.\n\n    Args:\n        config: The core configuration.\n        **kwargs: Additional keyword arguments.\n\n    Returns:\n        PegasusForGeneration: The initialized PegasusForGeneration instance.\n    \"\"\"\n    config.set_default_section(\"core/model/generation/pegasus\")\n    pretrained_name = config.getoption(\"pretrained_name\", \"default-pegasus\")\n    config_path = config.getoption(\"config_path\", None)\n    config_path = pop_value(\n        config_path,\n        nested_dict_value(pretrained_pegasus_infos, pretrained_name, \"config\"),\n    )\n\n    config_path = cached_path(config_path)\n    gradient_checkpointing = config.getoption(\"gradient_checkpointing\", False)\n\n    inst = cls(config_path, gradient_checkpointing)\n    pretrained_weight_path = config.getoption(\"pretrained_weight_path\", None)\n    weight_path = pop_value(\n        pretrained_weight_path,\n        nested_dict_value(pretrained_pegasus_infos, pretrained_name, \"weight\"),\n        check_none=False,\n    )\n\n    if weight_path is not None:\n        weight_path = cached_path(weight_path)\n        inst.from_pretrained(weight_path)\n\n    return inst\n</code></pre>",
             "title": "from_core_configure  <code>classmethod</code>"
         },
         {
             "location": "cli/models/pegasus/#unitorch.cli.models.pegasus.modeling.PegasusForGeneration.generate",
-            "text": "<pre><code>generate(\n    input_ids: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 0,\n    decoder_end_token_id: Optional[int] = 1,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n)\n</code></pre> <p>Generate sequences using the Pegasus model.</p> <p>Parameters:</p> Name Type Description Default <code>input_ids</code> <code>torch.Tensor</code> <p>Input token IDs.</p> required <code>num_beams</code> <code>int</code> <p>Number of beams for beam search. Defaults to 5.</p> <code>5</code> <code>decoder_start_token_id</code> <code>int</code> <p>Decoder start token ID. Defaults to 0.</p> <code>0</code> <code>decoder_end_token_id</code> <code>int</code> <p>Decoder end token ID. Defaults to 1.</p> <code>1</code> <code>num_return_sequences</code> <code>int</code> <p>Number of generated sequences to return. Defaults to 1.</p> <code>1</code> <code>min_gen_seq_length</code> <code>int</code> <p>Minimum generation sequence length. Defaults to 0.</p> <code>0</code> <code>max_gen_seq_length</code> <code>int</code> <p>Maximum generation sequence length. Defaults to 48.</p> <code>48</code> <code>repetition_penalty</code> <code>float</code> <p>Repetition penalty. Defaults to 1.0.</p> <code>1.0</code> <code>no_repeat_ngram_size</code> <code>int</code> <p>Size of n-grams to prevent repetition. Defaults to 0.</p> <code>0</code> <code>early_stopping</code> <code>bool</code> <p>Whether to perform early stopping. Defaults to True.</p> <code>True</code> <code>length_penalty</code> <code>float</code> <p>Length penalty. Defaults to 1.0.</p> <code>1.0</code> <code>num_beam_groups</code> <code>int</code> <p>Number of beam groups for diverse beam search. Defaults to 1.</p> <code>1</code> <code>diversity_penalty</code> <code>float</code> <p>Diversity penalty for diverse beam search. Defaults to 0.0.</p> <code>0.0</code> <code>do_sample</code> <code>bool</code> <p>Whether to use sampling for generation. Defaults to False.</p> <code>False</code> <code>temperature</code> <code>float</code> <p>Sampling temperature. Defaults to 1.0.</p> <code>1.0</code> <code>top_k</code> <code>int</code> <p>Top-k sampling parameter. Defaults to 50.</p> <code>50</code> <code>top_p</code> <code>float</code> <p>Top-p sampling parameter. Defaults to 1.0.</p> <code>1.0</code> <p>Returns:</p> Name Type Description <code>GenerationOutputs</code> <p>The generation outputs.</p> Source code in <code>src/unitorch/cli/models/pegasus/modeling.py</code> <pre><code>@add_default_section_for_function(\"core/model/generation/pegasus\")\n@torch.no_grad()\n@autocast()\ndef generate(\n    self,\n    input_ids: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 0,\n    decoder_end_token_id: Optional[int] = 1,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n):\n\"\"\"\n    Generate sequences using the Pegasus model.\n\n    Args:\n        input_ids (torch.Tensor): Input token IDs.\n        num_beams (int, optional): Number of beams for beam search. Defaults to 5.\n        decoder_start_token_id (int, optional): Decoder start token ID. Defaults to 0.\n        decoder_end_token_id (int, optional): Decoder end token ID. Defaults to 1.\n        num_return_sequences (int, optional): Number of generated sequences to return. Defaults to 1.\n        min_gen_seq_length (int, optional): Minimum generation sequence length. Defaults to 0.\n        max_gen_seq_length (int, optional): Maximum generation sequence length. Defaults to 48.\n        repetition_penalty (float, optional): Repetition penalty. Defaults to 1.0.\n        no_repeat_ngram_size (int, optional): Size of n-grams to prevent repetition. Defaults to 0.\n        early_stopping (bool, optional): Whether to perform early stopping. Defaults to True.\n        length_penalty (float, optional): Length penalty. Defaults to 1.0.\n        num_beam_groups (int, optional): Number of beam groups for diverse beam search. Defaults to 1.\n        diversity_penalty (float, optional): Diversity penalty for diverse beam search. Defaults to 0.0.\n        do_sample (bool, optional): Whether to use sampling for generation. Defaults to False.\n        temperature (float, optional): Sampling temperature. Defaults to 1.0.\n        top_k (int, optional): Top-k sampling parameter. Defaults to 50.\n        top_p (float, optional): Top-p sampling parameter. Defaults to 1.0.\n\n    Returns:\n        GenerationOutputs: The generation outputs.\n    \"\"\"\n\n    outputs = super().generate(\n        input_ids,\n        num_beams=num_beams,\n        decoder_start_token_id=decoder_start_token_id,\n        decoder_end_token_id=decoder_end_token_id,\n        num_return_sequences=num_return_sequences,\n        min_gen_seq_length=min_gen_seq_length,\n        max_gen_seq_length=max_gen_seq_length,\n        repetition_penalty=repetition_penalty,\n        no_repeat_ngram_size=no_repeat_ngram_size,\n        early_stopping=early_stopping,\n        length_penalty=length_penalty,\n        num_beam_groups=num_beam_groups,\n        diversity_penalty=diversity_penalty,\n        do_sample=do_sample,\n        temperature=temperature,\n        top_k=top_k,\n        top_p=top_p,\n    )\n\n    return GenerationOutputs(\n        sequences=outputs.sequences,\n        sequences_scores=outputs.sequences_scores,\n    )\n</code></pre>",
+            "text": "<pre><code>generate(\n    input_ids: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 0,\n    decoder_end_token_id: Optional[\n        Union[int, List[int]]\n    ] = 1,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n)\n</code></pre> <p>Generate sequences using the Pegasus model.</p> <p>Parameters:</p> Name Type Description Default <code>input_ids</code> <code>torch.Tensor</code> <p>Input token IDs.</p> required <code>num_beams</code> <code>int</code> <p>Number of beams for beam search. Defaults to 5.</p> <code>5</code> <code>decoder_start_token_id</code> <code>int</code> <p>Decoder start token ID. Defaults to 0.</p> <code>0</code> <code>decoder_end_token_id</code> <code>int or List[int]</code> <p>The ID(s) of the decoder end token(s). Defaults to 1.</p> <code>1</code> <code>num_return_sequences</code> <code>int</code> <p>Number of generated sequences to return. Defaults to 1.</p> <code>1</code> <code>min_gen_seq_length</code> <code>int</code> <p>Minimum generation sequence length. Defaults to 0.</p> <code>0</code> <code>max_gen_seq_length</code> <code>int</code> <p>Maximum generation sequence length. Defaults to 48.</p> <code>48</code> <code>repetition_penalty</code> <code>float</code> <p>Repetition penalty. Defaults to 1.0.</p> <code>1.0</code> <code>no_repeat_ngram_size</code> <code>int</code> <p>Size of n-grams to prevent repetition. Defaults to 0.</p> <code>0</code> <code>early_stopping</code> <code>bool</code> <p>Whether to perform early stopping. Defaults to True.</p> <code>True</code> <code>length_penalty</code> <code>float</code> <p>Length penalty. Defaults to 1.0.</p> <code>1.0</code> <code>num_beam_groups</code> <code>int</code> <p>Number of beam groups for diverse beam search. Defaults to 1.</p> <code>1</code> <code>diversity_penalty</code> <code>float</code> <p>Diversity penalty for diverse beam search. Defaults to 0.0.</p> <code>0.0</code> <code>do_sample</code> <code>bool</code> <p>Whether to use sampling for generation. Defaults to False.</p> <code>False</code> <code>temperature</code> <code>float</code> <p>Sampling temperature. Defaults to 1.0.</p> <code>1.0</code> <code>top_k</code> <code>int</code> <p>Top-k sampling parameter. Defaults to 50.</p> <code>50</code> <code>top_p</code> <code>float</code> <p>Top-p sampling parameter. Defaults to 1.0.</p> <code>1.0</code> <p>Returns:</p> Name Type Description <code>GenerationOutputs</code> <p>The generation outputs.</p> Source code in <code>src/unitorch/cli/models/pegasus/modeling.py</code> <pre><code>@add_default_section_for_function(\"core/model/generation/pegasus\")\n@torch.no_grad()\n@autocast()\ndef generate(\n    self,\n    input_ids: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 0,\n    decoder_end_token_id: Optional[Union[int, List[int]]] = 1,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n):\n\"\"\"\n    Generate sequences using the Pegasus model.\n\n    Args:\n        input_ids (torch.Tensor): Input token IDs.\n        num_beams (int, optional): Number of beams for beam search. Defaults to 5.\n        decoder_start_token_id (int, optional): Decoder start token ID. Defaults to 0.\n        decoder_end_token_id (int or List[int], optional): The ID(s) of the decoder end token(s). Defaults to 1.\n        num_return_sequences (int, optional): Number of generated sequences to return. Defaults to 1.\n        min_gen_seq_length (int, optional): Minimum generation sequence length. Defaults to 0.\n        max_gen_seq_length (int, optional): Maximum generation sequence length. Defaults to 48.\n        repetition_penalty (float, optional): Repetition penalty. Defaults to 1.0.\n        no_repeat_ngram_size (int, optional): Size of n-grams to prevent repetition. Defaults to 0.\n        early_stopping (bool, optional): Whether to perform early stopping. Defaults to True.\n        length_penalty (float, optional): Length penalty. Defaults to 1.0.\n        num_beam_groups (int, optional): Number of beam groups for diverse beam search. Defaults to 1.\n        diversity_penalty (float, optional): Diversity penalty for diverse beam search. Defaults to 0.0.\n        do_sample (bool, optional): Whether to use sampling for generation. Defaults to False.\n        temperature (float, optional): Sampling temperature. Defaults to 1.0.\n        top_k (int, optional): Top-k sampling parameter. Defaults to 50.\n        top_p (float, optional): Top-p sampling parameter. Defaults to 1.0.\n\n    Returns:\n        GenerationOutputs: The generation outputs.\n    \"\"\"\n\n    outputs = super().generate(\n        input_ids,\n        num_beams=num_beams,\n        decoder_start_token_id=decoder_start_token_id,\n        decoder_end_token_id=decoder_end_token_id,\n        num_return_sequences=num_return_sequences,\n        min_gen_seq_length=min_gen_seq_length,\n        max_gen_seq_length=max_gen_seq_length,\n        repetition_penalty=repetition_penalty,\n        no_repeat_ngram_size=no_repeat_ngram_size,\n        early_stopping=early_stopping,\n        length_penalty=length_penalty,\n        num_beam_groups=num_beam_groups,\n        diversity_penalty=diversity_penalty,\n        do_sample=do_sample,\n        temperature=temperature,\n        top_k=top_k,\n        top_p=top_p,\n    )\n\n    return GenerationOutputs(\n        sequences=outputs.sequences,\n        sequences_scores=outputs.sequences_scores,\n    )\n</code></pre>",
             "title": "generate"
         },
         {
             "location": "cli/models/prophetnet/",
             "text": "",
             "title": "unitorch.cli.models.prophetnet"
         },
@@ -1172,15 +1207,15 @@
         {
             "location": "cli/models/t5/#unitorch.cli.models.t5.modeling.T5ForGeneration.from_core_configure",
             "text": "<pre><code>from_core_configure(config, **kwargs)\n</code></pre> <p>Create an instance of T5ForGeneration from a core configuration.</p> <p>Parameters:</p> Name Type Description Default <code>config</code> <p>The core configuration.</p> required <code>**kwargs</code> <p>Additional keyword arguments.</p> <code>{}</code> <p>Returns:</p> Name Type Description <code>T5ForGeneration</code> <p>An instance of the T5ForGeneration model.</p> Source code in <code>src/unitorch/cli/models/t5/modeling.py</code> <pre><code>@classmethod\n@add_default_section_for_init(\"core/model/generation/t5\")\ndef from_core_configure(cls, config, **kwargs):\n\"\"\"\n    Create an instance of T5ForGeneration from a core configuration.\n\n    Args:\n        config: The core configuration.\n        **kwargs: Additional keyword arguments.\n\n    Returns:\n        T5ForGeneration: An instance of the T5ForGeneration model.\n    \"\"\"\n    config.set_default_section(\"core/model/generation/t5\")\n    pretrained_name = config.getoption(\"pretrained_name\", \"default-t5\")\n    config_path = config.getoption(\"config_path\", None)\n    config_path = pop_value(\n        config_path,\n        nested_dict_value(pretrained_t5_infos, pretrained_name, \"config\"),\n    )\n\n    config_path = cached_path(config_path)\n    gradient_checkpointing = config.getoption(\"gradient_checkpointing\", False)\n\n    inst = cls(config_path, gradient_checkpointing)\n    pretrained_weight_path = config.getoption(\"pretrained_weight_path\", None)\n    weight_path = pop_value(\n        pretrained_weight_path,\n        nested_dict_value(pretrained_t5_infos, pretrained_name, \"weight\"),\n        check_none=False,\n    )\n    if weight_path is not None:\n        weight_path = cached_path(weight_path)\n        inst.from_pretrained(weight_path)\n\n    return inst\n</code></pre>",
             "title": "from_core_configure  <code>classmethod</code>"
         },
         {
             "location": "cli/models/t5/#unitorch.cli.models.t5.modeling.T5ForGeneration.generate",
-            "text": "<pre><code>generate(\n    input_ids: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 0,\n    decoder_end_token_id: Optional[int] = 1,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n)\n</code></pre> <p>Generate sequences using the T5 model.</p> <p>Parameters:</p> Name Type Description Default <code>input_ids</code> <code>torch.Tensor</code> <p>Input token IDs.</p> required <code>num_beams</code> <code>int</code> <p>Number of beams for beam search. Defaults to 5.</p> <code>5</code> <code>decoder_start_token_id</code> <code>int</code> <p>Decoder start token ID. Defaults to 0.</p> <code>0</code> <code>decoder_end_token_id</code> <code>int</code> <p>Decoder end token ID. Defaults to 1.</p> <code>1</code> <code>num_return_sequences</code> <code>int</code> <p>Number of generated sequences to return. Defaults to 1.</p> <code>1</code> <code>min_gen_seq_length</code> <code>int</code> <p>Minimum generation sequence length. Defaults to 0.</p> <code>0</code> <code>max_gen_seq_length</code> <code>int</code> <p>Maximum generation sequence length. Defaults to 48.</p> <code>48</code> <code>repetition_penalty</code> <code>float</code> <p>Repetition penalty. Defaults to 1.0.</p> <code>1.0</code> <code>no_repeat_ngram_size</code> <code>int</code> <p>Size of n-grams to prevent repetition. Defaults to 0.</p> <code>0</code> <code>early_stopping</code> <code>bool</code> <p>Whether to perform early stopping. Defaults to True.</p> <code>True</code> <code>length_penalty</code> <code>float</code> <p>Length penalty. Defaults to 1.0.</p> <code>1.0</code> <code>num_beam_groups</code> <code>int</code> <p>Number of beam groups for diverse beam search. Defaults to 1.</p> <code>1</code> <code>diversity_penalty</code> <code>float</code> <p>Diversity penalty for diverse beam search. Defaults to 0.0.</p> <code>0.0</code> <code>do_sample</code> <code>bool</code> <p>Whether to use sampling for generation. Defaults to False.</p> <code>False</code> <code>temperature</code> <code>float</code> <p>Sampling temperature. Defaults to 1.0.</p> <code>1.0</code> <code>top_k</code> <code>int</code> <p>Top-k sampling parameter. Defaults to 50.</p> <code>50</code> <code>top_p</code> <code>float</code> <p>Top-p sampling parameter. Defaults to 1.0.</p> <code>1.0</code> <p>Returns:</p> Name Type Description <code>GenerationOutputs</code> <p>The generation outputs.</p> Source code in <code>src/unitorch/cli/models/t5/modeling.py</code> <pre><code>@add_default_section_for_function(\"core/model/generation/t5\")\n@torch.no_grad()\n@autocast()\ndef generate(\n    self,\n    input_ids: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 0,\n    decoder_end_token_id: Optional[int] = 1,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n):\n\"\"\"\n    Generate sequences using the T5 model.\n\n    Args:\n        input_ids (torch.Tensor): Input token IDs.\n        num_beams (int, optional): Number of beams for beam search. Defaults to 5.\n        decoder_start_token_id (int, optional): Decoder start token ID. Defaults to 0.\n        decoder_end_token_id (int, optional): Decoder end token ID. Defaults to 1.\n        num_return_sequences (int, optional): Number of generated sequences to return. Defaults to 1.\n        min_gen_seq_length (int, optional): Minimum generation sequence length. Defaults to 0.\n        max_gen_seq_length (int, optional): Maximum generation sequence length. Defaults to 48.\n        repetition_penalty (float, optional): Repetition penalty. Defaults to 1.0.\n        no_repeat_ngram_size (int, optional): Size of n-grams to prevent repetition. Defaults to 0.\n        early_stopping (bool, optional): Whether to perform early stopping. Defaults to True.\n        length_penalty (float, optional): Length penalty. Defaults to 1.0.\n        num_beam_groups (int, optional): Number of beam groups for diverse beam search. Defaults to 1.\n        diversity_penalty (float, optional): Diversity penalty for diverse beam search. Defaults to 0.0.\n        do_sample (bool, optional): Whether to use sampling for generation. Defaults to False.\n        temperature (float, optional): Sampling temperature. Defaults to 1.0.\n        top_k (int, optional): Top-k sampling parameter. Defaults to 50.\n        top_p (float, optional): Top-p sampling parameter. Defaults to 1.0.\n\n    Returns:\n        GenerationOutputs: The generation outputs.\n    \"\"\"\n\n    outputs = super().generate(\n        input_ids,\n        num_beams=num_beams,\n        decoder_start_token_id=decoder_start_token_id,\n        decoder_end_token_id=decoder_end_token_id,\n        num_return_sequences=num_return_sequences,\n        min_gen_seq_length=min_gen_seq_length,\n        max_gen_seq_length=max_gen_seq_length,\n        repetition_penalty=repetition_penalty,\n        no_repeat_ngram_size=no_repeat_ngram_size,\n        early_stopping=early_stopping,\n        length_penalty=length_penalty,\n        num_beam_groups=num_beam_groups,\n        diversity_penalty=diversity_penalty,\n        do_sample=do_sample,\n        temperature=temperature,\n        top_k=top_k,\n        top_p=top_p,\n    )\n\n    return GenerationOutputs(\n        sequences=outputs.sequences,\n        sequences_scores=outputs.sequences_scores,\n    )\n</code></pre>",
+            "text": "<pre><code>generate(\n    input_ids: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 0,\n    decoder_end_token_id: Optional[\n        Union[int, List[int]]\n    ] = 1,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n)\n</code></pre> <p>Generate sequences using the T5 model.</p> <p>Parameters:</p> Name Type Description Default <code>input_ids</code> <code>torch.Tensor</code> <p>Input token IDs.</p> required <code>num_beams</code> <code>int</code> <p>Number of beams for beam search. Defaults to 5.</p> <code>5</code> <code>decoder_start_token_id</code> <code>int</code> <p>Decoder start token ID. Defaults to 0.</p> <code>0</code> <code>decoder_end_token_id</code> <code>int or List[int]</code> <p>The ID(s) of the decoder end token(s). Defaults to 1.</p> <code>1</code> <code>num_return_sequences</code> <code>int</code> <p>Number of generated sequences to return. Defaults to 1.</p> <code>1</code> <code>min_gen_seq_length</code> <code>int</code> <p>Minimum generation sequence length. Defaults to 0.</p> <code>0</code> <code>max_gen_seq_length</code> <code>int</code> <p>Maximum generation sequence length. Defaults to 48.</p> <code>48</code> <code>repetition_penalty</code> <code>float</code> <p>Repetition penalty. Defaults to 1.0.</p> <code>1.0</code> <code>no_repeat_ngram_size</code> <code>int</code> <p>Size of n-grams to prevent repetition. Defaults to 0.</p> <code>0</code> <code>early_stopping</code> <code>bool</code> <p>Whether to perform early stopping. Defaults to True.</p> <code>True</code> <code>length_penalty</code> <code>float</code> <p>Length penalty. Defaults to 1.0.</p> <code>1.0</code> <code>num_beam_groups</code> <code>int</code> <p>Number of beam groups for diverse beam search. Defaults to 1.</p> <code>1</code> <code>diversity_penalty</code> <code>float</code> <p>Diversity penalty for diverse beam search. Defaults to 0.0.</p> <code>0.0</code> <code>do_sample</code> <code>bool</code> <p>Whether to use sampling for generation. Defaults to False.</p> <code>False</code> <code>temperature</code> <code>float</code> <p>Sampling temperature. Defaults to 1.0.</p> <code>1.0</code> <code>top_k</code> <code>int</code> <p>Top-k sampling parameter. Defaults to 50.</p> <code>50</code> <code>top_p</code> <code>float</code> <p>Top-p sampling parameter. Defaults to 1.0.</p> <code>1.0</code> <p>Returns:</p> Name Type Description <code>GenerationOutputs</code> <p>The generation outputs.</p> Source code in <code>src/unitorch/cli/models/t5/modeling.py</code> <pre><code>@add_default_section_for_function(\"core/model/generation/t5\")\n@torch.no_grad()\n@autocast()\ndef generate(\n    self,\n    input_ids: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 0,\n    decoder_end_token_id: Optional[Union[int, List[int]]] = 1,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n):\n\"\"\"\n    Generate sequences using the T5 model.\n\n    Args:\n        input_ids (torch.Tensor): Input token IDs.\n        num_beams (int, optional): Number of beams for beam search. Defaults to 5.\n        decoder_start_token_id (int, optional): Decoder start token ID. Defaults to 0.\n        decoder_end_token_id (int or List[int], optional): The ID(s) of the decoder end token(s). Defaults to 1.\n        num_return_sequences (int, optional): Number of generated sequences to return. Defaults to 1.\n        min_gen_seq_length (int, optional): Minimum generation sequence length. Defaults to 0.\n        max_gen_seq_length (int, optional): Maximum generation sequence length. Defaults to 48.\n        repetition_penalty (float, optional): Repetition penalty. Defaults to 1.0.\n        no_repeat_ngram_size (int, optional): Size of n-grams to prevent repetition. Defaults to 0.\n        early_stopping (bool, optional): Whether to perform early stopping. Defaults to True.\n        length_penalty (float, optional): Length penalty. Defaults to 1.0.\n        num_beam_groups (int, optional): Number of beam groups for diverse beam search. Defaults to 1.\n        diversity_penalty (float, optional): Diversity penalty for diverse beam search. Defaults to 0.0.\n        do_sample (bool, optional): Whether to use sampling for generation. Defaults to False.\n        temperature (float, optional): Sampling temperature. Defaults to 1.0.\n        top_k (int, optional): Top-k sampling parameter. Defaults to 50.\n        top_p (float, optional): Top-p sampling parameter. Defaults to 1.0.\n\n    Returns:\n        GenerationOutputs: The generation outputs.\n    \"\"\"\n\n    outputs = super().generate(\n        input_ids,\n        num_beams=num_beams,\n        decoder_start_token_id=decoder_start_token_id,\n        decoder_end_token_id=decoder_end_token_id,\n        num_return_sequences=num_return_sequences,\n        min_gen_seq_length=min_gen_seq_length,\n        max_gen_seq_length=max_gen_seq_length,\n        repetition_penalty=repetition_penalty,\n        no_repeat_ngram_size=no_repeat_ngram_size,\n        early_stopping=early_stopping,\n        length_penalty=length_penalty,\n        num_beam_groups=num_beam_groups,\n        diversity_penalty=diversity_penalty,\n        do_sample=do_sample,\n        temperature=temperature,\n        top_k=top_k,\n        top_p=top_p,\n    )\n\n    return GenerationOutputs(\n        sequences=outputs.sequences,\n        sequences_scores=outputs.sequences_scores,\n    )\n</code></pre>",
             "title": "generate"
         },
         {
             "location": "cli/models/visualbert/",
             "text": "",
             "title": "unitorch.cli.models.visualbert"
         },
@@ -1327,15 +1362,15 @@
         {
             "location": "cli/models/xpegasus/#unitorch.cli.models.xpegasus.modeling.XPegasusForGeneration.from_core_configure",
             "text": "<pre><code>from_core_configure(config, **kwargs)\n</code></pre> <p>Create an instance of XPegasusForGeneration from a core configuration.</p> <p>Parameters:</p> Name Type Description Default <code>config</code> <p>The core configuration.</p> required <code>**kwargs</code> <p>Additional keyword arguments.</p> <code>{}</code> <p>Returns:</p> Name Type Description <code>XPegasusForGeneration</code> <p>The instantiated XPegasusForGeneration model.</p> Source code in <code>src/unitorch/cli/models/xpegasus/modeling.py</code> <pre><code>@classmethod\n@add_default_section_for_init(\"core/model/generation/xpegasus\")\ndef from_core_configure(cls, config, **kwargs):\n\"\"\"\n    Create an instance of XPegasusForGeneration from a core configuration.\n\n    Args:\n        config: The core configuration.\n        **kwargs: Additional keyword arguments.\n\n    Returns:\n        XPegasusForGeneration: The instantiated XPegasusForGeneration model.\n    \"\"\"\n    config.set_default_section(\"core/model/generation/xpegasus\")\n    pretrained_name = config.getoption(\"pretrained_name\", \"default-xpegasus\")\n    config_path = config.getoption(\"config_path\", None)\n    config_path = pop_value(\n        config_path,\n        nested_dict_value(pretrained_xpegasus_infos, pretrained_name, \"config\"),\n    )\n\n    config_path = cached_path(config_path)\n    gradient_checkpointing = config.getoption(\"gradient_checkpointing\", False)\n\n    inst = cls(config_path, gradient_checkpointing)\n    pretrained_weight_path = config.getoption(\"pretrained_weight_path\", None)\n    weight_path = pop_value(\n        pretrained_weight_path,\n        nested_dict_value(pretrained_xpegasus_infos, pretrained_name, \"weight\"),\n        check_none=False,\n    )\n    if weight_path is not None:\n        weight_path = cached_path(weight_path)\n        inst.from_pretrained(weight_path)\n\n    return inst\n</code></pre>",
             "title": "from_core_configure  <code>classmethod</code>"
         },
         {
             "location": "cli/models/xpegasus/#unitorch.cli.models.xpegasus.modeling.XPegasusForGeneration.generate",
-            "text": "<pre><code>generate(\n    input_ids: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 0,\n    decoder_end_token_id: Optional[int] = 1,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n)\n</code></pre> <p>Generate sequences using the XPegasus model.</p> <p>Parameters:</p> Name Type Description Default <code>input_ids</code> <code>torch.Tensor</code> <p>Input token IDs.</p> required <code>num_beams</code> <code>int</code> <p>Number of beams for beam search. Defaults to 5.</p> <code>5</code> <code>decoder_start_token_id</code> <code>int</code> <p>Decoder start token ID. Defaults to 0.</p> <code>0</code> <code>decoder_end_token_id</code> <code>int</code> <p>Decoder end token ID. Defaults to 1.</p> <code>1</code> <code>num_return_sequences</code> <code>int</code> <p>Number of generated sequences to return. Defaults to 1.</p> <code>1</code> <code>min_gen_seq_length</code> <code>int</code> <p>Minimum generation sequence length. Defaults to 0.</p> <code>0</code> <code>max_gen_seq_length</code> <code>int</code> <p>Maximum generation sequence length. Defaults to 48.</p> <code>48</code> <code>repetition_penalty</code> <code>float</code> <p>Repetition penalty. Defaults to 1.0.</p> <code>1.0</code> <code>no_repeat_ngram_size</code> <code>int</code> <p>Size of n-grams to prevent repetition. Defaults to 0.</p> <code>0</code> <code>early_stopping</code> <code>bool</code> <p>Whether to perform early stopping. Defaults to True.</p> <code>True</code> <code>length_penalty</code> <code>float</code> <p>Length penalty. Defaults to 1.0.</p> <code>1.0</code> <code>num_beam_groups</code> <code>int</code> <p>Number of beam groups for diverse beam search. Defaults to 1.</p> <code>1</code> <code>diversity_penalty</code> <code>float</code> <p>Diversity penalty for diverse beam search. Defaults to 0.0.</p> <code>0.0</code> <code>do_sample</code> <code>bool</code> <p>Whether to use sampling for generation. Defaults to False.</p> <code>False</code> <code>temperature</code> <code>float</code> <p>Sampling temperature. Defaults to 1.0.</p> <code>1.0</code> <code>top_k</code> <code>int</code> <p>Top-k sampling parameter. Defaults to 50.</p> <code>50</code> <code>top_p</code> <code>float</code> <p>Top-p sampling parameter. Defaults to 1.0.</p> <code>1.0</code> <p>Returns:</p> Name Type Description <code>GenerationOutputs</code> <p>The generation outputs.</p> Source code in <code>src/unitorch/cli/models/xpegasus/modeling.py</code> <pre><code>@add_default_section_for_function(\"core/model/generation/xpegasus\")\n@torch.no_grad()\n@autocast()\ndef generate(\n    self,\n    input_ids: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 0,\n    decoder_end_token_id: Optional[int] = 1,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n):\n\"\"\"\n    Generate sequences using the XPegasus model.\n\n    Args:\n        input_ids (torch.Tensor): Input token IDs.\n        num_beams (int, optional): Number of beams for beam search. Defaults to 5.\n        decoder_start_token_id (int, optional): Decoder start token ID. Defaults to 0.\n        decoder_end_token_id (int, optional): Decoder end token ID. Defaults to 1.\n        num_return_sequences (int, optional): Number of generated sequences to return. Defaults to 1.\n        min_gen_seq_length (int, optional): Minimum generation sequence length. Defaults to 0.\n        max_gen_seq_length (int, optional): Maximum generation sequence length. Defaults to 48.\n        repetition_penalty (float, optional): Repetition penalty. Defaults to 1.0.\n        no_repeat_ngram_size (int, optional): Size of n-grams to prevent repetition. Defaults to 0.\n        early_stopping (bool, optional): Whether to perform early stopping. Defaults to True.\n        length_penalty (float, optional): Length penalty. Defaults to 1.0.\n        num_beam_groups (int, optional): Number of beam groups for diverse beam search. Defaults to 1.\n        diversity_penalty (float, optional): Diversity penalty for diverse beam search. Defaults to 0.0.\n        do_sample (bool, optional): Whether to use sampling for generation. Defaults to False.\n        temperature (float, optional): Sampling temperature. Defaults to 1.0.\n        top_k (int, optional): Top-k sampling parameter. Defaults to 50.\n        top_p (float, optional): Top-p sampling parameter. Defaults to 1.0.\n\n    Returns:\n        GenerationOutputs: The generation outputs.\n    \"\"\"\n    outputs = super().generate(\n        input_ids,\n        num_beams=num_beams,\n        decoder_start_token_id=decoder_start_token_id,\n        decoder_end_token_id=decoder_end_token_id,\n        num_return_sequences=num_return_sequences,\n        min_gen_seq_length=min_gen_seq_length,\n        max_gen_seq_length=max_gen_seq_length,\n        repetition_penalty=repetition_penalty,\n        no_repeat_ngram_size=no_repeat_ngram_size,\n        early_stopping=early_stopping,\n        length_penalty=length_penalty,\n        num_beam_groups=num_beam_groups,\n        diversity_penalty=diversity_penalty,\n        do_sample=do_sample,\n        temperature=temperature,\n        top_k=top_k,\n        top_p=top_p,\n    )\n\n    return GenerationOutputs(\n        sequences=outputs.sequences,\n        sequences_scores=outputs.sequences_scores,\n    )\n</code></pre>",
+            "text": "<pre><code>generate(\n    input_ids: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 0,\n    decoder_end_token_id: Optional[\n        Union[int, List[int]]\n    ] = 1,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n)\n</code></pre> <p>Generate sequences using the XPegasus model.</p> <p>Parameters:</p> Name Type Description Default <code>input_ids</code> <code>torch.Tensor</code> <p>Input token IDs.</p> required <code>num_beams</code> <code>int</code> <p>Number of beams for beam search. Defaults to 5.</p> <code>5</code> <code>decoder_start_token_id</code> <code>int</code> <p>Decoder start token ID. Defaults to 0.</p> <code>0</code> <code>decoder_end_token_id</code> <code>int or List[int]</code> <p>The ID(s) of the decoder end token(s). Defaults to 1.</p> <code>1</code> <code>num_return_sequences</code> <code>int</code> <p>Number of generated sequences to return. Defaults to 1.</p> <code>1</code> <code>min_gen_seq_length</code> <code>int</code> <p>Minimum generation sequence length. Defaults to 0.</p> <code>0</code> <code>max_gen_seq_length</code> <code>int</code> <p>Maximum generation sequence length. Defaults to 48.</p> <code>48</code> <code>repetition_penalty</code> <code>float</code> <p>Repetition penalty. Defaults to 1.0.</p> <code>1.0</code> <code>no_repeat_ngram_size</code> <code>int</code> <p>Size of n-grams to prevent repetition. Defaults to 0.</p> <code>0</code> <code>early_stopping</code> <code>bool</code> <p>Whether to perform early stopping. Defaults to True.</p> <code>True</code> <code>length_penalty</code> <code>float</code> <p>Length penalty. Defaults to 1.0.</p> <code>1.0</code> <code>num_beam_groups</code> <code>int</code> <p>Number of beam groups for diverse beam search. Defaults to 1.</p> <code>1</code> <code>diversity_penalty</code> <code>float</code> <p>Diversity penalty for diverse beam search. Defaults to 0.0.</p> <code>0.0</code> <code>do_sample</code> <code>bool</code> <p>Whether to use sampling for generation. Defaults to False.</p> <code>False</code> <code>temperature</code> <code>float</code> <p>Sampling temperature. Defaults to 1.0.</p> <code>1.0</code> <code>top_k</code> <code>int</code> <p>Top-k sampling parameter. Defaults to 50.</p> <code>50</code> <code>top_p</code> <code>float</code> <p>Top-p sampling parameter. Defaults to 1.0.</p> <code>1.0</code> <p>Returns:</p> Name Type Description <code>GenerationOutputs</code> <p>The generation outputs.</p> Source code in <code>src/unitorch/cli/models/xpegasus/modeling.py</code> <pre><code>@add_default_section_for_function(\"core/model/generation/xpegasus\")\n@torch.no_grad()\n@autocast()\ndef generate(\n    self,\n    input_ids: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 0,\n    decoder_end_token_id: Optional[Union[int, List[int]]] = 1,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n):\n\"\"\"\n    Generate sequences using the XPegasus model.\n\n    Args:\n        input_ids (torch.Tensor): Input token IDs.\n        num_beams (int, optional): Number of beams for beam search. Defaults to 5.\n        decoder_start_token_id (int, optional): Decoder start token ID. Defaults to 0.\n        decoder_end_token_id (int or List[int], optional): The ID(s) of the decoder end token(s). Defaults to 1.\n        num_return_sequences (int, optional): Number of generated sequences to return. Defaults to 1.\n        min_gen_seq_length (int, optional): Minimum generation sequence length. Defaults to 0.\n        max_gen_seq_length (int, optional): Maximum generation sequence length. Defaults to 48.\n        repetition_penalty (float, optional): Repetition penalty. Defaults to 1.0.\n        no_repeat_ngram_size (int, optional): Size of n-grams to prevent repetition. Defaults to 0.\n        early_stopping (bool, optional): Whether to perform early stopping. Defaults to True.\n        length_penalty (float, optional): Length penalty. Defaults to 1.0.\n        num_beam_groups (int, optional): Number of beam groups for diverse beam search. Defaults to 1.\n        diversity_penalty (float, optional): Diversity penalty for diverse beam search. Defaults to 0.0.\n        do_sample (bool, optional): Whether to use sampling for generation. Defaults to False.\n        temperature (float, optional): Sampling temperature. Defaults to 1.0.\n        top_k (int, optional): Top-k sampling parameter. Defaults to 50.\n        top_p (float, optional): Top-p sampling parameter. Defaults to 1.0.\n\n    Returns:\n        GenerationOutputs: The generation outputs.\n    \"\"\"\n    outputs = super().generate(\n        input_ids,\n        num_beams=num_beams,\n        decoder_start_token_id=decoder_start_token_id,\n        decoder_end_token_id=decoder_end_token_id,\n        num_return_sequences=num_return_sequences,\n        min_gen_seq_length=min_gen_seq_length,\n        max_gen_seq_length=max_gen_seq_length,\n        repetition_penalty=repetition_penalty,\n        no_repeat_ngram_size=no_repeat_ngram_size,\n        early_stopping=early_stopping,\n        length_penalty=length_penalty,\n        num_beam_groups=num_beam_groups,\n        diversity_penalty=diversity_penalty,\n        do_sample=do_sample,\n        temperature=temperature,\n        top_k=top_k,\n        top_p=top_p,\n    )\n\n    return GenerationOutputs(\n        sequences=outputs.sequences,\n        sequences_scores=outputs.sequences_scores,\n    )\n</code></pre>",
             "title": "generate"
         },
         {
             "location": "cli/models/xprophetnet/",
             "text": "",
             "title": "unitorch.cli.models.xprophetnet"
         },
@@ -1362,15 +1397,15 @@
         {
             "location": "cli/models/xprophetnet/#unitorch.cli.models.xprophetnet.modeling.XProphetNetForGeneration.from_core_configure",
             "text": "<pre><code>from_core_configure(config, **kwargs)\n</code></pre> <p>Create an instance of XProphetNetForGeneration from a core configuration.</p> <p>Parameters:</p> Name Type Description Default <code>config</code> <p>The core configuration.</p> required <code>**kwargs</code> <p>Additional keyword arguments.</p> <code>{}</code> <p>Returns:</p> Name Type Description <code>XProphetNetForGeneration</code> <p>An instance of XProphetNetForGeneration.</p> Source code in <code>src/unitorch/cli/models/xprophetnet/modeling.py</code> <pre><code>@classmethod\n@add_default_section_for_init(\"core/model/generation/xprophetnet\")\ndef from_core_configure(cls, config, **kwargs):\n\"\"\"\n    Create an instance of XProphetNetForGeneration from a core configuration.\n\n    Args:\n        config: The core configuration.\n        **kwargs: Additional keyword arguments.\n\n    Returns:\n        XProphetNetForGeneration: An instance of XProphetNetForGeneration.\n    \"\"\"\n    config.set_default_section(\"core/model/generation/xprophetnet\")\n    pretrained_name = config.getoption(\"pretrained_name\", \"default-xprophetnet\")\n    config_path = config.getoption(\"config_path\", None)\n    config_path = pop_value(\n        config_path,\n        nested_dict_value(pretrained_xprophetnet_infos, pretrained_name, \"config\"),\n    )\n\n    config_path = cached_path(config_path)\n    freeze_input_embedding = config.getoption(\"freeze_input_embedding\", True)\n    gradient_checkpointing = config.getoption(\"gradient_checkpointing\", False)\n\n    inst = cls(\n        config_path,\n        freeze_input_embedding=freeze_input_embedding,\n        gradient_checkpointing=gradient_checkpointing,\n    )\n    pretrained_weight_path = config.getoption(\"pretrained_weight_path\", None)\n    weight_path = pop_value(\n        pretrained_weight_path,\n        nested_dict_value(pretrained_xprophetnet_infos, pretrained_name, \"weight\"),\n        check_none=False,\n    )\n    if weight_path is not None:\n        weight_path = cached_path(weight_path)\n        inst.from_pretrained(weight_path)\n\n    return inst\n</code></pre>",
             "title": "from_core_configure  <code>classmethod</code>"
         },
         {
             "location": "cli/models/xprophetnet/#unitorch.cli.models.xprophetnet.modeling.XProphetNetForGeneration.generate",
-            "text": "<pre><code>generate(\n    input_ids: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 2,\n    decoder_end_token_id: Optional[int] = 2,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n)\n</code></pre> <p>Generate sequences using the XProphetNetForGeneration model.</p> <p>Parameters:</p> Name Type Description Default <code>input_ids</code> <code>torch.Tensor</code> <p>Input tensor IDs.</p> required <code>num_beams</code> <code>int</code> <p>The number of beams for beam search. Defaults to 5.</p> <code>5</code> <code>decoder_start_token_id</code> <code>int</code> <p>The ID of the decoder start token. Defaults to 2.</p> <code>2</code> <code>decoder_end_token_id</code> <code>int</code> <p>The ID of the decoder end token. Defaults to 2.</p> <code>2</code> <code>num_return_sequences</code> <code>int</code> <p>The number of returned sequences. Defaults to 1.</p> <code>1</code> <code>min_gen_seq_length</code> <code>int</code> <p>The minimum generated sequence length. Defaults to 0.</p> <code>0</code> <code>max_gen_seq_length</code> <code>int</code> <p>The maximum generated sequence length. Defaults to 48.</p> <code>48</code> <code>repetition_penalty</code> <code>float</code> <p>The repetition penalty. Defaults to 1.0.</p> <code>1.0</code> <code>no_repeat_ngram_size</code> <code>int</code> <p>The size of n-grams that should not be repeated. Defaults to 0.</p> <code>0</code> <code>early_stopping</code> <code>bool</code> <p>Whether to stop generation early. Defaults to True.</p> <code>True</code> <code>length_penalty</code> <code>float</code> <p>The length penalty. Defaults to 1.0.</p> <code>1.0</code> <code>num_beam_groups</code> <code>int</code> <p>The number of beam groups for diverse beam search. Defaults to 1.</p> <code>1</code> <code>diversity_penalty</code> <code>float</code> <p>The diversity penalty for diverse beam search. Defaults to 0.0.</p> <code>0.0</code> <code>do_sample</code> <code>bool</code> <p>Whether to use sampling for generation. Defaults to False.</p> <code>False</code> <code>temperature</code> <code>float</code> <p>The temperature for sampling. Defaults to 1.0.</p> <code>1.0</code> <code>top_k</code> <code>int</code> <p>The top-k value for sampling. Defaults to 50.</p> <code>50</code> <code>top_p</code> <code>float</code> <p>The top-p value for sampling. Defaults to 1.0.</p> <code>1.0</code> <p>Returns:</p> Name Type Description <code>GenerationOutputs</code> <p>The generation outputs.</p> Source code in <code>src/unitorch/cli/models/xprophetnet/modeling.py</code> <pre><code>@add_default_section_for_function(\"core/model/generation/xprophetnet\")\n@torch.no_grad()\n@autocast()\ndef generate(\n    self,\n    input_ids: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 2,\n    decoder_end_token_id: Optional[int] = 2,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n):\n\"\"\"\n    Generate sequences using the XProphetNetForGeneration model.\n\n    Args:\n        input_ids (torch.Tensor): Input tensor IDs.\n        num_beams (int, optional): The number of beams for beam search. Defaults to 5.\n        decoder_start_token_id (int, optional): The ID of the decoder start token. Defaults to 2.\n        decoder_end_token_id (int, optional): The ID of the decoder end token. Defaults to 2.\n        num_return_sequences (int, optional): The number of returned sequences. Defaults to 1.\n        min_gen_seq_length (int, optional): The minimum generated sequence length. Defaults to 0.\n        max_gen_seq_length (int, optional): The maximum generated sequence length. Defaults to 48.\n        repetition_penalty (float, optional): The repetition penalty. Defaults to 1.0.\n        no_repeat_ngram_size (int, optional): The size of n-grams that should not be repeated. Defaults to 0.\n        early_stopping (bool, optional): Whether to stop generation early. Defaults to True.\n        length_penalty (float, optional): The length penalty. Defaults to 1.0.\n        num_beam_groups (int, optional): The number of beam groups for diverse beam search. Defaults to 1.\n        diversity_penalty (float, optional): The diversity penalty for diverse beam search. Defaults to 0.0.\n        do_sample (bool, optional): Whether to use sampling for generation. Defaults to False.\n        temperature (float, optional): The temperature for sampling. Defaults to 1.0.\n        top_k (int, optional): The top-k value for sampling. Defaults to 50.\n        top_p (float, optional): The top-p value for sampling. Defaults to 1.0.\n\n    Returns:\n        GenerationOutputs: The generation outputs.\n    \"\"\"\n    outputs = super().generate(\n        input_ids,\n        num_beams=num_beams,\n        decoder_start_token_id=decoder_start_token_id,\n        decoder_end_token_id=decoder_end_token_id,\n        num_return_sequences=num_return_sequences,\n        min_gen_seq_length=min_gen_seq_length,\n        max_gen_seq_length=max_gen_seq_length,\n        repetition_penalty=repetition_penalty,\n        no_repeat_ngram_size=no_repeat_ngram_size,\n        early_stopping=early_stopping,\n        length_penalty=length_penalty,\n        num_beam_groups=num_beam_groups,\n        diversity_penalty=diversity_penalty,\n        do_sample=do_sample,\n        temperature=temperature,\n        top_k=top_k,\n        top_p=top_p,\n    )\n\n    return GenerationOutputs(\n        sequences=outputs.sequences,\n        sequences_scores=outputs.sequences_scores,\n    )\n</code></pre>",
+            "text": "<pre><code>generate(\n    input_ids: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 2,\n    decoder_end_token_id: Optional[\n        Union[int, List[int]]\n    ] = 2,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n)\n</code></pre> <p>Generate sequences using the XProphetNetForGeneration model.</p> <p>Parameters:</p> Name Type Description Default <code>input_ids</code> <code>torch.Tensor</code> <p>Input tensor IDs.</p> required <code>num_beams</code> <code>int</code> <p>The number of beams for beam search. Defaults to 5.</p> <code>5</code> <code>decoder_start_token_id</code> <code>int</code> <p>The ID of the decoder start token. Defaults to 2.</p> <code>2</code> <code>decoder_end_token_id</code> <code>int or List[int]</code> <p>The ID of the decoder end token. Defaults to 2.</p> <code>2</code> <code>num_return_sequences</code> <code>int</code> <p>The number of returned sequences. Defaults to 1.</p> <code>1</code> <code>min_gen_seq_length</code> <code>int</code> <p>The minimum generated sequence length. Defaults to 0.</p> <code>0</code> <code>max_gen_seq_length</code> <code>int</code> <p>The maximum generated sequence length. Defaults to 48.</p> <code>48</code> <code>repetition_penalty</code> <code>float</code> <p>The repetition penalty. Defaults to 1.0.</p> <code>1.0</code> <code>no_repeat_ngram_size</code> <code>int</code> <p>The size of n-grams that should not be repeated. Defaults to 0.</p> <code>0</code> <code>early_stopping</code> <code>bool</code> <p>Whether to stop generation early. Defaults to True.</p> <code>True</code> <code>length_penalty</code> <code>float</code> <p>The length penalty. Defaults to 1.0.</p> <code>1.0</code> <code>num_beam_groups</code> <code>int</code> <p>The number of beam groups for diverse beam search. Defaults to 1.</p> <code>1</code> <code>diversity_penalty</code> <code>float</code> <p>The diversity penalty for diverse beam search. Defaults to 0.0.</p> <code>0.0</code> <code>do_sample</code> <code>bool</code> <p>Whether to use sampling for generation. Defaults to False.</p> <code>False</code> <code>temperature</code> <code>float</code> <p>The temperature for sampling. Defaults to 1.0.</p> <code>1.0</code> <code>top_k</code> <code>int</code> <p>The top-k value for sampling. Defaults to 50.</p> <code>50</code> <code>top_p</code> <code>float</code> <p>The top-p value for sampling. Defaults to 1.0.</p> <code>1.0</code> <p>Returns:</p> Name Type Description <code>GenerationOutputs</code> <p>The generation outputs.</p> Source code in <code>src/unitorch/cli/models/xprophetnet/modeling.py</code> <pre><code>@add_default_section_for_function(\"core/model/generation/xprophetnet\")\n@torch.no_grad()\n@autocast()\ndef generate(\n    self,\n    input_ids: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 2,\n    decoder_end_token_id: Optional[Union[int, List[int]]] = 2,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n):\n\"\"\"\n    Generate sequences using the XProphetNetForGeneration model.\n\n    Args:\n        input_ids (torch.Tensor): Input tensor IDs.\n        num_beams (int, optional): The number of beams for beam search. Defaults to 5.\n        decoder_start_token_id (int, optional): The ID of the decoder start token. Defaults to 2.\n        decoder_end_token_id (int or List[int], optional): The ID of the decoder end token. Defaults to 2.\n        num_return_sequences (int, optional): The number of returned sequences. Defaults to 1.\n        min_gen_seq_length (int, optional): The minimum generated sequence length. Defaults to 0.\n        max_gen_seq_length (int, optional): The maximum generated sequence length. Defaults to 48.\n        repetition_penalty (float, optional): The repetition penalty. Defaults to 1.0.\n        no_repeat_ngram_size (int, optional): The size of n-grams that should not be repeated. Defaults to 0.\n        early_stopping (bool, optional): Whether to stop generation early. Defaults to True.\n        length_penalty (float, optional): The length penalty. Defaults to 1.0.\n        num_beam_groups (int, optional): The number of beam groups for diverse beam search. Defaults to 1.\n        diversity_penalty (float, optional): The diversity penalty for diverse beam search. Defaults to 0.0.\n        do_sample (bool, optional): Whether to use sampling for generation. Defaults to False.\n        temperature (float, optional): The temperature for sampling. Defaults to 1.0.\n        top_k (int, optional): The top-k value for sampling. Defaults to 50.\n        top_p (float, optional): The top-p value for sampling. Defaults to 1.0.\n\n    Returns:\n        GenerationOutputs: The generation outputs.\n    \"\"\"\n    outputs = super().generate(\n        input_ids,\n        num_beams=num_beams,\n        decoder_start_token_id=decoder_start_token_id,\n        decoder_end_token_id=decoder_end_token_id,\n        num_return_sequences=num_return_sequences,\n        min_gen_seq_length=min_gen_seq_length,\n        max_gen_seq_length=max_gen_seq_length,\n        repetition_penalty=repetition_penalty,\n        no_repeat_ngram_size=no_repeat_ngram_size,\n        early_stopping=early_stopping,\n        length_penalty=length_penalty,\n        num_beam_groups=num_beam_groups,\n        diversity_penalty=diversity_penalty,\n        do_sample=do_sample,\n        temperature=temperature,\n        top_k=top_k,\n        top_p=top_p,\n    )\n\n    return GenerationOutputs(\n        sequences=outputs.sequences,\n        sequences_scores=outputs.sequences_scores,\n    )\n</code></pre>",
             "title": "generate"
         },
         {
             "location": "examples/caption/blip/",
             "text": "<p>\u00a0\u00a0\u00a0\u00a0In this tutorial, we will learn how to perform image caption using the Blip model. Blip is a transformer-based model that has been pre-trained on a large corpus of text/image and can be fine-tuned for specific downstream tasks like multi-modal classification &amp; image caption.</p>",
             "title": "Blip Image Caption Tutorial"
         },
@@ -1732,15 +1767,15 @@
         {
             "location": "models/bart/#unitorch.models.bart.modeling.BartForGeneration.forward",
             "text": "<pre><code>forward(\n    input_ids: torch.Tensor,\n    attention_mask: torch.Tensor,\n    decoder_input_ids: torch.Tensor,\n    decoder_attention_mask: torch.Tensor,\n)\n</code></pre> <p>Performs forward pass of the BartForGeneration model.</p> <p>Parameters:</p> Name Type Description Default <code>input_ids</code> <code>torch.Tensor</code> <p>Tensor of input token IDs.</p> required <code>attention_mask</code> <code>torch.Tensor</code> <p>Tensor indicating which tokens should be attended to.</p> required <code>decoder_input_ids</code> <code>torch.Tensor</code> <p>Tensor of decoder input token IDs.</p> required <code>decoder_attention_mask</code> <code>torch.Tensor</code> <p>Tensor indicating which decoder tokens should be attended to.</p> required <p>Returns:</p> Type Description <code>torch.Tensor</code> <p>Output logits of the model.</p> Source code in <code>src/unitorch/models/bart/modeling.py</code> <pre><code>def forward(\n    self,\n    input_ids: torch.Tensor,\n    attention_mask: torch.Tensor,\n    decoder_input_ids: torch.Tensor,\n    decoder_attention_mask: torch.Tensor,\n):\n\"\"\"\n    Performs forward pass of the BartForGeneration model.\n\n    Args:\n        input_ids (torch.Tensor): Tensor of input token IDs.\n        attention_mask (torch.Tensor): Tensor indicating which tokens should be attended to.\n        decoder_input_ids (torch.Tensor): Tensor of decoder input token IDs.\n        decoder_attention_mask (torch.Tensor): Tensor indicating which decoder tokens should be attended to.\n\n    Returns:\n        (torch.Tensor): Output logits of the model.\n    \"\"\"\n    outputs = self.model(\n        input_ids=input_ids,\n        attention_mask=attention_mask,\n        decoder_input_ids=decoder_input_ids,\n        decoder_attention_mask=decoder_attention_mask,\n        return_dict=True,\n    )\n    logits = outputs.logits\n    print(\"model :\", logits[0, 0, 0].item(), logits[0, 0, 41552].item())\n    return logits\n</code></pre>",
             "title": "forward"
         },
         {
             "location": "models/bart/#unitorch.models.bart.modeling.BartForGeneration.generate",
-            "text": "<pre><code>generate(\n    input_ids: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 2,\n    decoder_end_token_id: Optional[int] = 2,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n)\n</code></pre> <p>Generates text using the BartForGeneration model.</p> <p>Parameters:</p> Name Type Description Default <code>input_ids</code> <code>torch.Tensor</code> <p>Tensor of input token IDs.</p> required <code>num_beams</code> <code>int</code> <p>Number of beams for beam search. Defaults to 5.</p> <code>5</code> <code>decoder_start_token_id</code> <code>int</code> <p>Start token ID for the decoder. Defaults to 2.</p> <code>2</code> <code>decoder_end_token_id</code> <code>int</code> <p>End token ID for the decoder. Defaults to 2.</p> <code>2</code> <code>num_return_sequences</code> <code>int</code> <p>Number of sequences to return. Defaults to 1.</p> <code>1</code> <code>min_gen_seq_length</code> <code>int</code> <p>Minimum length of generated sequences. Defaults to 0.</p> <code>0</code> <code>max_gen_seq_length</code> <code>int</code> <p>Maximum length of generated sequences. Defaults to 48.</p> <code>48</code> <code>repetition_penalty</code> <code>float</code> <p>Repetition penalty for generated sequences. Defaults to 1.0.</p> <code>1.0</code> <code>no_repeat_ngram_size</code> <code>int</code> <p>Size of n-grams to avoid repetition. Defaults to 0.</p> <code>0</code> <code>early_stopping</code> <code>bool</code> <p>Whether to stop generation early. Defaults to True.</p> <code>True</code> <code>length_penalty</code> <code>float</code> <p>Length penalty for generated sequences. Defaults to 1.0.</p> <code>1.0</code> <code>num_beam_groups</code> <code>int</code> <p>Number of beam groups for diverse beam search. Defaults to 1.</p> <code>1</code> <code>diversity_penalty</code> <code>float</code> <p>Diversity penalty for diverse beam search. Defaults to 0.0.</p> <code>0.0</code> <code>do_sample</code> <code>bool</code> <p>Whether to use sampling during generation. Defaults to False.</p> <code>False</code> <code>temperature</code> <code>float</code> <p>Temperature for sampling. Defaults to 1.0.</p> <code>1.0</code> <code>top_k</code> <code>int</code> <p>Value for top-k sampling. Defaults to 50.</p> <code>50</code> <code>top_p</code> <code>float</code> <p>Value for top-p sampling. Defaults to 1.0.</p> <code>1.0</code> <p>Returns:</p> Name Type Description <code>GenericOutputs</code> <p>Generated sequences and their scores.</p> Source code in <code>src/unitorch/models/bart/modeling.py</code> <pre><code>@torch.no_grad()\ndef generate(\n    self,\n    input_ids: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 2,\n    decoder_end_token_id: Optional[int] = 2,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n):\n\"\"\"\n    Generates text using the BartForGeneration model.\n\n    Args:\n        input_ids (torch.Tensor): Tensor of input token IDs.\n        num_beams (int, optional): Number of beams for beam search. Defaults to 5.\n        decoder_start_token_id (int, optional): Start token ID for the decoder. Defaults to 2.\n        decoder_end_token_id (int, optional): End token ID for the decoder. Defaults to 2.\n        num_return_sequences (int, optional): Number of sequences to return. Defaults to 1.\n        min_gen_seq_length (int, optional): Minimum length of generated sequences. Defaults to 0.\n        max_gen_seq_length (int, optional): Maximum length of generated sequences. Defaults to 48.\n        repetition_penalty (float, optional): Repetition penalty for generated sequences. Defaults to 1.0.\n        no_repeat_ngram_size (int, optional): Size of n-grams to avoid repetition. Defaults to 0.\n        early_stopping (bool, optional): Whether to stop generation early. Defaults to True.\n        length_penalty (float, optional): Length penalty for generated sequences. Defaults to 1.0.\n        num_beam_groups (int, optional): Number of beam groups for diverse beam search. Defaults to 1.\n        diversity_penalty (float, optional): Diversity penalty for diverse beam search. Defaults to 0.0.\n        do_sample (bool, optional): Whether to use sampling during generation. Defaults to False.\n        temperature (float, optional): Temperature for sampling. Defaults to 1.0.\n        top_k (int, optional): Value for top-k sampling. Defaults to 50.\n        top_p (float, optional): Value for top-p sampling. Defaults to 1.0.\n\n    Returns:\n        GenericOutputs: Generated sequences and their scores.\n    \"\"\"\n    outputs = self.model.generate(\n        input_ids,\n        max_length=max_gen_seq_length,\n        min_length=min_gen_seq_length,\n        num_beams=num_beams,\n        do_sample=do_sample,\n        decoder_start_token_id=decoder_start_token_id,\n        no_repeat_ngram_size=no_repeat_ngram_size,\n        early_stopping=early_stopping,\n        length_penalty=length_penalty,\n        repetition_penalty=repetition_penalty,\n        num_return_sequences=num_return_sequences,\n        bos_token_id=decoder_start_token_id,\n        eos_token_id=decoder_end_token_id,\n        num_beam_groups=num_beam_groups,\n        diversity_penalty=diversity_penalty,\n        temperature=temperature,\n        top_k=top_k,\n        top_p=top_p,\n        return_dict_in_generate=True,\n        output_scores=True,\n    )\n\n    sequences = outputs.sequences.reshape(\n        -1, num_return_sequences, outputs.sequences.size(-1)\n    )\n    outputs.sequences = torch.zeros(\n        sequences.size(0), num_return_sequences, max_gen_seq_length\n    ).to(device=sequences.device)\n    outputs.sequences[:, :, : sequences.size(-1)].copy_(sequences)\n\n    if num_return_sequences == 1:\n        outputs.sequences = outputs.sequences.reshape(-1, max_gen_seq_length)\n\n    return GenericOutputs(\n        sequences=outputs.sequences, sequences_scores=outputs.sequences_scores\n    )\n</code></pre>",
+            "text": "<pre><code>generate(\n    input_ids: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 2,\n    decoder_end_token_id: Optional[\n        Union[int, List[int]]\n    ] = 2,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n)\n</code></pre> <p>Generates text using the BartForGeneration model.</p> <p>Parameters:</p> Name Type Description Default <code>input_ids</code> <code>torch.Tensor</code> <p>Tensor of input token IDs.</p> required <code>num_beams</code> <code>int</code> <p>Number of beams for beam search. Defaults to 5.</p> <code>5</code> <code>decoder_start_token_id</code> <code>int</code> <p>The ID of the decoder start token. Defaults to 2.</p> <code>2</code> <code>decoder_end_token_id</code> <code>int or List[int]</code> <p>The ID(s) of the decoder end token(s). Defaults to 2.</p> <code>2</code> <code>num_return_sequences</code> <code>int</code> <p>Number of sequences to return. Defaults to 1.</p> <code>1</code> <code>min_gen_seq_length</code> <code>int</code> <p>Minimum length of generated sequences. Defaults to 0.</p> <code>0</code> <code>max_gen_seq_length</code> <code>int</code> <p>Maximum length of generated sequences. Defaults to 48.</p> <code>48</code> <code>repetition_penalty</code> <code>float</code> <p>Repetition penalty for generated sequences. Defaults to 1.0.</p> <code>1.0</code> <code>no_repeat_ngram_size</code> <code>int</code> <p>Size of n-grams to avoid repetition. Defaults to 0.</p> <code>0</code> <code>early_stopping</code> <code>bool</code> <p>Whether to stop generation early. Defaults to True.</p> <code>True</code> <code>length_penalty</code> <code>float</code> <p>Length penalty for generated sequences. Defaults to 1.0.</p> <code>1.0</code> <code>num_beam_groups</code> <code>int</code> <p>Number of beam groups for diverse beam search. Defaults to 1.</p> <code>1</code> <code>diversity_penalty</code> <code>float</code> <p>Diversity penalty for diverse beam search. Defaults to 0.0.</p> <code>0.0</code> <code>do_sample</code> <code>bool</code> <p>Whether to use sampling during generation. Defaults to False.</p> <code>False</code> <code>temperature</code> <code>float</code> <p>Temperature for sampling. Defaults to 1.0.</p> <code>1.0</code> <code>top_k</code> <code>int</code> <p>Value for top-k sampling. Defaults to 50.</p> <code>50</code> <code>top_p</code> <code>float</code> <p>Value for top-p sampling. Defaults to 1.0.</p> <code>1.0</code> <p>Returns:</p> Name Type Description <code>GenericOutputs</code> <p>Generated sequences and their scores.</p> Source code in <code>src/unitorch/models/bart/modeling.py</code> <pre><code>@torch.no_grad()\ndef generate(\n    self,\n    input_ids: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 2,\n    decoder_end_token_id: Optional[Union[int, List[int]]] = 2,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n):\n\"\"\"\n    Generates text using the BartForGeneration model.\n\n    Args:\n        input_ids (torch.Tensor): Tensor of input token IDs.\n        num_beams (int, optional): Number of beams for beam search. Defaults to 5.\n        decoder_start_token_id (int, optional): The ID of the decoder start token. Defaults to 2.\n        decoder_end_token_id (int or List[int], optional): The ID(s) of the decoder end token(s). Defaults to 2.\n        num_return_sequences (int, optional): Number of sequences to return. Defaults to 1.\n        min_gen_seq_length (int, optional): Minimum length of generated sequences. Defaults to 0.\n        max_gen_seq_length (int, optional): Maximum length of generated sequences. Defaults to 48.\n        repetition_penalty (float, optional): Repetition penalty for generated sequences. Defaults to 1.0.\n        no_repeat_ngram_size (int, optional): Size of n-grams to avoid repetition. Defaults to 0.\n        early_stopping (bool, optional): Whether to stop generation early. Defaults to True.\n        length_penalty (float, optional): Length penalty for generated sequences. Defaults to 1.0.\n        num_beam_groups (int, optional): Number of beam groups for diverse beam search. Defaults to 1.\n        diversity_penalty (float, optional): Diversity penalty for diverse beam search. Defaults to 0.0.\n        do_sample (bool, optional): Whether to use sampling during generation. Defaults to False.\n        temperature (float, optional): Temperature for sampling. Defaults to 1.0.\n        top_k (int, optional): Value for top-k sampling. Defaults to 50.\n        top_p (float, optional): Value for top-p sampling. Defaults to 1.0.\n\n    Returns:\n        GenericOutputs: Generated sequences and their scores.\n    \"\"\"\n    outputs = self.model.generate(\n        input_ids,\n        max_length=max_gen_seq_length,\n        min_length=min_gen_seq_length,\n        num_beams=num_beams,\n        do_sample=do_sample,\n        decoder_start_token_id=decoder_start_token_id,\n        no_repeat_ngram_size=no_repeat_ngram_size,\n        early_stopping=early_stopping,\n        length_penalty=length_penalty,\n        repetition_penalty=repetition_penalty,\n        num_return_sequences=num_return_sequences,\n        bos_token_id=decoder_start_token_id,\n        eos_token_id=decoder_end_token_id,\n        num_beam_groups=num_beam_groups,\n        diversity_penalty=diversity_penalty,\n        temperature=temperature,\n        top_k=top_k,\n        top_p=top_p,\n        return_dict_in_generate=True,\n        output_scores=True,\n    )\n\n    sequences = outputs.sequences.reshape(\n        -1, num_return_sequences, outputs.sequences.size(-1)\n    )\n    outputs.sequences = torch.zeros(\n        sequences.size(0), num_return_sequences, max_gen_seq_length\n    ).to(device=sequences.device)\n    outputs.sequences[:, :, : sequences.size(-1)].copy_(sequences)\n\n    if num_return_sequences == 1:\n        outputs.sequences = outputs.sequences.reshape(-1, max_gen_seq_length)\n\n    return GenericOutputs(\n        sequences=outputs.sequences, sequences_scores=outputs.sequences_scores\n    )\n</code></pre>",
             "title": "generate"
         },
         {
             "location": "models/beit/",
             "text": "",
             "title": "unitorch.models.beit"
         },
@@ -1872,15 +1907,15 @@
         {
             "location": "models/blip/#unitorch.models.blip.modeling.BlipForImageCaption.forward",
             "text": "<pre><code>forward(\n    pixel_values: torch.Tensor,\n    input_ids: Optional[torch.Tensor] = None,\n    attention_mask: Optional[torch.Tensor] = None,\n)\n</code></pre> <p>Forward pass of the BlipForImageCaption model.</p> <p>Parameters:</p> Name Type Description Default <code>pixel_values</code> <code>torch.Tensor</code> <p>Input pixel values.</p> required <code>input_ids</code> <code>Optional[torch.Tensor]</code> <p>Input token IDs. Defaults to None.</p> <code>None</code> <code>attention_mask</code> <code>Optional[torch.Tensor]</code> <p>Attention mask. Defaults to None.</p> <code>None</code> <p>Returns:</p> Type Description <code>torch.Tensor</code> <p>Logits for caption generation.</p> Source code in <code>src/unitorch/models/blip/modeling.py</code> <pre><code>def forward(\n    self,\n    pixel_values: torch.Tensor,\n    input_ids: Optional[torch.Tensor] = None,\n    attention_mask: Optional[torch.Tensor] = None,\n):\n\"\"\"\n    Forward pass of the BlipForImageCaption model.\n\n    Args:\n        pixel_values (torch.Tensor): Input pixel values.\n        input_ids (Optional[torch.Tensor], optional): Input token IDs. Defaults to None.\n        attention_mask (Optional[torch.Tensor], optional): Attention mask. Defaults to None.\n\n    Returns:\n        (torch.Tensor):Logits for caption generation.\n    \"\"\"\n    outputs = self.model(\n        pixel_values=pixel_values,\n        input_ids=input_ids,\n        attention_mask=attention_mask,\n        return_dict=True,\n    )\n    logits = outputs.decoder_logits\n    return logits\n</code></pre>",
             "title": "forward"
         },
         {
             "location": "models/blip/#unitorch.models.blip.modeling.BlipForImageCaption.generate",
-            "text": "<pre><code>generate(\n    pixel_values: torch.Tensor,\n    input_ids: Optional[torch.Tensor] = None,\n    attention_mask: Optional[torch.Tensor] = None,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 101,\n    decoder_end_token_id: Optional[int] = 102,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n)\n</code></pre> <p>Generates captions for the given input images.</p> <p>Parameters:</p> Name Type Description Default <code>pixel_values</code> <code>torch.Tensor</code> <p>Input pixel values.</p> required <code>input_ids</code> <code>Optional[torch.Tensor]</code> <p>Input token IDs. Defaults to None.</p> <code>None</code> <code>attention_mask</code> <code>Optional[torch.Tensor]</code> <p>Attention mask. Defaults to None.</p> <code>None</code> <code>num_beams</code> <code>Optional[int]</code> <p>Number of beams for beam search. Defaults to 5.</p> <code>5</code> <code>decoder_start_token_id</code> <code>Optional[int]</code> <p>ID of the start token for decoding. Defaults to 30522.</p> <code>101</code> <code>decoder_end_token_id</code> <code>Optional[int]</code> <p>ID of the end token for decoding. Defaults to 2.</p> <code>102</code> <code>num_return_sequences</code> <code>Optional[int]</code> <p>Number of caption sequences to return. Defaults to 1.</p> <code>1</code> <code>min_gen_seq_length</code> <code>Optional[int]</code> <p>Minimum length of generated sequences. Defaults to 0.</p> <code>0</code> <code>max_gen_seq_length</code> <code>Optional[int]</code> <p>Maximum length of generated sequences. Defaults to 48.</p> <code>48</code> <code>repetition_penalty</code> <code>Optional[float]</code> <p>Repetition penalty value. Defaults to 1.0.</p> <code>1.0</code> <code>no_repeat_ngram_size</code> <code>Optional[int]</code> <p>Size of n-grams to avoid repetition. Defaults to 0.</p> <code>0</code> <code>early_stopping</code> <code>Optional[bool]</code> <p>Whether to stop generation early. Defaults to True.</p> <code>True</code> <code>length_penalty</code> <code>Optional[float]</code> <p>Length penalty value. Defaults to 1.0.</p> <code>1.0</code> <code>num_beam_groups</code> <code>Optional[int]</code> <p>Number of groups for diverse beam search. Defaults to 1.</p> <code>1</code> <code>diversity_penalty</code> <code>Optional[float]</code> <p>Diversity penalty value. Defaults to 0.0.</p> <code>0.0</code> <code>do_sample</code> <code>Optional[bool]</code> <p>Whether to use sampling for generation. Defaults to False.</p> <code>False</code> <code>temperature</code> <code>Optional[float]</code> <p>Temperature value for sampling. Defaults to 1.0.</p> <code>1.0</code> <code>top_k</code> <code>Optional[int]</code> <p>Value of k for top-k sampling. Defaults to 50.</p> <code>50</code> <code>top_p</code> <code>Optional[float]</code> <p>Value of p for top-p sampling. Defaults to 1.0.</p> <code>1.0</code> <p>Returns:</p> Name Type Description <code>GenericOutputs</code> <p>Generated caption sequences and their scores.</p> Source code in <code>src/unitorch/models/blip/modeling.py</code> <pre><code>@torch.no_grad()\ndef generate(\n    self,\n    pixel_values: torch.Tensor,\n    input_ids: Optional[torch.Tensor] = None,\n    attention_mask: Optional[torch.Tensor] = None,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 101,\n    decoder_end_token_id: Optional[int] = 102,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n):\n\"\"\"\n    Generates captions for the given input images.\n\n    Args:\n        pixel_values (torch.Tensor): Input pixel values.\n        input_ids (Optional[torch.Tensor], optional): Input token IDs. Defaults to None.\n        attention_mask (Optional[torch.Tensor], optional): Attention mask. Defaults to None.\n        num_beams (Optional[int], optional): Number of beams for beam search. Defaults to 5.\n        decoder_start_token_id (Optional[int], optional): ID of the start token for decoding. Defaults to 30522.\n        decoder_end_token_id (Optional[int], optional): ID of the end token for decoding. Defaults to 2.\n        num_return_sequences (Optional[int], optional): Number of caption sequences to return. Defaults to 1.\n        min_gen_seq_length (Optional[int], optional): Minimum length of generated sequences. Defaults to 0.\n        max_gen_seq_length (Optional[int], optional): Maximum length of generated sequences. Defaults to 48.\n        repetition_penalty (Optional[float], optional): Repetition penalty value. Defaults to 1.0.\n        no_repeat_ngram_size (Optional[int], optional): Size of n-grams to avoid repetition. Defaults to 0.\n        early_stopping (Optional[bool], optional): Whether to stop generation early. Defaults to True.\n        length_penalty (Optional[float], optional): Length penalty value. Defaults to 1.0.\n        num_beam_groups (Optional[int], optional): Number of groups for diverse beam search. Defaults to 1.\n        diversity_penalty (Optional[float], optional): Diversity penalty value. Defaults to 0.0.\n        do_sample (Optional[bool], optional): Whether to use sampling for generation. Defaults to False.\n        temperature (Optional[float], optional): Temperature value for sampling. Defaults to 1.0.\n        top_k (Optional[int], optional): Value of k for top-k sampling. Defaults to 50.\n        top_p (Optional[float], optional): Value of p for top-p sampling. Defaults to 1.0.\n\n    Returns:\n        GenericOutputs: Generated caption sequences and their scores.\n    \"\"\"\n    outputs = self.model.generate(\n        pixel_values=pixel_values,\n        input_ids=input_ids,\n        attention_mask=attention_mask,\n        max_length=max_gen_seq_length,\n        min_length=min_gen_seq_length,\n        num_beams=num_beams,\n        do_sample=do_sample,\n        decoder_start_token_id=decoder_start_token_id,\n        no_repeat_ngram_size=no_repeat_ngram_size,\n        early_stopping=early_stopping,\n        length_penalty=length_penalty,\n        repetition_penalty=repetition_penalty,\n        num_return_sequences=num_return_sequences,\n        bos_token_id=decoder_start_token_id,\n        num_beam_groups=num_beam_groups,\n        diversity_penalty=diversity_penalty,\n        temperature=temperature,\n        top_k=top_k,\n        top_p=top_p,\n        return_dict_in_generate=True,\n        output_scores=True,\n    )\n\n    sequences = outputs.sequences.reshape(\n        -1, num_return_sequences, outputs.sequences.size(-1)\n    )\n    outputs.sequences = torch.zeros(\n        sequences.size(0), num_return_sequences, max_gen_seq_length\n    ).to(device=sequences.device)\n    outputs.sequences[:, :, : sequences.size(-1)].copy_(sequences)\n\n    if num_return_sequences == 1:\n        outputs.sequences = outputs.sequences.reshape(-1, max_gen_seq_length)\n\n    return GenericOutputs(\n        sequences=outputs.sequences, sequences_scores=outputs.sequences_scores\n    )\n</code></pre>",
+            "text": "<pre><code>generate(\n    pixel_values: torch.Tensor,\n    input_ids: Optional[torch.Tensor] = None,\n    attention_mask: Optional[torch.Tensor] = None,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 101,\n    decoder_end_token_id: Optional[\n        Union[int, List[int]]\n    ] = 102,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n)\n</code></pre> <p>Generates captions for the given input images.</p> <p>Parameters:</p> Name Type Description Default <code>pixel_values</code> <code>torch.Tensor</code> <p>Input pixel values.</p> required <code>input_ids</code> <code>Optional[torch.Tensor]</code> <p>Input token IDs. Defaults to None.</p> <code>None</code> <code>attention_mask</code> <code>Optional[torch.Tensor]</code> <p>Attention mask. Defaults to None.</p> <code>None</code> <code>num_beams</code> <code>Optional[int]</code> <p>Number of beams for beam search. Defaults to 5.</p> <code>5</code> <code>decoder_start_token_id</code> <code>Optional[int]</code> <p>ID of the start token for decoding. Defaults to 30522.</p> <code>101</code> <code>decoder_end_token_id</code> <code>int or List[int]</code> <p>ID of the end token for decoding. Defaults to 2.</p> <code>102</code> <code>num_return_sequences</code> <code>Optional[int]</code> <p>Number of caption sequences to return. Defaults to 1.</p> <code>1</code> <code>min_gen_seq_length</code> <code>Optional[int]</code> <p>Minimum length of generated sequences. Defaults to 0.</p> <code>0</code> <code>max_gen_seq_length</code> <code>Optional[int]</code> <p>Maximum length of generated sequences. Defaults to 48.</p> <code>48</code> <code>repetition_penalty</code> <code>Optional[float]</code> <p>Repetition penalty value. Defaults to 1.0.</p> <code>1.0</code> <code>no_repeat_ngram_size</code> <code>Optional[int]</code> <p>Size of n-grams to avoid repetition. Defaults to 0.</p> <code>0</code> <code>early_stopping</code> <code>Optional[bool]</code> <p>Whether to stop generation early. Defaults to True.</p> <code>True</code> <code>length_penalty</code> <code>Optional[float]</code> <p>Length penalty value. Defaults to 1.0.</p> <code>1.0</code> <code>num_beam_groups</code> <code>Optional[int]</code> <p>Number of groups for diverse beam search. Defaults to 1.</p> <code>1</code> <code>diversity_penalty</code> <code>Optional[float]</code> <p>Diversity penalty value. Defaults to 0.0.</p> <code>0.0</code> <code>do_sample</code> <code>Optional[bool]</code> <p>Whether to use sampling for generation. Defaults to False.</p> <code>False</code> <code>temperature</code> <code>Optional[float]</code> <p>Temperature value for sampling. Defaults to 1.0.</p> <code>1.0</code> <code>top_k</code> <code>Optional[int]</code> <p>Value of k for top-k sampling. Defaults to 50.</p> <code>50</code> <code>top_p</code> <code>Optional[float]</code> <p>Value of p for top-p sampling. Defaults to 1.0.</p> <code>1.0</code> <p>Returns:</p> Name Type Description <code>GenericOutputs</code> <p>Generated caption sequences and their scores.</p> Source code in <code>src/unitorch/models/blip/modeling.py</code> <pre><code>@torch.no_grad()\ndef generate(\n    self,\n    pixel_values: torch.Tensor,\n    input_ids: Optional[torch.Tensor] = None,\n    attention_mask: Optional[torch.Tensor] = None,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 101,\n    decoder_end_token_id: Optional[Union[int, List[int]]] = 102,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n):\n\"\"\"\n    Generates captions for the given input images.\n\n    Args:\n        pixel_values (torch.Tensor): Input pixel values.\n        input_ids (Optional[torch.Tensor], optional): Input token IDs. Defaults to None.\n        attention_mask (Optional[torch.Tensor], optional): Attention mask. Defaults to None.\n        num_beams (Optional[int], optional): Number of beams for beam search. Defaults to 5.\n        decoder_start_token_id (Optional[int], optional): ID of the start token for decoding. Defaults to 30522.\n        decoder_end_token_id (int or List[int], optional): ID of the end token for decoding. Defaults to 2.\n        num_return_sequences (Optional[int], optional): Number of caption sequences to return. Defaults to 1.\n        min_gen_seq_length (Optional[int], optional): Minimum length of generated sequences. Defaults to 0.\n        max_gen_seq_length (Optional[int], optional): Maximum length of generated sequences. Defaults to 48.\n        repetition_penalty (Optional[float], optional): Repetition penalty value. Defaults to 1.0.\n        no_repeat_ngram_size (Optional[int], optional): Size of n-grams to avoid repetition. Defaults to 0.\n        early_stopping (Optional[bool], optional): Whether to stop generation early. Defaults to True.\n        length_penalty (Optional[float], optional): Length penalty value. Defaults to 1.0.\n        num_beam_groups (Optional[int], optional): Number of groups for diverse beam search. Defaults to 1.\n        diversity_penalty (Optional[float], optional): Diversity penalty value. Defaults to 0.0.\n        do_sample (Optional[bool], optional): Whether to use sampling for generation. Defaults to False.\n        temperature (Optional[float], optional): Temperature value for sampling. Defaults to 1.0.\n        top_k (Optional[int], optional): Value of k for top-k sampling. Defaults to 50.\n        top_p (Optional[float], optional): Value of p for top-p sampling. Defaults to 1.0.\n\n    Returns:\n        GenericOutputs: Generated caption sequences and their scores.\n    \"\"\"\n    outputs = self.model.generate(\n        pixel_values=pixel_values,\n        input_ids=input_ids,\n        attention_mask=attention_mask,\n        max_length=max_gen_seq_length,\n        min_length=min_gen_seq_length,\n        num_beams=num_beams,\n        do_sample=do_sample,\n        decoder_start_token_id=decoder_start_token_id,\n        no_repeat_ngram_size=no_repeat_ngram_size,\n        early_stopping=early_stopping,\n        length_penalty=length_penalty,\n        repetition_penalty=repetition_penalty,\n        num_return_sequences=num_return_sequences,\n        bos_token_id=decoder_start_token_id,\n        num_beam_groups=num_beam_groups,\n        diversity_penalty=diversity_penalty,\n        temperature=temperature,\n        top_k=top_k,\n        top_p=top_p,\n        return_dict_in_generate=True,\n        output_scores=True,\n    )\n\n    sequences = outputs.sequences.reshape(\n        -1, num_return_sequences, outputs.sequences.size(-1)\n    )\n    outputs.sequences = torch.zeros(\n        sequences.size(0), num_return_sequences, max_gen_seq_length\n    ).to(device=sequences.device)\n    outputs.sequences[:, :, : sequences.size(-1)].copy_(sequences)\n\n    if num_return_sequences == 1:\n        outputs.sequences = outputs.sequences.reshape(-1, max_gen_seq_length)\n\n    return GenericOutputs(\n        sequences=outputs.sequences, sequences_scores=outputs.sequences_scores\n    )\n</code></pre>",
             "title": "generate"
         },
         {
             "location": "models/bloom/",
             "text": "",
             "title": "unitorch.models.bloom"
         },
@@ -1892,15 +1927,15 @@
         {
             "location": "models/bloom/#unitorch.models.bloom.processing.BloomProcessor.classification",
             "text": "<pre><code>classification(\n    text: str,\n    text_pair: Optional[str] = None,\n    max_seq_length: Optional[int] = None,\n) -&gt; GenericOutputs\n</code></pre> <p>Preprocesses text for classification.</p> <p>Parameters:</p> Name Type Description Default <code>text</code> <code>str</code> <p>The input text to classify.</p> required <code>text_pair</code> <code>Optional[str]</code> <p>The second input text for sequence classification. Defaults to None.</p> <code>None</code> <code>max_seq_length</code> <code>Optional[int]</code> <p>The maximum sequence length. Defaults to None.</p> <code>None</code> <p>Returns:</p> Name Type Description <code>GenericOutputs</code> <code>GenericOutputs</code> <p>The processed input IDs and attention mask tensors.</p> Source code in <code>src/unitorch/models/bloom/processing.py</code> <pre><code>def classification(\n    self,\n    text: str,\n    text_pair: Optional[str] = None,\n    max_seq_length: Optional[int] = None,\n) -&gt; GenericOutputs:\n\"\"\"\n    Preprocesses text for classification.\n\n    Args:\n        text (str): The input text to classify.\n        text_pair (Optional[str]): The second input text for sequence classification. Defaults to None.\n        max_seq_length (Optional[int]): The maximum sequence length. Defaults to None.\n\n    Returns:\n        GenericOutputs: The processed input IDs and attention mask tensors.\n    \"\"\"\n    max_seq_length = pop_value(\n        max_seq_length,\n        self.max_seq_length,\n    )\n\n    tokens = self.tokenizer.tokenize(str(text))\n    if text_pair is None:\n        tokens = tokens[:max_seq_length]\n        input_ids = self.tokenizer.convert_tokens_to_ids(tokens)\n    else:\n        tokens_pair = self.tokenizer.tokenize(str(text_pair))\n        truncate_sequence_pair(tokens, tokens_pair, max_seq_length)\n        tokens = tokens + tokens_pair\n        input_ids = self.tokenizer.convert_tokens_to_ids(tokens)\n\n    padding = [0] * (max_seq_length - len(input_ids))\n    attention_mask = [0] * len(padding) + [1] * len(input_ids)\n    input_ids = len(padding) * [self.pad_token_id] + input_ids\n\n    assert len(input_ids) == max_seq_length\n    assert len(attention_mask) == max_seq_length\n    return GenericOutputs(\n        input_ids=torch.tensor(input_ids, dtype=torch.long),\n        attention_mask=torch.tensor(attention_mask, dtype=torch.long),\n    )\n</code></pre>",
             "title": "classification"
         },
         {
             "location": "models/bloom/#unitorch.models.bloom.processing.BloomProcessor.generation",
-            "text": "<pre><code>generation(\n    text: str,\n    text_pair: str,\n    max_seq_length: Optional[int] = None,\n    max_gen_seq_length: Optional[int] = None,\n) -&gt; GenericOutputs\n</code></pre> <p>Preprocesses text for generation.</p> <p>Parameters:</p> Name Type Description Default <code>text</code> <code>str</code> <p>The input text for generation.</p> required <code>text_pair</code> <code>str</code> <p>The second input text for generation.</p> required <code>max_seq_length</code> <code>Optional[int]</code> <p>The maximum sequence length for classification. Defaults to None.</p> <code>None</code> <code>max_gen_seq_length</code> <code>Optional[int]</code> <p>The maximum generation sequence length. Defaults to None.</p> <code>None</code> <p>Returns:</p> Name Type Description <code>GenericOutputs</code> <code>GenericOutputs</code> <p>The processed input IDs and attention mask tensors.</p> Source code in <code>src/unitorch/models/bloom/processing.py</code> <pre><code>def generation(\n    self,\n    text: str,\n    text_pair: str,\n    max_seq_length: Optional[int] = None,\n    max_gen_seq_length: Optional[int] = None,\n) -&gt; GenericOutputs:\n\"\"\"\n    Preprocesses text for generation.\n\n    Args:\n        text (str): The input text for generation.\n        text_pair (str): The second input text for generation.\n        max_seq_length (Optional[int]): The maximum sequence length for classification. Defaults to None.\n        max_gen_seq_length (Optional[int]): The maximum generation sequence length. Defaults to None.\n\n    Returns:\n        GenericOutputs: The processed input IDs and attention mask tensors.\n    \"\"\"\n    max_seq_length = pop_value(\n        max_seq_length,\n        self.max_seq_length,\n    )\n    max_gen_seq_length = pop_value(\n        max_gen_seq_length,\n        self.max_gen_seq_length,\n    )\n\n    tokens = self.tokenizer.tokenize(str(text))[-max_seq_length:]\n    tokens_pair = self.tokenizer.tokenize(str(text_pair))[\n        : max_gen_seq_length - 1\n    ] + [self.eos_token]\n    padding_a = [self.pad_token] * (max_seq_length - len(tokens))\n    padding_b = [self.pad_token] * (max_gen_seq_length - len(tokens_pair))\n    attention_mask = (\n        [0] * len(padding_a)\n        + [1] * (len(tokens) + len(tokens_pair))\n        + [0] * len(padding_b)\n    )\n    _tokens = padding_a + tokens + tokens_pair + padding_b\n    input_ids = self.tokenizer.convert_tokens_to_ids(_tokens)\n\n    tokens_label = tokens_pair[1:max_gen_seq_length] + [self.pad_token] * (\n        max_gen_seq_length - len(tokens_pair) + 1\n    )\n    input_ids_label = self.tokenizer.convert_tokens_to_ids(tokens_label)\n    input_ids_label = [0] * max_seq_length + input_ids_label\n    attention_mask_label = [1] * len(tokens_pair[1:max_gen_seq_length]) + [0] * (\n        max_gen_seq_length - len(tokens_pair) + 1\n    )\n    attention_mask_label = [0] * max_seq_length + attention_mask_label\n\n    return GenericOutputs(\n        input_ids=torch.tensor(input_ids, dtype=torch.long),\n        attention_mask=torch.tensor(attention_mask, dtype=torch.long),\n        input_ids_label=torch.tensor(input_ids_label, dtype=torch.long),\n        attention_mask_label=torch.tensor(attention_mask_label, dtype=torch.long),\n    )\n</code></pre>",
+            "text": "<pre><code>generation(\n    text: str,\n    text_pair: str,\n    max_seq_length: Optional[int] = None,\n    max_gen_seq_length: Optional[int] = None,\n) -&gt; GenericOutputs\n</code></pre> <p>Preprocesses text for generation.</p> <p>Parameters:</p> Name Type Description Default <code>text</code> <code>str</code> <p>The input text for generation.</p> required <code>text_pair</code> <code>str</code> <p>The second input text for generation.</p> required <code>max_seq_length</code> <code>Optional[int]</code> <p>The maximum sequence length for classification. Defaults to None.</p> <code>None</code> <code>max_gen_seq_length</code> <code>Optional[int]</code> <p>The maximum generation sequence length. Defaults to None.</p> <code>None</code> <p>Returns:</p> Name Type Description <code>GenericOutputs</code> <code>GenericOutputs</code> <p>The processed input IDs and attention mask tensors.</p> Source code in <code>src/unitorch/models/bloom/processing.py</code> <pre><code>def generation(\n    self,\n    text: str,\n    text_pair: str,\n    max_seq_length: Optional[int] = None,\n    max_gen_seq_length: Optional[int] = None,\n) -&gt; GenericOutputs:\n\"\"\"\n    Preprocesses text for generation.\n\n    Args:\n        text (str): The input text for generation.\n        text_pair (str): The second input text for generation.\n        max_seq_length (Optional[int]): The maximum sequence length for classification. Defaults to None.\n        max_gen_seq_length (Optional[int]): The maximum generation sequence length. Defaults to None.\n\n    Returns:\n        GenericOutputs: The processed input IDs and attention mask tensors.\n    \"\"\"\n    max_seq_length = pop_value(\n        max_seq_length,\n        self.max_seq_length,\n    )\n    max_gen_seq_length = pop_value(\n        max_gen_seq_length,\n        self.max_gen_seq_length,\n    )\n\n    tokens = self.tokenizer.tokenize(str(text))[-max_seq_length:]\n    tokens_pair = self.tokenizer.tokenize(str(text_pair))[\n        : max_gen_seq_length - 1\n    ] + [self.eos_token]\n    padding_a = [self.pad_token] * (max_seq_length - len(tokens))\n    padding_b = [self.pad_token] * (max_gen_seq_length - len(tokens_pair))\n    attention_mask = (\n        [0] * len(padding_a)\n        + [1] * (len(tokens) + len(tokens_pair))\n        + [0] * len(padding_b)\n    )\n    _tokens = padding_a + tokens + tokens_pair + padding_b\n    input_ids = self.tokenizer.convert_tokens_to_ids(_tokens)\n\n    tokens_label = tokens_pair + [self.pad_token] * (\n        max_gen_seq_length - len(tokens_pair) + 1\n    )\n    input_ids_label = self.tokenizer.convert_tokens_to_ids(tokens_label)\n    input_ids_label = [0] * (max_seq_length - 1) + input_ids_label\n    attention_mask_label = [1] * len(tokens_pair) + [0] * (\n        max_gen_seq_length - len(tokens_pair) + 1\n    )\n    attention_mask_label = [0] * (max_seq_length - 1) + attention_mask_label\n\n    return GenericOutputs(\n        input_ids=torch.tensor(input_ids, dtype=torch.long),\n        attention_mask=torch.tensor(attention_mask, dtype=torch.long),\n        input_ids_label=torch.tensor(input_ids_label, dtype=torch.long),\n        attention_mask_label=torch.tensor(attention_mask_label, dtype=torch.long),\n    )\n</code></pre>",
             "title": "generation"
         },
         {
             "location": "models/bloom/#unitorch.models.bloom.processing.BloomProcessor.generation_inputs",
             "text": "<pre><code>generation_inputs(\n    text: str, max_seq_length: Optional[int] = None\n) -&gt; GenericOutputs\n</code></pre> <p>Preprocesses text as generation inputs.</p> <p>Parameters:</p> Name Type Description Default <code>text</code> <code>str</code> <p>The input text for generation.</p> required <code>max_seq_length</code> <code>Optional[int]</code> <p>The maximum sequence length. Defaults to None.</p> <code>None</code> <p>Returns:</p> Name Type Description <code>GenericOutputs</code> <code>GenericOutputs</code> <p>The processed input IDs tensor.</p> Source code in <code>src/unitorch/models/bloom/processing.py</code> <pre><code>def generation_inputs(\n    self,\n    text: str,\n    max_seq_length: Optional[int] = None,\n) -&gt; GenericOutputs:\n\"\"\"\n    Preprocesses text as generation inputs.\n\n    Args:\n        text (str): The input text for generation.\n        max_seq_length (Optional[int]): The maximum sequence length. Defaults to None.\n\n    Returns:\n        GenericOutputs: The processed input IDs tensor.\n    \"\"\"\n    max_seq_length = pop_value(\n        max_seq_length,\n        self.max_seq_length,\n    )\n    tokens = self.tokenizer.tokenize(str(text))[-max_seq_length:]\n    padding = [self.pad_token] * (max_seq_length - len(tokens))\n    tokens = padding + tokens\n    input_ids = self.tokenizer.convert_tokens_to_ids(tokens)\n\n    assert len(input_ids) == max_seq_length\n    return GenericOutputs(\n        input_ids=torch.tensor(input_ids, dtype=torch.long),\n    )\n</code></pre>",
             "title": "generation_inputs"
         },
@@ -1942,15 +1977,15 @@
         {
             "location": "models/bloom/#unitorch.models.bloom.modeling.BloomForGeneration.forward",
             "text": "<pre><code>forward(\n    input_ids: torch.Tensor,\n    attention_mask: Optional[torch.Tensor] = None,\n) -&gt; torch.Tensor\n</code></pre> <p>Forward pass of the BloomForGeneration model.</p> <p>Parameters:</p> Name Type Description Default <code>input_ids</code> <code>torch.Tensor</code> <p>The input token IDs.</p> required <code>attention_mask</code> <code>Optional[torch.Tensor]</code> <p>The attention mask tensor. Defaults to None.</p> <code>None</code> <p>Returns:</p> Type Description <code>torch.Tensor</code> <p>The output logits.</p> Source code in <code>src/unitorch/models/bloom/modeling.py</code> <pre><code>def forward(\n    self,\n    input_ids: torch.Tensor,\n    attention_mask: Optional[torch.Tensor] = None,\n) -&gt; torch.Tensor:\n\"\"\"\n    Forward pass of the BloomForGeneration model.\n\n    Args:\n        input_ids (torch.Tensor): The input token IDs.\n        attention_mask (Optional[torch.Tensor]): The attention mask tensor. Defaults to None.\n\n    Returns:\n        (torch.Tensor):The output logits.\n    \"\"\"\n    outputs = self.model(\n        input_ids,\n        attention_mask=attention_mask,\n        return_dict=True,\n    )\n    logits = outputs.logits\n    return logits\n</code></pre>",
             "title": "forward"
         },
         {
             "location": "models/bloom/#unitorch.models.bloom.modeling.BloomForGeneration.generate",
-            "text": "<pre><code>generate(\n    input_ids: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 1,\n    decoder_end_token_id: Optional[int] = 2,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n) -&gt; GenericOutputs\n</code></pre> <p>Generate sequences using the BloomForGeneration model.</p> <p>Parameters:</p> Name Type Description Default <code>input_ids</code> <code>torch.Tensor</code> <p>The input token IDs.</p> required <code>num_beams</code> <code>Optional[int]</code> <p>The number of beams for beam search. Defaults to 5.</p> <code>5</code> <code>decoder_start_token_id</code> <code>Optional[int]</code> <p>The ID of the start token for decoding. Defaults to 1.</p> <code>1</code> <code>decoder_end_token_id</code> <code>Optional[int]</code> <p>The ID of the end token for decoding. Defaults to 2.</p> <code>2</code> <code>num_return_sequences</code> <code>Optional[int]</code> <p>The number of generated sequences to return. Defaults to 1.</p> <code>1</code> <code>min_gen_seq_length</code> <code>Optional[int]</code> <p>The minimum length of the generated sequences. Defaults to 0.</p> <code>0</code> <code>max_gen_seq_length</code> <code>Optional[int]</code> <p>The maximum length of the generated sequences. Defaults to 48.</p> <code>48</code> <code>repetition_penalty</code> <code>Optional[float]</code> <p>The penalty for repeated n-grams. Defaults to 1.0.</p> <code>1.0</code> <code>no_repeat_ngram_size</code> <code>Optional[int]</code> <p>The size of n-grams to prevent repetition. Defaults to 0.</p> <code>0</code> <code>early_stopping</code> <code>Optional[bool]</code> <p>Whether to stop generation early based on specified conditions. Defaults to True.</p> <code>True</code> <code>length_penalty</code> <code>Optional[float]</code> <p>The penalty for longer sequences. Defaults to 1.0.</p> <code>1.0</code> <code>num_beam_groups</code> <code>Optional[int]</code> <p>The number of beam groups for diverse beam search. Defaults to 1.</p> <code>1</code> <code>diversity_penalty</code> <code>Optional[float]</code> <p>The penalty for diverse beam search. Defaults to 0.0.</p> <code>0.0</code> <code>do_sample</code> <code>Optional[bool]</code> <p>Whether to use sampling for generation. Defaults to False.</p> <code>False</code> <code>temperature</code> <code>Optional[float]</code> <p>The temperature for sampling. Defaults to 1.0.</p> <code>1.0</code> <code>top_k</code> <code>Optional[int]</code> <p>The number of top-k tokens to consider for sampling. Defaults to 50.</p> <code>50</code> <code>top_p</code> <code>Optional[float]</code> <p>The cumulative probability for top-p sampling. Defaults to 1.0.</p> <code>1.0</code> <p>Returns:</p> Name Type Description <code>GenericOutputs</code> <code>GenericOutputs</code> <p>The generated sequences and their scores.</p> Source code in <code>src/unitorch/models/bloom/modeling.py</code> <pre><code>@torch.no_grad()\ndef generate(\n    self,\n    input_ids: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 1,\n    decoder_end_token_id: Optional[int] = 2,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n) -&gt; GenericOutputs:\n\"\"\"\n    Generate sequences using the BloomForGeneration model.\n\n    Args:\n        input_ids (torch.Tensor): The input token IDs.\n        num_beams (Optional[int]): The number of beams for beam search. Defaults to 5.\n        decoder_start_token_id (Optional[int]): The ID of the start token for decoding. Defaults to 1.\n        decoder_end_token_id (Optional[int]): The ID of the end token for decoding. Defaults to 2.\n        num_return_sequences (Optional[int]): The number of generated sequences to return. Defaults to 1.\n        min_gen_seq_length (Optional[int]): The minimum length of the generated sequences. Defaults to 0.\n        max_gen_seq_length (Optional[int]): The maximum length of the generated sequences. Defaults to 48.\n        repetition_penalty (Optional[float]): The penalty for repeated n-grams. Defaults to 1.0.\n        no_repeat_ngram_size (Optional[int]): The size of n-grams to prevent repetition. Defaults to 0.\n        early_stopping (Optional[bool]): Whether to stop generation early based on specified conditions. Defaults to True.\n        length_penalty (Optional[float]): The penalty for longer sequences. Defaults to 1.0.\n        num_beam_groups (Optional[int]): The number of beam groups for diverse beam search. Defaults to 1.\n        diversity_penalty (Optional[float]): The penalty for diverse beam search. Defaults to 0.0.\n        do_sample (Optional[bool]): Whether to use sampling for generation. Defaults to False.\n        temperature (Optional[float]): The temperature for sampling. Defaults to 1.0.\n        top_k (Optional[int]): The number of top-k tokens to consider for sampling. Defaults to 50.\n        top_p (Optional[float]): The cumulative probability for top-p sampling. Defaults to 1.0.\n\n    Returns:\n        GenericOutputs: The generated sequences and their scores.\n    \"\"\"\n    input_seq_length = input_ids.size(1)\n    outputs = self.model.generate(\n        input_ids,\n        max_length=max_gen_seq_length + input_seq_length,\n        min_length=min_gen_seq_length + input_seq_length,\n        num_beams=num_beams,\n        do_sample=do_sample,\n        decoder_start_token_id=decoder_start_token_id,\n        no_repeat_ngram_size=no_repeat_ngram_size,\n        early_stopping=early_stopping,\n        length_penalty=length_penalty,\n        repetition_penalty=repetition_penalty,\n        num_return_sequences=num_return_sequences,\n        bos_token_id=decoder_start_token_id,\n        eos_token_id=decoder_end_token_id,\n        num_beam_groups=num_beam_groups,\n        diversity_penalty=diversity_penalty,\n        temperature=temperature,\n        top_k=top_k,\n        top_p=top_p,\n        return_dict_in_generate=True,\n        output_scores=True,\n    )\n    sequences = outputs.sequences.reshape(\n        -1, num_return_sequences, outputs.sequences.size(-1)\n    )\n    outputs.sequences = torch.zeros(\n        sequences.size(0), num_return_sequences, max_gen_seq_length\n    ).to(device=sequences.device)\n    outputs.sequences[:, :, : sequences.size(-1) - input_seq_length].copy_(\n        sequences[:, :, input_seq_length : sequences.size(-1)]\n    )\n\n    if num_return_sequences == 1:\n        outputs.sequences = outputs.sequences.reshape(-1, max_gen_seq_length)\n\n    return GenericOutputs(\n        sequences=outputs.sequences.long(),\n        sequences_scores=outputs.sequences_scores,\n    )\n</code></pre>",
+            "text": "<pre><code>generate(\n    input_ids: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 1,\n    decoder_end_token_id: Optional[\n        Union[int, List[int]]\n    ] = 2,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n) -&gt; GenericOutputs\n</code></pre> <p>Generate sequences using the BloomForGeneration model.</p> <p>Parameters:</p> Name Type Description Default <code>input_ids</code> <code>torch.Tensor</code> <p>The input token IDs.</p> required <code>num_beams</code> <code>Optional[int]</code> <p>The number of beams for beam search. Defaults to 5.</p> <code>5</code> <code>decoder_start_token_id</code> <code>Optional[int]</code> <p>The ID of the start token for decoding. Defaults to 1.</p> <code>1</code> <code>decoder_end_token_id</code> <code>Optional[int]</code> <p>The ID of the end token for decoding. Defaults to 2.</p> <code>2</code> <code>num_return_sequences</code> <code>Optional[int]</code> <p>The number of generated sequences to return. Defaults to 1.</p> <code>1</code> <code>min_gen_seq_length</code> <code>Optional[int]</code> <p>The minimum length of the generated sequences. Defaults to 0.</p> <code>0</code> <code>max_gen_seq_length</code> <code>Optional[int]</code> <p>The maximum length of the generated sequences. Defaults to 48.</p> <code>48</code> <code>repetition_penalty</code> <code>Optional[float]</code> <p>The penalty for repeated n-grams. Defaults to 1.0.</p> <code>1.0</code> <code>no_repeat_ngram_size</code> <code>Optional[int]</code> <p>The size of n-grams to prevent repetition. Defaults to 0.</p> <code>0</code> <code>early_stopping</code> <code>Optional[bool]</code> <p>Whether to stop generation early based on specified conditions. Defaults to True.</p> <code>True</code> <code>length_penalty</code> <code>Optional[float]</code> <p>The penalty for longer sequences. Defaults to 1.0.</p> <code>1.0</code> <code>num_beam_groups</code> <code>Optional[int]</code> <p>The number of beam groups for diverse beam search. Defaults to 1.</p> <code>1</code> <code>diversity_penalty</code> <code>Optional[float]</code> <p>The penalty for diverse beam search. Defaults to 0.0.</p> <code>0.0</code> <code>do_sample</code> <code>Optional[bool]</code> <p>Whether to use sampling for generation. Defaults to False.</p> <code>False</code> <code>temperature</code> <code>Optional[float]</code> <p>The temperature for sampling. Defaults to 1.0.</p> <code>1.0</code> <code>top_k</code> <code>Optional[int]</code> <p>The number of top-k tokens to consider for sampling. Defaults to 50.</p> <code>50</code> <code>top_p</code> <code>Optional[float]</code> <p>The cumulative probability for top-p sampling. Defaults to 1.0.</p> <code>1.0</code> <p>Returns:</p> Name Type Description <code>GenericOutputs</code> <code>GenericOutputs</code> <p>The generated sequences and their scores.</p> Source code in <code>src/unitorch/models/bloom/modeling.py</code> <pre><code>@torch.no_grad()\ndef generate(\n    self,\n    input_ids: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 1,\n    decoder_end_token_id: Optional[Union[int, List[int]]] = 2,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n) -&gt; GenericOutputs:\n\"\"\"\n    Generate sequences using the BloomForGeneration model.\n\n    Args:\n        input_ids (torch.Tensor): The input token IDs.\n        num_beams (Optional[int]): The number of beams for beam search. Defaults to 5.\n        decoder_start_token_id (Optional[int]): The ID of the start token for decoding. Defaults to 1.\n        decoder_end_token_id (Optional[int]): The ID of the end token for decoding. Defaults to 2.\n        num_return_sequences (Optional[int]): The number of generated sequences to return. Defaults to 1.\n        min_gen_seq_length (Optional[int]): The minimum length of the generated sequences. Defaults to 0.\n        max_gen_seq_length (Optional[int]): The maximum length of the generated sequences. Defaults to 48.\n        repetition_penalty (Optional[float]): The penalty for repeated n-grams. Defaults to 1.0.\n        no_repeat_ngram_size (Optional[int]): The size of n-grams to prevent repetition. Defaults to 0.\n        early_stopping (Optional[bool]): Whether to stop generation early based on specified conditions. Defaults to True.\n        length_penalty (Optional[float]): The penalty for longer sequences. Defaults to 1.0.\n        num_beam_groups (Optional[int]): The number of beam groups for diverse beam search. Defaults to 1.\n        diversity_penalty (Optional[float]): The penalty for diverse beam search. Defaults to 0.0.\n        do_sample (Optional[bool]): Whether to use sampling for generation. Defaults to False.\n        temperature (Optional[float]): The temperature for sampling. Defaults to 1.0.\n        top_k (Optional[int]): The number of top-k tokens to consider for sampling. Defaults to 50.\n        top_p (Optional[float]): The cumulative probability for top-p sampling. Defaults to 1.0.\n\n    Returns:\n        GenericOutputs: The generated sequences and their scores.\n    \"\"\"\n    input_seq_length = input_ids.size(1)\n    outputs = self.model.generate(\n        input_ids,\n        max_length=max_gen_seq_length + input_seq_length,\n        min_length=min_gen_seq_length + input_seq_length,\n        num_beams=num_beams,\n        do_sample=do_sample,\n        decoder_start_token_id=decoder_start_token_id,\n        no_repeat_ngram_size=no_repeat_ngram_size,\n        early_stopping=early_stopping,\n        length_penalty=length_penalty,\n        repetition_penalty=repetition_penalty,\n        num_return_sequences=num_return_sequences,\n        bos_token_id=decoder_start_token_id,\n        eos_token_id=decoder_end_token_id,\n        num_beam_groups=num_beam_groups,\n        diversity_penalty=diversity_penalty,\n        temperature=temperature,\n        top_k=top_k,\n        top_p=top_p,\n        return_dict_in_generate=True,\n        output_scores=True,\n    )\n    sequences = outputs.sequences.reshape(\n        -1, num_return_sequences, outputs.sequences.size(-1)\n    )\n    outputs.sequences = torch.zeros(\n        sequences.size(0), num_return_sequences, max_gen_seq_length\n    ).to(device=sequences.device)\n    outputs.sequences[:, :, : sequences.size(-1) - input_seq_length].copy_(\n        sequences[:, :, input_seq_length : sequences.size(-1)]\n    )\n\n    if num_return_sequences == 1:\n        outputs.sequences = outputs.sequences.reshape(-1, max_gen_seq_length)\n\n    return GenericOutputs(\n        sequences=outputs.sequences.long(),\n        sequences_scores=outputs.sequences_scores,\n    )\n</code></pre>",
             "title": "generate"
         },
         {
             "location": "models/chatglm/",
             "text": "",
             "title": "unitorch.models.chatglm"
         },
@@ -2012,15 +2047,15 @@
         {
             "location": "models/chatglm/#unitorch.models.chatglm.modeling.ChatGLMForGeneration.forward",
             "text": "<pre><code>forward(\n    input_ids: Optional[torch.Tensor],\n    attention_mask: Optional[torch.Tensor],\n    position_ids: Optional[torch.Tensor],\n) -&gt; torch.Tensor\n</code></pre> <p>Performs forward pass of the ChatGLMForGeneration model.</p> <p>Parameters:</p> Name Type Description Default <code>input_ids</code> <code>Optional[torch.Tensor]</code> <p>Tensor of input token IDs.</p> required <code>attention_mask</code> <code>Optional[torch.Tensor]</code> <p>Tensor of attention mask.</p> required <code>position_ids</code> <code>Optional[torch.Tensor]</code> <p>Tensor of position IDs.</p> required <p>Returns:</p> Type Description <code>torch.Tensor</code> <p>Tensor of logits.</p> Source code in <code>src/unitorch/models/chatglm/modeling.py</code> <pre><code>def forward(\n    self,\n    input_ids: Optional[torch.Tensor],\n    attention_mask: Optional[torch.Tensor],\n    position_ids: Optional[torch.Tensor],\n) -&gt; torch.Tensor:\n\"\"\"\n    Performs forward pass of the ChatGLMForGeneration model.\n\n    Args:\n        input_ids (Optional[torch.Tensor]): Tensor of input token IDs.\n        attention_mask (Optional[torch.Tensor]): Tensor of attention mask.\n        position_ids (Optional[torch.Tensor]): Tensor of position IDs.\n\n    Returns:\n        (torch.Tensor):Tensor of logits.\n    \"\"\"\n    outputs = self.model(\n        input_ids=input_ids,\n        attention_mask=attention_mask,\n        position_ids=position_ids,\n        return_dict=True,\n    )\n    logits = outputs.logits\n    return logits\n</code></pre>",
             "title": "forward"
         },
         {
             "location": "models/chatglm/#unitorch.models.chatglm.modeling.ChatGLMForGeneration.generate",
-            "text": "<pre><code>generate(\n    input_ids: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 2,\n    decoder_end_token_id: Optional[int] = 2,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n) -&gt; GenericOutputs\n</code></pre> <p>Generates sequences using the ChatGLMForGeneration model.</p> <p>Parameters:</p> Name Type Description Default <code>input_ids</code> <code>torch.Tensor</code> <p>The input token IDs.</p> required <code>num_beams</code> <code>Optional[int]</code> <p>The number of beams for beam search. Defaults to 5.</p> <code>5</code> <code>decoder_start_token_id</code> <code>Optional[int]</code> <p>The ID of the decoder start token. Defaults to 2.</p> <code>2</code> <code>decoder_end_token_id</code> <code>Optional[int]</code> <p>The ID of the decoder end token. Defaults to 2.</p> <code>2</code> <code>num_return_sequences</code> <code>Optional[int]</code> <p>The number of generated sequences to return. Defaults to 1.</p> <code>1</code> <code>min_gen_seq_length</code> <code>Optional[int]</code> <p>The minimum length of the generated sequences. Defaults to 0.</p> <code>0</code> <code>max_gen_seq_length</code> <code>Optional[int]</code> <p>The maximum length of the generated sequences. Defaults to 48.</p> <code>48</code> <code>repetition_penalty</code> <code>Optional[float]</code> <p>The repetition penalty for beam search. Defaults to 1.0.</p> <code>1.0</code> <code>no_repeat_ngram_size</code> <code>Optional[int]</code> <p>The size of n-grams to avoid repetition in beam search. Defaults to 0.</p> <code>0</code> <code>early_stopping</code> <code>Optional[bool]</code> <p>Whether to stop generation early based on the specified conditions. Defaults to True.</p> <code>True</code> <code>length_penalty</code> <code>Optional[float]</code> <p>The length penalty for beam search. Defaults to 1.0.</p> <code>1.0</code> <code>num_beam_groups</code> <code>Optional[int]</code> <p>The number of beam groups for diverse beam search. Defaults to 1.</p> <code>1</code> <code>diversity_penalty</code> <code>Optional[float]</code> <p>The diversity penalty for diverse beam search. Defaults to 0.0.</p> <code>0.0</code> <code>do_sample</code> <code>Optional[bool]</code> <p>Whether to use sampling for generation. Defaults to False.</p> <code>False</code> <code>temperature</code> <code>Optional[float]</code> <p>The temperature for sampling. Defaults to 1.0.</p> <code>1.0</code> <code>top_k</code> <code>Optional[int]</code> <p>The value of k for top-k sampling. Defaults to 50.</p> <code>50</code> <code>top_p</code> <code>Optional[float]</code> <p>The value of p for top-p sampling. Defaults to 1.0.</p> <code>1.0</code> <p>Returns:</p> Name Type Description <code>GenericOutputs</code> <code>GenericOutputs</code> <p>The generated sequences and their scores.</p> Source code in <code>src/unitorch/models/chatglm/modeling.py</code> <pre><code>@torch.no_grad()\ndef generate(\n    self,\n    input_ids: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 2,\n    decoder_end_token_id: Optional[int] = 2,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n) -&gt; GenericOutputs:\n\"\"\"\n    Generates sequences using the ChatGLMForGeneration model.\n\n    Args:\n        input_ids: The input token IDs.\n        num_beams (Optional[int]): The number of beams for beam search. Defaults to 5.\n        decoder_start_token_id (Optional[int]): The ID of the decoder start token. Defaults to 2.\n        decoder_end_token_id (Optional[int]): The ID of the decoder end token. Defaults to 2.\n        num_return_sequences (Optional[int]): The number of generated sequences to return. Defaults to 1.\n        min_gen_seq_length (Optional[int]): The minimum length of the generated sequences. Defaults to 0.\n        max_gen_seq_length (Optional[int]): The maximum length of the generated sequences. Defaults to 48.\n        repetition_penalty (Optional[float]): The repetition penalty for beam search. Defaults to 1.0.\n        no_repeat_ngram_size (Optional[int]): The size of n-grams to avoid repetition in beam search. Defaults to 0.\n        early_stopping (Optional[bool]): Whether to stop generation early based on the specified conditions. Defaults to True.\n        length_penalty (Optional[float]): The length penalty for beam search. Defaults to 1.0.\n        num_beam_groups (Optional[int]): The number of beam groups for diverse beam search. Defaults to 1.\n        diversity_penalty (Optional[float]): The diversity penalty for diverse beam search. Defaults to 0.0.\n        do_sample (Optional[bool]): Whether to use sampling for generation. Defaults to False.\n        temperature (Optional[float]): The temperature for sampling. Defaults to 1.0.\n        top_k (Optional[int]): The value of k for top-k sampling. Defaults to 50.\n        top_p (Optional[float]): The value of p for top-p sampling. Defaults to 1.0.\n\n    Returns:\n        GenericOutputs: The generated sequences and their scores.\n    \"\"\"\n    input_seq_length = input_ids.size(1)\n    outputs = self.model.generate(\n        input_ids,\n        max_length=max_gen_seq_length + input_seq_length,\n        min_length=min_gen_seq_length + input_seq_length,\n        num_beams=num_beams,\n        do_sample=do_sample,\n        decoder_start_token_id=decoder_start_token_id,\n        no_repeat_ngram_size=no_repeat_ngram_size,\n        early_stopping=early_stopping,\n        length_penalty=length_penalty,\n        repetition_penalty=repetition_penalty,\n        num_return_sequences=num_return_sequences,\n        bos_token_id=decoder_start_token_id,\n        eos_token_id=decoder_end_token_id,\n        num_beam_groups=num_beam_groups,\n        diversity_penalty=diversity_penalty,\n        temperature=temperature,\n        top_k=top_k,\n        top_p=top_p,\n        return_dict_in_generate=True,\n        output_scores=True,\n    )\n\n    sequences = outputs.sequences.reshape(\n        -1, num_return_sequences, outputs.sequences.size(-1)\n    )\n    outputs.sequences = torch.zeros(\n        sequences.size(0), num_return_sequences, max_gen_seq_length\n    ).to(device=sequences.device)\n    outputs.sequences[:, :, : sequences.size(-1) - input_seq_length].copy_(\n        sequences[:, :, input_seq_length : sequences.size(-1)]\n    )\n\n    if num_return_sequences == 1:\n        outputs.sequences = outputs.sequences.reshape(-1, max_gen_seq_length)\n\n    return GenericOutputs(\n        sequences=outputs.sequences.long(),\n        sequences_scores=outputs.sequences_scores,\n    )\n</code></pre>",
+            "text": "<pre><code>generate(\n    input_ids: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 2,\n    decoder_end_token_id: Optional[\n        Union[int, List[int]]\n    ] = 2,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n) -&gt; GenericOutputs\n</code></pre> <p>Generates sequences using the ChatGLMForGeneration model.</p> <p>Parameters:</p> Name Type Description Default <code>input_ids</code> <code>torch.Tensor</code> <p>The input token IDs.</p> required <code>num_beams</code> <code>Optional[int]</code> <p>The number of beams for beam search. Defaults to 5.</p> <code>5</code> <code>decoder_start_token_id</code> <code>Optional[int]</code> <p>The ID of the decoder start token. Defaults to 2.</p> <code>2</code> <code>decoder_end_token_id</code> <code>Optional[int]</code> <p>The ID of the decoder end token. Defaults to 2.</p> <code>2</code> <code>num_return_sequences</code> <code>Optional[int]</code> <p>The number of generated sequences to return. Defaults to 1.</p> <code>1</code> <code>min_gen_seq_length</code> <code>Optional[int]</code> <p>The minimum length of the generated sequences. Defaults to 0.</p> <code>0</code> <code>max_gen_seq_length</code> <code>Optional[int]</code> <p>The maximum length of the generated sequences. Defaults to 48.</p> <code>48</code> <code>repetition_penalty</code> <code>Optional[float]</code> <p>The repetition penalty for beam search. Defaults to 1.0.</p> <code>1.0</code> <code>no_repeat_ngram_size</code> <code>Optional[int]</code> <p>The size of n-grams to avoid repetition in beam search. Defaults to 0.</p> <code>0</code> <code>early_stopping</code> <code>Optional[bool]</code> <p>Whether to stop generation early based on the specified conditions. Defaults to True.</p> <code>True</code> <code>length_penalty</code> <code>Optional[float]</code> <p>The length penalty for beam search. Defaults to 1.0.</p> <code>1.0</code> <code>num_beam_groups</code> <code>Optional[int]</code> <p>The number of beam groups for diverse beam search. Defaults to 1.</p> <code>1</code> <code>diversity_penalty</code> <code>Optional[float]</code> <p>The diversity penalty for diverse beam search. Defaults to 0.0.</p> <code>0.0</code> <code>do_sample</code> <code>Optional[bool]</code> <p>Whether to use sampling for generation. Defaults to False.</p> <code>False</code> <code>temperature</code> <code>Optional[float]</code> <p>The temperature for sampling. Defaults to 1.0.</p> <code>1.0</code> <code>top_k</code> <code>Optional[int]</code> <p>The value of k for top-k sampling. Defaults to 50.</p> <code>50</code> <code>top_p</code> <code>Optional[float]</code> <p>The value of p for top-p sampling. Defaults to 1.0.</p> <code>1.0</code> <p>Returns:</p> Name Type Description <code>GenericOutputs</code> <code>GenericOutputs</code> <p>The generated sequences and their scores.</p> Source code in <code>src/unitorch/models/chatglm/modeling.py</code> <pre><code>@torch.no_grad()\ndef generate(\n    self,\n    input_ids: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 2,\n    decoder_end_token_id: Optional[Union[int, List[int]]] = 2,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n) -&gt; GenericOutputs:\n\"\"\"\n    Generates sequences using the ChatGLMForGeneration model.\n\n    Args:\n        input_ids: The input token IDs.\n        num_beams (Optional[int]): The number of beams for beam search. Defaults to 5.\n        decoder_start_token_id (Optional[int]): The ID of the decoder start token. Defaults to 2.\n        decoder_end_token_id (Optional[int]): The ID of the decoder end token. Defaults to 2.\n        num_return_sequences (Optional[int]): The number of generated sequences to return. Defaults to 1.\n        min_gen_seq_length (Optional[int]): The minimum length of the generated sequences. Defaults to 0.\n        max_gen_seq_length (Optional[int]): The maximum length of the generated sequences. Defaults to 48.\n        repetition_penalty (Optional[float]): The repetition penalty for beam search. Defaults to 1.0.\n        no_repeat_ngram_size (Optional[int]): The size of n-grams to avoid repetition in beam search. Defaults to 0.\n        early_stopping (Optional[bool]): Whether to stop generation early based on the specified conditions. Defaults to True.\n        length_penalty (Optional[float]): The length penalty for beam search. Defaults to 1.0.\n        num_beam_groups (Optional[int]): The number of beam groups for diverse beam search. Defaults to 1.\n        diversity_penalty (Optional[float]): The diversity penalty for diverse beam search. Defaults to 0.0.\n        do_sample (Optional[bool]): Whether to use sampling for generation. Defaults to False.\n        temperature (Optional[float]): The temperature for sampling. Defaults to 1.0.\n        top_k (Optional[int]): The value of k for top-k sampling. Defaults to 50.\n        top_p (Optional[float]): The value of p for top-p sampling. Defaults to 1.0.\n\n    Returns:\n        GenericOutputs: The generated sequences and their scores.\n    \"\"\"\n    input_seq_length = input_ids.size(1)\n    outputs = self.model.generate(\n        input_ids,\n        max_length=max_gen_seq_length + input_seq_length,\n        min_length=min_gen_seq_length + input_seq_length,\n        num_beams=num_beams,\n        do_sample=do_sample,\n        decoder_start_token_id=decoder_start_token_id,\n        no_repeat_ngram_size=no_repeat_ngram_size,\n        early_stopping=early_stopping,\n        length_penalty=length_penalty,\n        repetition_penalty=repetition_penalty,\n        num_return_sequences=num_return_sequences,\n        bos_token_id=decoder_start_token_id,\n        eos_token_id=decoder_end_token_id,\n        num_beam_groups=num_beam_groups,\n        diversity_penalty=diversity_penalty,\n        temperature=temperature,\n        top_k=top_k,\n        top_p=top_p,\n        return_dict_in_generate=True,\n        output_scores=True,\n    )\n\n    sequences = outputs.sequences.reshape(\n        -1, num_return_sequences, outputs.sequences.size(-1)\n    )\n    outputs.sequences = torch.zeros(\n        sequences.size(0), num_return_sequences, max_gen_seq_length\n    ).to(device=sequences.device)\n    outputs.sequences[:, :, : sequences.size(-1) - input_seq_length].copy_(\n        sequences[:, :, input_seq_length : sequences.size(-1)]\n    )\n\n    if num_return_sequences == 1:\n        outputs.sequences = outputs.sequences.reshape(-1, max_gen_seq_length)\n\n    return GenericOutputs(\n        sequences=outputs.sequences.long(),\n        sequences_scores=outputs.sequences_scores,\n    )\n</code></pre>",
             "title": "generate"
         },
         {
             "location": "models/clip/",
             "text": "",
             "title": "unitorch.models.clip"
         },
@@ -2147,15 +2182,15 @@
         {
             "location": "models/diffusers/#unitorch.models.bart.modeling.BartForGeneration.forward",
             "text": "<pre><code>forward(\n    input_ids: torch.Tensor,\n    attention_mask: torch.Tensor,\n    decoder_input_ids: torch.Tensor,\n    decoder_attention_mask: torch.Tensor,\n)\n</code></pre> <p>Performs forward pass of the BartForGeneration model.</p> <p>Parameters:</p> Name Type Description Default <code>input_ids</code> <code>torch.Tensor</code> <p>Tensor of input token IDs.</p> required <code>attention_mask</code> <code>torch.Tensor</code> <p>Tensor indicating which tokens should be attended to.</p> required <code>decoder_input_ids</code> <code>torch.Tensor</code> <p>Tensor of decoder input token IDs.</p> required <code>decoder_attention_mask</code> <code>torch.Tensor</code> <p>Tensor indicating which decoder tokens should be attended to.</p> required <p>Returns:</p> Type Description <code>torch.Tensor</code> <p>Output logits of the model.</p> Source code in <code>src/unitorch/models/bart/modeling.py</code> <pre><code>def forward(\n    self,\n    input_ids: torch.Tensor,\n    attention_mask: torch.Tensor,\n    decoder_input_ids: torch.Tensor,\n    decoder_attention_mask: torch.Tensor,\n):\n\"\"\"\n    Performs forward pass of the BartForGeneration model.\n\n    Args:\n        input_ids (torch.Tensor): Tensor of input token IDs.\n        attention_mask (torch.Tensor): Tensor indicating which tokens should be attended to.\n        decoder_input_ids (torch.Tensor): Tensor of decoder input token IDs.\n        decoder_attention_mask (torch.Tensor): Tensor indicating which decoder tokens should be attended to.\n\n    Returns:\n        (torch.Tensor): Output logits of the model.\n    \"\"\"\n    outputs = self.model(\n        input_ids=input_ids,\n        attention_mask=attention_mask,\n        decoder_input_ids=decoder_input_ids,\n        decoder_attention_mask=decoder_attention_mask,\n        return_dict=True,\n    )\n    logits = outputs.logits\n    print(\"model :\", logits[0, 0, 0].item(), logits[0, 0, 41552].item())\n    return logits\n</code></pre>",
             "title": "forward"
         },
         {
             "location": "models/diffusers/#unitorch.models.bart.modeling.BartForGeneration.generate",
-            "text": "<pre><code>generate(\n    input_ids: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 2,\n    decoder_end_token_id: Optional[int] = 2,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n)\n</code></pre> <p>Generates text using the BartForGeneration model.</p> <p>Parameters:</p> Name Type Description Default <code>input_ids</code> <code>torch.Tensor</code> <p>Tensor of input token IDs.</p> required <code>num_beams</code> <code>int</code> <p>Number of beams for beam search. Defaults to 5.</p> <code>5</code> <code>decoder_start_token_id</code> <code>int</code> <p>Start token ID for the decoder. Defaults to 2.</p> <code>2</code> <code>decoder_end_token_id</code> <code>int</code> <p>End token ID for the decoder. Defaults to 2.</p> <code>2</code> <code>num_return_sequences</code> <code>int</code> <p>Number of sequences to return. Defaults to 1.</p> <code>1</code> <code>min_gen_seq_length</code> <code>int</code> <p>Minimum length of generated sequences. Defaults to 0.</p> <code>0</code> <code>max_gen_seq_length</code> <code>int</code> <p>Maximum length of generated sequences. Defaults to 48.</p> <code>48</code> <code>repetition_penalty</code> <code>float</code> <p>Repetition penalty for generated sequences. Defaults to 1.0.</p> <code>1.0</code> <code>no_repeat_ngram_size</code> <code>int</code> <p>Size of n-grams to avoid repetition. Defaults to 0.</p> <code>0</code> <code>early_stopping</code> <code>bool</code> <p>Whether to stop generation early. Defaults to True.</p> <code>True</code> <code>length_penalty</code> <code>float</code> <p>Length penalty for generated sequences. Defaults to 1.0.</p> <code>1.0</code> <code>num_beam_groups</code> <code>int</code> <p>Number of beam groups for diverse beam search. Defaults to 1.</p> <code>1</code> <code>diversity_penalty</code> <code>float</code> <p>Diversity penalty for diverse beam search. Defaults to 0.0.</p> <code>0.0</code> <code>do_sample</code> <code>bool</code> <p>Whether to use sampling during generation. Defaults to False.</p> <code>False</code> <code>temperature</code> <code>float</code> <p>Temperature for sampling. Defaults to 1.0.</p> <code>1.0</code> <code>top_k</code> <code>int</code> <p>Value for top-k sampling. Defaults to 50.</p> <code>50</code> <code>top_p</code> <code>float</code> <p>Value for top-p sampling. Defaults to 1.0.</p> <code>1.0</code> <p>Returns:</p> Name Type Description <code>GenericOutputs</code> <p>Generated sequences and their scores.</p> Source code in <code>src/unitorch/models/bart/modeling.py</code> <pre><code>@torch.no_grad()\ndef generate(\n    self,\n    input_ids: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 2,\n    decoder_end_token_id: Optional[int] = 2,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n):\n\"\"\"\n    Generates text using the BartForGeneration model.\n\n    Args:\n        input_ids (torch.Tensor): Tensor of input token IDs.\n        num_beams (int, optional): Number of beams for beam search. Defaults to 5.\n        decoder_start_token_id (int, optional): Start token ID for the decoder. Defaults to 2.\n        decoder_end_token_id (int, optional): End token ID for the decoder. Defaults to 2.\n        num_return_sequences (int, optional): Number of sequences to return. Defaults to 1.\n        min_gen_seq_length (int, optional): Minimum length of generated sequences. Defaults to 0.\n        max_gen_seq_length (int, optional): Maximum length of generated sequences. Defaults to 48.\n        repetition_penalty (float, optional): Repetition penalty for generated sequences. Defaults to 1.0.\n        no_repeat_ngram_size (int, optional): Size of n-grams to avoid repetition. Defaults to 0.\n        early_stopping (bool, optional): Whether to stop generation early. Defaults to True.\n        length_penalty (float, optional): Length penalty for generated sequences. Defaults to 1.0.\n        num_beam_groups (int, optional): Number of beam groups for diverse beam search. Defaults to 1.\n        diversity_penalty (float, optional): Diversity penalty for diverse beam search. Defaults to 0.0.\n        do_sample (bool, optional): Whether to use sampling during generation. Defaults to False.\n        temperature (float, optional): Temperature for sampling. Defaults to 1.0.\n        top_k (int, optional): Value for top-k sampling. Defaults to 50.\n        top_p (float, optional): Value for top-p sampling. Defaults to 1.0.\n\n    Returns:\n        GenericOutputs: Generated sequences and their scores.\n    \"\"\"\n    outputs = self.model.generate(\n        input_ids,\n        max_length=max_gen_seq_length,\n        min_length=min_gen_seq_length,\n        num_beams=num_beams,\n        do_sample=do_sample,\n        decoder_start_token_id=decoder_start_token_id,\n        no_repeat_ngram_size=no_repeat_ngram_size,\n        early_stopping=early_stopping,\n        length_penalty=length_penalty,\n        repetition_penalty=repetition_penalty,\n        num_return_sequences=num_return_sequences,\n        bos_token_id=decoder_start_token_id,\n        eos_token_id=decoder_end_token_id,\n        num_beam_groups=num_beam_groups,\n        diversity_penalty=diversity_penalty,\n        temperature=temperature,\n        top_k=top_k,\n        top_p=top_p,\n        return_dict_in_generate=True,\n        output_scores=True,\n    )\n\n    sequences = outputs.sequences.reshape(\n        -1, num_return_sequences, outputs.sequences.size(-1)\n    )\n    outputs.sequences = torch.zeros(\n        sequences.size(0), num_return_sequences, max_gen_seq_length\n    ).to(device=sequences.device)\n    outputs.sequences[:, :, : sequences.size(-1)].copy_(sequences)\n\n    if num_return_sequences == 1:\n        outputs.sequences = outputs.sequences.reshape(-1, max_gen_seq_length)\n\n    return GenericOutputs(\n        sequences=outputs.sequences, sequences_scores=outputs.sequences_scores\n    )\n</code></pre>",
+            "text": "<pre><code>generate(\n    input_ids: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 2,\n    decoder_end_token_id: Optional[\n        Union[int, List[int]]\n    ] = 2,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n)\n</code></pre> <p>Generates text using the BartForGeneration model.</p> <p>Parameters:</p> Name Type Description Default <code>input_ids</code> <code>torch.Tensor</code> <p>Tensor of input token IDs.</p> required <code>num_beams</code> <code>int</code> <p>Number of beams for beam search. Defaults to 5.</p> <code>5</code> <code>decoder_start_token_id</code> <code>int</code> <p>The ID of the decoder start token. Defaults to 2.</p> <code>2</code> <code>decoder_end_token_id</code> <code>int or List[int]</code> <p>The ID(s) of the decoder end token(s). Defaults to 2.</p> <code>2</code> <code>num_return_sequences</code> <code>int</code> <p>Number of sequences to return. Defaults to 1.</p> <code>1</code> <code>min_gen_seq_length</code> <code>int</code> <p>Minimum length of generated sequences. Defaults to 0.</p> <code>0</code> <code>max_gen_seq_length</code> <code>int</code> <p>Maximum length of generated sequences. Defaults to 48.</p> <code>48</code> <code>repetition_penalty</code> <code>float</code> <p>Repetition penalty for generated sequences. Defaults to 1.0.</p> <code>1.0</code> <code>no_repeat_ngram_size</code> <code>int</code> <p>Size of n-grams to avoid repetition. Defaults to 0.</p> <code>0</code> <code>early_stopping</code> <code>bool</code> <p>Whether to stop generation early. Defaults to True.</p> <code>True</code> <code>length_penalty</code> <code>float</code> <p>Length penalty for generated sequences. Defaults to 1.0.</p> <code>1.0</code> <code>num_beam_groups</code> <code>int</code> <p>Number of beam groups for diverse beam search. Defaults to 1.</p> <code>1</code> <code>diversity_penalty</code> <code>float</code> <p>Diversity penalty for diverse beam search. Defaults to 0.0.</p> <code>0.0</code> <code>do_sample</code> <code>bool</code> <p>Whether to use sampling during generation. Defaults to False.</p> <code>False</code> <code>temperature</code> <code>float</code> <p>Temperature for sampling. Defaults to 1.0.</p> <code>1.0</code> <code>top_k</code> <code>int</code> <p>Value for top-k sampling. Defaults to 50.</p> <code>50</code> <code>top_p</code> <code>float</code> <p>Value for top-p sampling. Defaults to 1.0.</p> <code>1.0</code> <p>Returns:</p> Name Type Description <code>GenericOutputs</code> <p>Generated sequences and their scores.</p> Source code in <code>src/unitorch/models/bart/modeling.py</code> <pre><code>@torch.no_grad()\ndef generate(\n    self,\n    input_ids: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 2,\n    decoder_end_token_id: Optional[Union[int, List[int]]] = 2,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n):\n\"\"\"\n    Generates text using the BartForGeneration model.\n\n    Args:\n        input_ids (torch.Tensor): Tensor of input token IDs.\n        num_beams (int, optional): Number of beams for beam search. Defaults to 5.\n        decoder_start_token_id (int, optional): The ID of the decoder start token. Defaults to 2.\n        decoder_end_token_id (int or List[int], optional): The ID(s) of the decoder end token(s). Defaults to 2.\n        num_return_sequences (int, optional): Number of sequences to return. Defaults to 1.\n        min_gen_seq_length (int, optional): Minimum length of generated sequences. Defaults to 0.\n        max_gen_seq_length (int, optional): Maximum length of generated sequences. Defaults to 48.\n        repetition_penalty (float, optional): Repetition penalty for generated sequences. Defaults to 1.0.\n        no_repeat_ngram_size (int, optional): Size of n-grams to avoid repetition. Defaults to 0.\n        early_stopping (bool, optional): Whether to stop generation early. Defaults to True.\n        length_penalty (float, optional): Length penalty for generated sequences. Defaults to 1.0.\n        num_beam_groups (int, optional): Number of beam groups for diverse beam search. Defaults to 1.\n        diversity_penalty (float, optional): Diversity penalty for diverse beam search. Defaults to 0.0.\n        do_sample (bool, optional): Whether to use sampling during generation. Defaults to False.\n        temperature (float, optional): Temperature for sampling. Defaults to 1.0.\n        top_k (int, optional): Value for top-k sampling. Defaults to 50.\n        top_p (float, optional): Value for top-p sampling. Defaults to 1.0.\n\n    Returns:\n        GenericOutputs: Generated sequences and their scores.\n    \"\"\"\n    outputs = self.model.generate(\n        input_ids,\n        max_length=max_gen_seq_length,\n        min_length=min_gen_seq_length,\n        num_beams=num_beams,\n        do_sample=do_sample,\n        decoder_start_token_id=decoder_start_token_id,\n        no_repeat_ngram_size=no_repeat_ngram_size,\n        early_stopping=early_stopping,\n        length_penalty=length_penalty,\n        repetition_penalty=repetition_penalty,\n        num_return_sequences=num_return_sequences,\n        bos_token_id=decoder_start_token_id,\n        eos_token_id=decoder_end_token_id,\n        num_beam_groups=num_beam_groups,\n        diversity_penalty=diversity_penalty,\n        temperature=temperature,\n        top_k=top_k,\n        top_p=top_p,\n        return_dict_in_generate=True,\n        output_scores=True,\n    )\n\n    sequences = outputs.sequences.reshape(\n        -1, num_return_sequences, outputs.sequences.size(-1)\n    )\n    outputs.sequences = torch.zeros(\n        sequences.size(0), num_return_sequences, max_gen_seq_length\n    ).to(device=sequences.device)\n    outputs.sequences[:, :, : sequences.size(-1)].copy_(sequences)\n\n    if num_return_sequences == 1:\n        outputs.sequences = outputs.sequences.reshape(-1, max_gen_seq_length)\n\n    return GenericOutputs(\n        sequences=outputs.sequences, sequences_scores=outputs.sequences_scores\n    )\n</code></pre>",
             "title": "generate"
         },
         {
             "location": "models/llama/",
             "text": "",
             "title": "unitorch.models.llama"
         },
@@ -2167,15 +2202,15 @@
         {
             "location": "models/llama/#unitorch.models.llama.processing.LlamaProcessor.classification",
             "text": "<pre><code>classification(\n    text: str,\n    text_pair: Optional[str] = None,\n    max_seq_length: Optional[int] = None,\n)\n</code></pre> <p>Process text for classification.</p> <p>Parameters:</p> Name Type Description Default <code>text</code> <code>str</code> <p>Input text.</p> required <code>text_pair</code> <code>str</code> <p>Input text pair. Defaults to None.</p> <code>None</code> <code>max_seq_length</code> <code>int</code> <p>Maximum sequence length. Defaults to None.</p> <code>None</code> <p>Returns:</p> Name Type Description <code>GenericOutputs</code> <p>Processed input_ids and attention_mask tensors.</p> Source code in <code>src/unitorch/models/llama/processing.py</code> <pre><code>def classification(\n    self,\n    text: str,\n    text_pair: Optional[str] = None,\n    max_seq_length: Optional[int] = None,\n):\n\"\"\"\n    Process text for classification.\n\n    Args:\n        text (str): Input text.\n        text_pair (str, optional): Input text pair. Defaults to None.\n        max_seq_length (int, optional): Maximum sequence length. Defaults to None.\n\n    Returns:\n        GenericOutputs: Processed input_ids and attention_mask tensors.\n    \"\"\"\n    max_seq_length = pop_value(\n        max_seq_length,\n        self.max_seq_length,\n    )\n\n    tokens = self.tokenizer.tokenize(str(text))\n    if text_pair is None:\n        tokens = tokens[:max_seq_length]\n        input_ids = self.tokenizer.convert_tokens_to_ids(tokens)\n    else:\n        tokens_pair = self.tokenizer.tokenize(str(text_pair))\n        truncate_sequence_pair(tokens, tokens_pair, max_seq_length)\n        tokens = tokens + tokens_pair\n        input_ids = self.tokenizer.convert_tokens_to_ids(tokens)\n\n    padding = [0] * (max_seq_length - len(input_ids))\n    attention_mask = [0] * len(padding) + [1] * len(input_ids)\n    input_ids = len(padding) * [self.pad_token_id] + input_ids\n\n    assert len(input_ids) == max_seq_length\n    assert len(attention_mask) == max_seq_length\n    return GenericOutputs(\n        input_ids=torch.tensor(input_ids, dtype=torch.long),\n        attention_mask=torch.tensor(attention_mask, dtype=torch.long),\n    )\n</code></pre>",
             "title": "classification"
         },
         {
             "location": "models/llama/#unitorch.models.llama.processing.LlamaProcessor.generation",
-            "text": "<pre><code>generation(\n    text: str,\n    text_pair: str,\n    max_seq_length: Optional[int] = None,\n    max_gen_seq_length: Optional[int] = None,\n)\n</code></pre> <p>Process text for generation.</p> <p>Parameters:</p> Name Type Description Default <code>text</code> <code>str</code> <p>Input text.</p> required <code>text_pair</code> <code>str</code> <p>Input text pair.</p> required <code>max_seq_length</code> <code>int</code> <p>Maximum sequence length. Defaults to None.</p> <code>None</code> <code>max_gen_seq_length</code> <code>int</code> <p>Maximum generation sequence length. Defaults to None.</p> <code>None</code> <p>Returns:</p> Name Type Description <code>GenericOutputs</code> <p>Processed input_ids, attention_mask, input_ids_label, and attention_mask_label tensors.</p> Source code in <code>src/unitorch/models/llama/processing.py</code> <pre><code>def generation(\n    self,\n    text: str,\n    text_pair: str,\n    max_seq_length: Optional[int] = None,\n    max_gen_seq_length: Optional[int] = None,\n):\n\"\"\"\n    Process text for generation.\n\n    Args:\n        text (str): Input text.\n        text_pair (str): Input text pair.\n        max_seq_length (int, optional): Maximum sequence length. Defaults to None.\n        max_gen_seq_length (int, optional): Maximum generation sequence length. Defaults to None.\n\n    Returns:\n        GenericOutputs: Processed input_ids, attention_mask, input_ids_label, and attention_mask_label tensors.\n    \"\"\"\n    max_seq_length = pop_value(\n        max_seq_length,\n        self.max_seq_length,\n    )\n    max_gen_seq_length = pop_value(\n        max_gen_seq_length,\n        self.max_gen_seq_length,\n    )\n    max_seq_length = max_seq_length + max_gen_seq_length\n\n    tokens = [self.bos_token] + self.tokenizer.tokenize(str(text))[\n        1 - max_seq_length :\n    ]\n    tokens_pair = self.tokenizer.tokenize(str(text_pair))[\n        : max_gen_seq_length - 1\n    ] + [self.eos_token]\n    padding_a = [self.pad_token] * (max_seq_length - len(tokens))\n    padding_b = [self.pad_token] * (max_gen_seq_length - len(tokens_pair))\n    attention_mask = (\n        [0] * len(padding_a)\n        + [1] * (len(tokens) + len(tokens_pair))\n        + [0] * len(padding_b)\n    )\n    _tokens = padding_a + tokens + tokens_pair + padding_b\n    input_ids = self.tokenizer.convert_tokens_to_ids(_tokens)\n\n    tokens_label = tokens_pair[1:max_gen_seq_length] + [self.pad_token] * (\n        max_gen_seq_length - len(tokens_pair) + 1\n    )\n    input_ids_label = self.tokenizer.convert_tokens_to_ids(tokens_label)\n    input_ids_label = [0] * max_seq_length + input_ids_label\n    attention_mask_label = [1] * len(tokens_pair[1:max_gen_seq_length]) + [0] * (\n        max_gen_seq_length - len(tokens_pair) + 1\n    )\n    attention_mask_label = [0] * max_seq_length + attention_mask_label\n\n    return GenericOutputs(\n        input_ids=torch.tensor(input_ids, dtype=torch.long),\n        attention_mask=torch.tensor(attention_mask, dtype=torch.long),\n        input_ids_label=torch.tensor(input_ids_label, dtype=torch.long),\n        attention_mask_label=torch.tensor(attention_mask_label, dtype=torch.long),\n    )\n</code></pre>",
+            "text": "<pre><code>generation(\n    text: str,\n    text_pair: str,\n    max_seq_length: Optional[int] = None,\n    max_gen_seq_length: Optional[int] = None,\n)\n</code></pre> <p>Process text for generation.</p> <p>Parameters:</p> Name Type Description Default <code>text</code> <code>str</code> <p>Input text.</p> required <code>text_pair</code> <code>str</code> <p>Input text pair.</p> required <code>max_seq_length</code> <code>int</code> <p>Maximum sequence length. Defaults to None.</p> <code>None</code> <code>max_gen_seq_length</code> <code>int</code> <p>Maximum generation sequence length. Defaults to None.</p> <code>None</code> <p>Returns:</p> Name Type Description <code>GenericOutputs</code> <p>Processed input_ids, attention_mask, input_ids_label, and attention_mask_label tensors.</p> Source code in <code>src/unitorch/models/llama/processing.py</code> <pre><code>def generation(\n    self,\n    text: str,\n    text_pair: str,\n    max_seq_length: Optional[int] = None,\n    max_gen_seq_length: Optional[int] = None,\n):\n\"\"\"\n    Process text for generation.\n\n    Args:\n        text (str): Input text.\n        text_pair (str): Input text pair.\n        max_seq_length (int, optional): Maximum sequence length. Defaults to None.\n        max_gen_seq_length (int, optional): Maximum generation sequence length. Defaults to None.\n\n    Returns:\n        GenericOutputs: Processed input_ids, attention_mask, input_ids_label, and attention_mask_label tensors.\n    \"\"\"\n    max_seq_length = pop_value(\n        max_seq_length,\n        self.max_seq_length,\n    )\n    max_gen_seq_length = pop_value(\n        max_gen_seq_length,\n        self.max_gen_seq_length,\n    )\n    max_seq_length = max_seq_length + max_gen_seq_length\n\n    tokens = [self.bos_token] + self.tokenizer.tokenize(str(text))[\n        1 - max_seq_length :\n    ]\n    tokens_pair = self.tokenizer.tokenize(str(text_pair))[\n        : max_gen_seq_length - 1\n    ] + [self.eos_token]\n    padding_a = [self.pad_token] * (max_seq_length - len(tokens))\n    padding_b = [self.pad_token] * (max_gen_seq_length - len(tokens_pair))\n    attention_mask = (\n        [0] * len(padding_a)\n        + [1] * (len(tokens) + len(tokens_pair))\n        + [0] * len(padding_b)\n    )\n    _tokens = padding_a + tokens + tokens_pair + padding_b\n    input_ids = self.tokenizer.convert_tokens_to_ids(_tokens)\n\n    tokens_label = tokens_pair + [self.pad_token] * (\n        max_gen_seq_length - len(tokens_pair) + 1\n    )\n    input_ids_label = self.tokenizer.convert_tokens_to_ids(tokens_label)\n    input_ids_label = [0] * (max_seq_length - 1) + input_ids_label\n    attention_mask_label = [1] * len(tokens_pair) + [0] * (\n        max_gen_seq_length - len(tokens_pair) + 1\n    )\n    attention_mask_label = [0] * (max_seq_length - 1) + attention_mask_label\n\n    return GenericOutputs(\n        input_ids=torch.tensor(input_ids, dtype=torch.long),\n        attention_mask=torch.tensor(attention_mask, dtype=torch.long),\n        input_ids_label=torch.tensor(input_ids_label, dtype=torch.long),\n        attention_mask_label=torch.tensor(attention_mask_label, dtype=torch.long),\n    )\n</code></pre>",
             "title": "generation"
         },
         {
             "location": "models/llama/#unitorch.models.llama.processing.LlamaProcessor.generation_inputs",
             "text": "<pre><code>generation_inputs(\n    text: str, max_seq_length: Optional[int] = None\n)\n</code></pre> <p>Process text for generation inputs.</p> <p>Parameters:</p> Name Type Description Default <code>text</code> <code>str</code> <p>Input text.</p> required <code>max_seq_length</code> <code>int</code> <p>Maximum sequence length. Defaults to None.</p> <code>None</code> <p>Returns:</p> Name Type Description <code>GenericOutputs</code> <p>Processed input_ids tensor.</p> Source code in <code>src/unitorch/models/llama/processing.py</code> <pre><code>def generation_inputs(\n    self,\n    text: str,\n    max_seq_length: Optional[int] = None,\n):\n\"\"\"\n    Process text for generation inputs.\n\n    Args:\n        text (str): Input text.\n        max_seq_length (int, optional): Maximum sequence length. Defaults to None.\n\n    Returns:\n        GenericOutputs: Processed input_ids tensor.\n    \"\"\"\n    max_seq_length = pop_value(\n        max_seq_length,\n        self.max_seq_length,\n    )\n    tokens = [self.bos_token] + self.tokenizer.tokenize(str(text))[\n        1 - max_seq_length :\n    ]\n    padding = [self.pad_token] * (max_seq_length - len(tokens))\n    tokens = padding + tokens\n    input_ids = self.tokenizer.convert_tokens_to_ids(tokens)\n\n    assert len(input_ids) == max_seq_length\n    return GenericOutputs(\n        input_ids=torch.tensor(input_ids, dtype=torch.long),\n    )\n</code></pre>",
             "title": "generation_inputs"
         },
@@ -2217,15 +2252,15 @@
         {
             "location": "models/llama/#unitorch.models.llama.modeling.LlamaForGeneration.forward",
             "text": "<pre><code>forward(\n    input_ids: torch.Tensor,\n    attention_mask: Optional[torch.Tensor] = None,\n    position_ids: Optional[torch.Tensor] = None,\n)\n</code></pre> <p>Forward pass of the generation model.</p> <p>Parameters:</p> Name Type Description Default <code>input_ids</code> <code>torch.Tensor</code> <p>Input tensor of shape (batch_size, sequence_length). Defaults to None.</p> required <code>attention_mask</code> <code>torch.Tensor</code> <p>Attention mask tensor of shape (batch_size, sequence_length). Defaults to None.</p> <code>None</code> <code>position_ids</code> <code>torch.Tensor</code> <p>Position IDs tensor of shape (batch_size, sequence_length). Defaults to None.</p> <code>None</code> <p>Returns:</p> Type Description <p>torch Output logits.Tensor: tensor of shape (batch_size, sequence_length, vocab_size).</p> Source code in <code>src/unitorch/models/llama/modeling.py</code> <pre><code>def forward(\n    self,\n    input_ids: torch.Tensor,\n    attention_mask: Optional[torch.Tensor] = None,\n    position_ids: Optional[torch.Tensor] = None,\n):\n\"\"\"\n    Forward pass of the generation model.\n\n    Args:\n        input_ids (torch.Tensor, optional): Input tensor of shape (batch_size, sequence_length). Defaults to None.\n        attention_mask (torch.Tensor, optional): Attention mask tensor of shape (batch_size, sequence_length). Defaults to None.\n        position_ids (torch.Tensor, optional): Position IDs tensor of shape (batch_size, sequence_length). Defaults to None.\n\n    Returns:\n        torch Output logits.Tensor: tensor of shape (batch_size, sequence_length, vocab_size).\n    \"\"\"\n    outputs = self.model(\n        input_ids=input_ids,\n        attention_mask=attention_mask,\n        position_ids=position_ids,\n        return_dict=True,\n    )\n    logits = outputs.logits\n    return logits\n</code></pre>",
             "title": "forward"
         },
         {
             "location": "models/llama/#unitorch.models.llama.modeling.LlamaForGeneration.generate",
-            "text": "<pre><code>generate(\n    input_ids: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 1,\n    decoder_end_token_id: Optional[int] = 2,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n)\n</code></pre> <p>Generate text using the generation model.</p> <p>Parameters:</p> Name Type Description Default <code>input_ids</code> <code>torch.Tensor</code> <p>Input tensor of shape (batch_size, sequence_length).</p> required <code>num_beams</code> <code>int</code> <p>Number of beams for beam search. Defaults to 5.</p> <code>5</code> <code>decoder_start_token_id</code> <code>int</code> <p>Start token ID for the decoder. Defaults to 2.</p> <code>1</code> <code>decoder_end_token_id</code> <code>int</code> <p>End token ID for the decoder. Defaults to 2.</p> <code>2</code> <code>num_return_sequences</code> <code>int</code> <p>Number of generated sequences to return. Defaults to 1.</p> <code>1</code> <code>min_gen_seq_length</code> <code>int</code> <p>Minimum length of generated sequences. Defaults to 0.</p> <code>0</code> <code>max_gen_seq_length</code> <code>int</code> <p>Maximum length of generated sequences. Defaults to 48.</p> <code>48</code> <code>repetition_penalty</code> <code>float</code> <p>Penalty for repeated tokens. Defaults to 1.0.</p> <code>1.0</code> <code>no_repeat_ngram_size</code> <code>int</code> <p>Size of n-grams to avoid repeating. Defaults to 0.</p> <code>0</code> <code>early_stopping</code> <code>bool</code> <p>Whether to stop generation early. Defaults to True.</p> <code>True</code> <code>length_penalty</code> <code>float</code> <p>Penalty for longer sequences. Defaults to 1.0.</p> <code>1.0</code> <code>num_beam_groups</code> <code>int</code> <p>Number of beam groups for diverse beam search. Defaults to 1.</p> <code>1</code> <code>diversity_penalty</code> <code>float</code> <p>Penalty for diverse sequences in diverse beam search. Defaults to 0.0.</p> <code>0.0</code> <code>do_sample</code> <code>bool</code> <p>Whether to use sampling for generation. Defaults to False.</p> <code>False</code> <code>temperature</code> <code>float</code> <p>Sampling temperature. Defaults to 1.0.</p> <code>1.0</code> <code>top_k</code> <code>int</code> <p>Top-k value for sampling. Defaults to 50.</p> <code>50</code> <code>top_p</code> <code>float</code> <p>Top-p value for sampling. Defaults to 1.0.</p> <code>1.0</code> <p>Returns:</p> Name Type Description <code>GenericOutputs</code> <p>Generated sequences and their scores.</p> Source code in <code>src/unitorch/models/llama/modeling.py</code> <pre><code>@torch.no_grad()\ndef generate(\n    self,\n    input_ids: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 1,\n    decoder_end_token_id: Optional[int] = 2,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n):\n\"\"\"\n    Generate text using the generation model.\n\n    Args:\n        input_ids: Input tensor of shape (batch_size, sequence_length).\n        num_beams (int, optional): Number of beams for beam search. Defaults to 5.\n        decoder_start_token_id (int, optional): Start token ID for the decoder. Defaults to 2.\n        decoder_end_token_id (int, optional): End token ID for the decoder. Defaults to 2.\n        num_return_sequences (int, optional): Number of generated sequences to return. Defaults to 1.\n        min_gen_seq_length (int, optional): Minimum length of generated sequences. Defaults to 0.\n        max_gen_seq_length (int, optional): Maximum length of generated sequences. Defaults to 48.\n        repetition_penalty (float, optional): Penalty for repeated tokens. Defaults to 1.0.\n        no_repeat_ngram_size (int, optional): Size of n-grams to avoid repeating. Defaults to 0.\n        early_stopping (bool, optional): Whether to stop generation early. Defaults to True.\n        length_penalty (float, optional): Penalty for longer sequences. Defaults to 1.0.\n        num_beam_groups (int, optional): Number of beam groups for diverse beam search. Defaults to 1.\n        diversity_penalty (float, optional): Penalty for diverse sequences in diverse beam search. Defaults to 0.0.\n        do_sample (bool, optional): Whether to use sampling for generation. Defaults to False.\n        temperature (float, optional): Sampling temperature. Defaults to 1.0.\n        top_k (int, optional): Top-k value for sampling. Defaults to 50.\n        top_p (float, optional): Top-p value for sampling. Defaults to 1.0.\n\n    Returns:\n        GenericOutputs: Generated sequences and their scores.\n    \"\"\"\n    input_seq_length = input_ids.size(1)\n    outputs = self.model.generate(\n        input_ids,\n        max_length=max_gen_seq_length + input_seq_length,\n        min_length=min_gen_seq_length + input_seq_length,\n        num_beams=num_beams,\n        do_sample=do_sample,\n        decoder_start_token_id=decoder_start_token_id,\n        no_repeat_ngram_size=no_repeat_ngram_size,\n        early_stopping=early_stopping,\n        length_penalty=length_penalty,\n        repetition_penalty=repetition_penalty,\n        num_return_sequences=num_return_sequences,\n        bos_token_id=decoder_start_token_id,\n        eos_token_id=decoder_end_token_id,\n        num_beam_groups=num_beam_groups,\n        diversity_penalty=diversity_penalty,\n        temperature=temperature,\n        top_k=top_k,\n        top_p=top_p,\n        return_dict_in_generate=True,\n        output_scores=True,\n    )\n\n    sequences = outputs.sequences.reshape(\n        -1, num_return_sequences, outputs.sequences.size(-1)\n    )\n    outputs.sequences = torch.zeros(\n        sequences.size(0), num_return_sequences, max_gen_seq_length\n    ).to(device=sequences.device)\n    outputs.sequences[:, :, : sequences.size(-1) - input_seq_length].copy_(\n        sequences[:, :, input_seq_length : sequences.size(-1)]\n    )\n\n    if num_return_sequences == 1:\n        outputs.sequences = outputs.sequences.reshape(-1, max_gen_seq_length)\n\n    return GenericOutputs(\n        sequences=outputs.sequences.long(),\n        sequences_scores=outputs.sequences_scores,\n    )\n</code></pre>",
+            "text": "<pre><code>generate(\n    input_ids: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 1,\n    decoder_end_token_id: Optional[\n        Union[int, List[int]]\n    ] = 2,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n)\n</code></pre> <p>Generate text using the generation model.</p> <p>Parameters:</p> Name Type Description Default <code>input_ids</code> <code>torch.Tensor</code> <p>Input tensor of shape (batch_size, sequence_length).</p> required <code>num_beams</code> <code>int</code> <p>Number of beams for beam search. Defaults to 5.</p> <code>5</code> <code>decoder_start_token_id</code> <code>int</code> <p>The ID of the decoder start token. Defaults to 2.</p> <code>1</code> <code>decoder_end_token_id</code> <code>int or List[int]</code> <p>The ID(s) of the decoder end token(s). Defaults to 2.</p> <code>2</code> <code>num_return_sequences</code> <code>int</code> <p>Number of generated sequences to return. Defaults to 1.</p> <code>1</code> <code>min_gen_seq_length</code> <code>int</code> <p>Minimum length of generated sequences. Defaults to 0.</p> <code>0</code> <code>max_gen_seq_length</code> <code>int</code> <p>Maximum length of generated sequences. Defaults to 48.</p> <code>48</code> <code>repetition_penalty</code> <code>float</code> <p>Penalty for repeated tokens. Defaults to 1.0.</p> <code>1.0</code> <code>no_repeat_ngram_size</code> <code>int</code> <p>Size of n-grams to avoid repeating. Defaults to 0.</p> <code>0</code> <code>early_stopping</code> <code>bool</code> <p>Whether to stop generation early. Defaults to True.</p> <code>True</code> <code>length_penalty</code> <code>float</code> <p>Penalty for longer sequences. Defaults to 1.0.</p> <code>1.0</code> <code>num_beam_groups</code> <code>int</code> <p>Number of beam groups for diverse beam search. Defaults to 1.</p> <code>1</code> <code>diversity_penalty</code> <code>float</code> <p>Penalty for diverse sequences in diverse beam search. Defaults to 0.0.</p> <code>0.0</code> <code>do_sample</code> <code>bool</code> <p>Whether to use sampling for generation. Defaults to False.</p> <code>False</code> <code>temperature</code> <code>float</code> <p>Sampling temperature. Defaults to 1.0.</p> <code>1.0</code> <code>top_k</code> <code>int</code> <p>Top-k value for sampling. Defaults to 50.</p> <code>50</code> <code>top_p</code> <code>float</code> <p>Top-p value for sampling. Defaults to 1.0.</p> <code>1.0</code> <p>Returns:</p> Name Type Description <code>GenericOutputs</code> <p>Generated sequences and their scores.</p> Source code in <code>src/unitorch/models/llama/modeling.py</code> <pre><code>@torch.no_grad()\ndef generate(\n    self,\n    input_ids: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 1,\n    decoder_end_token_id: Optional[Union[int, List[int]]] = 2,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n):\n\"\"\"\n    Generate text using the generation model.\n\n    Args:\n        input_ids: Input tensor of shape (batch_size, sequence_length).\n        num_beams (int, optional): Number of beams for beam search. Defaults to 5.\n        decoder_start_token_id (int, optional): The ID of the decoder start token. Defaults to 2.\n        decoder_end_token_id (int or List[int], optional): The ID(s) of the decoder end token(s). Defaults to 2.\n        num_return_sequences (int, optional): Number of generated sequences to return. Defaults to 1.\n        min_gen_seq_length (int, optional): Minimum length of generated sequences. Defaults to 0.\n        max_gen_seq_length (int, optional): Maximum length of generated sequences. Defaults to 48.\n        repetition_penalty (float, optional): Penalty for repeated tokens. Defaults to 1.0.\n        no_repeat_ngram_size (int, optional): Size of n-grams to avoid repeating. Defaults to 0.\n        early_stopping (bool, optional): Whether to stop generation early. Defaults to True.\n        length_penalty (float, optional): Penalty for longer sequences. Defaults to 1.0.\n        num_beam_groups (int, optional): Number of beam groups for diverse beam search. Defaults to 1.\n        diversity_penalty (float, optional): Penalty for diverse sequences in diverse beam search. Defaults to 0.0.\n        do_sample (bool, optional): Whether to use sampling for generation. Defaults to False.\n        temperature (float, optional): Sampling temperature. Defaults to 1.0.\n        top_k (int, optional): Top-k value for sampling. Defaults to 50.\n        top_p (float, optional): Top-p value for sampling. Defaults to 1.0.\n\n    Returns:\n        GenericOutputs: Generated sequences and their scores.\n    \"\"\"\n    input_seq_length = input_ids.size(1)\n    outputs = self.model.generate(\n        input_ids,\n        max_length=max_gen_seq_length + input_seq_length,\n        min_length=min_gen_seq_length + input_seq_length,\n        num_beams=num_beams,\n        do_sample=do_sample,\n        decoder_start_token_id=decoder_start_token_id,\n        no_repeat_ngram_size=no_repeat_ngram_size,\n        early_stopping=early_stopping,\n        length_penalty=length_penalty,\n        repetition_penalty=repetition_penalty,\n        num_return_sequences=num_return_sequences,\n        bos_token_id=decoder_start_token_id,\n        eos_token_id=decoder_end_token_id,\n        num_beam_groups=num_beam_groups,\n        diversity_penalty=diversity_penalty,\n        temperature=temperature,\n        top_k=top_k,\n        top_p=top_p,\n        return_dict_in_generate=True,\n        output_scores=True,\n    )\n\n    sequences = outputs.sequences.reshape(\n        -1, num_return_sequences, outputs.sequences.size(-1)\n    )\n    outputs.sequences = torch.zeros(\n        sequences.size(0), num_return_sequences, max_gen_seq_length\n    ).to(device=sequences.device)\n    outputs.sequences[:, :, : sequences.size(-1) - input_seq_length].copy_(\n        sequences[:, :, input_seq_length : sequences.size(-1)]\n    )\n\n    if num_return_sequences == 1:\n        outputs.sequences = outputs.sequences.reshape(-1, max_gen_seq_length)\n\n    return GenericOutputs(\n        sequences=outputs.sequences.long(),\n        sequences_scores=outputs.sequences_scores,\n    )\n</code></pre>",
             "title": "generate"
         },
         {
             "location": "models/mbart/",
             "text": "",
             "title": "unitorch.models.mbart"
         },
@@ -2242,15 +2277,75 @@
         {
             "location": "models/mbart/#unitorch.models.mbart.modeling.MBartForGeneration.forward",
             "text": "<pre><code>forward(\n    input_ids: torch.Tensor,\n    attention_mask: torch.Tensor,\n    decoder_input_ids: torch.Tensor,\n    decoder_attention_mask: torch.Tensor,\n)\n</code></pre> <p>Performs forward pass of the MBartForGeneration model.</p> <p>Parameters:</p> Name Type Description Default <code>input_ids</code> <code>torch.Tensor</code> <p>Tensor of input token IDs.</p> required <code>attention_mask</code> <code>torch.Tensor</code> <p>Tensor of attention mask.</p> required <code>decoder_input_ids</code> <code>torch.Tensor</code> <p>Tensor of decoder input token IDs.</p> required <code>decoder_attention_mask</code> <code>torch.Tensor</code> <p>Tensor of decoder attention mask.</p> required <p>Returns:</p> Type Description <code>torch.Tensor</code> <p>The model's logits.</p> Source code in <code>src/unitorch/models/mbart/modeling.py</code> <pre><code>def forward(\n    self,\n    input_ids: torch.Tensor,\n    attention_mask: torch.Tensor,\n    decoder_input_ids: torch.Tensor,\n    decoder_attention_mask: torch.Tensor,\n):\n\"\"\"\n    Performs forward pass of the MBartForGeneration model.\n\n    Args:\n        input_ids (torch.Tensor): Tensor of input token IDs.\n        attention_mask (torch.Tensor): Tensor of attention mask.\n        decoder_input_ids (torch.Tensor): Tensor of decoder input token IDs.\n        decoder_attention_mask (torch.Tensor): Tensor of decoder attention mask.\n\n    Returns:\n        (torch.Tensor):The model's logits.\n    \"\"\"\n    outputs = self.model(\n        input_ids=input_ids,\n        attention_mask=attention_mask,\n        decoder_input_ids=decoder_input_ids,\n        decoder_attention_mask=decoder_attention_mask,\n        return_dict=True,\n    )\n    logits = outputs.logits\n    return logits\n</code></pre>",
             "title": "forward"
         },
         {
             "location": "models/mbart/#unitorch.models.mbart.modeling.MBartForGeneration.generate",
-            "text": "<pre><code>generate(\n    input_ids: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 2,\n    decoder_end_token_id: Optional[int] = 2,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n)\n</code></pre> <p>Generates sequences using the MBartForGeneration model.</p> <p>Parameters:</p> Name Type Description Default <code>input_ids</code> <code>torch.Tensor</code> <p>The input token IDs.</p> required <code>num_beams</code> <code>int</code> <p>The number of beams for beam search. Defaults to 5.</p> <code>5</code> <code>decoder_start_token_id</code> <code>int</code> <p>The decoder's start token ID. Defaults to 2.</p> <code>2</code> <code>decoder_end_token_id</code> <code>int</code> <p>The decoder's end token ID. Defaults to 2.</p> <code>2</code> <code>num_return_sequences</code> <code>int</code> <p>The number of generated sequences to return. Defaults to 1.</p> <code>1</code> <code>min_gen_seq_length</code> <code>int</code> <p>The minimum length of the generated sequences. Defaults to 0.</p> <code>0</code> <code>max_gen_seq_length</code> <code>int</code> <p>The maximum length of the generated sequences. Defaults to 48.</p> <code>48</code> <code>repetition_penalty</code> <code>float</code> <p>The repetition penalty. Defaults to 1.0.</p> <code>1.0</code> <code>no_repeat_ngram_size</code> <code>int</code> <p>The size of n-grams to avoid repeating. Defaults to 0.</p> <code>0</code> <code>early_stopping</code> <code>bool</code> <p>Whether to stop generation early. Defaults to True.</p> <code>True</code> <code>length_penalty</code> <code>float</code> <p>The length penalty. Defaults to 1.0.</p> <code>1.0</code> <code>num_beam_groups</code> <code>int</code> <p>The number of beam groups for diverse beam search. Defaults to 1.</p> <code>1</code> <code>diversity_penalty</code> <code>float</code> <p>The diversity penalty. Defaults to 0.0.</p> <code>0.0</code> <code>do_sample</code> <code>bool</code> <p>Whether to use sampling for generation. Defaults to False.</p> <code>False</code> <code>temperature</code> <code>float</code> <p>The temperature for sampling. Defaults to 1.0.</p> <code>1.0</code> <code>top_k</code> <code>int</code> <p>The value for top-k sampling. Defaults to 50.</p> <code>50</code> <code>top_p</code> <code>float</code> <p>The value for top-p (nucleus) sampling. Defaults to 1.0.</p> <code>1.0</code> <p>Returns:</p> Name Type Description <code>GenericOutputs</code> <p>The generated sequences and their scores.</p> Source code in <code>src/unitorch/models/mbart/modeling.py</code> <pre><code>@torch.no_grad()\ndef generate(\n    self,\n    input_ids: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 2,\n    decoder_end_token_id: Optional[int] = 2,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n):\n\"\"\"\n    Generates sequences using the MBartForGeneration model.\n\n    Args:\n        input_ids: The input token IDs.\n        num_beams (int, optional): The number of beams for beam search. Defaults to 5.\n        decoder_start_token_id (int, optional): The decoder's start token ID. Defaults to 2.\n        decoder_end_token_id (int, optional): The decoder's end token ID. Defaults to 2.\n        num_return_sequences (int, optional): The number of generated sequences to return. Defaults to 1.\n        min_gen_seq_length (int, optional): The minimum length of the generated sequences. Defaults to 0.\n        max_gen_seq_length (int, optional): The maximum length of the generated sequences. Defaults to 48.\n        repetition_penalty (float, optional): The repetition penalty. Defaults to 1.0.\n        no_repeat_ngram_size (int, optional): The size of n-grams to avoid repeating. Defaults to 0.\n        early_stopping (bool, optional): Whether to stop generation early. Defaults to True.\n        length_penalty (float, optional): The length penalty. Defaults to 1.0.\n        num_beam_groups (int, optional): The number of beam groups for diverse beam search. Defaults to 1.\n        diversity_penalty (float, optional): The diversity penalty. Defaults to 0.0.\n        do_sample (bool, optional): Whether to use sampling for generation. Defaults to False.\n        temperature (float, optional): The temperature for sampling. Defaults to 1.0.\n        top_k (int, optional): The value for top-k sampling. Defaults to 50.\n        top_p (float, optional): The value for top-p (nucleus) sampling. Defaults to 1.0.\n\n    Returns:\n        GenericOutputs: The generated sequences and their scores.\n    \"\"\"\n    outputs = self.model.generate(\n        input_ids,\n        max_length=max_gen_seq_length,\n        min_length=min_gen_seq_length,\n        num_beams=num_beams,\n        do_sample=do_sample,\n        decoder_start_token_id=decoder_start_token_id,\n        no_repeat_ngram_size=no_repeat_ngram_size,\n        early_stopping=early_stopping,\n        length_penalty=length_penalty,\n        repetition_penalty=repetition_penalty,\n        num_return_sequences=num_return_sequences,\n        bos_token_id=decoder_start_token_id,\n        eos_token_id=decoder_end_token_id,\n        num_beam_groups=num_beam_groups,\n        diversity_penalty=diversity_penalty,\n        temperature=temperature,\n        top_k=top_k,\n        top_p=top_p,\n        return_dict_in_generate=True,\n        output_scores=True,\n    )\n\n    sequences = outputs.sequences.reshape(\n        -1, num_return_sequences, outputs.sequences.size(-1)\n    )\n    outputs.sequences = torch.zeros(\n        sequences.size(0), num_return_sequences, max_gen_seq_length\n    ).to(device=sequences.device)\n    outputs.sequences[:, :, : sequences.size(-1)].copy_(sequences)\n\n    if num_return_sequences == 1:\n        outputs.sequences = outputs.sequences.reshape(-1, max_gen_seq_length)\n\n    return GenericOutputs(\n        sequences=outputs.sequences,\n        sequences_scores=outputs.sequences_scores,\n    )\n</code></pre>",
+            "text": "<pre><code>generate(\n    input_ids: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 2,\n    decoder_end_token_id: Optional[\n        Union[int, List[int]]\n    ] = 2,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n)\n</code></pre> <p>Generates sequences using the MBartForGeneration model.</p> <p>Parameters:</p> Name Type Description Default <code>input_ids</code> <code>torch.Tensor</code> <p>The input token IDs.</p> required <code>num_beams</code> <code>int</code> <p>The number of beams for beam search. Defaults to 5.</p> <code>5</code> <code>decoder_start_token_id</code> <code>int</code> <p>The decoder's start token ID. Defaults to 2.</p> <code>2</code> <code>decoder_end_token_id</code> <code>int or List[int]</code> <p>The decoder's end token ID. Defaults to 2.</p> <code>2</code> <code>num_return_sequences</code> <code>int</code> <p>The number of generated sequences to return. Defaults to 1.</p> <code>1</code> <code>min_gen_seq_length</code> <code>int</code> <p>The minimum length of the generated sequences. Defaults to 0.</p> <code>0</code> <code>max_gen_seq_length</code> <code>int</code> <p>The maximum length of the generated sequences. Defaults to 48.</p> <code>48</code> <code>repetition_penalty</code> <code>float</code> <p>The repetition penalty. Defaults to 1.0.</p> <code>1.0</code> <code>no_repeat_ngram_size</code> <code>int</code> <p>The size of n-grams to avoid repeating. Defaults to 0.</p> <code>0</code> <code>early_stopping</code> <code>bool</code> <p>Whether to stop generation early. Defaults to True.</p> <code>True</code> <code>length_penalty</code> <code>float</code> <p>The length penalty. Defaults to 1.0.</p> <code>1.0</code> <code>num_beam_groups</code> <code>int</code> <p>The number of beam groups for diverse beam search. Defaults to 1.</p> <code>1</code> <code>diversity_penalty</code> <code>float</code> <p>The diversity penalty. Defaults to 0.0.</p> <code>0.0</code> <code>do_sample</code> <code>bool</code> <p>Whether to use sampling for generation. Defaults to False.</p> <code>False</code> <code>temperature</code> <code>float</code> <p>The temperature for sampling. Defaults to 1.0.</p> <code>1.0</code> <code>top_k</code> <code>int</code> <p>The value for top-k sampling. Defaults to 50.</p> <code>50</code> <code>top_p</code> <code>float</code> <p>The value for top-p (nucleus) sampling. Defaults to 1.0.</p> <code>1.0</code> <p>Returns:</p> Name Type Description <code>GenericOutputs</code> <p>The generated sequences and their scores.</p> Source code in <code>src/unitorch/models/mbart/modeling.py</code> <pre><code>@torch.no_grad()\ndef generate(\n    self,\n    input_ids: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 2,\n    decoder_end_token_id: Optional[Union[int, List[int]]] = 2,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n):\n\"\"\"\n    Generates sequences using the MBartForGeneration model.\n\n    Args:\n        input_ids: The input token IDs.\n        num_beams (int, optional): The number of beams for beam search. Defaults to 5.\n        decoder_start_token_id (int, optional): The decoder's start token ID. Defaults to 2.\n        decoder_end_token_id (int or List[int], optional): The decoder's end token ID. Defaults to 2.\n        num_return_sequences (int, optional): The number of generated sequences to return. Defaults to 1.\n        min_gen_seq_length (int, optional): The minimum length of the generated sequences. Defaults to 0.\n        max_gen_seq_length (int, optional): The maximum length of the generated sequences. Defaults to 48.\n        repetition_penalty (float, optional): The repetition penalty. Defaults to 1.0.\n        no_repeat_ngram_size (int, optional): The size of n-grams to avoid repeating. Defaults to 0.\n        early_stopping (bool, optional): Whether to stop generation early. Defaults to True.\n        length_penalty (float, optional): The length penalty. Defaults to 1.0.\n        num_beam_groups (int, optional): The number of beam groups for diverse beam search. Defaults to 1.\n        diversity_penalty (float, optional): The diversity penalty. Defaults to 0.0.\n        do_sample (bool, optional): Whether to use sampling for generation. Defaults to False.\n        temperature (float, optional): The temperature for sampling. Defaults to 1.0.\n        top_k (int, optional): The value for top-k sampling. Defaults to 50.\n        top_p (float, optional): The value for top-p (nucleus) sampling. Defaults to 1.0.\n\n    Returns:\n        GenericOutputs: The generated sequences and their scores.\n    \"\"\"\n    outputs = self.model.generate(\n        input_ids,\n        max_length=max_gen_seq_length,\n        min_length=min_gen_seq_length,\n        num_beams=num_beams,\n        do_sample=do_sample,\n        decoder_start_token_id=decoder_start_token_id,\n        no_repeat_ngram_size=no_repeat_ngram_size,\n        early_stopping=early_stopping,\n        length_penalty=length_penalty,\n        repetition_penalty=repetition_penalty,\n        num_return_sequences=num_return_sequences,\n        bos_token_id=decoder_start_token_id,\n        eos_token_id=decoder_end_token_id,\n        num_beam_groups=num_beam_groups,\n        diversity_penalty=diversity_penalty,\n        temperature=temperature,\n        top_k=top_k,\n        top_p=top_p,\n        return_dict_in_generate=True,\n        output_scores=True,\n    )\n\n    sequences = outputs.sequences.reshape(\n        -1, num_return_sequences, outputs.sequences.size(-1)\n    )\n    outputs.sequences = torch.zeros(\n        sequences.size(0), num_return_sequences, max_gen_seq_length\n    ).to(device=sequences.device)\n    outputs.sequences[:, :, : sequences.size(-1)].copy_(sequences)\n\n    if num_return_sequences == 1:\n        outputs.sequences = outputs.sequences.reshape(-1, max_gen_seq_length)\n\n    return GenericOutputs(\n        sequences=outputs.sequences,\n        sequences_scores=outputs.sequences_scores,\n    )\n</code></pre>",
+            "title": "generate"
+        },
+        {
+            "location": "models/minigpt4/",
+            "text": "",
+            "title": "unitorch.models.minigpt4"
+        },
+        {
+            "location": "models/minigpt4/#minigpt4blip2llamaprocessor",
+            "text": "<p>         Bases: <code>HfTextClassificationProcessor</code>, <code>HfImageClassificationProcessor</code>, <code>HfTextGenerationProcessor</code></p> <p>Initialize the LlamaProcessor.</p> <p>Parameters:</p> Name Type Description Default <code>vocab_file</code> <code>str</code> <p>Path to the vocabulary file.</p> required <code>max_seq_length</code> <code>int</code> <p>Maximum sequence length for text classification. Defaults to 128.</p> required <code>max_gen_seq_length</code> <code>int</code> <p>Maximum sequence length for text generation. Defaults to 48.</p> <code>48</code> Source code in <code>src/unitorch/models/minigpt4/processing.py</code> <pre><code>def __init__(\n    self,\n    vocab_file: str,\n    vision_config_path: str,\n    max_prefix_seq_length: Optional[int] = 32,\n    max_suffix_seq_length: Optional[int] = 128,\n    max_gen_seq_length: Optional[int] = 48,\n):\n\"\"\"\n    Initialize the LlamaProcessor.\n\n    Args:\n        vocab_file (str): Path to the vocabulary file.\n        max_seq_length (int, optional): Maximum sequence length for text classification. Defaults to 128.\n        max_gen_seq_length (int, optional): Maximum sequence length for text generation. Defaults to 48.\n    \"\"\"\n    tokenizer = LlamaTokenizer(vocab_file=vocab_file)\n    tokenizer.cls_token = tokenizer.bos_token\n    tokenizer.sep_token = tokenizer.eos_token\n    tokenizer.pad_token = tokenizer.unk_token\n    tokenizer.cls_token_id = tokenizer.bos_token_id\n    tokenizer.sep_token_id = tokenizer.eos_token_id\n    tokenizer.pad_token_id = tokenizer.unk_token_id\n    vision_processor = BlipImageProcessor.from_json_file(vision_config_path)\n    HfTextClassificationProcessor.__init__(\n        self,\n        tokenizer=tokenizer,\n        max_seq_length=max_prefix_seq_length,\n    )\n    HfTextGenerationProcessor.__init__(\n        self,\n        tokenizer=tokenizer,\n        max_seq_length=max_prefix_seq_length,\n        max_gen_seq_length=max_gen_seq_length,\n    )\n    HfImageClassificationProcessor.__init__(self, vision_processor=vision_processor)\n    self.max_prefix_seq_length = max_prefix_seq_length\n    self.max_suffix_seq_length = max_suffix_seq_length\n</code></pre>",
+            "title": "MiniGPT4Blip2LlamaProcessor"
+        },
+        {
+            "location": "models/minigpt4/#unitorch.models.minigpt4.processing.MiniGPT4Blip2LlamaProcessor.generation",
+            "text": "<pre><code>generation(\n    prefix_text: str,\n    suffix_text: str,\n    text_pair: str,\n    image: Image.Image,\n    max_prefix_seq_length: Optional[int] = None,\n    max_suffix_seq_length: Optional[int] = None,\n    max_gen_seq_length: Optional[int] = None,\n)\n</code></pre> <p>Process text for generation.</p> <p>Parameters:</p> Name Type Description Default <code>text</code> <code>str</code> <p>Input text.</p> required <code>text_pair</code> <code>str</code> <p>Input text pair.</p> required <code>max_seq_length</code> <code>int</code> <p>Maximum sequence length. Defaults to None.</p> required <code>max_gen_seq_length</code> <code>int</code> <p>Maximum generation sequence length. Defaults to None.</p> <code>None</code> <p>Returns:</p> Name Type Description <code>GenericOutputs</code> <p>Processed input_ids, attention_mask, input_ids_label, and attention_mask_label tensors.</p> Source code in <code>src/unitorch/models/minigpt4/processing.py</code> <pre><code>def generation(\n    self,\n    prefix_text: str,\n    suffix_text: str,\n    text_pair: str,\n    image: Image.Image,\n    max_prefix_seq_length: Optional[int] = None,\n    max_suffix_seq_length: Optional[int] = None,\n    max_gen_seq_length: Optional[int] = None,\n):\n\"\"\"\n    Process text for generation.\n\n    Args:\n        text (str): Input text.\n        text_pair (str): Input text pair.\n        max_seq_length (int, optional): Maximum sequence length. Defaults to None.\n        max_gen_seq_length (int, optional): Maximum generation sequence length. Defaults to None.\n\n    Returns:\n        GenericOutputs: Processed input_ids, attention_mask, input_ids_label, and attention_mask_label tensors.\n    \"\"\"\n    max_prefix_seq_length = pop_value(\n        max_prefix_seq_length,\n        self.max_prefix_seq_length,\n    )\n    max_suffix_seq_length = pop_value(\n        max_suffix_seq_length,\n        self.max_suffix_seq_length,\n    )\n    max_gen_seq_length = pop_value(\n        max_gen_seq_length,\n        self.max_gen_seq_length,\n    )\n\n    prefix_tokens = self.tokenizer.tokenize(str(prefix_text))[\n        : max_prefix_seq_length - 1\n    ]\n    suffix_tokens = self.tokenizer.tokenize(str(suffix_text))[\n        :max_suffix_seq_length\n    ]\n\n    prefix_tokens = [self.bos_token] + prefix_tokens\n    prefix_padding = [self.pad_token] * (max_prefix_seq_length - len(prefix_tokens))\n    prefix_attention_mask = [0] * len(prefix_padding) + [1] * len(prefix_tokens)\n    prefix_tokens = prefix_padding + prefix_tokens\n    prefix_input_ids = self.tokenizer.convert_tokens_to_ids(prefix_tokens)\n\n    suffix_padding = [self.pad_token] * (max_suffix_seq_length - len(suffix_tokens))\n    suffix_attention_mask = [0] * len(suffix_padding) + [1] * len(suffix_tokens)\n    suffix_tokens = suffix_padding + suffix_tokens\n    suffix_input_ids = self.tokenizer.convert_tokens_to_ids(suffix_tokens)\n\n    tokens_pair = self.tokenizer.tokenize(str(text_pair))[\n        : max_gen_seq_length - 1\n    ] + [self.eos_token]\n\n    padding_pair = [self.pad_token] * (max_gen_seq_length - len(tokens_pair))\n    input_ids_pair = self.tokenizer.convert_tokens_to_ids(\n        tokens_pair + padding_pair\n    )\n    attention_mask_pair = [1] * len(tokens_pair) + [0] * len(padding_pair)\n\n    tokens_label = tokens_pair + [self.pad_token] * (\n        max_gen_seq_length - len(tokens_pair) + 1\n    )\n    input_ids_label = self.tokenizer.convert_tokens_to_ids(tokens_label)\n    input_ids_label = [0] * (max_suffix_seq_length - 1) + input_ids_label\n    attention_mask_label = [1] * len(tokens_pair) + [0] * (\n        max_gen_seq_length - len(tokens_pair) + 1\n    )\n    attention_mask_label = [0] * (max_suffix_seq_length - 1) + attention_mask_label\n\n    outputs = HfImageClassificationProcessor.classification(\n        self,\n        image=image,\n    )\n\n    return GenericOutputs(\n        prefix_input_ids=torch.tensor(prefix_input_ids, dtype=torch.long),\n        prefix_attention_mask=torch.tensor(prefix_attention_mask, dtype=torch.long),\n        suffix_input_ids=torch.tensor(suffix_input_ids, dtype=torch.long),\n        suffix_attention_mask=torch.tensor(suffix_attention_mask, dtype=torch.long),\n        input_ids_pair=torch.tensor(input_ids_pair, dtype=torch.long),\n        attention_mask_pair=torch.tensor(attention_mask_pair, dtype=torch.long),\n        input_ids_label=torch.tensor(input_ids_label, dtype=torch.long),\n        attention_mask_label=torch.tensor(attention_mask_label, dtype=torch.long),\n        pixel_values=outputs.pixel_values,\n    )\n</code></pre>",
+            "title": "generation"
+        },
+        {
+            "location": "models/minigpt4/#unitorch.models.minigpt4.processing.MiniGPT4Blip2LlamaProcessor.generation_inputs",
+            "text": "<pre><code>generation_inputs(\n    prefix_text: str,\n    suffix_text: str,\n    image: Image.Image,\n    max_prefix_seq_length: Optional[int] = None,\n    max_suffix_seq_length: Optional[int] = None,\n)\n</code></pre> <p>Process text for generation inputs.</p> <p>Parameters:</p> Name Type Description Default <code>text</code> <code>str</code> <p>Input text.</p> required <code>max_seq_length</code> <code>int</code> <p>Maximum sequence length. Defaults to None.</p> required <p>Returns:</p> Name Type Description <code>GenericOutputs</code> <p>Processed input_ids tensor.</p> Source code in <code>src/unitorch/models/minigpt4/processing.py</code> <pre><code>def generation_inputs(\n    self,\n    prefix_text: str,\n    suffix_text: str,\n    image: Image.Image,\n    max_prefix_seq_length: Optional[int] = None,\n    max_suffix_seq_length: Optional[int] = None,\n):\n\"\"\"\n    Process text for generation inputs.\n\n    Args:\n        text (str): Input text.\n        max_seq_length (int, optional): Maximum sequence length. Defaults to None.\n\n    Returns:\n        GenericOutputs: Processed input_ids tensor.\n    \"\"\"\n    max_prefix_seq_length = pop_value(\n        max_prefix_seq_length,\n        self.max_prefix_seq_length,\n    )\n    max_suffix_seq_length = pop_value(\n        max_suffix_seq_length,\n        self.max_suffix_seq_length,\n    )\n    prefix_tokens = self.tokenizer.tokenize(str(prefix_text))[\n        : max_prefix_seq_length - 1\n    ]\n    suffix_tokens = self.tokenizer.tokenize(str(suffix_text))[\n        :max_suffix_seq_length\n    ]\n\n    prefix_tokens = [self.bos_token] + prefix_tokens\n    prefix_padding = [self.pad_token] * (max_prefix_seq_length - len(prefix_tokens))\n    prefix_tokens = prefix_padding + prefix_tokens\n    prefix_input_ids = self.tokenizer.convert_tokens_to_ids(prefix_tokens)\n\n    suffix_padding = [self.pad_token] * (max_suffix_seq_length - len(suffix_tokens))\n    suffix_tokens = suffix_padding + suffix_tokens\n    suffix_input_ids = self.tokenizer.convert_tokens_to_ids(suffix_tokens)\n\n    outputs = HfImageClassificationProcessor.classification(\n        self,\n        image=image,\n    )\n\n    return GenericOutputs(\n        prefix_input_ids=torch.tensor(prefix_input_ids, dtype=torch.long),\n        suffix_input_ids=torch.tensor(suffix_input_ids, dtype=torch.long),\n        pixel_values=outputs.pixel_values,\n    )\n</code></pre>",
+            "title": "generation_inputs"
+        },
+        {
+            "location": "models/minigpt4/#unitorch.models.minigpt4.processing.MiniGPT4Blip2LlamaProcessor.generation_labels",
+            "text": "<pre><code>generation_labels(\n    text: str, max_gen_seq_length: Optional[int] = None\n)\n</code></pre> <p>Process text for generation labels.</p> <p>Parameters:</p> Name Type Description Default <code>text</code> <code>str</code> <p>Input text.</p> required <code>max_gen_seq_length</code> <code>int</code> <p>Maximum generation sequence length. Defaults to None.</p> <code>None</code> <p>Returns:</p> Name Type Description <code>GenericOutputs</code> <p>Processed input_ids and attention_mask tensors.</p> Source code in <code>src/unitorch/models/minigpt4/processing.py</code> <pre><code>def generation_labels(\n    self,\n    text: str,\n    max_gen_seq_length: Optional[int] = None,\n):\n\"\"\"\n    Process text for generation labels.\n\n    Args:\n        text (str): Input text.\n        max_gen_seq_length (int, optional): Maximum generation sequence length. Defaults to None.\n\n    Returns:\n        GenericOutputs: Processed input_ids and attention_mask tensors.\n    \"\"\"\n    max_gen_seq_length = pop_value(\n        max_gen_seq_length,\n        self.max_gen_seq_length,\n    )\n    tokens = self.tokenizer.tokenize(str(text))[: max_gen_seq_length - 1] + [\n        self.eos_token\n    ]\n    padding = [self.pad_token] * (max_gen_seq_length - len(tokens))\n    input_ids = self.tokenizer.convert_tokens_to_ids(tokens)\n    attention_mask = [1] * len(input_ids)\n\n    padding = [0] * (max_gen_seq_length - len(input_ids))\n    input_ids += [self.pad_token_id] * len(padding)\n    attention_mask += padding\n\n    assert len(input_ids) == max_gen_seq_length\n    assert len(attention_mask) == max_gen_seq_length\n    return GenericOutputs(\n        input_ids=torch.tensor(input_ids, dtype=torch.long),\n        attention_mask=torch.tensor(attention_mask, dtype=torch.long),\n    )\n</code></pre>",
+            "title": "generation_labels"
+        },
+        {
+            "location": "models/minigpt4/#unitorch.models.minigpt4.processing.MiniGPT4Blip2LlamaProcessor.prompt",
+            "text": "<pre><code>prompt(\n    prefix_text: str,\n    suffix_text: str,\n    image: Image.Image,\n    max_prefix_seq_length: Optional[int] = None,\n    max_suffix_seq_length: Optional[int] = None,\n)\n</code></pre> <p>Process text as a prompt.</p> <p>Parameters:</p> Name Type Description Default <code>text</code> <code>str</code> <p>Input text.</p> required <code>max_seq_length</code> <code>int</code> <p>Maximum sequence length. Defaults to None.</p> required <p>Returns:</p> Name Type Description <code>GenericOutputs</code> <p>Processed input_ids tensor.</p> Source code in <code>src/unitorch/models/minigpt4/processing.py</code> <pre><code>def prompt(\n    self,\n    prefix_text: str,\n    suffix_text: str,\n    image: Image.Image,\n    max_prefix_seq_length: Optional[int] = None,\n    max_suffix_seq_length: Optional[int] = None,\n):\n\"\"\"\n    Process text as a prompt.\n\n    Args:\n        text (str): Input text.\n        max_seq_length (int, optional): Maximum sequence length. Defaults to None.\n\n    Returns:\n        GenericOutputs: Processed input_ids tensor.\n    \"\"\"\n    max_prefix_seq_length = pop_value(\n        max_prefix_seq_length,\n        self.max_prefix_seq_length,\n    )\n    max_suffix_seq_length = pop_value(\n        max_suffix_seq_length,\n        self.max_suffix_seq_length,\n    )\n    prefix_tokens = self.tokenizer.tokenize(str(prefix_text))[\n        : max_prefix_seq_length - 1\n    ]\n    suffix_tokens = self.tokenizer.tokenize(str(suffix_text))[\n        :max_suffix_seq_length\n    ]\n\n    prefix_tokens = [self.bos_token] + prefix_tokens\n    prefix_padding = [self.pad_token] * (max_prefix_seq_length - len(prefix_tokens))\n    prefix_tokens = prefix_padding + prefix_tokens\n    prefix_input_ids = self.tokenizer.convert_tokens_to_ids(prefix_tokens)\n\n    suffix_padding = [self.pad_token] * (max_suffix_seq_length - len(suffix_tokens))\n    suffix_tokens = suffix_padding + suffix_tokens\n    suffix_input_ids = self.tokenizer.convert_tokens_to_ids(suffix_tokens)\n\n    outputs = HfImageClassificationProcessor.classification(\n        self,\n        image=image,\n    )\n\n    return GenericOutputs(\n        prefix_input_ids=torch.tensor(prefix_input_ids, dtype=torch.long),\n        suffix_input_ids=torch.tensor(suffix_input_ids, dtype=torch.long),\n        pixel_values=outputs.pixel_values,\n    )\n</code></pre>",
+            "title": "prompt"
+        },
+        {
+            "location": "models/minigpt4/#minigpt4blip2llamamodel",
+            "text": "<p>         Bases: <code>nn.Module</code></p> <p>MiniGPT4Blip2LlamaModel is a model that combines the Blip2VisionModel, Blip2QFormerModel, and LlamaForCausalLM models for generation. It inherits from the nn.Module class.</p> <p>Initializes a MiniGPT4Blip2LlamaModel instance.</p> <p>Parameters:</p> Name Type Description Default <code>blip2_config</code> <code>Blip2Config</code> <p>The configuration for the Blip2 model.</p> required <code>llama_config</code> <code>LlamaConfig</code> <p>The configuration for the Llama model.</p> required Source code in <code>src/unitorch/models/minigpt4/modeling.py</code> <pre><code>def __init__(\n    self,\n    blip2_config: Blip2Config,\n    llama_config: LlamaConfig,\n):\n\"\"\"\n    Initializes a MiniGPT4Blip2LlamaModel instance.\n\n    Args:\n        blip2_config (Blip2Config): The configuration for the Blip2 model.\n        llama_config (LlamaConfig): The configuration for the Llama model.\n    \"\"\"\n    super().__init__()\n    self.blip2_config = blip2_config\n    self.vision_model = Blip2VisionModel(self.blip2_config.vision_config)\n\n    self.query_tokens = nn.Parameter(\n        torch.zeros(\n            1,\n            self.blip2_config.num_query_tokens,\n            self.blip2_config.qformer_config.hidden_size,\n        )\n    )\n    self.qformer = Blip2QFormerModel(self.blip2_config.qformer_config)\n\n    self.llama_config = llama_config\n    self.language_projection = nn.Linear(\n        self.blip2_config.qformer_config.hidden_size, self.llama_config.hidden_size\n    )\n    self.llama = LlamaForCausalLM(self.llama_config)\n</code></pre>",
+            "title": "MiniGPT4Blip2LlamaModel"
+        },
+        {
+            "location": "models/minigpt4/#unitorch.models.minigpt4.modeling.MiniGPT4Blip2LlamaModel.forward",
+            "text": "<pre><code>forward(\n    pixel_values: torch.Tensor,\n    prefix_input_ids: torch.Tensor,\n    suffix_input_ids: torch.Tensor,\n    decoder_input_ids: torch.Tensor,\n    prefix_attention_mask: Optional[torch.Tensor] = None,\n    suffix_attention_mask: Optional[torch.Tensor] = None,\n    decoder_attention_mask: Optional[torch.Tensor] = None,\n)\n</code></pre> <p>Performs a forward pass of the MiniGPT4Blip2LlamaModel.</p> <p>Parameters:</p> Name Type Description Default <code>pixel_values</code> <code>torch.Tensor</code> <p>The pixel values.</p> required <code>prefix_input_ids</code> <code>torch.Tensor</code> <p>The input IDs for the prefix tokens.</p> required <code>suffix_input_ids</code> <code>torch.Tensor</code> <p>The input IDs for the suffix tokens.</p> required <code>decoder_input_ids</code> <code>torch.Tensor</code> <p>The input IDs for the decoder tokens.</p> required <code>prefix_attention_mask</code> <code>torch.Tensor</code> <p>The attention mask for the prefix tokens.</p> <code>None</code> <code>suffix_attention_mask</code> <code>torch.Tensor</code> <p>The attention mask for the suffix tokens.</p> <code>None</code> <code>decoder_attention_mask</code> <code>torch.Tensor</code> <p>The attention mask for the decoder tokens.</p> <code>None</code> <p>Returns:</p> Name Type Description <code>outputs</code> <p>The model outputs.</p> Source code in <code>src/unitorch/models/minigpt4/modeling.py</code> <pre><code>def forward(\n    self,\n    pixel_values: torch.Tensor,\n    prefix_input_ids: torch.Tensor,\n    suffix_input_ids: torch.Tensor,\n    decoder_input_ids: torch.Tensor,\n    prefix_attention_mask: Optional[torch.Tensor] = None,\n    suffix_attention_mask: Optional[torch.Tensor] = None,\n    decoder_attention_mask: Optional[torch.Tensor] = None,\n):\n\"\"\"\n    Performs a forward pass of the MiniGPT4Blip2LlamaModel.\n\n    Args:\n        pixel_values (torch.Tensor): The pixel values.\n        prefix_input_ids (torch.Tensor): The input IDs for the prefix tokens.\n        suffix_input_ids (torch.Tensor): The input IDs for the suffix tokens.\n        decoder_input_ids (torch.Tensor): The input IDs for the decoder tokens.\n        prefix_attention_mask (torch.Tensor, optional): The attention mask for the prefix tokens.\n        suffix_attention_mask (torch.Tensor, optional): The attention mask for the suffix tokens.\n        decoder_attention_mask (torch.Tensor, optional): The attention mask for the decoder tokens.\n\n    Returns:\n        outputs: The model outputs.\n    \"\"\"\n    vision_outputs = self.vision_model(\n        pixel_values=pixel_values,\n    )\n    image_embeds = vision_outputs[0]\n    image_attention_mask = torch.ones(\n        image_embeds.size()[:-1], dtype=torch.long, device=image_embeds.device\n    )\n\n    query_tokens = self.query_tokens.expand(image_embeds.shape[0], -1, -1)\n    query_outputs = self.qformer(\n        query_embeds=query_tokens,\n        encoder_hidden_states=image_embeds,\n        encoder_attention_mask=image_attention_mask,\n    )\n    query_embeds = query_outputs[0]\n\n    language_model_inputs = self.language_projection(query_embeds)\n    language_model_attention_mask = torch.ones(\n        language_model_inputs.size()[:-1],\n        dtype=torch.long,\n        device=language_model_inputs.device,\n    )\n    prefix_inputs_embeds = self.llama.get_input_embeddings()(prefix_input_ids)\n    suffix_inputs_embeds = self.llama.get_input_embeddings()(suffix_input_ids)\n    decoder_input_embeds = self.llama.get_input_embeddings()(decoder_input_ids)\n    inputs_embeds = torch.cat(\n        [\n            prefix_inputs_embeds,\n            language_model_inputs,\n            suffix_inputs_embeds,\n            decoder_input_embeds,\n        ],\n        dim=1,\n    )\n    expected_device = language_model_attention_mask.device\n\n    if prefix_attention_mask is None:\n        prefix_attention_mask = torch.ones(\n            prefix_inputs_embeds.size()[:-1],\n            dtype=torch.long,\n            device=expected_device,\n        )\n\n    if suffix_attention_mask is None:\n        suffix_attention_mask = torch.ones(\n            suffix_inputs_embeds.size()[:-1],\n            dtype=torch.long,\n            device=expected_device,\n        )\n\n    if decoder_attention_mask is None:\n        decoder_attention_mask = torch.ones(\n            decoder_input_embeds.size()[:-1],\n            dtype=torch.long,\n            device=expected_device,\n        )\n\n    attention_mask = torch.cat(\n        [\n            prefix_attention_mask,\n            language_model_attention_mask,\n            suffix_attention_mask,\n            decoder_attention_mask.to(expected_device),\n        ],\n        dim=1,\n    )\n    outputs = self.llama(\n        inputs_embeds=inputs_embeds,\n        attention_mask=attention_mask,\n        return_dict=True,\n    )\n    return outputs\n</code></pre>",
+            "title": "forward"
+        },
+        {
+            "location": "models/minigpt4/#unitorch.models.minigpt4.modeling.MiniGPT4Blip2LlamaModel.generate",
+            "text": "<pre><code>generate(\n    pixel_values: torch.FloatTensor,\n    prefix_input_ids: Optional[torch.Tensor] = None,\n    suffix_input_ids: Optional[torch.Tensor] = None,\n    **generate_kwargs: Optional[torch.Tensor]\n)\n</code></pre> <p>Generates sequences using the MiniGPT4Blip2LlamaModel.</p> <p>Parameters:</p> Name Type Description Default <code>pixel_values</code> <code>torch.FloatTensor</code> <p>The pixel values.</p> required <code>prefix_input_ids</code> <code>torch.Tensor</code> <p>The input IDs for the prefix tokens. Defaults to None.</p> <code>None</code> <code>suffix_input_ids</code> <code>torch.Tensor</code> <p>The input IDs for the suffix tokens. Defaults to None.</p> <code>None</code> <code>**generate_kwargs</code> <p>Additional keyword arguments for sequence generation.</p> <code>{}</code> <p>Returns:</p> Name Type Description <code>outputs</code> <p>The generation outputs.</p> Source code in <code>src/unitorch/models/minigpt4/modeling.py</code> <pre><code>def generate(\n    self,\n    pixel_values: torch.FloatTensor,\n    prefix_input_ids: Optional[torch.Tensor] = None,\n    suffix_input_ids: Optional[torch.Tensor] = None,\n    **generate_kwargs,\n):\n\"\"\"\n    Generates sequences using the MiniGPT4Blip2LlamaModel.\n\n    Args:\n        pixel_values (torch.FloatTensor): The pixel values.\n        prefix_input_ids (torch.Tensor, optional): The input IDs for the prefix tokens. Defaults to None.\n        suffix_input_ids (torch.Tensor, optional): The input IDs for the suffix tokens. Defaults to None.\n        **generate_kwargs: Additional keyword arguments for sequence generation.\n\n    Returns:\n        outputs: The generation outputs.\n    \"\"\"\n    vision_outputs = self.vision_model(\n        pixel_values=pixel_values,\n    )\n    image_embeds = vision_outputs[0]\n    image_attention_mask = torch.ones(\n        image_embeds.size()[:-1], dtype=torch.long, device=image_embeds.device\n    )\n\n    query_tokens = self.query_tokens.expand(image_embeds.shape[0], -1, -1)\n    query_outputs = self.qformer(\n        query_embeds=query_tokens,\n        encoder_hidden_states=image_embeds,\n        encoder_attention_mask=image_attention_mask,\n    )\n    query_embeds = query_outputs[0]\n\n    inputs_embeds = self.language_projection(query_embeds)\n\n    attention_mask = torch.ones(\n        inputs_embeds.size(0), inputs_embeds.size(1), dtype=torch.bool\n    ).to(inputs_embeds.device)\n\n    if prefix_input_ids is not None:\n        prefix_inputs_embeds = self.llama.get_input_embeddings()(prefix_input_ids)\n        inputs_embeds = torch.cat([prefix_inputs_embeds, inputs_embeds], dim=1)\n        attention_mask = torch.cat(\n            [prefix_input_ids.ne(self.blip2_config.pad_token_id), attention_mask],\n            dim=1,\n        )\n\n    if suffix_input_ids is not None:\n        suffix_inputs_embeds = self.llama.get_input_embeddings()(suffix_input_ids)\n        inputs_embeds = torch.cat([inputs_embeds, suffix_inputs_embeds], dim=1)\n        attention_mask = torch.cat(\n            [attention_mask, suffix_input_ids.ne(self.blip2_config.pad_token_id)],\n            dim=1,\n        )\n\n    outputs = self.llama.generate(\n        inputs_embeds=inputs_embeds,\n        attention_mask=attention_mask,\n        **generate_kwargs,\n    )\n\n    return outputs\n</code></pre>",
+            "title": "generate"
+        },
+        {
+            "location": "models/minigpt4/#minigpt4blip2llamaforgeneration",
+            "text": "<p>         Bases: <code>GenericModel</code></p> <p>MiniGPT4Blip2LlamaForGeneration is a generation model that combines the MiniGPT4Blip2LlamaModel with generation capabilities. It inherits from the GenericModel class.</p> <p>Initializes a MiniGPT4Blip2LlamaForGeneration instance.</p> <p>Parameters:</p> Name Type Description Default <code>blip2_config_path</code> <code>str</code> <p>The path to the Blip2 model configuration file.</p> required <code>llama_config_path</code> <code>str</code> <p>The path to the Llama model configuration file.</p> required <code>pad_token_id</code> <code>int</code> <p>The ID of the padding token. Defaults to 0.</p> <code>0</code> <code>freeze_vision_model</code> <code>bool</code> <p>Whether to freeze the parameters of the vision model. Defaults to True.</p> <code>True</code> <code>freeze_qformer_model</code> <code>bool</code> <p>Whether to freeze the parameters of the qformer model. Defaults to True.</p> <code>True</code> <code>freeze_llama_model</code> <code>bool</code> <p>Whether to freeze the parameters of the llama model. Defaults to True.</p> <code>True</code> <code>gradient_checkpointing</code> <code>bool</code> <p>Whether to use gradient checkpointing. Defaults to False.</p> <code>False</code> Source code in <code>src/unitorch/models/minigpt4/modeling.py</code> <pre><code>def __init__(\n    self,\n    blip2_config_path: str,\n    llama_config_path: str,\n    pad_token_id: Optional[int] = 0,\n    freeze_vision_model: Optional[bool] = True,\n    freeze_qformer_model: Optional[bool] = True,\n    freeze_llama_model: Optional[bool] = True,\n    gradient_checkpointing: Optional[bool] = False,\n):\n\"\"\"\n    Initializes a MiniGPT4Blip2LlamaForGeneration instance.\n\n    Args:\n        blip2_config_path (str): The path to the Blip2 model configuration file.\n        llama_config_path (str): The path to the Llama model configuration file.\n        pad_token_id (int, optional): The ID of the padding token. Defaults to 0.\n        freeze_vision_model (bool, optional): Whether to freeze the parameters of the vision model. Defaults to True.\n        freeze_qformer_model (bool, optional): Whether to freeze the parameters of the qformer model. Defaults to True.\n        freeze_llama_model (bool, optional): Whether to freeze the parameters of the llama model. Defaults to True.\n        gradient_checkpointing (bool, optional): Whether to use gradient checkpointing. Defaults to False.\n    \"\"\"\n    super().__init__()\n    self.blip2_config = Blip2Config.from_json_file(blip2_config_path)\n    self.blip2_config.pad_token_id = pad_token_id\n    self.llama_config = LlamaConfig.from_json_file(llama_config_path)\n    self.llama_config.gradient_checkpointing = gradient_checkpointing\n    self.model = MiniGPT4Blip2LlamaModel(self.blip2_config, self.llama_config)\n    self.init_weights()\n\n    if freeze_vision_model:\n        for param in self.model.vision_model.parameters():\n            param.requires_grad = False\n\n    if freeze_qformer_model:\n        for param in self.model.qformer.parameters():\n            param.requires_grad = False\n\n    if freeze_llama_model:\n        for param in self.model.llama.parameters():\n            param.requires_grad = False\n</code></pre>",
+            "title": "MiniGPT4Blip2LlamaForGeneration"
+        },
+        {
+            "location": "models/minigpt4/#unitorch.models.minigpt4.modeling.MiniGPT4Blip2LlamaForGeneration.forward",
+            "text": "<pre><code>forward(\n    pixel_values: torch.Tensor,\n    prefix_input_ids: torch.Tensor,\n    suffix_input_ids: torch.Tensor,\n    decoder_input_ids: torch.Tensor,\n    prefix_attention_mask: Optional[torch.Tensor] = None,\n    suffix_attention_mask: Optional[torch.Tensor] = None,\n    decoder_attention_mask: Optional[torch.Tensor] = None,\n)\n</code></pre> <p>Performs a forward pass of the MiniGPT4Blip2LlamaForGeneration model.</p> <p>Parameters:</p> Name Type Description Default <code>pixel_values</code> <code>torch.Tensor</code> <p>The pixel values.</p> required <code>prefix_input_ids</code> <code>torch.Tensor</code> <p>The input IDs for the prefix tokens.</p> required <code>suffix_input_ids</code> <code>torch.Tensor</code> <p>The input IDs for the suffix tokens.</p> required <code>decoder_input_ids</code> <code>torch.Tensor</code> <p>The input IDs for the decoder tokens.</p> required <code>prefix_attention_mask</code> <code>torch.Tensor</code> <p>The attention mask for the prefix tokens.</p> <code>None</code> <code>suffix_attention_mask</code> <code>torch.Tensor</code> <p>The attention mask for the suffix tokens.</p> <code>None</code> <code>decoder_attention_mask</code> <code>torch.Tensor</code> <p>The attention mask for the decoder tokens.</p> <code>None</code> <p>Returns:</p> Name Type Description <code>logits</code> <p>The output logits.</p> Source code in <code>src/unitorch/models/minigpt4/modeling.py</code> <pre><code>def forward(\n    self,\n    pixel_values: torch.Tensor,\n    prefix_input_ids: torch.Tensor,\n    suffix_input_ids: torch.Tensor,\n    decoder_input_ids: torch.Tensor,\n    prefix_attention_mask: Optional[torch.Tensor] = None,\n    suffix_attention_mask: Optional[torch.Tensor] = None,\n    decoder_attention_mask: Optional[torch.Tensor] = None,\n):\n\"\"\"\n    Performs a forward pass of the MiniGPT4Blip2LlamaForGeneration model.\n\n    Args:\n        pixel_values (torch.Tensor): The pixel values.\n        prefix_input_ids (torch.Tensor): The input IDs for the prefix tokens.\n        suffix_input_ids (torch.Tensor): The input IDs for the suffix tokens.\n        decoder_input_ids (torch.Tensor): The input IDs for the decoder tokens.\n        prefix_attention_mask (torch.Tensor, optional): The attention mask for the prefix tokens.\n        suffix_attention_mask (torch.Tensor, optional): The attention mask for the suffix tokens.\n        decoder_attention_mask (torch.Tensor, optional): The attention mask for the decoder tokens.\n\n    Returns:\n        logits: The output logits.\n    \"\"\"\n    outputs = self.model(\n        pixel_values=pixel_values,\n        prefix_input_ids=prefix_input_ids,\n        suffix_input_ids=suffix_input_ids,\n        decoder_input_ids=decoder_input_ids,\n        prefix_attention_mask=prefix_attention_mask,\n        suffix_attention_mask=suffix_attention_mask,\n        decoder_attention_mask=decoder_attention_mask,\n    )\n    logits = outputs.logits[\n        :, -suffix_input_ids.size(1) - decoder_input_ids.size(1) :, :\n    ]\n    return logits\n</code></pre>",
+            "title": "forward"
+        },
+        {
+            "location": "models/minigpt4/#unitorch.models.minigpt4.modeling.MiniGPT4Blip2LlamaForGeneration.generate",
+            "text": "<pre><code>generate(\n    pixel_values: torch.Tensor,\n    prefix_input_ids: torch.Tensor,\n    suffix_input_ids: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 1,\n    decoder_end_token_id: Optional[\n        Union[int, List[int]]\n    ] = 2,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n)\n</code></pre> <p>Generates sequences using the MiniGPT4Blip2LlamaForGeneration model.</p> <p>Parameters:</p> Name Type Description Default <code>pixel_values</code> <code>torch.Tensor</code> <p>The pixel values.</p> required <code>prefix_input_ids</code> <code>torch.Tensor</code> <p>The input IDs for the prefix tokens.</p> required <code>suffix_input_ids</code> <code>torch.Tensor</code> <p>The input IDs for the suffix tokens.</p> required <code>num_beams</code> <code>int</code> <p>The number of beams for beam search. Defaults to 5.</p> <code>5</code> <code>decoder_start_token_id</code> <code>int</code> <p>The ID of the decoder start token. Defaults to 1.</p> <code>1</code> <code>decoder_end_token_id</code> <code>int or List[int]</code> <p>The ID(s) of the decoder end token(s). Defaults to 2.</p> <code>2</code> <code>num_return_sequences</code> <code>int</code> <p>The number of generated sequences to return. Defaults to 1.</p> <code>1</code> <code>min_gen_seq_length</code> <code>int</code> <p>The minimum length of the generated sequences. Defaults to 0.</p> <code>0</code> <code>max_gen_seq_length</code> <code>int</code> <p>The maximum length of the generated sequences. Defaults to 48.</p> <code>48</code> <code>repetition_penalty</code> <code>float</code> <p>The repetition penalty. Defaults to 1.0.</p> <code>1.0</code> <code>no_repeat_ngram_size</code> <code>int</code> <p>The size of the n-grams to avoid repeating. Defaults to 0.</p> <code>0</code> <code>early_stopping</code> <code>bool</code> <p>Whether to stop generation early when all beams are finished. Defaults to True.</p> <code>True</code> <code>length_penalty</code> <code>float</code> <p>The length penalty. Defaults to 1.0.</p> <code>1.0</code> <code>num_beam_groups</code> <code>int</code> <p>The number of groups for diverse beam search. Defaults to 1.</p> <code>1</code> <code>diversity_penalty</code> <code>float</code> <p>The diversity penalty. Defaults to 0.0.</p> <code>0.0</code> <code>do_sample</code> <code>bool</code> <p>Whether to use sampling for generation. Defaults to False.</p> <code>False</code> <code>temperature</code> <code>float</code> <p>The temperature value for sampling. Defaults to 1.0.</p> <code>1.0</code> <code>top_k</code> <code>int</code> <p>The value for top-k sampling. Defaults to 50.</p> <code>50</code> <code>top_p</code> <code>float</code> <p>The value for top-p sampling. Defaults to 1.0.</p> <code>1.0</code> <p>Returns:</p> Name Type Description <code>outputs</code> <code>GenericOutputs</code> <p>The generated sequences and their scores.</p> Source code in <code>src/unitorch/models/minigpt4/modeling.py</code> <pre><code>@torch.no_grad()\ndef generate(\n    self,\n    pixel_values: torch.Tensor,\n    prefix_input_ids: torch.Tensor,\n    suffix_input_ids: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 1,\n    decoder_end_token_id: Optional[Union[int, List[int]]] = 2,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n):\n\"\"\"\n    Generates sequences using the MiniGPT4Blip2LlamaForGeneration model.\n\n    Args:\n        pixel_values (torch.Tensor): The pixel values.\n        prefix_input_ids (torch.Tensor): The input IDs for the prefix tokens.\n        suffix_input_ids (torch.Tensor): The input IDs for the suffix tokens.\n        num_beams (int, optional): The number of beams for beam search. Defaults to 5.\n        decoder_start_token_id (int, optional): The ID of the decoder start token. Defaults to 1.\n        decoder_end_token_id (int or List[int], optional): The ID(s) of the decoder end token(s). Defaults to 2.\n        num_return_sequences (int, optional): The number of generated sequences to return. Defaults to 1.\n        min_gen_seq_length (int, optional): The minimum length of the generated sequences. Defaults to 0.\n        max_gen_seq_length (int, optional): The maximum length of the generated sequences. Defaults to 48.\n        repetition_penalty (float, optional): The repetition penalty. Defaults to 1.0.\n        no_repeat_ngram_size (int, optional): The size of the n-grams to avoid repeating. Defaults to 0.\n        early_stopping (bool, optional): Whether to stop generation early when all beams are finished. Defaults to True.\n        length_penalty (float, optional): The length penalty. Defaults to 1.0.\n        num_beam_groups (int, optional): The number of groups for diverse beam search. Defaults to 1.\n        diversity_penalty (float, optional): The diversity penalty. Defaults to 0.0.\n        do_sample (bool, optional): Whether to use sampling for generation. Defaults to False.\n        temperature (float, optional): The temperature value for sampling. Defaults to 1.0.\n        top_k (int, optional): The value for top-k sampling. Defaults to 50.\n        top_p (float, optional): The value for top-p sampling. Defaults to 1.0.\n\n    Returns:\n        outputs (GenericOutputs): The generated sequences and their scores.\n    \"\"\"\n    outputs = self.model.generate(\n        pixel_values=pixel_values,\n        prefix_input_ids=prefix_input_ids,\n        suffix_input_ids=suffix_input_ids,\n        max_length=max_gen_seq_length,\n        min_length=min_gen_seq_length,\n        num_beams=num_beams,\n        do_sample=do_sample,\n        decoder_start_token_id=decoder_start_token_id,\n        no_repeat_ngram_size=no_repeat_ngram_size,\n        early_stopping=early_stopping,\n        length_penalty=length_penalty,\n        repetition_penalty=repetition_penalty,\n        num_return_sequences=num_return_sequences,\n        bos_token_id=decoder_start_token_id,\n        eos_token_id=decoder_end_token_id,\n        num_beam_groups=num_beam_groups,\n        diversity_penalty=diversity_penalty,\n        temperature=temperature,\n        top_k=top_k,\n        top_p=top_p,\n        return_dict_in_generate=True,\n        output_scores=True,\n    )\n\n    sequences = outputs.sequences.reshape(\n        -1, num_return_sequences, outputs.sequences.size(-1)\n    )\n    outputs.sequences = torch.zeros(\n        sequences.size(0), num_return_sequences, max_gen_seq_length\n    ).to(device=sequences.device)\n    outputs.sequences[:, :, : sequences.size(-1)].copy_(\n        sequences[:, :, : sequences.size(-1)]\n    )\n\n    if num_return_sequences == 1:\n        outputs.sequences = outputs.sequences.reshape(-1, max_gen_seq_length)\n\n    return GenericOutputs(\n        sequences=outputs.sequences.long(),\n        sequences_scores=outputs.sequences_scores,\n    )\n</code></pre>",
             "title": "generate"
         },
         {
             "location": "models/mt5/",
             "text": "",
             "title": "unitorch.models.mt5"
         },
@@ -2267,15 +2362,15 @@
         {
             "location": "models/mt5/#unitorch.models.mt5.modeling.MT5ForGeneration.forward",
             "text": "<pre><code>forward(\n    input_ids: torch.Tensor,\n    attention_mask: torch.Tensor,\n    decoder_input_ids: torch.Tensor,\n    decoder_attention_mask: torch.Tensor,\n)\n</code></pre> <p>Performs forward pass of the MT5ForGeneration model.</p> <p>Parameters:</p> Name Type Description Default <code>input_ids</code> <code>torch.Tensor</code> <p>Tensor of input token IDs.</p> required <code>attention_mask</code> <code>torch.Tensor</code> <p>Tensor of attention mask.</p> required <code>decoder_input_ids</code> <code>torch.Tensor</code> <p>Tensor of decoder input token IDs.</p> required <code>decoder_attention_mask</code> <code>torch.Tensor</code> <p>Tensor of decoder attention mask.</p> required <p>Returns:</p> Type Description <code>torch.Tensor</code> <p>The model's logits.</p> Source code in <code>src/unitorch/models/mt5/modeling.py</code> <pre><code>def forward(\n    self,\n    input_ids: torch.Tensor,\n    attention_mask: torch.Tensor,\n    decoder_input_ids: torch.Tensor,\n    decoder_attention_mask: torch.Tensor,\n):\n\"\"\"\n    Performs forward pass of the MT5ForGeneration model.\n\n    Args:\n        input_ids (torch.Tensor): Tensor of input token IDs.\n        attention_mask (torch.Tensor): Tensor of attention mask.\n        decoder_input_ids (torch.Tensor): Tensor of decoder input token IDs.\n        decoder_attention_mask (torch.Tensor): Tensor of decoder attention mask.\n\n    Returns:\n        (torch.Tensor):The model's logits.\n    \"\"\"\n    outputs = self.model(\n        input_ids=input_ids,\n        attention_mask=attention_mask,\n        decoder_input_ids=decoder_input_ids,\n        decoder_attention_mask=decoder_attention_mask,\n        return_dict=True,\n    )\n    logits = outputs.logits\n    return logits\n</code></pre>",
             "title": "forward"
         },
         {
             "location": "models/mt5/#unitorch.models.mt5.modeling.MT5ForGeneration.generate",
-            "text": "<pre><code>generate(\n    input_ids: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 0,\n    decoder_end_token_id: Optional[int] = 1,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n)\n</code></pre> <p>Generates sequences using the MT5ForGeneration model.</p> <p>Parameters:</p> Name Type Description Default <code>input_ids</code> <code>torch.Tensor</code> <p>The input token IDs.</p> required <code>num_beams</code> <code>int</code> <p>The number of beams for beam search. Defaults to 5.</p> <code>5</code> <code>decoder_start_token_id</code> <code>int</code> <p>The decoder's start token ID. Defaults to 2.</p> <code>0</code> <code>decoder_end_token_id</code> <code>int</code> <p>The decoder's end token ID. Defaults to 2.</p> <code>1</code> <code>num_return_sequences</code> <code>int</code> <p>The number of generated sequences to return. Defaults to 1.</p> <code>1</code> <code>min_gen_seq_length</code> <code>int</code> <p>The minimum length of the generated sequences. Defaults to 0.</p> <code>0</code> <code>max_gen_seq_length</code> <code>int</code> <p>The maximum length of the generated sequences. Defaults to 48.</p> <code>48</code> <code>repetition_penalty</code> <code>float</code> <p>The repetition penalty. Defaults to 1.0.</p> <code>1.0</code> <code>no_repeat_ngram_size</code> <code>int</code> <p>The size of n-grams to avoid repeating. Defaults to 0.</p> <code>0</code> <code>early_stopping</code> <code>bool</code> <p>Whether to stop generation early. Defaults to True.</p> <code>True</code> <code>length_penalty</code> <code>float</code> <p>The length penalty. Defaults to 1.0.</p> <code>1.0</code> <code>num_beam_groups</code> <code>int</code> <p>The number of beam groups for diverse beam search. Defaults to 1.</p> <code>1</code> <code>diversity_penalty</code> <code>float</code> <p>The diversity penalty. Defaults to 0.0.</p> <code>0.0</code> <code>do_sample</code> <code>bool</code> <p>Whether to use sampling for generation. Defaults to False.</p> <code>False</code> <code>temperature</code> <code>float</code> <p>The temperature for sampling. Defaults to 1.0.</p> <code>1.0</code> <code>top_k</code> <code>int</code> <p>The value for top-k sampling. Defaults to 50.</p> <code>50</code> <code>top_p</code> <code>float</code> <p>The value for top-p (nucleus) sampling. Defaults to 1.0.</p> <code>1.0</code> <p>Returns:</p> Name Type Description <code>GenericOutputs</code> <p>The generated sequences and their scores.</p> Source code in <code>src/unitorch/models/mt5/modeling.py</code> <pre><code>@torch.no_grad()\ndef generate(\n    self,\n    input_ids: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 0,\n    decoder_end_token_id: Optional[int] = 1,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n):\n\"\"\"\n    Generates sequences using the MT5ForGeneration model.\n\n    Args:\n        input_ids: The input token IDs.\n        num_beams (int, optional): The number of beams for beam search. Defaults to 5.\n        decoder_start_token_id (int, optional): The decoder's start token ID. Defaults to 2.\n        decoder_end_token_id (int, optional): The decoder's end token ID. Defaults to 2.\n        num_return_sequences (int, optional): The number of generated sequences to return. Defaults to 1.\n        min_gen_seq_length (int, optional): The minimum length of the generated sequences. Defaults to 0.\n        max_gen_seq_length (int, optional): The maximum length of the generated sequences. Defaults to 48.\n        repetition_penalty (float, optional): The repetition penalty. Defaults to 1.0.\n        no_repeat_ngram_size (int, optional): The size of n-grams to avoid repeating. Defaults to 0.\n        early_stopping (bool, optional): Whether to stop generation early. Defaults to True.\n        length_penalty (float, optional): The length penalty. Defaults to 1.0.\n        num_beam_groups (int, optional): The number of beam groups for diverse beam search. Defaults to 1.\n        diversity_penalty (float, optional): The diversity penalty. Defaults to 0.0.\n        do_sample (bool, optional): Whether to use sampling for generation. Defaults to False.\n        temperature (float, optional): The temperature for sampling. Defaults to 1.0.\n        top_k (int, optional): The value for top-k sampling. Defaults to 50.\n        top_p (float, optional): The value for top-p (nucleus) sampling. Defaults to 1.0.\n\n    Returns:\n        GenericOutputs: The generated sequences and their scores.\n    \"\"\"\n    outputs = self.model.generate(\n        input_ids,\n        max_length=max_gen_seq_length,\n        min_length=min_gen_seq_length,\n        num_beams=num_beams,\n        do_sample=do_sample,\n        decoder_start_token_id=decoder_start_token_id,\n        no_repeat_ngram_size=no_repeat_ngram_size,\n        early_stopping=early_stopping,\n        length_penalty=length_penalty,\n        repetition_penalty=repetition_penalty,\n        num_return_sequences=num_return_sequences,\n        bos_token_id=decoder_start_token_id,\n        eos_token_id=decoder_end_token_id,\n        num_beam_groups=num_beam_groups,\n        diversity_penalty=diversity_penalty,\n        temperature=temperature,\n        top_k=top_k,\n        top_p=top_p,\n        return_dict_in_generate=True,\n        output_scores=True,\n    )\n\n    sequences = outputs.sequences.reshape(\n        -1, num_return_sequences, outputs.sequences.size(-1)\n    )\n    outputs.sequences = torch.zeros(\n        sequences.size(0), num_return_sequences, max_gen_seq_length\n    ).to(device=sequences.device)\n    outputs.sequences[:, :, : sequences.size(-1)].copy_(sequences)\n\n    if num_return_sequences == 1:\n        outputs.sequences = outputs.sequences.reshape(-1, max_gen_seq_length)\n\n    return GenericOutputs(\n        sequences=outputs.sequences,\n        sequences_scores=outputs.sequences_scores,\n    )\n</code></pre>",
+            "text": "<pre><code>generate(\n    input_ids: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 0,\n    decoder_end_token_id: Optional[\n        Union[int, List[int]]\n    ] = 1,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n)\n</code></pre> <p>Generates sequences using the MT5ForGeneration model.</p> <p>Parameters:</p> Name Type Description Default <code>input_ids</code> <code>torch.Tensor</code> <p>The input token IDs.</p> required <code>num_beams</code> <code>int</code> <p>The number of beams for beam search. Defaults to 5.</p> <code>5</code> <code>decoder_start_token_id</code> <code>int</code> <p>The decoder's start token ID. Defaults to 2.</p> <code>0</code> <code>decoder_end_token_id</code> <code>int or List[int]</code> <p>The decoder's end token ID. Defaults to 2.</p> <code>1</code> <code>num_return_sequences</code> <code>int</code> <p>The number of generated sequences to return. Defaults to 1.</p> <code>1</code> <code>min_gen_seq_length</code> <code>int</code> <p>The minimum length of the generated sequences. Defaults to 0.</p> <code>0</code> <code>max_gen_seq_length</code> <code>int</code> <p>The maximum length of the generated sequences. Defaults to 48.</p> <code>48</code> <code>repetition_penalty</code> <code>float</code> <p>The repetition penalty. Defaults to 1.0.</p> <code>1.0</code> <code>no_repeat_ngram_size</code> <code>int</code> <p>The size of n-grams to avoid repeating. Defaults to 0.</p> <code>0</code> <code>early_stopping</code> <code>bool</code> <p>Whether to stop generation early. Defaults to True.</p> <code>True</code> <code>length_penalty</code> <code>float</code> <p>The length penalty. Defaults to 1.0.</p> <code>1.0</code> <code>num_beam_groups</code> <code>int</code> <p>The number of beam groups for diverse beam search. Defaults to 1.</p> <code>1</code> <code>diversity_penalty</code> <code>float</code> <p>The diversity penalty. Defaults to 0.0.</p> <code>0.0</code> <code>do_sample</code> <code>bool</code> <p>Whether to use sampling for generation. Defaults to False.</p> <code>False</code> <code>temperature</code> <code>float</code> <p>The temperature for sampling. Defaults to 1.0.</p> <code>1.0</code> <code>top_k</code> <code>int</code> <p>The value for top-k sampling. Defaults to 50.</p> <code>50</code> <code>top_p</code> <code>float</code> <p>The value for top-p (nucleus) sampling. Defaults to 1.0.</p> <code>1.0</code> <p>Returns:</p> Name Type Description <code>GenericOutputs</code> <p>The generated sequences and their scores.</p> Source code in <code>src/unitorch/models/mt5/modeling.py</code> <pre><code>@torch.no_grad()\ndef generate(\n    self,\n    input_ids: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 0,\n    decoder_end_token_id: Optional[Union[int, List[int]]] = 1,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n):\n\"\"\"\n    Generates sequences using the MT5ForGeneration model.\n\n    Args:\n        input_ids: The input token IDs.\n        num_beams (int, optional): The number of beams for beam search. Defaults to 5.\n        decoder_start_token_id (int, optional): The decoder's start token ID. Defaults to 2.\n        decoder_end_token_id (int or List[int], optional): The decoder's end token ID. Defaults to 2.\n        num_return_sequences (int, optional): The number of generated sequences to return. Defaults to 1.\n        min_gen_seq_length (int, optional): The minimum length of the generated sequences. Defaults to 0.\n        max_gen_seq_length (int, optional): The maximum length of the generated sequences. Defaults to 48.\n        repetition_penalty (float, optional): The repetition penalty. Defaults to 1.0.\n        no_repeat_ngram_size (int, optional): The size of n-grams to avoid repeating. Defaults to 0.\n        early_stopping (bool, optional): Whether to stop generation early. Defaults to True.\n        length_penalty (float, optional): The length penalty. Defaults to 1.0.\n        num_beam_groups (int, optional): The number of beam groups for diverse beam search. Defaults to 1.\n        diversity_penalty (float, optional): The diversity penalty. Defaults to 0.0.\n        do_sample (bool, optional): Whether to use sampling for generation. Defaults to False.\n        temperature (float, optional): The temperature for sampling. Defaults to 1.0.\n        top_k (int, optional): The value for top-k sampling. Defaults to 50.\n        top_p (float, optional): The value for top-p (nucleus) sampling. Defaults to 1.0.\n\n    Returns:\n        GenericOutputs: The generated sequences and their scores.\n    \"\"\"\n    outputs = self.model.generate(\n        input_ids,\n        max_length=max_gen_seq_length,\n        min_length=min_gen_seq_length,\n        num_beams=num_beams,\n        do_sample=do_sample,\n        decoder_start_token_id=decoder_start_token_id,\n        no_repeat_ngram_size=no_repeat_ngram_size,\n        early_stopping=early_stopping,\n        length_penalty=length_penalty,\n        repetition_penalty=repetition_penalty,\n        num_return_sequences=num_return_sequences,\n        bos_token_id=decoder_start_token_id,\n        eos_token_id=decoder_end_token_id,\n        num_beam_groups=num_beam_groups,\n        diversity_penalty=diversity_penalty,\n        temperature=temperature,\n        top_k=top_k,\n        top_p=top_p,\n        return_dict_in_generate=True,\n        output_scores=True,\n    )\n\n    sequences = outputs.sequences.reshape(\n        -1, num_return_sequences, outputs.sequences.size(-1)\n    )\n    outputs.sequences = torch.zeros(\n        sequences.size(0), num_return_sequences, max_gen_seq_length\n    ).to(device=sequences.device)\n    outputs.sequences[:, :, : sequences.size(-1)].copy_(sequences)\n\n    if num_return_sequences == 1:\n        outputs.sequences = outputs.sequences.reshape(-1, max_gen_seq_length)\n\n    return GenericOutputs(\n        sequences=outputs.sequences,\n        sequences_scores=outputs.sequences_scores,\n    )\n</code></pre>",
             "title": "generate"
         },
         {
             "location": "models/peft/",
             "text": "",
             "title": "unitorch.models.peft"
         },
@@ -2297,15 +2392,15 @@
         {
             "location": "models/peft/#unitorch.models.peft.modeling_bloom_adalora.BloomAdaLoraForGeneration.forward",
             "text": "<pre><code>forward(\n    input_ids: torch.Tensor,\n    attention_mask: Optional[torch.Tensor] = None,\n    position_ids: Optional[torch.Tensor] = None,\n)\n</code></pre> <p>Forward pass of the generation model.</p> <p>Parameters:</p> Name Type Description Default <code>input_ids</code> <code>torch.Tensor</code> <p>Input tensor of shape (batch_size, sequence_length). Defaults to None.</p> required <code>attention_mask</code> <code>torch.Tensor</code> <p>Attention mask tensor of shape (batch_size, sequence_length). Defaults to None.</p> <code>None</code> <code>position_ids</code> <code>torch.Tensor</code> <p>Position IDs tensor of shape (batch_size, sequence_length). Defaults to None.</p> <code>None</code> <p>Returns:</p> Type Description <p>torch Output logits.Tensor: tensor of shape (batch_size, sequence_length, vocab_size).</p> Source code in <code>src/unitorch/models/peft/modeling_bloom_adalora.py</code> <pre><code>def forward(\n    self,\n    input_ids: torch.Tensor,\n    attention_mask: Optional[torch.Tensor] = None,\n    position_ids: Optional[torch.Tensor] = None,\n):\n\"\"\"\n    Forward pass of the generation model.\n\n    Args:\n        input_ids (torch.Tensor, optional): Input tensor of shape (batch_size, sequence_length). Defaults to None.\n        attention_mask (torch.Tensor, optional): Attention mask tensor of shape (batch_size, sequence_length). Defaults to None.\n        position_ids (torch.Tensor, optional): Position IDs tensor of shape (batch_size, sequence_length). Defaults to None.\n\n    Returns:\n        torch Output logits.Tensor: tensor of shape (batch_size, sequence_length, vocab_size).\n    \"\"\"\n    outputs = self.peft_model(\n        input_ids=input_ids,\n        attention_mask=attention_mask,\n        position_ids=position_ids,\n        return_dict=True,\n    )\n    logits = outputs.logits\n    return logits\n</code></pre>",
             "title": "forward"
         },
         {
             "location": "models/peft/#unitorch.models.peft.modeling_bloom_adalora.BloomAdaLoraForGeneration.generate",
-            "text": "<pre><code>generate(\n    input_ids: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 1,\n    decoder_end_token_id: Optional[int] = 2,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n)\n</code></pre> <p>Generate text using the generation model.</p> <p>Parameters:</p> Name Type Description Default <code>input_ids</code> <code>torch.Tensor</code> <p>Input tensor of shape (batch_size, sequence_length).</p> required <code>num_beams</code> <code>int</code> <p>Number of beams for beam search. Defaults to 5.</p> <code>5</code> <code>decoder_start_token_id</code> <code>int</code> <p>Start token ID for the decoder. Defaults to 2.</p> <code>1</code> <code>decoder_end_token_id</code> <code>int</code> <p>End token ID for the decoder. Defaults to 2.</p> <code>2</code> <code>num_return_sequences</code> <code>int</code> <p>Number of generated sequences to return. Defaults to 1.</p> <code>1</code> <code>min_gen_seq_length</code> <code>int</code> <p>Minimum length of generated sequences. Defaults to 0.</p> <code>0</code> <code>max_gen_seq_length</code> <code>int</code> <p>Maximum length of generated sequences. Defaults to 48.</p> <code>48</code> <code>repetition_penalty</code> <code>float</code> <p>Penalty for repeated tokens. Defaults to 1.0.</p> <code>1.0</code> <code>no_repeat_ngram_size</code> <code>int</code> <p>Size of n-grams to avoid repeating. Defaults to 0.</p> <code>0</code> <code>early_stopping</code> <code>bool</code> <p>Whether to stop generation early. Defaults to True.</p> <code>True</code> <code>length_penalty</code> <code>float</code> <p>Penalty for longer sequences. Defaults to 1.0.</p> <code>1.0</code> <code>num_beam_groups</code> <code>int</code> <p>Number of beam groups for diverse beam search. Defaults to 1.</p> <code>1</code> <code>diversity_penalty</code> <code>float</code> <p>Penalty for diverse sequences in diverse beam search. Defaults to 0.0.</p> <code>0.0</code> <code>do_sample</code> <code>bool</code> <p>Whether to use sampling for generation. Defaults to False.</p> <code>False</code> <code>temperature</code> <code>float</code> <p>Sampling temperature. Defaults to 1.0.</p> <code>1.0</code> <code>top_k</code> <code>int</code> <p>Top-k value for sampling. Defaults to 50.</p> <code>50</code> <code>top_p</code> <code>float</code> <p>Top-p value for sampling. Defaults to 1.0.</p> <code>1.0</code> <p>Returns:</p> Name Type Description <code>GenericOutputs</code> <p>Generated sequences and their scores.</p> Source code in <code>src/unitorch/models/peft/modeling_bloom_adalora.py</code> <pre><code>@torch.no_grad()\ndef generate(\n    self,\n    input_ids: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 1,\n    decoder_end_token_id: Optional[int] = 2,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n):\n\"\"\"\n    Generate text using the generation model.\n\n    Args:\n        input_ids: Input tensor of shape (batch_size, sequence_length).\n        num_beams (int, optional): Number of beams for beam search. Defaults to 5.\n        decoder_start_token_id (int, optional): Start token ID for the decoder. Defaults to 2.\n        decoder_end_token_id (int, optional): End token ID for the decoder. Defaults to 2.\n        num_return_sequences (int, optional): Number of generated sequences to return. Defaults to 1.\n        min_gen_seq_length (int, optional): Minimum length of generated sequences. Defaults to 0.\n        max_gen_seq_length (int, optional): Maximum length of generated sequences. Defaults to 48.\n        repetition_penalty (float, optional): Penalty for repeated tokens. Defaults to 1.0.\n        no_repeat_ngram_size (int, optional): Size of n-grams to avoid repeating. Defaults to 0.\n        early_stopping (bool, optional): Whether to stop generation early. Defaults to True.\n        length_penalty (float, optional): Penalty for longer sequences. Defaults to 1.0.\n        num_beam_groups (int, optional): Number of beam groups for diverse beam search. Defaults to 1.\n        diversity_penalty (float, optional): Penalty for diverse sequences in diverse beam search. Defaults to 0.0.\n        do_sample (bool, optional): Whether to use sampling for generation. Defaults to False.\n        temperature (float, optional): Sampling temperature. Defaults to 1.0.\n        top_k (int, optional): Top-k value for sampling. Defaults to 50.\n        top_p (float, optional): Top-p value for sampling. Defaults to 1.0.\n\n    Returns:\n        GenericOutputs: Generated sequences and their scores.\n    \"\"\"\n    input_seq_length = input_ids.size(1)\n    outputs = self.peft_model.generate(\n        input_ids=input_ids,\n        max_length=max_gen_seq_length + input_seq_length,\n        min_length=min_gen_seq_length + input_seq_length,\n        num_beams=num_beams,\n        do_sample=do_sample,\n        decoder_start_token_id=decoder_start_token_id,\n        no_repeat_ngram_size=no_repeat_ngram_size,\n        early_stopping=early_stopping,\n        length_penalty=length_penalty,\n        repetition_penalty=repetition_penalty,\n        num_return_sequences=num_return_sequences,\n        bos_token_id=decoder_start_token_id,\n        eos_token_id=decoder_end_token_id,\n        num_beam_groups=num_beam_groups,\n        diversity_penalty=diversity_penalty,\n        temperature=temperature,\n        top_k=top_k,\n        top_p=top_p,\n        return_dict_in_generate=True,\n        output_scores=True,\n    )\n\n    sequences = outputs.sequences.reshape(\n        -1, num_return_sequences, outputs.sequences.size(-1)\n    )\n    outputs.sequences = torch.zeros(\n        sequences.size(0), num_return_sequences, max_gen_seq_length\n    ).to(device=sequences.device)\n    outputs.sequences[:, :, : sequences.size(-1) - input_seq_length].copy_(\n        sequences[:, :, input_seq_length : sequences.size(-1)]\n    )\n\n    if num_return_sequences == 1:\n        outputs.sequences = outputs.sequences.reshape(-1, max_gen_seq_length)\n\n    return GenericOutputs(\n        sequences=outputs.sequences.long(),\n        sequences_scores=outputs.sequences_scores,\n    )\n</code></pre>",
+            "text": "<pre><code>generate(\n    input_ids: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 1,\n    decoder_end_token_id: Optional[\n        Union[int, List[int]]\n    ] = 2,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n)\n</code></pre> <p>Generate text using the generation model.</p> <p>Parameters:</p> Name Type Description Default <code>input_ids</code> <code>torch.Tensor</code> <p>Input tensor of shape (batch_size, sequence_length).</p> required <code>num_beams</code> <code>int</code> <p>Number of beams for beam search. Defaults to 5.</p> <code>5</code> <code>decoder_start_token_id</code> <code>int</code> <p>The ID of the decoder start token. Defaults to 2.</p> <code>1</code> <code>decoder_end_token_id</code> <code>int or List[int]</code> <p>The ID(s) of the decoder end token(s). Defaults to 2.</p> <code>2</code> <code>num_return_sequences</code> <code>int</code> <p>Number of generated sequences to return. Defaults to 1.</p> <code>1</code> <code>min_gen_seq_length</code> <code>int</code> <p>Minimum length of generated sequences. Defaults to 0.</p> <code>0</code> <code>max_gen_seq_length</code> <code>int</code> <p>Maximum length of generated sequences. Defaults to 48.</p> <code>48</code> <code>repetition_penalty</code> <code>float</code> <p>Penalty for repeated tokens. Defaults to 1.0.</p> <code>1.0</code> <code>no_repeat_ngram_size</code> <code>int</code> <p>Size of n-grams to avoid repeating. Defaults to 0.</p> <code>0</code> <code>early_stopping</code> <code>bool</code> <p>Whether to stop generation early. Defaults to True.</p> <code>True</code> <code>length_penalty</code> <code>float</code> <p>Penalty for longer sequences. Defaults to 1.0.</p> <code>1.0</code> <code>num_beam_groups</code> <code>int</code> <p>Number of beam groups for diverse beam search. Defaults to 1.</p> <code>1</code> <code>diversity_penalty</code> <code>float</code> <p>Penalty for diverse sequences in diverse beam search. Defaults to 0.0.</p> <code>0.0</code> <code>do_sample</code> <code>bool</code> <p>Whether to use sampling for generation. Defaults to False.</p> <code>False</code> <code>temperature</code> <code>float</code> <p>Sampling temperature. Defaults to 1.0.</p> <code>1.0</code> <code>top_k</code> <code>int</code> <p>Top-k value for sampling. Defaults to 50.</p> <code>50</code> <code>top_p</code> <code>float</code> <p>Top-p value for sampling. Defaults to 1.0.</p> <code>1.0</code> <p>Returns:</p> Name Type Description <code>GenericOutputs</code> <p>Generated sequences and their scores.</p> Source code in <code>src/unitorch/models/peft/modeling_bloom_adalora.py</code> <pre><code>@torch.no_grad()\ndef generate(\n    self,\n    input_ids: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 1,\n    decoder_end_token_id: Optional[Union[int, List[int]]] = 2,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n):\n\"\"\"\n    Generate text using the generation model.\n\n    Args:\n        input_ids: Input tensor of shape (batch_size, sequence_length).\n        num_beams (int, optional): Number of beams for beam search. Defaults to 5.\n        decoder_start_token_id (int, optional): The ID of the decoder start token. Defaults to 2.\n        decoder_end_token_id (int or List[int], optional): The ID(s) of the decoder end token(s). Defaults to 2.\n        num_return_sequences (int, optional): Number of generated sequences to return. Defaults to 1.\n        min_gen_seq_length (int, optional): Minimum length of generated sequences. Defaults to 0.\n        max_gen_seq_length (int, optional): Maximum length of generated sequences. Defaults to 48.\n        repetition_penalty (float, optional): Penalty for repeated tokens. Defaults to 1.0.\n        no_repeat_ngram_size (int, optional): Size of n-grams to avoid repeating. Defaults to 0.\n        early_stopping (bool, optional): Whether to stop generation early. Defaults to True.\n        length_penalty (float, optional): Penalty for longer sequences. Defaults to 1.0.\n        num_beam_groups (int, optional): Number of beam groups for diverse beam search. Defaults to 1.\n        diversity_penalty (float, optional): Penalty for diverse sequences in diverse beam search. Defaults to 0.0.\n        do_sample (bool, optional): Whether to use sampling for generation. Defaults to False.\n        temperature (float, optional): Sampling temperature. Defaults to 1.0.\n        top_k (int, optional): Top-k value for sampling. Defaults to 50.\n        top_p (float, optional): Top-p value for sampling. Defaults to 1.0.\n\n    Returns:\n        GenericOutputs: Generated sequences and their scores.\n    \"\"\"\n    input_seq_length = input_ids.size(1)\n    outputs = self.peft_model.generate(\n        input_ids=input_ids,\n        max_length=max_gen_seq_length + input_seq_length,\n        min_length=min_gen_seq_length + input_seq_length,\n        num_beams=num_beams,\n        do_sample=do_sample,\n        decoder_start_token_id=decoder_start_token_id,\n        no_repeat_ngram_size=no_repeat_ngram_size,\n        early_stopping=early_stopping,\n        length_penalty=length_penalty,\n        repetition_penalty=repetition_penalty,\n        num_return_sequences=num_return_sequences,\n        bos_token_id=decoder_start_token_id,\n        eos_token_id=decoder_end_token_id,\n        num_beam_groups=num_beam_groups,\n        diversity_penalty=diversity_penalty,\n        temperature=temperature,\n        top_k=top_k,\n        top_p=top_p,\n        return_dict_in_generate=True,\n        output_scores=True,\n    )\n\n    sequences = outputs.sequences.reshape(\n        -1, num_return_sequences, outputs.sequences.size(-1)\n    )\n    outputs.sequences = torch.zeros(\n        sequences.size(0), num_return_sequences, max_gen_seq_length\n    ).to(device=sequences.device)\n    outputs.sequences[:, :, : sequences.size(-1) - input_seq_length].copy_(\n        sequences[:, :, input_seq_length : sequences.size(-1)]\n    )\n\n    if num_return_sequences == 1:\n        outputs.sequences = outputs.sequences.reshape(-1, max_gen_seq_length)\n\n    return GenericOutputs(\n        sequences=outputs.sequences.long(),\n        sequences_scores=outputs.sequences_scores,\n    )\n</code></pre>",
             "title": "generate"
         },
         {
             "location": "models/peft/#bloomloraforclassification",
             "text": "<p>         Bases: <code>GenericModel</code>, <code>PeftCheckpointMixin</code></p> Source code in <code>src/unitorch/models/peft/modeling_bloom_lora.py</code> <pre><code>def __init__(\n    self,\n    config_path: str,\n    lora_r: Optional[int] = 16,\n    lora_alpha: Optional[int] = 32,\n    lora_dropout: Optional[float] = 0.05,\n    fan_in_fan_out: Optional[bool] = True,\n    target_modules: Optional[Union[List[str], str]] = [\"query_key_value\"],\n    num_classes: Optional[int] = 1,\n    hidden_dropout_prob: Optional[float] = 0.1,\n    gradient_checkpointing: Optional[bool] = False,\n):\n    super().__init__()\n    self.config = BloomConfig.from_json_file(config_path)\n    self.config.gradient_checkpointing = gradient_checkpointing\n    self.peft_config = LoraConfig(\n        r=lora_r,\n        lora_alpha=lora_alpha,\n        lora_dropout=lora_dropout,\n        fan_in_fan_out=fan_in_fan_out,\n        target_modules=target_modules,\n    )\n    self.peft_model = PeftModelForSequenceClassification(\n        BloomModel(self.config), self.peft_config\n    )\n    self.dropout = nn.Dropout(hidden_dropout_prob)\n    self.classifier = nn.Linear(self.config.hidden_size, num_classes)\n    self.init_weights()\n</code></pre>",
             "title": "BloomLoraForClassification"
         },
@@ -2322,15 +2417,15 @@
         {
             "location": "models/peft/#unitorch.models.peft.modeling_bloom_lora.BloomLoraForGeneration.forward",
             "text": "<pre><code>forward(\n    input_ids: torch.Tensor,\n    attention_mask: Optional[torch.Tensor] = None,\n    position_ids: Optional[torch.Tensor] = None,\n)\n</code></pre> <p>Forward pass of the generation model.</p> <p>Parameters:</p> Name Type Description Default <code>input_ids</code> <code>torch.Tensor</code> <p>Input tensor of shape (batch_size, sequence_length). Defaults to None.</p> required <code>attention_mask</code> <code>torch.Tensor</code> <p>Attention mask tensor of shape (batch_size, sequence_length). Defaults to None.</p> <code>None</code> <code>position_ids</code> <code>torch.Tensor</code> <p>Position IDs tensor of shape (batch_size, sequence_length). Defaults to None.</p> <code>None</code> <p>Returns:</p> Type Description <p>torch Output logits.Tensor: tensor of shape (batch_size, sequence_length, vocab_size).</p> Source code in <code>src/unitorch/models/peft/modeling_bloom_lora.py</code> <pre><code>def forward(\n    self,\n    input_ids: torch.Tensor,\n    attention_mask: Optional[torch.Tensor] = None,\n    position_ids: Optional[torch.Tensor] = None,\n):\n\"\"\"\n    Forward pass of the generation model.\n\n    Args:\n        input_ids (torch.Tensor, optional): Input tensor of shape (batch_size, sequence_length). Defaults to None.\n        attention_mask (torch.Tensor, optional): Attention mask tensor of shape (batch_size, sequence_length). Defaults to None.\n        position_ids (torch.Tensor, optional): Position IDs tensor of shape (batch_size, sequence_length). Defaults to None.\n\n    Returns:\n        torch Output logits.Tensor: tensor of shape (batch_size, sequence_length, vocab_size).\n    \"\"\"\n    outputs = self.peft_model(\n        input_ids=input_ids,\n        attention_mask=attention_mask,\n        position_ids=position_ids,\n        return_dict=True,\n    )\n    logits = outputs.logits\n    return logits\n</code></pre>",
             "title": "forward"
         },
         {
             "location": "models/peft/#unitorch.models.peft.modeling_bloom_lora.BloomLoraForGeneration.generate",
-            "text": "<pre><code>generate(\n    input_ids: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 1,\n    decoder_end_token_id: Optional[int] = 2,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n)\n</code></pre> <p>Generate text using the generation model.</p> <p>Parameters:</p> Name Type Description Default <code>input_ids</code> <code>torch.Tensor</code> <p>Input tensor of shape (batch_size, sequence_length).</p> required <code>num_beams</code> <code>int</code> <p>Number of beams for beam search. Defaults to 5.</p> <code>5</code> <code>decoder_start_token_id</code> <code>int</code> <p>Start token ID for the decoder. Defaults to 2.</p> <code>1</code> <code>decoder_end_token_id</code> <code>int</code> <p>End token ID for the decoder. Defaults to 2.</p> <code>2</code> <code>num_return_sequences</code> <code>int</code> <p>Number of generated sequences to return. Defaults to 1.</p> <code>1</code> <code>min_gen_seq_length</code> <code>int</code> <p>Minimum length of generated sequences. Defaults to 0.</p> <code>0</code> <code>max_gen_seq_length</code> <code>int</code> <p>Maximum length of generated sequences. Defaults to 48.</p> <code>48</code> <code>repetition_penalty</code> <code>float</code> <p>Penalty for repeated tokens. Defaults to 1.0.</p> <code>1.0</code> <code>no_repeat_ngram_size</code> <code>int</code> <p>Size of n-grams to avoid repeating. Defaults to 0.</p> <code>0</code> <code>early_stopping</code> <code>bool</code> <p>Whether to stop generation early. Defaults to True.</p> <code>True</code> <code>length_penalty</code> <code>float</code> <p>Penalty for longer sequences. Defaults to 1.0.</p> <code>1.0</code> <code>num_beam_groups</code> <code>int</code> <p>Number of beam groups for diverse beam search. Defaults to 1.</p> <code>1</code> <code>diversity_penalty</code> <code>float</code> <p>Penalty for diverse sequences in diverse beam search. Defaults to 0.0.</p> <code>0.0</code> <code>do_sample</code> <code>bool</code> <p>Whether to use sampling for generation. Defaults to False.</p> <code>False</code> <code>temperature</code> <code>float</code> <p>Sampling temperature. Defaults to 1.0.</p> <code>1.0</code> <code>top_k</code> <code>int</code> <p>Top-k value for sampling. Defaults to 50.</p> <code>50</code> <code>top_p</code> <code>float</code> <p>Top-p value for sampling. Defaults to 1.0.</p> <code>1.0</code> <p>Returns:</p> Name Type Description <code>GenericOutputs</code> <p>Generated sequences and their scores.</p> Source code in <code>src/unitorch/models/peft/modeling_bloom_lora.py</code> <pre><code>@torch.no_grad()\ndef generate(\n    self,\n    input_ids: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 1,\n    decoder_end_token_id: Optional[int] = 2,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n):\n\"\"\"\n    Generate text using the generation model.\n\n    Args:\n        input_ids: Input tensor of shape (batch_size, sequence_length).\n        num_beams (int, optional): Number of beams for beam search. Defaults to 5.\n        decoder_start_token_id (int, optional): Start token ID for the decoder. Defaults to 2.\n        decoder_end_token_id (int, optional): End token ID for the decoder. Defaults to 2.\n        num_return_sequences (int, optional): Number of generated sequences to return. Defaults to 1.\n        min_gen_seq_length (int, optional): Minimum length of generated sequences. Defaults to 0.\n        max_gen_seq_length (int, optional): Maximum length of generated sequences. Defaults to 48.\n        repetition_penalty (float, optional): Penalty for repeated tokens. Defaults to 1.0.\n        no_repeat_ngram_size (int, optional): Size of n-grams to avoid repeating. Defaults to 0.\n        early_stopping (bool, optional): Whether to stop generation early. Defaults to True.\n        length_penalty (float, optional): Penalty for longer sequences. Defaults to 1.0.\n        num_beam_groups (int, optional): Number of beam groups for diverse beam search. Defaults to 1.\n        diversity_penalty (float, optional): Penalty for diverse sequences in diverse beam search. Defaults to 0.0.\n        do_sample (bool, optional): Whether to use sampling for generation. Defaults to False.\n        temperature (float, optional): Sampling temperature. Defaults to 1.0.\n        top_k (int, optional): Top-k value for sampling. Defaults to 50.\n        top_p (float, optional): Top-p value for sampling. Defaults to 1.0.\n\n    Returns:\n        GenericOutputs: Generated sequences and their scores.\n    \"\"\"\n    input_seq_length = input_ids.size(1)\n    outputs = self.peft_model.generate(\n        input_ids=input_ids,\n        max_length=max_gen_seq_length + input_seq_length,\n        min_length=min_gen_seq_length + input_seq_length,\n        num_beams=num_beams,\n        do_sample=do_sample,\n        decoder_start_token_id=decoder_start_token_id,\n        no_repeat_ngram_size=no_repeat_ngram_size,\n        early_stopping=early_stopping,\n        length_penalty=length_penalty,\n        repetition_penalty=repetition_penalty,\n        num_return_sequences=num_return_sequences,\n        bos_token_id=decoder_start_token_id,\n        eos_token_id=decoder_end_token_id,\n        num_beam_groups=num_beam_groups,\n        diversity_penalty=diversity_penalty,\n        temperature=temperature,\n        top_k=top_k,\n        top_p=top_p,\n        return_dict_in_generate=True,\n        output_scores=True,\n    )\n\n    sequences = outputs.sequences.reshape(\n        -1, num_return_sequences, outputs.sequences.size(-1)\n    )\n    outputs.sequences = torch.zeros(\n        sequences.size(0), num_return_sequences, max_gen_seq_length\n    ).to(device=sequences.device)\n    outputs.sequences[:, :, : sequences.size(-1) - input_seq_length].copy_(\n        sequences[:, :, input_seq_length : sequences.size(-1)]\n    )\n\n    if num_return_sequences == 1:\n        outputs.sequences = outputs.sequences.reshape(-1, max_gen_seq_length)\n\n    return GenericOutputs(\n        sequences=outputs.sequences.long(),\n        sequences_scores=outputs.sequences_scores,\n    )\n</code></pre>",
+            "text": "<pre><code>generate(\n    input_ids: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 1,\n    decoder_end_token_id: Optional[\n        Union[int, List[int]]\n    ] = 2,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n)\n</code></pre> <p>Generate text using the generation model.</p> <p>Parameters:</p> Name Type Description Default <code>input_ids</code> <code>torch.Tensor</code> <p>Input tensor of shape (batch_size, sequence_length).</p> required <code>num_beams</code> <code>int</code> <p>Number of beams for beam search. Defaults to 5.</p> <code>5</code> <code>decoder_start_token_id</code> <code>int</code> <p>The ID of the decoder start token. Defaults to 2.</p> <code>1</code> <code>decoder_end_token_id</code> <code>int or List[int]</code> <p>The ID(s) of the decoder end token(s). Defaults to 2.</p> <code>2</code> <code>num_return_sequences</code> <code>int</code> <p>Number of generated sequences to return. Defaults to 1.</p> <code>1</code> <code>min_gen_seq_length</code> <code>int</code> <p>Minimum length of generated sequences. Defaults to 0.</p> <code>0</code> <code>max_gen_seq_length</code> <code>int</code> <p>Maximum length of generated sequences. Defaults to 48.</p> <code>48</code> <code>repetition_penalty</code> <code>float</code> <p>Penalty for repeated tokens. Defaults to 1.0.</p> <code>1.0</code> <code>no_repeat_ngram_size</code> <code>int</code> <p>Size of n-grams to avoid repeating. Defaults to 0.</p> <code>0</code> <code>early_stopping</code> <code>bool</code> <p>Whether to stop generation early. Defaults to True.</p> <code>True</code> <code>length_penalty</code> <code>float</code> <p>Penalty for longer sequences. Defaults to 1.0.</p> <code>1.0</code> <code>num_beam_groups</code> <code>int</code> <p>Number of beam groups for diverse beam search. Defaults to 1.</p> <code>1</code> <code>diversity_penalty</code> <code>float</code> <p>Penalty for diverse sequences in diverse beam search. Defaults to 0.0.</p> <code>0.0</code> <code>do_sample</code> <code>bool</code> <p>Whether to use sampling for generation. Defaults to False.</p> <code>False</code> <code>temperature</code> <code>float</code> <p>Sampling temperature. Defaults to 1.0.</p> <code>1.0</code> <code>top_k</code> <code>int</code> <p>Top-k value for sampling. Defaults to 50.</p> <code>50</code> <code>top_p</code> <code>float</code> <p>Top-p value for sampling. Defaults to 1.0.</p> <code>1.0</code> <p>Returns:</p> Name Type Description <code>GenericOutputs</code> <p>Generated sequences and their scores.</p> Source code in <code>src/unitorch/models/peft/modeling_bloom_lora.py</code> <pre><code>@torch.no_grad()\ndef generate(\n    self,\n    input_ids: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 1,\n    decoder_end_token_id: Optional[Union[int, List[int]]] = 2,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n):\n\"\"\"\n    Generate text using the generation model.\n\n    Args:\n        input_ids: Input tensor of shape (batch_size, sequence_length).\n        num_beams (int, optional): Number of beams for beam search. Defaults to 5.\n        decoder_start_token_id (int, optional): The ID of the decoder start token. Defaults to 2.\n        decoder_end_token_id (int or List[int], optional): The ID(s) of the decoder end token(s). Defaults to 2.\n        num_return_sequences (int, optional): Number of generated sequences to return. Defaults to 1.\n        min_gen_seq_length (int, optional): Minimum length of generated sequences. Defaults to 0.\n        max_gen_seq_length (int, optional): Maximum length of generated sequences. Defaults to 48.\n        repetition_penalty (float, optional): Penalty for repeated tokens. Defaults to 1.0.\n        no_repeat_ngram_size (int, optional): Size of n-grams to avoid repeating. Defaults to 0.\n        early_stopping (bool, optional): Whether to stop generation early. Defaults to True.\n        length_penalty (float, optional): Penalty for longer sequences. Defaults to 1.0.\n        num_beam_groups (int, optional): Number of beam groups for diverse beam search. Defaults to 1.\n        diversity_penalty (float, optional): Penalty for diverse sequences in diverse beam search. Defaults to 0.0.\n        do_sample (bool, optional): Whether to use sampling for generation. Defaults to False.\n        temperature (float, optional): Sampling temperature. Defaults to 1.0.\n        top_k (int, optional): Top-k value for sampling. Defaults to 50.\n        top_p (float, optional): Top-p value for sampling. Defaults to 1.0.\n\n    Returns:\n        GenericOutputs: Generated sequences and their scores.\n    \"\"\"\n    input_seq_length = input_ids.size(1)\n    outputs = self.peft_model.generate(\n        input_ids=input_ids,\n        max_length=max_gen_seq_length + input_seq_length,\n        min_length=min_gen_seq_length + input_seq_length,\n        num_beams=num_beams,\n        do_sample=do_sample,\n        decoder_start_token_id=decoder_start_token_id,\n        no_repeat_ngram_size=no_repeat_ngram_size,\n        early_stopping=early_stopping,\n        length_penalty=length_penalty,\n        repetition_penalty=repetition_penalty,\n        num_return_sequences=num_return_sequences,\n        bos_token_id=decoder_start_token_id,\n        eos_token_id=decoder_end_token_id,\n        num_beam_groups=num_beam_groups,\n        diversity_penalty=diversity_penalty,\n        temperature=temperature,\n        top_k=top_k,\n        top_p=top_p,\n        return_dict_in_generate=True,\n        output_scores=True,\n    )\n\n    sequences = outputs.sequences.reshape(\n        -1, num_return_sequences, outputs.sequences.size(-1)\n    )\n    outputs.sequences = torch.zeros(\n        sequences.size(0), num_return_sequences, max_gen_seq_length\n    ).to(device=sequences.device)\n    outputs.sequences[:, :, : sequences.size(-1) - input_seq_length].copy_(\n        sequences[:, :, input_seq_length : sequences.size(-1)]\n    )\n\n    if num_return_sequences == 1:\n        outputs.sequences = outputs.sequences.reshape(-1, max_gen_seq_length)\n\n    return GenericOutputs(\n        sequences=outputs.sequences.long(),\n        sequences_scores=outputs.sequences_scores,\n    )\n</code></pre>",
             "title": "generate"
         },
         {
             "location": "models/peft/#llamaadaloraforclassification",
             "text": "<p>         Bases: <code>GenericModel</code>, <code>PeftCheckpointMixin</code></p> Source code in <code>src/unitorch/models/peft/modeling_llama_adalora.py</code> <pre><code>def __init__(\n    self,\n    config_path: str,\n    target_r: Optional[int] = 8,\n    init_r: Optional[int] = 12,\n    tinit: Optional[int] = 0,\n    tfinal: Optional[int] = 0,\n    deltaT: Optional[int] = 1,\n    beta1: Optional[float] = 0.85,\n    beta2: Optional[float] = 0.85,\n    orth_reg_weight: Optional[float] = 0.5,\n    total_step: Optional[int] = None,\n    rank_pattern: Optional[dict] = None,\n    num_classes: Optional[int] = 1,\n    hidden_dropout_prob: Optional[float] = 0.1,\n    gradient_checkpointing: Optional[bool] = False,\n):\n    super().__init__()\n    self.config = LlamaConfig.from_json_file(config_path)\n    self.config.gradient_checkpointing = gradient_checkpointing\n    self.peft_config = AdaLoraConfig(\n        target_r=target_r,\n        init_r=init_r,\n        tinit=tinit,\n        tfinal=tfinal,\n        deltaT=deltaT,\n        beta1=beta1,\n        beta2=beta2,\n        orth_reg_weight=orth_reg_weight,\n        total_step=total_step,\n        rank_pattern=rank_pattern,\n    )\n    self.peft_model = PeftModelForSequenceClassification(\n        LlamaModel(self.config), self.peft_config\n    )\n    self.dropout = nn.Dropout(hidden_dropout_prob)\n    self.classifier = nn.Linear(self.config.hidden_size, num_classes)\n    self.init_weights()\n</code></pre>",
             "title": "LlamaAdaLoraForClassification"
         },
@@ -2347,15 +2442,15 @@
         {
             "location": "models/peft/#unitorch.models.peft.modeling_llama_adalora.LlamaAdaLoraForGeneration.forward",
             "text": "<pre><code>forward(\n    input_ids: torch.Tensor,\n    attention_mask: Optional[torch.Tensor] = None,\n    position_ids: Optional[torch.Tensor] = None,\n)\n</code></pre> <p>Forward pass of the generation model.</p> <p>Parameters:</p> Name Type Description Default <code>input_ids</code> <code>torch.Tensor</code> <p>Input tensor of shape (batch_size, sequence_length). Defaults to None.</p> required <code>attention_mask</code> <code>torch.Tensor</code> <p>Attention mask tensor of shape (batch_size, sequence_length). Defaults to None.</p> <code>None</code> <code>position_ids</code> <code>torch.Tensor</code> <p>Position IDs tensor of shape (batch_size, sequence_length). Defaults to None.</p> <code>None</code> <p>Returns:</p> Type Description <p>torch Output logits.Tensor: tensor of shape (batch_size, sequence_length, vocab_size).</p> Source code in <code>src/unitorch/models/peft/modeling_llama_adalora.py</code> <pre><code>def forward(\n    self,\n    input_ids: torch.Tensor,\n    attention_mask: Optional[torch.Tensor] = None,\n    position_ids: Optional[torch.Tensor] = None,\n):\n\"\"\"\n    Forward pass of the generation model.\n\n    Args:\n        input_ids (torch.Tensor, optional): Input tensor of shape (batch_size, sequence_length). Defaults to None.\n        attention_mask (torch.Tensor, optional): Attention mask tensor of shape (batch_size, sequence_length). Defaults to None.\n        position_ids (torch.Tensor, optional): Position IDs tensor of shape (batch_size, sequence_length). Defaults to None.\n\n    Returns:\n        torch Output logits.Tensor: tensor of shape (batch_size, sequence_length, vocab_size).\n    \"\"\"\n    outputs = self.peft_model(\n        input_ids=input_ids,\n        attention_mask=attention_mask,\n        position_ids=position_ids,\n        return_dict=True,\n    )\n    logits = outputs.logits\n    return logits\n</code></pre>",
             "title": "forward"
         },
         {
             "location": "models/peft/#unitorch.models.peft.modeling_llama_adalora.LlamaAdaLoraForGeneration.generate",
-            "text": "<pre><code>generate(\n    input_ids: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 1,\n    decoder_end_token_id: Optional[int] = 2,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n)\n</code></pre> <p>Generate text using the generation model.</p> <p>Parameters:</p> Name Type Description Default <code>input_ids</code> <code>torch.Tensor</code> <p>Input tensor of shape (batch_size, sequence_length).</p> required <code>num_beams</code> <code>int</code> <p>Number of beams for beam search. Defaults to 5.</p> <code>5</code> <code>decoder_start_token_id</code> <code>int</code> <p>Start token ID for the decoder. Defaults to 2.</p> <code>1</code> <code>decoder_end_token_id</code> <code>int</code> <p>End token ID for the decoder. Defaults to 2.</p> <code>2</code> <code>num_return_sequences</code> <code>int</code> <p>Number of generated sequences to return. Defaults to 1.</p> <code>1</code> <code>min_gen_seq_length</code> <code>int</code> <p>Minimum length of generated sequences. Defaults to 0.</p> <code>0</code> <code>max_gen_seq_length</code> <code>int</code> <p>Maximum length of generated sequences. Defaults to 48.</p> <code>48</code> <code>repetition_penalty</code> <code>float</code> <p>Penalty for repeated tokens. Defaults to 1.0.</p> <code>1.0</code> <code>no_repeat_ngram_size</code> <code>int</code> <p>Size of n-grams to avoid repeating. Defaults to 0.</p> <code>0</code> <code>early_stopping</code> <code>bool</code> <p>Whether to stop generation early. Defaults to True.</p> <code>True</code> <code>length_penalty</code> <code>float</code> <p>Penalty for longer sequences. Defaults to 1.0.</p> <code>1.0</code> <code>num_beam_groups</code> <code>int</code> <p>Number of beam groups for diverse beam search. Defaults to 1.</p> <code>1</code> <code>diversity_penalty</code> <code>float</code> <p>Penalty for diverse sequences in diverse beam search. Defaults to 0.0.</p> <code>0.0</code> <code>do_sample</code> <code>bool</code> <p>Whether to use sampling for generation. Defaults to False.</p> <code>False</code> <code>temperature</code> <code>float</code> <p>Sampling temperature. Defaults to 1.0.</p> <code>1.0</code> <code>top_k</code> <code>int</code> <p>Top-k value for sampling. Defaults to 50.</p> <code>50</code> <code>top_p</code> <code>float</code> <p>Top-p value for sampling. Defaults to 1.0.</p> <code>1.0</code> <p>Returns:</p> Name Type Description <code>GenericOutputs</code> <p>Generated sequences and their scores.</p> Source code in <code>src/unitorch/models/peft/modeling_llama_adalora.py</code> <pre><code>@torch.no_grad()\ndef generate(\n    self,\n    input_ids: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 1,\n    decoder_end_token_id: Optional[int] = 2,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n):\n\"\"\"\n    Generate text using the generation model.\n\n    Args:\n        input_ids: Input tensor of shape (batch_size, sequence_length).\n        num_beams (int, optional): Number of beams for beam search. Defaults to 5.\n        decoder_start_token_id (int, optional): Start token ID for the decoder. Defaults to 2.\n        decoder_end_token_id (int, optional): End token ID for the decoder. Defaults to 2.\n        num_return_sequences (int, optional): Number of generated sequences to return. Defaults to 1.\n        min_gen_seq_length (int, optional): Minimum length of generated sequences. Defaults to 0.\n        max_gen_seq_length (int, optional): Maximum length of generated sequences. Defaults to 48.\n        repetition_penalty (float, optional): Penalty for repeated tokens. Defaults to 1.0.\n        no_repeat_ngram_size (int, optional): Size of n-grams to avoid repeating. Defaults to 0.\n        early_stopping (bool, optional): Whether to stop generation early. Defaults to True.\n        length_penalty (float, optional): Penalty for longer sequences. Defaults to 1.0.\n        num_beam_groups (int, optional): Number of beam groups for diverse beam search. Defaults to 1.\n        diversity_penalty (float, optional): Penalty for diverse sequences in diverse beam search. Defaults to 0.0.\n        do_sample (bool, optional): Whether to use sampling for generation. Defaults to False.\n        temperature (float, optional): Sampling temperature. Defaults to 1.0.\n        top_k (int, optional): Top-k value for sampling. Defaults to 50.\n        top_p (float, optional): Top-p value for sampling. Defaults to 1.0.\n\n    Returns:\n        GenericOutputs: Generated sequences and their scores.\n    \"\"\"\n    input_seq_length = input_ids.size(1)\n    outputs = self.peft_model.generate(\n        input_ids=input_ids,\n        max_length=max_gen_seq_length + input_seq_length,\n        min_length=min_gen_seq_length + input_seq_length,\n        num_beams=num_beams,\n        do_sample=do_sample,\n        decoder_start_token_id=decoder_start_token_id,\n        no_repeat_ngram_size=no_repeat_ngram_size,\n        early_stopping=early_stopping,\n        length_penalty=length_penalty,\n        repetition_penalty=repetition_penalty,\n        num_return_sequences=num_return_sequences,\n        bos_token_id=decoder_start_token_id,\n        eos_token_id=decoder_end_token_id,\n        num_beam_groups=num_beam_groups,\n        diversity_penalty=diversity_penalty,\n        temperature=temperature,\n        top_k=top_k,\n        top_p=top_p,\n        return_dict_in_generate=True,\n        output_scores=True,\n    )\n\n    sequences = outputs.sequences.reshape(\n        -1, num_return_sequences, outputs.sequences.size(-1)\n    )\n    outputs.sequences = torch.zeros(\n        sequences.size(0), num_return_sequences, max_gen_seq_length\n    ).to(device=sequences.device)\n    outputs.sequences[:, :, : sequences.size(-1) - input_seq_length].copy_(\n        sequences[:, :, input_seq_length : sequences.size(-1)]\n    )\n\n    if num_return_sequences == 1:\n        outputs.sequences = outputs.sequences.reshape(-1, max_gen_seq_length)\n\n    return GenericOutputs(\n        sequences=outputs.sequences.long(),\n        sequences_scores=outputs.sequences_scores,\n    )\n</code></pre>",
+            "text": "<pre><code>generate(\n    input_ids: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 1,\n    decoder_end_token_id: Optional[\n        Union[int, List[int]]\n    ] = 2,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n)\n</code></pre> <p>Generate text using the generation model.</p> <p>Parameters:</p> Name Type Description Default <code>input_ids</code> <code>torch.Tensor</code> <p>Input tensor of shape (batch_size, sequence_length).</p> required <code>num_beams</code> <code>int</code> <p>Number of beams for beam search. Defaults to 5.</p> <code>5</code> <code>decoder_start_token_id</code> <code>int</code> <p>The ID of the decoder start token. Defaults to 2.</p> <code>1</code> <code>decoder_end_token_id</code> <code>int or List[int]</code> <p>The ID(s) of the decoder end token(s). Defaults to 2.</p> <code>2</code> <code>num_return_sequences</code> <code>int</code> <p>Number of generated sequences to return. Defaults to 1.</p> <code>1</code> <code>min_gen_seq_length</code> <code>int</code> <p>Minimum length of generated sequences. Defaults to 0.</p> <code>0</code> <code>max_gen_seq_length</code> <code>int</code> <p>Maximum length of generated sequences. Defaults to 48.</p> <code>48</code> <code>repetition_penalty</code> <code>float</code> <p>Penalty for repeated tokens. Defaults to 1.0.</p> <code>1.0</code> <code>no_repeat_ngram_size</code> <code>int</code> <p>Size of n-grams to avoid repeating. Defaults to 0.</p> <code>0</code> <code>early_stopping</code> <code>bool</code> <p>Whether to stop generation early. Defaults to True.</p> <code>True</code> <code>length_penalty</code> <code>float</code> <p>Penalty for longer sequences. Defaults to 1.0.</p> <code>1.0</code> <code>num_beam_groups</code> <code>int</code> <p>Number of beam groups for diverse beam search. Defaults to 1.</p> <code>1</code> <code>diversity_penalty</code> <code>float</code> <p>Penalty for diverse sequences in diverse beam search. Defaults to 0.0.</p> <code>0.0</code> <code>do_sample</code> <code>bool</code> <p>Whether to use sampling for generation. Defaults to False.</p> <code>False</code> <code>temperature</code> <code>float</code> <p>Sampling temperature. Defaults to 1.0.</p> <code>1.0</code> <code>top_k</code> <code>int</code> <p>Top-k value for sampling. Defaults to 50.</p> <code>50</code> <code>top_p</code> <code>float</code> <p>Top-p value for sampling. Defaults to 1.0.</p> <code>1.0</code> <p>Returns:</p> Name Type Description <code>GenericOutputs</code> <p>Generated sequences and their scores.</p> Source code in <code>src/unitorch/models/peft/modeling_llama_adalora.py</code> <pre><code>@torch.no_grad()\ndef generate(\n    self,\n    input_ids: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 1,\n    decoder_end_token_id: Optional[Union[int, List[int]]] = 2,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n):\n\"\"\"\n    Generate text using the generation model.\n\n    Args:\n        input_ids: Input tensor of shape (batch_size, sequence_length).\n        num_beams (int, optional): Number of beams for beam search. Defaults to 5.\n        decoder_start_token_id (int, optional): The ID of the decoder start token. Defaults to 2.\n        decoder_end_token_id (int or List[int], optional): The ID(s) of the decoder end token(s). Defaults to 2.\n        num_return_sequences (int, optional): Number of generated sequences to return. Defaults to 1.\n        min_gen_seq_length (int, optional): Minimum length of generated sequences. Defaults to 0.\n        max_gen_seq_length (int, optional): Maximum length of generated sequences. Defaults to 48.\n        repetition_penalty (float, optional): Penalty for repeated tokens. Defaults to 1.0.\n        no_repeat_ngram_size (int, optional): Size of n-grams to avoid repeating. Defaults to 0.\n        early_stopping (bool, optional): Whether to stop generation early. Defaults to True.\n        length_penalty (float, optional): Penalty for longer sequences. Defaults to 1.0.\n        num_beam_groups (int, optional): Number of beam groups for diverse beam search. Defaults to 1.\n        diversity_penalty (float, optional): Penalty for diverse sequences in diverse beam search. Defaults to 0.0.\n        do_sample (bool, optional): Whether to use sampling for generation. Defaults to False.\n        temperature (float, optional): Sampling temperature. Defaults to 1.0.\n        top_k (int, optional): Top-k value for sampling. Defaults to 50.\n        top_p (float, optional): Top-p value for sampling. Defaults to 1.0.\n\n    Returns:\n        GenericOutputs: Generated sequences and their scores.\n    \"\"\"\n    input_seq_length = input_ids.size(1)\n    outputs = self.peft_model.generate(\n        input_ids=input_ids,\n        max_length=max_gen_seq_length + input_seq_length,\n        min_length=min_gen_seq_length + input_seq_length,\n        num_beams=num_beams,\n        do_sample=do_sample,\n        decoder_start_token_id=decoder_start_token_id,\n        no_repeat_ngram_size=no_repeat_ngram_size,\n        early_stopping=early_stopping,\n        length_penalty=length_penalty,\n        repetition_penalty=repetition_penalty,\n        num_return_sequences=num_return_sequences,\n        bos_token_id=decoder_start_token_id,\n        eos_token_id=decoder_end_token_id,\n        num_beam_groups=num_beam_groups,\n        diversity_penalty=diversity_penalty,\n        temperature=temperature,\n        top_k=top_k,\n        top_p=top_p,\n        return_dict_in_generate=True,\n        output_scores=True,\n    )\n\n    sequences = outputs.sequences.reshape(\n        -1, num_return_sequences, outputs.sequences.size(-1)\n    )\n    outputs.sequences = torch.zeros(\n        sequences.size(0), num_return_sequences, max_gen_seq_length\n    ).to(device=sequences.device)\n    outputs.sequences[:, :, : sequences.size(-1) - input_seq_length].copy_(\n        sequences[:, :, input_seq_length : sequences.size(-1)]\n    )\n\n    if num_return_sequences == 1:\n        outputs.sequences = outputs.sequences.reshape(-1, max_gen_seq_length)\n\n    return GenericOutputs(\n        sequences=outputs.sequences.long(),\n        sequences_scores=outputs.sequences_scores,\n    )\n</code></pre>",
             "title": "generate"
         },
         {
             "location": "models/peft/#llamaloraforclassification",
             "text": "<p>         Bases: <code>GenericModel</code>, <code>PeftCheckpointMixin</code></p> Source code in <code>src/unitorch/models/peft/modeling_llama_lora.py</code> <pre><code>def __init__(\n    self,\n    config_path: str,\n    lora_r: Optional[int] = 16,\n    lora_alpha: Optional[int] = 32,\n    lora_dropout: Optional[float] = 0.05,\n    fan_in_fan_out: Optional[bool] = True,\n    target_modules: Optional[Union[List[str], str]] = [\"q_proj\", \"v_proj\"],\n    num_classes: Optional[int] = 1,\n    hidden_dropout_prob: Optional[float] = 0.1,\n    gradient_checkpointing: Optional[bool] = False,\n):\n    super().__init__()\n    self.config = LlamaConfig.from_json_file(config_path)\n    self.config.gradient_checkpointing = gradient_checkpointing\n    self.peft_config = LoraConfig(\n        r=lora_r,\n        lora_alpha=lora_alpha,\n        lora_dropout=lora_dropout,\n        fan_in_fan_out=fan_in_fan_out,\n        target_modules=target_modules,\n    )\n    self.peft_model = PeftModelForSequenceClassification(\n        LlamaModel(self.config), self.peft_config\n    )\n    self.dropout = nn.Dropout(hidden_dropout_prob)\n    self.classifier = nn.Linear(self.config.hidden_size, num_classes)\n    self.init_weights()\n</code></pre>",
             "title": "LlamaLoraForClassification"
         },
@@ -2372,15 +2467,15 @@
         {
             "location": "models/peft/#unitorch.models.peft.modeling_llama_lora.LlamaLoraForGeneration.forward",
             "text": "<pre><code>forward(\n    input_ids: torch.Tensor,\n    attention_mask: Optional[torch.Tensor] = None,\n    position_ids: Optional[torch.Tensor] = None,\n)\n</code></pre> <p>Forward pass of the generation model.</p> <p>Parameters:</p> Name Type Description Default <code>input_ids</code> <code>torch.Tensor</code> <p>Input tensor of shape (batch_size, sequence_length). Defaults to None.</p> required <code>attention_mask</code> <code>torch.Tensor</code> <p>Attention mask tensor of shape (batch_size, sequence_length). Defaults to None.</p> <code>None</code> <code>position_ids</code> <code>torch.Tensor</code> <p>Position IDs tensor of shape (batch_size, sequence_length). Defaults to None.</p> <code>None</code> <p>Returns:</p> Type Description <p>torch Output logits.Tensor: tensor of shape (batch_size, sequence_length, vocab_size).</p> Source code in <code>src/unitorch/models/peft/modeling_llama_lora.py</code> <pre><code>def forward(\n    self,\n    input_ids: torch.Tensor,\n    attention_mask: Optional[torch.Tensor] = None,\n    position_ids: Optional[torch.Tensor] = None,\n):\n\"\"\"\n    Forward pass of the generation model.\n\n    Args:\n        input_ids (torch.Tensor, optional): Input tensor of shape (batch_size, sequence_length). Defaults to None.\n        attention_mask (torch.Tensor, optional): Attention mask tensor of shape (batch_size, sequence_length). Defaults to None.\n        position_ids (torch.Tensor, optional): Position IDs tensor of shape (batch_size, sequence_length). Defaults to None.\n\n    Returns:\n        torch Output logits.Tensor: tensor of shape (batch_size, sequence_length, vocab_size).\n    \"\"\"\n    outputs = self.peft_model(\n        input_ids=input_ids,\n        attention_mask=attention_mask,\n        position_ids=position_ids,\n        return_dict=True,\n    )\n    logits = outputs.logits\n    return logits\n</code></pre>",
             "title": "forward"
         },
         {
             "location": "models/peft/#unitorch.models.peft.modeling_llama_lora.LlamaLoraForGeneration.generate",
-            "text": "<pre><code>generate(\n    input_ids: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 1,\n    decoder_end_token_id: Optional[int] = 2,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n)\n</code></pre> <p>Generate text using the generation model.</p> <p>Parameters:</p> Name Type Description Default <code>input_ids</code> <code>torch.Tensor</code> <p>Input tensor of shape (batch_size, sequence_length).</p> required <code>num_beams</code> <code>int</code> <p>Number of beams for beam search. Defaults to 5.</p> <code>5</code> <code>decoder_start_token_id</code> <code>int</code> <p>Start token ID for the decoder. Defaults to 2.</p> <code>1</code> <code>decoder_end_token_id</code> <code>int</code> <p>End token ID for the decoder. Defaults to 2.</p> <code>2</code> <code>num_return_sequences</code> <code>int</code> <p>Number of generated sequences to return. Defaults to 1.</p> <code>1</code> <code>min_gen_seq_length</code> <code>int</code> <p>Minimum length of generated sequences. Defaults to 0.</p> <code>0</code> <code>max_gen_seq_length</code> <code>int</code> <p>Maximum length of generated sequences. Defaults to 48.</p> <code>48</code> <code>repetition_penalty</code> <code>float</code> <p>Penalty for repeated tokens. Defaults to 1.0.</p> <code>1.0</code> <code>no_repeat_ngram_size</code> <code>int</code> <p>Size of n-grams to avoid repeating. Defaults to 0.</p> <code>0</code> <code>early_stopping</code> <code>bool</code> <p>Whether to stop generation early. Defaults to True.</p> <code>True</code> <code>length_penalty</code> <code>float</code> <p>Penalty for longer sequences. Defaults to 1.0.</p> <code>1.0</code> <code>num_beam_groups</code> <code>int</code> <p>Number of beam groups for diverse beam search. Defaults to 1.</p> <code>1</code> <code>diversity_penalty</code> <code>float</code> <p>Penalty for diverse sequences in diverse beam search. Defaults to 0.0.</p> <code>0.0</code> <code>do_sample</code> <code>bool</code> <p>Whether to use sampling for generation. Defaults to False.</p> <code>False</code> <code>temperature</code> <code>float</code> <p>Sampling temperature. Defaults to 1.0.</p> <code>1.0</code> <code>top_k</code> <code>int</code> <p>Top-k value for sampling. Defaults to 50.</p> <code>50</code> <code>top_p</code> <code>float</code> <p>Top-p value for sampling. Defaults to 1.0.</p> <code>1.0</code> <p>Returns:</p> Name Type Description <code>GenericOutputs</code> <p>Generated sequences and their scores.</p> Source code in <code>src/unitorch/models/peft/modeling_llama_lora.py</code> <pre><code>@torch.no_grad()\ndef generate(\n    self,\n    input_ids: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 1,\n    decoder_end_token_id: Optional[int] = 2,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n):\n\"\"\"\n    Generate text using the generation model.\n\n    Args:\n        input_ids: Input tensor of shape (batch_size, sequence_length).\n        num_beams (int, optional): Number of beams for beam search. Defaults to 5.\n        decoder_start_token_id (int, optional): Start token ID for the decoder. Defaults to 2.\n        decoder_end_token_id (int, optional): End token ID for the decoder. Defaults to 2.\n        num_return_sequences (int, optional): Number of generated sequences to return. Defaults to 1.\n        min_gen_seq_length (int, optional): Minimum length of generated sequences. Defaults to 0.\n        max_gen_seq_length (int, optional): Maximum length of generated sequences. Defaults to 48.\n        repetition_penalty (float, optional): Penalty for repeated tokens. Defaults to 1.0.\n        no_repeat_ngram_size (int, optional): Size of n-grams to avoid repeating. Defaults to 0.\n        early_stopping (bool, optional): Whether to stop generation early. Defaults to True.\n        length_penalty (float, optional): Penalty for longer sequences. Defaults to 1.0.\n        num_beam_groups (int, optional): Number of beam groups for diverse beam search. Defaults to 1.\n        diversity_penalty (float, optional): Penalty for diverse sequences in diverse beam search. Defaults to 0.0.\n        do_sample (bool, optional): Whether to use sampling for generation. Defaults to False.\n        temperature (float, optional): Sampling temperature. Defaults to 1.0.\n        top_k (int, optional): Top-k value for sampling. Defaults to 50.\n        top_p (float, optional): Top-p value for sampling. Defaults to 1.0.\n\n    Returns:\n        GenericOutputs: Generated sequences and their scores.\n    \"\"\"\n    input_seq_length = input_ids.size(1)\n    outputs = self.peft_model.generate(\n        input_ids=input_ids,\n        max_length=max_gen_seq_length + input_seq_length,\n        min_length=min_gen_seq_length + input_seq_length,\n        num_beams=num_beams,\n        do_sample=do_sample,\n        decoder_start_token_id=decoder_start_token_id,\n        no_repeat_ngram_size=no_repeat_ngram_size,\n        early_stopping=early_stopping,\n        length_penalty=length_penalty,\n        repetition_penalty=repetition_penalty,\n        num_return_sequences=num_return_sequences,\n        bos_token_id=decoder_start_token_id,\n        eos_token_id=decoder_end_token_id,\n        num_beam_groups=num_beam_groups,\n        diversity_penalty=diversity_penalty,\n        temperature=temperature,\n        top_k=top_k,\n        top_p=top_p,\n        return_dict_in_generate=True,\n        output_scores=True,\n    )\n\n    sequences = outputs.sequences.reshape(\n        -1, num_return_sequences, outputs.sequences.size(-1)\n    )\n    outputs.sequences = torch.zeros(\n        sequences.size(0), num_return_sequences, max_gen_seq_length\n    ).to(device=sequences.device)\n    outputs.sequences[:, :, : sequences.size(-1) - input_seq_length].copy_(\n        sequences[:, :, input_seq_length : sequences.size(-1)]\n    )\n\n    if num_return_sequences == 1:\n        outputs.sequences = outputs.sequences.reshape(-1, max_gen_seq_length)\n\n    return GenericOutputs(\n        sequences=outputs.sequences.long(),\n        sequences_scores=outputs.sequences_scores,\n    )\n</code></pre>",
+            "text": "<pre><code>generate(\n    input_ids: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 1,\n    decoder_end_token_id: Optional[\n        Union[int, List[int]]\n    ] = 2,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n)\n</code></pre> <p>Generate text using the generation model.</p> <p>Parameters:</p> Name Type Description Default <code>input_ids</code> <code>torch.Tensor</code> <p>Input tensor of shape (batch_size, sequence_length).</p> required <code>num_beams</code> <code>int</code> <p>Number of beams for beam search. Defaults to 5.</p> <code>5</code> <code>decoder_start_token_id</code> <code>int</code> <p>The ID of the decoder start token. Defaults to 2.</p> <code>1</code> <code>decoder_end_token_id</code> <code>int or List[int]</code> <p>The ID(s) of the decoder end token(s). Defaults to 2.</p> <code>2</code> <code>num_return_sequences</code> <code>int</code> <p>Number of generated sequences to return. Defaults to 1.</p> <code>1</code> <code>min_gen_seq_length</code> <code>int</code> <p>Minimum length of generated sequences. Defaults to 0.</p> <code>0</code> <code>max_gen_seq_length</code> <code>int</code> <p>Maximum length of generated sequences. Defaults to 48.</p> <code>48</code> <code>repetition_penalty</code> <code>float</code> <p>Penalty for repeated tokens. Defaults to 1.0.</p> <code>1.0</code> <code>no_repeat_ngram_size</code> <code>int</code> <p>Size of n-grams to avoid repeating. Defaults to 0.</p> <code>0</code> <code>early_stopping</code> <code>bool</code> <p>Whether to stop generation early. Defaults to True.</p> <code>True</code> <code>length_penalty</code> <code>float</code> <p>Penalty for longer sequences. Defaults to 1.0.</p> <code>1.0</code> <code>num_beam_groups</code> <code>int</code> <p>Number of beam groups for diverse beam search. Defaults to 1.</p> <code>1</code> <code>diversity_penalty</code> <code>float</code> <p>Penalty for diverse sequences in diverse beam search. Defaults to 0.0.</p> <code>0.0</code> <code>do_sample</code> <code>bool</code> <p>Whether to use sampling for generation. Defaults to False.</p> <code>False</code> <code>temperature</code> <code>float</code> <p>Sampling temperature. Defaults to 1.0.</p> <code>1.0</code> <code>top_k</code> <code>int</code> <p>Top-k value for sampling. Defaults to 50.</p> <code>50</code> <code>top_p</code> <code>float</code> <p>Top-p value for sampling. Defaults to 1.0.</p> <code>1.0</code> <p>Returns:</p> Name Type Description <code>GenericOutputs</code> <p>Generated sequences and their scores.</p> Source code in <code>src/unitorch/models/peft/modeling_llama_lora.py</code> <pre><code>@torch.no_grad()\ndef generate(\n    self,\n    input_ids: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 1,\n    decoder_end_token_id: Optional[Union[int, List[int]]] = 2,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n):\n\"\"\"\n    Generate text using the generation model.\n\n    Args:\n        input_ids: Input tensor of shape (batch_size, sequence_length).\n        num_beams (int, optional): Number of beams for beam search. Defaults to 5.\n        decoder_start_token_id (int, optional): The ID of the decoder start token. Defaults to 2.\n        decoder_end_token_id (int or List[int], optional): The ID(s) of the decoder end token(s). Defaults to 2.\n        num_return_sequences (int, optional): Number of generated sequences to return. Defaults to 1.\n        min_gen_seq_length (int, optional): Minimum length of generated sequences. Defaults to 0.\n        max_gen_seq_length (int, optional): Maximum length of generated sequences. Defaults to 48.\n        repetition_penalty (float, optional): Penalty for repeated tokens. Defaults to 1.0.\n        no_repeat_ngram_size (int, optional): Size of n-grams to avoid repeating. Defaults to 0.\n        early_stopping (bool, optional): Whether to stop generation early. Defaults to True.\n        length_penalty (float, optional): Penalty for longer sequences. Defaults to 1.0.\n        num_beam_groups (int, optional): Number of beam groups for diverse beam search. Defaults to 1.\n        diversity_penalty (float, optional): Penalty for diverse sequences in diverse beam search. Defaults to 0.0.\n        do_sample (bool, optional): Whether to use sampling for generation. Defaults to False.\n        temperature (float, optional): Sampling temperature. Defaults to 1.0.\n        top_k (int, optional): Top-k value for sampling. Defaults to 50.\n        top_p (float, optional): Top-p value for sampling. Defaults to 1.0.\n\n    Returns:\n        GenericOutputs: Generated sequences and their scores.\n    \"\"\"\n    input_seq_length = input_ids.size(1)\n    outputs = self.peft_model.generate(\n        input_ids=input_ids,\n        max_length=max_gen_seq_length + input_seq_length,\n        min_length=min_gen_seq_length + input_seq_length,\n        num_beams=num_beams,\n        do_sample=do_sample,\n        decoder_start_token_id=decoder_start_token_id,\n        no_repeat_ngram_size=no_repeat_ngram_size,\n        early_stopping=early_stopping,\n        length_penalty=length_penalty,\n        repetition_penalty=repetition_penalty,\n        num_return_sequences=num_return_sequences,\n        bos_token_id=decoder_start_token_id,\n        eos_token_id=decoder_end_token_id,\n        num_beam_groups=num_beam_groups,\n        diversity_penalty=diversity_penalty,\n        temperature=temperature,\n        top_k=top_k,\n        top_p=top_p,\n        return_dict_in_generate=True,\n        output_scores=True,\n    )\n\n    sequences = outputs.sequences.reshape(\n        -1, num_return_sequences, outputs.sequences.size(-1)\n    )\n    outputs.sequences = torch.zeros(\n        sequences.size(0), num_return_sequences, max_gen_seq_length\n    ).to(device=sequences.device)\n    outputs.sequences[:, :, : sequences.size(-1) - input_seq_length].copy_(\n        sequences[:, :, input_seq_length : sequences.size(-1)]\n    )\n\n    if num_return_sequences == 1:\n        outputs.sequences = outputs.sequences.reshape(-1, max_gen_seq_length)\n\n    return GenericOutputs(\n        sequences=outputs.sequences.long(),\n        sequences_scores=outputs.sequences_scores,\n    )\n</code></pre>",
             "title": "generate"
         },
         {
             "location": "models/pegasus/",
             "text": "",
             "title": "unitorch.models.pegasus"
         },
@@ -2397,15 +2492,15 @@
         {
             "location": "models/pegasus/#unitorch.models.pegasus.modeling.PegasusForGeneration.forward",
             "text": "<pre><code>forward(\n    input_ids: torch.Tensor,\n    attention_mask: torch.Tensor,\n    decoder_input_ids: torch.Tensor,\n    decoder_attention_mask: torch.Tensor,\n)\n</code></pre> <p>Performs a forward pass of the PegasusForGeneration model.</p> <p>Parameters:</p> Name Type Description Default <code>input_ids</code> <code>torch.Tensor</code> <p>Tensor of input token IDs.</p> required <code>attention_mask</code> <code>torch.Tensor</code> <p>Tensor of attention mask.</p> required <code>decoder_input_ids</code> <code>torch.Tensor</code> <p>Tensor of decoder input token IDs.</p> required <code>decoder_attention_mask</code> <code>torch.Tensor</code> <p>Tensor of decoder attention mask.</p> required <p>Returns:</p> Type Description <code>torch.Tensor</code> <p>The model's logits.</p> Source code in <code>src/unitorch/models/pegasus/modeling.py</code> <pre><code>def forward(\n    self,\n    input_ids: torch.Tensor,\n    attention_mask: torch.Tensor,\n    decoder_input_ids: torch.Tensor,\n    decoder_attention_mask: torch.Tensor,\n):\n\"\"\"\n    Performs a forward pass of the PegasusForGeneration model.\n\n    Args:\n        input_ids (torch.Tensor): Tensor of input token IDs.\n        attention_mask (torch.Tensor): Tensor of attention mask.\n        decoder_input_ids (torch.Tensor): Tensor of decoder input token IDs.\n        decoder_attention_mask (torch.Tensor): Tensor of decoder attention mask.\n\n    Returns:\n        (torch.Tensor):The model's logits.\n    \"\"\"\n    outputs = self.model(\n        input_ids=input_ids,\n        attention_mask=attention_mask,\n        decoder_input_ids=decoder_input_ids,\n        decoder_attention_mask=decoder_attention_mask,\n        return_dict=True,\n    )\n    logits = outputs.logits\n    return logits\n</code></pre>",
             "title": "forward"
         },
         {
             "location": "models/pegasus/#unitorch.models.pegasus.modeling.PegasusForGeneration.generate",
-            "text": "<pre><code>generate(\n    input_ids: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 0,\n    decoder_end_token_id: Optional[int] = 1,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n)\n</code></pre> <p>Generates sequences using the PegasusForGeneration model.</p> <p>Parameters:</p> Name Type Description Default <code>input_ids</code> <code>torch.Tensor</code> <p>The input token IDs.</p> required <code>num_beams</code> <code>int</code> <p>The number of beams for beam search. Defaults to 5.</p> <code>5</code> <code>decoder_start_token_id</code> <code>int</code> <p>The decoder's start token ID. Defaults to 2.</p> <code>0</code> <code>decoder_end_token_id</code> <code>int</code> <p>The decoder's end token ID. Defaults to 2.</p> <code>1</code> <code>num_return_sequences</code> <code>int</code> <p>The number of generated sequences to return. Defaults to 1.</p> <code>1</code> <code>min_gen_seq_length</code> <code>int</code> <p>The minimum length of the generated sequences. Defaults to 0.</p> <code>0</code> <code>max_gen_seq_length</code> <code>int</code> <p>The maximum length of the generated sequences. Defaults to 48.</p> <code>48</code> <code>repetition_penalty</code> <code>float</code> <p>The repetition penalty. Defaults to 1.0.</p> <code>1.0</code> <code>no_repeat_ngram_size</code> <code>int</code> <p>The size of n-grams to avoid repeating. Defaults to 0.</p> <code>0</code> <code>early_stopping</code> <code>bool</code> <p>Whether to stop generation early. Defaults to True.</p> <code>True</code> <code>length_penalty</code> <code>float</code> <p>The length penalty. Defaults to 1.0.</p> <code>1.0</code> <code>num_beam_groups</code> <code>int</code> <p>The number of beam groups for diverse beam search. Defaults to 1.</p> <code>1</code> <code>diversity_penalty</code> <code>float</code> <p>The diversity penalty. Defaults to 0.0.</p> <code>0.0</code> <code>do_sample</code> <code>bool</code> <p>Whether to use sampling for generation. Defaults to False.</p> <code>False</code> <code>temperature</code> <code>float</code> <p>The temperature for sampling. Defaults to 1.0.</p> <code>1.0</code> <code>top_k</code> <code>int</code> <p>The value for top-k sampling. Defaults to 50.</p> <code>50</code> <code>top_p</code> <code>float</code> <p>The value for top-p (nucleus) sampling. Defaults to 1.0.</p> <code>1.0</code> <p>Returns:</p> Name Type Description <code>GenericOutputs</code> <p>The generated sequences and their scores.</p> Source code in <code>src/unitorch/models/pegasus/modeling.py</code> <pre><code>@torch.no_grad()\ndef generate(\n    self,\n    input_ids: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 0,\n    decoder_end_token_id: Optional[int] = 1,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n):\n\"\"\"\n    Generates sequences using the PegasusForGeneration model.\n\n    Args:\n        input_ids: The input token IDs.\n        num_beams (int, optional): The number of beams for beam search. Defaults to 5.\n        decoder_start_token_id (int, optional): The decoder's start token ID. Defaults to 2.\n        decoder_end_token_id (int, optional): The decoder's end token ID. Defaults to 2.\n        num_return_sequences (int, optional): The number of generated sequences to return. Defaults to 1.\n        min_gen_seq_length (int, optional): The minimum length of the generated sequences. Defaults to 0.\n        max_gen_seq_length (int, optional): The maximum length of the generated sequences. Defaults to 48.\n        repetition_penalty (float, optional): The repetition penalty. Defaults to 1.0.\n        no_repeat_ngram_size (int, optional): The size of n-grams to avoid repeating. Defaults to 0.\n        early_stopping (bool, optional): Whether to stop generation early. Defaults to True.\n        length_penalty (float, optional): The length penalty. Defaults to 1.0.\n        num_beam_groups (int, optional): The number of beam groups for diverse beam search. Defaults to 1.\n        diversity_penalty (float, optional): The diversity penalty. Defaults to 0.0.\n        do_sample (bool, optional): Whether to use sampling for generation. Defaults to False.\n        temperature (float, optional): The temperature for sampling. Defaults to 1.0.\n        top_k (int, optional): The value for top-k sampling. Defaults to 50.\n        top_p (float, optional): The value for top-p (nucleus) sampling. Defaults to 1.0.\n\n    Returns:\n        GenericOutputs: The generated sequences and their scores.\n    \"\"\"\n    outputs = self.model.generate(\n        input_ids,\n        max_length=max_gen_seq_length,\n        min_length=min_gen_seq_length,\n        num_beams=num_beams,\n        do_sample=do_sample,\n        decoder_start_token_id=decoder_start_token_id,\n        no_repeat_ngram_size=no_repeat_ngram_size,\n        early_stopping=early_stopping,\n        length_penalty=length_penalty,\n        repetition_penalty=repetition_penalty,\n        num_return_sequences=num_return_sequences,\n        bos_token_id=decoder_start_token_id,\n        eos_token_id=decoder_end_token_id,\n        num_beam_groups=num_beam_groups,\n        diversity_penalty=diversity_penalty,\n        temperature=temperature,\n        top_k=top_k,\n        top_p=top_p,\n        return_dict_in_generate=True,\n        output_scores=True,\n    )\n\n    sequences = outputs.sequences.reshape(\n        -1, num_return_sequences, outputs.sequences.size(-1)\n    )\n    outputs.sequences = torch.zeros(\n        sequences.size(0), num_return_sequences, max_gen_seq_length\n    ).to(device=sequences.device)\n    outputs.sequences[:, :, : sequences.size(-1)].copy_(sequences)\n\n    if num_return_sequences == 1:\n        outputs.sequences = outputs.sequences.reshape(-1, max_gen_seq_length)\n\n    return GenericOutputs(\n        sequences=outputs.sequences,\n        sequences_scores=outputs.sequences_scores,\n    )\n</code></pre>",
+            "text": "<pre><code>generate(\n    input_ids: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 0,\n    decoder_end_token_id: Optional[\n        Union[int, List[int]]\n    ] = 1,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n)\n</code></pre> <p>Generates sequences using the PegasusForGeneration model.</p> <p>Parameters:</p> Name Type Description Default <code>input_ids</code> <code>torch.Tensor</code> <p>The input token IDs.</p> required <code>num_beams</code> <code>int</code> <p>The number of beams for beam search. Defaults to 5.</p> <code>5</code> <code>decoder_start_token_id</code> <code>int</code> <p>The decoder's start token ID. Defaults to 2.</p> <code>0</code> <code>decoder_end_token_id</code> <code>int or List[int]</code> <p>The decoder's end token ID. Defaults to 2.</p> <code>1</code> <code>num_return_sequences</code> <code>int</code> <p>The number of generated sequences to return. Defaults to 1.</p> <code>1</code> <code>min_gen_seq_length</code> <code>int</code> <p>The minimum length of the generated sequences. Defaults to 0.</p> <code>0</code> <code>max_gen_seq_length</code> <code>int</code> <p>The maximum length of the generated sequences. Defaults to 48.</p> <code>48</code> <code>repetition_penalty</code> <code>float</code> <p>The repetition penalty. Defaults to 1.0.</p> <code>1.0</code> <code>no_repeat_ngram_size</code> <code>int</code> <p>The size of n-grams to avoid repeating. Defaults to 0.</p> <code>0</code> <code>early_stopping</code> <code>bool</code> <p>Whether to stop generation early. Defaults to True.</p> <code>True</code> <code>length_penalty</code> <code>float</code> <p>The length penalty. Defaults to 1.0.</p> <code>1.0</code> <code>num_beam_groups</code> <code>int</code> <p>The number of beam groups for diverse beam search. Defaults to 1.</p> <code>1</code> <code>diversity_penalty</code> <code>float</code> <p>The diversity penalty. Defaults to 0.0.</p> <code>0.0</code> <code>do_sample</code> <code>bool</code> <p>Whether to use sampling for generation. Defaults to False.</p> <code>False</code> <code>temperature</code> <code>float</code> <p>The temperature for sampling. Defaults to 1.0.</p> <code>1.0</code> <code>top_k</code> <code>int</code> <p>The value for top-k sampling. Defaults to 50.</p> <code>50</code> <code>top_p</code> <code>float</code> <p>The value for top-p (nucleus) sampling. Defaults to 1.0.</p> <code>1.0</code> <p>Returns:</p> Name Type Description <code>GenericOutputs</code> <p>The generated sequences and their scores.</p> Source code in <code>src/unitorch/models/pegasus/modeling.py</code> <pre><code>@torch.no_grad()\ndef generate(\n    self,\n    input_ids: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 0,\n    decoder_end_token_id: Optional[Union[int, List[int]]] = 1,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n):\n\"\"\"\n    Generates sequences using the PegasusForGeneration model.\n\n    Args:\n        input_ids: The input token IDs.\n        num_beams (int, optional): The number of beams for beam search. Defaults to 5.\n        decoder_start_token_id (int, optional): The decoder's start token ID. Defaults to 2.\n        decoder_end_token_id (int or List[int], optional): The decoder's end token ID. Defaults to 2.\n        num_return_sequences (int, optional): The number of generated sequences to return. Defaults to 1.\n        min_gen_seq_length (int, optional): The minimum length of the generated sequences. Defaults to 0.\n        max_gen_seq_length (int, optional): The maximum length of the generated sequences. Defaults to 48.\n        repetition_penalty (float, optional): The repetition penalty. Defaults to 1.0.\n        no_repeat_ngram_size (int, optional): The size of n-grams to avoid repeating. Defaults to 0.\n        early_stopping (bool, optional): Whether to stop generation early. Defaults to True.\n        length_penalty (float, optional): The length penalty. Defaults to 1.0.\n        num_beam_groups (int, optional): The number of beam groups for diverse beam search. Defaults to 1.\n        diversity_penalty (float, optional): The diversity penalty. Defaults to 0.0.\n        do_sample (bool, optional): Whether to use sampling for generation. Defaults to False.\n        temperature (float, optional): The temperature for sampling. Defaults to 1.0.\n        top_k (int, optional): The value for top-k sampling. Defaults to 50.\n        top_p (float, optional): The value for top-p (nucleus) sampling. Defaults to 1.0.\n\n    Returns:\n        GenericOutputs: The generated sequences and their scores.\n    \"\"\"\n    outputs = self.model.generate(\n        input_ids,\n        max_length=max_gen_seq_length,\n        min_length=min_gen_seq_length,\n        num_beams=num_beams,\n        do_sample=do_sample,\n        decoder_start_token_id=decoder_start_token_id,\n        no_repeat_ngram_size=no_repeat_ngram_size,\n        early_stopping=early_stopping,\n        length_penalty=length_penalty,\n        repetition_penalty=repetition_penalty,\n        num_return_sequences=num_return_sequences,\n        bos_token_id=decoder_start_token_id,\n        eos_token_id=decoder_end_token_id,\n        num_beam_groups=num_beam_groups,\n        diversity_penalty=diversity_penalty,\n        temperature=temperature,\n        top_k=top_k,\n        top_p=top_p,\n        return_dict_in_generate=True,\n        output_scores=True,\n    )\n\n    sequences = outputs.sequences.reshape(\n        -1, num_return_sequences, outputs.sequences.size(-1)\n    )\n    outputs.sequences = torch.zeros(\n        sequences.size(0), num_return_sequences, max_gen_seq_length\n    ).to(device=sequences.device)\n    outputs.sequences[:, :, : sequences.size(-1)].copy_(sequences)\n\n    if num_return_sequences == 1:\n        outputs.sequences = outputs.sequences.reshape(-1, max_gen_seq_length)\n\n    return GenericOutputs(\n        sequences=outputs.sequences,\n        sequences_scores=outputs.sequences_scores,\n    )\n</code></pre>",
             "title": "generate"
         },
         {
             "location": "models/prophetnet/",
             "text": "",
             "title": "unitorch.models.prophetnet"
         },
@@ -2482,15 +2577,15 @@
         {
             "location": "models/t5/#unitorch.models.t5.modeling.T5ForGeneration.forward",
             "text": "<pre><code>forward(\n    input_ids: torch.Tensor,\n    attention_mask: torch.Tensor,\n    decoder_input_ids: torch.Tensor,\n    decoder_attention_mask: torch.Tensor,\n)\n</code></pre> <p>Performs forward pass of the T5ForGeneration model.</p> <p>Parameters:</p> Name Type Description Default <code>input_ids</code> <code>torch.Tensor</code> <p>Tensor of input token IDs.</p> required <code>attention_mask</code> <code>torch.Tensor</code> <p>Tensor of attention mask.</p> required <code>decoder_input_ids</code> <code>torch.Tensor</code> <p>Tensor of decoder input token IDs.</p> required <code>decoder_attention_mask</code> <code>torch.Tensor</code> <p>Tensor of decoder attention mask.</p> required <p>Returns:</p> Type Description <code>torch.Tensor</code> <p>The model's logits.</p> Source code in <code>src/unitorch/models/t5/modeling.py</code> <pre><code>def forward(\n    self,\n    input_ids: torch.Tensor,\n    attention_mask: torch.Tensor,\n    decoder_input_ids: torch.Tensor,\n    decoder_attention_mask: torch.Tensor,\n):\n\"\"\"\n    Performs forward pass of the T5ForGeneration model.\n\n    Args:\n        input_ids (torch.Tensor): Tensor of input token IDs.\n        attention_mask (torch.Tensor): Tensor of attention mask.\n        decoder_input_ids (torch.Tensor): Tensor of decoder input token IDs.\n        decoder_attention_mask (torch.Tensor): Tensor of decoder attention mask.\n\n    Returns:\n        (torch.Tensor):The model's logits.\n    \"\"\"\n    outputs = self.model(\n        input_ids=input_ids,\n        attention_mask=attention_mask,\n        decoder_input_ids=decoder_input_ids,\n        decoder_attention_mask=decoder_attention_mask,\n        return_dict=True,\n    )\n    logits = outputs.logits\n    return logits\n</code></pre>",
             "title": "forward"
         },
         {
             "location": "models/t5/#unitorch.models.t5.modeling.T5ForGeneration.generate",
-            "text": "<pre><code>generate(\n    input_ids: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 0,\n    decoder_end_token_id: Optional[int] = 1,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n)\n</code></pre> <p>Generates sequences using the T5ForGeneration model.</p> <p>Parameters:</p> Name Type Description Default <code>input_ids</code> <code>torch.Tensor</code> <p>The input token IDs.</p> required <code>num_beams</code> <code>int</code> <p>The number of beams for beam search. Defaults to 5.</p> <code>5</code> <code>decoder_start_token_id</code> <code>int</code> <p>The decoder's start token ID. Defaults to 2.</p> <code>0</code> <code>decoder_end_token_id</code> <code>int</code> <p>The decoder's end token ID. Defaults to 2.</p> <code>1</code> <code>num_return_sequences</code> <code>int</code> <p>The number of generated sequences to return. Defaults to 1.</p> <code>1</code> <code>min_gen_seq_length</code> <code>int</code> <p>The minimum length of the generated sequences. Defaults to 0.</p> <code>0</code> <code>max_gen_seq_length</code> <code>int</code> <p>The maximum length of the generated sequences. Defaults to 48.</p> <code>48</code> <code>repetition_penalty</code> <code>float</code> <p>The repetition penalty. Defaults to 1.0.</p> <code>1.0</code> <code>no_repeat_ngram_size</code> <code>int</code> <p>The size of n-grams to avoid repeating. Defaults to 0.</p> <code>0</code> <code>early_stopping</code> <code>bool</code> <p>Whether to stop generation early. Defaults to True.</p> <code>True</code> <code>length_penalty</code> <code>float</code> <p>The length penalty. Defaults to 1.0.</p> <code>1.0</code> <code>num_beam_groups</code> <code>int</code> <p>The number of beam groups for diverse beam search. Defaults to 1.</p> <code>1</code> <code>diversity_penalty</code> <code>float</code> <p>The diversity penalty. Defaults to 0.0.</p> <code>0.0</code> <code>do_sample</code> <code>bool</code> <p>Whether to use sampling for generation. Defaults to False.</p> <code>False</code> <code>temperature</code> <code>float</code> <p>The temperature for sampling. Defaults to 1.0.</p> <code>1.0</code> <code>top_k</code> <code>int</code> <p>The value for top-k sampling. Defaults to 50.</p> <code>50</code> <code>top_p</code> <code>float</code> <p>The value for top-p (nucleus) sampling. Defaults to 1.0.</p> <code>1.0</code> <p>Returns:</p> Name Type Description <code>GenericOutputs</code> <p>The generated sequences and their scores.</p> Source code in <code>src/unitorch/models/t5/modeling.py</code> <pre><code>@torch.no_grad()\ndef generate(\n    self,\n    input_ids: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 0,\n    decoder_end_token_id: Optional[int] = 1,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n):\n\"\"\"\n    Generates sequences using the T5ForGeneration model.\n\n    Args:\n        input_ids: The input token IDs.\n        num_beams (int, optional): The number of beams for beam search. Defaults to 5.\n        decoder_start_token_id (int, optional): The decoder's start token ID. Defaults to 2.\n        decoder_end_token_id (int, optional): The decoder's end token ID. Defaults to 2.\n        num_return_sequences (int, optional): The number of generated sequences to return. Defaults to 1.\n        min_gen_seq_length (int, optional): The minimum length of the generated sequences. Defaults to 0.\n        max_gen_seq_length (int, optional): The maximum length of the generated sequences. Defaults to 48.\n        repetition_penalty (float, optional): The repetition penalty. Defaults to 1.0.\n        no_repeat_ngram_size (int, optional): The size of n-grams to avoid repeating. Defaults to 0.\n        early_stopping (bool, optional): Whether to stop generation early. Defaults to True.\n        length_penalty (float, optional): The length penalty. Defaults to 1.0.\n        num_beam_groups (int, optional): The number of beam groups for diverse beam search. Defaults to 1.\n        diversity_penalty (float, optional): The diversity penalty. Defaults to 0.0.\n        do_sample (bool, optional): Whether to use sampling for generation. Defaults to False.\n        temperature (float, optional): The temperature for sampling. Defaults to 1.0.\n        top_k (int, optional): The value for top-k sampling. Defaults to 50.\n        top_p (float, optional): The value for top-p (nucleus) sampling. Defaults to 1.0.\n\n    Returns:\n        GenericOutputs: The generated sequences and their scores.\n    \"\"\"\n    outputs = self.model.generate(\n        input_ids,\n        max_length=max_gen_seq_length,\n        min_length=min_gen_seq_length,\n        num_beams=num_beams,\n        do_sample=do_sample,\n        decoder_start_token_id=decoder_start_token_id,\n        no_repeat_ngram_size=no_repeat_ngram_size,\n        early_stopping=early_stopping,\n        length_penalty=length_penalty,\n        repetition_penalty=repetition_penalty,\n        num_return_sequences=num_return_sequences,\n        bos_token_id=decoder_start_token_id,\n        eos_token_id=decoder_end_token_id,\n        num_beam_groups=num_beam_groups,\n        diversity_penalty=diversity_penalty,\n        temperature=temperature,\n        top_k=top_k,\n        top_p=top_p,\n        return_dict_in_generate=True,\n        output_scores=True,\n    )\n\n    sequences = outputs.sequences.reshape(\n        -1, num_return_sequences, outputs.sequences.size(-1)\n    )\n    outputs.sequences = torch.zeros(\n        sequences.size(0), num_return_sequences, max_gen_seq_length\n    ).to(device=sequences.device)\n    outputs.sequences[:, :, : sequences.size(-1)].copy_(sequences)\n\n    if num_return_sequences == 1:\n        outputs.sequences = outputs.sequences.reshape(-1, max_gen_seq_length)\n\n    return GenericOutputs(\n        sequences=outputs.sequences,\n        sequences_scores=outputs.sequences_scores,\n    )\n</code></pre>",
+            "text": "<pre><code>generate(\n    input_ids: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 0,\n    decoder_end_token_id: Optional[\n        Union[int, List[int]]\n    ] = 1,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n)\n</code></pre> <p>Generates sequences using the T5ForGeneration model.</p> <p>Parameters:</p> Name Type Description Default <code>input_ids</code> <code>torch.Tensor</code> <p>The input token IDs.</p> required <code>num_beams</code> <code>int</code> <p>The number of beams for beam search. Defaults to 5.</p> <code>5</code> <code>decoder_start_token_id</code> <code>int</code> <p>The decoder's start token ID. Defaults to 2.</p> <code>0</code> <code>decoder_end_token_id</code> <code>int or List[int]</code> <p>The decoder's end token ID. Defaults to 2.</p> <code>1</code> <code>num_return_sequences</code> <code>int</code> <p>The number of generated sequences to return. Defaults to 1.</p> <code>1</code> <code>min_gen_seq_length</code> <code>int</code> <p>The minimum length of the generated sequences. Defaults to 0.</p> <code>0</code> <code>max_gen_seq_length</code> <code>int</code> <p>The maximum length of the generated sequences. Defaults to 48.</p> <code>48</code> <code>repetition_penalty</code> <code>float</code> <p>The repetition penalty. Defaults to 1.0.</p> <code>1.0</code> <code>no_repeat_ngram_size</code> <code>int</code> <p>The size of n-grams to avoid repeating. Defaults to 0.</p> <code>0</code> <code>early_stopping</code> <code>bool</code> <p>Whether to stop generation early. Defaults to True.</p> <code>True</code> <code>length_penalty</code> <code>float</code> <p>The length penalty. Defaults to 1.0.</p> <code>1.0</code> <code>num_beam_groups</code> <code>int</code> <p>The number of beam groups for diverse beam search. Defaults to 1.</p> <code>1</code> <code>diversity_penalty</code> <code>float</code> <p>The diversity penalty. Defaults to 0.0.</p> <code>0.0</code> <code>do_sample</code> <code>bool</code> <p>Whether to use sampling for generation. Defaults to False.</p> <code>False</code> <code>temperature</code> <code>float</code> <p>The temperature for sampling. Defaults to 1.0.</p> <code>1.0</code> <code>top_k</code> <code>int</code> <p>The value for top-k sampling. Defaults to 50.</p> <code>50</code> <code>top_p</code> <code>float</code> <p>The value for top-p (nucleus) sampling. Defaults to 1.0.</p> <code>1.0</code> <p>Returns:</p> Name Type Description <code>GenericOutputs</code> <p>The generated sequences and their scores.</p> Source code in <code>src/unitorch/models/t5/modeling.py</code> <pre><code>@torch.no_grad()\ndef generate(\n    self,\n    input_ids: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 0,\n    decoder_end_token_id: Optional[Union[int, List[int]]] = 1,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n):\n\"\"\"\n    Generates sequences using the T5ForGeneration model.\n\n    Args:\n        input_ids: The input token IDs.\n        num_beams (int, optional): The number of beams for beam search. Defaults to 5.\n        decoder_start_token_id (int, optional): The decoder's start token ID. Defaults to 2.\n        decoder_end_token_id (int or List[int], optional): The decoder's end token ID. Defaults to 2.\n        num_return_sequences (int, optional): The number of generated sequences to return. Defaults to 1.\n        min_gen_seq_length (int, optional): The minimum length of the generated sequences. Defaults to 0.\n        max_gen_seq_length (int, optional): The maximum length of the generated sequences. Defaults to 48.\n        repetition_penalty (float, optional): The repetition penalty. Defaults to 1.0.\n        no_repeat_ngram_size (int, optional): The size of n-grams to avoid repeating. Defaults to 0.\n        early_stopping (bool, optional): Whether to stop generation early. Defaults to True.\n        length_penalty (float, optional): The length penalty. Defaults to 1.0.\n        num_beam_groups (int, optional): The number of beam groups for diverse beam search. Defaults to 1.\n        diversity_penalty (float, optional): The diversity penalty. Defaults to 0.0.\n        do_sample (bool, optional): Whether to use sampling for generation. Defaults to False.\n        temperature (float, optional): The temperature for sampling. Defaults to 1.0.\n        top_k (int, optional): The value for top-k sampling. Defaults to 50.\n        top_p (float, optional): The value for top-p (nucleus) sampling. Defaults to 1.0.\n\n    Returns:\n        GenericOutputs: The generated sequences and their scores.\n    \"\"\"\n    outputs = self.model.generate(\n        input_ids,\n        max_length=max_gen_seq_length,\n        min_length=min_gen_seq_length,\n        num_beams=num_beams,\n        do_sample=do_sample,\n        decoder_start_token_id=decoder_start_token_id,\n        no_repeat_ngram_size=no_repeat_ngram_size,\n        early_stopping=early_stopping,\n        length_penalty=length_penalty,\n        repetition_penalty=repetition_penalty,\n        num_return_sequences=num_return_sequences,\n        bos_token_id=decoder_start_token_id,\n        eos_token_id=decoder_end_token_id,\n        num_beam_groups=num_beam_groups,\n        diversity_penalty=diversity_penalty,\n        temperature=temperature,\n        top_k=top_k,\n        top_p=top_p,\n        return_dict_in_generate=True,\n        output_scores=True,\n    )\n\n    sequences = outputs.sequences.reshape(\n        -1, num_return_sequences, outputs.sequences.size(-1)\n    )\n    outputs.sequences = torch.zeros(\n        sequences.size(0), num_return_sequences, max_gen_seq_length\n    ).to(device=sequences.device)\n    outputs.sequences[:, :, : sequences.size(-1)].copy_(sequences)\n\n    if num_return_sequences == 1:\n        outputs.sequences = outputs.sequences.reshape(-1, max_gen_seq_length)\n\n    return GenericOutputs(\n        sequences=outputs.sequences,\n        sequences_scores=outputs.sequences_scores,\n    )\n</code></pre>",
             "title": "generate"
         },
         {
             "location": "models/visualbert/",
             "text": "",
             "title": "unitorch.models.visualbert"
         },
@@ -2607,15 +2702,15 @@
         {
             "location": "models/xpegasus/#unitorch.models.xpegasus.modeling.XPegasusForGeneration.forward",
             "text": "<pre><code>forward(\n    input_ids: torch.Tensor,\n    attention_mask: torch.Tensor,\n    decoder_input_ids: torch.Tensor,\n    decoder_attention_mask: torch.Tensor,\n)\n</code></pre> <p>Performs forward pass of the XPegasusForGeneration model.</p> <p>Parameters:</p> Name Type Description Default <code>input_ids</code> <code>torch.Tensor</code> <p>Tensor of input token IDs.</p> required <code>attention_mask</code> <code>torch.Tensor</code> <p>Tensor of attention mask.</p> required <code>decoder_input_ids</code> <code>torch.Tensor</code> <p>Tensor of decoder input token IDs.</p> required <code>decoder_attention_mask</code> <code>torch.Tensor</code> <p>Tensor of decoder attention mask.</p> required <p>Returns:</p> Type Description <code>torch.Tensor</code> <p>The model's logits.</p> Source code in <code>src/unitorch/models/xpegasus/modeling.py</code> <pre><code>def forward(\n    self,\n    input_ids: torch.Tensor,\n    attention_mask: torch.Tensor,\n    decoder_input_ids: torch.Tensor,\n    decoder_attention_mask: torch.Tensor,\n):\n\"\"\"\n    Performs forward pass of the XPegasusForGeneration model.\n\n    Args:\n        input_ids (torch.Tensor): Tensor of input token IDs.\n        attention_mask (torch.Tensor): Tensor of attention mask.\n        decoder_input_ids (torch.Tensor): Tensor of decoder input token IDs.\n        decoder_attention_mask (torch.Tensor): Tensor of decoder attention mask.\n\n    Returns:\n        (torch.Tensor):The model's logits.\n    \"\"\"\n    outputs = self.model(\n        input_ids=input_ids,\n        attention_mask=attention_mask,\n        decoder_input_ids=decoder_input_ids,\n        decoder_attention_mask=decoder_attention_mask,\n        return_dict=True,\n    )\n    logits = outputs.logits\n    return logits\n</code></pre>",
             "title": "forward"
         },
         {
             "location": "models/xpegasus/#unitorch.models.xpegasus.modeling.XPegasusForGeneration.generate",
-            "text": "<pre><code>generate(\n    input_ids: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 0,\n    decoder_end_token_id: Optional[int] = 1,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n)\n</code></pre> <p>Generates sequences using the XPegasusForGeneration model.</p> <p>Parameters:</p> Name Type Description Default <code>input_ids</code> <code>torch.Tensor</code> <p>The input token IDs.</p> required <code>num_beams</code> <code>int</code> <p>The number of beams for beam search. Defaults to 5.</p> <code>5</code> <code>decoder_start_token_id</code> <code>int</code> <p>The decoder's start token ID. Defaults to 2.</p> <code>0</code> <code>decoder_end_token_id</code> <code>int</code> <p>The decoder's end token ID. Defaults to 2.</p> <code>1</code> <code>num_return_sequences</code> <code>int</code> <p>The number of generated sequences to return. Defaults to 1.</p> <code>1</code> <code>min_gen_seq_length</code> <code>int</code> <p>The minimum length of the generated sequences. Defaults to 0.</p> <code>0</code> <code>max_gen_seq_length</code> <code>int</code> <p>The maximum length of the generated sequences. Defaults to 48.</p> <code>48</code> <code>repetition_penalty</code> <code>float</code> <p>The repetition penalty. Defaults to 1.0.</p> <code>1.0</code> <code>no_repeat_ngram_size</code> <code>int</code> <p>The size of n-grams to avoid repeating. Defaults to 0.</p> <code>0</code> <code>early_stopping</code> <code>bool</code> <p>Whether to stop generation early. Defaults to True.</p> <code>True</code> <code>length_penalty</code> <code>float</code> <p>The length penalty. Defaults to 1.0.</p> <code>1.0</code> <code>num_beam_groups</code> <code>int</code> <p>The number of beam groups for diverse beam search. Defaults to 1.</p> <code>1</code> <code>diversity_penalty</code> <code>float</code> <p>The diversity penalty. Defaults to 0.0.</p> <code>0.0</code> <code>do_sample</code> <code>bool</code> <p>Whether to use sampling for generation. Defaults to False.</p> <code>False</code> <code>temperature</code> <code>float</code> <p>The temperature for sampling. Defaults to 1.0.</p> <code>1.0</code> <code>top_k</code> <code>int</code> <p>The value for top-k sampling. Defaults to 50.</p> <code>50</code> <code>top_p</code> <code>float</code> <p>The value for top-p (nucleus) sampling. Defaults to 1.0.</p> <code>1.0</code> <p>Returns:</p> Name Type Description <code>GenericOutputs</code> <p>The generated sequences and their scores.</p> Source code in <code>src/unitorch/models/xpegasus/modeling.py</code> <pre><code>@torch.no_grad()\ndef generate(\n    self,\n    input_ids: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 0,\n    decoder_end_token_id: Optional[int] = 1,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n):\n\"\"\"\n    Generates sequences using the XPegasusForGeneration model.\n\n    Args:\n        input_ids: The input token IDs.\n        num_beams (int, optional): The number of beams for beam search. Defaults to 5.\n        decoder_start_token_id (int, optional): The decoder's start token ID. Defaults to 2.\n        decoder_end_token_id (int, optional): The decoder's end token ID. Defaults to 2.\n        num_return_sequences (int, optional): The number of generated sequences to return. Defaults to 1.\n        min_gen_seq_length (int, optional): The minimum length of the generated sequences. Defaults to 0.\n        max_gen_seq_length (int, optional): The maximum length of the generated sequences. Defaults to 48.\n        repetition_penalty (float, optional): The repetition penalty. Defaults to 1.0.\n        no_repeat_ngram_size (int, optional): The size of n-grams to avoid repeating. Defaults to 0.\n        early_stopping (bool, optional): Whether to stop generation early. Defaults to True.\n        length_penalty (float, optional): The length penalty. Defaults to 1.0.\n        num_beam_groups (int, optional): The number of beam groups for diverse beam search. Defaults to 1.\n        diversity_penalty (float, optional): The diversity penalty. Defaults to 0.0.\n        do_sample (bool, optional): Whether to use sampling for generation. Defaults to False.\n        temperature (float, optional): The temperature for sampling. Defaults to 1.0.\n        top_k (int, optional): The value for top-k sampling. Defaults to 50.\n        top_p (float, optional): The value for top-p (nucleus) sampling. Defaults to 1.0.\n\n    Returns:\n        GenericOutputs: The generated sequences and their scores.\n    \"\"\"\n    outputs = self.model.generate(\n        input_ids,\n        max_length=max_gen_seq_length,\n        min_length=min_gen_seq_length,\n        num_beams=num_beams,\n        do_sample=do_sample,\n        decoder_start_token_id=decoder_start_token_id,\n        no_repeat_ngram_size=no_repeat_ngram_size,\n        early_stopping=early_stopping,\n        length_penalty=length_penalty,\n        repetition_penalty=repetition_penalty,\n        num_return_sequences=num_return_sequences,\n        bos_token_id=decoder_start_token_id,\n        eos_token_id=decoder_end_token_id,\n        num_beam_groups=num_beam_groups,\n        diversity_penalty=diversity_penalty,\n        temperature=temperature,\n        top_k=top_k,\n        top_p=top_p,\n        return_dict_in_generate=True,\n        output_scores=True,\n    )\n\n    sequences = outputs.sequences.reshape(\n        -1, num_return_sequences, outputs.sequences.size(-1)\n    )\n    outputs.sequences = torch.zeros(\n        sequences.size(0), num_return_sequences, max_gen_seq_length\n    ).to(device=sequences.device)\n    outputs.sequences[:, :, : sequences.size(-1)].copy_(sequences)\n\n    if num_return_sequences == 1:\n        outputs.sequences = outputs.sequences.reshape(-1, max_gen_seq_length)\n\n    return GenericOutputs(\n        sequences=outputs.sequences,\n        sequences_scores=outputs.sequences_scores,\n    )\n</code></pre>",
+            "text": "<pre><code>generate(\n    input_ids: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 0,\n    decoder_end_token_id: Optional[\n        Union[int, List[int]]\n    ] = 1,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n)\n</code></pre> <p>Generates sequences using the XPegasusForGeneration model.</p> <p>Parameters:</p> Name Type Description Default <code>input_ids</code> <code>torch.Tensor</code> <p>The input token IDs.</p> required <code>num_beams</code> <code>int</code> <p>The number of beams for beam search. Defaults to 5.</p> <code>5</code> <code>decoder_start_token_id</code> <code>int</code> <p>The decoder's start token ID. Defaults to 2.</p> <code>0</code> <code>decoder_end_token_id</code> <code>int or List[int]</code> <p>The decoder's end token ID. Defaults to 2.</p> <code>1</code> <code>num_return_sequences</code> <code>int</code> <p>The number of generated sequences to return. Defaults to 1.</p> <code>1</code> <code>min_gen_seq_length</code> <code>int</code> <p>The minimum length of the generated sequences. Defaults to 0.</p> <code>0</code> <code>max_gen_seq_length</code> <code>int</code> <p>The maximum length of the generated sequences. Defaults to 48.</p> <code>48</code> <code>repetition_penalty</code> <code>float</code> <p>The repetition penalty. Defaults to 1.0.</p> <code>1.0</code> <code>no_repeat_ngram_size</code> <code>int</code> <p>The size of n-grams to avoid repeating. Defaults to 0.</p> <code>0</code> <code>early_stopping</code> <code>bool</code> <p>Whether to stop generation early. Defaults to True.</p> <code>True</code> <code>length_penalty</code> <code>float</code> <p>The length penalty. Defaults to 1.0.</p> <code>1.0</code> <code>num_beam_groups</code> <code>int</code> <p>The number of beam groups for diverse beam search. Defaults to 1.</p> <code>1</code> <code>diversity_penalty</code> <code>float</code> <p>The diversity penalty. Defaults to 0.0.</p> <code>0.0</code> <code>do_sample</code> <code>bool</code> <p>Whether to use sampling for generation. Defaults to False.</p> <code>False</code> <code>temperature</code> <code>float</code> <p>The temperature for sampling. Defaults to 1.0.</p> <code>1.0</code> <code>top_k</code> <code>int</code> <p>The value for top-k sampling. Defaults to 50.</p> <code>50</code> <code>top_p</code> <code>float</code> <p>The value for top-p (nucleus) sampling. Defaults to 1.0.</p> <code>1.0</code> <p>Returns:</p> Name Type Description <code>GenericOutputs</code> <p>The generated sequences and their scores.</p> Source code in <code>src/unitorch/models/xpegasus/modeling.py</code> <pre><code>@torch.no_grad()\ndef generate(\n    self,\n    input_ids: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 0,\n    decoder_end_token_id: Optional[Union[int, List[int]]] = 1,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n):\n\"\"\"\n    Generates sequences using the XPegasusForGeneration model.\n\n    Args:\n        input_ids: The input token IDs.\n        num_beams (int, optional): The number of beams for beam search. Defaults to 5.\n        decoder_start_token_id (int, optional): The decoder's start token ID. Defaults to 2.\n        decoder_end_token_id (int or List[int], optional): The decoder's end token ID. Defaults to 2.\n        num_return_sequences (int, optional): The number of generated sequences to return. Defaults to 1.\n        min_gen_seq_length (int, optional): The minimum length of the generated sequences. Defaults to 0.\n        max_gen_seq_length (int, optional): The maximum length of the generated sequences. Defaults to 48.\n        repetition_penalty (float, optional): The repetition penalty. Defaults to 1.0.\n        no_repeat_ngram_size (int, optional): The size of n-grams to avoid repeating. Defaults to 0.\n        early_stopping (bool, optional): Whether to stop generation early. Defaults to True.\n        length_penalty (float, optional): The length penalty. Defaults to 1.0.\n        num_beam_groups (int, optional): The number of beam groups for diverse beam search. Defaults to 1.\n        diversity_penalty (float, optional): The diversity penalty. Defaults to 0.0.\n        do_sample (bool, optional): Whether to use sampling for generation. Defaults to False.\n        temperature (float, optional): The temperature for sampling. Defaults to 1.0.\n        top_k (int, optional): The value for top-k sampling. Defaults to 50.\n        top_p (float, optional): The value for top-p (nucleus) sampling. Defaults to 1.0.\n\n    Returns:\n        GenericOutputs: The generated sequences and their scores.\n    \"\"\"\n    outputs = self.model.generate(\n        input_ids,\n        max_length=max_gen_seq_length,\n        min_length=min_gen_seq_length,\n        num_beams=num_beams,\n        do_sample=do_sample,\n        decoder_start_token_id=decoder_start_token_id,\n        no_repeat_ngram_size=no_repeat_ngram_size,\n        early_stopping=early_stopping,\n        length_penalty=length_penalty,\n        repetition_penalty=repetition_penalty,\n        num_return_sequences=num_return_sequences,\n        bos_token_id=decoder_start_token_id,\n        eos_token_id=decoder_end_token_id,\n        num_beam_groups=num_beam_groups,\n        diversity_penalty=diversity_penalty,\n        temperature=temperature,\n        top_k=top_k,\n        top_p=top_p,\n        return_dict_in_generate=True,\n        output_scores=True,\n    )\n\n    sequences = outputs.sequences.reshape(\n        -1, num_return_sequences, outputs.sequences.size(-1)\n    )\n    outputs.sequences = torch.zeros(\n        sequences.size(0), num_return_sequences, max_gen_seq_length\n    ).to(device=sequences.device)\n    outputs.sequences[:, :, : sequences.size(-1)].copy_(sequences)\n\n    if num_return_sequences == 1:\n        outputs.sequences = outputs.sequences.reshape(-1, max_gen_seq_length)\n\n    return GenericOutputs(\n        sequences=outputs.sequences,\n        sequences_scores=outputs.sequences_scores,\n    )\n</code></pre>",
             "title": "generate"
         },
         {
             "location": "models/xprophetnet/",
             "text": "",
             "title": "unitorch.models.xprophetnet"
         },
@@ -2632,15 +2727,15 @@
         {
             "location": "models/xprophetnet/#unitorch.models.xprophetnet.modeling.XProphetNetForGeneration.forward",
             "text": "<pre><code>forward(\n    input_ids: torch.Tensor,\n    attention_mask: torch.Tensor,\n    decoder_input_ids: torch.Tensor,\n    decoder_attention_mask: torch.Tensor,\n)\n</code></pre> <p>Performs forward pass of the XPegasusForGeneration model.</p> <p>Parameters:</p> Name Type Description Default <code>input_ids</code> <code>torch.Tensor</code> <p>Tensor of input token IDs.</p> required <code>attention_mask</code> <code>torch.Tensor</code> <p>Tensor of attention mask.</p> required <code>decoder_input_ids</code> <code>torch.Tensor</code> <p>Tensor of decoder input token IDs.</p> required <code>decoder_attention_mask</code> <code>torch.Tensor</code> <p>Tensor of decoder attention mask.</p> required <p>Returns:</p> Type Description <code>torch.Tensor</code> <p>The model's logits.</p> Source code in <code>src/unitorch/models/xprophetnet/modeling.py</code> <pre><code>def forward(\n    self,\n    input_ids: torch.Tensor,\n    attention_mask: torch.Tensor,\n    decoder_input_ids: torch.Tensor,\n    decoder_attention_mask: torch.Tensor,\n):\n\"\"\"\n    Performs forward pass of the XPegasusForGeneration model.\n\n    Args:\n        input_ids (torch.Tensor): Tensor of input token IDs.\n        attention_mask (torch.Tensor): Tensor of attention mask.\n        decoder_input_ids (torch.Tensor): Tensor of decoder input token IDs.\n        decoder_attention_mask (torch.Tensor): Tensor of decoder attention mask.\n\n    Returns:\n        (torch.Tensor):The model's logits.\n    \"\"\"\n    outputs = self.model(\n        input_ids=input_ids,\n        attention_mask=attention_mask,\n        decoder_input_ids=decoder_input_ids,\n        decoder_attention_mask=decoder_attention_mask,\n        return_dict=True,\n    )\n    logits = outputs.logits.unsqueeze(1)\n    if outputs.logits_ngram is not None:\n        logits_ngram = outputs.logits_ngram\n        logits = torch.cat([logits, logits_ngram], dim=1)\n    return logits\n</code></pre>",
             "title": "forward"
         },
         {
             "location": "models/xprophetnet/#unitorch.models.xprophetnet.modeling.XProphetNetForGeneration.generate",
-            "text": "<pre><code>generate(\n    input_ids: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 2,\n    decoder_end_token_id: Optional[int] = 2,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n)\n</code></pre> <p>Generates sequences using the XPegasusForGeneration model.</p> <p>Parameters:</p> Name Type Description Default <code>input_ids</code> <code>torch.Tensor</code> <p>The input token IDs.</p> required <code>num_beams</code> <code>int</code> <p>The number of beams for beam search. Defaults to 5.</p> <code>5</code> <code>decoder_start_token_id</code> <code>int</code> <p>The decoder's start token ID. Defaults to 2.</p> <code>2</code> <code>decoder_end_token_id</code> <code>int</code> <p>The decoder's end token ID. Defaults to 2.</p> <code>2</code> <code>num_return_sequences</code> <code>int</code> <p>The number of generated sequences to return. Defaults to 1.</p> <code>1</code> <code>min_gen_seq_length</code> <code>int</code> <p>The minimum length of the generated sequences. Defaults to 0.</p> <code>0</code> <code>max_gen_seq_length</code> <code>int</code> <p>The maximum length of the generated sequences. Defaults to 48.</p> <code>48</code> <code>repetition_penalty</code> <code>float</code> <p>The repetition penalty. Defaults to 1.0.</p> <code>1.0</code> <code>no_repeat_ngram_size</code> <code>int</code> <p>The size of n-grams to avoid repeating. Defaults to 0.</p> <code>0</code> <code>early_stopping</code> <code>bool</code> <p>Whether to stop generation early. Defaults to True.</p> <code>True</code> <code>length_penalty</code> <code>float</code> <p>The length penalty. Defaults to 1.0.</p> <code>1.0</code> <code>num_beam_groups</code> <code>int</code> <p>The number of beam groups for diverse beam search. Defaults to 1.</p> <code>1</code> <code>diversity_penalty</code> <code>float</code> <p>The diversity penalty. Defaults to 0.0.</p> <code>0.0</code> <code>do_sample</code> <code>bool</code> <p>Whether to use sampling for generation. Defaults to False.</p> <code>False</code> <code>temperature</code> <code>float</code> <p>The temperature for sampling. Defaults to 1.0.</p> <code>1.0</code> <code>top_k</code> <code>int</code> <p>The value for top-k sampling. Defaults to 50.</p> <code>50</code> <code>top_p</code> <code>float</code> <p>The value for top-p (nucleus) sampling. Defaults to 1.0.</p> <code>1.0</code> <p>Returns:</p> Name Type Description <code>GenericOutputs</code> <p>The generated sequences and their scores.</p> Source code in <code>src/unitorch/models/xprophetnet/modeling.py</code> <pre><code>@torch.no_grad()\ndef generate(\n    self,\n    input_ids: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 2,\n    decoder_end_token_id: Optional[int] = 2,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n):\n\"\"\"\n    Generates sequences using the XPegasusForGeneration model.\n\n    Args:\n        input_ids: The input token IDs.\n        num_beams (int, optional): The number of beams for beam search. Defaults to 5.\n        decoder_start_token_id (int, optional): The decoder's start token ID. Defaults to 2.\n        decoder_end_token_id (int, optional): The decoder's end token ID. Defaults to 2.\n        num_return_sequences (int, optional): The number of generated sequences to return. Defaults to 1.\n        min_gen_seq_length (int, optional): The minimum length of the generated sequences. Defaults to 0.\n        max_gen_seq_length (int, optional): The maximum length of the generated sequences. Defaults to 48.\n        repetition_penalty (float, optional): The repetition penalty. Defaults to 1.0.\n        no_repeat_ngram_size (int, optional): The size of n-grams to avoid repeating. Defaults to 0.\n        early_stopping (bool, optional): Whether to stop generation early. Defaults to True.\n        length_penalty (float, optional): The length penalty. Defaults to 1.0.\n        num_beam_groups (int, optional): The number of beam groups for diverse beam search. Defaults to 1.\n        diversity_penalty (float, optional): The diversity penalty. Defaults to 0.0.\n        do_sample (bool, optional): Whether to use sampling for generation. Defaults to False.\n        temperature (float, optional): The temperature for sampling. Defaults to 1.0.\n        top_k (int, optional): The value for top-k sampling. Defaults to 50.\n        top_p (float, optional): The value for top-p (nucleus) sampling. Defaults to 1.0.\n\n    Returns:\n        GenericOutputs: The generated sequences and their scores.\n    \"\"\"\n    outputs = self.model.generate(\n        input_ids,\n        max_length=max_gen_seq_length,\n        min_length=min_gen_seq_length,\n        num_beams=num_beams,\n        do_sample=do_sample,\n        decoder_start_token_id=decoder_start_token_id,\n        no_repeat_ngram_size=no_repeat_ngram_size,\n        early_stopping=early_stopping,\n        length_penalty=length_penalty,\n        repetition_penalty=repetition_penalty,\n        num_return_sequences=num_return_sequences,\n        bos_token_id=decoder_start_token_id,\n        eos_token_id=decoder_end_token_id,\n        num_beam_groups=num_beam_groups,\n        diversity_penalty=diversity_penalty,\n        temperature=temperature,\n        top_k=top_k,\n        top_p=top_p,\n        return_dict_in_generate=True,\n        output_scores=True,\n    )\n\n    sequences = outputs.sequences.reshape(\n        -1, num_return_sequences, outputs.sequences.size(-1)\n    )\n    outputs.sequences = torch.zeros(\n        sequences.size(0), num_return_sequences, max_gen_seq_length\n    ).to(device=sequences.device)\n    outputs.sequences[:, :, : sequences.size(-1)].copy_(sequences)\n\n    if num_return_sequences == 1:\n        outputs.sequences = outputs.sequences.reshape(-1, max_gen_seq_length)\n\n    return GenericOutputs(\n        sequences=outputs.sequences,\n        sequences_scores=outputs.sequences_scores,\n    )\n</code></pre>",
+            "text": "<pre><code>generate(\n    input_ids: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 2,\n    decoder_end_token_id: Optional[\n        Union[int, List[int]]\n    ] = 2,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n)\n</code></pre> <p>Generates sequences using the XPegasusForGeneration model.</p> <p>Parameters:</p> Name Type Description Default <code>input_ids</code> <code>torch.Tensor</code> <p>The input token IDs.</p> required <code>num_beams</code> <code>int</code> <p>The number of beams for beam search. Defaults to 5.</p> <code>5</code> <code>decoder_start_token_id</code> <code>int</code> <p>The decoder's start token ID. Defaults to 2.</p> <code>2</code> <code>decoder_end_token_id</code> <code>int or List[int]</code> <p>The decoder's end token ID. Defaults to 2.</p> <code>2</code> <code>num_return_sequences</code> <code>int</code> <p>The number of generated sequences to return. Defaults to 1.</p> <code>1</code> <code>min_gen_seq_length</code> <code>int</code> <p>The minimum length of the generated sequences. Defaults to 0.</p> <code>0</code> <code>max_gen_seq_length</code> <code>int</code> <p>The maximum length of the generated sequences. Defaults to 48.</p> <code>48</code> <code>repetition_penalty</code> <code>float</code> <p>The repetition penalty. Defaults to 1.0.</p> <code>1.0</code> <code>no_repeat_ngram_size</code> <code>int</code> <p>The size of n-grams to avoid repeating. Defaults to 0.</p> <code>0</code> <code>early_stopping</code> <code>bool</code> <p>Whether to stop generation early. Defaults to True.</p> <code>True</code> <code>length_penalty</code> <code>float</code> <p>The length penalty. Defaults to 1.0.</p> <code>1.0</code> <code>num_beam_groups</code> <code>int</code> <p>The number of beam groups for diverse beam search. Defaults to 1.</p> <code>1</code> <code>diversity_penalty</code> <code>float</code> <p>The diversity penalty. Defaults to 0.0.</p> <code>0.0</code> <code>do_sample</code> <code>bool</code> <p>Whether to use sampling for generation. Defaults to False.</p> <code>False</code> <code>temperature</code> <code>float</code> <p>The temperature for sampling. Defaults to 1.0.</p> <code>1.0</code> <code>top_k</code> <code>int</code> <p>The value for top-k sampling. Defaults to 50.</p> <code>50</code> <code>top_p</code> <code>float</code> <p>The value for top-p (nucleus) sampling. Defaults to 1.0.</p> <code>1.0</code> <p>Returns:</p> Name Type Description <code>GenericOutputs</code> <p>The generated sequences and their scores.</p> Source code in <code>src/unitorch/models/xprophetnet/modeling.py</code> <pre><code>@torch.no_grad()\ndef generate(\n    self,\n    input_ids: torch.Tensor,\n    num_beams: Optional[int] = 5,\n    decoder_start_token_id: Optional[int] = 2,\n    decoder_end_token_id: Optional[Union[int, List[int]]] = 2,\n    num_return_sequences: Optional[int] = 1,\n    min_gen_seq_length: Optional[int] = 0,\n    max_gen_seq_length: Optional[int] = 48,\n    repetition_penalty: Optional[float] = 1.0,\n    no_repeat_ngram_size: Optional[int] = 0,\n    early_stopping: Optional[bool] = True,\n    length_penalty: Optional[float] = 1.0,\n    num_beam_groups: Optional[int] = 1,\n    diversity_penalty: Optional[float] = 0.0,\n    do_sample: Optional[bool] = False,\n    temperature: Optional[float] = 1.0,\n    top_k: Optional[int] = 50,\n    top_p: Optional[float] = 1.0,\n):\n\"\"\"\n    Generates sequences using the XPegasusForGeneration model.\n\n    Args:\n        input_ids: The input token IDs.\n        num_beams (int, optional): The number of beams for beam search. Defaults to 5.\n        decoder_start_token_id (int, optional): The decoder's start token ID. Defaults to 2.\n        decoder_end_token_id (int or List[int], optional): The decoder's end token ID. Defaults to 2.\n        num_return_sequences (int, optional): The number of generated sequences to return. Defaults to 1.\n        min_gen_seq_length (int, optional): The minimum length of the generated sequences. Defaults to 0.\n        max_gen_seq_length (int, optional): The maximum length of the generated sequences. Defaults to 48.\n        repetition_penalty (float, optional): The repetition penalty. Defaults to 1.0.\n        no_repeat_ngram_size (int, optional): The size of n-grams to avoid repeating. Defaults to 0.\n        early_stopping (bool, optional): Whether to stop generation early. Defaults to True.\n        length_penalty (float, optional): The length penalty. Defaults to 1.0.\n        num_beam_groups (int, optional): The number of beam groups for diverse beam search. Defaults to 1.\n        diversity_penalty (float, optional): The diversity penalty. Defaults to 0.0.\n        do_sample (bool, optional): Whether to use sampling for generation. Defaults to False.\n        temperature (float, optional): The temperature for sampling. Defaults to 1.0.\n        top_k (int, optional): The value for top-k sampling. Defaults to 50.\n        top_p (float, optional): The value for top-p (nucleus) sampling. Defaults to 1.0.\n\n    Returns:\n        GenericOutputs: The generated sequences and their scores.\n    \"\"\"\n    outputs = self.model.generate(\n        input_ids,\n        max_length=max_gen_seq_length,\n        min_length=min_gen_seq_length,\n        num_beams=num_beams,\n        do_sample=do_sample,\n        decoder_start_token_id=decoder_start_token_id,\n        no_repeat_ngram_size=no_repeat_ngram_size,\n        early_stopping=early_stopping,\n        length_penalty=length_penalty,\n        repetition_penalty=repetition_penalty,\n        num_return_sequences=num_return_sequences,\n        bos_token_id=decoder_start_token_id,\n        eos_token_id=decoder_end_token_id,\n        num_beam_groups=num_beam_groups,\n        diversity_penalty=diversity_penalty,\n        temperature=temperature,\n        top_k=top_k,\n        top_p=top_p,\n        return_dict_in_generate=True,\n        output_scores=True,\n    )\n\n    sequences = outputs.sequences.reshape(\n        -1, num_return_sequences, outputs.sequences.size(-1)\n    )\n    outputs.sequences = torch.zeros(\n        sequences.size(0), num_return_sequences, max_gen_seq_length\n    ).to(device=sequences.device)\n    outputs.sequences[:, :, : sequences.size(-1)].copy_(sequences)\n\n    if num_return_sequences == 1:\n        outputs.sequences = outputs.sequences.reshape(-1, max_gen_seq_length)\n\n    return GenericOutputs(\n        sequences=outputs.sequences,\n        sequences_scores=outputs.sequences_scores,\n    )\n</code></pre>",
             "title": "generate"
         },
         {
             "location": "coverage/",
             "text": "",
             "title": "Coverage"
         }
```

### Comparing `unitorch-0.0.0.4/examples/README.md` & `unitorch-0.0.0.5/examples/README.md`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/examples/configs/caption/blip.ini` & `unitorch-0.0.0.5/examples/configs/caption/blip.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/examples/configs/classification/bert.ini` & `unitorch-0.0.0.5/examples/configs/classification/bert.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/examples/configs/classification/clip.ini` & `unitorch-0.0.0.5/examples/configs/classification/clip.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/examples/configs/classification/image_clip.ini` & `unitorch-0.0.0.5/examples/configs/classification/image_clip.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/examples/configs/classification/lora/bloom.ini` & `unitorch-0.0.0.5/examples/configs/classification/lora/bloom.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/examples/configs/classification/lora/bloom_ds.ini` & `unitorch-0.0.0.5/examples/configs/classification/lora/bloom_ds.ini`

 * *Files 14% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 max_gen_seq_length = 36
 
 [core/writer/csv]
 escapechar = \
 
 # task
 [core/task/deepspeed/supervised]
-config_path = https://huggingface.co/fuliucansheng/peft/resolve/main/deepspeed.adamw.json
+config_path = https://raw.githubusercontent.com/fuliucansheng/unitorch/master/examples/configs/deepspeed/adamw.json
 model = core/model/classification/peft/lora/bloom
 dataset = core/dataset/ast
 loss_fn = core/loss/ce
 score_fn = core/score/acc
 monitor_fns = ['core/score/acc']
 
 ckpt_freq = 2000
@@ -54,8 +54,8 @@
 writer = core/writer/csv
 
 from_ckpt_dir = ${core/cli:from_ckpt_dir}
 to_ckpt_dir = ${core/cli:cache_dir}
 output_path = ${core/cli:cache_dir}/output.txt
 train_batch_size = 4
 dev_batch_size = 4
-test_batch_size = 4
+test_batch_size = 4
```

### Comparing `unitorch-0.0.0.4/examples/configs/classification/lora/llama.ini` & `unitorch-0.0.0.5/examples/configs/classification/lora/llama.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/examples/configs/classification/lora/llama_ds.ini` & `unitorch-0.0.0.5/examples/configs/classification/lora/llama_ds.ini`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 dev_file = ./dev.tsv
 test_file = ./test.tsv
 pretrained_weight_folder = ./llama-7b
 
 # model
 [core/model/classification/peft/lora/llama]
 pretrained_name = llama-7b
-pretrained_weight_path = [                       
+pretrained_weight_path = [
     '${core/cli:pretrained_weight_folder}/pytorch_model-00001-of-00002.bin',
     '${core/cli:pretrained_weight_folder}/pytorch_model-00002-of-00002.bin',
   ]
 num_classes = 2
 
 # dataset
 [core/dataset/ast]
@@ -39,15 +39,15 @@
 max_gen_seq_length = 36
 
 [core/writer/csv]
 escapechar = \
 
 # task
 [core/task/deepspeed/supervised]
-config_path = https://huggingface.co/fuliucansheng/peft/resolve/main/deepspeed.adamw.json
+config_path = https://raw.githubusercontent.com/fuliucansheng/unitorch/master/examples/configs/deepspeed/adamw.json
 model = core/model/classification/peft/lora/llama
 dataset = core/dataset/ast
 loss_fn = core/loss/ce
 score_fn = core/score/acc
 monitor_fns = ['core/score/acc']
 
 ckpt_freq = 2000
@@ -58,8 +58,8 @@
 writer = core/writer/csv
 
 from_ckpt_dir = ${core/cli:from_ckpt_dir}
 to_ckpt_dir = ${core/cli:cache_dir}
 output_path = ${core/cli:cache_dir}/output.txt
 train_batch_size = 4
 dev_batch_size = 4
-test_batch_size = 4
+test_batch_size = 4
```

### Comparing `unitorch-0.0.0.4/examples/configs/classification/roberta.ini` & `unitorch-0.0.0.5/examples/configs/classification/roberta.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/examples/configs/classification/swin.ini` & `unitorch-0.0.0.5/examples/configs/classification/swin.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/examples/configs/classification/text_clip.ini` & `unitorch-0.0.0.5/examples/configs/classification/text_clip.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/examples/configs/diffusion/controlnet/canny.ini` & `unitorch-0.0.0.5/examples/configs/diffusion/controlnet/canny.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/examples/configs/diffusion/stable-v1.5.ini` & `unitorch-0.0.0.5/examples/configs/diffusion/stable-v1.5.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/examples/configs/diffusion/stable-v2.1.ini` & `unitorch-0.0.0.5/examples/configs/diffusion/stable-v2.1.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/examples/configs/diffusion/stable-v2.ini` & `unitorch-0.0.0.5/examples/configs/diffusion/stable-v2.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/examples/configs/generation/bart.ini` & `unitorch-0.0.0.5/examples/configs/generation/bart.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/examples/configs/generation/bloom.ini` & `unitorch-0.0.0.5/examples/configs/generation/bloom.ini`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 dev_file = ./dev.tsv
 test_file = ./test.tsv
 
 # model
 [core/model/generation/bloom]
 pretrained_name = bloom-560m
 no_repeat_ngram_size = 3
-max_gen_seq_length = 15
+max_gen_seq_length = 36
 
 # dataset
 [core/dataset/ast]
 names = ['encode', 'decode']
 
 [core/dataset/ast/train]
 data_files = ${core/cli:train_file}
@@ -28,16 +28,16 @@
 names = ['encode']
 data_files = ${core/cli:test_file}
 preprocess_functions = ['core/process/bloom/generation/inputs(encode)']
 
 # process
 [core/process/bloom]
 pretrained_name = bloom-560m
-max_seq_length = 5
-max_gen_seq_length = 15
+max_seq_length = 64
+max_gen_seq_length = 36
 
 [core/writer/csv]
 escapechar = \
 
 # optim
 [core/optim/adamw]
 learning_rate = 0.0001
```

### Comparing `unitorch-0.0.0.4/examples/configs/generation/chatglm.ini` & `unitorch-0.0.0.5/examples/configs/generation/chatglm.ini`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 dev_file = ./dev.tsv
 test_file = ./test.tsv
 
 # model
 [core/model/generation/chatglm]
 pretrained_name = chatglm-6b
 no_repeat_ngram_size = 3
-max_gen_seq_length = 15
+max_gen_seq_length = 36
 
 # dataset
 [core/dataset/ast]
 names = ['encode', 'decode']
 
 [core/dataset/ast/train]
 data_files = ${core/cli:train_file}
@@ -28,16 +28,16 @@
 names = ['encode']
 data_files = ${core/cli:test_file}
 preprocess_functions = ['core/process/chatglm/generation/inputs(encode)']
 
 # process
 [core/process/chatglm]
 pretrained_name = chatglm-6b
-max_seq_length = 5
-max_gen_seq_length = 15
+max_seq_length = 64
+max_gen_seq_length = 36
 
 [core/writer/csv]
 escapechar = \
 
 # optim
 [core/optim/adamw]
 learning_rate = 0.0001
```

### Comparing `unitorch-0.0.0.4/examples/configs/generation/llama.ini` & `unitorch-0.0.0.5/examples/configs/generation/llama.ini`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 dev_file = ./dev.tsv
 test_file = ./test.tsv
 
 # model
 [core/model/generation/llama]
 pretrained_name = llama-7b
 no_repeat_ngram_size = 3
-max_gen_seq_length = 15
+max_gen_seq_length = 36
 
 # dataset
 [core/dataset/ast]
 names = ['encode', 'decode']
 
 [core/dataset/ast/train]
 data_files = ${core/cli:train_file}
@@ -28,16 +28,16 @@
 names = ['encode']
 data_files = ${core/cli:test_file}
 preprocess_functions = ['core/process/llama/generation/inputs(encode)']
 
 # process
 [core/process/llama]
 pretrained_name = llama-7b
-max_seq_length = 5
-max_gen_seq_length = 15
+max_seq_length = 64
+max_gen_seq_length = 36
 
 [core/writer/csv]
 escapechar = \
 
 # optim
 [core/optim/adamw]
 learning_rate = 0.0001
```

### Comparing `unitorch-0.0.0.4/examples/configs/generation/lora/bloom.ini` & `unitorch-0.0.0.5/examples/configs/generation/mt5.ini`

 * *Files 14% similar despite different names*

```diff
@@ -3,67 +3,62 @@
 from_ckpt_dir = ./cache
 cache_dir = ./cache
 train_file = ./train.tsv
 dev_file = ./dev.tsv
 test_file = ./test.tsv
 
 # model
-[core/model/generation/peft/lora/bloom]
-pretrained_name = bloom-560m
-max_gen_seq_length = 36
-num_beams = 2
+[core/model/generation/mt5]
+pretrained_name = mt5-base
+no_repeat_ngram_size = 3
+max_gen_seq_length = 15
 
 # dataset
 [core/dataset/ast]
-names = ['query', 'doc']
+names = ['encode', 'decode']
 
 [core/dataset/ast/train]
 data_files = ${core/cli:train_file}
-preprocess_functions = ['core/process/bloom/generation(query, doc)']
+preprocess_functions = ['core/process/mt5/generation(encode, decode)']
 
 [core/dataset/ast/dev]
 data_files = ${core/cli:dev_file}
-preprocess_functions = ['core/process/bloom/generation/inputs(query)', 'core/process/bloom/generation/labels(doc)']
+preprocess_functions = ['core/process/mt5/generation/inputs(encode)', 'core/process/mt5/generation/labels(decode)']
 
 [core/dataset/ast/test]
+names = ['encode']
 data_files = ${core/cli:test_file}
-preprocess_functions = ['core/process/bloom/generation/inputs(query)']
+preprocess_functions = ['core/process/mt5/generation/inputs(encode)']
 
 # process
-[core/process/bloom]
-pretrained_name = bloom-560m
-max_seq_length = 6
-max_gen_seq_length = 36
+[core/process/mt5]
+pretrained_name = mt5-base
+max_seq_length = 24
+max_gen_seq_length = 15
 
 # optim
 [core/optim/adamw]
-learning_rate = 0.00001
+learning_rate = 0.0001
 
 # scheduler
 [core/scheduler/linear_warmup]
 num_warmup_rate = 0.001
 
-[core/writer/csv]
-escapechar = \
-
 # task
 [core/task/supervised]
-model = core/model/generation/peft/lora/bloom
+model = core/model/generation/mt5
 optim = core/optim/adamw
 scheduler = core/scheduler/linear_warmup
 dataset = core/dataset/ast
 loss_fn = core/loss/lm
 score_fn = core/score/bleu
-monitor_fns = ['core/score/bleu']
-
-ckpt_freq = 2000
-
-output_header = ['query', 'doc']
-postprocess_fn = core/postprocess/bloom/detokenize
+monitor_fns = ['core/score/bleu', 'core/score/rouge1', 'core/score/rouge2', 'core/score/rougel']
+output_header = ['encode']
+postprocess_fn = core/postprocess/mt5/detokenize
 writer = core/writer/csv
 
 from_ckpt_dir = ${core/cli:from_ckpt_dir}
 to_ckpt_dir = ${core/cli:cache_dir}
 output_path = ${core/cli:cache_dir}/output.txt
 train_batch_size = 4
-dev_batch_size = 4
-test_batch_size = 4
+dev_batch_size = 8
+test_batch_size = 8
```

### Comparing `unitorch-0.0.0.4/examples/configs/generation/lora/bloom_ds.ini` & `unitorch-0.0.0.5/examples/configs/generation/lora/bloom.ini`

 * *Files 18% similar despite different names*

```diff
@@ -1,61 +1,69 @@
 [core/cli]
-task_name = core/task/deepspeed/supervised
+task_name = core/task/supervised
 from_ckpt_dir = ./cache
 cache_dir = ./cache
 train_file = ./train.tsv
 dev_file = ./dev.tsv
 test_file = ./test.tsv
 
 # model
 [core/model/generation/peft/lora/bloom]
 pretrained_name = bloom-560m
 max_gen_seq_length = 36
 num_beams = 2
 
 # dataset
 [core/dataset/ast]
-names = ['query', 'doc']
+names = ['encode', 'decode']
 
 [core/dataset/ast/train]
 data_files = ${core/cli:train_file}
-preprocess_functions = ['core/process/bloom/generation(query, doc)']
+preprocess_functions = ['core/process/bloom/generation(encode, decode)']
 
 [core/dataset/ast/dev]
 data_files = ${core/cli:dev_file}
-preprocess_functions = ['core/process/bloom/generation/inputs(query)', 'core/process/bloom/generation/labels(doc)']
+preprocess_functions = ['core/process/bloom/generation/inputs(encode)', 'core/process/bloom/generation/labels(decode)']
 
 [core/dataset/ast/test]
 data_files = ${core/cli:test_file}
-preprocess_functions = ['core/process/bloom/generation/inputs(query)']
+preprocess_functions = ['core/process/bloom/generation/inputs(encode)']
 
 # process
 [core/process/bloom]
 pretrained_name = bloom-560m
-max_seq_length = 6
+max_seq_length = 64
 max_gen_seq_length = 36
 
+# optim
+[core/optim/adamw]
+learning_rate = 0.00001
+
+# scheduler
+[core/scheduler/linear_warmup]
+num_warmup_rate = 0.001
+
 [core/writer/csv]
 escapechar = \
 
 # task
-[core/task/deepspeed/supervised]
-config_path = https://huggingface.co/fuliucansheng/peft/resolve/main/deepspeed.adamw.json
+[core/task/supervised]
 model = core/model/generation/peft/lora/bloom
+optim = core/optim/adamw
+scheduler = core/scheduler/linear_warmup
 dataset = core/dataset/ast
 loss_fn = core/loss/lm
 score_fn = core/score/bleu
 monitor_fns = ['core/score/bleu']
 
 ckpt_freq = 2000
-learning_rate = 0.00001
 
-output_header = ['query', 'doc']
+output_header = ['encode', 'decode']
 postprocess_fn = core/postprocess/bloom/detokenize
 writer = core/writer/csv
 
 from_ckpt_dir = ${core/cli:from_ckpt_dir}
 to_ckpt_dir = ${core/cli:cache_dir}
 output_path = ${core/cli:cache_dir}/output.txt
 train_batch_size = 4
 dev_batch_size = 4
-test_batch_size = 4
+test_batch_size = 4
```

### Comparing `unitorch-0.0.0.4/examples/configs/generation/lora/llama.ini` & `unitorch-0.0.0.5/examples/configs/generation/lora/llama_ds.ini`

 * *Files 13% similar despite different names*

```diff
@@ -1,69 +1,61 @@
 [core/cli]
-task_name = core/task/supervised
+task_name = core/task/deepspeed/supervised
 from_ckpt_dir = ./cache
 cache_dir = ./cache
 train_file = ./train.tsv
 dev_file = ./dev.tsv
 test_file = ./test.tsv
 
 # model
 [core/model/generation/peft/lora/llama]
 pretrained_name = llama-7b
 max_gen_seq_length = 36
 num_beams = 2
 
 # dataset
 [core/dataset/ast]
-names = ['query', 'doc']
+names = ['encode', 'decode']
 
 [core/dataset/ast/train]
 data_files = ${core/cli:train_file}
-preprocess_functions = ['core/process/llama/generation(query, doc)']
+preprocess_functions = ['core/process/llama/generation(encode, decode)']
 
 [core/dataset/ast/dev]
 data_files = ${core/cli:dev_file}
-preprocess_functions = ['core/process/llama/generation/inputs(query)', 'core/process/llama/generation/labels(doc)']
+preprocess_functions = ['core/process/llama/generation/inputs(encode)', 'core/process/llama/generation/labels(decode)']
 
 [core/dataset/ast/test]
 data_files = ${core/cli:test_file}
-preprocess_functions = ['core/process/llama/generation/inputs(query)']
+preprocess_functions = ['core/process/llama/generation/inputs(encode)']
 
 # process
 [core/process/llama]
 pretrained_name = llama-7b
-max_seq_length = 6
+max_seq_length = 64
 max_gen_seq_length = 36
 
-# optim
-[core/optim/adamw]
-learning_rate = 0.00001
-
-# scheduler
-[core/scheduler/linear_warmup]
-num_warmup_rate = 0.001
-
 [core/writer/csv]
 escapechar = \
 
 # task
-[core/task/supervised]
+[core/task/deepspeed/supervised]
+config_path = https://raw.githubusercontent.com/fuliucansheng/unitorch/master/examples/configs/deepspeed/adamw.json
 model = core/model/generation/peft/lora/llama
-optim = core/optim/adamw
-scheduler = core/scheduler/linear_warmup
 dataset = core/dataset/ast
 loss_fn = core/loss/lm
 score_fn = core/score/bleu
 monitor_fns = ['core/score/bleu']
 
 ckpt_freq = 2000
+learning_rate = 0.00001
 
-output_header = ['query', 'doc']
+output_header = ['encode', 'decode']
 postprocess_fn = core/postprocess/llama/detokenize
 writer = core/writer/csv
 
 from_ckpt_dir = ${core/cli:from_ckpt_dir}
 to_ckpt_dir = ${core/cli:cache_dir}
 output_path = ${core/cli:cache_dir}/output.txt
 train_batch_size = 4
 dev_batch_size = 4
-test_batch_size = 4
+test_batch_size = 4
```

### Comparing `unitorch-0.0.0.4/examples/configs/generation/lora/llama_ds.ini` & `unitorch-0.0.0.5/examples/configs/generation/mbart.ini`

 * *Files 20% similar despite different names*

```diff
@@ -1,61 +1,65 @@
 [core/cli]
-task_name = core/task/deepspeed/supervised
+task_name = core/task/supervised
 from_ckpt_dir = ./cache
 cache_dir = ./cache
 train_file = ./train.tsv
 dev_file = ./dev.tsv
 test_file = ./test.tsv
 
 # model
-[core/model/generation/peft/lora/llama]
-pretrained_name = llama-7b
-max_gen_seq_length = 36
-num_beams = 2
+[core/model/generation/mbart]
+pretrained_name = mbart-large-cc25
+freeze_input_embedding = True
+no_repeat_ngram_size = 3
+max_gen_seq_length = 15
 
 # dataset
 [core/dataset/ast]
-names = ['query', 'doc']
+names = ['encode', 'decode']
 
 [core/dataset/ast/train]
 data_files = ${core/cli:train_file}
-preprocess_functions = ['core/process/llama/generation(query, doc)']
+preprocess_functions = ['core/process/mbart/generation(encode, decode)']
 
 [core/dataset/ast/dev]
 data_files = ${core/cli:dev_file}
-preprocess_functions = ['core/process/llama/generation/inputs(query)', 'core/process/llama/generation/labels(doc)']
+preprocess_functions = ['core/process/mbart/generation/inputs(encode)', 'core/process/mbart/generation/labels(decode)']
 
 [core/dataset/ast/test]
+names = ['encode']
 data_files = ${core/cli:test_file}
-preprocess_functions = ['core/process/llama/generation/inputs(query)']
+preprocess_functions = ['core/process/mbart/generation/inputs(encode)']
 
 # process
-[core/process/llama]
-pretrained_name = llama-7b
-max_seq_length = 6
-max_gen_seq_length = 36
-
-[core/writer/csv]
-escapechar = \
+[core/process/mbart]
+pretrained_name = mbart-large-cc25
+max_seq_length = 24
+max_gen_seq_length = 15
+
+# optim
+[core/optim/adamw]
+learning_rate = 0.0001
+
+# scheduler
+[core/scheduler/linear_warmup]
+num_warmup_rate = 0.001
 
 # task
-[core/task/deepspeed/supervised]
-config_path = https://huggingface.co/fuliucansheng/peft/resolve/main/deepspeed.adamw.json
-model = core/model/generation/peft/lora/llama
+[core/task/supervised]
+model = core/model/generation/mbart
+optim = core/optim/adamw
+scheduler = core/scheduler/linear_warmup
 dataset = core/dataset/ast
 loss_fn = core/loss/lm
 score_fn = core/score/bleu
-monitor_fns = ['core/score/bleu']
-
-ckpt_freq = 2000
-learning_rate = 0.00001
-
-output_header = ['query', 'doc']
-postprocess_fn = core/postprocess/llama/detokenize
+monitor_fns = ['core/score/bleu', 'core/score/rouge1', 'core/score/rouge2', 'core/score/rougel']
+output_header = ['encode']
+postprocess_fn = core/postprocess/mbart/detokenize
 writer = core/writer/csv
 
 from_ckpt_dir = ${core/cli:from_ckpt_dir}
 to_ckpt_dir = ${core/cli:cache_dir}
 output_path = ${core/cli:cache_dir}/output.txt
 train_batch_size = 4
-dev_batch_size = 4
-test_batch_size = 4
+dev_batch_size = 8
+test_batch_size = 8
```

### Comparing `unitorch-0.0.0.4/examples/configs/generation/mbart.ini` & `unitorch-0.0.0.5/examples/configs/generation/t5.ini`

 * *Files 10% similar despite different names*

```diff
@@ -3,62 +3,61 @@
 from_ckpt_dir = ./cache
 cache_dir = ./cache
 train_file = ./train.tsv
 dev_file = ./dev.tsv
 test_file = ./test.tsv
 
 # model
-[core/model/generation/mbart]
-pretrained_name = mbart-large-cc25
-freeze_input_embedding = True
+[core/model/generation/t5]
+pretrained_name = t5-base
 no_repeat_ngram_size = 3
 max_gen_seq_length = 15
 
 # dataset
 [core/dataset/ast]
 names = ['encode', 'decode']
 
 [core/dataset/ast/train]
 data_files = ${core/cli:train_file}
-preprocess_functions = ['core/process/mbart/generation(encode, decode)']
+preprocess_functions = ['core/process/t5/generation(encode, decode)']
 
 [core/dataset/ast/dev]
 data_files = ${core/cli:dev_file}
-preprocess_functions = ['core/process/mbart/generation/inputs(encode)', 'core/process/mbart/generation/labels(decode)']
+preprocess_functions = ['core/process/t5/generation/inputs(encode)', 'core/process/t5/generation/labels(decode)']
 
 [core/dataset/ast/test]
 names = ['encode']
 data_files = ${core/cli:test_file}
-preprocess_functions = ['core/process/mbart/generation/inputs(encode)']
+preprocess_functions = ['core/process/t5/generation/inputs(encode)']
 
 # process
-[core/process/mbart]
-pretrained_name = mbart-large-cc25
+[core/process/t5]
+pretrained_name = t5-base
 max_seq_length = 24
 max_gen_seq_length = 15
 
 # optim
 [core/optim/adamw]
 learning_rate = 0.0001
 
 # scheduler
 [core/scheduler/linear_warmup]
 num_warmup_rate = 0.001
 
 # task
 [core/task/supervised]
-model = core/model/generation/mbart
+model = core/model/generation/t5
 optim = core/optim/adamw
 scheduler = core/scheduler/linear_warmup
 dataset = core/dataset/ast
 loss_fn = core/loss/lm
 score_fn = core/score/bleu
 monitor_fns = ['core/score/bleu', 'core/score/rouge1', 'core/score/rouge2', 'core/score/rougel']
 output_header = ['encode']
-postprocess_fn = core/postprocess/mbart/detokenize
+postprocess_fn = core/postprocess/t5/detokenize
 writer = core/writer/csv
 
 from_ckpt_dir = ${core/cli:from_ckpt_dir}
 to_ckpt_dir = ${core/cli:cache_dir}
 output_path = ${core/cli:cache_dir}/output.txt
 train_batch_size = 4
 dev_batch_size = 8
```

### Comparing `unitorch-0.0.0.4/examples/configs/generation/mt5.ini` & `unitorch-0.0.0.5/examples/configs/generation/lora/bloom_ds.ini`

 * *Files 15% similar despite different names*

```diff
@@ -1,64 +1,61 @@
 [core/cli]
-task_name = core/task/supervised
+task_name = core/task/deepspeed/supervised
 from_ckpt_dir = ./cache
 cache_dir = ./cache
 train_file = ./train.tsv
 dev_file = ./dev.tsv
 test_file = ./test.tsv
 
 # model
-[core/model/generation/mt5]
-pretrained_name = mt5-base
-no_repeat_ngram_size = 3
-max_gen_seq_length = 15
+[core/model/generation/peft/lora/bloom]
+pretrained_name = bloom-560m
+max_gen_seq_length = 36
+num_beams = 2
 
 # dataset
 [core/dataset/ast]
 names = ['encode', 'decode']
 
 [core/dataset/ast/train]
 data_files = ${core/cli:train_file}
-preprocess_functions = ['core/process/mt5/generation(encode, decode)']
+preprocess_functions = ['core/process/bloom/generation(encode, decode)']
 
 [core/dataset/ast/dev]
 data_files = ${core/cli:dev_file}
-preprocess_functions = ['core/process/mt5/generation/inputs(encode)', 'core/process/mt5/generation/labels(decode)']
+preprocess_functions = ['core/process/bloom/generation/inputs(encode)', 'core/process/bloom/generation/labels(decode)']
 
 [core/dataset/ast/test]
-names = ['encode']
 data_files = ${core/cli:test_file}
-preprocess_functions = ['core/process/mt5/generation/inputs(encode)']
+preprocess_functions = ['core/process/bloom/generation/inputs(encode)']
 
 # process
-[core/process/mt5]
-pretrained_name = mt5-base
-max_seq_length = 24
-max_gen_seq_length = 15
-
-# optim
-[core/optim/adamw]
-learning_rate = 0.0001
-
-# scheduler
-[core/scheduler/linear_warmup]
-num_warmup_rate = 0.001
+[core/process/bloom]
+pretrained_name = bloom-560m
+max_seq_length = 64
+max_gen_seq_length = 36
+
+[core/writer/csv]
+escapechar = \
 
 # task
-[core/task/supervised]
-model = core/model/generation/mt5
-optim = core/optim/adamw
-scheduler = core/scheduler/linear_warmup
+[core/task/deepspeed/supervised]
+config_path = https://raw.githubusercontent.com/fuliucansheng/unitorch/master/examples/configs/deepspeed/adamw.json
+model = core/model/generation/peft/lora/bloom
 dataset = core/dataset/ast
 loss_fn = core/loss/lm
 score_fn = core/score/bleu
-monitor_fns = ['core/score/bleu', 'core/score/rouge1', 'core/score/rouge2', 'core/score/rougel']
-output_header = ['encode']
-postprocess_fn = core/postprocess/mt5/detokenize
+monitor_fns = ['core/score/bleu']
+
+ckpt_freq = 2000
+learning_rate = 0.00001
+
+output_header = ['encode', 'decode']
+postprocess_fn = core/postprocess/bloom/detokenize
 writer = core/writer/csv
 
 from_ckpt_dir = ${core/cli:from_ckpt_dir}
 to_ckpt_dir = ${core/cli:cache_dir}
 output_path = ${core/cli:cache_dir}/output.txt
 train_batch_size = 4
-dev_batch_size = 8
-test_batch_size = 8
+dev_batch_size = 4
+test_batch_size = 4
```

### Comparing `unitorch-0.0.0.4/examples/configs/generation/pegasus.ini` & `unitorch-0.0.0.5/examples/configs/generation/pegasus.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/examples/configs/generation/xpegasus.ini` & `unitorch-0.0.0.5/examples/configs/generation/xpegasus.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/examples/configs/generation/xprophetnet.ini` & `unitorch-0.0.0.5/examples/configs/generation/xprophetnet.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/examples/configs/pretrain/clip.ini` & `unitorch-0.0.0.5/examples/configs/pretrain/clip.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/pyproject.toml` & `unitorch-0.0.0.5/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -28,22 +28,24 @@
 dynamic = ["version", "dependencies"]
 
 [project.optional-dependencies]
 deepspeed = ["deepspeed==0.9.0", "mpi4py==3.1.4"]
 diffusers = ["diffusers==0.16.1"]
 accelerate = ["accelerate==0.20.3"]
 chatglm = ["protobuf==3.20.0", "icetk==0.0.4", "cpm_kernels==1.0.11"]
+fastapi = ["fastapi>=0.99.0"]
 all = ["unitorch[deepspeed,diffusers,accelerate,chatglm]"]
 
 [project.scripts]
 unitorch-train = "unitorch.cli.console.train:cli_main"
 unitorch-eval = "unitorch.cli.console.eval:cli_main"
 unitorch-infer = "unitorch.cli.console.infer:cli_main"
 unitorch-script= "unitorch.cli.console.script:cli_main"
 unitorch-service = "unitorch.cli.console.service:cli_main"
+unitorch-fastapi = "unitorch.cli.console.fastapi:cli_main"
 
 [tool.setuptools]
 include-package-data = true
 
 [tool.setuptools.packages.find]
 where = ["src"]
```

### Comparing `unitorch-0.0.0.4/setup.py` & `unitorch-0.0.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/__init__.py` & `unitorch-0.0.0.5/src/unitorch/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 
 def get_cache_home():
     return UNITORCH_CACHE
 
 
 ### version
-VERSION = "0.0.0.4"
+VERSION = "0.0.0.5"
 
 ### is offline mode
 UNITORCH_OFFLINE = os.environ.get("UNITORCH_OFFLINE", "0").upper()
 
 
 def is_offline_mode():
     return UNITORCH_OFFLINE in ENV_VARS_TRUE_VALUES
```

### Comparing `unitorch-0.0.0.4/src/unitorch/cli/__init__.py` & `unitorch-0.0.0.5/src/unitorch/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/cli/console/eval.py` & `unitorch-0.0.0.5/src/unitorch/cli/console/eval.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/cli/console/infer.py` & `unitorch-0.0.0.5/src/unitorch/cli/console/train.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     registered_task,
     registered_script,
     init_registered_module,
 )
 
 
 @fire.decorators.SetParseFn(str)
-def infer(config_path_or_dir: str, **kwargs):
+def train(config_path_or_dir: str, **kwargs):
     config_file = kwargs.pop("config_file", "config.ini")
 
     if os.path.isdir(config_path_or_dir):
         config_path = os.path.join(config_path_or_dir, config_file)
         sys.path.insert(0, config_path_or_dir)
         for f in os.listdir(config_path_or_dir):
             fpath = os.path.normpath(os.path.join(config_path_or_dir, f))
@@ -61,14 +61,14 @@
     if depends_libraries:
         for library in depends_libraries:
             import_library(library)
 
     assert task_name is not None and task_name in registered_task
     cli_task = init_registered_module(task_name, config, registered_task)
 
-    cli_task.infer()
+    cli_task.train()
 
     os._exit(0)
 
 
 def cli_main():
-    fire.Fire(infer)
+    fire.Fire(train)
```

### Comparing `unitorch-0.0.0.4/src/unitorch/cli/console/script.py` & `unitorch-0.0.0.5/src/unitorch/cli/console/script.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 import unitorch.cli
 from transformers.utils import is_remote_url
 from unitorch.cli import CoreConfigureParser
 from unitorch.cli import (
     import_library,
     cached_path,
     set_global_config,
-    registered_task,
     registered_script,
     init_registered_module,
 )
 
 
 @fire.decorators.SetParseFn(str)
 def script(script_path_or_dir: str, **kwargs):
```

### Comparing `unitorch-0.0.0.4/src/unitorch/cli/console/service.py` & `unitorch-0.0.0.5/src/unitorch/cli/console/service.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/cli/console/train.py` & `unitorch-0.0.0.5/src/unitorch/cli/console/infer.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,21 +10,20 @@
 from transformers.utils import is_remote_url
 from unitorch.cli import CoreConfigureParser
 from unitorch.cli import (
     import_library,
     cached_path,
     set_global_config,
     registered_task,
-    registered_script,
     init_registered_module,
 )
 
 
 @fire.decorators.SetParseFn(str)
-def train(config_path_or_dir: str, **kwargs):
+def infer(config_path_or_dir: str, **kwargs):
     config_file = kwargs.pop("config_file", "config.ini")
 
     if os.path.isdir(config_path_or_dir):
         config_path = os.path.join(config_path_or_dir, config_file)
         sys.path.insert(0, config_path_or_dir)
         for f in os.listdir(config_path_or_dir):
             fpath = os.path.normpath(os.path.join(config_path_or_dir, f))
@@ -61,14 +60,14 @@
     if depends_libraries:
         for library in depends_libraries:
             import_library(library)
 
     assert task_name is not None and task_name in registered_task
     cli_task = init_registered_module(task_name, config, registered_task)
 
-    cli_task.train()
+    cli_task.infer()
 
     os._exit(0)
 
 
 def cli_main():
-    fire.Fire(train)
+    fire.Fire(infer)
```

### Comparing `unitorch-0.0.0.4/src/unitorch/cli/core.py` & `unitorch-0.0.0.5/src/unitorch/cli/core.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/cli/datasets/hf.py` & `unitorch-0.0.0.5/src/unitorch/cli/datasets/hf.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/cli/decorators.py` & `unitorch-0.0.0.5/src/unitorch/cli/decorators.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/cli/loss/__init__.py` & `unitorch-0.0.0.5/src/unitorch/cli/loss/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/cli/loss/ranking.py` & `unitorch-0.0.0.5/src/unitorch/cli/loss/ranking.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/cli/models/__init__.py` & `unitorch-0.0.0.5/src/unitorch/cli/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,14 +76,15 @@
 import unitorch.cli.models.bert
 import unitorch.cli.models.beit
 import unitorch.cli.models.blip
 import unitorch.cli.models.bloom
 import unitorch.cli.models.chatglm
 import unitorch.cli.models.clip
 import unitorch.cli.models.deberta
+import unitorch.cli.models.minigpt4
 import unitorch.cli.models.llama
 import unitorch.cli.models.mbart
 import unitorch.cli.models.mt5
 import unitorch.cli.models.pegasus
 import unitorch.cli.models.peft
 import unitorch.cli.models.prophetnet
 import unitorch.cli.models.roberta
```

### Comparing `unitorch-0.0.0.4/src/unitorch/cli/models/bart/__init__.py` & `unitorch-0.0.0.5/src/unitorch/cli/models/bart/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/cli/models/bart/modeling.py` & `unitorch-0.0.0.5/src/unitorch/cli/models/bart/modeling.py`

 * *Files 0% similar despite different names*

```diff
@@ -106,15 +106,15 @@
     @torch.no_grad()
     @autocast()
     def generate(
         self,
         input_ids: torch.Tensor,
         num_beams: Optional[int] = 5,
         decoder_start_token_id: Optional[int] = 2,
-        decoder_end_token_id: Optional[int] = 2,
+        decoder_end_token_id: Optional[Union[int, List[int]]] = 2,
         num_return_sequences: Optional[int] = 1,
         min_gen_seq_length: Optional[int] = 0,
         max_gen_seq_length: Optional[int] = 48,
         repetition_penalty: Optional[float] = 1.0,
         no_repeat_ngram_size: Optional[int] = 0,
         early_stopping: Optional[bool] = True,
         length_penalty: Optional[float] = 1.0,
@@ -128,15 +128,15 @@
         """
         Generate sequences using the BartForGeneration model.
 
         Args:
             input_ids (torch.Tensor): Input IDs.
             num_beams (int, optional): Number of beams for beam search.
             decoder_start_token_id (int, optional): ID of the decoder start token.
-            decoder_end_token_id (int, optional): ID of the decoder end token.
+            decoder_end_token_id (int or List[int], optional): ID of the decoder end token.
             num_return_sequences (int, optional): Number of generated sequences to return.
             min_gen_seq_length (int, optional): Minimum length of generated sequences.
             max_gen_seq_length (int, optional): Maximum length of generated sequences.
             repetition_penalty (float, optional): Repetition penalty.
             no_repeat_ngram_size (int, optional): Size of n-grams to avoid repeating.
             early_stopping (bool, optional): Whether to stop generation early.
             length_penalty (float, optional): Length penalty for generated sequences.
```

### Comparing `unitorch-0.0.0.4/src/unitorch/cli/models/bart/processing.py` & `unitorch-0.0.0.5/src/unitorch/cli/models/bart/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/cli/models/beit/__init__.py` & `unitorch-0.0.0.5/src/unitorch/cli/models/beit/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/cli/models/beit/modeling.py` & `unitorch-0.0.0.5/src/unitorch/cli/models/beit/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/cli/models/beit/processing.py` & `unitorch-0.0.0.5/src/unitorch/cli/models/beit/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/cli/models/bert/__init__.py` & `unitorch-0.0.0.5/src/unitorch/cli/models/bert/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/cli/models/bert/modeling.py` & `unitorch-0.0.0.5/src/unitorch/cli/models/bert/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/cli/models/bert/processing.py` & `unitorch-0.0.0.5/src/unitorch/cli/models/bert/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/cli/models/blip/__init__.py` & `unitorch-0.0.0.5/src/unitorch/cli/models/blip/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/cli/models/blip/modeling.py` & `unitorch-0.0.0.5/src/unitorch/cli/models/blip/modeling.py`

 * *Files 1% similar despite different names*

```diff
@@ -521,15 +521,15 @@
     @torch.no_grad()
     @autocast()
     def generate(
         self,
         pixel_values: torch.Tensor,
         num_beams: Optional[int] = 5,
         decoder_start_token_id: Optional[int] = 101,
-        decoder_end_token_id: Optional[int] = 102,
+        decoder_end_token_id: Optional[Union[int, List[int]]] = 102,
         num_return_sequences: Optional[int] = 1,
         min_gen_seq_length: Optional[int] = 0,
         max_gen_seq_length: Optional[int] = 48,
         repetition_penalty: Optional[float] = 1.0,
         no_repeat_ngram_size: Optional[int] = 0,
         early_stopping: Optional[bool] = True,
         length_penalty: Optional[float] = 1.0,
@@ -543,15 +543,15 @@
         """
         Generate captions using the BlipForImageCaption model.
 
         Args:
             pixel_values (torch.Tensor): The pixel values of the images.
             num_beams (int, optional): The number of beams for beam search. Defaults to 5.
             decoder_start_token_id (int, optional): The start token ID for the decoder. Defaults to 30522.
-            decoder_end_token_id (int, optional): The end token ID for the decoder. Defaults to 2.
+            decoder_end_token_id (int or List[int], optional): The end token ID for the decoder. Defaults to 2.
             num_return_sequences (int, optional): The number of sequences to return. Defaults to 1.
             min_gen_seq_length (int, optional): The minimum length of generated sequences. Defaults to 0.
             max_gen_seq_length (int, optional): The maximum length of generated sequences. Defaults to 48.
             repetition_penalty (float, optional): The repetition penalty. Defaults to 1.0.
             no_repeat_ngram_size (int, optional): The size of n-grams to avoid repeating. Defaults to 0.
             early_stopping (bool, optional): Whether to perform early stopping. Defaults to True.
             length_penalty (float, optional): The length penalty. Defaults to 1.0.
```

### Comparing `unitorch-0.0.0.4/src/unitorch/cli/models/blip/processing.py` & `unitorch-0.0.0.5/src/unitorch/cli/models/blip/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/cli/models/bloom/__init__.py` & `unitorch-0.0.0.5/src/unitorch/cli/models/bloom/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/cli/models/bloom/modeling.py` & `unitorch-0.0.0.5/src/unitorch/cli/models/bloom/modeling.py`

 * *Files 1% similar despite different names*

```diff
@@ -277,15 +277,15 @@
     @torch.no_grad()
     @autocast()
     def generate(
         self,
         input_ids: torch.Tensor,
         num_beams: Optional[int] = 5,
         decoder_start_token_id: Optional[int] = 1,
-        decoder_end_token_id: Optional[int] = 2,
+        decoder_end_token_id: Optional[Union[int, List[int]]] = 2,
         num_return_sequences: Optional[int] = 1,
         min_gen_seq_length: Optional[int] = 0,
         max_gen_seq_length: Optional[int] = 48,
         repetition_penalty: Optional[float] = 1.0,
         no_repeat_ngram_size: Optional[int] = 0,
         early_stopping: Optional[bool] = True,
         length_penalty: Optional[float] = 1.0,
@@ -299,15 +299,15 @@
         """
         Generate sequences using the Bloom model.
 
         Args:
             input_ids (torch.Tensor): Input token IDs.
             num_beams (int, optional): Number of beams for beam search. Defaults to 5.
             decoder_start_token_id (int, optional): Decoder start token ID. Defaults to 0.
-            decoder_end_token_id (int, optional): Decoder end token ID. Defaults to 1.
+            decoder_end_token_id (int or List[int], optional): The ID(s) of the decoder end token(s). Defaults to 1.
             num_return_sequences (int, optional): Number of generated sequences to return. Defaults to 1.
             min_gen_seq_length (int, optional): Minimum generation sequence length. Defaults to 0.
             max_gen_seq_length (int, optional): Maximum generation sequence length. Defaults to 48.
             repetition_penalty (float, optional): Repetition penalty. Defaults to 1.0.
             no_repeat_ngram_size (int, optional): Size of n-grams to prevent repetition. Defaults to 0.
             early_stopping (bool, optional): Whether to perform early stopping. Defaults to True.
             length_penalty (float, optional): Length penalty. Defaults to 1.0.
```

### Comparing `unitorch-0.0.0.4/src/unitorch/cli/models/bloom/processing.py` & `unitorch-0.0.0.5/src/unitorch/cli/models/bloom/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/cli/models/chatglm/__init__.py` & `unitorch-0.0.0.5/src/unitorch/cli/models/chatglm/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/cli/models/chatglm/modeling.py` & `unitorch-0.0.0.5/src/unitorch/cli/models/chatglm/modeling.py`

 * *Files 2% similar despite different names*

```diff
@@ -287,15 +287,15 @@
     @torch.no_grad()
     @autocast()
     def generate(
         self,
         input_ids: torch.Tensor,
         num_beams: Optional[int] = 5,
         decoder_start_token_id: Optional[int] = 2,
-        decoder_end_token_id: Optional[int] = 2,
+        decoder_end_token_id: Optional[Union[int, List[int]]] = 2,
         num_return_sequences: Optional[int] = 1,
         min_gen_seq_length: Optional[int] = 0,
         max_gen_seq_length: Optional[int] = 48,
         repetition_penalty: Optional[float] = 1.0,
         no_repeat_ngram_size: Optional[int] = 0,
         early_stopping: Optional[bool] = True,
         length_penalty: Optional[float] = 1.0,
@@ -309,15 +309,15 @@
         """
         Generate sequences using the ChatGLM model.
 
         Args:
             input_ids (torch.Tensor): Input token IDs.
             num_beams (int, optional): Number of beams for beam search. Defaults to 5.
             decoder_start_token_id (int, optional): Decoder start token ID. Defaults to 0.
-            decoder_end_token_id (int, optional): Decoder end token ID. Defaults to 1.
+            decoder_end_token_id (int or List[int], optional): The ID(s) of the decoder end token(s). Defaults to 1.
             num_return_sequences (int, optional): Number of generated sequences to return. Defaults to 1.
             min_gen_seq_length (int, optional): Minimum generation sequence length. Defaults to 0.
             max_gen_seq_length (int, optional): Maximum generation sequence length. Defaults to 48.
             repetition_penalty (float, optional): Repetition penalty. Defaults to 1.0.
             no_repeat_ngram_size (int, optional): Size of n-grams to prevent repetition. Defaults to 0.
             early_stopping (bool, optional): Whether to perform early stopping. Defaults to True.
             length_penalty (float, optional): Length penalty. Defaults to 1.0.
```

### Comparing `unitorch-0.0.0.4/src/unitorch/cli/models/chatglm/processing.py` & `unitorch-0.0.0.5/src/unitorch/cli/models/chatglm/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/cli/models/classification_utils.py` & `unitorch-0.0.0.5/src/unitorch/cli/models/classification_utils.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/cli/models/clip/__init__.py` & `unitorch-0.0.0.5/src/unitorch/cli/models/clip/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/cli/models/clip/modeling.py` & `unitorch-0.0.0.5/src/unitorch/cli/models/clip/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/cli/models/clip/processing.py` & `unitorch-0.0.0.5/src/unitorch/cli/models/clip/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/cli/models/deberta/__init__.py` & `unitorch-0.0.0.5/src/unitorch/cli/models/deberta/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/cli/models/deberta/modeling.py` & `unitorch-0.0.0.5/src/unitorch/cli/models/deberta/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/cli/models/deberta/modeling_v2.py` & `unitorch-0.0.0.5/src/unitorch/cli/models/deberta/modeling_v2.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/cli/models/deberta/processing.py` & `unitorch-0.0.0.5/src/unitorch/cli/models/deberta/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/cli/models/deberta/processing_v2.py` & `unitorch-0.0.0.5/src/unitorch/cli/models/deberta/processing_v2.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/cli/models/detection_utils.py` & `unitorch-0.0.0.5/src/unitorch/cli/models/detection_utils.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/cli/models/diffusers/__init__.py` & `unitorch-0.0.0.5/src/unitorch/cli/models/diffusers/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/cli/models/diffusers/modeling_controlnet.py` & `unitorch-0.0.0.5/src/unitorch/cli/models/diffusers/modeling_controlnet.py`

 * *Files 0% similar despite different names*

```diff
@@ -134,22 +134,23 @@
         if weight_path is None and pretrain_infos is not None:
             weight_path = [
                 cached_path(nested_dict_value(pretrain_infos, "unet", "weight")),
                 cached_path(nested_dict_value(pretrain_infos, "text", "weight")),
                 cached_path(nested_dict_value(pretrain_infos, "vae", "weight")),
                 # cached_path(nested_dict_value(pretrain_infos, "controlnet", "weight")),
             ]
-            controlnet = cached_path(nested_dict_value(pretrain_infos, "controlnet", "weight"))
+            controlnet = cached_path(
+                nested_dict_value(pretrain_infos, "controlnet", "weight")
+            )
             state_dict = torch.load(controlnet, map_location="cpu")
-            state_dict = {f"controlnet.{k}": v for k, v in state_dict.items()} 
-
+            state_dict = {f"controlnet.{k}": v for k, v in state_dict.items()}
 
         if weight_path is not None:
             inst.from_pretrained(weight_path, state_dict=state_dict)
-        
+
         return inst
 
     @autocast()
     def forward(
         self,
         input_ids: torch.Tensor,
         pixel_values: torch.Tensor,
```

### Comparing `unitorch-0.0.0.4/src/unitorch/cli/models/diffusers/modeling_stable.py` & `unitorch-0.0.0.5/src/unitorch/cli/models/diffusers/modeling_stable.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/cli/models/diffusers/processing_controlnet.py` & `unitorch-0.0.0.5/src/unitorch/cli/models/diffusers/processing_controlnet.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/cli/models/diffusers/processing_stable.py` & `unitorch-0.0.0.5/src/unitorch/cli/models/diffusers/processing_stable.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/cli/models/diffusion_utils.py` & `unitorch-0.0.0.5/src/unitorch/cli/models/diffusion_utils.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/cli/models/generation_utils.py` & `unitorch-0.0.0.5/src/unitorch/cli/models/generation_utils.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/cli/models/image_utils.py` & `unitorch-0.0.0.5/src/unitorch/cli/models/image_utils.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/cli/models/label_utils.py` & `unitorch-0.0.0.5/src/unitorch/cli/models/label_utils.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/cli/models/llama/__init__.py` & `unitorch-0.0.0.5/src/unitorch/cli/models/llama/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -36,14 +36,35 @@
         "config": "https://huggingface.co/huggyllama/llama-13b/resolve/main/config.json",
         "vocab": "https://huggingface.co/huggyllama/llama-13b/resolve/main/tokenizer.model",
         "weight": [
             f"https://huggingface.co/huggyllama/llama-13b/resolve/main/pytorch_model-{str(i).rjust(5, '0')}-of-00003.bin"
             for i in range(1, 4)
         ],
     },
+    "open-llama-3b": {
+        "config": "https://huggingface.co/openlm-research/open_llama_3b/resolve/main/config.json",
+        "vocab": "https://huggingface.co/openlm-research/open_llama_3b/resolve/main/tokenizer.model",
+        "weight": "https://huggingface.co/openlm-research/open_llama_3b/resolve/main/pytorch_model.bin",
+    },
+    "open-llama-7b": {
+        "config": "https://huggingface.co/openlm-research/open_llama_7b/resolve/main/config.json",
+        "vocab": "https://huggingface.co/openlm-research/open_llama_7b/resolve/main/tokenizer.model",
+        "weight": [
+            f"https://huggingface.co/openlm-research/open_llama_7b/resolve/main/pytorch_model-{str(i).rjust(5, '0')}-of-00002.bin"
+            for i in range(1, 3)
+        ],
+    },
+    "open-llama-13b": {
+        "config": "https://huggingface.co/openlm-research/open_llama_13b/resolve/main/config.json",
+        "vocab": "https://huggingface.co/openlm-research/open_llama_13b/resolve/main/tokenizer.model",
+        "weight": [
+            f"https://huggingface.co/openlm-research/open_llama_13b/resolve/main/pytorch_model-{str(i).rjust(5, '0')}-of-00003.bin"
+            for i in range(1, 4)
+        ],
+    },
 }
 
 import unitorch.cli.models.llama.modeling
 import unitorch.cli.models.llama.processing
 from unitorch.cli.models.llama.modeling import (
     LlamaForClassification,
     LlamaForPretrain,
```

### Comparing `unitorch-0.0.0.4/src/unitorch/cli/models/llama/modeling.py` & `unitorch-0.0.0.5/src/unitorch/cli/models/llama/modeling.py`

 * *Files 1% similar despite different names*

```diff
@@ -294,15 +294,15 @@
     @torch.no_grad()
     @autocast()
     def generate(
         self,
         input_ids: torch.Tensor,
         num_beams: Optional[int] = 5,
         decoder_start_token_id: Optional[int] = 1,
-        decoder_end_token_id: Optional[int] = 2,
+        decoder_end_token_id: Optional[Union[int, List[int]]] = 2,
         num_return_sequences: Optional[int] = 1,
         min_gen_seq_length: Optional[int] = 0,
         max_gen_seq_length: Optional[int] = 48,
         repetition_penalty: Optional[float] = 1.0,
         no_repeat_ngram_size: Optional[int] = 0,
         early_stopping: Optional[bool] = True,
         length_penalty: Optional[float] = 1.0,
@@ -315,16 +315,16 @@
     ):
         """
         Generate sequences using the Llama model.
 
         Args:
             input_ids (torch.Tensor): Input token IDs.
             num_beams (int, optional): Number of beams for beam search. Defaults to 5.
-            decoder_start_token_id (int, optional): Decoder start token ID. Defaults to 0.
-            decoder_end_token_id (int, optional): Decoder end token ID. Defaults to 1.
+            decoder_start_token_id (int, optional): Decoder start token ID. Defaults to 1.
+            decoder_end_token_id (int or List[int], optional): The ID(s) of the decoder end token(s). Defaults to 2.
             num_return_sequences (int, optional): Number of generated sequences to return. Defaults to 1.
             min_gen_seq_length (int, optional): Minimum generation sequence length. Defaults to 0.
             max_gen_seq_length (int, optional): Maximum generation sequence length. Defaults to 48.
             repetition_penalty (float, optional): Repetition penalty. Defaults to 1.0.
             no_repeat_ngram_size (int, optional): Size of n-grams to prevent repetition. Defaults to 0.
             early_stopping (bool, optional): Whether to perform early stopping. Defaults to True.
             length_penalty (float, optional): Length penalty. Defaults to 1.0.
```

### Comparing `unitorch-0.0.0.4/src/unitorch/cli/models/llama/processing.py` & `unitorch-0.0.0.5/src/unitorch/cli/models/llama/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/cli/models/mbart/__init__.py` & `unitorch-0.0.0.5/src/unitorch/cli/models/mbart/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/cli/models/mbart/modeling.py` & `unitorch-0.0.0.5/src/unitorch/cli/models/mbart/modeling.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,15 +115,15 @@
     @torch.no_grad()
     @autocast()
     def generate(
         self,
         input_ids: torch.Tensor,
         num_beams: Optional[int] = 5,
         decoder_start_token_id: Optional[int] = 2,
-        decoder_end_token_id: Optional[int] = 2,
+        decoder_end_token_id: Optional[Union[int, List[int]]] = 2,
         num_return_sequences: Optional[int] = 1,
         min_gen_seq_length: Optional[int] = 0,
         max_gen_seq_length: Optional[int] = 48,
         repetition_penalty: Optional[float] = 1.0,
         no_repeat_ngram_size: Optional[int] = 0,
         early_stopping: Optional[bool] = True,
         length_penalty: Optional[float] = 1.0,
@@ -137,15 +137,15 @@
         """
         Generate sequences using the MBart model.
 
         Args:
             input_ids (torch.Tensor): Input token IDs.
             num_beams (int, optional): Number of beams for beam search. Defaults to 5.
             decoder_start_token_id (int, optional): Decoder start token ID. Defaults to 0.
-            decoder_end_token_id (int, optional): Decoder end token ID. Defaults to 1.
+            decoder_end_token_id (int or List[int], optional): The ID(s) of the decoder end token(s). Defaults to 1.
             num_return_sequences (int, optional): Number of generated sequences to return. Defaults to 1.
             min_gen_seq_length (int, optional): Minimum generation sequence length. Defaults to 0.
             max_gen_seq_length (int, optional): Maximum generation sequence length. Defaults to 48.
             repetition_penalty (float, optional): Repetition penalty. Defaults to 1.0.
             no_repeat_ngram_size (int, optional): Size of n-grams to prevent repetition. Defaults to 0.
             early_stopping (bool, optional): Whether to perform early stopping. Defaults to True.
             length_penalty (float, optional): Length penalty. Defaults to 1.0.
```

### Comparing `unitorch-0.0.0.4/src/unitorch/cli/models/mbart/processing.py` & `unitorch-0.0.0.5/src/unitorch/cli/models/mbart/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/cli/models/modeling_utils.py` & `unitorch-0.0.0.5/src/unitorch/cli/models/modeling_utils.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/cli/models/mt5/__init__.py` & `unitorch-0.0.0.5/src/unitorch/cli/models/mt5/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/cli/models/mt5/modeling.py` & `unitorch-0.0.0.5/src/unitorch/cli/models/mt5/modeling.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,15 +106,15 @@
     @torch.no_grad()
     @autocast()
     def generate(
         self,
         input_ids: torch.Tensor,
         num_beams: Optional[int] = 5,
         decoder_start_token_id: Optional[int] = 0,
-        decoder_end_token_id: Optional[int] = 1,
+        decoder_end_token_id: Optional[Union[int, List[int]]] = 1,
         num_return_sequences: Optional[int] = 1,
         min_gen_seq_length: Optional[int] = 0,
         max_gen_seq_length: Optional[int] = 48,
         repetition_penalty: Optional[float] = 1.0,
         no_repeat_ngram_size: Optional[int] = 0,
         early_stopping: Optional[bool] = True,
         length_penalty: Optional[float] = 1.0,
@@ -128,15 +128,15 @@
         """
         Generate sequences using the MT5 model.
 
         Args:
             input_ids (torch.Tensor): Input token IDs.
             num_beams (int, optional): Number of beams for beam search. Defaults to 5.
             decoder_start_token_id (int, optional): Decoder start token ID. Defaults to 0.
-            decoder_end_token_id (int, optional): Decoder end token ID. Defaults to 1.
+            decoder_end_token_id (int or List[int], optional): The ID(s) of the decoder end token(s). Defaults to 1.
             num_return_sequences (int, optional): Number of generated sequences to return. Defaults to 1.
             min_gen_seq_length (int, optional): Minimum generation sequence length. Defaults to 0.
             max_gen_seq_length (int, optional): Maximum generation sequence length. Defaults to 48.
             repetition_penalty (float, optional): Repetition penalty. Defaults to 1.0.
             no_repeat_ngram_size (int, optional): Size of n-grams to prevent repetition. Defaults to 0.
             early_stopping (bool, optional): Whether to perform early stopping. Defaults to True.
             length_penalty (float, optional): Length penalty. Defaults to 1.0.
```

### Comparing `unitorch-0.0.0.4/src/unitorch/cli/models/mt5/processing.py` & `unitorch-0.0.0.5/src/unitorch/cli/models/mt5/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/cli/models/peft/__init__.py` & `unitorch-0.0.0.5/src/unitorch/cli/models/peft/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/cli/models/peft/modeling_bloom.py` & `unitorch-0.0.0.5/src/unitorch/cli/models/peft/modeling_bloom.py`

 * *Files 2% similar despite different names*

```diff
@@ -339,15 +339,15 @@
     @torch.no_grad()
     @autocast()
     def generate(
         self,
         input_ids: torch.Tensor,
         num_beams: Optional[int] = 5,
         decoder_start_token_id: Optional[int] = 1,
-        decoder_end_token_id: Optional[int] = 2,
+        decoder_end_token_id: Optional[Union[int, List[int]]] = 2,
         num_return_sequences: Optional[int] = 1,
         min_gen_seq_length: Optional[int] = 0,
         max_gen_seq_length: Optional[int] = 48,
         repetition_penalty: Optional[float] = 1.0,
         no_repeat_ngram_size: Optional[int] = 0,
         early_stopping: Optional[bool] = True,
         length_penalty: Optional[float] = 1.0,
@@ -361,15 +361,15 @@
         """
         Generate sequences using the Bloom model.
 
         Args:
             input_ids (torch.Tensor): Input token IDs.
             num_beams (int, optional): Number of beams for beam search. Defaults to 5.
             decoder_start_token_id (int, optional): Decoder start token ID. Defaults to 0.
-            decoder_end_token_id (int, optional): Decoder end token ID. Defaults to 1.
+            decoder_end_token_id (int or List[int], optional): The ID(s) of the decoder end token(s). Defaults to 1.
             num_return_sequences (int, optional): Number of generated sequences to return. Defaults to 1.
             min_gen_seq_length (int, optional): Minimum generation sequence length. Defaults to 0.
             max_gen_seq_length (int, optional): Maximum generation sequence length. Defaults to 48.
             repetition_penalty (float, optional): Repetition penalty. Defaults to 1.0.
             no_repeat_ngram_size (int, optional): Size of n-grams to prevent repetition. Defaults to 0.
             early_stopping (bool, optional): Whether to perform early stopping. Defaults to True.
             length_penalty (float, optional): Length penalty. Defaults to 1.0.
@@ -671,15 +671,15 @@
     @torch.no_grad()
     @autocast()
     def generate(
         self,
         input_ids: torch.Tensor,
         num_beams: Optional[int] = 5,
         decoder_start_token_id: Optional[int] = 1,
-        decoder_end_token_id: Optional[int] = 2,
+        decoder_end_token_id: Optional[Union[int, List[int]]] = 2,
         num_return_sequences: Optional[int] = 1,
         min_gen_seq_length: Optional[int] = 0,
         max_gen_seq_length: Optional[int] = 48,
         repetition_penalty: Optional[float] = 1.0,
         no_repeat_ngram_size: Optional[int] = 0,
         early_stopping: Optional[bool] = True,
         length_penalty: Optional[float] = 1.0,
@@ -693,15 +693,15 @@
         """
         Generate sequences using the Bloom model.
 
         Args:
             input_ids (torch.Tensor): Input token IDs.
             num_beams (int, optional): Number of beams for beam search. Defaults to 5.
             decoder_start_token_id (int, optional): Decoder start token ID. Defaults to 0.
-            decoder_end_token_id (int, optional): Decoder end token ID. Defaults to 1.
+            decoder_end_token_id (int or List[int], optional): The ID(s) of the decoder end token(s). Defaults to 1.
             num_return_sequences (int, optional): Number of generated sequences to return. Defaults to 1.
             min_gen_seq_length (int, optional): Minimum generation sequence length. Defaults to 0.
             max_gen_seq_length (int, optional): Maximum generation sequence length. Defaults to 48.
             repetition_penalty (float, optional): Repetition penalty. Defaults to 1.0.
             no_repeat_ngram_size (int, optional): Size of n-grams to prevent repetition. Defaults to 0.
             early_stopping (bool, optional): Whether to perform early stopping. Defaults to True.
             length_penalty (float, optional): Length penalty. Defaults to 1.0.
```

### Comparing `unitorch-0.0.0.4/src/unitorch/cli/models/peft/modeling_llama.py` & `unitorch-0.0.0.5/src/unitorch/cli/models/peft/modeling_llama.py`

 * *Files 1% similar despite different names*

```diff
@@ -340,15 +340,15 @@
     @torch.no_grad()
     @autocast()
     def generate(
         self,
         input_ids: torch.Tensor,
         num_beams: Optional[int] = 5,
         decoder_start_token_id: Optional[int] = 1,
-        decoder_end_token_id: Optional[int] = 2,
+        decoder_end_token_id: Optional[Union[int, List[int]]] = 2,
         num_return_sequences: Optional[int] = 1,
         min_gen_seq_length: Optional[int] = 0,
         max_gen_seq_length: Optional[int] = 48,
         repetition_penalty: Optional[float] = 1.0,
         no_repeat_ngram_size: Optional[int] = 0,
         early_stopping: Optional[bool] = True,
         length_penalty: Optional[float] = 1.0,
@@ -362,15 +362,15 @@
         """
         Generate sequences using the Llama model.
 
         Args:
             input_ids (torch.Tensor): Input token IDs.
             num_beams (int, optional): Number of beams for beam search. Defaults to 5.
             decoder_start_token_id (int, optional): Decoder start token ID. Defaults to 0.
-            decoder_end_token_id (int, optional): Decoder end token ID. Defaults to 1.
+            decoder_end_token_id (int or List[int], optional): The ID(s) of the decoder end token(s). Defaults to 1.
             num_return_sequences (int, optional): Number of generated sequences to return. Defaults to 1.
             min_gen_seq_length (int, optional): Minimum generation sequence length. Defaults to 0.
             max_gen_seq_length (int, optional): Maximum generation sequence length. Defaults to 48.
             repetition_penalty (float, optional): Repetition penalty. Defaults to 1.0.
             no_repeat_ngram_size (int, optional): Size of n-grams to prevent repetition. Defaults to 0.
             early_stopping (bool, optional): Whether to perform early stopping. Defaults to True.
             length_penalty (float, optional): Length penalty. Defaults to 1.0.
@@ -674,15 +674,15 @@
     @torch.no_grad()
     @autocast()
     def generate(
         self,
         input_ids: torch.Tensor,
         num_beams: Optional[int] = 5,
         decoder_start_token_id: Optional[int] = 1,
-        decoder_end_token_id: Optional[int] = 2,
+        decoder_end_token_id: Optional[Union[int, List[int]]] = 2,
         num_return_sequences: Optional[int] = 1,
         min_gen_seq_length: Optional[int] = 0,
         max_gen_seq_length: Optional[int] = 48,
         repetition_penalty: Optional[float] = 1.0,
         no_repeat_ngram_size: Optional[int] = 0,
         early_stopping: Optional[bool] = True,
         length_penalty: Optional[float] = 1.0,
@@ -696,15 +696,15 @@
         """
         Generate sequences using the Llama model.
 
         Args:
             input_ids (torch.Tensor): Input token IDs.
             num_beams (int, optional): Number of beams for beam search. Defaults to 5.
             decoder_start_token_id (int, optional): Decoder start token ID. Defaults to 0.
-            decoder_end_token_id (int, optional): Decoder end token ID. Defaults to 1.
+            decoder_end_token_id (int or List[int], optional): The ID(s) of the decoder end token(s). Defaults to 1.
             num_return_sequences (int, optional): Number of generated sequences to return. Defaults to 1.
             min_gen_seq_length (int, optional): Minimum generation sequence length. Defaults to 0.
             max_gen_seq_length (int, optional): Maximum generation sequence length. Defaults to 48.
             repetition_penalty (float, optional): Repetition penalty. Defaults to 1.0.
             no_repeat_ngram_size (int, optional): Size of n-grams to prevent repetition. Defaults to 0.
             early_stopping (bool, optional): Whether to perform early stopping. Defaults to True.
             length_penalty (float, optional): Length penalty. Defaults to 1.0.
```

### Comparing `unitorch-0.0.0.4/src/unitorch/cli/models/pegasus/__init__.py` & `unitorch-0.0.0.5/src/unitorch/cli/models/pegasus/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/cli/models/pegasus/modeling.py` & `unitorch-0.0.0.5/src/unitorch/cli/models/pegasus/modeling.py`

 * *Files 0% similar despite different names*

```diff
@@ -107,15 +107,15 @@
     @torch.no_grad()
     @autocast()
     def generate(
         self,
         input_ids: torch.Tensor,
         num_beams: Optional[int] = 5,
         decoder_start_token_id: Optional[int] = 0,
-        decoder_end_token_id: Optional[int] = 1,
+        decoder_end_token_id: Optional[Union[int, List[int]]] = 1,
         num_return_sequences: Optional[int] = 1,
         min_gen_seq_length: Optional[int] = 0,
         max_gen_seq_length: Optional[int] = 48,
         repetition_penalty: Optional[float] = 1.0,
         no_repeat_ngram_size: Optional[int] = 0,
         early_stopping: Optional[bool] = True,
         length_penalty: Optional[float] = 1.0,
@@ -129,15 +129,15 @@
         """
         Generate sequences using the Pegasus model.
 
         Args:
             input_ids (torch.Tensor): Input token IDs.
             num_beams (int, optional): Number of beams for beam search. Defaults to 5.
             decoder_start_token_id (int, optional): Decoder start token ID. Defaults to 0.
-            decoder_end_token_id (int, optional): Decoder end token ID. Defaults to 1.
+            decoder_end_token_id (int or List[int], optional): The ID(s) of the decoder end token(s). Defaults to 1.
             num_return_sequences (int, optional): Number of generated sequences to return. Defaults to 1.
             min_gen_seq_length (int, optional): Minimum generation sequence length. Defaults to 0.
             max_gen_seq_length (int, optional): Maximum generation sequence length. Defaults to 48.
             repetition_penalty (float, optional): Repetition penalty. Defaults to 1.0.
             no_repeat_ngram_size (int, optional): Size of n-grams to prevent repetition. Defaults to 0.
             early_stopping (bool, optional): Whether to perform early stopping. Defaults to True.
             length_penalty (float, optional): Length penalty. Defaults to 1.0.
```

### Comparing `unitorch-0.0.0.4/src/unitorch/cli/models/pegasus/processing.py` & `unitorch-0.0.0.5/src/unitorch/cli/models/pegasus/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/cli/models/processing_utils.py` & `unitorch-0.0.0.5/src/unitorch/cli/models/processing_utils.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/cli/models/random_utils.py` & `unitorch-0.0.0.5/src/unitorch/cli/models/random_utils.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/cli/models/ranking_utils.py` & `unitorch-0.0.0.5/src/unitorch/cli/models/ranking_utils.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/cli/models/roberta/__init__.py` & `unitorch-0.0.0.5/src/unitorch/cli/models/roberta/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/cli/models/roberta/modeling.py` & `unitorch-0.0.0.5/src/unitorch/cli/models/roberta/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/cli/models/roberta/processing.py` & `unitorch-0.0.0.5/src/unitorch/cli/models/roberta/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/cli/models/segmentation_utils.py` & `unitorch-0.0.0.5/src/unitorch/cli/models/segmentation_utils.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/cli/models/swin/__init__.py` & `unitorch-0.0.0.5/src/unitorch/cli/models/swin/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/cli/models/swin/modeling.py` & `unitorch-0.0.0.5/src/unitorch/cli/models/swin/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/cli/models/swin/processing.py` & `unitorch-0.0.0.5/src/unitorch/cli/models/swin/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/cli/models/t5/__init__.py` & `unitorch-0.0.0.5/src/unitorch/cli/models/t5/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/cli/models/t5/modeling.py` & `unitorch-0.0.0.5/src/unitorch/cli/models/t5/modeling.py`

 * *Files 0% similar despite different names*

```diff
@@ -107,15 +107,15 @@
     @torch.no_grad()
     @autocast()
     def generate(
         self,
         input_ids: torch.Tensor,
         num_beams: Optional[int] = 5,
         decoder_start_token_id: Optional[int] = 0,
-        decoder_end_token_id: Optional[int] = 1,
+        decoder_end_token_id: Optional[Union[int, List[int]]] = 1,
         num_return_sequences: Optional[int] = 1,
         min_gen_seq_length: Optional[int] = 0,
         max_gen_seq_length: Optional[int] = 48,
         repetition_penalty: Optional[float] = 1.0,
         no_repeat_ngram_size: Optional[int] = 0,
         early_stopping: Optional[bool] = True,
         length_penalty: Optional[float] = 1.0,
@@ -129,15 +129,15 @@
         """
         Generate sequences using the T5 model.
 
         Args:
             input_ids (torch.Tensor): Input token IDs.
             num_beams (int, optional): Number of beams for beam search. Defaults to 5.
             decoder_start_token_id (int, optional): Decoder start token ID. Defaults to 0.
-            decoder_end_token_id (int, optional): Decoder end token ID. Defaults to 1.
+            decoder_end_token_id (int or List[int], optional): The ID(s) of the decoder end token(s). Defaults to 1.
             num_return_sequences (int, optional): Number of generated sequences to return. Defaults to 1.
             min_gen_seq_length (int, optional): Minimum generation sequence length. Defaults to 0.
             max_gen_seq_length (int, optional): Maximum generation sequence length. Defaults to 48.
             repetition_penalty (float, optional): Repetition penalty. Defaults to 1.0.
             no_repeat_ngram_size (int, optional): Size of n-grams to prevent repetition. Defaults to 0.
             early_stopping (bool, optional): Whether to perform early stopping. Defaults to True.
             length_penalty (float, optional): Length penalty. Defaults to 1.0.
```

### Comparing `unitorch-0.0.0.4/src/unitorch/cli/models/t5/processing.py` & `unitorch-0.0.0.5/src/unitorch/cli/models/t5/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/cli/models/visualbert/__init__.py` & `unitorch-0.0.0.5/src/unitorch/cli/models/visualbert/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/cli/models/visualbert/modeling.py` & `unitorch-0.0.0.5/src/unitorch/cli/models/visualbert/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/cli/models/visualbert/processing.py` & `unitorch-0.0.0.5/src/unitorch/cli/models/visualbert/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/cli/models/vit/__init__.py` & `unitorch-0.0.0.5/src/unitorch/cli/models/vit/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/cli/models/vit/modeling.py` & `unitorch-0.0.0.5/src/unitorch/cli/models/vit/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/cli/models/vit/processing.py` & `unitorch-0.0.0.5/src/unitorch/cli/models/vit/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/cli/models/xlm_roberta/__init__.py` & `unitorch-0.0.0.5/src/unitorch/cli/models/xlm_roberta/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/cli/models/xlm_roberta/modeling.py` & `unitorch-0.0.0.5/src/unitorch/cli/models/xlm_roberta/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/cli/models/xlm_roberta/processing.py` & `unitorch-0.0.0.5/src/unitorch/cli/models/xlm_roberta/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/cli/models/xpegasus/__init__.py` & `unitorch-0.0.0.5/src/unitorch/cli/models/xpegasus/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/cli/models/xpegasus/modeling.py` & `unitorch-0.0.0.5/src/unitorch/cli/models/xpegasus/modeling.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,15 +71,15 @@
         )
         if weight_path is not None:
             weight_path = cached_path(weight_path)
             inst.from_pretrained(weight_path)
 
         return inst
 
-    #@autocast()
+    # @autocast()
     def forward(
         self,
         input_ids: torch.Tensor,
         attention_mask: torch.Tensor,
         decoder_input_ids: torch.Tensor,
         decoder_attention_mask: torch.Tensor,
     ):
@@ -107,15 +107,15 @@
     @torch.no_grad()
     @autocast()
     def generate(
         self,
         input_ids: torch.Tensor,
         num_beams: Optional[int] = 5,
         decoder_start_token_id: Optional[int] = 0,
-        decoder_end_token_id: Optional[int] = 1,
+        decoder_end_token_id: Optional[Union[int, List[int]]] = 1,
         num_return_sequences: Optional[int] = 1,
         min_gen_seq_length: Optional[int] = 0,
         max_gen_seq_length: Optional[int] = 48,
         repetition_penalty: Optional[float] = 1.0,
         no_repeat_ngram_size: Optional[int] = 0,
         early_stopping: Optional[bool] = True,
         length_penalty: Optional[float] = 1.0,
@@ -129,15 +129,15 @@
         """
         Generate sequences using the XPegasus model.
 
         Args:
             input_ids (torch.Tensor): Input token IDs.
             num_beams (int, optional): Number of beams for beam search. Defaults to 5.
             decoder_start_token_id (int, optional): Decoder start token ID. Defaults to 0.
-            decoder_end_token_id (int, optional): Decoder end token ID. Defaults to 1.
+            decoder_end_token_id (int or List[int], optional): The ID(s) of the decoder end token(s). Defaults to 1.
             num_return_sequences (int, optional): Number of generated sequences to return. Defaults to 1.
             min_gen_seq_length (int, optional): Minimum generation sequence length. Defaults to 0.
             max_gen_seq_length (int, optional): Maximum generation sequence length. Defaults to 48.
             repetition_penalty (float, optional): Repetition penalty. Defaults to 1.0.
             no_repeat_ngram_size (int, optional): Size of n-grams to prevent repetition. Defaults to 0.
             early_stopping (bool, optional): Whether to perform early stopping. Defaults to True.
             length_penalty (float, optional): Length penalty. Defaults to 1.0.
```

### Comparing `unitorch-0.0.0.4/src/unitorch/cli/models/xpegasus/processing.py` & `unitorch-0.0.0.5/src/unitorch/cli/models/xpegasus/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/cli/models/xprophetnet/__init__.py` & `unitorch-0.0.0.5/src/unitorch/cli/models/xprophetnet/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/cli/models/xprophetnet/modeling.py` & `unitorch-0.0.0.5/src/unitorch/cli/models/xprophetnet/modeling.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,15 +116,15 @@
     @torch.no_grad()
     @autocast()
     def generate(
         self,
         input_ids: torch.Tensor,
         num_beams: Optional[int] = 5,
         decoder_start_token_id: Optional[int] = 2,
-        decoder_end_token_id: Optional[int] = 2,
+        decoder_end_token_id: Optional[Union[int, List[int]]] = 2,
         num_return_sequences: Optional[int] = 1,
         min_gen_seq_length: Optional[int] = 0,
         max_gen_seq_length: Optional[int] = 48,
         repetition_penalty: Optional[float] = 1.0,
         no_repeat_ngram_size: Optional[int] = 0,
         early_stopping: Optional[bool] = True,
         length_penalty: Optional[float] = 1.0,
@@ -138,15 +138,15 @@
         """
         Generate sequences using the XProphetNetForGeneration model.
 
         Args:
             input_ids (torch.Tensor): Input tensor IDs.
             num_beams (int, optional): The number of beams for beam search. Defaults to 5.
             decoder_start_token_id (int, optional): The ID of the decoder start token. Defaults to 2.
-            decoder_end_token_id (int, optional): The ID of the decoder end token. Defaults to 2.
+            decoder_end_token_id (int or List[int], optional): The ID of the decoder end token. Defaults to 2.
             num_return_sequences (int, optional): The number of returned sequences. Defaults to 1.
             min_gen_seq_length (int, optional): The minimum generated sequence length. Defaults to 0.
             max_gen_seq_length (int, optional): The maximum generated sequence length. Defaults to 48.
             repetition_penalty (float, optional): The repetition penalty. Defaults to 1.0.
             no_repeat_ngram_size (int, optional): The size of n-grams that should not be repeated. Defaults to 0.
             early_stopping (bool, optional): Whether to stop generation early. Defaults to True.
             length_penalty (float, optional): The length penalty. Defaults to 1.0.
```

### Comparing `unitorch-0.0.0.4/src/unitorch/cli/models/xprophetnet/processing.py` & `unitorch-0.0.0.5/src/unitorch/cli/models/xprophetnet/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/cli/optim/__init__.py` & `unitorch-0.0.0.5/src/unitorch/cli/optim/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/cli/optim/lion.py` & `unitorch-0.0.0.5/src/unitorch/cli/optim/lion.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/cli/scheduler/warmup.py` & `unitorch-0.0.0.5/src/unitorch/cli/scheduler/warmup.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/cli/score/__init__.py` & `unitorch-0.0.0.5/src/unitorch/cli/score/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/cli/services/zip_image/service.py` & `unitorch-0.0.0.5/src/unitorch/cli/services/zip_image/service.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/cli/tasks/deepspeed.py` & `unitorch-0.0.0.5/src/unitorch/cli/tasks/deepspeed.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/cli/tasks/supervised.py` & `unitorch-0.0.0.5/src/unitorch/cli/tasks/supervised.py`

 * *Files 1% similar despite different names*

```diff
@@ -375,15 +375,18 @@
                 self.config,
                 registered_optim,
                 params=self.model.parameters(),
             )
 
         if os.path.exists(from_ckpt_dir):
             self.model.from_checkpoint(from_ckpt_dir)
-            optim.from_checkpoint(from_ckpt_dir, weight_name="pytorch_optim.bin",)
+            optim.from_checkpoint(
+                from_ckpt_dir,
+                weight_name="pytorch_optim.bin",
+            )
 
         if os.path.exists(to_ckpt_dir):
             self.model.from_checkpoint(
                 to_ckpt_dir,
                 weight_name="pytorch_model_latest.bin",
             )
             optim.from_checkpoint(
```

### Comparing `unitorch-0.0.0.4/src/unitorch/cli/writer/__init__.py` & `unitorch-0.0.0.5/src/unitorch/cli/writer/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/datasets/hf.py` & `unitorch-0.0.0.5/src/unitorch/datasets/hf.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/loss/__init__.py` & `unitorch-0.0.0.5/src/unitorch/loss/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/loss/prophetnet.py` & `unitorch-0.0.0.5/src/unitorch/loss/prophetnet.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/loss/ranking.py` & `unitorch-0.0.0.5/src/unitorch/loss/ranking.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/models/__init__.py` & `unitorch-0.0.0.5/src/unitorch/models/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -96,15 +96,15 @@
                 weight_path = [weight_path]
             for path in weight_path:
                 logging.debug(f"Loading weights from {path}")
             state_dicts += [
                 torch.load(hf_cached_path(path), map_location="cpu")
                 for path in weight_path
             ]
-        
+
         if state_dict:
             state_dicts += state_dict if isinstance(state_dict, list) else [state_dict]
 
         self_state_dict = self.state_dict()  # Get the current state_dict of the model
         load_keys = []  # Keep track of the keys loaded from the state_dict(s)
         non_load_keys = []  # Keep track of the keys not loaded from the state_dict(s)
 
@@ -207,14 +207,15 @@
 import unitorch.models.bert
 import unitorch.models.blip
 import unitorch.models.bloom
 import unitorch.models.chatglm
 import unitorch.models.clip
 import unitorch.models.deberta
 import unitorch.models.diffusers
+import unitorch.models.minigpt4
 import unitorch.models.llama
 import unitorch.models.mbart
 import unitorch.models.mt5
 import unitorch.models.pegasus
 import unitorch.models.peft
 import unitorch.models.prophetnet
 import unitorch.models.roberta
```

### Comparing `unitorch-0.0.0.4/src/unitorch/models/bart/modeling.py` & `unitorch-0.0.0.5/src/unitorch/models/bart/modeling.py`

 * *Files 2% similar despite different names*

```diff
@@ -233,15 +233,15 @@
 
     @torch.no_grad()
     def generate(
         self,
         input_ids: torch.Tensor,
         num_beams: Optional[int] = 5,
         decoder_start_token_id: Optional[int] = 2,
-        decoder_end_token_id: Optional[int] = 2,
+        decoder_end_token_id: Optional[Union[int, List[int]]] = 2,
         num_return_sequences: Optional[int] = 1,
         min_gen_seq_length: Optional[int] = 0,
         max_gen_seq_length: Optional[int] = 48,
         repetition_penalty: Optional[float] = 1.0,
         no_repeat_ngram_size: Optional[int] = 0,
         early_stopping: Optional[bool] = True,
         length_penalty: Optional[float] = 1.0,
@@ -254,16 +254,16 @@
     ):
         """
         Generates text using the BartForGeneration model.
 
         Args:
             input_ids (torch.Tensor): Tensor of input token IDs.
             num_beams (int, optional): Number of beams for beam search. Defaults to 5.
-            decoder_start_token_id (int, optional): Start token ID for the decoder. Defaults to 2.
-            decoder_end_token_id (int, optional): End token ID for the decoder. Defaults to 2.
+            decoder_start_token_id (int, optional): The ID of the decoder start token. Defaults to 2.
+            decoder_end_token_id (int or List[int], optional): The ID(s) of the decoder end token(s). Defaults to 2.
             num_return_sequences (int, optional): Number of sequences to return. Defaults to 1.
             min_gen_seq_length (int, optional): Minimum length of generated sequences. Defaults to 0.
             max_gen_seq_length (int, optional): Maximum length of generated sequences. Defaults to 48.
             repetition_penalty (float, optional): Repetition penalty for generated sequences. Defaults to 1.0.
             no_repeat_ngram_size (int, optional): Size of n-grams to avoid repetition. Defaults to 0.
             early_stopping (bool, optional): Whether to stop generation early. Defaults to True.
             length_penalty (float, optional): Length penalty for generated sequences. Defaults to 1.0.
```

### Comparing `unitorch-0.0.0.4/src/unitorch/models/bart/processing.py` & `unitorch-0.0.0.5/src/unitorch/models/bart/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/models/beit/modeling.py` & `unitorch-0.0.0.5/src/unitorch/models/beit/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/models/beit/processing.py` & `unitorch-0.0.0.5/src/unitorch/models/beit/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/models/bert/modeling.py` & `unitorch-0.0.0.5/src/unitorch/models/bert/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/models/bert/processing.py` & `unitorch-0.0.0.5/src/unitorch/models/bert/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/models/blip/modeling.py` & `unitorch-0.0.0.5/src/unitorch/models/blip/modeling.py`

 * *Files 0% similar despite different names*

```diff
@@ -703,15 +703,15 @@
     def generate(
         self,
         pixel_values: torch.Tensor,
         input_ids: Optional[torch.Tensor] = None,
         attention_mask: Optional[torch.Tensor] = None,
         num_beams: Optional[int] = 5,
         decoder_start_token_id: Optional[int] = 101,
-        decoder_end_token_id: Optional[int] = 102,
+        decoder_end_token_id: Optional[Union[int, List[int]]] = 102,
         num_return_sequences: Optional[int] = 1,
         min_gen_seq_length: Optional[int] = 0,
         max_gen_seq_length: Optional[int] = 48,
         repetition_penalty: Optional[float] = 1.0,
         no_repeat_ngram_size: Optional[int] = 0,
         early_stopping: Optional[bool] = True,
         length_penalty: Optional[float] = 1.0,
@@ -727,15 +727,15 @@
 
         Args:
             pixel_values (torch.Tensor): Input pixel values.
             input_ids (Optional[torch.Tensor], optional): Input token IDs. Defaults to None.
             attention_mask (Optional[torch.Tensor], optional): Attention mask. Defaults to None.
             num_beams (Optional[int], optional): Number of beams for beam search. Defaults to 5.
             decoder_start_token_id (Optional[int], optional): ID of the start token for decoding. Defaults to 30522.
-            decoder_end_token_id (Optional[int], optional): ID of the end token for decoding. Defaults to 2.
+            decoder_end_token_id (int or List[int], optional): ID of the end token for decoding. Defaults to 2.
             num_return_sequences (Optional[int], optional): Number of caption sequences to return. Defaults to 1.
             min_gen_seq_length (Optional[int], optional): Minimum length of generated sequences. Defaults to 0.
             max_gen_seq_length (Optional[int], optional): Maximum length of generated sequences. Defaults to 48.
             repetition_penalty (Optional[float], optional): Repetition penalty value. Defaults to 1.0.
             no_repeat_ngram_size (Optional[int], optional): Size of n-grams to avoid repetition. Defaults to 0.
             early_stopping (Optional[bool], optional): Whether to stop generation early. Defaults to True.
             length_penalty (Optional[float], optional): Length penalty value. Defaults to 1.0.
```

### Comparing `unitorch-0.0.0.4/src/unitorch/models/blip/processing.py` & `unitorch-0.0.0.5/src/unitorch/models/blip/processing.py`

 * *Files 1% similar despite different names*

```diff
@@ -197,23 +197,23 @@
             input_ids=outputs.input_ids,
             attention_mask=outputs.attention_mask,
         )
 
     def generation(
         self,
         text: str,
-        image: str,
+        image: Image.Image,
         max_gen_seq_length: Optional[int] = None,
     ) -> GenericOutputs:
         """
         Generate inputs, labels, and tokens for image to text generation.
 
         Args:
             text (str): The input text.
-            image (PIL.Image.Image): The input image to caption.
+            image (Image.Image): The input image to caption.
             max_gen_seq_length (int, optional): Maximum generated sequence length. Defaults to None.
 
         Returns:
             GenericOutputs: The generated input tokens, attention masks, label tokens, and attention masks.
         """
 
         max_gen_seq_length = pop_value(max_gen_seq_length, self.max_gen_seq_length)
```

### Comparing `unitorch-0.0.0.4/src/unitorch/models/bloom/modeling.py` & `unitorch-0.0.0.5/src/unitorch/models/bloom/modeling.py`

 * *Files 1% similar despite different names*

```diff
@@ -185,15 +185,15 @@
 
     @torch.no_grad()
     def generate(
         self,
         input_ids: torch.Tensor,
         num_beams: Optional[int] = 5,
         decoder_start_token_id: Optional[int] = 1,
-        decoder_end_token_id: Optional[int] = 2,
+        decoder_end_token_id: Optional[Union[int, List[int]]] = 2,
         num_return_sequences: Optional[int] = 1,
         min_gen_seq_length: Optional[int] = 0,
         max_gen_seq_length: Optional[int] = 48,
         repetition_penalty: Optional[float] = 1.0,
         no_repeat_ngram_size: Optional[int] = 0,
         early_stopping: Optional[bool] = True,
         length_penalty: Optional[float] = 1.0,
```

### Comparing `unitorch-0.0.0.4/src/unitorch/models/bloom/processing.py` & `unitorch-0.0.0.5/src/unitorch/models/bloom/processing.py`

 * *Files 4% similar despite different names*

```diff
@@ -230,23 +230,23 @@
             [0] * len(padding_a)
             + [1] * (len(tokens) + len(tokens_pair))
             + [0] * len(padding_b)
         )
         _tokens = padding_a + tokens + tokens_pair + padding_b
         input_ids = self.tokenizer.convert_tokens_to_ids(_tokens)
 
-        tokens_label = tokens_pair[1:max_gen_seq_length] + [self.pad_token] * (
+        tokens_label = tokens_pair + [self.pad_token] * (
             max_gen_seq_length - len(tokens_pair) + 1
         )
         input_ids_label = self.tokenizer.convert_tokens_to_ids(tokens_label)
-        input_ids_label = [0] * max_seq_length + input_ids_label
-        attention_mask_label = [1] * len(tokens_pair[1:max_gen_seq_length]) + [0] * (
+        input_ids_label = [0] * (max_seq_length - 1) + input_ids_label
+        attention_mask_label = [1] * len(tokens_pair) + [0] * (
             max_gen_seq_length - len(tokens_pair) + 1
         )
-        attention_mask_label = [0] * max_seq_length + attention_mask_label
+        attention_mask_label = [0] * (max_seq_length - 1) + attention_mask_label
 
         return GenericOutputs(
             input_ids=torch.tensor(input_ids, dtype=torch.long),
             attention_mask=torch.tensor(attention_mask, dtype=torch.long),
             input_ids_label=torch.tensor(input_ids_label, dtype=torch.long),
             attention_mask_label=torch.tensor(attention_mask_label, dtype=torch.long),
         )
```

### Comparing `unitorch-0.0.0.4/src/unitorch/models/chatglm/configuration_chatglm.py` & `unitorch-0.0.0.5/src/unitorch/models/chatglm/configuration_chatglm.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/models/chatglm/modeling.py` & `unitorch-0.0.0.5/src/unitorch/models/chatglm/modeling.py`

 * *Files 0% similar despite different names*

```diff
@@ -183,15 +183,15 @@
 
     @torch.no_grad()
     def generate(
         self,
         input_ids: torch.Tensor,
         num_beams: Optional[int] = 5,
         decoder_start_token_id: Optional[int] = 2,
-        decoder_end_token_id: Optional[int] = 2,
+        decoder_end_token_id: Optional[Union[int, List[int]]] = 2,
         num_return_sequences: Optional[int] = 1,
         min_gen_seq_length: Optional[int] = 0,
         max_gen_seq_length: Optional[int] = 48,
         repetition_penalty: Optional[float] = 1.0,
         no_repeat_ngram_size: Optional[int] = 0,
         early_stopping: Optional[bool] = True,
         length_penalty: Optional[float] = 1.0,
```

### Comparing `unitorch-0.0.0.4/src/unitorch/models/chatglm/modeling_chatglm.py` & `unitorch-0.0.0.5/src/unitorch/models/chatglm/modeling_chatglm.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/models/chatglm/processing.py` & `unitorch-0.0.0.5/src/unitorch/models/chatglm/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/models/chatglm/quantization.py` & `unitorch-0.0.0.5/src/unitorch/models/chatglm/quantization.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/models/chatglm/tokenization_chatglm.py` & `unitorch-0.0.0.5/src/unitorch/models/chatglm/tokenization_chatglm.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/models/clip/modeling.py` & `unitorch-0.0.0.5/src/unitorch/models/clip/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/models/clip/processing.py` & `unitorch-0.0.0.5/src/unitorch/models/clip/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/models/deberta/modeling.py` & `unitorch-0.0.0.5/src/unitorch/models/deberta/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/models/deberta/modeling_v2.py` & `unitorch-0.0.0.5/src/unitorch/models/deberta/modeling_v2.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/models/deberta/processing.py` & `unitorch-0.0.0.5/src/unitorch/models/deberta/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/models/deberta/processing_v2.py` & `unitorch-0.0.0.5/src/unitorch/models/deberta/processing_v2.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/models/diffusers/__init__.py` & `unitorch-0.0.0.5/src/unitorch/models/diffusers/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Copyright (c) FULIUCANSHENG.
 # Licensed under the MIT License.
 
 from unitorch import is_diffusers_available
 
 if is_diffusers_available():
-
     from unitorch.models.diffusers.modeling_controlnet import (
         ControlNetForImageGeneration,
     )
     from unitorch.models.diffusers.processing_controlnet import ControlNetProcessor
     from unitorch.models.diffusers.processing_stable import StableProcessor
     from unitorch.models.diffusers.modeling_stable import (
         StableForImageGeneration,
```

### Comparing `unitorch-0.0.0.4/src/unitorch/models/diffusers/modeling_controlnet.py` & `unitorch-0.0.0.5/src/unitorch/models/diffusers/modeling_controlnet.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/models/diffusers/modeling_stable.py` & `unitorch-0.0.0.5/src/unitorch/models/diffusers/modeling_stable.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/models/diffusers/processing_controlnet.py` & `unitorch-0.0.0.5/src/unitorch/models/diffusers/processing_controlnet.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/models/diffusers/processing_stable.py` & `unitorch-0.0.0.5/src/unitorch/models/diffusers/processing_stable.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/models/llama/modeling.py` & `unitorch-0.0.0.5/src/unitorch/models/llama/modeling.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,15 +127,15 @@
         )
         loss = torch.mean(loss)
         return loss
 
 
 class LlamaForGeneration(GenericModel):
     prefix_keys_in_state_dict = {
-        "^(?!model\.model\.)model\.": "model.",
+        "^(?!model\.model\.|model\.lm_head\.)model\.": "model.",
         "^lm_head.": "model.",
     }
 
     def __init__(
         self,
         config_path: str,
         gradient_checkpointing: Optional[bool] = False,
@@ -181,15 +181,15 @@
 
     @torch.no_grad()
     def generate(
         self,
         input_ids: torch.Tensor,
         num_beams: Optional[int] = 5,
         decoder_start_token_id: Optional[int] = 1,
-        decoder_end_token_id: Optional[int] = 2,
+        decoder_end_token_id: Optional[Union[int, List[int]]] = 2,
         num_return_sequences: Optional[int] = 1,
         min_gen_seq_length: Optional[int] = 0,
         max_gen_seq_length: Optional[int] = 48,
         repetition_penalty: Optional[float] = 1.0,
         no_repeat_ngram_size: Optional[int] = 0,
         early_stopping: Optional[bool] = True,
         length_penalty: Optional[float] = 1.0,
@@ -202,16 +202,16 @@
     ):
         """
         Generate text using the generation model.
 
         Args:
             input_ids: Input tensor of shape (batch_size, sequence_length).
             num_beams (int, optional): Number of beams for beam search. Defaults to 5.
-            decoder_start_token_id (int, optional): Start token ID for the decoder. Defaults to 2.
-            decoder_end_token_id (int, optional): End token ID for the decoder. Defaults to 2.
+            decoder_start_token_id (int, optional): The ID of the decoder start token. Defaults to 2.
+            decoder_end_token_id (int or List[int], optional): The ID(s) of the decoder end token(s). Defaults to 2.
             num_return_sequences (int, optional): Number of generated sequences to return. Defaults to 1.
             min_gen_seq_length (int, optional): Minimum length of generated sequences. Defaults to 0.
             max_gen_seq_length (int, optional): Maximum length of generated sequences. Defaults to 48.
             repetition_penalty (float, optional): Penalty for repeated tokens. Defaults to 1.0.
             no_repeat_ngram_size (int, optional): Size of n-grams to avoid repeating. Defaults to 0.
             early_stopping (bool, optional): Whether to stop generation early. Defaults to True.
             length_penalty (float, optional): Penalty for longer sequences. Defaults to 1.0.
```

### Comparing `unitorch-0.0.0.4/src/unitorch/models/llama/processing.py` & `unitorch-0.0.0.5/src/unitorch/models/llama/processing.py`

 * *Files 1% similar despite different names*

```diff
@@ -235,23 +235,23 @@
             [0] * len(padding_a)
             + [1] * (len(tokens) + len(tokens_pair))
             + [0] * len(padding_b)
         )
         _tokens = padding_a + tokens + tokens_pair + padding_b
         input_ids = self.tokenizer.convert_tokens_to_ids(_tokens)
 
-        tokens_label = tokens_pair[1:max_gen_seq_length] + [self.pad_token] * (
+        tokens_label = tokens_pair + [self.pad_token] * (
             max_gen_seq_length - len(tokens_pair) + 1
         )
         input_ids_label = self.tokenizer.convert_tokens_to_ids(tokens_label)
-        input_ids_label = [0] * max_seq_length + input_ids_label
-        attention_mask_label = [1] * len(tokens_pair[1:max_gen_seq_length]) + [0] * (
+        input_ids_label = [0] * (max_seq_length - 1) + input_ids_label
+        attention_mask_label = [1] * len(tokens_pair) + [0] * (
             max_gen_seq_length - len(tokens_pair) + 1
         )
-        attention_mask_label = [0] * max_seq_length + attention_mask_label
+        attention_mask_label = [0] * (max_seq_length - 1) + attention_mask_label
 
         return GenericOutputs(
             input_ids=torch.tensor(input_ids, dtype=torch.long),
             attention_mask=torch.tensor(attention_mask, dtype=torch.long),
             input_ids_label=torch.tensor(input_ids_label, dtype=torch.long),
             attention_mask_label=torch.tensor(attention_mask_label, dtype=torch.long),
         )
```

### Comparing `unitorch-0.0.0.4/src/unitorch/models/mbart/modeling.py` & `unitorch-0.0.0.5/src/unitorch/models/mbart/modeling.py`

 * *Files 0% similar despite different names*

```diff
@@ -177,15 +177,15 @@
         attn_output = self.out_proj(attn_output)
 
         return attn_output, attn_weights_reshaped, past_key_value
 
 
 class MBartForGeneration(GenericModel):
     prefix_keys_in_state_dict = {
-        "^(?!model\.model\.)model\.": "model.",
+        "^(?!model\.model\.|model\.lm_head\.)model\.": "model.",
         "^lm_head.": "model.",
     }
 
     def __init__(
         self,
         config_path: str,
         freeze_input_embedding: Optional[bool] = True,
@@ -241,15 +241,15 @@
 
     @torch.no_grad()
     def generate(
         self,
         input_ids: torch.Tensor,
         num_beams: Optional[int] = 5,
         decoder_start_token_id: Optional[int] = 2,
-        decoder_end_token_id: Optional[int] = 2,
+        decoder_end_token_id: Optional[Union[int, List[int]]] = 2,
         num_return_sequences: Optional[int] = 1,
         min_gen_seq_length: Optional[int] = 0,
         max_gen_seq_length: Optional[int] = 48,
         repetition_penalty: Optional[float] = 1.0,
         no_repeat_ngram_size: Optional[int] = 0,
         early_stopping: Optional[bool] = True,
         length_penalty: Optional[float] = 1.0,
@@ -263,15 +263,15 @@
         """
         Generates sequences using the MBartForGeneration model.
 
         Args:
             input_ids: The input token IDs.
             num_beams (int, optional): The number of beams for beam search. Defaults to 5.
             decoder_start_token_id (int, optional): The decoder's start token ID. Defaults to 2.
-            decoder_end_token_id (int, optional): The decoder's end token ID. Defaults to 2.
+            decoder_end_token_id (int or List[int], optional): The decoder's end token ID. Defaults to 2.
             num_return_sequences (int, optional): The number of generated sequences to return. Defaults to 1.
             min_gen_seq_length (int, optional): The minimum length of the generated sequences. Defaults to 0.
             max_gen_seq_length (int, optional): The maximum length of the generated sequences. Defaults to 48.
             repetition_penalty (float, optional): The repetition penalty. Defaults to 1.0.
             no_repeat_ngram_size (int, optional): The size of n-grams to avoid repeating. Defaults to 0.
             early_stopping (bool, optional): Whether to stop generation early. Defaults to True.
             length_penalty (float, optional): The length penalty. Defaults to 1.0.
```

### Comparing `unitorch-0.0.0.4/src/unitorch/models/mbart/processing.py` & `unitorch-0.0.0.5/src/unitorch/models/mbart/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/models/modeling_ema.py` & `unitorch-0.0.0.5/src/unitorch/models/modeling_ema.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/models/mt5/modeling.py` & `unitorch-0.0.0.5/src/unitorch/models/mt5/modeling.py`

 * *Files 1% similar despite different names*

```diff
@@ -273,15 +273,15 @@
 
     @torch.no_grad()
     def generate(
         self,
         input_ids: torch.Tensor,
         num_beams: Optional[int] = 5,
         decoder_start_token_id: Optional[int] = 0,
-        decoder_end_token_id: Optional[int] = 1,
+        decoder_end_token_id: Optional[Union[int, List[int]]] = 1,
         num_return_sequences: Optional[int] = 1,
         min_gen_seq_length: Optional[int] = 0,
         max_gen_seq_length: Optional[int] = 48,
         repetition_penalty: Optional[float] = 1.0,
         no_repeat_ngram_size: Optional[int] = 0,
         early_stopping: Optional[bool] = True,
         length_penalty: Optional[float] = 1.0,
@@ -295,15 +295,15 @@
         """
         Generates sequences using the MT5ForGeneration model.
 
         Args:
             input_ids: The input token IDs.
             num_beams (int, optional): The number of beams for beam search. Defaults to 5.
             decoder_start_token_id (int, optional): The decoder's start token ID. Defaults to 2.
-            decoder_end_token_id (int, optional): The decoder's end token ID. Defaults to 2.
+            decoder_end_token_id (int or List[int], optional): The decoder's end token ID. Defaults to 2.
             num_return_sequences (int, optional): The number of generated sequences to return. Defaults to 1.
             min_gen_seq_length (int, optional): The minimum length of the generated sequences. Defaults to 0.
             max_gen_seq_length (int, optional): The maximum length of the generated sequences. Defaults to 48.
             repetition_penalty (float, optional): The repetition penalty. Defaults to 1.0.
             no_repeat_ngram_size (int, optional): The size of n-grams to avoid repeating. Defaults to 0.
             early_stopping (bool, optional): Whether to stop generation early. Defaults to True.
             length_penalty (float, optional): The length penalty. Defaults to 1.0.
```

### Comparing `unitorch-0.0.0.4/src/unitorch/models/mt5/processing.py` & `unitorch-0.0.0.5/src/unitorch/models/mt5/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/models/peft/__init__.py` & `unitorch-0.0.0.5/src/unitorch/models/peft/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/models/peft/modeling_bloom_adalora.py` & `unitorch-0.0.0.5/src/unitorch/models/peft/modeling_bloom_adalora.py`

 * *Files 2% similar despite different names*

```diff
@@ -159,15 +159,15 @@
 
     @torch.no_grad()
     def generate(
         self,
         input_ids: torch.Tensor,
         num_beams: Optional[int] = 5,
         decoder_start_token_id: Optional[int] = 1,
-        decoder_end_token_id: Optional[int] = 2,
+        decoder_end_token_id: Optional[Union[int, List[int]]] = 2,
         num_return_sequences: Optional[int] = 1,
         min_gen_seq_length: Optional[int] = 0,
         max_gen_seq_length: Optional[int] = 48,
         repetition_penalty: Optional[float] = 1.0,
         no_repeat_ngram_size: Optional[int] = 0,
         early_stopping: Optional[bool] = True,
         length_penalty: Optional[float] = 1.0,
@@ -180,16 +180,16 @@
     ):
         """
         Generate text using the generation model.
 
         Args:
             input_ids: Input tensor of shape (batch_size, sequence_length).
             num_beams (int, optional): Number of beams for beam search. Defaults to 5.
-            decoder_start_token_id (int, optional): Start token ID for the decoder. Defaults to 2.
-            decoder_end_token_id (int, optional): End token ID for the decoder. Defaults to 2.
+            decoder_start_token_id (int, optional): The ID of the decoder start token. Defaults to 2.
+            decoder_end_token_id (int or List[int], optional): The ID(s) of the decoder end token(s). Defaults to 2.
             num_return_sequences (int, optional): Number of generated sequences to return. Defaults to 1.
             min_gen_seq_length (int, optional): Minimum length of generated sequences. Defaults to 0.
             max_gen_seq_length (int, optional): Maximum length of generated sequences. Defaults to 48.
             repetition_penalty (float, optional): Penalty for repeated tokens. Defaults to 1.0.
             no_repeat_ngram_size (int, optional): Size of n-grams to avoid repeating. Defaults to 0.
             early_stopping (bool, optional): Whether to stop generation early. Defaults to True.
             length_penalty (float, optional): Penalty for longer sequences. Defaults to 1.0.
```

### Comparing `unitorch-0.0.0.4/src/unitorch/models/peft/modeling_bloom_lora.py` & `unitorch-0.0.0.5/src/unitorch/models/peft/modeling_bloom_lora.py`

 * *Files 2% similar despite different names*

```diff
@@ -138,15 +138,15 @@
 
     @torch.no_grad()
     def generate(
         self,
         input_ids: torch.Tensor,
         num_beams: Optional[int] = 5,
         decoder_start_token_id: Optional[int] = 1,
-        decoder_end_token_id: Optional[int] = 2,
+        decoder_end_token_id: Optional[Union[int, List[int]]] = 2,
         num_return_sequences: Optional[int] = 1,
         min_gen_seq_length: Optional[int] = 0,
         max_gen_seq_length: Optional[int] = 48,
         repetition_penalty: Optional[float] = 1.0,
         no_repeat_ngram_size: Optional[int] = 0,
         early_stopping: Optional[bool] = True,
         length_penalty: Optional[float] = 1.0,
@@ -159,16 +159,16 @@
     ):
         """
         Generate text using the generation model.
 
         Args:
             input_ids: Input tensor of shape (batch_size, sequence_length).
             num_beams (int, optional): Number of beams for beam search. Defaults to 5.
-            decoder_start_token_id (int, optional): Start token ID for the decoder. Defaults to 2.
-            decoder_end_token_id (int, optional): End token ID for the decoder. Defaults to 2.
+            decoder_start_token_id (int, optional): The ID of the decoder start token. Defaults to 2.
+            decoder_end_token_id (int or List[int], optional): The ID(s) of the decoder end token(s). Defaults to 2.
             num_return_sequences (int, optional): Number of generated sequences to return. Defaults to 1.
             min_gen_seq_length (int, optional): Minimum length of generated sequences. Defaults to 0.
             max_gen_seq_length (int, optional): Maximum length of generated sequences. Defaults to 48.
             repetition_penalty (float, optional): Penalty for repeated tokens. Defaults to 1.0.
             no_repeat_ngram_size (int, optional): Size of n-grams to avoid repeating. Defaults to 0.
             early_stopping (bool, optional): Whether to stop generation early. Defaults to True.
             length_penalty (float, optional): Penalty for longer sequences. Defaults to 1.0.
```

### Comparing `unitorch-0.0.0.4/src/unitorch/models/peft/modeling_llama_adalora.py` & `unitorch-0.0.0.5/src/unitorch/models/peft/modeling_llama_adalora.py`

 * *Files 2% similar despite different names*

```diff
@@ -159,15 +159,15 @@
 
     @torch.no_grad()
     def generate(
         self,
         input_ids: torch.Tensor,
         num_beams: Optional[int] = 5,
         decoder_start_token_id: Optional[int] = 1,
-        decoder_end_token_id: Optional[int] = 2,
+        decoder_end_token_id: Optional[Union[int, List[int]]] = 2,
         num_return_sequences: Optional[int] = 1,
         min_gen_seq_length: Optional[int] = 0,
         max_gen_seq_length: Optional[int] = 48,
         repetition_penalty: Optional[float] = 1.0,
         no_repeat_ngram_size: Optional[int] = 0,
         early_stopping: Optional[bool] = True,
         length_penalty: Optional[float] = 1.0,
@@ -180,16 +180,16 @@
     ):
         """
         Generate text using the generation model.
 
         Args:
             input_ids: Input tensor of shape (batch_size, sequence_length).
             num_beams (int, optional): Number of beams for beam search. Defaults to 5.
-            decoder_start_token_id (int, optional): Start token ID for the decoder. Defaults to 2.
-            decoder_end_token_id (int, optional): End token ID for the decoder. Defaults to 2.
+            decoder_start_token_id (int, optional): The ID of the decoder start token. Defaults to 2.
+            decoder_end_token_id (int or List[int], optional): The ID(s) of the decoder end token(s). Defaults to 2.
             num_return_sequences (int, optional): Number of generated sequences to return. Defaults to 1.
             min_gen_seq_length (int, optional): Minimum length of generated sequences. Defaults to 0.
             max_gen_seq_length (int, optional): Maximum length of generated sequences. Defaults to 48.
             repetition_penalty (float, optional): Penalty for repeated tokens. Defaults to 1.0.
             no_repeat_ngram_size (int, optional): Size of n-grams to avoid repeating. Defaults to 0.
             early_stopping (bool, optional): Whether to stop generation early. Defaults to True.
             length_penalty (float, optional): Penalty for longer sequences. Defaults to 1.0.
```

### Comparing `unitorch-0.0.0.4/src/unitorch/models/peft/modeling_llama_lora.py` & `unitorch-0.0.0.5/src/unitorch/models/peft/modeling_llama_lora.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,15 +132,15 @@
 
     @torch.no_grad()
     def generate(
         self,
         input_ids: torch.Tensor,
         num_beams: Optional[int] = 5,
         decoder_start_token_id: Optional[int] = 1,
-        decoder_end_token_id: Optional[int] = 2,
+        decoder_end_token_id: Optional[Union[int, List[int]]] = 2,
         num_return_sequences: Optional[int] = 1,
         min_gen_seq_length: Optional[int] = 0,
         max_gen_seq_length: Optional[int] = 48,
         repetition_penalty: Optional[float] = 1.0,
         no_repeat_ngram_size: Optional[int] = 0,
         early_stopping: Optional[bool] = True,
         length_penalty: Optional[float] = 1.0,
@@ -153,16 +153,16 @@
     ):
         """
         Generate text using the generation model.
 
         Args:
             input_ids: Input tensor of shape (batch_size, sequence_length).
             num_beams (int, optional): Number of beams for beam search. Defaults to 5.
-            decoder_start_token_id (int, optional): Start token ID for the decoder. Defaults to 2.
-            decoder_end_token_id (int, optional): End token ID for the decoder. Defaults to 2.
+            decoder_start_token_id (int, optional): The ID of the decoder start token. Defaults to 2.
+            decoder_end_token_id (int or List[int], optional): The ID(s) of the decoder end token(s). Defaults to 2.
             num_return_sequences (int, optional): Number of generated sequences to return. Defaults to 1.
             min_gen_seq_length (int, optional): Minimum length of generated sequences. Defaults to 0.
             max_gen_seq_length (int, optional): Maximum length of generated sequences. Defaults to 48.
             repetition_penalty (float, optional): Penalty for repeated tokens. Defaults to 1.0.
             no_repeat_ngram_size (int, optional): Size of n-grams to avoid repeating. Defaults to 0.
             early_stopping (bool, optional): Whether to stop generation early. Defaults to True.
             length_penalty (float, optional): Penalty for longer sequences. Defaults to 1.0.
```

### Comparing `unitorch-0.0.0.4/src/unitorch/models/pegasus/modeling.py` & `unitorch-0.0.0.5/src/unitorch/models/pegasus/modeling.py`

 * *Files 1% similar despite different names*

```diff
@@ -178,15 +178,15 @@
         attn_output = self.out_proj(attn_output)
 
         return attn_output, attn_weights_reshaped, past_key_value
 
 
 class PegasusForGeneration(GenericModel):
     prefix_keys_in_state_dict = {
-        "^(?!model\.model\.)model\.": "model.",
+        "^(?!model\.model\.|model\.lm_head\.)model\.": "model.",
         "^lm_head.": "model.",
     }
 
     def __init__(
         self,
         config_path: str,
         gradient_checkpointing: Optional[bool] = False,
@@ -236,15 +236,15 @@
 
     @torch.no_grad()
     def generate(
         self,
         input_ids: torch.Tensor,
         num_beams: Optional[int] = 5,
         decoder_start_token_id: Optional[int] = 0,
-        decoder_end_token_id: Optional[int] = 1,
+        decoder_end_token_id: Optional[Union[int, List[int]]] = 1,
         num_return_sequences: Optional[int] = 1,
         min_gen_seq_length: Optional[int] = 0,
         max_gen_seq_length: Optional[int] = 48,
         repetition_penalty: Optional[float] = 1.0,
         no_repeat_ngram_size: Optional[int] = 0,
         early_stopping: Optional[bool] = True,
         length_penalty: Optional[float] = 1.0,
@@ -258,15 +258,15 @@
         """
         Generates sequences using the PegasusForGeneration model.
 
         Args:
             input_ids: The input token IDs.
             num_beams (int, optional): The number of beams for beam search. Defaults to 5.
             decoder_start_token_id (int, optional): The decoder's start token ID. Defaults to 2.
-            decoder_end_token_id (int, optional): The decoder's end token ID. Defaults to 2.
+            decoder_end_token_id (int or List[int], optional): The decoder's end token ID. Defaults to 2.
             num_return_sequences (int, optional): The number of generated sequences to return. Defaults to 1.
             min_gen_seq_length (int, optional): The minimum length of the generated sequences. Defaults to 0.
             max_gen_seq_length (int, optional): The maximum length of the generated sequences. Defaults to 48.
             repetition_penalty (float, optional): The repetition penalty. Defaults to 1.0.
             no_repeat_ngram_size (int, optional): The size of n-grams to avoid repeating. Defaults to 0.
             early_stopping (bool, optional): Whether to stop generation early. Defaults to True.
             length_penalty (float, optional): The length penalty. Defaults to 1.0.
```

### Comparing `unitorch-0.0.0.4/src/unitorch/models/pegasus/processing.py` & `unitorch-0.0.0.5/src/unitorch/models/pegasus/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/models/processing_utils.py` & `unitorch-0.0.0.5/src/unitorch/models/processing_utils.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/models/prophetnet/modeling.py` & `unitorch-0.0.0.5/src/unitorch/models/prophetnet/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/models/prophetnet/processing.py` & `unitorch-0.0.0.5/src/unitorch/models/prophetnet/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/models/roberta/modeling.py` & `unitorch-0.0.0.5/src/unitorch/models/roberta/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/models/roberta/processing.py` & `unitorch-0.0.0.5/src/unitorch/models/roberta/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/models/swin/modeling.py` & `unitorch-0.0.0.5/src/unitorch/models/swin/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/models/swin/processing.py` & `unitorch-0.0.0.5/src/unitorch/models/swin/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/models/t5/modeling.py` & `unitorch-0.0.0.5/src/unitorch/models/t5/modeling.py`

 * *Files 1% similar despite different names*

```diff
@@ -252,15 +252,15 @@
 
     @torch.no_grad()
     def generate(
         self,
         input_ids: torch.Tensor,
         num_beams: Optional[int] = 5,
         decoder_start_token_id: Optional[int] = 0,
-        decoder_end_token_id: Optional[int] = 1,
+        decoder_end_token_id: Optional[Union[int, List[int]]] = 1,
         num_return_sequences: Optional[int] = 1,
         min_gen_seq_length: Optional[int] = 0,
         max_gen_seq_length: Optional[int] = 48,
         repetition_penalty: Optional[float] = 1.0,
         no_repeat_ngram_size: Optional[int] = 0,
         early_stopping: Optional[bool] = True,
         length_penalty: Optional[float] = 1.0,
@@ -274,15 +274,15 @@
         """
         Generates sequences using the T5ForGeneration model.
 
         Args:
             input_ids: The input token IDs.
             num_beams (int, optional): The number of beams for beam search. Defaults to 5.
             decoder_start_token_id (int, optional): The decoder's start token ID. Defaults to 2.
-            decoder_end_token_id (int, optional): The decoder's end token ID. Defaults to 2.
+            decoder_end_token_id (int or List[int], optional): The decoder's end token ID. Defaults to 2.
             num_return_sequences (int, optional): The number of generated sequences to return. Defaults to 1.
             min_gen_seq_length (int, optional): The minimum length of the generated sequences. Defaults to 0.
             max_gen_seq_length (int, optional): The maximum length of the generated sequences. Defaults to 48.
             repetition_penalty (float, optional): The repetition penalty. Defaults to 1.0.
             no_repeat_ngram_size (int, optional): The size of n-grams to avoid repeating. Defaults to 0.
             early_stopping (bool, optional): Whether to stop generation early. Defaults to True.
             length_penalty (float, optional): The length penalty. Defaults to 1.0.
```

### Comparing `unitorch-0.0.0.4/src/unitorch/models/t5/processing.py` & `unitorch-0.0.0.5/src/unitorch/models/t5/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/models/visualbert/modeling.py` & `unitorch-0.0.0.5/src/unitorch/models/visualbert/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/models/visualbert/processing.py` & `unitorch-0.0.0.5/src/unitorch/models/visualbert/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/models/vit/modeling.py` & `unitorch-0.0.0.5/src/unitorch/models/vit/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/models/vit/processing.py` & `unitorch-0.0.0.5/src/unitorch/models/vit/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/models/xlm_roberta/modeling.py` & `unitorch-0.0.0.5/src/unitorch/models/xlm_roberta/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/models/xlm_roberta/processing.py` & `unitorch-0.0.0.5/src/unitorch/models/xlm_roberta/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/models/xpegasus/modeling.py` & `unitorch-0.0.0.5/src/unitorch/models/xpegasus/modeling.py`

 * *Files 2% similar despite different names*

```diff
@@ -241,15 +241,15 @@
 
     @torch.no_grad()
     def generate(
         self,
         input_ids: torch.Tensor,
         num_beams: Optional[int] = 5,
         decoder_start_token_id: Optional[int] = 0,
-        decoder_end_token_id: Optional[int] = 1,
+        decoder_end_token_id: Optional[Union[int, List[int]]] = 1,
         num_return_sequences: Optional[int] = 1,
         min_gen_seq_length: Optional[int] = 0,
         max_gen_seq_length: Optional[int] = 48,
         repetition_penalty: Optional[float] = 1.0,
         no_repeat_ngram_size: Optional[int] = 0,
         early_stopping: Optional[bool] = True,
         length_penalty: Optional[float] = 1.0,
@@ -263,15 +263,15 @@
         """
         Generates sequences using the XPegasusForGeneration model.
 
         Args:
             input_ids: The input token IDs.
             num_beams (int, optional): The number of beams for beam search. Defaults to 5.
             decoder_start_token_id (int, optional): The decoder's start token ID. Defaults to 2.
-            decoder_end_token_id (int, optional): The decoder's end token ID. Defaults to 2.
+            decoder_end_token_id (int or List[int], optional): The decoder's end token ID. Defaults to 2.
             num_return_sequences (int, optional): The number of generated sequences to return. Defaults to 1.
             min_gen_seq_length (int, optional): The minimum length of the generated sequences. Defaults to 0.
             max_gen_seq_length (int, optional): The maximum length of the generated sequences. Defaults to 48.
             repetition_penalty (float, optional): The repetition penalty. Defaults to 1.0.
             no_repeat_ngram_size (int, optional): The size of n-grams to avoid repeating. Defaults to 0.
             early_stopping (bool, optional): Whether to stop generation early. Defaults to True.
             length_penalty (float, optional): The length penalty. Defaults to 1.0.
```

### Comparing `unitorch-0.0.0.4/src/unitorch/models/xpegasus/processing.py` & `unitorch-0.0.0.5/src/unitorch/models/xpegasus/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/models/xprophetnet/modeling.py` & `unitorch-0.0.0.5/src/unitorch/models/xprophetnet/modeling.py`

 * *Files 0% similar despite different names*

```diff
@@ -235,15 +235,15 @@
 
     @torch.no_grad()
     def generate(
         self,
         input_ids: torch.Tensor,
         num_beams: Optional[int] = 5,
         decoder_start_token_id: Optional[int] = 2,
-        decoder_end_token_id: Optional[int] = 2,
+        decoder_end_token_id: Optional[Union[int, List[int]]] = 2,
         num_return_sequences: Optional[int] = 1,
         min_gen_seq_length: Optional[int] = 0,
         max_gen_seq_length: Optional[int] = 48,
         repetition_penalty: Optional[float] = 1.0,
         no_repeat_ngram_size: Optional[int] = 0,
         early_stopping: Optional[bool] = True,
         length_penalty: Optional[float] = 1.0,
@@ -257,15 +257,15 @@
         """
         Generates sequences using the XPegasusForGeneration model.
 
         Args:
             input_ids: The input token IDs.
             num_beams (int, optional): The number of beams for beam search. Defaults to 5.
             decoder_start_token_id (int, optional): The decoder's start token ID. Defaults to 2.
-            decoder_end_token_id (int, optional): The decoder's end token ID. Defaults to 2.
+            decoder_end_token_id (int or List[int], optional): The decoder's end token ID. Defaults to 2.
             num_return_sequences (int, optional): The number of generated sequences to return. Defaults to 1.
             min_gen_seq_length (int, optional): The minimum length of the generated sequences. Defaults to 0.
             max_gen_seq_length (int, optional): The maximum length of the generated sequences. Defaults to 48.
             repetition_penalty (float, optional): The repetition penalty. Defaults to 1.0.
             no_repeat_ngram_size (int, optional): The size of n-grams to avoid repeating. Defaults to 0.
             early_stopping (bool, optional): Whether to stop generation early. Defaults to True.
             length_penalty (float, optional): The length penalty. Defaults to 1.0.
```

### Comparing `unitorch-0.0.0.4/src/unitorch/models/xprophetnet/processing.py` & `unitorch-0.0.0.5/src/unitorch/models/xprophetnet/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/modules/classifier.py` & `unitorch-0.0.0.5/src/unitorch/modules/classifier.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/modules/replace/beam_search_v2.py` & `unitorch-0.0.0.5/src/unitorch/modules/replace/beam_search_v2.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/modules/replace/datasets_v2.py` & `unitorch-0.0.0.5/src/unitorch/modules/replace/datasets_v2.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/modules/replace/hf_hub_v2.py` & `unitorch-0.0.0.5/src/unitorch/modules/replace/hf_hub_v2.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/modules/timm.py` & `unitorch-0.0.0.5/src/unitorch/modules/timm.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/ops/dyhead.py` & `unitorch-0.0.0.5/src/unitorch/ops/dyhead.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/ops/ngram_repeat_block.py` & `unitorch-0.0.0.5/src/unitorch/ops/ngram_repeat_block.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/optim/lion.py` & `unitorch-0.0.0.5/src/unitorch/optim/lion.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/scheduler/warmup.py` & `unitorch-0.0.0.5/src/unitorch/scheduler/warmup.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/score/__init__.py` & `unitorch-0.0.0.5/src/unitorch/score/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/score/bleu.py` & `unitorch-0.0.0.5/src/unitorch/score/bleu.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/score/map.py` & `unitorch-0.0.0.5/src/unitorch/score/map.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/score/rouge.py` & `unitorch-0.0.0.5/src/unitorch/score/rouge.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/utils/__init__.py` & `unitorch-0.0.0.5/src/unitorch/utils/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,14 +35,15 @@
     nested_dict_value,
 )
 from unitorch.utils.image_utils import make_grid
 from unitorch.utils.import_utils import (
     is_deepspeed_available,
     is_accelerate_available,
     is_megatron_available,
+    is_fastapi_available,
     is_diffusers_available,
     is_torch_available,
     is_torch2_available,
 )
 from unitorch.utils.io import GenericWriter, IOProcess, PostProcess, GENERATE_FINISHED
 from unitorch.utils.torch_utils import get_local_rank
 from unitorch.utils.torch_utils import (
```

### Comparing `unitorch-0.0.0.4/src/unitorch/utils/decorators.py` & `unitorch-0.0.0.5/src/unitorch/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/utils/functional.py` & `unitorch-0.0.0.5/src/unitorch/utils/functional.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/utils/image_utils.py` & `unitorch-0.0.0.5/src/unitorch/utils/image_utils.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/utils/import_utils.py` & `unitorch-0.0.0.5/src/unitorch/utils/import_utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -43,14 +43,27 @@
     _megatron_available = False
 
 
 def is_megatron_available():
     return _megatron_available or is_offline_debug_mode()
 
 
+# fastapi
+_fastapi_available = importlib.util.find_spec("fastapi") is not None
+try:
+    _fastapi_version = importlib_metadata.version("fastapi")
+    logging.debug(f"Successfully imported fastapi version {_fastapi_version}")
+except importlib_metadata.PackageNotFoundError:
+    _fastapi_available = False
+
+
+def is_fastapi_available():
+    return _fastapi_available or is_offline_debug_mode()
+
+
 # diffusers
 _diffusers_available = importlib.util.find_spec("diffusers") is not None
 try:
     _diffusers_version = importlib_metadata.version("diffusers")
     logging.debug(f"Successfully imported diffusers version {_diffusers_version}")
 except importlib_metadata.PackageNotFoundError:
     _diffusers_available = False
```

### Comparing `unitorch-0.0.0.4/src/unitorch/utils/io.py` & `unitorch-0.0.0.5/src/unitorch/utils/io.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/utils/palette.py` & `unitorch-0.0.0.5/src/unitorch/utils/palette.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch/utils/torch_utils.py` & `unitorch-0.0.0.5/src/unitorch/utils/torch_utils.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/src/unitorch.egg-info/PKG-INFO` & `unitorch-0.0.0.5/src/unitorch.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unitorch
-Version: 0.0.0.4
+Version: 0.0.0.5
 Summary: unitorch provides efficient implementation of popular unified NLU / NLG / CV / CTR / MM / RL models with PyTorch.
 Author-email: fuliucansheng <fuliucansheng@gmail.com>
 License: MIT
 Keywords: PyTorch
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
@@ -18,14 +18,15 @@
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: deepspeed
 Provides-Extra: diffusers
 Provides-Extra: accelerate
 Provides-Extra: chatglm
+Provides-Extra: fastapi
 Provides-Extra: all
 License-File: LICENSE
 
 <div align="Center"> 
 
 ![unitorch](unitorch.png)
 
@@ -48,14 +49,15 @@
  
 🔥 unitorch is a library that simplifies and accelerates the development of unified models for natural language understanding, natural language generation, computer vision, click-through rate prediction, multimodal learning and reinforcement learning. It is built on top of PyTorch and integrates seamlessly with popular frameworks such as transformers, peft, diffusers, and fastseq. With unitorch, you can use a single command line tool or a one-line code ` import unitorch` import to leverage the state-of-the-art models and datasets without sacrificing performance or accuracy.
 
 ------------------------------------
 
 # What's New Model
 
+* **MiniGPT-4** released with the paper [MiniGPT-4: Enhancing Vision-Language Understanding with Advanced Large Language Models](https://arxiv.org/abs/2304.10592) by Deyao Zhu, Jun Chen, Xiaoqian Shen, Xiang Li, Mohamed Elhoseiny.
 * **LLaMA** released with the paper [LLaMA: Open and Efficient Foundation Language Models](https://arxiv.org/abs/2302.13971) by Hugo Touvron, Thibaut Lavril, Gautier Izacard, Xavier Martinet, Marie-Anne Lachaux, Timothée Lacroix, Baptiste Rozière, Naman Goyal, Eric Hambro, Faisal Azhar, Aurelien Rodriguez, Armand Joulin, Edouard Grave, Guillaume Lample.
 * **BLOOM** released with the paper [BLOOM: A 176B-Parameter Open-Access Multilingual Language Model](https://arxiv.org/abs/2211.05100) by BigScience Workshop: Teven Le Scao, Angela Fan, Christopher Akiki, Ellie Pavlick, Suzana Ilić, Daniel Hesslow...
 * **PEGASUS-X** released with the paper [Investigating Efficiently Extending Transformers for Long Input Summarization](https://arxiv.org/abs/2208.04347) by Jason Phang, Yao Zhao, Peter J. Liu.
 * **BLIP** released with the paper [BLIP: Bootstrapping Language-Image Pre-training for Unified Vision-Language Understanding and Generation](https://arxiv.org/abs/2201.12086) by Junnan Li, Dongxu Li, Caiming Xiong, Steven Hoi.
 * **BEiT** released with the paper [BEiT: BERT Pre-Training of Image Transformers](https://arxiv.org/abs/2106.08254) by Hangbo Bao, Li Dong, Songhao Piao, Furu Wei.
 * **Swin Transformer** released with the paper [Swin Transformer: Hierarchical Vision Transformer using Shifted Windows](https://arxiv.org/abs/2103.14030) by Ze Liu, Yutong Lin, Yue Cao, Han Hu, Yixuan Wei, Zheng Zhang, Stephen Lin, Baining Guo.
 * **CLIP** released with the paper [Learning Transferable Visual Models From Natural Language Supervision](https://arxiv.org/abs/2103.00020) by Alec Radford, Jong Wook Kim, Chris Hallacy, Aditya Ramesh, Gabriel Goh, Sandhini Agarwal, Girish Sastry, Amanda Askell, Pamela Mishkin, Jack Clark, Gretchen Krueger, Ilya Sutskever.
```

### Comparing `unitorch-0.0.0.4/src/unitorch.egg-info/SOURCES.txt` & `unitorch-0.0.0.5/src/unitorch.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,27 @@
 setup.cfg
 setup.py
 .pytest_cache/README.md
 benchmarks/README.md
 docs/search/search_index.json
 examples/README.md
 examples/configs/caption/blip.ini
+examples/configs/caption/minigpt4.ini
+examples/configs/caption/minigpt4_ds.ini
 examples/configs/classification/bert.ini
 examples/configs/classification/clip.ini
 examples/configs/classification/image_clip.ini
 examples/configs/classification/roberta.ini
 examples/configs/classification/swin.ini
 examples/configs/classification/text_clip.ini
 examples/configs/classification/lora/bloom.ini
 examples/configs/classification/lora/bloom_ds.ini
 examples/configs/classification/lora/llama.ini
 examples/configs/classification/lora/llama_ds.ini
+examples/configs/deepspeed/adamw.json
 examples/configs/diffusion/stable-v1.5.ini
 examples/configs/diffusion/stable-v2.1.ini
 examples/configs/diffusion/stable-v2.ini
 examples/configs/diffusion/controlnet/canny.ini
 examples/configs/generation/bart.ini
 examples/configs/generation/bloom.ini
 examples/configs/generation/chatglm.ini
@@ -56,14 +59,15 @@
 src/unitorch.egg-info/requires.txt
 src/unitorch.egg-info/top_level.txt
 src/unitorch/cli/__init__.py
 src/unitorch/cli/core.py
 src/unitorch/cli/decorators.py
 src/unitorch/cli/console/__init__.py
 src/unitorch/cli/console/eval.py
+src/unitorch/cli/console/fastapi.py
 src/unitorch/cli/console/infer.py
 src/unitorch/cli/console/script.py
 src/unitorch/cli/console/service.py
 src/unitorch/cli/console/train.py
 src/unitorch/cli/datasets/__init__.py
 src/unitorch/cli/datasets/hf.py
 src/unitorch/cli/loss/__init__.py
@@ -77,14 +81,15 @@
 src/unitorch/cli/models/label_utils.py
 src/unitorch/cli/models/modeling_utils.py
 src/unitorch/cli/models/processing_utils.py
 src/unitorch/cli/models/random_utils.py
 src/unitorch/cli/models/ranking_utils.py
 src/unitorch/cli/models/segmentation_utils.py
 src/unitorch/cli/models/bart/__init__.py
+src/unitorch/cli/models/bart/fastapi.py
 src/unitorch/cli/models/bart/modeling.py
 src/unitorch/cli/models/bart/processing.py
 src/unitorch/cli/models/beit/__init__.py
 src/unitorch/cli/models/beit/modeling.py
 src/unitorch/cli/models/beit/processing.py
 src/unitorch/cli/models/bert/__init__.py
 src/unitorch/cli/models/bert/modeling.py
@@ -113,14 +118,17 @@
 src/unitorch/cli/models/diffusers/processing_stable.py
 src/unitorch/cli/models/llama/__init__.py
 src/unitorch/cli/models/llama/modeling.py
 src/unitorch/cli/models/llama/processing.py
 src/unitorch/cli/models/mbart/__init__.py
 src/unitorch/cli/models/mbart/modeling.py
 src/unitorch/cli/models/mbart/processing.py
+src/unitorch/cli/models/minigpt4/__init__.py
+src/unitorch/cli/models/minigpt4/modeling.py
+src/unitorch/cli/models/minigpt4/processing.py
 src/unitorch/cli/models/mt5/__init__.py
 src/unitorch/cli/models/mt5/modeling.py
 src/unitorch/cli/models/mt5/processing.py
 src/unitorch/cli/models/peft/__init__.py
 src/unitorch/cli/models/peft/modeling_bloom.py
 src/unitorch/cli/models/peft/modeling_llama.py
 src/unitorch/cli/models/pegasus/__init__.py
@@ -186,14 +194,17 @@
 src/unitorch/models/beit/processing.py
 src/unitorch/models/bert/__init__.py
 src/unitorch/models/bert/modeling.py
 src/unitorch/models/bert/processing.py
 src/unitorch/models/blip/__init__.py
 src/unitorch/models/blip/modeling.py
 src/unitorch/models/blip/processing.py
+src/unitorch/models/blip2/__init__.py
+src/unitorch/models/blip2/modeling.py
+src/unitorch/models/blip2/processing.py
 src/unitorch/models/bloom/__init__.py
 src/unitorch/models/bloom/modeling.py
 src/unitorch/models/bloom/processing.py
 src/unitorch/models/chatglm/__init__.py
 src/unitorch/models/chatglm/configuration_chatglm.py
 src/unitorch/models/chatglm/modeling.py
 src/unitorch/models/chatglm/modeling_chatglm.py
@@ -215,14 +226,17 @@
 src/unitorch/models/diffusers/processing_stable.py
 src/unitorch/models/llama/__init__.py
 src/unitorch/models/llama/modeling.py
 src/unitorch/models/llama/processing.py
 src/unitorch/models/mbart/__init__.py
 src/unitorch/models/mbart/modeling.py
 src/unitorch/models/mbart/processing.py
+src/unitorch/models/minigpt4/__init__.py
+src/unitorch/models/minigpt4/modeling.py
+src/unitorch/models/minigpt4/processing.py
 src/unitorch/models/mt5/__init__.py
 src/unitorch/models/mt5/modeling.py
 src/unitorch/models/mt5/processing.py
 src/unitorch/models/peft/__init__.py
 src/unitorch/models/peft/modeling_bloom_adalora.py
 src/unitorch/models/peft/modeling_bloom_lora.py
 src/unitorch/models/peft/modeling_llama_adalora.py
@@ -309,14 +323,15 @@
 wiki/cli/models/chatglm.md
 wiki/cli/models/clip.md
 wiki/cli/models/deberta.md
 wiki/cli/models/diffusers.md
 wiki/cli/models/index.md
 wiki/cli/models/llama.md
 wiki/cli/models/mbart.md
+wiki/cli/models/minigpt4.md
 wiki/cli/models/mt5.md
 wiki/cli/models/peft.md
 wiki/cli/models/pegasus.md
 wiki/cli/models/prophetnet.md
 wiki/cli/models/roberta.md
 wiki/cli/models/swin.md
 wiki/cli/models/t5.md
@@ -341,14 +356,15 @@
 wiki/models/chatglm.md
 wiki/models/clip.md
 wiki/models/deberta.md
 wiki/models/diffusers.md
 wiki/models/index.md
 wiki/models/llama.md
 wiki/models/mbart.md
+wiki/models/minigpt4.md
 wiki/models/mt5.md
 wiki/models/peft.md
 wiki/models/pegasus.md
 wiki/models/prophetnet.md
 wiki/models/roberta.md
 wiki/models/swin.md
 wiki/models/t5.md
```

### Comparing `unitorch-0.0.0.4/wiki/cli/models/blip.md` & `unitorch-0.0.0.5/wiki/cli/models/blip.md`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/wiki/cli/models/bloom.md` & `unitorch-0.0.0.5/wiki/cli/models/bloom.md`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/wiki/cli/models/chatglm.md` & `unitorch-0.0.0.5/wiki/cli/models/chatglm.md`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/wiki/cli/models/clip.md` & `unitorch-0.0.0.5/wiki/cli/models/clip.md`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/wiki/cli/models/deberta.md` & `unitorch-0.0.0.5/wiki/cli/models/deberta.md`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/wiki/cli/models/llama.md` & `unitorch-0.0.0.5/wiki/cli/models/llama.md`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/wiki/cli/models/peft.md` & `unitorch-0.0.0.5/wiki/cli/models/peft.md`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/wiki/cli/models/visualbert.md` & `unitorch-0.0.0.5/wiki/cli/models/visualbert.md`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/wiki/cli/models/xlm_roberta.md` & `unitorch-0.0.0.5/wiki/cli/models/xlm_roberta.md`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/wiki/cli/postprocess.md` & `unitorch-0.0.0.5/wiki/cli/postprocess.md`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/wiki/configuration.md` & `unitorch-0.0.0.5/wiki/configuration.md`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/wiki/examples/caption/blip.md` & `unitorch-0.0.0.5/wiki/examples/caption/blip.md`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/wiki/examples/classification/clip.md` & `unitorch-0.0.0.5/wiki/examples/classification/clip.md`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/wiki/examples/classification/roberta.md` & `unitorch-0.0.0.5/wiki/examples/classification/roberta.md`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/wiki/examples/classification/swin.md` & `unitorch-0.0.0.5/wiki/examples/classification/swin.md`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/wiki/examples/generation/bart.md` & `unitorch-0.0.0.5/wiki/examples/generation/bart.md`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/wiki/examples/service/zip_image.md` & `unitorch-0.0.0.5/wiki/examples/service/zip_image.md`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/wiki/index.md` & `unitorch-0.0.0.5/wiki/index.md`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/wiki/installation.md` & `unitorch-0.0.0.5/wiki/installation.md`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/wiki/models/peft.md` & `unitorch-0.0.0.5/wiki/models/peft.md`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.4/wiki/overview.md` & `unitorch-0.0.0.5/wiki/overview.md`

 * *Files identical despite different names*

