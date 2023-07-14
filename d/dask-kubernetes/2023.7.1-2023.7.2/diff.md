# Comparing `tmp/dask-kubernetes-2023.7.1.tar.gz` & `tmp/dask-kubernetes-2023.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dask-kubernetes-2023.7.1.tar", last modified: Thu Jul 13 16:04:15 2023, max compression
+gzip compressed data, was "dask-kubernetes-2023.7.2.tar", last modified: Fri Jul 14 15:52:45 2023, max compression
```

## Comparing `dask-kubernetes-2023.7.1.tar` & `dask-kubernetes-2023.7.2.tar`

### file list

```diff
@@ -1,118 +1,118 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:04:15.247977 dask-kubernetes-2023.7.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-07-13 16:04:15.247977 dask-kubernetes-2023.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:04:15.247977 dask-kubernetes-2023.7.1/dask_kubernetes/
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-13 16:04:15.247977 dask-kubernetes-2023.7.1/dask_kubernetes/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:04:15.239977 dask-kubernetes-2023.7.1/dask_kubernetes/aiopykube/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/aiopykube/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/aiopykube/dask.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/aiopykube/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/aiopykube/objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/aiopykube/query.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:04:15.239977 dask-kubernetes-2023.7.1/dask_kubernetes/aiopykube/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/aiopykube/tests/test_pykube_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/aiopykube/tests/test_query.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:04:15.239977 dask-kubernetes-2023.7.1/dask_kubernetes/classic/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/classic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28558 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/classic/kubecluster.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:04:15.239977 dask-kubernetes-2023.7.1/dask_kubernetes/classic/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/classic/tests/config-demo.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/classic/tests/fake_gcp_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    28838 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/classic/tests/test_async.py
--rw-r--r--   0 runner    (1001) docker     (123)    15197 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/classic/tests/test_sync.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:04:15.239977 dask-kubernetes-2023.7.1/dask_kubernetes/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/cli/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:04:15.239977 dask-kubernetes-2023.7.1/dask_kubernetes/common/
--rw-r--r--   0 runner    (1001) docker     (123)    16612 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/common/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     8212 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/common/networking.py
--rw-r--r--   0 runner    (1001) docker     (123)    12627 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/common/objects.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:04:15.239977 dask-kubernetes-2023.7.1/dask_kubernetes/common/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/common/tests/test_kind.py
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/common/tests/test_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/common/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:04:15.239977 dask-kubernetes-2023.7.1/dask_kubernetes/experimental/
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/experimental/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:04:15.243977 dask-kubernetes-2023.7.1/dask_kubernetes/helm/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/helm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12156 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/helm/helmcluster.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:04:15.243977 dask-kubernetes-2023.7.1/dask_kubernetes/helm/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:04:15.243977 dask-kubernetes-2023.7.1/dask_kubernetes/helm/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/helm/tests/resources/values.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6567 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/helm/tests/test_helm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/kubernetes.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:04:15.243977 dask-kubernetes-2023.7.1/dask_kubernetes/operator/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/operator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4568 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/operator/_objects.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:04:15.243977 dask-kubernetes-2023.7.1/dask_kubernetes/operator/controller/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/operator/controller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33038 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/operator/controller/controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:04:15.243977 dask-kubernetes-2023.7.1/dask_kubernetes/operator/controller/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/operator/controller/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:04:15.243977 dask-kubernetes-2023.7.1/dask_kubernetes/operator/controller/plugins/noop/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/operator/controller/plugins/noop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/operator/controller/plugins/noop/noop.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:04:15.243977 dask-kubernetes-2023.7.1/dask_kubernetes/operator/controller/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:04:15.243977 dask-kubernetes-2023.7.1/dask_kubernetes/operator/controller/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/operator/controller/tests/resources/failedjob.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/operator/controller/tests/resources/simplecluster.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/operator/controller/tests/resources/simplejob.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/operator/controller/tests/resources/simpleworkergroup.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    26316 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/operator/controller/tests/test_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:04:15.243977 dask-kubernetes-2023.7.1/dask_kubernetes/operator/customresources/
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/operator/customresources/daskautoscaler.patch.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/operator/customresources/daskautoscaler.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/operator/customresources/daskcluster.patch.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/operator/customresources/daskcluster.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/operator/customresources/daskjob.patch.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/operator/customresources/daskjob.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/operator/customresources/daskworkergroup.patch.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/operator/customresources/daskworkergroup.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/operator/customresources/templates.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:04:15.235977 dask-kubernetes-2023.7.1/dask_kubernetes/operator/deployment/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:04:15.243977 dask-kubernetes-2023.7.1/dask_kubernetes/operator/deployment/helm/
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/operator/deployment/helm/chartpress.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:04:15.243977 dask-kubernetes-2023.7.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/Chart.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:04:15.243977 dask-kubernetes-2023.7.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskautoscaler.yaml
--rw-r--r--   0 runner    (1001) docker     (123)   283847 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskcluster.yaml
--rw-r--r--   0 runner    (1001) docker     (123)   471240 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskjob.yaml
--rw-r--r--   0 runner    (1001) docker     (123)   140704 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskworkergroup.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:04:15.247977 dask-kubernetes-2023.7.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/clusterrole.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/clusterrolebinding.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/deployment.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/podmonitor-workers.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/role.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/rolebinding.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/serviceaccount.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/servicemonitor-scheduler.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/values.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:04:15.247977 dask-kubernetes-2023.7.1/dask_kubernetes/operator/kubecluster/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/operator/kubecluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/operator/kubecluster/discovery.py
--rw-r--r--   0 runner    (1001) docker     (123)    42764 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/operator/kubecluster/kubecluster.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:04:15.247977 dask-kubernetes-2023.7.1/dask_kubernetes/operator/kubecluster/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/operator/kubecluster/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/operator/kubecluster/tests/test_discovery.py
--rw-r--r--   0 runner    (1001) docker     (123)     7302 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/dask_kubernetes/operator/kubecluster/tests/test_kubecluster.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:04:15.239977 dask-kubernetes-2023.7.1/dask_kubernetes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-07-13 16:04:15.000000 dask-kubernetes-2023.7.1/dask_kubernetes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-07-13 16:04:15.000000 dask-kubernetes-2023.7.1/dask_kubernetes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 16:04:15.000000 dask-kubernetes-2023.7.1/dask_kubernetes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-13 16:04:15.000000 dask-kubernetes-2023.7.1/dask_kubernetes.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 16:04:15.000000 dask-kubernetes-2023.7.1/dask_kubernetes.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-13 16:04:15.000000 dask-kubernetes-2023.7.1/dask_kubernetes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-13 16:04:15.000000 dask-kubernetes-2023.7.1/dask_kubernetes.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-07-13 16:04:15.247977 dask-kubernetes-2023.7.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1032 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    68747 2023-07-13 16:04:07.000000 dask-kubernetes-2023.7.1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:52:45.149387 dask-kubernetes-2023.7.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-07-14 15:52:45.149387 dask-kubernetes-2023.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:52:45.149387 dask-kubernetes-2023.7.2/dask_kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-14 15:52:45.149387 dask-kubernetes-2023.7.2/dask_kubernetes/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:52:45.141387 dask-kubernetes-2023.7.2/dask_kubernetes/aiopykube/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/aiopykube/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/aiopykube/dask.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/aiopykube/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/aiopykube/objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/aiopykube/query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:52:45.141387 dask-kubernetes-2023.7.2/dask_kubernetes/aiopykube/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/aiopykube/tests/test_pykube_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/aiopykube/tests/test_query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:52:45.141387 dask-kubernetes-2023.7.2/dask_kubernetes/classic/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/classic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28558 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/classic/kubecluster.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:52:45.141387 dask-kubernetes-2023.7.2/dask_kubernetes/classic/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/classic/tests/config-demo.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/classic/tests/fake_gcp_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28838 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/classic/tests/test_async.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15197 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/classic/tests/test_sync.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:52:45.141387 dask-kubernetes-2023.7.2/dask_kubernetes/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/cli/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:52:45.141387 dask-kubernetes-2023.7.2/dask_kubernetes/common/
+-rw-r--r--   0 runner    (1001) docker     (123)    16612 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/common/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8212 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/common/networking.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12627 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/common/objects.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:52:45.141387 dask-kubernetes-2023.7.2/dask_kubernetes/common/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/common/tests/test_kind.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/common/tests/test_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/common/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:52:45.141387 dask-kubernetes-2023.7.2/dask_kubernetes/experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/experimental/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:52:45.141387 dask-kubernetes-2023.7.2/dask_kubernetes/helm/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/helm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12156 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/helm/helmcluster.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:52:45.141387 dask-kubernetes-2023.7.2/dask_kubernetes/helm/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:52:45.141387 dask-kubernetes-2023.7.2/dask_kubernetes/helm/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/helm/tests/resources/values.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6567 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/helm/tests/test_helm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/kubernetes.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:52:45.141387 dask-kubernetes-2023.7.2/dask_kubernetes/operator/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/operator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4568 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/operator/_objects.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:52:45.141387 dask-kubernetes-2023.7.2/dask_kubernetes/operator/controller/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/operator/controller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32989 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/operator/controller/controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:52:45.141387 dask-kubernetes-2023.7.2/dask_kubernetes/operator/controller/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/operator/controller/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:52:45.141387 dask-kubernetes-2023.7.2/dask_kubernetes/operator/controller/plugins/noop/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/operator/controller/plugins/noop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/operator/controller/plugins/noop/noop.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:52:45.141387 dask-kubernetes-2023.7.2/dask_kubernetes/operator/controller/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:52:45.141387 dask-kubernetes-2023.7.2/dask_kubernetes/operator/controller/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/operator/controller/tests/resources/failedjob.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/operator/controller/tests/resources/simplecluster.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/operator/controller/tests/resources/simplejob.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/operator/controller/tests/resources/simpleworkergroup.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    26316 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/operator/controller/tests/test_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:52:45.145387 dask-kubernetes-2023.7.2/dask_kubernetes/operator/customresources/
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/operator/customresources/daskautoscaler.patch.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/operator/customresources/daskautoscaler.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/operator/customresources/daskcluster.patch.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/operator/customresources/daskcluster.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/operator/customresources/daskjob.patch.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/operator/customresources/daskjob.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/operator/customresources/daskworkergroup.patch.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/operator/customresources/daskworkergroup.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/operator/customresources/templates.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:52:45.137386 dask-kubernetes-2023.7.2/dask_kubernetes/operator/deployment/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:52:45.145387 dask-kubernetes-2023.7.2/dask_kubernetes/operator/deployment/helm/
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/operator/deployment/helm/chartpress.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:52:45.145387 dask-kubernetes-2023.7.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/Chart.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:52:45.145387 dask-kubernetes-2023.7.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskautoscaler.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)   283847 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskcluster.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)   471240 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskjob.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)   140704 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskworkergroup.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:52:45.145387 dask-kubernetes-2023.7.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/clusterrole.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/clusterrolebinding.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/deployment.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/podmonitor-workers.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/role.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/rolebinding.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/serviceaccount.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/servicemonitor-scheduler.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/values.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:52:45.149387 dask-kubernetes-2023.7.2/dask_kubernetes/operator/kubecluster/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/operator/kubecluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/operator/kubecluster/discovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42764 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/operator/kubecluster/kubecluster.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:52:45.149387 dask-kubernetes-2023.7.2/dask_kubernetes/operator/kubecluster/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/operator/kubecluster/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/operator/kubecluster/tests/test_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7302 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/dask_kubernetes/operator/kubecluster/tests/test_kubecluster.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:52:45.137386 dask-kubernetes-2023.7.2/dask_kubernetes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-07-14 15:52:45.000000 dask-kubernetes-2023.7.2/dask_kubernetes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-07-14 15:52:45.000000 dask-kubernetes-2023.7.2/dask_kubernetes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 15:52:45.000000 dask-kubernetes-2023.7.2/dask_kubernetes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-14 15:52:45.000000 dask-kubernetes-2023.7.2/dask_kubernetes.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 15:52:45.000000 dask-kubernetes-2023.7.2/dask_kubernetes.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-14 15:52:45.000000 dask-kubernetes-2023.7.2/dask_kubernetes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-14 15:52:45.000000 dask-kubernetes-2023.7.2/dask_kubernetes.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-07-14 15:52:45.149387 dask-kubernetes-2023.7.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1032 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68747 2023-07-14 15:52:29.000000 dask-kubernetes-2023.7.2/versioneer.py
```

### Comparing `dask-kubernetes-2023.7.1/LICENSE` & `dask-kubernetes-2023.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.1/PKG-INFO` & `dask-kubernetes-2023.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dask-kubernetes
-Version: 2023.7.1
+Version: 2023.7.2
 Summary: Native Kubernetes integration for Dask
 Home-page: https://github.com/dask/dask-kubernetes
 Maintainer: Jacob Tomlinson
 License: BSD
 Keywords: dask,kubernetes,distributed
 Requires-Python: >=3.9
 License-File: LICENSE
```

### Comparing `dask-kubernetes-2023.7.1/README.rst` & `dask-kubernetes-2023.7.2/README.rst`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.1/dask_kubernetes/__init__.py` & `dask-kubernetes-2023.7.2/dask_kubernetes/__init__.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.1/dask_kubernetes/aiopykube/dask.py` & `dask-kubernetes-2023.7.2/dask_kubernetes/aiopykube/dask.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.1/dask_kubernetes/aiopykube/mixins.py` & `dask-kubernetes-2023.7.2/dask_kubernetes/aiopykube/mixins.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.1/dask_kubernetes/aiopykube/objects.py` & `dask-kubernetes-2023.7.2/dask_kubernetes/aiopykube/objects.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.1/dask_kubernetes/aiopykube/query.py` & `dask-kubernetes-2023.7.2/dask_kubernetes/aiopykube/query.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.1/dask_kubernetes/aiopykube/tests/test_pykube_objects.py` & `dask-kubernetes-2023.7.2/dask_kubernetes/aiopykube/tests/test_pykube_objects.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.1/dask_kubernetes/aiopykube/tests/test_query.py` & `dask-kubernetes-2023.7.2/dask_kubernetes/aiopykube/tests/test_query.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.1/dask_kubernetes/classic/kubecluster.py` & `dask-kubernetes-2023.7.2/dask_kubernetes/classic/kubecluster.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.1/dask_kubernetes/classic/tests/config-demo.yaml` & `dask-kubernetes-2023.7.2/dask_kubernetes/classic/tests/config-demo.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.1/dask_kubernetes/classic/tests/test_async.py` & `dask-kubernetes-2023.7.2/dask_kubernetes/classic/tests/test_async.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.1/dask_kubernetes/classic/tests/test_sync.py` & `dask-kubernetes-2023.7.2/dask_kubernetes/classic/tests/test_sync.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.1/dask_kubernetes/cli/cli.py` & `dask-kubernetes-2023.7.2/dask_kubernetes/cli/cli.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.1/dask_kubernetes/common/auth.py` & `dask-kubernetes-2023.7.2/dask_kubernetes/common/auth.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.1/dask_kubernetes/common/networking.py` & `dask-kubernetes-2023.7.2/dask_kubernetes/common/networking.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.1/dask_kubernetes/common/objects.py` & `dask-kubernetes-2023.7.2/dask_kubernetes/common/objects.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.1/dask_kubernetes/common/tests/test_kind.py` & `dask-kubernetes-2023.7.2/dask_kubernetes/common/tests/test_kind.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.1/dask_kubernetes/common/tests/test_objects.py` & `dask-kubernetes-2023.7.2/dask_kubernetes/common/tests/test_objects.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.1/dask_kubernetes/common/utils.py` & `dask-kubernetes-2023.7.2/dask_kubernetes/common/utils.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.1/dask_kubernetes/conftest.py` & `dask-kubernetes-2023.7.2/dask_kubernetes/conftest.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.1/dask_kubernetes/experimental/__init__.py` & `dask-kubernetes-2023.7.2/dask_kubernetes/experimental/__init__.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.1/dask_kubernetes/helm/helmcluster.py` & `dask-kubernetes-2023.7.2/dask_kubernetes/helm/helmcluster.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.1/dask_kubernetes/helm/tests/test_helm.py` & `dask-kubernetes-2023.7.2/dask_kubernetes/helm/tests/test_helm.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.1/dask_kubernetes/kubernetes.yaml` & `dask-kubernetes-2023.7.2/dask_kubernetes/kubernetes.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.1/dask_kubernetes/operator/_objects.py` & `dask-kubernetes-2023.7.2/dask_kubernetes/operator/_objects.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.1/dask_kubernetes/operator/controller/controller.py` & `dask-kubernetes-2023.7.2/dask_kubernetes/operator/controller/controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import time
 from contextlib import suppress
 from datetime import datetime
 from uuid import uuid4
 
 import aiohttp
 import kopf
+import kr8s
 from kr8s.asyncio.objects import Pod
 import kubernetes_asyncio as kubernetes
 from importlib_metadata import entry_points
 from kubernetes_asyncio.client import ApiException
 
 from dask_kubernetes.operator._objects import (
     DaskCluster,
@@ -461,21 +462,20 @@
             await scheduler_comm.retire_workers(names=workers_to_close)
             return workers_to_close
 
     # Finally fall back to last-in-first-out scaling
     logger.debug(
         f"Scaling {worker_group_name} failed via the Dask RPC, falling back to LIFO scaling"
     )
-    async with kubernetes.client.api_client.ApiClient() as api_client:
-        api = kubernetes.client.CoreV1Api(api_client)
-        workers = await api.list_namespaced_pod(
-            namespace=namespace,
-            label_selector=f"dask.org/workergroup-name={worker_group_name}",
-        )
-        return [w["metadata"]["name"] for w in workers.items[:-n_workers]]
+    workers = await kr8s.asyncio.get(
+        "pods",
+        namespace=namespace,
+        label_selector={"dask.org/workergroup-name": worker_group_name},
+    )
+    return [w.name for w in workers[:-n_workers]]
 
 
 async def check_scheduler_idle(scheduler_service_name, namespace, logger):
     # Try getting idle time via HTTP API
     dashboard_address = await get_scheduler_address(
         scheduler_service_name,
         namespace,
@@ -630,16 +630,21 @@
             worker_spec = spec["worker"]
             if "metadata" in worker_spec:
                 if "annotations" in worker_spec["metadata"]:
                     annotations.update(**worker_spec["metadata"]["annotations"])
                 if "labels" in worker_spec["metadata"]:
                     labels.update(**worker_spec["metadata"]["labels"])
 
-            SIZE = dask.config.get("kubernetes.controller.worker-allocation.batch-size")
-            DELAY = dask.config.get("kubernetes.controller.worker-allocation.delay")
+            SIZE = int(
+                dask.config.get("kubernetes.controller.worker-allocation.batch-size")
+                or 0
+            )
+            DELAY = int(
+                dask.config.get("kubernetes.controller.worker-allocation.delay") or 0
+            )
             batch_size = min(workers_needed, SIZE) if SIZE else workers_needed
             if workers_needed > 0:
                 for _ in range(batch_size):
                     data = build_worker_deployment_spec(
                         worker_group_name=name,
                         namespace=namespace,
                         cluster_name=cluster_name,
```

### Comparing `dask-kubernetes-2023.7.1/dask_kubernetes/operator/controller/tests/resources/failedjob.yaml` & `dask-kubernetes-2023.7.2/dask_kubernetes/operator/controller/tests/resources/failedjob.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.1/dask_kubernetes/operator/controller/tests/resources/simplecluster.yaml` & `dask-kubernetes-2023.7.2/dask_kubernetes/operator/controller/tests/resources/simplecluster.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.1/dask_kubernetes/operator/controller/tests/resources/simplejob.yaml` & `dask-kubernetes-2023.7.2/dask_kubernetes/operator/controller/tests/resources/simplejob.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.1/dask_kubernetes/operator/controller/tests/resources/simpleworkergroup.yaml` & `dask-kubernetes-2023.7.2/dask_kubernetes/operator/controller/tests/resources/simpleworkergroup.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.1/dask_kubernetes/operator/controller/tests/test_controller.py` & `dask-kubernetes-2023.7.2/dask_kubernetes/operator/controller/tests/test_controller.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.1/dask_kubernetes/operator/customresources/daskautoscaler.yaml` & `dask-kubernetes-2023.7.2/dask_kubernetes/operator/customresources/daskautoscaler.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.1/dask_kubernetes/operator/customresources/daskcluster.patch.yaml` & `dask-kubernetes-2023.7.2/dask_kubernetes/operator/customresources/daskcluster.patch.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.1/dask_kubernetes/operator/customresources/daskcluster.yaml` & `dask-kubernetes-2023.7.2/dask_kubernetes/operator/customresources/daskcluster.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.1/dask_kubernetes/operator/customresources/daskjob.patch.yaml` & `dask-kubernetes-2023.7.2/dask_kubernetes/operator/customresources/daskjob.patch.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.1/dask_kubernetes/operator/customresources/daskjob.yaml` & `dask-kubernetes-2023.7.2/dask_kubernetes/operator/customresources/daskjob.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.1/dask_kubernetes/operator/customresources/daskworkergroup.yaml` & `dask-kubernetes-2023.7.2/dask_kubernetes/operator/customresources/daskworkergroup.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.1/dask_kubernetes/operator/customresources/templates.yaml` & `dask-kubernetes-2023.7.2/dask_kubernetes/operator/customresources/templates.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.1/dask_kubernetes/operator/deployment/helm/chartpress.yaml` & `dask-kubernetes-2023.7.2/dask_kubernetes/operator/deployment/helm/chartpress.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskautoscaler.yaml` & `dask-kubernetes-2023.7.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskautoscaler.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskcluster.yaml` & `dask-kubernetes-2023.7.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskcluster.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskjob.yaml` & `dask-kubernetes-2023.7.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskjob.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskworkergroup.yaml` & `dask-kubernetes-2023.7.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskworkergroup.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/clusterrole.yaml` & `dask-kubernetes-2023.7.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/clusterrole.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/clusterrolebinding.yaml` & `dask-kubernetes-2023.7.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/clusterrolebinding.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/deployment.yaml` & `dask-kubernetes-2023.7.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/deployment.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -29,20 +29,22 @@
       containers:
         - name: {{ .Chart.Name }}
           securityContext:
             {{- toYaml .Values.securityContext | nindent 12 }}
           image: "{{ .Values.image.name }}:{{ .Values.image.tag }}"
           imagePullPolicy: {{ .Values.image.pullPolicy }}
           env:
+            {{- with .Values.workerAllocation.size }}
             - name: DASK_KUBERNETES__CONTROLLER__WORKER_ALLOCATION__BATCH_SIZE
-              value:
-                {{- toYaml .Values.workerAllocation.size | nindent 16 }}
+              value: {{ . | quote }}
+            {{- end }}
+            {{- with .Values.workerAllocation.delay }}
             - name: DASK_KUBERNETES__CONTROLLER__WORKER_ALLOCATION__DELAY
-              value:
-                {{- toYaml .Values.workerAllocation.delay | nindent 16 }}
+              value: {{ . | quote }}
+            {{- end }}
           args:
             - --liveness=http://0.0.0.0:8080/healthz
           {{- with .Values.kopfArgs }}
             {{- toYaml . | nindent 12 }}
           {{- end }}
           resources:
             {{- toYaml .Values.resources | nindent 12 }}
```

### Comparing `dask-kubernetes-2023.7.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/podmonitor-workers.yaml` & `dask-kubernetes-2023.7.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/podmonitor-workers.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/role.yaml` & `dask-kubernetes-2023.7.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/role.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/servicemonitor-scheduler.yaml` & `dask-kubernetes-2023.7.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/servicemonitor-scheduler.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/values.yaml` & `dask-kubernetes-2023.7.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/values.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.1/dask_kubernetes/operator/kubecluster/discovery.py` & `dask-kubernetes-2023.7.2/dask_kubernetes/operator/kubecluster/discovery.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.1/dask_kubernetes/operator/kubecluster/kubecluster.py` & `dask-kubernetes-2023.7.2/dask_kubernetes/operator/kubecluster/kubecluster.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.1/dask_kubernetes/operator/kubecluster/tests/conftest.py` & `dask-kubernetes-2023.7.2/dask_kubernetes/operator/kubecluster/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.1/dask_kubernetes/operator/kubecluster/tests/test_discovery.py` & `dask-kubernetes-2023.7.2/dask_kubernetes/operator/kubecluster/tests/test_discovery.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.1/dask_kubernetes/operator/kubecluster/tests/test_kubecluster.py` & `dask-kubernetes-2023.7.2/dask_kubernetes/operator/kubecluster/tests/test_kubecluster.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.1/dask_kubernetes.egg-info/PKG-INFO` & `dask-kubernetes-2023.7.2/dask_kubernetes.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dask-kubernetes
-Version: 2023.7.1
+Version: 2023.7.2
 Summary: Native Kubernetes integration for Dask
 Home-page: https://github.com/dask/dask-kubernetes
 Maintainer: Jacob Tomlinson
 License: BSD
 Keywords: dask,kubernetes,distributed
 Requires-Python: >=3.9
 License-File: LICENSE
```

### Comparing `dask-kubernetes-2023.7.1/dask_kubernetes.egg-info/SOURCES.txt` & `dask-kubernetes-2023.7.2/dask_kubernetes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.1/setup.cfg` & `dask-kubernetes-2023.7.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.1/setup.py` & `dask-kubernetes-2023.7.2/setup.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2023.7.1/versioneer.py` & `dask-kubernetes-2023.7.2/versioneer.py`

 * *Files identical despite different names*

