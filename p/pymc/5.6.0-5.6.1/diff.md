# Comparing `tmp/pymc-5.6.0.tar.gz` & `tmp/pymc-5.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pymc-5.6.0.tar", last modified: Tue Jul  4 12:11:14 2023, max compression
+gzip compressed data, was "dist/pymc-5.6.1.tar", last modified: Fri Jul 14 07:23:02 2023, max compression
```

## Comparing `pymc-5.6.0.tar` & `pymc-5.6.1.tar`

### file list

```diff
@@ -1,134 +1,134 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:11:14.000000 pymc-5.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-07-04 12:11:04.000000 pymc-5.6.0/ARCHITECTURE.md
--rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-07-04 12:11:04.000000 pymc-5.6.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-04 12:11:04.000000 pymc-5.6.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    42347 2023-07-04 12:11:04.000000 pymc-5.6.0/GOVERNANCE.md
--rw-r--r--   0 runner    (1001) docker     (123)    12865 2023-07-04 12:11:04.000000 pymc-5.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-04 12:11:04.000000 pymc-5.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11542 2023-07-04 12:11:14.000000 pymc-5.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9130 2023-07-04 12:11:04.000000 pymc-5.6.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)    81106 2023-07-04 12:11:04.000000 pymc-5.6.0/RELEASE-NOTES.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:11:14.000000 pymc-5.6.0/pymc/
--rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-04 12:11:14.000000 pymc-5.6.0/pymc/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:11:14.000000 pymc-5.6.0/pymc/backends/
--rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21822 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/backends/arviz.py
--rw-r--r--   0 runner    (1001) docker     (123)    19525 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/backends/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    10381 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/backends/mcbackend.py
--rw-r--r--   0 runner    (1001) docker     (123)     8127 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/backends/ndarray.py
--rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/backends/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/blocking.py
--rw-r--r--   0 runner    (1001) docker     (123)    16820 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:11:14.000000 pymc-5.6.0/pymc/distributions/
--rw-r--r--   0 runner    (1001) docker     (123)     4218 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/distributions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9764 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/distributions/bound.py
--rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/distributions/censored.py
--rw-r--r--   0 runner    (1001) docker     (123)   118744 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/distributions/continuous.py
--rw-r--r--   0 runner    (1001) docker     (123)    42226 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/distributions/discrete.py
--rw-r--r--   0 runner    (1001) docker     (123)    15229 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/distributions/dist_math.py
--rw-r--r--   0 runner    (1001) docker     (123)    46063 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/distributions/distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)    36248 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/distributions/mixture.py
--rw-r--r--   0 runner    (1001) docker     (123)    89229 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/distributions/multivariate.py
--rw-r--r--   0 runner    (1001) docker     (123)    18231 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/distributions/shape_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    12579 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/distributions/simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)    38767 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/distributions/timeseries.py
--rw-r--r--   0 runner    (1001) docker     (123)    12769 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/distributions/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)    14684 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/distributions/truncated.py
--rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7579 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/func_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:11:14.000000 pymc-5.6.0/pymc/gp/
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/gp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32081 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/gp/cov.py
--rw-r--r--   0 runner    (1001) docker     (123)    49766 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/gp/gp.py
--rw-r--r--   0 runner    (1001) docker     (123)    14494 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/gp/hsgp_approx.py
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/gp/mean.py
--rw-r--r--   0 runner    (1001) docker     (123)     7734 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/gp/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    11097 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/initial_point.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:11:14.000000 pymc-5.6.0/pymc/logprob/
--rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/logprob/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5111 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/logprob/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)    22033 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/logprob/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     5464 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/logprob/binary.py
--rw-r--r--   0 runner    (1001) docker     (123)     8678 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/logprob/censoring.py
--rw-r--r--   0 runner    (1001) docker     (123)     5051 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/logprob/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/logprob/cumsum.py
--rw-r--r--   0 runner    (1001) docker     (123)    21063 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/logprob/mixture.py
--rw-r--r--   0 runner    (1001) docker     (123)    19901 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/logprob/rewriting.py
--rw-r--r--   0 runner    (1001) docker     (123)    22586 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/logprob/scan.py
--rw-r--r--   0 runner    (1001) docker     (123)    11975 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/logprob/tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)    35387 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/logprob/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     9828 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/logprob/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    15253 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/math.py
--rw-r--r--   0 runner    (1001) docker     (123)    85069 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    16575 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/model_graph.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:11:14.000000 pymc-5.6.0/pymc/ode/
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/ode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9657 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/ode/ode.py
--rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/ode/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:11:14.000000 pymc-5.6.0/pymc/plots/
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10014 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/printing.py
--rw-r--r--   0 runner    (1001) docker     (123)    39443 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/pytensorf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:11:14.000000 pymc-5.6.0/pymc/sampling/
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/sampling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29883 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/sampling/forward.py
--rw-r--r--   0 runner    (1001) docker     (123)    25876 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/sampling/jax.py
--rw-r--r--   0 runner    (1001) docker     (123)    51405 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/sampling/mcmc.py
--rw-r--r--   0 runner    (1001) docker     (123)    15599 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/sampling/parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)    15011 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/sampling/population.py
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/sampling_jax.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:11:14.000000 pymc-5.6.0/pymc/smc/
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/smc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24432 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/smc/kernels.py
--rw-r--r--   0 runner    (1001) docker     (123)    14868 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/smc/sampling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:11:14.000000 pymc-5.6.0/pymc/stats/
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/stats/convergence.py
--rw-r--r--   0 runner    (1001) docker     (123)     4704 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/stats/log_likelihood.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:11:14.000000 pymc-5.6.0/pymc/step_methods/
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/step_methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7034 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/step_methods/arraystep.py
--rw-r--r--   0 runner    (1001) docker     (123)    10641 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/step_methods/compound.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:11:14.000000 pymc-5.6.0/pymc/step_methods/hmc/
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/step_methods/hmc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9044 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/step_methods/hmc/base_hmc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7519 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/step_methods/hmc/hmc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/step_methods/hmc/integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    17591 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/step_methods/hmc/nuts.py
--rw-r--r--   0 runner    (1001) docker     (123)    27526 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/step_methods/hmc/quadpotential.py
--rw-r--r--   0 runner    (1001) docker     (123)    35731 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/step_methods/metropolis.py
--rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/step_methods/slicer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/step_methods/step_sizes.py
--rw-r--r--   0 runner    (1001) docker     (123)    36022 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:11:14.000000 pymc-5.6.0/pymc/tuning/
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/tuning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/tuning/scaling.py
--rw-r--r--   0 runner    (1001) docker     (123)     9296 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/tuning/starting.py
--rw-r--r--   0 runner    (1001) docker     (123)    16919 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:11:14.000000 pymc-5.6.0/pymc/variational/
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/variational/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13158 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/variational/approximations.py
--rw-r--r--   0 runner    (1001) docker     (123)     4710 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/variational/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)    28608 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/variational/inference.py
--rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/variational/minibatch_rv.py
--rw-r--r--   0 runner    (1001) docker     (123)     4566 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/variational/operators.py
--rw-r--r--   0 runner    (1001) docker     (123)    57336 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/variational/opvi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/variational/stein.py
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/variational/test_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    37930 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/variational/updates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-07-04 12:11:04.000000 pymc-5.6.0/pymc/vartypes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:11:14.000000 pymc-5.6.0/pymc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11542 2023-07-04 12:11:14.000000 pymc-5.6.0/pymc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-07-04 12:11:14.000000 pymc-5.6.0/pymc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 12:11:14.000000 pymc-5.6.0/pymc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-04 12:11:14.000000 pymc-5.6.0/pymc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-04 12:11:14.000000 pymc-5.6.0/pymc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-04 12:11:04.000000 pymc-5.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-04 12:11:04.000000 pymc-5.6.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:11:14.000000 pymc-5.6.0/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)      833 2023-07-04 12:11:04.000000 pymc-5.6.0/scripts/docker_container.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      181 2023-07-04 12:11:04.000000 pymc-5.6.0/scripts/test.sh
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-04 12:11:14.000000 pymc-5.6.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2698 2023-07-04 12:11:04.000000 pymc-5.6.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    81282 2023-07-04 12:11:04.000000 pymc-5.6.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:23:02.000000 pymc-5.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-07-14 07:22:52.000000 pymc-5.6.1/ARCHITECTURE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-07-14 07:22:52.000000 pymc-5.6.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-14 07:22:52.000000 pymc-5.6.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    42347 2023-07-14 07:22:52.000000 pymc-5.6.1/GOVERNANCE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    12865 2023-07-14 07:22:52.000000 pymc-5.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-14 07:22:52.000000 pymc-5.6.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11542 2023-07-14 07:23:02.000000 pymc-5.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9130 2023-07-14 07:22:52.000000 pymc-5.6.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    81106 2023-07-14 07:22:52.000000 pymc-5.6.1/RELEASE-NOTES.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:23:02.000000 pymc-5.6.1/pymc/
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-14 07:23:02.000000 pymc-5.6.1/pymc/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:23:02.000000 pymc-5.6.1/pymc/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21822 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/backends/arviz.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19525 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/backends/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10381 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/backends/mcbackend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8127 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/backends/ndarray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/backends/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/blocking.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16820 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:23:02.000000 pymc-5.6.1/pymc/distributions/
+-rw-r--r--   0 runner    (1001) docker     (123)     4218 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/distributions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9764 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/distributions/bound.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/distributions/censored.py
+-rw-r--r--   0 runner    (1001) docker     (123)   118744 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/distributions/continuous.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42226 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/distributions/discrete.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15229 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/distributions/dist_math.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46117 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/distributions/distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36248 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/distributions/mixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)    89229 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/distributions/multivariate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18227 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/distributions/shape_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12579 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/distributions/simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38767 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/distributions/timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12769 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/distributions/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14684 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/distributions/truncated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7579 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/func_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:23:02.000000 pymc-5.6.1/pymc/gp/
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/gp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32081 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/gp/cov.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49766 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/gp/gp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14494 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/gp/hsgp_approx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/gp/mean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7734 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/gp/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11097 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/initial_point.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:23:02.000000 pymc-5.6.1/pymc/logprob/
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/logprob/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5111 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/logprob/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22033 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/logprob/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5464 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/logprob/binary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8678 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/logprob/censoring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5051 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/logprob/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/logprob/cumsum.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21063 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/logprob/mixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19899 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/logprob/rewriting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22586 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/logprob/scan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11975 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/logprob/tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35387 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/logprob/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9828 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/logprob/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15253 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/math.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85727 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16575 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/model_graph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:23:02.000000 pymc-5.6.1/pymc/ode/
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/ode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9657 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/ode/ode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/ode/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:23:02.000000 pymc-5.6.1/pymc/plots/
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10014 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/printing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39443 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/pytensorf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:23:02.000000 pymc-5.6.1/pymc/sampling/
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/sampling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29883 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/sampling/forward.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25872 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/sampling/jax.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51405 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/sampling/mcmc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15599 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/sampling/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15011 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/sampling/population.py
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/sampling_jax.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:23:02.000000 pymc-5.6.1/pymc/smc/
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/smc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24432 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/smc/kernels.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14868 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/smc/sampling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:23:02.000000 pymc-5.6.1/pymc/stats/
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/stats/convergence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4704 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/stats/log_likelihood.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:23:02.000000 pymc-5.6.1/pymc/step_methods/
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/step_methods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7034 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/step_methods/arraystep.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10641 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/step_methods/compound.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:23:02.000000 pymc-5.6.1/pymc/step_methods/hmc/
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/step_methods/hmc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9044 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/step_methods/hmc/base_hmc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7519 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/step_methods/hmc/hmc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/step_methods/hmc/integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17591 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/step_methods/hmc/nuts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27526 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/step_methods/hmc/quadpotential.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35731 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/step_methods/metropolis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/step_methods/slicer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/step_methods/step_sizes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36022 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:23:02.000000 pymc-5.6.1/pymc/tuning/
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/tuning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/tuning/scaling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9296 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/tuning/starting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16919 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:23:02.000000 pymc-5.6.1/pymc/variational/
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/variational/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13158 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/variational/approximations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4710 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/variational/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28608 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/variational/inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/variational/minibatch_rv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4566 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/variational/operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57336 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/variational/opvi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/variational/stein.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/variational/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37930 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/variational/updates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-07-14 07:22:52.000000 pymc-5.6.1/pymc/vartypes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:23:02.000000 pymc-5.6.1/pymc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11542 2023-07-14 07:23:02.000000 pymc-5.6.1/pymc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-07-14 07:23:02.000000 pymc-5.6.1/pymc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 07:23:02.000000 pymc-5.6.1/pymc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-14 07:23:02.000000 pymc-5.6.1/pymc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-14 07:23:02.000000 pymc-5.6.1/pymc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-14 07:22:52.000000 pymc-5.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-14 07:22:52.000000 pymc-5.6.1/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 07:23:02.000000 pymc-5.6.1/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      833 2023-07-14 07:22:52.000000 pymc-5.6.1/scripts/docker_container.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      181 2023-07-14 07:22:52.000000 pymc-5.6.1/scripts/test.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-14 07:23:02.000000 pymc-5.6.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2698 2023-07-14 07:22:52.000000 pymc-5.6.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81282 2023-07-14 07:22:52.000000 pymc-5.6.1/versioneer.py
```

### Comparing `pymc-5.6.0/ARCHITECTURE.md` & `pymc-5.6.1/ARCHITECTURE.md`

 * *Files identical despite different names*

### Comparing `pymc-5.6.0/CODE_OF_CONDUCT.md` & `pymc-5.6.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pymc-5.6.0/CONTRIBUTING.md` & `pymc-5.6.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pymc-5.6.0/GOVERNANCE.md` & `pymc-5.6.1/GOVERNANCE.md`

 * *Files identical despite different names*

### Comparing `pymc-5.6.0/LICENSE` & `pymc-5.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pymc-5.6.0/PKG-INFO` & `pymc-5.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymc
-Version: 5.6.0
+Version: 5.6.1
 Summary: Probabilistic Programming in Python: Bayesian Modeling and Probabilistic Machine Learning with PyTensor
 Home-page: http://github.com/pymc-devs/pymc
 Maintainer: PyMC Developers
 Maintainer-email: pymc.devs@gmail.com
 License: Apache License, Version 2.0
 Description: .. image:: https://cdn.rawgit.com/pymc-devs/pymc/main/docs/logos/svg/PyMC_banner.svg
             :height: 100px
```

### Comparing `pymc-5.6.0/README.rst` & `pymc-5.6.1/README.rst`

 * *Files identical despite different names*

### Comparing `pymc-5.6.0/RELEASE-NOTES.md` & `pymc-5.6.1/RELEASE-NOTES.md`

 * *Files identical despite different names*

### Comparing `pymc-5.6.0/pymc/__init__.py` & `pymc-5.6.1/pymc/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.0/pymc/backends/__init__.py` & `pymc-5.6.1/pymc/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.0/pymc/backends/arviz.py` & `pymc-5.6.1/pymc/backends/arviz.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.0/pymc/backends/base.py` & `pymc-5.6.1/pymc/backends/base.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.0/pymc/backends/mcbackend.py` & `pymc-5.6.1/pymc/backends/mcbackend.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.0/pymc/backends/ndarray.py` & `pymc-5.6.1/pymc/backends/ndarray.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.0/pymc/backends/report.py` & `pymc-5.6.1/pymc/backends/report.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.0/pymc/blocking.py` & `pymc-5.6.1/pymc/blocking.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.0/pymc/data.py` & `pymc-5.6.1/pymc/data.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.0/pymc/distributions/__init__.py` & `pymc-5.6.1/pymc/distributions/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.0/pymc/distributions/bound.py` & `pymc-5.6.1/pymc/distributions/bound.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.0/pymc/distributions/censored.py` & `pymc-5.6.1/pymc/distributions/censored.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.0/pymc/distributions/continuous.py` & `pymc-5.6.1/pymc/distributions/continuous.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.0/pymc/distributions/discrete.py` & `pymc-5.6.1/pymc/distributions/discrete.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.0/pymc/distributions/dist_math.py` & `pymc-5.6.1/pymc/distributions/dist_math.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.0/pymc/distributions/distribution.py` & `pymc-5.6.1/pymc/distributions/distribution.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     rv_size_is_none,
     shape_from_dims,
 )
 from pymc.exceptions import BlockModelAccessError
 from pymc.logprob.abstract import MeasurableVariable, _icdf, _logcdf, _logprob
 from pymc.logprob.basic import logp
 from pymc.logprob.rewriting import logprob_rewrites_db
-from pymc.model import BlockModelAccess
+from pymc.model import new_or_existing_block_model_access
 from pymc.printing import str_for_dist
 from pymc.pytensorf import collect_default_updates, convert_observed_data, floatX
 from pymc.util import UNSET, _add_future_warning_tag
 from pymc.vartypes import continuous_types, string_types
 
 __all__ = [
     "CustomDist",
@@ -641,15 +641,15 @@
         size=None,
         ndim_supp: int,
         class_name: str,
     ):
         size = normalize_size_param(size)
         dummy_size_param = size.type()
         dummy_dist_params = [dist_param.type() for dist_param in dist_params]
-        with BlockModelAccess(
+        with new_or_existing_block_model_access(
             error_msg_on_access="Model variables cannot be created in the dist function. Use the `.dist` API"
         ):
             dummy_rv = dist(*dummy_dist_params, dummy_size_param)
         dummy_params = [dummy_size_param] + dummy_dist_params
         dummy_updates_dict = collect_default_updates(inputs=dummy_params, outputs=(dummy_rv,))
 
         rv_type = type(
@@ -1044,15 +1044,15 @@
     @classmethod
     def is_symbolic_random(self, random, dist_params):
         if random is None:
             return False
         # Try calling random with symbolic inputs
         try:
             size = normalize_size_param(None)
-            with BlockModelAccess(
+            with new_or_existing_block_model_access(
                 error_msg_on_access="Model variables cannot be created in the random function. Use the `.dist` API to create such variables."
             ):
                 out = random(*dist_params, size)
         except BlockModelAccessError:
             raise
         except Exception:
             # If it fails we assume it was not
```

### Comparing `pymc-5.6.0/pymc/distributions/mixture.py` & `pymc-5.6.1/pymc/distributions/mixture.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.0/pymc/distributions/multivariate.py` & `pymc-5.6.1/pymc/distributions/multivariate.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.0/pymc/distributions/shape_utils.py` & `pymc-5.6.1/pymc/distributions/shape_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -403,15 +403,15 @@
     # Old specify_shape is still valid for support dimensions. We do not reintroduce
     # checks for resized dimensions, although we could...
     else:
         ndim_supp = new_var.owner.op.ndim_supp
         if ndim_supp > 0:
             new_shapes[-ndim_supp:] = shapes[-ndim_supp:]
 
-    # specify_shape has a wrong signature https://github.com/pytensor-devs/pytensor/issues/1164
+    # specify_shape has a wrong signature https://github.com/aesara-devs/aesara/issues/1164
     return pt.specify_shape(new_var, new_shapes)  # type: ignore
 
 
 def get_support_shape(
     support_shape: Optional[Sequence[Union[int, np.ndarray, TensorVariable]]],
     *,
     shape: Optional[Shape] = None,
```

### Comparing `pymc-5.6.0/pymc/distributions/simulator.py` & `pymc-5.6.1/pymc/distributions/simulator.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.0/pymc/distributions/timeseries.py` & `pymc-5.6.1/pymc/distributions/timeseries.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.0/pymc/distributions/transforms.py` & `pymc-5.6.1/pymc/distributions/transforms.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.0/pymc/distributions/truncated.py` & `pymc-5.6.1/pymc/distributions/truncated.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.0/pymc/exceptions.py` & `pymc-5.6.1/pymc/exceptions.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.0/pymc/func_utils.py` & `pymc-5.6.1/pymc/func_utils.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.0/pymc/gp/__init__.py` & `pymc-5.6.1/pymc/gp/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.0/pymc/gp/cov.py` & `pymc-5.6.1/pymc/gp/cov.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.0/pymc/gp/gp.py` & `pymc-5.6.1/pymc/gp/gp.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.0/pymc/gp/hsgp_approx.py` & `pymc-5.6.1/pymc/gp/hsgp_approx.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.0/pymc/gp/mean.py` & `pymc-5.6.1/pymc/gp/mean.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.0/pymc/gp/util.py` & `pymc-5.6.1/pymc/gp/util.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.0/pymc/initial_point.py` & `pymc-5.6.1/pymc/initial_point.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.0/pymc/logprob/__init__.py` & `pymc-5.6.1/pymc/logprob/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.0/pymc/logprob/abstract.py` & `pymc-5.6.1/pymc/logprob/abstract.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.0/pymc/logprob/basic.py` & `pymc-5.6.1/pymc/logprob/basic.py`

 * *Files 0% similar despite different names*

```diff
@@ -426,31 +426,31 @@
         sigma2_rv = pt.random.invgamma(0.5, 0.5)
         Y_rv = pt.random.normal(0, pt.sqrt(sigma2_rv))
 
     This graph for ``Y_rv`` is equivalent to the following hierarchical model:
 
     .. math::
 
-        \Sigma^2 \sim& \operatorname{InvGamma}(0.5, 0.5) \\
-        Y \sim& \operatorname{N}(0, \Sigma)
+        \sigma^2 \sim& \operatorname{InvGamma}(0.5, 0.5) \\
+        Y \sim& \operatorname{N}(0, \sigma^2)
 
     If we create a value variable for ``Y_rv``, i.e. ``y_vv = pt.scalar("y")``,
     the graph of ``conditional_logp({Y_rv: y_vv})`` is equivalent to the
-    conditional log-probability :math:`\log p(Y = y \mid \Sigma^2)`, with a stochastic
+    conditional log-probability :math:`\log p_{Y \mid \sigma^2}(y \mid s^2)`, with a stochastic
     ``sigma2_rv``.
 
     If we specify a value variable for ``sigma2_rv``, i.e.
-    ``s_vv = pt.scalar("s2")``, then ``conditional_logp({Y_rv: y_vv, sigma2_rv: s_vv})``
+    ``s2_vv = pt.scalar("s2")``, then ``conditional_logp({Y_rv: y_vv, sigma2_rv: s2_vv})``
     yields the conditional log-probabilities of the two variables.
     The sum of the two terms gives their joint log-probability.
 
     .. math::
 
-        \log p(Y = y, \Sigma^2 = \sigma^2) =
-            \log p(Y = y \mid \Sigma^2 = \sigma^2) + \log p(\Sigma^2 = \sigma^2)
+        \log p_{Y, \sigma^2}(y, s^2) =
+            \log p_{Y \mid \sigma^2}(y \mid s^2) + \log p_{\sigma^2}(s^2)
 
 
     Parameters
     ----------
     rv_values: dict
         A ``dict`` of variables that maps stochastic elements
         (e.g. `RandomVariable`\s) to symbolic `Variable`\s representing their
```

### Comparing `pymc-5.6.0/pymc/logprob/binary.py` & `pymc-5.6.1/pymc/logprob/binary.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.0/pymc/logprob/censoring.py` & `pymc-5.6.1/pymc/logprob/censoring.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.0/pymc/logprob/checks.py` & `pymc-5.6.1/pymc/logprob/checks.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.0/pymc/logprob/cumsum.py` & `pymc-5.6.1/pymc/logprob/cumsum.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.0/pymc/logprob/mixture.py` & `pymc-5.6.1/pymc/logprob/mixture.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.0/pymc/logprob/rewriting.py` & `pymc-5.6.1/pymc/logprob/rewriting.py`

 * *Files 0% similar despite different names*

```diff
@@ -414,15 +414,15 @@
     because--at the very least--canonicalization is always performed and the
     measurable IR includes manipulations that are not applicable to outside of
     the context of measurability/log-probabilities.
 
     For instance, some `Op`s will be lifted through `MeasurableVariable`\s in
     this IR, and the resulting graphs will not be computationally sound,
     because they wouldn't produce independent samples when the original graph
-    would.  See https://github.com/pytensor-devs/aeppl/pull/78.
+    would.  See https://github.com/aesara-devs/aeppl/pull/78.
 
     Returns
     -------
     A `FunctionGraph` of the measurable IR, a copy of `rv_values` containing
     the new, cloned versions of the original variables in `rv_values`, and
     a ``dict`` mapping all the original variables to their cloned values in
     `FunctionGraph`.
```

### Comparing `pymc-5.6.0/pymc/logprob/scan.py` & `pymc-5.6.1/pymc/logprob/scan.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.0/pymc/logprob/tensor.py` & `pymc-5.6.1/pymc/logprob/tensor.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.0/pymc/logprob/transforms.py` & `pymc-5.6.1/pymc/logprob/transforms.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.0/pymc/logprob/utils.py` & `pymc-5.6.1/pymc/logprob/utils.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.0/pymc/math.py` & `pymc-5.6.1/pymc/math.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.0/pymc/model.py` & `pymc-5.6.1/pymc/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,14 +46,15 @@
 from pytensor.graph.basic import Constant, Variable, graph_inputs
 from pytensor.scalar import Cast
 from pytensor.tensor.elemwise import Elemwise
 from pytensor.tensor.random.op import RandomVariable
 from pytensor.tensor.random.type import RandomType
 from pytensor.tensor.sharedvar import ScalarSharedVariable
 from pytensor.tensor.var import TensorConstant, TensorVariable
+from typing_extensions import Self
 
 from pymc.blocking import DictToArrayBijection, RaveledVars
 from pymc.data import GenTensorVariable, is_minibatch
 from pymc.distributions.transforms import _default_transform
 from pymc.exceptions import (
     BlockModelAccessError,
     ImputationWarning,
@@ -139,27 +140,27 @@
         cls, name, bases, nmspc, context_class: Optional[Type] = None, **kwargs
     ):  # pylint: disable=unused-argument
         """Add ``__enter__`` and ``__exit__`` methods to the new class automatically."""
         if context_class is not None:
             cls._context_class = context_class
         super().__init__(name, bases, nmspc)
 
-    def get_context(cls, error_if_none=True) -> Optional[T]:
+    def get_context(cls, error_if_none=True, allow_block_model_access=False) -> Optional[T]:
         """Return the most recently pushed context object of type ``cls``
         on the stack, or ``None``. If ``error_if_none`` is True (default),
         raise a ``TypeError`` instead of returning ``None``."""
         try:
             candidate: Optional[T] = cls.get_contexts()[-1]
         except IndexError:
             # Calling code expects to get a TypeError if the entity
             # is unfound, and there's too much to fix.
             if error_if_none:
                 raise TypeError(f"No {cls} on context stack")
             return None
-        if isinstance(candidate, BlockModelAccess):
+        if isinstance(candidate, BlockModelAccess) and not allow_block_model_access:
             raise BlockModelAccessError(candidate.error_msg_on_access)
         return candidate
 
     def get_contexts(cls) -> List[T]:
         """Return a stack of context instances for the ``context_class``
         of ``cls``."""
         # This lazily creates the context class's contexts
@@ -209,15 +210,17 @@
     def __init_subclass__(cls, **kwargs):
         super().__init_subclass__(**kwargs)
         cls.context_class = super().context_class
 
     # Initialize object in its own context...
     # Merged from InitContextMeta in the original.
     def __call__(cls, *args, **kwargs):
-        instance = cls.__new__(cls, *args, **kwargs)
+        # We type hint Model here so type checkers understand that Model is a context manager.
+        # This metaclass is only used for Model, so this is safe to do. See #6809 for more info.
+        instance: "Model" = cls.__new__(cls, *args, **kwargs)
         with instance:  # appends context
             instance.__init__(*args, **kwargs)
         return instance
 
 
 def modelcontext(model: Optional["Model"]) -> "Model":
     """
@@ -474,18 +477,18 @@
             CustomModel(mean=2, name='second')
 
         # variables inside both scopes will be named like `first::*`, `second::*`
     """
 
     if TYPE_CHECKING:
 
-        def __enter__(self: "Model") -> "Model":
+        def __enter__(self: Self) -> Self:
             ...
 
-        def __exit__(self: "Model", *exc: Any) -> bool:
+        def __exit__(self, exc_type: None, exc_val: None, exc_tb: None) -> None:
             ...
 
     def __new__(cls, *args, **kwargs):
         # resolves the parent instance
         instance = super().__new__(cls)
         if kwargs.get("model") is not None:
             instance._parent = kwargs.get("model")
@@ -1885,14 +1888,22 @@
 class BlockModelAccess(Model):
     """Can be used to prevent user access to Model contexts"""
 
     def __init__(self, *args, error_msg_on_access="Model access is blocked", **kwargs):
         self.error_msg_on_access = error_msg_on_access
 
 
+def new_or_existing_block_model_access(*args, **kwargs):
+    """Return a BlockModelAccess in the stack or create a new one if none is found."""
+    model = Model.get_context(error_if_none=False, allow_block_model_access=True)
+    if isinstance(model, BlockModelAccess):
+        return model
+    return BlockModelAccess(*args, **kwargs)
+
+
 def set_data(new_data, model=None, *, coords=None):
     """Sets the value of one or more data container variables.  Note that the shape is also
     dynamic, it is updated when the value is changed.  See the examples below for two common
     use-cases that take advantage of this behavior.
 
     Parameters
     ----------
```

### Comparing `pymc-5.6.0/pymc/model_graph.py` & `pymc-5.6.1/pymc/model_graph.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.0/pymc/ode/__init__.py` & `pymc-5.6.1/pymc/ode/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.0/pymc/ode/ode.py` & `pymc-5.6.1/pymc/ode/ode.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.0/pymc/ode/utils.py` & `pymc-5.6.1/pymc/ode/utils.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.0/pymc/plots/__init__.py` & `pymc-5.6.1/pymc/plots/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.0/pymc/printing.py` & `pymc-5.6.1/pymc/printing.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.0/pymc/pytensorf.py` & `pymc-5.6.1/pymc/pytensorf.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.0/pymc/sampling/__init__.py` & `pymc-5.6.1/pymc/sampling/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.0/pymc/sampling/forward.py` & `pymc-5.6.1/pymc/sampling/forward.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.0/pymc/sampling/jax.py` & `pymc-5.6.1/pymc/sampling/jax.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,15 +111,15 @@
     graph = _replace_shared_variables(outputs) if outputs is not None else None
 
     fgraph = FunctionGraph(inputs=inputs, outputs=graph, clone=True)
     # We need to add a Supervisor to the fgraph to be able to run the
     # JAX sequential optimizer without warnings. We made sure there
     # are no mutable input variables, so we only need to check for
     # "destroyers". This should be automatically handled by PyTensor
-    # once https://github.com/pytensor-devs/pytensor/issues/637 is fixed.
+    # once https://github.com/aesara-devs/aesara/issues/637 is fixed.
     fgraph.attach_feature(
         Supervisor(
             input
             for input in fgraph.inputs
             if not (hasattr(fgraph, "destroyers") and fgraph.has_destroyers([input]))
         )
     )
```

### Comparing `pymc-5.6.0/pymc/sampling/mcmc.py` & `pymc-5.6.1/pymc/sampling/mcmc.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.0/pymc/sampling/parallel.py` & `pymc-5.6.1/pymc/sampling/parallel.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.0/pymc/sampling/population.py` & `pymc-5.6.1/pymc/sampling/population.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.0/pymc/sampling_jax.py` & `pymc-5.6.1/pymc/sampling_jax.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.0/pymc/smc/__init__.py` & `pymc-5.6.1/pymc/smc/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.0/pymc/smc/kernels.py` & `pymc-5.6.1/pymc/smc/kernels.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.0/pymc/smc/sampling.py` & `pymc-5.6.1/pymc/smc/sampling.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.0/pymc/stats/__init__.py` & `pymc-5.6.1/pymc/stats/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.0/pymc/stats/convergence.py` & `pymc-5.6.1/pymc/stats/convergence.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.0/pymc/stats/log_likelihood.py` & `pymc-5.6.1/pymc/stats/log_likelihood.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.0/pymc/step_methods/__init__.py` & `pymc-5.6.1/pymc/step_methods/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.0/pymc/step_methods/arraystep.py` & `pymc-5.6.1/pymc/step_methods/arraystep.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.0/pymc/step_methods/compound.py` & `pymc-5.6.1/pymc/step_methods/compound.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.0/pymc/step_methods/hmc/__init__.py` & `pymc-5.6.1/pymc/step_methods/hmc/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.0/pymc/step_methods/hmc/base_hmc.py` & `pymc-5.6.1/pymc/step_methods/hmc/base_hmc.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.0/pymc/step_methods/hmc/hmc.py` & `pymc-5.6.1/pymc/step_methods/hmc/hmc.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.0/pymc/step_methods/hmc/integration.py` & `pymc-5.6.1/pymc/step_methods/hmc/integration.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.0/pymc/step_methods/hmc/nuts.py` & `pymc-5.6.1/pymc/step_methods/hmc/nuts.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.0/pymc/step_methods/hmc/quadpotential.py` & `pymc-5.6.1/pymc/step_methods/hmc/quadpotential.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.0/pymc/step_methods/metropolis.py` & `pymc-5.6.1/pymc/step_methods/metropolis.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.0/pymc/step_methods/slicer.py` & `pymc-5.6.1/pymc/step_methods/slicer.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.0/pymc/step_methods/step_sizes.py` & `pymc-5.6.1/pymc/step_methods/step_sizes.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.0/pymc/testing.py` & `pymc-5.6.1/pymc/testing.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.0/pymc/tuning/__init__.py` & `pymc-5.6.1/pymc/tuning/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.0/pymc/tuning/scaling.py` & `pymc-5.6.1/pymc/tuning/scaling.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.0/pymc/tuning/starting.py` & `pymc-5.6.1/pymc/tuning/starting.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.0/pymc/util.py` & `pymc-5.6.1/pymc/util.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.0/pymc/variational/__init__.py` & `pymc-5.6.1/pymc/variational/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.0/pymc/variational/approximations.py` & `pymc-5.6.1/pymc/variational/approximations.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.0/pymc/variational/callbacks.py` & `pymc-5.6.1/pymc/variational/callbacks.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.0/pymc/variational/inference.py` & `pymc-5.6.1/pymc/variational/inference.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.0/pymc/variational/minibatch_rv.py` & `pymc-5.6.1/pymc/variational/minibatch_rv.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.0/pymc/variational/operators.py` & `pymc-5.6.1/pymc/variational/operators.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.0/pymc/variational/opvi.py` & `pymc-5.6.1/pymc/variational/opvi.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.0/pymc/variational/stein.py` & `pymc-5.6.1/pymc/variational/stein.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.0/pymc/variational/test_functions.py` & `pymc-5.6.1/pymc/variational/test_functions.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.0/pymc/variational/updates.py` & `pymc-5.6.1/pymc/variational/updates.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.0/pymc/vartypes.py` & `pymc-5.6.1/pymc/vartypes.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.0/pymc.egg-info/PKG-INFO` & `pymc-5.6.1/pymc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymc
-Version: 5.6.0
+Version: 5.6.1
 Summary: Probabilistic Programming in Python: Bayesian Modeling and Probabilistic Machine Learning with PyTensor
 Home-page: http://github.com/pymc-devs/pymc
 Maintainer: PyMC Developers
 Maintainer-email: pymc.devs@gmail.com
 License: Apache License, Version 2.0
 Description: .. image:: https://cdn.rawgit.com/pymc-devs/pymc/main/docs/logos/svg/PyMC_banner.svg
             :height: 100px
```

### Comparing `pymc-5.6.0/pymc.egg-info/SOURCES.txt` & `pymc-5.6.1/pymc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pymc-5.6.0/scripts/docker_container.sh` & `pymc-5.6.1/scripts/docker_container.sh`

 * *Files identical despite different names*

### Comparing `pymc-5.6.0/setup.py` & `pymc-5.6.1/setup.py`

 * *Files identical despite different names*

### Comparing `pymc-5.6.0/versioneer.py` & `pymc-5.6.1/versioneer.py`

 * *Files identical despite different names*

