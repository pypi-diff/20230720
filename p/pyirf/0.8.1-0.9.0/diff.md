# Comparing `tmp/pyirf-0.8.1.tar.gz` & `tmp/pyirf-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyirf-0.8.1.tar", last modified: Thu Mar 16 13:57:14 2023, max compression
+gzip compressed data, was "pyirf-0.9.0.tar", last modified: Thu Jul 20 12:03:52 2023, max compression
```

## Comparing `pyirf-0.8.1.tar` & `pyirf-0.9.0.tar`

### file list

```diff
@@ -1,131 +1,142 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:57:14.278235 pyirf-0.8.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:57:14.258235 pyirf-0.8.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-03-16 13:57:08.000000 pyirf-0.8.1/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:57:14.258235 pyirf-0.8.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-03-16 13:57:08.000000 pyirf-0.8.1/.github/workflows/changelog.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-03-16 13:57:08.000000 pyirf-0.8.1/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-03-16 13:57:08.000000 pyirf-0.8.1/.github/workflows/deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-03-16 13:57:08.000000 pyirf-0.8.1/.github/workflows/release-drafter.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-03-16 13:57:08.000000 pyirf-0.8.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-03-16 13:57:08.000000 pyirf-0.8.1/.mailmap
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-16 13:57:08.000000 pyirf-0.8.1/.prospector.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-03-16 13:57:08.000000 pyirf-0.8.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-03-16 13:57:08.000000 pyirf-0.8.1/.zenodo.json
--rw-r--r--   0 runner    (1001) docker     (123)    11481 2023-03-16 13:57:08.000000 pyirf-0.8.1/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-03-16 13:57:08.000000 pyirf-0.8.1/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-03-16 13:57:08.000000 pyirf-0.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-03-16 13:57:08.000000 pyirf-0.8.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-03-16 13:57:14.278235 pyirf-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-03-16 13:57:08.000000 pyirf-0.8.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:57:14.262235 pyirf-0.8.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-03-16 13:57:08.000000 pyirf-0.8.1/docs/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-03-16 13:57:08.000000 pyirf-0.8.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:57:14.262235 pyirf-0.8.1/docs/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-03-16 13:57:08.000000 pyirf-0.8.1/docs/benchmarks/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-03-16 13:57:08.000000 pyirf-0.8.1/docs/binning.rst
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-03-16 13:57:08.000000 pyirf-0.8.1/docs/changelog.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:57:14.262235 pyirf-0.8.1/docs/changes/
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-03-16 13:57:08.000000 pyirf-0.8.1/docs/changes/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-03-16 13:57:08.000000 pyirf-0.8.1/docs/changes/template.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-03-16 13:57:08.000000 pyirf-0.8.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     4962 2023-03-16 13:57:08.000000 pyirf-0.8.1/docs/contribute.rst
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-03-16 13:57:08.000000 pyirf-0.8.1/docs/cut_optimization.rst
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-03-16 13:57:08.000000 pyirf-0.8.1/docs/cuts.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-03-16 13:57:08.000000 pyirf-0.8.1/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-03-16 13:57:08.000000 pyirf-0.8.1/docs/gammapy.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-03-16 13:57:08.000000 pyirf-0.8.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-03-16 13:57:08.000000 pyirf-0.8.1/docs/install.rst
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-03-16 13:57:08.000000 pyirf-0.8.1/docs/interpolation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5120 2023-03-16 13:57:08.000000 pyirf-0.8.1/docs/introduction.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:57:14.262235 pyirf-0.8.1/docs/io/
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-03-16 13:57:08.000000 pyirf-0.8.1/docs/io/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:57:14.262235 pyirf-0.8.1/docs/irf/
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-03-16 13:57:08.000000 pyirf-0.8.1/docs/irf/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:57:14.262235 pyirf-0.8.1/docs/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)    14217 2023-03-16 13:57:08.000000 pyirf-0.8.1/docs/notebooks/fact_example.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-03-16 13:57:08.000000 pyirf-0.8.1/docs/notebooks/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-03-16 13:57:08.000000 pyirf-0.8.1/docs/sensitivity.rst
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-03-16 13:57:08.000000 pyirf-0.8.1/docs/simulation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-03-16 13:57:08.000000 pyirf-0.8.1/docs/spectral.rst
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-03-16 13:57:08.000000 pyirf-0.8.1/docs/statistics.rst
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-03-16 13:57:08.000000 pyirf-0.8.1/docs/utils.rst
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-03-16 13:57:08.000000 pyirf-0.8.1/download_irfs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      394 2023-03-16 13:57:08.000000 pyirf-0.8.1/download_private_data.sh
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-03-16 13:57:08.000000 pyirf-0.8.1/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:57:14.266235 pyirf-0.8.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     9717 2023-03-16 13:57:08.000000 pyirf-0.8.1/examples/calculate_eventdisplay_irfs.py
--rw-r--r--   0 runner    (1001) docker     (123)    19809 2023-03-16 13:57:08.000000 pyirf-0.8.1/examples/comparison_with_EventDisplay.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-03-16 13:57:08.000000 pyirf-0.8.1/examples/plot_spectra.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:57:14.266235 pyirf-0.8.1/pyirf/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-03-16 13:57:08.000000 pyirf-0.8.1/pyirf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-03-16 13:57:14.000000 pyirf-0.8.1/pyirf/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:57:14.270235 pyirf-0.8.1/pyirf/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-03-16 13:57:08.000000 pyirf-0.8.1/pyirf/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-03-16 13:57:08.000000 pyirf-0.8.1/pyirf/benchmarks/angular_resolution.py
--rw-r--r--   0 runner    (1001) docker     (123)     4803 2023-03-16 13:57:08.000000 pyirf-0.8.1/pyirf/benchmarks/energy_bias_resolution.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:57:14.270235 pyirf-0.8.1/pyirf/benchmarks/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 13:57:08.000000 pyirf-0.8.1/pyirf/benchmarks/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-03-16 13:57:08.000000 pyirf-0.8.1/pyirf/benchmarks/tests/test_angular_resolution.py
--rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-03-16 13:57:08.000000 pyirf-0.8.1/pyirf/benchmarks/tests/test_bias_resolution.py
--rw-r--r--   0 runner    (1001) docker     (123)     8378 2023-03-16 13:57:08.000000 pyirf-0.8.1/pyirf/binning.py
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-03-16 13:57:08.000000 pyirf-0.8.1/pyirf/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5657 2023-03-16 13:57:08.000000 pyirf-0.8.1/pyirf/cut_optimization.py
--rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-03-16 13:57:08.000000 pyirf-0.8.1/pyirf/cuts.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-03-16 13:57:08.000000 pyirf-0.8.1/pyirf/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-03-16 13:57:08.000000 pyirf-0.8.1/pyirf/gammapy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:57:14.270235 pyirf-0.8.1/pyirf/interpolation/
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-03-16 13:57:08.000000 pyirf-0.8.1/pyirf/interpolation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8869 2023-03-16 13:57:08.000000 pyirf-0.8.1/pyirf/interpolation/base_interpolators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-03-16 13:57:08.000000 pyirf-0.8.1/pyirf/interpolation/griddata_interpolator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6898 2023-03-16 13:57:08.000000 pyirf-0.8.1/pyirf/interpolation/interpolate_irfs.py
--rw-r--r--   0 runner    (1001) docker     (123)     9271 2023-03-16 13:57:08.000000 pyirf-0.8.1/pyirf/interpolation/quantile_interpolator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:57:14.270235 pyirf-0.8.1/pyirf/interpolation/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7949 2023-03-16 13:57:08.000000 pyirf-0.8.1/pyirf/interpolation/tests/test_base_interpolators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-03-16 13:57:08.000000 pyirf-0.8.1/pyirf/interpolation/tests/test_griddata_interpolator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4960 2023-03-16 13:57:08.000000 pyirf-0.8.1/pyirf/interpolation/tests/test_interpolate_irfs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3892 2023-03-16 13:57:08.000000 pyirf-0.8.1/pyirf/interpolation/tests/test_quantile_interpolator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:57:14.274235 pyirf-0.8.1/pyirf/io/
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-03-16 13:57:08.000000 pyirf-0.8.1/pyirf/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-03-16 13:57:08.000000 pyirf-0.8.1/pyirf/io/eventdisplay.py
--rw-r--r--   0 runner    (1001) docker     (123)    10793 2023-03-16 13:57:08.000000 pyirf-0.8.1/pyirf/io/gadf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:57:14.274235 pyirf-0.8.1/pyirf/io/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 13:57:08.000000 pyirf-0.8.1/pyirf/io/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4770 2023-03-16 13:57:08.000000 pyirf-0.8.1/pyirf/io/tests/test_gadf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:57:14.274235 pyirf-0.8.1/pyirf/irf/
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-03-16 13:57:08.000000 pyirf-0.8.1/pyirf/irf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-03-16 13:57:08.000000 pyirf-0.8.1/pyirf/irf/background.py
--rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-03-16 13:57:08.000000 pyirf-0.8.1/pyirf/irf/effective_area.py
--rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-03-16 13:57:08.000000 pyirf-0.8.1/pyirf/irf/energy_dispersion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-03-16 13:57:08.000000 pyirf-0.8.1/pyirf/irf/psf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:57:14.274235 pyirf-0.8.1/pyirf/irf/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-03-16 13:57:08.000000 pyirf-0.8.1/pyirf/irf/tests/test_background.py
--rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-03-16 13:57:08.000000 pyirf-0.8.1/pyirf/irf/tests/test_effective_area.py
--rw-r--r--   0 runner    (1001) docker     (123)     6157 2023-03-16 13:57:08.000000 pyirf-0.8.1/pyirf/irf/tests/test_energy_dispersion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-03-16 13:57:08.000000 pyirf-0.8.1/pyirf/irf/tests/test_psf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:57:14.274235 pyirf-0.8.1/pyirf/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-03-16 13:57:08.000000 pyirf-0.8.1/pyirf/resources/dampe_p+he.ecsv
--rw-r--r--   0 runner    (1001) docker     (123)    12057 2023-03-16 13:57:08.000000 pyirf-0.8.1/pyirf/sensitivity.py
--rw-r--r--   0 runner    (1001) docker     (123)     7312 2023-03-16 13:57:08.000000 pyirf-0.8.1/pyirf/simulations.py
--rw-r--r--   0 runner    (1001) docker     (123)    12621 2023-03-16 13:57:08.000000 pyirf-0.8.1/pyirf/spectral.py
--rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-03-16 13:57:08.000000 pyirf-0.8.1/pyirf/statistics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:57:14.278235 pyirf-0.8.1/pyirf/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 13:57:08.000000 pyirf-0.8.1/pyirf/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7263 2023-03-16 13:57:08.000000 pyirf-0.8.1/pyirf/tests/test_binning.py
--rw-r--r--   0 runner    (1001) docker     (123)     4897 2023-03-16 13:57:08.000000 pyirf-0.8.1/pyirf/tests/test_cuts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-03-16 13:57:08.000000 pyirf-0.8.1/pyirf/tests/test_gammapy_interop.py
--rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-03-16 13:57:08.000000 pyirf-0.8.1/pyirf/tests/test_sensitivity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-03-16 13:57:08.000000 pyirf-0.8.1/pyirf/tests/test_simulations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-03-16 13:57:08.000000 pyirf-0.8.1/pyirf/tests/test_spectral.py
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-03-16 13:57:08.000000 pyirf-0.8.1/pyirf/tests/test_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-03-16 13:57:08.000000 pyirf-0.8.1/pyirf/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4551 2023-03-16 13:57:08.000000 pyirf-0.8.1/pyirf/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-03-16 13:57:08.000000 pyirf-0.8.1/pyirf/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 13:57:14.270235 pyirf-0.8.1/pyirf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-03-16 13:57:14.000000 pyirf-0.8.1/pyirf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-03-16 13:57:14.000000 pyirf-0.8.1/pyirf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-16 13:57:14.000000 pyirf-0.8.1/pyirf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-03-16 13:57:14.000000 pyirf-0.8.1/pyirf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-16 13:57:14.000000 pyirf-0.8.1/pyirf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-03-16 13:57:08.000000 pyirf-0.8.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-03-16 13:57:14.278235 pyirf-0.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-03-16 13:57:08.000000 pyirf-0.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:03:52.183626 pyirf-0.9.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:03:52.175626 pyirf-0.9.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-20 12:03:46.000000 pyirf-0.9.0/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:03:52.175626 pyirf-0.9.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-20 12:03:46.000000 pyirf-0.9.0/.github/workflows/changelog.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-07-20 12:03:46.000000 pyirf-0.9.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-07-20 12:03:46.000000 pyirf-0.9.0/.github/workflows/deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-20 12:03:46.000000 pyirf-0.9.0/.github/workflows/release-drafter.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-07-20 12:03:46.000000 pyirf-0.9.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-07-20 12:03:46.000000 pyirf-0.9.0/.mailmap
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-20 12:03:46.000000 pyirf-0.9.0/.prospector.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-20 12:03:46.000000 pyirf-0.9.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-07-20 12:03:46.000000 pyirf-0.9.0/.zenodo.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13643 2023-07-20 12:03:46.000000 pyirf-0.9.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-07-20 12:03:46.000000 pyirf-0.9.0/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-07-20 12:03:46.000000 pyirf-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-20 12:03:46.000000 pyirf-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-07-20 12:03:52.187626 pyirf-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-07-20 12:03:46.000000 pyirf-0.9.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:03:52.175626 pyirf-0.9.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-07-20 12:03:46.000000 pyirf-0.9.0/docs/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-20 12:03:46.000000 pyirf-0.9.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:03:52.175626 pyirf-0.9.0/docs/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-20 12:03:46.000000 pyirf-0.9.0/docs/benchmarks/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-20 12:03:46.000000 pyirf-0.9.0/docs/binning.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-20 12:03:46.000000 pyirf-0.9.0/docs/changelog.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:03:52.175626 pyirf-0.9.0/docs/changes/
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-20 12:03:46.000000 pyirf-0.9.0/docs/changes/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-07-20 12:03:46.000000 pyirf-0.9.0/docs/changes/template.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-07-20 12:03:46.000000 pyirf-0.9.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4962 2023-07-20 12:03:46.000000 pyirf-0.9.0/docs/contribute.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-20 12:03:46.000000 pyirf-0.9.0/docs/cut_optimization.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-20 12:03:46.000000 pyirf-0.9.0/docs/cuts.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-07-20 12:03:46.000000 pyirf-0.9.0/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-20 12:03:46.000000 pyirf-0.9.0/docs/gammapy.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-07-20 12:03:46.000000 pyirf-0.9.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-07-20 12:03:46.000000 pyirf-0.9.0/docs/install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-07-20 12:03:46.000000 pyirf-0.9.0/docs/interpolation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5120 2023-07-20 12:03:46.000000 pyirf-0.9.0/docs/introduction.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:03:52.175626 pyirf-0.9.0/docs/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-07-20 12:03:46.000000 pyirf-0.9.0/docs/io/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:03:52.175626 pyirf-0.9.0/docs/irf/
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-07-20 12:03:46.000000 pyirf-0.9.0/docs/irf/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:03:52.175626 pyirf-0.9.0/docs/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)    14217 2023-07-20 12:03:46.000000 pyirf-0.9.0/docs/notebooks/fact_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-20 12:03:46.000000 pyirf-0.9.0/docs/notebooks/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-20 12:03:46.000000 pyirf-0.9.0/docs/sensitivity.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-20 12:03:46.000000 pyirf-0.9.0/docs/simulation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-20 12:03:46.000000 pyirf-0.9.0/docs/spectral.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-20 12:03:46.000000 pyirf-0.9.0/docs/statistics.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-20 12:03:46.000000 pyirf-0.9.0/docs/utils.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-07-20 12:03:46.000000 pyirf-0.9.0/download_irfs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      394 2023-07-20 12:03:46.000000 pyirf-0.9.0/download_private_data.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-20 12:03:46.000000 pyirf-0.9.0/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:03:52.179626 pyirf-0.9.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     9717 2023-07-20 12:03:46.000000 pyirf-0.9.0/examples/calculate_eventdisplay_irfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19809 2023-07-20 12:03:46.000000 pyirf-0.9.0/examples/comparison_with_EventDisplay.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-07-20 12:03:46.000000 pyirf-0.9.0/examples/plot_spectra.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:03:52.179626 pyirf-0.9.0/pyirf/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-20 12:03:46.000000 pyirf-0.9.0/pyirf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-20 12:03:52.000000 pyirf-0.9.0/pyirf/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:03:52.179626 pyirf-0.9.0/pyirf/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-20 12:03:46.000000 pyirf-0.9.0/pyirf/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-07-20 12:03:46.000000 pyirf-0.9.0/pyirf/benchmarks/angular_resolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4806 2023-07-20 12:03:46.000000 pyirf-0.9.0/pyirf/benchmarks/energy_bias_resolution.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:03:52.179626 pyirf-0.9.0/pyirf/benchmarks/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 12:03:46.000000 pyirf-0.9.0/pyirf/benchmarks/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-07-20 12:03:46.000000 pyirf-0.9.0/pyirf/benchmarks/tests/test_angular_resolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-07-20 12:03:46.000000 pyirf-0.9.0/pyirf/benchmarks/tests/test_bias_resolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8378 2023-07-20 12:03:46.000000 pyirf-0.9.0/pyirf/binning.py
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-07-20 12:03:46.000000 pyirf-0.9.0/pyirf/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5657 2023-07-20 12:03:46.000000 pyirf-0.9.0/pyirf/cut_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-07-20 12:03:46.000000 pyirf-0.9.0/pyirf/cuts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-20 12:03:46.000000 pyirf-0.9.0/pyirf/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-07-20 12:03:46.000000 pyirf-0.9.0/pyirf/gammapy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:03:52.183626 pyirf-0.9.0/pyirf/interpolation/
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-07-20 12:03:46.000000 pyirf-0.9.0/pyirf/interpolation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-07-20 12:03:46.000000 pyirf-0.9.0/pyirf/interpolation/base_extrapolators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-07-20 12:03:46.000000 pyirf-0.9.0/pyirf/interpolation/base_interpolators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27675 2023-07-20 12:03:46.000000 pyirf-0.9.0/pyirf/interpolation/component_estimators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-07-20 12:03:46.000000 pyirf-0.9.0/pyirf/interpolation/griddata_interpolator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12592 2023-07-20 12:03:46.000000 pyirf-0.9.0/pyirf/interpolation/moment_morph_interpolator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5777 2023-07-20 12:03:46.000000 pyirf-0.9.0/pyirf/interpolation/nearest_neighbor_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8561 2023-07-20 12:03:46.000000 pyirf-0.9.0/pyirf/interpolation/nearest_simplex_extrapolator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8756 2023-07-20 12:03:46.000000 pyirf-0.9.0/pyirf/interpolation/quantile_interpolator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:03:52.183626 pyirf-0.9.0/pyirf/interpolation/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-07-20 12:03:46.000000 pyirf-0.9.0/pyirf/interpolation/tests/test_base_extrapolators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-07-20 12:03:46.000000 pyirf-0.9.0/pyirf/interpolation/tests/test_base_interpolators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16912 2023-07-20 12:03:46.000000 pyirf-0.9.0/pyirf/interpolation/tests/test_component_estimator_base_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5905 2023-07-20 12:03:46.000000 pyirf-0.9.0/pyirf/interpolation/tests/test_component_estimator_specific_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-07-20 12:03:46.000000 pyirf-0.9.0/pyirf/interpolation/tests/test_griddata_interpolator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18555 2023-07-20 12:03:46.000000 pyirf-0.9.0/pyirf/interpolation/tests/test_moment_morph_interpolator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-07-20 12:03:46.000000 pyirf-0.9.0/pyirf/interpolation/tests/test_nearest_neighbor_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11444 2023-07-20 12:03:46.000000 pyirf-0.9.0/pyirf/interpolation/tests/test_nearest_simplex_extrapolator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-07-20 12:03:46.000000 pyirf-0.9.0/pyirf/interpolation/tests/test_quantile_interpolator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5714 2023-07-20 12:03:46.000000 pyirf-0.9.0/pyirf/interpolation/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5998 2023-07-20 12:03:46.000000 pyirf-0.9.0/pyirf/interpolation/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:03:52.183626 pyirf-0.9.0/pyirf/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-20 12:03:46.000000 pyirf-0.9.0/pyirf/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-07-20 12:03:46.000000 pyirf-0.9.0/pyirf/io/eventdisplay.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10793 2023-07-20 12:03:46.000000 pyirf-0.9.0/pyirf/io/gadf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:03:52.183626 pyirf-0.9.0/pyirf/io/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 12:03:46.000000 pyirf-0.9.0/pyirf/io/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4770 2023-07-20 12:03:46.000000 pyirf-0.9.0/pyirf/io/tests/test_gadf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:03:52.183626 pyirf-0.9.0/pyirf/irf/
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-20 12:03:46.000000 pyirf-0.9.0/pyirf/irf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-07-20 12:03:46.000000 pyirf-0.9.0/pyirf/irf/background.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-07-20 12:03:46.000000 pyirf-0.9.0/pyirf/irf/effective_area.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-07-20 12:03:46.000000 pyirf-0.9.0/pyirf/irf/energy_dispersion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-07-20 12:03:46.000000 pyirf-0.9.0/pyirf/irf/psf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:03:52.183626 pyirf-0.9.0/pyirf/irf/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-07-20 12:03:46.000000 pyirf-0.9.0/pyirf/irf/tests/test_background.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-07-20 12:03:46.000000 pyirf-0.9.0/pyirf/irf/tests/test_effective_area.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6157 2023-07-20 12:03:46.000000 pyirf-0.9.0/pyirf/irf/tests/test_energy_dispersion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-07-20 12:03:46.000000 pyirf-0.9.0/pyirf/irf/tests/test_psf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:03:52.183626 pyirf-0.9.0/pyirf/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-07-20 12:03:46.000000 pyirf-0.9.0/pyirf/resources/dampe_p+he.ecsv
+-rw-r--r--   0 runner    (1001) docker     (123)    11982 2023-07-20 12:03:46.000000 pyirf-0.9.0/pyirf/sensitivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7312 2023-07-20 12:03:46.000000 pyirf-0.9.0/pyirf/simulations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12704 2023-07-20 12:03:46.000000 pyirf-0.9.0/pyirf/spectral.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-07-20 12:03:46.000000 pyirf-0.9.0/pyirf/statistics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:03:52.183626 pyirf-0.9.0/pyirf/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 12:03:46.000000 pyirf-0.9.0/pyirf/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7263 2023-07-20 12:03:46.000000 pyirf-0.9.0/pyirf/tests/test_binning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4897 2023-07-20 12:03:46.000000 pyirf-0.9.0/pyirf/tests/test_cuts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-07-20 12:03:46.000000 pyirf-0.9.0/pyirf/tests/test_gammapy_interop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-07-20 12:03:46.000000 pyirf-0.9.0/pyirf/tests/test_sensitivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-07-20 12:03:46.000000 pyirf-0.9.0/pyirf/tests/test_simulations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-07-20 12:03:46.000000 pyirf-0.9.0/pyirf/tests/test_spectral.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-07-20 12:03:46.000000 pyirf-0.9.0/pyirf/tests/test_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-07-20 12:03:46.000000 pyirf-0.9.0/pyirf/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4551 2023-07-20 12:03:46.000000 pyirf-0.9.0/pyirf/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-07-20 12:03:46.000000 pyirf-0.9.0/pyirf/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:03:52.179626 pyirf-0.9.0/pyirf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-07-20 12:03:52.000000 pyirf-0.9.0/pyirf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-07-20 12:03:52.000000 pyirf-0.9.0/pyirf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 12:03:52.000000 pyirf-0.9.0/pyirf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-20 12:03:52.000000 pyirf-0.9.0/pyirf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-20 12:03:52.000000 pyirf-0.9.0/pyirf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-07-20 12:03:46.000000 pyirf-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-07-20 12:03:52.187626 pyirf-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-07-20 12:03:46.000000 pyirf-0.9.0/setup.py
```

### Comparing `pyirf-0.8.1/.github/workflows/changelog.yml` & `pyirf-0.9.0/.github/workflows/changelog.yml`

 * *Files identical despite different names*

### Comparing `pyirf-0.8.1/.github/workflows/ci.yml` & `pyirf-0.9.0/.github/workflows/ci.yml`

 * *Files 15% similar despite different names*

```diff
@@ -14,32 +14,32 @@
   GITHUB_PR_NUMBER: ${{ github.event.number }}
 
 jobs:
   tests:
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: ["3.8", "3.9", "3.10"]
+        python-version: ["3.9", "3.10", "3.11"]
 
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v3
         with:
           fetch-depth: 0
 
       - uses: actions/cache@v3 
         id: cache-irfs
         with:
           path: ./irfs
           key: irf-cache
 
       # make sure we have version info
       - run: git fetch --tags
 
       - name: Set up Python ${{ matrix.python-version }}
-        uses: actions/setup-python@v2
+        uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
 
       - name: Install dependencies
         run: |
           python --version
           pip install -U pip setuptools wheel restructuredtext_lint
@@ -54,27 +54,27 @@
         if: steps.cache-irfs.outputs.cache-hit != 'true'
         run: python download_irfs.py
 
       - name: Tests
         run: |
           pytest --cov=pyirf --cov-report=xml
 
-      - uses: codecov/codecov-action@v1
+      - uses: codecov/codecov-action@v3
 
   docs:
     runs-on: ubuntu-latest
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v3
         with:
           fetch-depth: 0
 
       - name: Set up Python
-        uses: actions/setup-python@v2
+        uses: actions/setup-python@v4
         with:
-          python-version: 3.8
+          python-version: 3.9
 
       - name: Install doc dependencies
         run: |
           sudo apt update --yes && sudo apt install --yes git build-essential pandoc curl graphviz
           pip install -U pip setuptools wheel towncrier
           pip install -e .[docs]
           git describe --tags
```

### Comparing `pyirf-0.8.1/.github/workflows/deploy.yml` & `pyirf-0.9.0/.github/workflows/deploy.yml`

 * *Files 15% similar despite different names*

```diff
@@ -5,23 +5,23 @@
     tags:
       - 'v*'
 
 jobs:
   deploy:
     runs-on: ubuntu-latest
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v3
         with:
           fetch-depth: 0
 
 
       - name: Set up Python
-        uses: actions/setup-python@v2
+        uses: actions/setup-python@v4
         with:
-          python-version: 3.8
+          python-version: 3.9
 
       - name: Install dependencies
         run: |
           python --version
           pip install -U pip setuptools wheel setuptools_scm[toml]
           # make sure we have the version, grep will exit with 1 if it finds 0.0.0
           python setup.py --version | grep -v '0.0.0'
```

### Comparing `pyirf-0.8.1/.gitignore` & `pyirf-0.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pyirf-0.8.1/.mailmap` & `pyirf-0.9.0/.mailmap`

 * *Files identical despite different names*

### Comparing `pyirf-0.8.1/.zenodo.json` & `pyirf-0.9.0/.zenodo.json`

 * *Files identical despite different names*

### Comparing `pyirf-0.8.1/CHANGES.rst` & `pyirf-0.9.0/CHANGES.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,59 @@
+pyirf 0.9.0 (2023-07-19)
+========================
+
+
+API Changes
+-----------
+
+- Change the interpolation API to top-level estimator classes that instantiate
+  inter- and extrapolator objects. Drops the ``interpolate_xyz`` functions
+  originally used to interpolate a xyz IRF component in favour of a ``XYZEstimator``
+  class. Moves data checks from intepolator to estimator classes.
+
+  Direct usage of interpolator objects is now discuraged, use estimator objects instead. [`#228 <https://github.com/cta-observatory/pyirf/pull/228>`__]
+
+
+Bug Fixes
+---------
+
+- Correctly fill n_events in ``angular_resolution``, was always 0 before. [`#231 <https://github.com/cta-observatory/pyirf/pull/231>`__]
+
+- Remove condition that relative sensitivity must be > 1.
+  This condition was added by error and resulted in returning
+  nan if the flux needed to fulfill the conditions is larger than
+  the reference flux used to weight the events. [`#241 <https://github.com/cta-observatory/pyirf/pull/241>`__]
+
+
+New Features
+------------
+
+- Add moment morphing as second interpolation method able to handle discretized PDF 
+  components of IRFs. [`#229 <https://github.com/cta-observatory/pyirf/pull/229>`__]
+
+- Add a base structure for extrapolators similar to the interpolation case
+  as well as a first extrapolator for parametrized components, extrapolating from the
+  nearest simplex in one or two dimensions. [`#236 <https://github.com/cta-observatory/pyirf/pull/236>`__]
+
+- Add an extrapolator for discretized PDF components, extrapolating from the
+  nearest simplex in one or two dimensions utilizing the same approach moment morphing
+  interpolation uses. [`#237 <https://github.com/cta-observatory/pyirf/pull/237>`__]
+
+- Add a ``DiscretePDFNearestNeighborSearcher`` and a ``ParametrizedNearestNeighborSearcher`` to support nearest neighbor approaches 
+  as alternatives to inter-/ and extrapolation [`#232 <https://github.com/cta-observatory/pyirf/pull/232>`__]
+
+
+
+Maintenance
+-----------
+
+- Drop python 3.8 support in accordance with `NEP 29 <https://numpy.org/neps/nep-0029-deprecation_policy.html>`_ [`#243 <https://github.com/cta-observatory/pyirf/pull/243>`__]
+
+
+
 pyirf 0.8.1 (2023-03-16)
 ========================
 
 
 New Features
 ------------
```

### Comparing `pyirf-0.8.1/CODEOWNERS` & `pyirf-0.9.0/CODEOWNERS`

 * *Files 12% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 # These owners will be the default owners for everything in
 # the repo. Unless a later match takes precedence,
 # @global-owner1 and @global-owner2 will be requested for
 # review when someone opens a pull request.
 # *       @global-owner1 @global-owner2
 * @maxnoe @HealthyPear
 
+pyirf/interpolation/* @RuneDominik
+
 # Order is important; the last matching pattern takes the most
 # precedence. When someone opens a pull request that only
 # modifies JS files, only @js-owner and not the global
 # owner(s) will be requested for a review.
 # *.js    @js-owner
 
 # You can also use email addresses if you prefer. They'll be
```

### Comparing `pyirf-0.8.1/LICENSE` & `pyirf-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyirf-0.8.1/PKG-INFO` & `pyirf-0.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 Metadata-Version: 2.1
 Name: pyirf
-Version: 0.8.1
+Version: 0.9.0
 Summary: A python library to calculate IACT IRFs and Sensitivities
 Home-page: https://github.com/cta-observatory/pyirf
 Author: CTA Consortium, Analysis and Simulation Working Group
-Author-email: maximilian.noethe@tu-dortmund.de
+Author-email: maximilian.linhoff@tu-dortmund.de
 License: MIT
 Project-URL: Bug Tracker, https://github.com/cta-observatory/pyirf/issues
 Project-URL: Documentation, https://cta-observatory.github.io/pyirf
 Project-URL: Source Code, https://github.com/cta-observatory/pyirf
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.9
 Provides-Extra: docs
 Provides-Extra: tests
 Provides-Extra: gammapy
 Provides-Extra: dev
 Provides-Extra: all
 License-File: LICENSE
 
 ==========================================
 pyirf |ci| |codacy| |coverage| |doilatest|
 ==========================================
 
-.. |ci| image:: https://github.com/cta-observatory/pyirf/workflows/CI/badge.svg?branch=master
-  :target: https://github.com/cta-observatory/pyirf/actions?query=workflow%3ACI+branch%3Amaster
+.. |ci| image:: https://github.com/cta-observatory/pyirf/workflows/CI/badge.svg?branch=main
+  :target: https://github.com/cta-observatory/pyirf/actions?query=workflow%3ACI+branch%3Amain
 .. |codacy| image:: https://app.codacy.com/project/badge/Grade/669fef80d3d54070960e66351477e383
   :target: https://www.codacy.com/gh/cta-observatory/pyirf/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=cta-observatory/pyirf&amp;utm_campaign=Badge_Grade
-.. |coverage| image:: https://codecov.io/gh/cta-observatory/pyirf/branch/master/graph/badge.svg
+.. |coverage| image:: https://codecov.io/gh/cta-observatory/pyirf/branch/main/graph/badge.svg
   :target: https://codecov.io/gh/cta-observatory/pyirf
 .. |doilatest| image:: https://zenodo.org/badge/DOI/10.5281/zenodo.4740755.svg
   :target: https://doi.org/10.5281/zenodo.4740755
 
 *pyirf* is a python library for the generation of Instrument Response
 Functions (IRFs) and sensitivities for the
 `Cherenkov Telescope Array (CTA) <https://www.cta-observatory.org/>`_ .
```

### Comparing `pyirf-0.8.1/README.rst` & `pyirf-0.9.0/README.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 ==========================================
 pyirf |ci| |codacy| |coverage| |doilatest|
 ==========================================
 
-.. |ci| image:: https://github.com/cta-observatory/pyirf/workflows/CI/badge.svg?branch=master
-  :target: https://github.com/cta-observatory/pyirf/actions?query=workflow%3ACI+branch%3Amaster
+.. |ci| image:: https://github.com/cta-observatory/pyirf/workflows/CI/badge.svg?branch=main
+  :target: https://github.com/cta-observatory/pyirf/actions?query=workflow%3ACI+branch%3Amain
 .. |codacy| image:: https://app.codacy.com/project/badge/Grade/669fef80d3d54070960e66351477e383
   :target: https://www.codacy.com/gh/cta-observatory/pyirf/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=cta-observatory/pyirf&amp;utm_campaign=Badge_Grade
-.. |coverage| image:: https://codecov.io/gh/cta-observatory/pyirf/branch/master/graph/badge.svg
+.. |coverage| image:: https://codecov.io/gh/cta-observatory/pyirf/branch/main/graph/badge.svg
   :target: https://codecov.io/gh/cta-observatory/pyirf
 .. |doilatest| image:: https://zenodo.org/badge/DOI/10.5281/zenodo.4740755.svg
   :target: https://doi.org/10.5281/zenodo.4740755
 
 *pyirf* is a python library for the generation of Instrument Response
 Functions (IRFs) and sensitivities for the
 `Cherenkov Telescope Array (CTA) <https://www.cta-observatory.org/>`_ .
```

### Comparing `pyirf-0.8.1/docs/AUTHORS.rst` & `pyirf-0.9.0/docs/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `pyirf-0.8.1/docs/Makefile` & `pyirf-0.9.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyirf-0.8.1/docs/changes/README.md` & `pyirf-0.9.0/docs/changes/README.md`

 * *Files identical despite different names*

### Comparing `pyirf-0.8.1/docs/changes/template.rst` & `pyirf-0.9.0/docs/changes/template.rst`

 * *Files identical despite different names*

### Comparing `pyirf-0.8.1/docs/conf.py` & `pyirf-0.9.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyirf-0.8.1/docs/contribute.rst` & `pyirf-0.9.0/docs/contribute.rst`

 * *Files identical despite different names*

### Comparing `pyirf-0.8.1/docs/examples.rst` & `pyirf-0.9.0/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `pyirf-0.8.1/docs/index.rst` & `pyirf-0.9.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pyirf-0.8.1/docs/install.rst` & `pyirf-0.9.0/docs/install.rst`

 * *Files identical despite different names*

### Comparing `pyirf-0.8.1/docs/introduction.rst` & `pyirf-0.9.0/docs/introduction.rst`

 * *Files identical despite different names*

### Comparing `pyirf-0.8.1/docs/irf/index.rst` & `pyirf-0.9.0/docs/irf/index.rst`

 * *Files identical despite different names*

### Comparing `pyirf-0.8.1/docs/notebooks/fact_example.ipynb` & `pyirf-0.9.0/docs/notebooks/fact_example.ipynb`

 * *Files identical despite different names*

### Comparing `pyirf-0.8.1/download_irfs.py` & `pyirf-0.9.0/download_irfs.py`

 * *Files identical despite different names*

### Comparing `pyirf-0.8.1/examples/calculate_eventdisplay_irfs.py` & `pyirf-0.9.0/examples/calculate_eventdisplay_irfs.py`

 * *Files identical despite different names*

### Comparing `pyirf-0.8.1/examples/comparison_with_EventDisplay.ipynb` & `pyirf-0.9.0/examples/comparison_with_EventDisplay.ipynb`

 * *Files identical despite different names*

### Comparing `pyirf-0.8.1/examples/plot_spectra.py` & `pyirf-0.9.0/examples/plot_spectra.py`

 * *Files identical despite different names*

### Comparing `pyirf-0.8.1/pyirf/benchmarks/angular_resolution.py` & `pyirf-0.9.0/pyirf/benchmarks/angular_resolution.py`

 * *Files 3% similar despite different names*

```diff
@@ -54,8 +54,9 @@
     if len(events) == 0:
         return result
 
     # use groupby operations to calculate the percentile in each bin
     by_bin = table[valid].group_by(bin_index[valid])
     for bin_idx, group in zip(by_bin.groups.keys, by_bin.groups):
         result[key][bin_idx] = np.nanquantile(group["theta"], ONE_SIGMA_QUANTILE)
+        result["n_events"][bin_idx] = len(group)
     return result
```

### Comparing `pyirf-0.8.1/pyirf/benchmarks/energy_bias_resolution.py` & `pyirf-0.9.0/pyirf/benchmarks/energy_bias_resolution.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     return resolution
 
 
 def energy_bias_resolution(
     events,
     energy_bins,
     energy_type="true",
-    bias_function=np.median,
+    bias_function=np.nanmedian,
     resolution_function=inter_quantile_distance,
 ):
     """
     Calculate bias and energy resolution.
 
     Parameters
     ----------
```

### Comparing `pyirf-0.8.1/pyirf/benchmarks/tests/test_angular_resolution.py` & `pyirf-0.9.0/pyirf/benchmarks/tests/test_angular_resolution.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,15 +41,19 @@
 
     events['theta'] = events['theta'].to(unit)
 
     # add nans to test if nans are ignored
     events["true_energy"].value[500] = np.nan
     events["true_energy"].value[1500] = np.nan
 
-    ang_res = angular_resolution(
+    table = angular_resolution(
         events,
         [1, 10, 100] * u.TeV,
-    )['angular_resolution']
+    )
 
+    ang_res = table['angular_resolution']
     assert len(ang_res) == 2
     assert u.isclose(ang_res[0], TRUE_RES_1 * u.deg, rtol=0.05)
     assert u.isclose(ang_res[1], TRUE_RES_2 * u.deg, rtol=0.05)
+
+    # one value in each bin is nan, which is ignored
+    np.testing.assert_array_equal(table["n_events"], [998, 998])
```

### Comparing `pyirf-0.8.1/pyirf/benchmarks/tests/test_bias_resolution.py` & `pyirf-0.9.0/pyirf/benchmarks/tests/test_bias_resolution.py`

 * *Files identical despite different names*

### Comparing `pyirf-0.8.1/pyirf/binning.py` & `pyirf-0.9.0/pyirf/binning.py`

 * *Files identical despite different names*

### Comparing `pyirf-0.8.1/pyirf/conftest.py` & `pyirf-0.9.0/pyirf/conftest.py`

 * *Files identical despite different names*

### Comparing `pyirf-0.8.1/pyirf/cut_optimization.py` & `pyirf-0.9.0/pyirf/cut_optimization.py`

 * *Files identical despite different names*

### Comparing `pyirf-0.8.1/pyirf/cuts.py` & `pyirf-0.9.0/pyirf/cuts.py`

 * *Files identical despite different names*

### Comparing `pyirf-0.8.1/pyirf/exceptions.py` & `pyirf-0.9.0/pyirf/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyirf-0.8.1/pyirf/gammapy.py` & `pyirf-0.9.0/pyirf/gammapy.py`

 * *Files identical despite different names*

### Comparing `pyirf-0.8.1/pyirf/interpolation/griddata_interpolator.py` & `pyirf-0.9.0/pyirf/interpolation/griddata_interpolator.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,53 +5,63 @@
 
 from .base_interpolators import ParametrizedInterpolator
 
 __all__ = ["GridDataInterpolator"]
 
 
 class GridDataInterpolator(ParametrizedInterpolator):
-    def __init__(self, grid_points, params):
-        """GridDataInterpolator constructor
+    def __init__(self, grid_points, params, **griddata_kwargs):
+        """Parametrized Interpolator using scipy.interpolate.griddata
 
         Parameters
         ----------
         grid_points: np.ndarray, shape=(N, O)
             Grid points at which interpolation templates exist
         params: np.ndarray, shape=(N, ...)
             Structured array of corresponding parameter values at each
             point in grid_points.
             First dimesion has to correspond to number of grid_points
+        griddata_kwargs: dict
+            Keyword-Arguments passed to scipy.griddata [1], e.g.
+            interpolation method. Defaults to None, which uses scipy's
+            defaults
 
         Raises
         ------
         TypeError:
             When params is not a np.ndarray
         ValueError:
             When number of points grid_points and params is not matching
+
+        References
+        ----------
+        .. [1] Scipy Documentation, scipy.interpolate.griddata
+               https://docs.scipy.org/doc/scipy/reference/generated/scipy.interpolate.griddata.html
+
         """
         super().__init__(grid_points, params)
 
-    def interpolate(self, target_point, **kwargs):
+        self.griddata_kwargs = griddata_kwargs
+
+    def interpolate(self, target_point):
         """
         Wrapper around scipy.interpolate.griddata [1]
 
         Parameters
         ----------
         target_point: np.ndarray, shape=(1, O)
             Target point for interpolation
-        **kwargs:
-            Passed to scipy.interpolate.griddata [1]
 
         Returns
         -------
         interpolant: np.ndarray
 
         References
         ----------
         .. [1] Scipy Documentation, scipy.interpolate.griddata
-               https://docs.scipy.org/doc/scipy/reference/generated
+               https://docs.scipy.org/doc/scipy/reference/generated/scipy.interpolate.griddata.html
         """
         interpolant = griddata(
-            self.grid_points, self.params, target_point, **kwargs
+            self.grid_points, self.params, target_point, **self.griddata_kwargs
         ).squeeze()
 
         return interpolant.reshape(1, *self.params.shape[1:])
```

### Comparing `pyirf-0.8.1/pyirf/interpolation/quantile_interpolator.py` & `pyirf-0.9.0/pyirf/interpolation/quantile_interpolator.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np
 from scipy.interpolate import griddata, interp1d
 
-from .base_interpolators import BinnedInterpolator
+from .base_interpolators import DiscretePDFInterpolator
 
 __all__ = ["QuantileInterpolator"]
 
 
 def cdf_values(bin_contents):
     """
     compute cdf values and assure they are normed to unity
@@ -144,62 +144,50 @@
         out=np.zeros_like(pdf_values),
         where=norm[..., np.newaxis] != 0,
     )
 
     return normed_pdf_values
 
 
-class QuantileInterpolator(BinnedInterpolator):
-    def __init__(
-        self, grid_points, bin_edges, bin_contents, axis, quantile_resolution=1e-3
-    ):
+class QuantileInterpolator(DiscretePDFInterpolator):
+    def __init__(self, grid_points, bin_edges, bin_contents, quantile_resolution=1e-3):
         """BinnedInterpolator constructor
 
         Parameters
         ----------
         grid_points: np.ndarray
             Grid points at which interpolation templates exist
         bin_edges: np.ndarray
             Edges of the data binning
         bin_contents: np.ndarray
             Content of each bin in bin_edges for
             each point in grid_points. First dimesion has to correspond to number
-            of grid_points, the dimension indicated by axis has to correspond to number
+            of grid_points, the last axis has to correspond to number
             of bins for the quantity that should be interpolated
             (e.g. the Migra axis for EDisp)
-        axis: int
-            Interpolation axis
         quantile_resolution: float
             Spacing between quantiles
 
         Raises
         ------
-        TypeError:
-            When bin_edges is not a np.ndarray
-        TypeError:
-            When bin_content is not a np.ndarray
         ValueError:
-            When number of bins in bin_edges and contents bin_contents is
-            not matching
-        ValueError:
-            When number of histograms in bin_contents and points in grid_points
-            is not matching
+            When last axis in bin_contents and number of bins are not equal.
 
         Note
         ----
-            Also calls pyirf.interpolation.BaseInterpolators.__call__
+            Also calls __init__ of pyirf.interpolation.BaseInterpolator and
+            DiscretePDFInterpolator
         """
-        self.axis = axis
-
         # Remember input shape
         self.input_shape = bin_contents.shape
 
-        # To have the needed axis always at the last index, as the number of indices is
-        # not safely propageted through the interpolation but the last element remains the last element
-        bin_contents = np.swapaxes(bin_contents, self.axis, -1)
+        if self.input_shape[-1] != len(bin_edges) - 1:
+            raise ValueError(
+                "Number of bins along last axis and those specified by bin_edges not matching."
+            )
 
         # include 0-bin at first position in each pdf to avoid edge-effects where the CDF would otherwise
         # start at a value != 0, also extend edges with one bin to the left
         fill_zeros = np.zeros(shape=bin_contents.shape[:-1])[..., np.newaxis]
         bin_contents = np.concatenate((fill_zeros, bin_contents), axis=-1)
         bin_edges = np.append(bin_edges[0] - np.diff(bin_edges)[0], bin_edges)
 
@@ -214,31 +202,28 @@
 
         # Compute CDF values
         self.cdfs = cdf_values(self.bin_contents)
 
         # compute ppf values at quantiles, determine quantile step of [1]
         self.ppfs = ppf_values(self.bin_mids, self.cdfs, self.quantiles)
 
-    def interpolate(self, target_point, **kwargs):
+    def interpolate(self, target_point):
         """
         Takes a grid of binned pdfs for a bunch of different parameters
         and interpolates it to given value of those parameters.
         This function provides an adapted version of the quantile interpolation introduced
         in [1].
         Instead of following this method closely, it implements different approaches to the
         steps shown in Fig. 5 of [1].
 
         Parameters
         ----------
         target_point: numpy.ndarray, shape=(O)
             Value for which the interpolation is performed (target point)
 
-        **kwargs:
-            Currently ignored
-
         Returns
         -------
         f_new: numpy.ndarray, shape=(1,...,M,...)
             Interpolated and binned pdf
 
         References
         ----------
@@ -256,10 +241,8 @@
             self.bin_edges, interpolated_ppfs, self.quantiles
         )[..., 1:]
 
         # Renormalize pdf to sum of 1
         normed_interpolated_pdfs = norm_pdf(interpolated_pdfs)
 
         # Re-swap axes and set all nans to zero
-        return np.swapaxes(
-            np.nan_to_num(normed_interpolated_pdfs), self.axis, -1
-        ).reshape(1, *self.input_shape[1:])
+        return np.nan_to_num(normed_interpolated_pdfs).reshape(1, *self.input_shape[1:])
```

### Comparing `pyirf-0.8.1/pyirf/interpolation/tests/test_griddata_interpolator.py` & `pyirf-0.9.0/pyirf/interpolation/tests/test_griddata_interpolator.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,52 +1,50 @@
-"""Tests for base interpolator classes"""
+"""Tests for GridDataInterpolator"""
 import numpy as np
 
 
 def test_GridDataInterpolator_1DGrid():
-    """Test checks performed to enforce correct data structure"""
+    """Test GridDataInterpolator on 1D Grid"""
     from pyirf.interpolation import GridDataInterpolator
 
     grid_points = np.array([[0], [1]])
     target_point = np.array([[0.5]])
 
     dummy_data1 = np.array([[[0, 1], [1, 1]], [[0, 2], [2, 3]], [[0, 3], [3, 5]]])
     dummy_data2 = np.array([[[0, 2], [2, 2]], [[0, 4], [4, 6]], [[0, 6], [6, 10]]])
 
     dummy_data = np.array([dummy_data1, dummy_data2])
 
-    Interpolator = GridDataInterpolator(
-        grid_points=grid_points,
-        params=dummy_data,
+    interpolator = GridDataInterpolator(
+        grid_points=grid_points, params=dummy_data, method="linear"
     )
-    interpolant = Interpolator(target_point)
+    interpolant = interpolator(target_point)
 
     dummy_data_target = 1.5 * dummy_data1
 
     assert np.allclose(interpolant, dummy_data_target)
     assert interpolant.shape == (1, *dummy_data.shape[1:])
 
 
 def test_GridDataInterpolator_2DGrid():
-    """Test checks performed to enforce correct data structure"""
+    """Test GridDataInterpolator on 2D Grid"""
     from pyirf.interpolation import GridDataInterpolator
 
     grid_points = np.array([[0, 0], [0, 1], [1, 0], [1, 1]])
     target_point = np.array([[0.5, 0.5]])
 
     dummy_data1 = np.array([[[0, 1], [1, 1]], [[0, 2], [2, 3]], [[0, 3], [3, 5]]])
     dummy_data2 = np.array([[[0, 2], [1, 2]], [[0, 4], [2, 6]], [[0, 6], [3, 10]]])
     dummy_data3 = np.array([[[0, 1], [2, 1]], [[0, 2], [4, 3]], [[0, 3], [6, 5]]])
     dummy_data4 = np.array([[[0, 2], [2, 2]], [[0, 4], [4, 6]], [[0, 6], [6, 10]]])
 
     dummy_data = np.array([dummy_data1, dummy_data2, dummy_data3, dummy_data4])
 
-    Interpolator = GridDataInterpolator(
-        grid_points=grid_points,
-        params=dummy_data,
+    interpolator = GridDataInterpolator(
+        grid_points=grid_points, params=dummy_data, method="linear"
     )
-    interpolant = Interpolator(target_point)
+    interpolant = interpolator(target_point)
 
     dummy_data_target = 1.5 * dummy_data1
 
     assert np.allclose(interpolant, dummy_data_target)
     assert interpolant.shape == (1, *dummy_data.shape[1:])
```

### Comparing `pyirf-0.8.1/pyirf/interpolation/tests/test_interpolate_irfs.py` & `pyirf-0.9.0/pyirf/interpolation/tests/test_component_estimator_specific_classes.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,44 +1,47 @@
 import astropy.units as u
 import numpy as np
-from scipy.stats import expon
-
-import pyirf.interpolation as interp
 from pyirf.utils import cone_solid_angle
+from scipy.stats import expon
 
 
-def test_interpolate_energy_dispersion(prod5_irfs):
-    from pyirf.interpolation import interpolate_energy_dispersion
+def test_EnergyDispersionEstimator(prod5_irfs):
+    from pyirf.interpolation import EnergyDispersionEstimator, QuantileInterpolator
 
     zen_pnt = np.array([key.value for key in prod5_irfs.keys()])
     edisps = np.array([irf["edisp"].data for irf in prod5_irfs.values()])
     bin_edges = list(prod5_irfs.values())[0]["edisp"].axes["migra"].edges
 
-    interp = interpolate_energy_dispersion(
-        migra_bins=bin_edges,
-        edisps=edisps[[0, 2]],
+    estimator = EnergyDispersionEstimator(
         grid_points=zen_pnt[[0, 2]],
-        target_point=zen_pnt[[1]],
-        quantile_resolution=1e-3,
+        migra_bins=bin_edges,
+        energy_dispersion=edisps[[0, 2]],
+        interpolator_cls=QuantileInterpolator,
+        interpolator_kwargs={"quantile_resolution": 1e-3},
+        extrapolator_cls=None,
+        extrapolator_kwargs=None,
+        axis=-2,
     )
 
+    interp = estimator(target_point=zen_pnt[[1]])
+
     assert np.max(interp) <= 1
     assert np.min(interp) >= 0
     assert np.all(np.isfinite(interp))
     assert np.all(
         np.logical_or(
             np.isclose(np.sum(interp, axis=-2), 1),
             np.isclose(np.sum(interp, axis=-2), 0),
         )
     )
     assert interp.shape == edisps[[1]].shape
 
 
-def test_interpolate_psf_table():
-    from pyirf.interpolation import interpolate_psf_table
+def test_PSFTableEstimator():
+    from pyirf.interpolation import PSFTableEstimator, QuantileInterpolator
 
     # dummy psf_table with 30 bins of true energ and 6 bins of fov-offset, rad-axis
     # to be inflated later
     dummy_psf_template = np.ones((30, 6, 1))
 
     zen_pnt = np.array([20, 40, 60])
     bin_edges = np.linspace(0, 1, 31) * u.deg
@@ -47,42 +50,52 @@
     def hist(pnt):
         """Create dummy psf for given pointing"""
         histogram = np.diff(expon(scale=pnt / 400).cdf(bin_edges))
         normed_hist = histogram / np.sum(histogram)
 
         return normed_hist / omegas
 
-    dummy_psfs = np.array(
-        [np.apply_along_axis(hist, -1, dummy_psf_template * pnt) for pnt in zen_pnt]
+    dummy_psfs = (
+        np.array(
+            [np.apply_along_axis(hist, -1, dummy_psf_template * pnt) for pnt in zen_pnt]
+        )
+        * u.sr**-1
     )
 
-    interp = interpolate_psf_table(
-        source_offset_bins=bin_edges,
-        psfs=dummy_psfs[[0, 2]],
+    estimator = PSFTableEstimator(
         grid_points=zen_pnt[[0, 2]],
-        target_point=zen_pnt[[1]],
-        quantile_resolution=1e-3,
+        source_offset_bins=bin_edges,
+        psf=dummy_psfs[[0, 2]],
+        interpolator_cls=QuantileInterpolator,
+        interpolator_kwargs={"quantile_resolution": 1e-3},
+        extrapolator_cls=None,
+        extrapolator_kwargs=None,
+        axis=-1,
     )
 
+    interp = estimator(target_point=zen_pnt[[1]])
+
     interp *= omegas[np.newaxis, np.newaxis, np.newaxis, ...]
 
     assert np.max(interp) <= 1
     assert np.min(interp) >= 0
     assert np.all(np.isfinite(interp))
     assert np.all(
         np.logical_or(
             np.isclose(np.sum(interp, axis=-1), 1),
             np.isclose(np.sum(interp, axis=-1), 0),
         )
     )
     assert interp.shape == dummy_psfs[[1]].shape
 
 
-def test_interpolate_effective_area_per_energy_and_fov():
+def test_EffectiveAreaEstimator_sythetic_data():
     """Test of interpolating of effective area using dummy model files."""
+    from pyirf.interpolation import EffectiveAreaEstimator, GridDataInterpolator
+
     n_en = 20
     n_th = 1
     en = np.logspace(-2, 2, n_en)
     # applying a simple sigmoid function
     aeff0 = 1.0e4 / (1 + 1 / en**2) * u.m**2
 
     # assume that for parameters 'x' and 'y' the Aeff scales x*y*Aeff0
@@ -96,64 +109,80 @@
         for yy in y:
             aeff[i_grid, 0, :] = aeff0 * xx * yy / 10
             pars[i_grid, :] = np.array([xx, yy])
             i_grid += 1
     aeff *= u.m**2
     pars0 = np.array([1, 10])
     min_aeff = 1 * u.m**2
-    aeff_interp = interp.interpolate_effective_area_per_energy_and_fov(
-        aeff, pars, pars0, min_effective_area=min_aeff, method="linear"
+
+    estimator = EffectiveAreaEstimator(
+        grid_points=pars,
+        effective_area=aeff,
+        interpolator_cls=GridDataInterpolator,
+        interpolator_kwargs=None,
+        extrapolator_cls=None,
+        extrapolator_kwargs=None,
+        min_effective_area=min_aeff,
     )
+    aeff_interp = estimator(pars0)
 
     # allowing for 3% accuracy except of close to the minimum value of Aeff
     assert np.allclose(aeff_interp[:, 0], aeff0, rtol=0.03, atol=min_aeff)
 
 
-def test_interpolate_effective_area_per_energy_and_fov_prod5(prod5_irfs):
+def test_EffectiveAreaEstimator_prod5(prod5_irfs):
     """Test of interpolation of effective are on prod5 irfs"""
-    from pyirf.interpolation import interpolate_effective_area_per_energy_and_fov
+    from pyirf.interpolation import EffectiveAreaEstimator, GridDataInterpolator
 
     zen_pnt = np.array([key.value for key in prod5_irfs.keys()])
     aeffs = np.array([irf["aeff"].data for irf in prod5_irfs.values()])
+    min_aeff = 1 * u.m**2
 
-    interp = interpolate_effective_area_per_energy_and_fov(
-        effective_area=aeffs[[0, 2]] * u.m**2,
+    estimator = EffectiveAreaEstimator(
         grid_points=zen_pnt[[0, 2]],
-        target_point=zen_pnt[[1]],
-        min_effective_area=1 * u.m**2,
-    ).value
+        effective_area=aeffs[[0, 2]] * u.m**2,
+        interpolator_cls=GridDataInterpolator,
+        interpolator_kwargs={"method": "linear"},
+        extrapolator_cls=None,
+        extrapolator_kwargs=None,
+        min_effective_area=min_aeff,
+    )
+    interp = estimator(zen_pnt[[1]]).value
 
     assert np.all(np.isfinite(interp))
     assert interp.shape == aeffs[[1]].shape
     assert np.all(interp >= 0)
 
     assert np.all(
         np.logical_or(
             np.logical_or(
                 np.logical_and(aeffs[[0]] <= interp, interp <= aeffs[[2]]),
                 np.logical_and(aeffs[[2]] <= interp, interp <= aeffs[[0]]),
             ),
-            interp == 0,
+            np.logical_or(interp == 0, interp == min_aeff.value),
         )
     )
 
 
-def test_interpolate_rad_max():
-    from pyirf.interpolation import interpolate_rad_max
+def test_RadMaxEstimator():
+    from pyirf.interpolation import GridDataInterpolator, RadMaxEstimator
 
     # linear test case
     rad_max_1 = np.array([[0, 0], [1, 0], [2, 1], [3, 2]])
     rad_max_2 = 2 * rad_max_1
     rad_max = np.array([rad_max_1, rad_max_2])
 
     grid_points = np.array([[0], [1]])
     target_point = np.array([0.5])
 
-    interp = interpolate_rad_max(
-        rad_max=rad_max,
+    estimator = RadMaxEstimator(
         grid_points=grid_points,
-        target_point=target_point,
-        method="linear",
+        rad_max=rad_max,
+        interpolator_cls=GridDataInterpolator,
+        interpolator_kwargs=None,
+        extrapolator_cls=None,
+        extrapolator_kwargs=None,
     )
+    interp = estimator(target_point)
 
     assert interp.shape == (1, *rad_max_1.shape)
     assert np.allclose(interp, 1.5 * rad_max_1)
```

### Comparing `pyirf-0.8.1/pyirf/interpolation/tests/test_quantile_interpolator.py` & `pyirf-0.9.0/pyirf/interpolation/tests/test_quantile_interpolator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import numpy as np
 import pytest
-from scipy.stats import norm
-
 from pyirf.binning import bin_center
+from scipy.stats import norm
 
 
 @pytest.fixture
 def data():
     """Create common dataset containing binned Gaussians for interpolation testing. Binned PDFs sum to 1."""
     bin_edges = np.linspace(-5, 30, 101)
     distributions = [norm(5, 1), norm(10, 2), norm(15, 3)]
@@ -41,16 +40,15 @@
     assert np.max(cdf_est) == 1
 
     # Assert estimated and true cdf are matching
     assert np.allclose(cdf_est, data["distributions"][0].cdf(data["bin_edges"][1:]))
 
 
 def test_ppf_values(data):
-    from pyirf.interpolation.quantile_interpolator import (cdf_values,
-                                                           ppf_values)
+    from pyirf.interpolation.quantile_interpolator import cdf_values, ppf_values
 
     # Create quantiles, ignore the 0% and 100% quantile as they are analytically +- inf
     quantiles = np.linspace(0, 1, 10)[1:-2]
 
     # True ppf-values
     ppf_true = data["distributions"][0].ppf(quantiles)
     bin_mids = bin_center(data["bin_edges"])
@@ -60,17 +58,19 @@
     ppf_est = ppf_values(bin_mids, cdf_est, quantiles)
 
     # Assert truth and estimation match allowing for +- bin_width deviation
     assert np.allclose(ppf_true, ppf_est, atol=np.diff(data["bin_edges"])[0])
 
 
 def test_pdf_from_ppf(data):
-    from pyirf.interpolation.quantile_interpolator import (cdf_values,
-                                                           pdf_from_ppf,
-                                                           ppf_values)
+    from pyirf.interpolation.quantile_interpolator import (
+        cdf_values,
+        pdf_from_ppf,
+        ppf_values,
+    )
 
     # Create quantiles
     quantiles = np.linspace(0, 1, 1000)
     bin_mids = bin_center(data["bin_edges"])
 
     # Estimate ppf-values
     cdf_est = cdf_values(data["binned_pdfs"][0])
@@ -94,15 +94,14 @@
     from pyirf.interpolation import QuantileInterpolator
 
     interpolator = QuantileInterpolator(
         grid_points=data["grid_points"][[0, 2]],
         bin_edges=data["bin_edges"],
         bin_contents=data["binned_pdfs"][[0, 2], :],
         quantile_resolution=1e-3,
-        axis=-1,
     )
 
     interp = interpolator(
         target_point=np.array([data["grid_points"][1]]),
     ).squeeze()
 
     bin_mids = bin_center(data["bin_edges"])
```

### Comparing `pyirf-0.8.1/pyirf/io/eventdisplay.py` & `pyirf-0.9.0/pyirf/io/eventdisplay.py`

 * *Files identical despite different names*

### Comparing `pyirf-0.8.1/pyirf/io/gadf.py` & `pyirf-0.9.0/pyirf/io/gadf.py`

 * *Files identical despite different names*

### Comparing `pyirf-0.8.1/pyirf/io/tests/test_gadf.py` & `pyirf-0.9.0/pyirf/io/tests/test_gadf.py`

 * *Files identical despite different names*

### Comparing `pyirf-0.8.1/pyirf/irf/background.py` & `pyirf-0.9.0/pyirf/irf/background.py`

 * *Files identical despite different names*

### Comparing `pyirf-0.8.1/pyirf/irf/effective_area.py` & `pyirf-0.9.0/pyirf/irf/effective_area.py`

 * *Files identical despite different names*

### Comparing `pyirf-0.8.1/pyirf/irf/energy_dispersion.py` & `pyirf-0.9.0/pyirf/irf/energy_dispersion.py`

 * *Files identical despite different names*

### Comparing `pyirf-0.8.1/pyirf/irf/psf.py` & `pyirf-0.9.0/pyirf/irf/psf.py`

 * *Files identical despite different names*

### Comparing `pyirf-0.8.1/pyirf/irf/tests/test_background.py` & `pyirf-0.9.0/pyirf/irf/tests/test_background.py`

 * *Files identical despite different names*

### Comparing `pyirf-0.8.1/pyirf/irf/tests/test_effective_area.py` & `pyirf-0.9.0/pyirf/irf/tests/test_effective_area.py`

 * *Files identical despite different names*

### Comparing `pyirf-0.8.1/pyirf/irf/tests/test_energy_dispersion.py` & `pyirf-0.9.0/pyirf/irf/tests/test_energy_dispersion.py`

 * *Files identical despite different names*

### Comparing `pyirf-0.8.1/pyirf/irf/tests/test_psf.py` & `pyirf-0.9.0/pyirf/irf/tests/test_psf.py`

 * *Files identical despite different names*

### Comparing `pyirf-0.8.1/pyirf/resources/dampe_p+he.ecsv` & `pyirf-0.9.0/pyirf/resources/dampe_p+he.ecsv`

 * *Files identical despite different names*

### Comparing `pyirf-0.8.1/pyirf/sensitivity.py` & `pyirf-0.9.0/pyirf/sensitivity.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,18 +63,14 @@
     except (RuntimeError, ValueError) as e:
         log.warn(
             "Could not calculate relative significance for"
             f" n_signal={n_signal:.1f}, n_off={n_off:.1f}, returning nan {e}"
         )
         return np.nan
 
-    # less than min_sigma
-    if relative_flux > 1:
-        return np.nan
-
     # scale to achieved flux level
     n_signal = n_signal * relative_flux
     min_excess = min_excess_over_background * n_background
     min_signal = max(min_signal_events, min_excess)
 
     # if we violate the min signal events condition,
     # increase flux until we meet the requirement
```

### Comparing `pyirf-0.8.1/pyirf/simulations.py` & `pyirf-0.9.0/pyirf/simulations.py`

 * *Files identical despite different names*

### Comparing `pyirf-0.8.1/pyirf/spectral.py` & `pyirf-0.9.0/pyirf/spectral.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 """
 Functions and classes for calculating spectral weights
 """
+import sys
+from importlib.resources import as_file, files
+
 import astropy.units as u
 import numpy as np
-from scipy.interpolate import interp1d
-from pkg_resources import resource_filename
 from astropy.table import QTable
+from scipy.interpolate import interp1d
 
 from .utils import cone_solid_angle
 
 #: Unit of a point source flux
 #:
 #: Number of particles per Energy, time and area
-POINT_SOURCE_FLUX_UNIT = (1 / u.TeV / u.s / u.m ** 2).unit
+POINT_SOURCE_FLUX_UNIT = (1 / u.TeV / u.s / u.m**2).unit
 
 #: Unit of a diffuse flux
 #:
 #: Number of particles per Energy, time, area and solid_angle
 DIFFUSE_FLUX_UNIT = POINT_SOURCE_FLUX_UNIT / u.sr
 
 
@@ -88,15 +90,15 @@
 
     @u.quantity_input(
         normalization=[DIFFUSE_FLUX_UNIT, POINT_SOURCE_FLUX_UNIT], e_ref=u.TeV
     )
     def __init__(self, normalization, index, e_ref=1 * u.TeV):
         """Create a new PowerLaw spectrum"""
         if index > 0:
-            raise ValueError(f'Index must be < 0, got {index}')
+            raise ValueError(f"Index must be < 0, got {index}")
 
         self.normalization = normalization
         self.index = index
         self.e_ref = e_ref
 
     @u.quantity_input(energy=u.TeV)
     def __call__(self, energy):
@@ -119,21 +121,25 @@
         if viewcone.value > 0:
             solid_angle = 2 * np.pi * (1 - np.cos(viewcone)) * u.sr
             unit = DIFFUSE_FLUX_UNIT
         else:
             solid_angle = 1
             unit = POINT_SOURCE_FLUX_UNIT
 
-        A = np.pi * simulated_event_info.max_impact ** 2
+        A = np.pi * simulated_event_info.max_impact**2
 
         delta = e_max ** (index + 1) - e_min ** (index + 1)
-        nom = (index + 1) * e_ref ** index * n_showers
+        nom = (index + 1) * e_ref**index * n_showers
         denom = (A * obstime * solid_angle) * delta
 
-        return cls(normalization=(nom / denom).to(unit), index=index, e_ref=e_ref,)
+        return cls(
+            normalization=(nom / denom).to(unit),
+            index=index,
+            e_ref=e_ref,
+        )
 
     def __repr__(self):
         return f"{self.__class__.__name__}({self.normalization} * (E / {self.e_ref})**{self.index})"
 
     @u.quantity_input(inner=u.rad, outer=u.rad)
     def integrate_cone(self, inner, outer):
         """Integrate this powerlaw over solid angle in the given cone
@@ -159,15 +165,14 @@
         return PowerLaw(
             normalization=self.normalization * solid_angle,
             index=self.index,
             e_ref=self.e_ref,
         )
 
 
-
 class LogParabola:
     r"""
     A log parabola flux parameterization.
 
     .. math::
 
         \Phi(E, \Phi_0, \alpha, \beta, E_\text{ref}) =
@@ -307,15 +312,15 @@
 
         if self.log_energy:
             x = np.log10(x)
 
         y = self.interp(x)
 
         if self.log_flux:
-            y = 10 ** y
+            y = 10**y
 
         return u.Quantity(y, self.flux_unit, copy=False)
 
     @classmethod
     def from_table(
         cls, table: QTable, log_energy=True, log_flux=True, reference_energy=1 * u.TeV
     ):
@@ -341,51 +346,57 @@
 
 #: Power Law parametrization of the Crab Nebula spectrum as published by HEGRA
 #:
 #: From "The Crab Nebula and Pulsar between 500 GeV and 80 TeV: Observations with the HEGRA stereoscopic air Cherenkov telescopes",
 #: Aharonian et al, 2004, ApJ 614.2
 #: doi.org/10.1086/423931
 CRAB_HEGRA = PowerLaw(
-    normalization=2.83e-11 / (u.TeV * u.cm ** 2 * u.s), index=-2.62, e_ref=1 * u.TeV,
+    normalization=2.83e-11 / (u.TeV * u.cm**2 * u.s),
+    index=-2.62,
+    e_ref=1 * u.TeV,
 )
 
 #: Log-Parabola parametrization of the Crab Nebula spectrum as published by MAGIC
 #:
 #: From "Measurement of the Crab Nebula spectrum over three decades in energy with the MAGIC telescopes",
 #: Aleksìc et al., 2015, JHEAP
 #: https://doi.org/10.1016/j.jheap.2015.01.002
 CRAB_MAGIC_JHEAP2015 = LogParabola(
-    normalization=3.23e-11 / (u.TeV * u.cm ** 2 * u.s), a=-2.47, b=-0.24,
+    normalization=3.23e-11 / (u.TeV * u.cm**2 * u.s),
+    a=-2.47,
+    b=-0.24,
 )
 
 
 #: All particle spectrum
 #:
 #: (30.2) from "The Review of Particle Physics (2020)"
 #: https://pdg.lbl.gov/2020/reviews/rpp2020-rev-cosmic-rays.pdf
 PDG_ALL_PARTICLE = PowerLaw(
-    normalization=1.8e4 / (u.GeV * u.m ** 2 * u.s * u.sr), index=-2.7, e_ref=1 * u.GeV,
+    normalization=1.8e4 / (u.GeV * u.m**2 * u.s * u.sr),
+    index=-2.7,
+    e_ref=1 * u.GeV,
 )
 
 #: Proton spectrum definition defined in the CTA Prod3b IRF Document
 #:
 #: From "Description of CTA Instrument Response Functions (Production 3b Simulation)", section 4.3.1
 #: https://gitlab.cta-observatory.org/cta-consortium/aswg/documentation/internal_reports/irfs-reports/prod3b-irf-description
 IRFDOC_PROTON_SPECTRUM = PowerLaw(
-    normalization=9.8e-6 / (u.cm ** 2 * u.s * u.TeV * u.sr),
+    normalization=9.8e-6 / (u.cm**2 * u.s * u.TeV * u.sr),
     index=-2.62,
     e_ref=1 * u.TeV,
 )
 
 #: Electron spectrum definition defined in the CTA Prod3b IRF Document
 #:
 #: From "Description of CTA Instrument Response Functions (Production 3b Simulation)", section 4.3.1
 #: https://gitlab.cta-observatory.org/cta-consortium/aswg/documentation/internal_reports/irfs-reports/prod3b-irf-description
 IRFDOC_ELECTRON_SPECTRUM = PowerLawWithExponentialGaussian(
-    normalization=2.385e-9 / (u.TeV * u.cm ** 2 * u.s * u.sr),
+    normalization=2.385e-9 / (u.TeV * u.cm**2 * u.s * u.sr),
     index=-3.43,
     e_ref=1 * u.TeV,
     mu=-0.101,
     sigma=0.741,
     f=1.950,
 )
 
@@ -393,10 +404,9 @@
 #:
 #: Datapoints obtained from obtained from:
 #: https://inspirehep.net/files/62efc8374ffced58ea7e3a333bfa1217
 #: Points are from DAMPE, up to  8 TeV.
 #: For higher energies we assume a
 #: flattening of the dF/dE*E^2.7 more or less in the middle of the large
 #: spread of the available data reported on the same proceeding.
-DAMPE_P_He_SPECTRUM = TableInterpolationSpectrum.from_file(
-    resource_filename("pyirf", "resources/dampe_p+he.ecsv")
-)
+with as_file(files("pyirf") / "resources/dampe_p+he.ecsv") as _path:
+    DAMPE_P_He_SPECTRUM = TableInterpolationSpectrum.from_file(_path)
```

### Comparing `pyirf-0.8.1/pyirf/statistics.py` & `pyirf-0.9.0/pyirf/statistics.py`

 * *Files identical despite different names*

### Comparing `pyirf-0.8.1/pyirf/tests/test_binning.py` & `pyirf-0.9.0/pyirf/tests/test_binning.py`

 * *Files identical despite different names*

### Comparing `pyirf-0.8.1/pyirf/tests/test_cuts.py` & `pyirf-0.9.0/pyirf/tests/test_cuts.py`

 * *Files identical despite different names*

### Comparing `pyirf-0.8.1/pyirf/tests/test_gammapy_interop.py` & `pyirf-0.9.0/pyirf/tests/test_gammapy_interop.py`

 * *Files identical despite different names*

### Comparing `pyirf-0.8.1/pyirf/tests/test_sensitivity.py` & `pyirf-0.9.0/pyirf/tests/test_sensitivity.py`

 * *Files 13% similar despite different names*

```diff
@@ -47,20 +47,21 @@
     })
     bg_hist = signal_hist.copy()
     bg_hist['n'] = 20
     bg_hist['n_weighted'] = 50
 
     sensitivity = calculate_sensitivity(signal_hist, bg_hist, alpha=0.2)
 
-    # too small sensitivity
+    # sensitivity smaller than 1
     signal_hist['n_weighted'] = [10, 10]
     sensitivity = calculate_sensitivity(signal_hist, bg_hist, alpha=0.2)
 
     assert len(sensitivity) == len(signal_hist)
-    assert np.all(np.isnan(sensitivity['relative_sensitivity']))
+    np.testing.assert_almost_equal(5.0, sensitivity['significance'])
+    np.testing.assert_array_less(1.0, sensitivity['relative_sensitivity'])
 
     # not above 5 percent of remaining background
     signal_hist['n_weighted'] = 699
     bg_hist['n_weighted'] = 70_000
     sensitivity = calculate_sensitivity(signal_hist, bg_hist, alpha=0.2)
     assert len(sensitivity) == len(signal_hist)
     # we scale up the signal until we meet the requirement, so
@@ -71,14 +72,20 @@
     signal_hist['n_weighted'] = [9, 9]
     bg_hist['n_weighted'] = [1, 1]
     sensitivity = calculate_sensitivity(signal_hist, bg_hist, alpha=0.2)
     # we scale up the signal until we meet the requirement, so
     # we must have more than 5 sigma
     assert np.all(sensitivity['significance'] >= 5)
 
+    # No background at all, li&ma not applicable => event count requirement
+    signal_hist['n_weighted'] = [5, 5]
+    bg_hist['n_weighted'] = [0, 0]
+    sensitivity = calculate_sensitivity(signal_hist, bg_hist, alpha=0.2)
+    np.testing.assert_equal(sensitivity['relative_sensitivity'], 2)
+
 
 def test_estimate_background():
     from pyirf.sensitivity import estimate_background
     N = 1000
     events = QTable({
         'reco_source_fov_offset': np.append(np.full(N, 0.5), np.full(N, 1.5)) * u.deg,
         'reco_energy': np.tile([5, 50], N) * u.TeV,
```

### Comparing `pyirf-0.8.1/pyirf/tests/test_simulations.py` & `pyirf-0.9.0/pyirf/tests/test_simulations.py`

 * *Files identical despite different names*

### Comparing `pyirf-0.8.1/pyirf/tests/test_spectral.py` & `pyirf-0.9.0/pyirf/tests/test_spectral.py`

 * *Files identical despite different names*

### Comparing `pyirf-0.8.1/pyirf/tests/test_statistics.py` & `pyirf-0.9.0/pyirf/tests/test_statistics.py`

 * *Files identical despite different names*

### Comparing `pyirf-0.8.1/pyirf/tests/test_utils.py` & `pyirf-0.9.0/pyirf/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `pyirf-0.8.1/pyirf/utils.py` & `pyirf-0.9.0/pyirf/utils.py`

 * *Files identical despite different names*

### Comparing `pyirf-0.8.1/pyirf/version.py` & `pyirf-0.9.0/pyirf/version.py`

 * *Files identical despite different names*

### Comparing `pyirf-0.8.1/pyirf.egg-info/PKG-INFO` & `pyirf-0.9.0/pyirf.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 Metadata-Version: 2.1
 Name: pyirf
-Version: 0.8.1
+Version: 0.9.0
 Summary: A python library to calculate IACT IRFs and Sensitivities
 Home-page: https://github.com/cta-observatory/pyirf
 Author: CTA Consortium, Analysis and Simulation Working Group
-Author-email: maximilian.noethe@tu-dortmund.de
+Author-email: maximilian.linhoff@tu-dortmund.de
 License: MIT
 Project-URL: Bug Tracker, https://github.com/cta-observatory/pyirf/issues
 Project-URL: Documentation, https://cta-observatory.github.io/pyirf
 Project-URL: Source Code, https://github.com/cta-observatory/pyirf
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.9
 Provides-Extra: docs
 Provides-Extra: tests
 Provides-Extra: gammapy
 Provides-Extra: dev
 Provides-Extra: all
 License-File: LICENSE
 
 ==========================================
 pyirf |ci| |codacy| |coverage| |doilatest|
 ==========================================
 
-.. |ci| image:: https://github.com/cta-observatory/pyirf/workflows/CI/badge.svg?branch=master
-  :target: https://github.com/cta-observatory/pyirf/actions?query=workflow%3ACI+branch%3Amaster
+.. |ci| image:: https://github.com/cta-observatory/pyirf/workflows/CI/badge.svg?branch=main
+  :target: https://github.com/cta-observatory/pyirf/actions?query=workflow%3ACI+branch%3Amain
 .. |codacy| image:: https://app.codacy.com/project/badge/Grade/669fef80d3d54070960e66351477e383
   :target: https://www.codacy.com/gh/cta-observatory/pyirf/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=cta-observatory/pyirf&amp;utm_campaign=Badge_Grade
-.. |coverage| image:: https://codecov.io/gh/cta-observatory/pyirf/branch/master/graph/badge.svg
+.. |coverage| image:: https://codecov.io/gh/cta-observatory/pyirf/branch/main/graph/badge.svg
   :target: https://codecov.io/gh/cta-observatory/pyirf
 .. |doilatest| image:: https://zenodo.org/badge/DOI/10.5281/zenodo.4740755.svg
   :target: https://doi.org/10.5281/zenodo.4740755
 
 *pyirf* is a python library for the generation of Instrument Response
 Functions (IRFs) and sensitivities for the
 `Cherenkov Telescope Array (CTA) <https://www.cta-observatory.org/>`_ .
```

### Comparing `pyirf-0.8.1/pyirf.egg-info/SOURCES.txt` & `pyirf-0.9.0/pyirf.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -70,22 +70,33 @@
 pyirf/benchmarks/__init__.py
 pyirf/benchmarks/angular_resolution.py
 pyirf/benchmarks/energy_bias_resolution.py
 pyirf/benchmarks/tests/__init__.py
 pyirf/benchmarks/tests/test_angular_resolution.py
 pyirf/benchmarks/tests/test_bias_resolution.py
 pyirf/interpolation/__init__.py
+pyirf/interpolation/base_extrapolators.py
 pyirf/interpolation/base_interpolators.py
+pyirf/interpolation/component_estimators.py
 pyirf/interpolation/griddata_interpolator.py
-pyirf/interpolation/interpolate_irfs.py
+pyirf/interpolation/moment_morph_interpolator.py
+pyirf/interpolation/nearest_neighbor_searcher.py
+pyirf/interpolation/nearest_simplex_extrapolator.py
 pyirf/interpolation/quantile_interpolator.py
+pyirf/interpolation/utils.py
+pyirf/interpolation/tests/test_base_extrapolators.py
 pyirf/interpolation/tests/test_base_interpolators.py
+pyirf/interpolation/tests/test_component_estimator_base_classes.py
+pyirf/interpolation/tests/test_component_estimator_specific_classes.py
 pyirf/interpolation/tests/test_griddata_interpolator.py
-pyirf/interpolation/tests/test_interpolate_irfs.py
+pyirf/interpolation/tests/test_moment_morph_interpolator.py
+pyirf/interpolation/tests/test_nearest_neighbor_searcher.py
+pyirf/interpolation/tests/test_nearest_simplex_extrapolator.py
 pyirf/interpolation/tests/test_quantile_interpolator.py
+pyirf/interpolation/tests/test_utils.py
 pyirf/io/__init__.py
 pyirf/io/eventdisplay.py
 pyirf/io/gadf.py
 pyirf/io/tests/__init__.py
 pyirf/io/tests/test_gadf.py
 pyirf/irf/__init__.py
 pyirf/irf/background.py
```

### Comparing `pyirf-0.8.1/pyirf.egg-info/requires.txt` & `pyirf-0.9.0/pyirf.egg-info/requires.txt`

 * *Ordering differences only*

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 astropy>=4.0.2
 matplotlib
 numpy>=1.18
 scipy
 tqdm
 
 [all]
-pytest
-nbsphinx
-awkward1
-sphinx
-numpydoc
+ogadf-schema~=0.2.3
 uproot~=4.0
 tables
-awkward~=1.0
-sphinx_rtd_theme
+sphinx
 setuptools_scm
+pytest-cov
+numpydoc
+pytest
+sphinx_automodapi
+nbsphinx
 notebook
 towncrier
-uproot
-pytest-cov
 gammapy~=1.0
-ogadf-schema~=0.2.3
-sphinx_automodapi
+awkward1
+uproot
+sphinx_rtd_theme
+awkward~=1.0
 
 [dev]
 pytest
 pytest-cov
 gammapy~=1.0
 ogadf-schema~=0.2.3
 uproot~=4.0
```

### Comparing `pyirf-0.8.1/pyproject.toml` & `pyirf-0.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyirf-0.8.1/setup.cfg` & `pyirf-0.9.0/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 [metadata]
 name = pyirf
 description = A python library to calculate IACT IRFs and Sensitivities
 url = https://github.com/cta-observatory/pyirf
 author = CTA Consortium, Analysis and Simulation Working Group
-author_email = maximilian.noethe@tu-dortmund.de
+author_email = maximilian.linhoff@tu-dortmund.de
 license = MIT
 long_description = file: README.rst
 github_project = cta-observatory/pyirf
 project_urls = 
 	Bug Tracker = https://github.com/cta-observatory/pyirf/issues
 	Documentation = https://cta-observatory.github.io/pyirf
 	Source Code = https://github.com/cta-observatory/pyirf
 classifiers = 
 	Development Status :: 4 - Beta
 	License :: OSI Approved :: MIT License
 	Intended Audience :: Science/Research
 	Topic :: Scientific/Engineering :: Astronomy
 	Topic :: Scientific/Engineering :: Physics
 	Programming Language :: Python :: 3 :: Only
-	Programming Language :: Python :: 3.6
-	Programming Language :: Python :: 3.7
-	Programming Language :: Python :: 3.8
+	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 requires_dist = setuptools
 
 [options]
-python_requires = >=3.8
+python_requires = >=3.9
 setup_requires = setuptools_scm[toml]
 
 [flake8]
 exclude = 
 	build,
 	docs,
 	.eggs
```

### Comparing `pyirf-0.8.1/setup.py` & `pyirf-0.9.0/setup.py`

 * *Files identical despite different names*

