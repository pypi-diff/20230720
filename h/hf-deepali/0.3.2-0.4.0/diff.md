# Comparing `tmp/hf-deepali-0.3.2.tar.gz` & `tmp/hf-deepali-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hf-deepali-0.3.2.tar", last modified: Fri Jul  7 02:10:15 2023, max compression
+gzip compressed data, was "hf-deepali-0.4.0.tar", last modified: Thu Jul 20 21:47:07 2023, max compression
```

## Comparing `hf-deepali-0.3.2.tar` & `hf-deepali-0.4.0.tar`

### file list

```diff
@@ -1,251 +1,259 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:10:15.017692 hf-deepali-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:10:14.969689 hf-deepali-0.3.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:10:14.977689 hf-deepali-0.3.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:10:14.977689 hf-deepali-0.3.2/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10941 2023-07-07 02:10:15.017692 hf-deepali-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9791 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/TODO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:10:14.981690 hf-deepali-0.3.2/conda/
--rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/conda/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/conda/README.md
--rw-r--r--   0 runner    (1001) docker     (123)   546679 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/conda/environment.conda-lock.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/conda/environment.devenv.yml
--rw-r--r--   0 runner    (1001) docker     (123)    53215 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/conda/environment.linux-64.lock
--rw-r--r--   0 runner    (1001) docker     (123)    15437 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/conda/environment.linux-64.yml
--rw-r--r--   0 runner    (1001) docker     (123)    45237 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/conda/environment.osx-64.lock
--rw-r--r--   0 runner    (1001) docker     (123)    13327 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/conda/environment.osx-64.yml
--rw-r--r--   0 runner    (1001) docker     (123)    47796 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/conda/environment.win-64.lock
--rw-r--r--   0 runner    (1001) docker     (123)    14101 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/conda/environment.win-64.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:10:14.981690 hf-deepali-0.3.2/docker/
--rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/docker/Dockerfile
--rwxr-xr-x   0 runner    (1001) docker     (123)     1666 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/docker/build
--rwxr-xr-x   0 runner    (1001) docker     (123)     7011 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/docker/run
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:10:14.981690 hf-deepali-0.3.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/docs/_citations.bib
--rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/docs/_config.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:10:14.981690 hf-deepali-0.3.2/docs/_images/
--rw-r--r--   0 runner    (1001) docker     (123)   390208 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/docs/_images/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/docs/_toc.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:10:14.981690 hf-deepali-0.3.2/docs/basics/
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/docs/basics/example-page.md
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/docs/basics/installation.md
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:10:14.969689 hf-deepali-0.3.2/docs/reference/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:10:14.981690 hf-deepali-0.3.2/docs/reference/core/
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/docs/reference/core/domain.md
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/docs/reference/core/flow.md
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/docs/reference/core/image.md
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/docs/reference/core/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/docs/reference/core/kernels.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:10:14.981690 hf-deepali-0.3.2/docs/reference/data/
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/docs/reference/data/dataset.md
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/docs/reference/data/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/docs/reference/data/sampler.md
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/docs/reference/data/tensor.md
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/docs/reference/data/transforms.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:10:14.981690 hf-deepali-0.3.2/docs/reference/losses/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/docs/reference/losses/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:10:14.981690 hf-deepali-0.3.2/docs/reference/modules/
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/docs/reference/modules/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:10:14.981690 hf-deepali-0.3.2/docs/reference/networks/
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/docs/reference/networks/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:10:14.985690 hf-deepali-0.3.2/docs/reference/spatial/
--rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/docs/reference/spatial/common.md
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/docs/reference/spatial/composite.md
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/docs/reference/spatial/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/docs/reference/spatial/transformer.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:10:14.985690 hf-deepali-0.3.2/docs/reference/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/docs/reference/utils/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:10:14.985690 hf-deepali-0.3.2/docs/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/docs/tutorials/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/docs/tutorials/example-myst-notebook.md
--rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/docs/tutorials/example-notebook.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    45130 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/docs/tutorials/pairwise-registration-intro.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:10:14.985690 hf-deepali-0.3.2/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/examples/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:10:14.985690 hf-deepali-0.3.2/examples/ffd/
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/examples/ffd/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/examples/ffd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/examples/ffd/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5296 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/examples/ffd/engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/examples/ffd/hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)    15655 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/examples/ffd/losses.py
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/examples/ffd/optim.py
--rw-r--r--   0 runner    (1001) docker     (123)    32029 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/examples/ffd/pairwise.py
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/examples/ffd/params.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5486 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/examples/ffd/register.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:10:14.989690 hf-deepali-0.3.2/examples/istn/
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/examples/istn/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/examples/istn/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:10:14.989690 hf-deepali-0.3.2/examples/istn/models/
--rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/examples/istn/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/examples/istn/models/itn.py
--rw-r--r--   0 runner    (1001) docker     (123)    23118 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/examples/istn/models/stn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/examples/istn/params.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/examples/istn/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)    27864 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/examples/istn/train.py
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/pyrightconfig.json
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 02:10:15.017692 hf-deepali-0.3.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:10:14.973689 hf-deepali-0.3.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:10:14.973689 hf-deepali-0.3.2/src/deepali/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:10:14.993690 hf-deepali-0.3.2/src/deepali/core/
--rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19990 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/core/_kornia.py
--rw-r--r--   0 runner    (1001) docker     (123)    20523 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/core/affine.py
--rw-r--r--   0 runner    (1001) docker     (123)    23068 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/core/bspline.py
--rw-r--r--   0 runner    (1001) docker     (123)     7192 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    24560 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/core/cube.py
--rw-r--r--   0 runner    (1001) docker     (123)     8783 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/core/enum.py
--rw-r--r--   0 runner    (1001) docker     (123)    20230 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/core/flow.py
--rw-r--r--   0 runner    (1001) docker     (123)     6600 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/core/functional.py
--rw-r--r--   0 runner    (1001) docker     (123)    74085 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/core/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)    78527 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/core/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/core/itertools.py
--rw-r--r--   0 runner    (1001) docker     (123)    11707 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/core/kernels.py
--rw-r--r--   0 runner    (1001) docker     (123)    19590 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/core/linalg.py
--rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/core/math.py
--rw-r--r--   0 runner    (1001) docker     (123)    16778 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/core/nnutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3680 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/core/path.py
--rw-r--r--   0 runner    (1001) docker     (123)    15209 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/core/pointset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4571 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/core/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     9358 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/core/tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5921 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/core/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:10:14.997691 hf-deepali-0.3.2/src/deepali/data/
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/data/collate.py
--rw-r--r--   0 runner    (1001) docker     (123)    19020 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/data/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    24026 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/data/flow.py
--rw-r--r--   0 runner    (1001) docker     (123)    60823 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/data/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/data/partition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/data/prepare.py
--rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/data/sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     6687 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/data/sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/data/tensor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:10:14.997691 hf-deepali-0.3.2/src/deepali/data/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/data/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16698 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/data/transforms/image.py
--rw-r--r--   0 runner    (1001) docker     (123)    10220 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/data/transforms/item.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:10:14.997691 hf-deepali-0.3.2/src/deepali/losses/
--rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7721 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/losses/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/losses/bspline.py
--rw-r--r--   0 runner    (1001) docker     (123)     6510 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/losses/flow.py
--rw-r--r--   0 runner    (1001) docker     (123)    66444 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/losses/functional.py
--rw-r--r--   0 runner    (1001) docker     (123)    13371 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/losses/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/losses/params.py
--rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/losses/pointset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:10:15.001691 hf-deepali-0.3.2/src/deepali/modules/
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/modules/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/modules/flow.py
--rw-r--r--   0 runner    (1001) docker     (123)     4478 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/modules/image.py
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/modules/lambd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/modules/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/modules/output.py
--rw-r--r--   0 runner    (1001) docker     (123)    14625 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/modules/sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/modules/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:10:15.001691 hf-deepali-0.3.2/src/deepali/networks/
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/networks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:10:15.001691 hf-deepali-0.3.2/src/deepali/networks/blocks/
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/networks/blocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15305 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/networks/blocks/residual.py
--rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/networks/blocks/skip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:10:15.005691 hf-deepali-0.3.2/src/deepali/networks/layers/
--rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/networks/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5029 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/networks/layers/acti.py
--rw-r--r--   0 runner    (1001) docker     (123)    15670 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/networks/layers/conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/networks/layers/join.py
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/networks/layers/lambd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/networks/layers/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     6239 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/networks/layers/norm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4590 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/networks/layers/pool.py
--rw-r--r--   0 runner    (1001) docker     (123)    18748 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/networks/layers/upsample.py
--rw-r--r--   0 runner    (1001) docker     (123)    19757 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/networks/resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    42873 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/networks/unet.py
--rw-r--r--   0 runner    (1001) docker     (123)     6251 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/networks/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:10:15.005691 hf-deepali-0.3.2/src/deepali/spatial/
--rw-r--r--   0 runner    (1001) docker     (123)     8561 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/spatial/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22600 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/spatial/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    13325 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/spatial/bspline.py
--rw-r--r--   0 runner    (1001) docker     (123)    14024 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/spatial/composite.py
--rw-r--r--   0 runner    (1001) docker     (123)    16517 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/spatial/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/spatial/image.py
--rw-r--r--   0 runner    (1001) docker     (123)    29197 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/spatial/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)    12595 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/spatial/nonrigid.py
--rw-r--r--   0 runner    (1001) docker     (123)    17025 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/spatial/parametric.py
--rw-r--r--   0 runner    (1001) docker     (123)    12248 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/spatial/transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:10:15.005691 hf-deepali-0.3.2/src/deepali/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:10:15.009692 hf-deepali-0.3.2/src/deepali/utils/aws/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/utils/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15321 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/utils/aws/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:10:15.009692 hf-deepali-0.3.2/src/deepali/utils/aws/s3/
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/utils/aws/s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21551 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/utils/aws/s3/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/utils/aws/s3/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    10203 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/utils/aws/s3/object.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:10:15.009692 hf-deepali-0.3.2/src/deepali/utils/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/utils/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13233 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/utils/cli/argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/utils/cli/environ.py
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/utils/cli/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/utils/cli/warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:10:15.009692 hf-deepali-0.3.2/src/deepali/utils/ignite/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/utils/ignite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13542 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/utils/ignite/handlers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:10:15.009692 hf-deepali-0.3.2/src/deepali/utils/ignite/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/utils/ignite/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/utils/ignite/metrics/average_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/utils/ignite/metrics/binary_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/utils/ignite/metrics/multilabel_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)     6641 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/utils/ignite/output_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/utils/ignite/score_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:10:15.013692 hf-deepali-0.3.2/src/deepali/utils/sitk/
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/utils/sitk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11201 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/utils/sitk/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/utils/sitk/imageio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/utils/sitk/numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     6195 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/utils/sitk/sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/utils/sitk/torch.py
--rw-r--r--   0 runner    (1001) docker     (123)     6660 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/utils/tensorboard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:10:15.013692 hf-deepali-0.3.2/src/deepali/utils/vtk/
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/utils/vtk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/utils/vtk/idlist.py
--rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/utils/vtk/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/utils/vtk/numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/utils/vtk/polydataio.py
--rw-r--r--   0 runner    (1001) docker     (123)     5933 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/src/deepali/utils/vtk/simpleitk.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:10:15.013692 hf-deepali-0.3.2/src/hf_deepali.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10941 2023-07-07 02:10:14.000000 hf-deepali-0.3.2/src/hf_deepali.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6060 2023-07-07 02:10:14.000000 hf-deepali-0.3.2/src/hf_deepali.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 02:10:14.000000 hf-deepali-0.3.2/src/hf_deepali.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-07 02:10:14.000000 hf-deepali-0.3.2/src/hf_deepali.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-07 02:10:14.000000 hf-deepali-0.3.2/src/hf_deepali.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 02:10:15.017692 hf-deepali-0.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5659 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/tests/_test_core_bspline.py
--rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/tests/test_core_bspline.py
--rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/tests/test_core_cube.py
--rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/tests/test_core_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     4518 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/tests/test_core_image_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4027 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/tests/test_core_random.py
--rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/tests/test_core_tensor_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8564 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/tests/test_data_flow.py
--rw-r--r--   0 runner    (1001) docker     (123)    23869 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/tests/test_data_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     6038 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/tests/test_network_blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)    11278 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/tests/test_network_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/tests/test_network_resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-07-07 02:09:56.000000 hf-deepali-0.3.2/tests/test_network_unet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:47:07.030537 hf-deepali-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:47:06.994537 hf-deepali-0.4.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:47:06.998537 hf-deepali-0.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:47:07.002537 hf-deepali-0.4.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10941 2023-07-20 21:47:07.030537 hf-deepali-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9791 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/TODO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:47:07.002537 hf-deepali-0.4.0/conda/
+-rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/conda/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/conda/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)   550833 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/conda/environment.conda-lock.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/conda/environment.devenv.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    53576 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/conda/environment.linux-64.lock
+-rw-r--r--   0 runner    (1001) docker     (123)    15553 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/conda/environment.linux-64.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    45592 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/conda/environment.osx-64.lock
+-rw-r--r--   0 runner    (1001) docker     (123)    13443 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/conda/environment.osx-64.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    48151 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/conda/environment.win-64.lock
+-rw-r--r--   0 runner    (1001) docker     (123)    14217 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/conda/environment.win-64.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:47:07.002537 hf-deepali-0.4.0/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/docker/Dockerfile
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1699 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/docker/build
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7011 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/docker/run
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:47:07.002537 hf-deepali-0.4.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/docs/_citations.bib
+-rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/docs/_config.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:47:07.006537 hf-deepali-0.4.0/docs/_images/
+-rw-r--r--   0 runner    (1001) docker     (123)   390208 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/docs/_images/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/docs/_toc.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:47:07.006537 hf-deepali-0.4.0/docs/basics/
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/docs/basics/example-page.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/docs/basics/installation.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:47:06.994537 hf-deepali-0.4.0/docs/reference/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:47:07.006537 hf-deepali-0.4.0/docs/reference/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/docs/reference/core/domain.md
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/docs/reference/core/flow.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/docs/reference/core/image.md
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/docs/reference/core/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/docs/reference/core/kernels.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:47:07.006537 hf-deepali-0.4.0/docs/reference/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/docs/reference/data/dataset.md
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/docs/reference/data/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/docs/reference/data/sampler.md
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/docs/reference/data/tensor.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/docs/reference/data/transforms.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:47:07.006537 hf-deepali-0.4.0/docs/reference/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/docs/reference/losses/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:47:07.006537 hf-deepali-0.4.0/docs/reference/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/docs/reference/modules/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:47:07.006537 hf-deepali-0.4.0/docs/reference/networks/
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/docs/reference/networks/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:47:07.006537 hf-deepali-0.4.0/docs/reference/spatial/
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/docs/reference/spatial/common.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/docs/reference/spatial/composite.md
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/docs/reference/spatial/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/docs/reference/spatial/transformer.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:47:07.006537 hf-deepali-0.4.0/docs/reference/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/docs/reference/utils/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:47:07.010537 hf-deepali-0.4.0/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/docs/tutorials/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/docs/tutorials/example-myst-notebook.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/docs/tutorials/example-notebook.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    45126 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/docs/tutorials/pairwise-registration-intro.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:47:07.010537 hf-deepali-0.4.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/examples/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:47:07.010537 hf-deepali-0.4.0/examples/ffd/
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/examples/ffd/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/examples/ffd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/examples/ffd/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5296 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/examples/ffd/engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/examples/ffd/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15655 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/examples/ffd/losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/examples/ffd/optim.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32029 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/examples/ffd/pairwise.py
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/examples/ffd/params.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5420 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/examples/ffd/register.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:47:07.010537 hf-deepali-0.4.0/examples/istn/
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/examples/istn/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/examples/istn/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:47:07.010537 hf-deepali-0.4.0/examples/istn/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/examples/istn/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/examples/istn/models/itn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23150 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/examples/istn/models/stn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/examples/istn/params.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/examples/istn/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    27820 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/examples/istn/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/pyrightconfig.json
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 21:47:07.030537 hf-deepali-0.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:47:06.998537 hf-deepali-0.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:47:06.998537 hf-deepali-0.4.0/src/deepali/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:47:07.014537 hf-deepali-0.4.0/src/deepali/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19990 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/core/_kornia.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20501 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/core/affine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17034 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/core/argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23034 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/core/bspline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/core/collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7377 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24560 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/core/cube.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8783 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/core/enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/core/environ.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20232 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/core/flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6674 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/core/functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74082 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/core/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78487 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/core/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/core/itertools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11673 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/core/kernels.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19580 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/core/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/core/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/core/math.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16779 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/core/nnutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6303 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/core/pathlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15209 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/core/pointset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/core/psutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5815 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/core/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/core/tempfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9342 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/core/tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/core/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:47:07.014537 hf-deepali-0.4.0/src/deepali/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4120 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/data/collate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19033 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/data/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24776 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/data/flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62290 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/data/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/data/partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/data/prepare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/data/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6687 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/data/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3824 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/data/tensor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:47:07.018537 hf-deepali-0.4.0/src/deepali/data/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/data/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16685 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/data/transforms/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10262 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/data/transforms/item.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:47:07.018537 hf-deepali-0.4.0/src/deepali/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7734 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/losses/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/losses/bspline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6513 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/losses/flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66499 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/losses/functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13384 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/losses/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/losses/params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2921 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/losses/pointset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:47:07.018537 hf-deepali-0.4.0/src/deepali/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/modules/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/modules/flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/modules/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/modules/lambd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/modules/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/modules/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14656 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/modules/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/modules/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:47:07.018537 hf-deepali-0.4.0/src/deepali/networks/
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/networks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:47:07.018537 hf-deepali-0.4.0/src/deepali/networks/blocks/
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/networks/blocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15316 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/networks/blocks/residual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3567 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/networks/blocks/skip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:47:07.022537 hf-deepali-0.4.0/src/deepali/networks/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/networks/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5029 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/networks/layers/acti.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15589 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/networks/layers/conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/networks/layers/join.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/networks/layers/lambd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/networks/layers/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6239 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/networks/layers/norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4590 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/networks/layers/pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18771 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/networks/layers/upsample.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19788 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/networks/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42916 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/networks/unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6198 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/networks/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:47:07.022537 hf-deepali-0.4.0/src/deepali/spatial/
+-rw-r--r--   0 runner    (1001) docker     (123)     8567 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/spatial/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22608 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/spatial/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13362 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/spatial/bspline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14042 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/spatial/composite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16560 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/spatial/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/spatial/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29233 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/spatial/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12619 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/spatial/nonrigid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17031 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/spatial/parametric.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12273 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/spatial/transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:47:07.022537 hf-deepali-0.4.0/src/deepali/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:47:07.022537 hf-deepali-0.4.0/src/deepali/utils/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/utils/aws/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:47:07.022537 hf-deepali-0.4.0/src/deepali/utils/aws/s3/
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/utils/aws/s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21866 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/utils/aws/s3/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/utils/aws/s3/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10890 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/utils/aws/s3/object.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:47:07.026538 hf-deepali-0.4.0/src/deepali/utils/ignite/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/utils/ignite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13571 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/utils/ignite/handlers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:47:07.026538 hf-deepali-0.4.0/src/deepali/utils/ignite/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/utils/ignite/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/utils/ignite/metrics/average_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/utils/ignite/metrics/binary_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/utils/ignite/metrics/multilabel_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6691 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/utils/ignite/output_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/utils/ignite/score_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:47:07.026538 hf-deepali-0.4.0/src/deepali/utils/imageio/
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/utils/imageio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15784 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/utils/imageio/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4480 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/utils/imageio/nifti.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/utils/imageio/sitk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/utils/ipython.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:47:07.026538 hf-deepali-0.4.0/src/deepali/utils/simpleitk/
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/utils/simpleitk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13664 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/utils/simpleitk/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/utils/simpleitk/imageio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/utils/simpleitk/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6246 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/utils/simpleitk/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/utils/simpleitk/torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13159 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/utils/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6661 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/utils/tensorboard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:47:07.026538 hf-deepali-0.4.0/src/deepali/utils/vtk/
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/utils/vtk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/utils/vtk/idlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/utils/vtk/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/utils/vtk/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/utils/vtk/polydataio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5988 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/src/deepali/utils/vtk/simpleitk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:47:07.030537 hf-deepali-0.4.0/src/hf_deepali.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10941 2023-07-20 21:47:06.000000 hf-deepali-0.4.0/src/hf_deepali.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6310 2023-07-20 21:47:06.000000 hf-deepali-0.4.0/src/hf_deepali.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 21:47:06.000000 hf-deepali-0.4.0/src/hf_deepali.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-20 21:47:06.000000 hf-deepali-0.4.0/src/hf_deepali.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-20 21:47:06.000000 hf-deepali-0.4.0/src/hf_deepali.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:47:07.030537 hf-deepali-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5659 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/tests/_test_core_bspline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/tests/test_core_bspline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/tests/test_core_cube.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/tests/test_core_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4518 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/tests/test_core_image_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4027 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/tests/test_core_random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/tests/test_core_tensor_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8564 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/tests/test_data_flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23869 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/tests/test_data_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6038 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/tests/test_network_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11273 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/tests/test_network_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/tests/test_network_resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/tests/test_network_unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-07-20 21:46:49.000000 hf-deepali-0.4.0/tests/test_utils_imageio_meta.py
```

### Comparing `hf-deepali-0.3.2/.github/workflows/docs.yml` & `hf-deepali-0.4.0/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.2/.github/workflows/release.yml` & `hf-deepali-0.4.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.2/.github/workflows/tests.yml` & `hf-deepali-0.4.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.2/.gitignore` & `hf-deepali-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.2/.vscode/extensions.json` & `hf-deepali-0.4.0/.vscode/extensions.json`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.2/.vscode/launch.json` & `hf-deepali-0.4.0/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.2/.vscode/settings.json` & `hf-deepali-0.4.0/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.2/CODE_OF_CONDUCT.md` & `hf-deepali-0.4.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.2/LICENSE` & `hf-deepali-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.2/PKG-INFO` & `hf-deepali-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hf-deepali
-Version: 0.3.2
+Version: 0.4.0
 Summary: Image, point set, and surface registration library for PyTorch.
 Maintainer-email: Andreas Schuh <andreas.schuh@imperial.ac.uk>
 License: Apache-2.0
 Project-URL: Homepage, https://biomedia.github.io/deepali
 Project-URL: Repository, https://github.com/BioMedIA/deepali.git
 Project-URL: Bug Tracker, https://github.com/BioMedIA/deepali/issues
 Keywords: medical-imaging,image-registration,spatial-transformer-networks
```

### Comparing `hf-deepali-0.3.2/README.md` & `hf-deepali-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.2/TODO` & `hf-deepali-0.4.0/TODO`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.2/conda/Makefile` & `hf-deepali-0.4.0/conda/Makefile`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.2/conda/README.md` & `hf-deepali-0.4.0/conda/README.md`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.2/conda/environment.conda-lock.yml` & `hf-deepali-0.4.0/conda/environment.conda-lock.yml`

 * *Files 1% similar despite different names*

```diff
@@ -17,17 +17,17 @@
   - url: pytorch
     used_env_vars: []
   - url: nvidia
     used_env_vars: []
   - url: nodefaults
     used_env_vars: []
   content_hash:
-    linux-64: 8bbc0023a299b67380a6493155cba6c46fd177739fbaea7c67b86663b42d8354
-    osx-64: 1664d2c199c9cddb402252a38f5527d218754e954cbb25a82da7fecc8cbae3f6
-    win-64: fe02ca598f6ebbae4e65d2a2d45af1db4913dae4b25d021473f905afc52e3198
+    linux-64: c6bd68ba63788a00937c8cd1d91bb1e5813d242d7089005156ab1a663f53aee1
+    osx-64: 533a7567b393584157366e71374225596e814fe74cfcb03642d3b4e184d58c87
+    win-64: 6255d416b6866feefaa84cbaf27b3a7608f8bb60e8d5e51ca00574e0f3970f20
   platforms:
   - linux-64
   - osx-64
   - win-64
   sources:
   - environment.devenv.linux-64.yml
   - environment.devenv.osx-64.yml
@@ -456,25 +456,25 @@
   name: double-conversion
   optional: false
   platform: linux-64
   url: https://conda.anaconda.org/conda-forge/linux-64/double-conversion-3.2.0-h27087fc_1.tar.bz2
   version: 3.2.0
 - category: main
   dependencies:
-    libgcc-ng: '>=9.4.0'
-    libstdcxx-ng: '>=9.4.0'
+    libgcc-ng: '>=12'
+    libstdcxx-ng: '>=12'
   hash:
-    md5: 61af675be1ebd2ab75ebc70b8687b84d
-    sha256: f3ab736a612088dc99b1ff70ddd92e331020c3b3514a21293d15eed902def775
+    md5: c2acfc9bc0d0c53f83bbf0f582cb0e7a
+    sha256: 1dfe42f82ccd06ca4b19cfbbef483385f284be90f6b40c26831004b192c98bda
   manager: conda
   name: eigen
   optional: false
   platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/eigen-3.4.0-h4bd325d_0.tar.bz2
-  version: 3.4.0
+  url: https://conda.anaconda.org/conda-forge/linux-64/eigen-3.4.1-h00ab1b0_0.conda
+  version: 3.4.1
 - category: main
   dependencies:
     libgcc-ng: '>=12'
     libgfortran-ng: ''
     libgfortran5: '>=11.4.0'
     libstdcxx-ng: '>=12'
   hash:
@@ -1549,21 +1549,21 @@
   version: 4.2.0
 - category: main
   dependencies:
     libgcc-ng: '>=12'
     libstdcxx-ng: '>=12'
     openssl: '>=3.1.1,<4.0a0'
   hash:
-    md5: b241363e3b72bae6dfbd31e9fecf7d26
-    sha256: 0ec502aaee1b9cb82947a1f56ad599d2ac79c9c25ccf2f44224a69e1e16f537e
+    md5: a55ff0ed12efd86cf3a3dfb750adb950
+    sha256: edc73f41509b41b2c907c82443a5c44fd44219012cdbf15042d93d16affe91ab
   manager: conda
   name: mysql-common
   optional: false
   platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/mysql-common-8.0.33-hf1915f5_1.conda
+  url: https://conda.anaconda.org/conda-forge/linux-64/mysql-common-8.0.33-hf1915f5_2.conda
   version: 8.0.33
 - category: main
   dependencies:
     libffi: '>=3.4.2,<3.5.0a0'
     libgcc-ng: '>=12'
     libtasn1: '>=4.18.0,<5.0a0'
   hash:
@@ -1671,21 +1671,21 @@
   version: 1.2.13
 - category: main
   dependencies:
     libgcc-ng: '>=12'
     libstdcxx-ng: '>=12'
     libzlib: '>=1.2.13,<1.3.0a0'
   hash:
-    md5: 6b63daed8feeca47be78f323e793d555
-    sha256: fbe49a8c8df83c2eccb37c5863ad98baeb29796ec96f2c503783d7b89bf80c98
+    md5: 32ae18eb2a687912fc9e92a501c0a11b
+    sha256: a7f7e765dfb7af5265a38080e46f18cb07cfeecf81fe28fad23c4538e7d521c3
   manager: conda
   name: zstd
   optional: false
   platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/zstd-1.5.2-h3eb15da_6.conda
+  url: https://conda.anaconda.org/conda-forge/linux-64/zstd-1.5.2-hfc55251_7.conda
   version: 1.5.2
 - category: main
   dependencies:
     libbrotlidec: 1.0.9 h166bdaf_9
     libbrotlienc: 1.0.9 h166bdaf_9
     libgcc-ng: '>=12'
   hash:
@@ -1805,41 +1805,41 @@
     libffi: '>=3.4,<4.0a0'
     libgcc-ng: '>=12'
     libiconv: '>=1.17,<2.0a0'
     libstdcxx-ng: '>=12'
     libzlib: '>=1.2.13,<1.3.0a0'
     pcre2: '>=10.40,<10.41.0a0'
   hash:
-    md5: a64f11b244b2c112cd3fa1cbe9493999
-    sha256: 6a34c6b123f06fcee7e28e981ec0daad09bce35616ad8e9e61ef84be7fad4d92
+    md5: c6f951789c888f7bbd2dd6858eab69de
+    sha256: e909b5e648d1ace172aac2ddf9d755f72429b134155a9b07156acb58a77ceee1
   manager: conda
   name: libglib
   optional: false
   platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/libglib-2.76.3-hebfc3b9_0.conda
-  version: 2.76.3
+  url: https://conda.anaconda.org/conda-forge/linux-64/libglib-2.76.4-hebfc3b9_0.conda
+  version: 2.76.4
 - category: main
   dependencies:
     c-ares: '>=1.19.1,<2.0a0'
     libabseil: '>=20230125.3,<20230126.0a0'
     libgcc-ng: '>=12'
     libprotobuf: '>=4.23.3,<4.23.4.0a0'
     libstdcxx-ng: '>=12'
     libzlib: '>=1.2.13,<1.3.0a0'
     openssl: '>=3.1.1,<4.0a0'
     re2: '>=2023.3.2,<2023.3.3.0a0'
   hash:
-    md5: 6cf9ef21c7ef12df628bf46ad67189d3
-    sha256: f50ab3e6577d1ed3408b5f2a6352fc26bdab3b959dacf0ca93001cf33d35d5f0
+    md5: a87e780f3d9cc7cf432e47ced83a67ce
+    sha256: 6790a521ac39d267955cd71a5d45a3045c2c76591cab094a7dcbde7445d303a4
   manager: conda
   name: libgrpc
   optional: false
   platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/libgrpc-1.56.0-h3905398_2.conda
-  version: 1.56.0
+  url: https://conda.anaconda.org/conda-forge/linux-64/libgrpc-1.56.2-h3905398_0.conda
+  version: 1.56.2
 - category: main
   dependencies:
     libgcc-ng: '>=12'
     libstdcxx-ng: '>=12'
     libxml2: '>=2.10.3,<2.11.0a0'
   hash:
     md5: a3ede1b8e47f993ff1fe3908b23bb307
@@ -1979,25 +1979,25 @@
   url: https://conda.anaconda.org/conda-forge/linux-64/mpc-1.3.1-hfe3b2da_0.conda
   version: 1.3.1
 - category: main
   dependencies:
     libgcc-ng: '>=12'
     libstdcxx-ng: '>=12'
     libzlib: '>=1.2.13,<1.3.0a0'
-    mysql-common: 8.0.33 hf1915f5_1
+    mysql-common: 8.0.33 hf1915f5_2
     openssl: '>=3.1.1,<4.0a0'
     zstd: '>=1.5.2,<1.6.0a0'
   hash:
-    md5: a04ac37f0659929f3ba0f33c7f3d750f
-    sha256: d10f737f835a90d441c5cc0c15e46b4d34594a080f67a1e6cd64ac76bf3e6269
+    md5: b2f09078f50b9e859aca3f0dc1cc8b7e
+    sha256: f4d396571cbaee6074063d4f46fb6f37b70caed68376cd5af14b9c2f2a90926b
   manager: conda
   name: mysql-libs
   optional: false
   platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/mysql-libs-8.0.33-hca2cd23_1.conda
+  url: https://conda.anaconda.org/conda-forge/linux-64/mysql-libs-8.0.33-hca2cd23_2.conda
   version: 8.0.33
 - category: main
   dependencies:
     __glibc: '>=2.17,<3.0.a0'
     libgcc-ng: '>=12'
     libsqlite: '>=3.40.0,<4.0a0'
     libstdcxx-ng: '>=12'
@@ -2260,35 +2260,35 @@
   platform: linux-64
   url: https://conda.anaconda.org/conda-forge/noarch/certifi-2023.5.7-pyhd8ed1ab_0.conda
   version: 2023.5.7
 - category: main
   dependencies:
     python: '>=3.7'
   hash:
-    md5: 7fcff9f6f123696e940bda77bd4d6551
-    sha256: 06cd371fc98f076797d6450f6f337cb679b1060c99680fb7e044591493333194
+    md5: 313516e9a4b08b12dfb1e1cd390a96e3
+    sha256: 0666a95fbbd2299008162e2126c009191e5953d1cad1878bf9f4d8d634af1dd4
   manager: conda
   name: charset-normalizer
   optional: false
   platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-3.1.0-pyhd8ed1ab_0.conda
-  version: 3.1.0
+  url: https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-3.2.0-pyhd8ed1ab_0.conda
+  version: 3.2.0
 - category: main
   dependencies:
     __unix: ''
     python: '>=3.8'
   hash:
-    md5: 20e4087407c7cb04a40817114b333dbf
-    sha256: 23676470b591b100393bb0f6c46fe10624dcbefc696a6a9f42932ed8816ef0ea
+    md5: 64dbb3b205546691a61204d1cfb208e3
+    sha256: 73392cf4851bf7c89e99518effea01d531360a4894c4218e768d5e03e89d7943
   manager: conda
   name: click
   optional: false
   platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/noarch/click-8.1.3-unix_pyhd8ed1ab_2.tar.bz2
-  version: 8.1.3
+  url: https://conda.anaconda.org/conda-forge/noarch/click-8.1.6-unix_pyh707e725_0.conda
+  version: 8.1.6
 - category: main
   dependencies:
     python: '>=3.7'
   hash:
     md5: 3faab06a954c2a04039983f2c4a50d99
     sha256: 2c1b2e9755ce3102bca8d69e8f26e4f087ece73f50418186aee7c74bef8e1698
   manager: conda
@@ -2465,22 +2465,22 @@
   version: 2.14.2
 - category: main
   dependencies:
     libgcc-ng: '>=12'
     python: '>=3.10,<3.11.0a0'
     python_abi: 3.10.* *_cp310
   hash:
-    md5: 25e1626333f9a0646579a162e7b174ee
-    sha256: 1a213bfa274e847d08cf0d8b068dc94be002c9f17acd040b5c9f2ead80c3c7c0
+    md5: e239a69f354349af1117e336dd124067
+    sha256: 36246402e402b5cd55ee3b216fc9a07591f554c46aabc50dcabd4607f6a33e94
   manager: conda
   name: frozenlist
   optional: false
   platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/frozenlist-1.3.3-py310h5764c6d_0.tar.bz2
-  version: 1.3.3
+  url: https://conda.anaconda.org/conda-forge/linux-64/frozenlist-1.4.0-py310h2372a71_0.conda
+  version: 1.4.0
 - category: main
   dependencies:
     python: '>=3.8'
   hash:
     md5: 50ea2067ec92dfcc38b4f07992d7e235
     sha256: 0015e12d85b454ca8e09085e9e788a6156f4f1da1b270019cab2658381d60258
   manager: conda
@@ -2506,26 +2506,26 @@
   optional: false
   platform: linux-64
   url: https://conda.anaconda.org/conda-forge/linux-64/gdk-pixbuf-2.42.8-hff1cb4f_1.tar.bz2
   version: 2.42.8
 - category: main
   dependencies:
     libgcc-ng: '>=12'
-    libglib: 2.76.3 hebfc3b9_0
+    libglib: 2.76.4 hebfc3b9_0
     libstdcxx-ng: '>=12'
     libzlib: '>=1.2.13,<1.3.0a0'
   hash:
-    md5: 8951eedf3cdf94dd733c1b5eee1f4880
-    sha256: 22882b3516eee26fc0482ad85b0c697ab8be4f345e238b60891866758392ebb6
+    md5: 76ac435b8668f636a39fcb155c3543fd
+    sha256: 6940a5d60d1fd8a14e8597e1e65e1a6e3a811368f279d4a2ab66ed73a2c26b31
   manager: conda
   name: glib-tools
   optional: false
   platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/glib-tools-2.76.3-hfc55251_0.conda
-  version: 2.76.3
+  url: https://conda.anaconda.org/conda-forge/linux-64/glib-tools-2.76.4-hfc55251_0.conda
+  version: 2.76.4
 - category: main
   dependencies:
     gmp: '>=6.2.1,<7.0a0'
     libgcc-ng: '>=12'
     mpc: '>=1.2.1,<2.0a0'
     mpfr: '>=4.1.0,<5.0a0'
     python: '>=3.10,<3.11.0a0'
@@ -2553,28 +2553,28 @@
   optional: false
   platform: linux-64
   url: https://conda.anaconda.org/conda-forge/linux-64/greenlet-2.0.2-py310hc6cd4ac_1.conda
   version: 2.0.2
 - category: main
   dependencies:
     libgcc-ng: '>=12'
-    libgrpc: 1.56.0 h3905398_2
+    libgrpc: 1.56.2 h3905398_0
     libstdcxx-ng: '>=12'
     libzlib: '>=1.2.13,<1.3.0a0'
     python: '>=3.10,<3.11.0a0'
     python_abi: 3.10.* *_cp310
   hash:
-    md5: 78282ea7b261ed53a615faba16532e82
-    sha256: ecd0f91a9cf71fb9bd4790b9ddc7028e519dd36291afd5c2a763e9cfaf60dcb0
+    md5: 0828bcffd8123a89f688e83ba95a356b
+    sha256: d7f8af86e0827f03accb32b811ff16f9f9c22eac1666f9dffb17873c62e43ad5
   manager: conda
   name: grpcio
   optional: false
   platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/grpcio-1.56.0-py310h1b8f574_2.conda
-  version: 1.56.0
+  url: https://conda.anaconda.org/conda-forge/linux-64/grpcio-1.56.2-py310h1b8f574_0.conda
+  version: 1.56.2
 - category: main
   dependencies:
     libgcc-ng: '>=12'
     libglib: '>=2.76.3,<3.0a0'
     libstdcxx-ng: '>=12'
   hash:
     md5: 4d8df0b0db060d33c9a702ada998a8fe
@@ -3047,22 +3047,22 @@
   platform: linux-64
   url: https://conda.anaconda.org/conda-forge/noarch/ply-3.11-py_1.tar.bz2
   version: '3.11'
 - category: main
   dependencies:
     python: '>=3.6'
   hash:
-    md5: 95c5be3c7cbd872509d16c216617fdab
-    sha256: eb11fd8b927d9c5ff9482cfbd6cd810a43a1351c44a288e9680542ea698a19a0
+    md5: 02153b6b760bbec00cfe9e4c97993d06
+    sha256: a149184fde856dba7968fc50ca89dbb07ebe84abd710d4076e2fada1b9399231
   manager: conda
   name: prometheus_client
   optional: false
   platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/noarch/prometheus_client-0.17.0-pyhd8ed1ab_0.conda
-  version: 0.17.0
+  url: https://conda.anaconda.org/conda-forge/noarch/prometheus_client-0.17.1-pyhd8ed1ab_0.conda
+  version: 0.17.1
 - category: main
   dependencies:
     libgcc-ng: '>=12'
     python: '>=3.10,<3.11.0a0'
     python_abi: 3.10.* *_cp310
   hash:
     md5: b0f0a014fc04012c05f39df15fe270ce
@@ -3157,34 +3157,34 @@
   platform: linux-64
   url: https://conda.anaconda.org/conda-forge/noarch/pygments-2.15.1-pyhd8ed1ab_0.conda
   version: 2.15.1
 - category: main
   dependencies:
     python: '>=3.6'
   hash:
-    md5: 99e28be5a278e2319834d7dc99e7bfdd
-    sha256: f3a64306fa0f405f10f4108d7ff42043d6fd393f940f9e98e395a3756687fc98
+    md5: 912c0194f898fdb783021fd25f913c31
+    sha256: 88ac94c42ade15113397e30d1831dd341399b5262fb5330b9240f915c33cd232
   manager: conda
   name: pyjwt
   optional: false
   platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/noarch/pyjwt-2.7.0-pyhd8ed1ab_0.conda
-  version: 2.7.0
+  url: https://conda.anaconda.org/conda-forge/noarch/pyjwt-2.8.0-pyhd8ed1ab_0.conda
+  version: 2.8.0
 - category: main
   dependencies:
     python: '>=3.6'
   hash:
-    md5: d3ed087d1f7f8f5590e8e87b57a8ce64
-    sha256: 18e3bd52c64f23bbc7c200fd2fc4152dd29423936dc43e8f129cb43f1af0136c
+    md5: e8fbc1b54b25f4b08281467bc13b70cc
+    sha256: 4acc7151cef5920d130f2e0a7615559cce8bfb037aeecb14d4d359ae3d9bc51b
   manager: conda
   name: pyparsing
   optional: false
   platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/noarch/pyparsing-3.1.0-pyhd8ed1ab_0.conda
-  version: 3.1.0
+  url: https://conda.anaconda.org/conda-forge/noarch/pyparsing-3.0.9-pyhd8ed1ab_0.tar.bz2
+  version: 3.0.9
 - category: main
   dependencies:
     libgcc-ng: '>=12'
     python: '>=3.10,<3.11.0a0'
     python_abi: 3.10.* *_cp310
   hash:
     md5: f732bec05ecc2e302a868d971ae484e0
@@ -3309,14 +3309,28 @@
   name: rfc3986-validator
   optional: false
   platform: linux-64
   url: https://conda.anaconda.org/conda-forge/noarch/rfc3986-validator-0.1.1-pyh9f0ad1d_0.tar.bz2
   version: 0.1.1
 - category: main
   dependencies:
+    libgcc-ng: '>=12'
+    python: '>=3.10,<3.11.0a0'
+    python_abi: 3.10.* *_cp310
+  hash:
+    md5: 2f9b517412af46255cef5e53a22c264e
+    sha256: 4a74013e0e9dd6fa984a10edb53276cf42308d99404375b81548af019bfd068d
+  manager: conda
+  name: ruamel.yaml.clib
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/ruamel.yaml.clib-0.2.7-py310h1fa729e_1.conda
+  version: 0.2.7
+- category: main
+  dependencies:
     __linux: ''
     python: '>=3.6'
   hash:
     md5: ada5a17adcd10be4fc7e37e4166ba0e2
     sha256: e74d3faf51a6cc429898da0209d95b209270160f3edbf2f6d8b61a99428301cd
   manager: conda
   name: send2trash
@@ -3561,22 +3575,22 @@
   platform: linux-64
   url: https://conda.anaconda.org/conda-forge/linux-64/typed-ast-1.5.5-py310h2372a71_0.conda
   version: 1.5.5
 - category: main
   dependencies:
     python: '>=3.7'
   hash:
-    md5: 4a3014a4d107d15475d106b751c4e352
-    sha256: 90a8d56c8015af1575d504d5f77d95a806cd999fc178a06ab51a349f1f744672
+    md5: c39d6a09fe819de4951c2642629d9115
+    sha256: 6edd6d5be690be492712cb747b6d62707f0d0c34ef56eefc796d91e5a03187d1
   manager: conda
   name: typing_extensions
   optional: false
   platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.6.3-pyha770c72_0.conda
-  version: 4.6.3
+  url: https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.7.1-pyha770c72_0.conda
+  version: 4.7.1
 - category: main
   dependencies:
     python: '>=3.6.1'
   hash:
     md5: eb67e3cace64c66233e2d35949e20f92
     sha256: 9e3758b620397f56fb709f796969de436d63b7117897159619b87938e1f78739
   manager: conda
@@ -3647,21 +3661,21 @@
   platform: linux-64
   url: https://conda.anaconda.org/conda-forge/noarch/websocket-client-1.6.1-pyhd8ed1ab_0.conda
   version: 1.6.1
 - category: main
   dependencies:
     python: '>=3.7'
   hash:
-    md5: 49bb0d9e60ce1db25e151780331bb5f3
-    sha256: 79b4d29b0c004014a2abd5fc2c9fcd35cc6256222b960c2a317a27c4b0d8884d
+    md5: c95fac682453aeffa12db7ae5a721bec
+    sha256: e91cbb3c0ad9a9507dd030f5493831cb52da120329e0d0793711e8300a36db22
   manager: conda
   name: wheel
   optional: false
   platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/noarch/wheel-0.40.0-pyhd8ed1ab_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/wheel-0.40.0-pyhd8ed1ab_1.conda
   version: 0.40.0
 - category: main
   dependencies:
     python: '>=3.7'
   hash:
     md5: 2e9ebddf0b93d0fb203d0906b8052c4f
     sha256: a73d34f8169e206bccfb356c093ff5ced803b953bbcc1480ed27976f97598d68
@@ -3756,24 +3770,24 @@
   name: xorg-libxt
   optional: false
   platform: linux-64
   url: https://conda.anaconda.org/conda-forge/linux-64/xorg-libxt-1.3.0-hd590300_0.conda
   version: 1.3.0
 - category: main
   dependencies:
-    python: '>=3.7'
+    python: '>=3.8'
   hash:
-    md5: 13018819ca8f5b7cc675a8faf1f5fedf
-    sha256: 241de30545299be9bcea3addf8a2c22a3b3d4ba6730890e150ab690ac937a3d2
+    md5: 2da0451b54c4563c32490cb1b7cf68a1
+    sha256: 16d72127e150a3d5cbdc0b82c4069ef5be135c64bc99e71e7928507910669b41
   manager: conda
   name: zipp
   optional: false
   platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/noarch/zipp-3.15.0-pyhd8ed1ab_0.conda
-  version: 3.15.0
+  url: https://conda.anaconda.org/conda-forge/noarch/zipp-3.16.2-pyhd8ed1ab_0.conda
+  version: 3.16.2
 - category: main
   dependencies:
     pygments: ''
     python: '>=3.6'
   hash:
     md5: 46a2e6e3dfa718ce3492018d5a110dd6
     sha256: ce532e2da08fb2b77df281e3d42e2b2131641bdd6a6e8127f3718ae6860bd70d
@@ -3800,22 +3814,22 @@
   dependencies:
     exceptiongroup: ''
     idna: '>=2.8'
     python: '>=3.7'
     sniffio: '>=1.1'
     typing_extensions: ''
   hash:
-    md5: 2b35a85d654a47aac8f34c1bb6de7142
-    sha256: 863c11a6a0e937977229b405a16f6d43fff543dfe5b1a66da9c42ec0cbdaaf33
+    md5: 7b517e7a6f0790337906c055aa97ca49
+    sha256: 62637ac498bcf47783cbf4f48e9b09e4e2f5a6ad42f43ca8f632c353827b94f4
   manager: conda
   name: anyio
   optional: false
   platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/noarch/anyio-3.7.0-pyhd8ed1ab_1.conda
-  version: 3.7.0
+  url: https://conda.anaconda.org/conda-forge/noarch/anyio-3.7.1-pyhd8ed1ab_0.conda
+  version: 3.7.1
 - category: main
   dependencies:
     python: '>=3.5'
     six: ''
   hash:
     md5: bf7f54dd0f25c3f06ecb82a07341841a
     sha256: 7ed530efddd47a96c11197906b4008405b90e3bc2f4e0df722a36e0e6103fd9c
@@ -4001,22 +4015,22 @@
     brotli: ''
     libgcc-ng: '>=12'
     munkres: ''
     python: '>=3.10,<3.11.0a0'
     python_abi: 3.10.* *_cp310
     unicodedata2: '>=14.0.0'
   hash:
-    md5: d3d83b419c81ac718a9221442707882b
-    sha256: e5d22bcf75a4414d84000a3d905c70d4d2a1db96c0dfbf5a89169817351b2bb7
+    md5: 606aea800172f81896b21cabc5575206
+    sha256: b9e1a3b84c670fab1c491b29c6b36f630aa520f45f08a44440851f46750d85c1
   manager: conda
   name: fonttools
   optional: false
   platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/fonttools-4.40.0-py310h2372a71_0.conda
-  version: 4.40.0
+  url: https://conda.anaconda.org/conda-forge/linux-64/fonttools-4.41.0-py310h2372a71_0.conda
+  version: 4.41.0
 - category: main
   dependencies:
     libgcc-ng: '>=9.3.0'
     libglu: ''
     libstdcxx-ng: '>=9.3.0'
     xorg-libx11: ''
     xorg-libxext: ''
@@ -4028,29 +4042,29 @@
   optional: false
   platform: linux-64
   url: https://conda.anaconda.org/conda-forge/linux-64/glew-2.1.0-h9c3ff4c_2.tar.bz2
   version: 2.1.0
 - category: main
   dependencies:
     gettext: '>=0.21.1,<1.0a0'
-    glib-tools: 2.76.3 hfc55251_0
+    glib-tools: 2.76.4 hfc55251_0
     libgcc-ng: '>=12'
-    libglib: 2.76.3 hebfc3b9_0
+    libglib: 2.76.4 hebfc3b9_0
     libstdcxx-ng: '>=12'
     libzlib: '>=1.2.13,<1.3.0a0'
     python: '*'
   hash:
-    md5: 950e02f5665f5f4ff0437a6acba58798
-    sha256: c783d185d4f1296b9e9810f400b208d5e3a073198d753b3203ae83521941325d
+    md5: dbcec5fd9c6c8be24b23575048755a59
+    sha256: 85de9ec71a143e9b86e381e865341f2d706387f3d3facaf935d4598b6dfa7229
   manager: conda
   name: glib
   optional: false
   platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/glib-2.76.3-hfc55251_0.conda
-  version: 2.76.3
+  url: https://conda.anaconda.org/conda-forge/linux-64/glib-2.76.4-hfc55251_0.conda
+  version: 2.76.4
 - category: main
   dependencies:
     libaec: '>=1.0.6,<2.0a0'
     libcurl: '>=7.87.0,<9.0a0'
     libgcc-ng: '>=12'
     libgfortran-ng: ''
     libgfortran5: '>=10.4.0'
@@ -4067,35 +4081,35 @@
   url: https://conda.anaconda.org/conda-forge/linux-64/hdf5-1.12.2-nompi_h4df4325_101.conda
   version: 1.12.2
 - category: main
   dependencies:
     python: '>=3.8'
     zipp: '>=0.5'
   hash:
-    md5: ba3786c6846e46038fe60c785d46dc81
-    sha256: 1ffffc30dc67d8329d47c6d22de726cfd28d7ed236bca54f52fc0bdcd0a53fc7
+    md5: 4e9f59a060c3be52bc4ddc46ee9b6946
+    sha256: 2797ed927d65324309b6c630190d917b9f2111e0c217b721f80429aeb57f9fcf
   manager: conda
   name: importlib-metadata
   optional: false
   platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-6.7.0-pyha770c72_0.conda
-  version: 6.7.0
+  url: https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-6.8.0-pyha770c72_0.conda
+  version: 6.8.0
 - category: main
   dependencies:
-    python: '>=3.7'
+    python: '>=3.8'
     zipp: '>=3.1.0'
   hash:
-    md5: e5fd2260a231ee63b6969f4801082f2b
-    sha256: 091cca3e010f7a7353152f0abda2d68cfd83ddde80a15e974d9e18b2047e7be2
+    md5: a08b6be5bf18b9d2a927d3457750f82e
+    sha256: 94c1b2831c0f908ae56212d9aeb9c9173051d307682b4fedfd88fef774b0b8f7
   manager: conda
   name: importlib_resources
   optional: false
   platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/noarch/importlib_resources-5.12.0-pyhd8ed1ab_0.conda
-  version: 5.12.0
+  url: https://conda.anaconda.org/conda-forge/noarch/importlib_resources-6.0.0-pyhd8ed1ab_1.conda
+  version: 6.0.0
 - category: main
   dependencies:
     parso: '>=0.8.0,<0.9.0'
     python: '>=3.6'
   hash:
     md5: b5e695ef9c3f0d27d6cd96bf5adc9e07
     sha256: abe63ae6e1b13f83500608d94004cb8d485b264083511d77f79253e775cd546c
@@ -4490,14 +4504,30 @@
   optional: false
   platform: linux-64
   url: https://conda.anaconda.org/conda-forge/noarch/rsa-4.9-pyhd8ed1ab_0.tar.bz2
   version: '4.9'
 - category: main
   dependencies:
     libgcc-ng: '>=12'
+    python: '>=3.10,<3.11.0a0'
+    python_abi: 3.10.* *_cp310
+    ruamel.yaml.clib: '>=0.1.2'
+    setuptools: ''
+  hash:
+    md5: 9a03abf74d5069bda767c1bce7a41e0b
+    sha256: bdbd5b73bc92f3bd4eea8b8475d912a9d42562ed494163fd3987404f514beb70
+  manager: conda
+  name: ruamel.yaml
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/ruamel.yaml-0.17.32-py310h2372a71_0.conda
+  version: 0.17.32
+- category: main
+  dependencies:
+    libgcc-ng: '>=12'
     libstdcxx-ng: '>=12'
     packaging: ''
     ply: ''
     python: '>=3.10,<3.11.0a0'
     python_abi: 3.10.* *_cp310
     tomli: ''
   hash:
@@ -4577,24 +4607,24 @@
   name: tqdm
   optional: false
   platform: linux-64
   url: https://conda.anaconda.org/conda-forge/noarch/tqdm-4.65.0-pyhd8ed1ab_1.conda
   version: 4.65.0
 - category: main
   dependencies:
-    typing_extensions: 4.6.3 pyha770c72_0
+    typing_extensions: 4.7.1 pyha770c72_0
   hash:
-    md5: 3876f650ed7d0f95d70fa4b647621909
-    sha256: d2334dab270e13182403cc3a394e3da8e7acb409e94059a6d9223d2ac053f90a
+    md5: f96688577f1faa58096d06a45136afa2
+    sha256: d5d19b8f5b275240c19616a46d67ec57250b3720ba88200da8c732c3fcbfc21d
   manager: conda
   name: typing-extensions
   optional: false
   platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.6.3-hd8ed1ab_0.conda
-  version: 4.6.3
+  url: https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.7.1-hd8ed1ab_0.conda
+  version: 4.7.1
 - category: main
   dependencies:
     markupsafe: '>=2.1.1'
     python: '>=3.8'
   hash:
     md5: 55fbbb3e67185820ee2007395bfe0073
     sha256: 28515f7ddb8a20f1436b9ac3a6ba2aa9be337995e4ee63c72d0f5d0efd6a2062
@@ -4639,22 +4669,22 @@
   dependencies:
     lazy-object-proxy: '>=1.4.0'
     python: '>=3.10,<3.11.0a0'
     python_abi: 3.10.* *_cp310
     typing-extensions: '>=4.0.0'
     wrapt: <2,>=1.11
   hash:
-    md5: 1ed3ebb3837ac50a6bf762b44cf2315c
-    sha256: 8cdc0fccc2b657d5577737d31fa35fd38d5907d6235fb66d7e7fde9971779208
+    md5: 8ad02555d6ecdb8fd5f1963690c59699
+    sha256: 4fc0a7b5015ca87fad4cf49f4f371a0e58e3a47bd4a9ae032daf7759b7e94734
   manager: conda
   name: astroid
   optional: false
   platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/astroid-2.15.5-py310hff52083_0.conda
-  version: 2.15.5
+  url: https://conda.anaconda.org/conda-forge/linux-64/astroid-2.15.6-py310hff52083_0.conda
+  version: 2.15.6
 - category: main
   dependencies:
     python: '>=3.6'
     typing-extensions: '>=3.6.5'
   hash:
     md5: 25e79f9a1133556671becbd65a170c78
     sha256: a08b78e6fadee1ffac0f255363d2a08a0c589c7403fd2a71c1c0b6aafd5e0737
@@ -4683,22 +4713,22 @@
   dependencies:
     cffi: '>=1.12'
     libgcc-ng: '>=12'
     openssl: '>=3.1.1,<4.0a0'
     python: '>=3.10,<3.11.0a0'
     python_abi: 3.10.* *_cp310
   hash:
-    md5: bd5501a8ae0df5ef36b9ed03035ebe3a
-    sha256: b50152a7149abea394c771fba544a302831f11135a0d0dc676a73784176a8361
+    md5: 3e80a669e7a1890ebb91370f2e818129
+    sha256: 824ac449d3262e2374cb84e070d61be17f15c1d579fa68301ac050f1efa59a07
   manager: conda
   name: cryptography
   optional: false
   platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/cryptography-41.0.1-py310h75e40e8_0.conda
-  version: 41.0.1
+  url: https://conda.anaconda.org/conda-forge/linux-64/cryptography-41.0.2-py310h75e40e8_0.conda
+  version: 41.0.2
 - category: main
   dependencies:
     aom: '>=3.5.0,<3.6.0a0'
     bzip2: '>=1.0.8,<2.0a0'
     fontconfig: '>=2.14.1,<3.0a0'
     fonts-conda-ecosystem: ''
     freetype: '>=2.12.1,<3.0a0'
@@ -4771,24 +4801,24 @@
   name: harfbuzz
   optional: false
   platform: linux-64
   url: https://conda.anaconda.org/conda-forge/linux-64/harfbuzz-6.0.0-h8e241bc_0.conda
   version: 6.0.0
 - category: main
   dependencies:
-    importlib-metadata: '>=6.7.0,<6.7.1.0a0'
+    importlib-metadata: '>=6.8.0,<6.8.1.0a0'
   hash:
-    md5: 27a4cec373ec84d1c1aa02a1e37f8eaf
-    sha256: f46d34a06e63f220dd04f7ac211dd2b4812b6b8a9e851467cd2e0218174d2dfd
+    md5: b279b07ce18058034e5b3606ba103a8b
+    sha256: b96e01dc42d547d6d9ceb1c5b52a5232cc04e40153534350f702c3e0418a6b3f
   manager: conda
   name: importlib_metadata
   optional: false
   platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-6.7.0-hd8ed1ab_0.conda
-  version: 6.7.0
+  url: https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-6.8.0-hd8ed1ab_0.conda
+  version: 6.8.0
 - category: main
   dependencies:
     attrs: '>=17.4.0'
     importlib-metadata: ''
     importlib_resources: '>=1.4.0'
     pkgutil-resolve-name: '>=1.3.10'
     pyrsistent: '!=0.17.0,!=0.17.1,!=0.17.2,>=0.14.0'
@@ -4912,22 +4942,22 @@
   url: https://conda.anaconda.org/conda-forge/linux-64/mkl-devel-2022.1.0-ha770c72_916.tar.bz2
   version: 2022.1.0
 - category: main
   dependencies:
     python: '>=3.7'
     typing-extensions: '>=4.6.3'
   hash:
-    md5: 3e4aca765371893ad848397794600632
-    sha256: 5f382d0d3509784152506e0e022bb5a30d254555e809804491207196f890af67
+    md5: 044e7a1e0ad42c4e67110bd078150a63
+    sha256: 885611bd528abaf3e31bc0bfaad3a619cfe89db61d886b53c2a9ec9ff50edebe
   manager: conda
   name: platformdirs
   optional: false
   platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.8.0-pyhd8ed1ab_0.conda
-  version: 3.8.0
+  url: https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.9.1-pyhd8ed1ab_0.conda
+  version: 3.9.1
 - category: main
   dependencies:
     alsa-lib: '>=1.2.8,<1.2.9.0a0'
     dbus: '>=1.13.6,<2.0a0'
     fftw: '>=3.3.10,<4.0a0'
     gstreamer-orc: '>=0.4.33,<0.5.0a0'
     jack: '>=1.9.22,<1.10.0a0'
@@ -5020,22 +5050,22 @@
   dependencies:
     greenlet: '!=0.4.17'
     libgcc-ng: '>=12'
     python: '>=3.10,<3.11.0a0'
     python_abi: 3.10.* *_cp310
     typing-extensions: '>=4.2.0'
   hash:
-    md5: 5addfcf598875b2e4febacbc98aa2d29
-    sha256: 146012656f7ecc7e56871407f3509a2e8c050054bced89428d702ec6adad18bd
+    md5: 2460f5ca3ab3265b80ee06a1d4b5b374
+    sha256: 552dfa70a26967d5b52cba2dc2cfe3c06f8b1c8e8029f648b1297a5febab82a1
   manager: conda
   name: sqlalchemy
   optional: false
   platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/sqlalchemy-2.0.17-py310h2372a71_0.conda
-  version: 2.0.17
+  url: https://conda.anaconda.org/conda-forge/linux-64/sqlalchemy-2.0.19-py310h2372a71_0.conda
+  version: 2.0.19
 - category: main
   dependencies:
     asttokens: ''
     executing: ''
     pure_eval: ''
     python: '>=3.5'
   hash:
@@ -5069,22 +5099,22 @@
     frozenlist: '>=1.1.1'
     libgcc-ng: '>=12'
     multidict: '>=4.5,<7.0'
     python: '>=3.10,<3.11.0a0'
     python_abi: 3.10.* *_cp310
     yarl: '>=1.0,<2.0'
   hash:
-    md5: 05d01d95b7838f86796b18a80fd42584
-    sha256: 475f5618a9b6228bd1b5ac37c1866ff01d52c39d04fe2c53ddd3ae888f6d19a1
+    md5: 0b05c509a96d0bf4bb424fe184170795
+    sha256: 5cb7647fe64617424027125dab858b96cd0d7b91b1c39fbc7d508a500b7ba9c1
   manager: conda
   name: aiohttp
   optional: false
   platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/aiohttp-3.8.4-py310h2372a71_1.conda
-  version: 3.8.4
+  url: https://conda.anaconda.org/conda-forge/linux-64/aiohttp-3.8.5-py310h2372a71_0.conda
+  version: 3.8.5
 - category: main
   dependencies:
     argon2-cffi-bindings: ''
     flit-core: '>=3.4,<4'
     python: '>=3.6'
   hash:
     md5: a0b402db58f73aaab8ee0ca1025a362e
@@ -5390,40 +5420,40 @@
   dependencies:
     jsonschema: '>=2.6'
     jupyter_core: ''
     python: '>=3.8'
     python-fastjsonschema: ''
     traitlets: '>=5.1'
   hash:
-    md5: f525a01528c3eba1d381a232a6971c6a
-    sha256: 3c6be17e84dc71db605a9e088fa7af7d47edab45d15da8e2a2ab3f29ec5ec081
+    md5: 3ec35d84fc1775215061517eb4660693
+    sha256: d8b1ad3c219b39e5e325785606853ff1cd334769228490ac977b85aa95e94ba0
   manager: conda
   name: nbformat
   optional: false
   platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/noarch/nbformat-5.9.0-pyhd8ed1ab_0.conda
-  version: 5.9.0
+  url: https://conda.anaconda.org/conda-forge/noarch/nbformat-5.9.1-pyhd8ed1ab_0.conda
+  version: 5.9.1
 - category: main
   dependencies:
     libblas: '>=3.9.0,<4.0a0'
     libcblas: '>=3.9.0,<4.0a0'
     libgcc-ng: '>=12'
     liblapack: '>=3.9.0,<4.0a0'
     libstdcxx-ng: '>=12'
     python: '>=3.10,<3.11.0a0'
     python_abi: 3.10.* *_cp310
   hash:
-    md5: 03319f78e5c9c8d90c0110e2c6ed24f6
-    sha256: bee4c383e78effeccbf854636b174e7242cfb486daa5387cfa57963d3c65628e
+    md5: 3810cbf2635cb1d0edb97715d4ad74e7
+    sha256: 38ec15fe0afe9fb90bd50314ccd506f0e7d1642db0c7eb2b77627d448aa9ee6c
   manager: conda
   name: numpy
   optional: false
   platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/numpy-1.25.0-py310ha4c1d20_0.conda
-  version: 1.25.0
+  url: https://conda.anaconda.org/conda-forge/linux-64/numpy-1.25.1-py310ha4c1d20_0.conda
+  version: 1.25.1
 - category: main
   dependencies:
     prompt-toolkit: '>=3.0.39,<3.0.40.0a0'
   hash:
     md5: 4bbbe67d5df19db30f04b8e344dc9976
     sha256: 89f7fecc7355181dbc2ab851e668a2fce6aa4830b336a34c93b59bda93206270
   manager: conda
@@ -5627,14 +5657,29 @@
   name: nbclient
   optional: false
   platform: linux-64
   url: https://conda.anaconda.org/conda-forge/noarch/nbclient-0.7.4-pyhd8ed1ab_0.conda
   version: 0.7.4
 - category: main
   dependencies:
+    numpy: '>=1.19'
+    packaging: '>=17'
+    python: '>=3.10,<3.11.0a0'
+    python_abi: 3.10.* *_cp310
+  hash:
+    md5: 01c0095d68f52a2ebe4154974b668bef
+    sha256: d4a335babe7fd6ab3e32bc3601f096a805307b66e150d44c979bb3f6129adcb6
+  manager: conda
+  name: nibabel
+  optional: false
+  platform: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/nibabel-5.1.0-py310hff52083_2.conda
+  version: 5.1.0
+- category: main
+  dependencies:
     libgcc-ng: '>=12'
     libstdcxx-ng: '>=12'
     numpy: '>=1.21.6,<2.0a0'
     python: '>=3.10,<3.11.0a0'
     python-dateutil: '>=2.8.1'
     python_abi: 3.10.* *_cp310
     pytz: '>=2020.1'
@@ -5759,22 +5804,22 @@
     python: '>=3.6'
     pyu2f: '>=0.1.5'
     requests: '>=2.20.0,<3.0.0dev'
     rsa: '>=3.1.4,<5'
     six: '>=1.9.0'
     urllib3: <2.0
   hash:
-    md5: 8c5dd8609d314721d990c1d1fd607f81
-    sha256: 6b097ca9b31961d6a983f81dc295012e9c99c4c1a5a83a93ab2fcc6528af428f
+    md5: 5583192796d1ebcf39b1e3e0958aa259
+    sha256: 1a75b167cb01f533c01716bc663d4859a0d55d47dd96eebb39b5aa4b51205b44
   manager: conda
   name: google-auth
   optional: false
   platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/noarch/google-auth-2.21.0-pyh1a96a4e_0.conda
-  version: 2.21.0
+  url: https://conda.anaconda.org/conda-forge/noarch/google-auth-2.22.0-pyh1a96a4e_0.conda
+  version: 2.22.0
 - category: main
   dependencies:
     __linux: ''
     comm: '>=0.1.1'
     debugpy: '>=1.6.5'
     ipython: '>=7.23.1'
     jupyter_client: '>=6.1.12'
@@ -5825,28 +5870,28 @@
     freetype: '>=2.12.1,<3.0a0'
     kiwisolver: '>=1.0.1'
     libgcc-ng: '>=12'
     libstdcxx-ng: '>=12'
     numpy: '>=1.21.6,<2.0a0'
     packaging: '>=20.0'
     pillow: '>=6.2.0'
-    pyparsing: '>=2.3.1'
+    pyparsing: '>=2.3.1,<3.1'
     python: '>=3.10,<3.11.0a0'
     python-dateutil: '>=2.7'
     python_abi: 3.10.* *_cp310
     tk: '>=8.6.12,<8.7.0a0'
   hash:
-    md5: 68b2dd34c69d08b05a9db5e3596fe3ee
-    sha256: d2be8ac0a90aa12ba808f8777d1837b5aa983fc3c7c60c600e8fe6bd9352541c
+    md5: 9b55c9041c5a7f80f184a2cb05ec9663
+    sha256: 28ff078d33e18b52a455d58d24ab7b959b4db98411470afd5869f30fbb54250b
   manager: conda
   name: matplotlib-base
   optional: false
   platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/matplotlib-base-3.7.1-py310he60537e_0.conda
-  version: 3.7.1
+  url: https://conda.anaconda.org/conda-forge/linux-64/matplotlib-base-3.7.2-py310hf38f957_0.conda
+  version: 3.7.2
 - category: main
   dependencies:
     beautifulsoup4: ''
     bleach: ''
     defusedxml: ''
     entrypoints: '>=0.2.2'
     jinja2: '>=3.0'
@@ -5855,26 +5900,26 @@
     markupsafe: '>=2.0'
     mistune: '>=2.0.3,<4'
     nbclient: '>=0.5.0'
     nbformat: '>=5.1'
     packaging: ''
     pandocfilters: '>=1.4.1'
     pygments: '>=2.4.1'
-    python: '>=3.7'
+    python: '>=3.8'
     tinycss2: ''
     traitlets: '>=5.0'
   hash:
-    md5: 879782bde4bbdb4c7b5d4054504a20d5
-    sha256: cebfc8c620bdc950e92f72562d281fc57d696497e30bef5bc9e517be757b1c2f
+    md5: 32dde1678bb003c90d4bc0c2dbd21814
+    sha256: 76ad7689d35fe031459c422f142c9d8e7a02f6922049b7a0183fc70aaef02f0a
   manager: conda
   name: nbconvert-core
   optional: false
   platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/noarch/nbconvert-core-7.6.0-pyhd8ed1ab_0.conda
-  version: 7.6.0
+  url: https://conda.anaconda.org/conda-forge/noarch/nbconvert-core-7.7.1-pyhd8ed1ab_1.conda
+  version: 7.7.1
 - category: main
   dependencies:
     packaging: '>=20.0'
     platformdirs: '>=2.5.0'
     python: '>=3.7'
     requests: '>=2.19.0'
   hash:
@@ -6037,28 +6082,28 @@
   name: jupyter_server
   optional: false
   platform: linux-64
   url: https://conda.anaconda.org/conda-forge/noarch/jupyter_server-2.7.0-pyhd8ed1ab_0.conda
   version: 2.7.0
 - category: main
   dependencies:
-    matplotlib-base: '>=3.7.1,<3.7.2.0a0'
+    matplotlib-base: '>=3.7.2,<3.7.3.0a0'
     pyqt: '>=5.10'
     python: '>=3.10,<3.11.0a0'
     python_abi: 3.10.* *_cp310
     tornado: '>=5'
   hash:
-    md5: c2b60c44d38d32779006a15c2581f0d1
-    sha256: afa2e34dadad3e403e262b554f8e3e518f0ceb516711bf594f2693d4c7d6ac31
+    md5: 7e454b4a61754714a4a4d183641374da
+    sha256: 73abc4f8d301573e16e92e3a16b284162bc3e97498468cd863ad395ed1967d56
   manager: conda
   name: matplotlib
   optional: false
   platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/matplotlib-3.7.1-py310hff52083_0.conda
-  version: 3.7.1
+  url: https://conda.anaconda.org/conda-forge/linux-64/matplotlib-3.7.2-py310hff52083_0.conda
+  version: 3.7.2
 - category: main
   dependencies:
     docutils: '>=0.15,<0.20'
     jinja2: ''
     markdown-it-py: '>=1.0.0,<3.0.0'
     mdit-py-plugins: '>=0.3.1,<1'
     python: '>=3.7'
@@ -6072,26 +6117,26 @@
   name: myst-parser
   optional: false
   platform: linux-64
   url: https://conda.anaconda.org/conda-forge/noarch/myst-parser-0.18.1-pyhd8ed1ab_0.tar.bz2
   version: 0.18.1
 - category: main
   dependencies:
-    nbconvert-core: 7.6.0 pyhd8ed1ab_0
+    nbconvert-core: 7.7.1 pyhd8ed1ab_1
     pandoc: ''
-    python: '>=3.7'
+    python: '>=3.8'
   hash:
-    md5: e8172ca42f2869bb90185c9356899e81
-    sha256: 07204ee7a7f429aa30c78897629c79859a60ef77fd1c2b9d9a1ad084c144a84f
+    md5: 796b056965d7146bcac082fa2a83943d
+    sha256: b5b2823e7951a5ba41b1020b7cce109fec7f2ebe540234bf8a17c54615c2f679
   manager: conda
   name: nbconvert-pandoc
   optional: false
   platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/noarch/nbconvert-pandoc-7.6.0-pyhd8ed1ab_0.conda
-  version: 7.6.0
+  url: https://conda.anaconda.org/conda-forge/noarch/nbconvert-pandoc-7.7.1-pyhd8ed1ab_1.conda
+  version: 7.7.1
 - category: main
   dependencies:
     accessible-pygments: ''
     babel: ''
     beautifulsoup4: ''
     docutils: '!=0.17.0'
     packaging: ''
@@ -6349,26 +6394,26 @@
   name: myst-nb
   optional: false
   platform: linux-64
   url: https://conda.anaconda.org/conda-forge/noarch/myst-nb-0.17.2-pyhd8ed1ab_0.conda
   version: 0.17.2
 - category: main
   dependencies:
-    nbconvert-core: 7.6.0 pyhd8ed1ab_0
-    nbconvert-pandoc: 7.6.0 pyhd8ed1ab_0
-    python: '>=3.7'
+    nbconvert-core: 7.7.1 pyhd8ed1ab_1
+    nbconvert-pandoc: 7.7.1 pyhd8ed1ab_1
+    python: '>=3.8'
   hash:
-    md5: 59976ee8df1c6f82c4aa94b5fd6b745e
-    sha256: c4fa59b7a23456c7488863b9521bfca2a62ed5061150402b7f66c6c8b3b332ea
+    md5: 95d9d1523df069792cd059f412be0d6e
+    sha256: c49a87861db316b322f919825820bc7193cbfa8a4a8b21b5ffe16a133644d400
   manager: conda
   name: nbconvert
   optional: false
   platform: linux-64
-  url: https://conda.anaconda.org/conda-forge/noarch/nbconvert-7.6.0-pyhd8ed1ab_0.conda
-  version: 7.6.0
+  url: https://conda.anaconda.org/conda-forge/noarch/nbconvert-7.7.1-pyhd8ed1ab_1.conda
+  version: 7.7.1
 - category: main
   dependencies:
     jupyter_server: '>=1.8,<3'
     python: '>=3.7'
   hash:
     md5: 67e0fe74c156267d9159e9133df7fd37
     sha256: f028d7ad1f2175cde307db08b60d07e371b9d6f035cfae6c81ea94b4c408c538
@@ -7151,24 +7196,24 @@
   name: double-conversion
   optional: false
   platform: osx-64
   url: https://conda.anaconda.org/conda-forge/osx-64/double-conversion-3.2.0-hf0c8a7f_1.tar.bz2
   version: 3.2.0
 - category: main
   dependencies:
-    libcxx: '>=11.1.0'
+    libcxx: '>=15.0.7'
   hash:
-    md5: f47a426ed1340c966f539c42187e3331
-    sha256: 16a1b30fb2ee932211274cfeab1fe92700822c87eeb2e5f256ab82b82c8e0092
+    md5: 4b30cbb5ec44b4ce28e92daac53f3132
+    sha256: 1a78245598a5665a7fd3451a171e11ac3ee9ef954a833454bf9522eadf0fb528
   manager: conda
   name: eigen
   optional: false
   platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/osx-64/eigen-3.4.0-h940c156_0.tar.bz2
-  version: 3.4.0
+  url: https://conda.anaconda.org/conda-forge/osx-64/eigen-3.4.1-h1c7c39f_0.conda
+  version: 3.4.1
 - category: main
   dependencies:
     libexpat: 2.5.0 hf0c8a7f_1
   hash:
     md5: e12630038077877cbb6c7851e139c17c
     sha256: 15c04a5a690b337b50fb7550cce057d843cf94dd0109d576ec9bc3448a8571d0
   manager: conda
@@ -7617,24 +7662,23 @@
   name: zlib
   optional: false
   platform: osx-64
   url: https://conda.anaconda.org/conda-forge/osx-64/zlib-1.2.13-h8a1eda9_5.conda
   version: 1.2.13
 - category: main
   dependencies:
-    libcxx: '>=14.0.6'
     libzlib: '>=1.2.13,<1.3.0a0'
   hash:
-    md5: 40a188783d3c425bdccc9ae9104acbb8
-    sha256: f845dafb0b488703ce81e25b6f27ed909ee9061b730c172e6b084fcf7156231f
+    md5: b274ec4dbf15a6e20900e397610567a0
+    sha256: 8d6768da7c3170693c0649188e7575474046f8610d8074903cf84e403e3411e8
   manager: conda
   name: zstd
   optional: false
   platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/osx-64/zstd-1.5.2-hbc0c0cd_6.conda
+  url: https://conda.anaconda.org/conda-forge/osx-64/zstd-1.5.2-h829000d_7.conda
   version: 1.5.2
 - category: main
   dependencies:
     libbrotlidec: 1.0.9 hb7f2c08_9
     libbrotlienc: 1.0.9 hb7f2c08_9
   hash:
     md5: 72c526f7ffa265473e6c75fd90605e52
@@ -7742,22 +7786,22 @@
     gettext: '>=0.21.1,<1.0a0'
     libcxx: '>=15.0.7'
     libffi: '>=3.4,<4.0a0'
     libiconv: '>=1.17,<2.0a0'
     libzlib: '>=1.2.13,<1.3.0a0'
     pcre2: '>=10.40,<10.41.0a0'
   hash:
-    md5: 3687b3c1d257dec787418281cfc58358
-    sha256: b9396d779ed9c12e4777500497f87414629e943f2f433d059f3378f8d5d4f57e
+    md5: 05c728fccc40277119bf94cf08e38384
+    sha256: 8d53545974278511739df2711b59087eb7c991fb0e278864a8f5a21db04fd961
   manager: conda
   name: libglib
   optional: false
   platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/osx-64/libglib-2.76.3-hc62aa5d_0.conda
-  version: 2.76.3
+  url: https://conda.anaconda.org/conda-forge/osx-64/libglib-2.76.4-hc62aa5d_0.conda
+  version: 2.76.4
 - category: main
   dependencies:
     gettext: '>=0.21.1,<1.0a0'
     libunistring: '>=0,<1.0a0'
   hash:
     md5: bd109fd705b4ce40a62759129bc4ef5a
     sha256: a85127270c37fe2046372d706c44b7c707605dc1f8b97f80e8a1e1978bd3f8f5
@@ -7899,21 +7943,21 @@
   url: https://conda.anaconda.org/conda-forge/osx-64/mpfr-4.2.0-h4f9bd69_0.conda
   version: 4.2.0
 - category: main
   dependencies:
     libcxx: '>=15.0.7'
     openssl: '>=3.1.1,<4.0a0'
   hash:
-    md5: bfbfd93ef846f67d53f40bcf28b91621
-    sha256: 72cc42ab185b275c888d15d06b28e4d81e48c32af782188aea37020c4329452c
+    md5: 6f1f77589d0af4e85e32f896d2a51f4e
+    sha256: 5f9dbac890eedc04c6e3e37d6d5f150a6a99ec3e04e7d3ebf6c1574698c9f865
   manager: conda
   name: mysql-common
   optional: false
   platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/osx-64/mysql-common-8.0.33-hc6116ba_1.conda
+  url: https://conda.anaconda.org/conda-forge/osx-64/mysql-common-8.0.33-hc6116ba_2.conda
   version: 8.0.33
 - category: main
   dependencies:
     libcxx: '>=14.0.6'
     libsqlite: '>=3.40.0,<4.0a0'
     libzlib: '>=1.2.13,<1.3.0a0'
     nspr: '>=4.35,<5.0a0'
@@ -8110,35 +8154,35 @@
   platform: osx-64
   url: https://conda.anaconda.org/conda-forge/noarch/certifi-2023.5.7-pyhd8ed1ab_0.conda
   version: 2023.5.7
 - category: main
   dependencies:
     python: '>=3.7'
   hash:
-    md5: 7fcff9f6f123696e940bda77bd4d6551
-    sha256: 06cd371fc98f076797d6450f6f337cb679b1060c99680fb7e044591493333194
+    md5: 313516e9a4b08b12dfb1e1cd390a96e3
+    sha256: 0666a95fbbd2299008162e2126c009191e5953d1cad1878bf9f4d8d634af1dd4
   manager: conda
   name: charset-normalizer
   optional: false
   platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-3.1.0-pyhd8ed1ab_0.conda
-  version: 3.1.0
+  url: https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-3.2.0-pyhd8ed1ab_0.conda
+  version: 3.2.0
 - category: main
   dependencies:
     __unix: ''
     python: '>=3.8'
   hash:
-    md5: 20e4087407c7cb04a40817114b333dbf
-    sha256: 23676470b591b100393bb0f6c46fe10624dcbefc696a6a9f42932ed8816ef0ea
+    md5: 64dbb3b205546691a61204d1cfb208e3
+    sha256: 73392cf4851bf7c89e99518effea01d531360a4894c4218e768d5e03e89d7943
   manager: conda
   name: click
   optional: false
   platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/noarch/click-8.1.3-unix_pyhd8ed1ab_2.tar.bz2
-  version: 8.1.3
+  url: https://conda.anaconda.org/conda-forge/noarch/click-8.1.6-unix_pyh707e725_0.conda
+  version: 8.1.6
 - category: main
   dependencies:
     python: '>=3.7'
   hash:
     md5: 3faab06a954c2a04039983f2c4a50d99
     sha256: 2c1b2e9755ce3102bca8d69e8f26e4f087ece73f50418186aee7c74bef8e1698
   manager: conda
@@ -8312,22 +8356,22 @@
   url: https://conda.anaconda.org/conda-forge/osx-64/fontconfig-2.14.2-h5bb23bf_0.conda
   version: 2.14.2
 - category: main
   dependencies:
     python: '>=3.10,<3.11.0a0'
     python_abi: 3.10.* *_cp310
   hash:
-    md5: a3236ddc60f49384eba9348391293038
-    sha256: 741b1c53ac1dcb24a5685e61a1c88638ab52ecfaf097acc8c250594045529cb7
+    md5: f436715de06c55f25e12867550a3589a
+    sha256: 140545a45d32bc87baabefeecb3a5d9d7596ff67450b0483ee07189c160ad8d0
   manager: conda
   name: frozenlist
   optional: false
   platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/osx-64/frozenlist-1.3.3-py310h90acd4f_0.tar.bz2
-  version: 1.3.3
+  url: https://conda.anaconda.org/conda-forge/osx-64/frozenlist-1.4.0-py310h6729b98_0.conda
+  version: 1.4.0
 - category: main
   dependencies:
     python: '>=3.8'
   hash:
     md5: 50ea2067ec92dfcc38b4f07992d7e235
     sha256: 0015e12d85b454ca8e09085e9e788a6156f4f1da1b270019cab2658381d60258
   manager: conda
@@ -8352,25 +8396,25 @@
   optional: false
   platform: osx-64
   url: https://conda.anaconda.org/conda-forge/osx-64/gdk-pixbuf-2.42.8-h3648f77_1.tar.bz2
   version: 2.42.8
 - category: main
   dependencies:
     libcxx: '>=15.0.7'
-    libglib: 2.76.3 hc62aa5d_0
+    libglib: 2.76.4 hc62aa5d_0
     libzlib: '>=1.2.13,<1.3.0a0'
   hash:
-    md5: 43d414c01245d3655df3115c078b90d8
-    sha256: a95d455634ccfb35631932171489a41a9868718fb7a9c558829f6cb3aa0d5584
+    md5: 6a8b2c5e964467242058c27bace19c7f
+    sha256: 72473b42349eeb3b1693c80a611eee71f532add9de3ab617b6891c07b09bd79a
   manager: conda
   name: glib-tools
   optional: false
   platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/osx-64/glib-tools-2.76.3-h7d26f99_0.conda
-  version: 2.76.3
+  url: https://conda.anaconda.org/conda-forge/osx-64/glib-tools-2.76.4-h7d26f99_0.conda
+  version: 2.76.4
 - category: main
   dependencies:
     gettext: '>=0.19.8.1,<1.0a0'
     libcxx: '>=14.0.4'
     libidn2: '>=2,<3.0a0'
     libtasn1: '>=4.19.0,<5.0a0'
     nettle: '>=3.8.1,<3.9.0a0'
@@ -8559,22 +8603,22 @@
     libabseil: '>=20230125.3,<20230126.0a0'
     libcxx: '>=15.0.7'
     libprotobuf: '>=4.23.3,<4.23.4.0a0'
     libzlib: '>=1.2.13,<1.3.0a0'
     openssl: '>=3.1.1,<4.0a0'
     re2: '>=2023.3.2,<2023.3.3.0a0'
   hash:
-    md5: 46a189776f694d37c24c5c1fc301bf50
-    sha256: 6eb1860ab843c2711e67e1d084efe3cbc74ef8785fa8d908e9ef57879b9ebeee
+    md5: c0bb2505f166b769ae3e1e01dce31fe9
+    sha256: 253641caf1fa1c8c8389ea0afe4db86db484fd5482fb42c475696384f6854df8
   manager: conda
   name: libgrpc
   optional: false
   platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/osx-64/libgrpc-1.56.0-he6801ca_2.conda
-  version: 1.56.0
+  url: https://conda.anaconda.org/conda-forge/osx-64/libgrpc-1.56.2-he6801ca_0.conda
+  version: 1.56.2
 - category: main
   dependencies:
     krb5: '>=1.20.1,<1.21.0a0'
     libzlib: '>=1.2.13,<1.3.0a0'
     openssl: '>=3.1.0,<4.0a0'
   hash:
     md5: 571aa9141d1a823202bb4cd794c939b0
@@ -8738,25 +8782,25 @@
   platform: osx-64
   url: https://conda.anaconda.org/conda-forge/noarch/mypy_extensions-1.0.0-pyha770c72_0.conda
   version: 1.0.0
 - category: main
   dependencies:
     libcxx: '>=15.0.7'
     libzlib: '>=1.2.13,<1.3.0a0'
-    mysql-common: 8.0.33 hc6116ba_1
+    mysql-common: 8.0.33 hc6116ba_2
     openssl: '>=3.1.1,<4.0a0'
     zstd: '>=1.5.2,<1.6.0a0'
   hash:
-    md5: b1ba5ec2e4a774e8e4887f0f7592b574
-    sha256: 4af3a969518d0558b13d458901018220c69207e82d2a2a945c563778541fb356
+    md5: 0e750706160c8e178864b890d3afd164
+    sha256: 0a6fbdfccf3437292b4c4fc721fec33d5f73d7ffb23cdd14d5d8332c923d677f
   manager: conda
   name: mysql-libs
   optional: false
   platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/osx-64/mysql-libs-8.0.33-haa61052_1.conda
+  url: https://conda.anaconda.org/conda-forge/osx-64/mysql-libs-8.0.33-haa61052_2.conda
   version: 8.0.33
 - category: main
   dependencies:
     python: '>=3.5'
   hash:
     md5: 7b868f21adde0d9b8b38f9c16836589b
     sha256: 594d240d8be933b6e47b78b786269cc89ffa34874544d9dbed1c6afc9213869b
@@ -8889,22 +8933,22 @@
   platform: osx-64
   url: https://conda.anaconda.org/conda-forge/noarch/ply-3.11-py_1.tar.bz2
   version: '3.11'
 - category: main
   dependencies:
     python: '>=3.6'
   hash:
-    md5: 95c5be3c7cbd872509d16c216617fdab
-    sha256: eb11fd8b927d9c5ff9482cfbd6cd810a43a1351c44a288e9680542ea698a19a0
+    md5: 02153b6b760bbec00cfe9e4c97993d06
+    sha256: a149184fde856dba7968fc50ca89dbb07ebe84abd710d4076e2fada1b9399231
   manager: conda
   name: prometheus_client
   optional: false
   platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/noarch/prometheus_client-0.17.0-pyhd8ed1ab_0.conda
-  version: 0.17.0
+  url: https://conda.anaconda.org/conda-forge/noarch/prometheus_client-0.17.1-pyhd8ed1ab_0.conda
+  version: 0.17.1
 - category: main
   dependencies:
     python: '>=3.10,<3.11.0a0'
     python_abi: 3.10.* *_cp310
   hash:
     md5: 1111504c53989e065a98171156fc376a
     sha256: bfa0da6d3a561d1357ac7f8dfccc781d8aac6804f5697065893e423a7fffc8d0
@@ -8998,34 +9042,34 @@
   platform: osx-64
   url: https://conda.anaconda.org/conda-forge/noarch/pygments-2.15.1-pyhd8ed1ab_0.conda
   version: 2.15.1
 - category: main
   dependencies:
     python: '>=3.6'
   hash:
-    md5: 99e28be5a278e2319834d7dc99e7bfdd
-    sha256: f3a64306fa0f405f10f4108d7ff42043d6fd393f940f9e98e395a3756687fc98
+    md5: 912c0194f898fdb783021fd25f913c31
+    sha256: 88ac94c42ade15113397e30d1831dd341399b5262fb5330b9240f915c33cd232
   manager: conda
   name: pyjwt
   optional: false
   platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/noarch/pyjwt-2.7.0-pyhd8ed1ab_0.conda
-  version: 2.7.0
+  url: https://conda.anaconda.org/conda-forge/noarch/pyjwt-2.8.0-pyhd8ed1ab_0.conda
+  version: 2.8.0
 - category: main
   dependencies:
     python: '>=3.6'
   hash:
-    md5: d3ed087d1f7f8f5590e8e87b57a8ce64
-    sha256: 18e3bd52c64f23bbc7c200fd2fc4152dd29423936dc43e8f129cb43f1af0136c
+    md5: e8fbc1b54b25f4b08281467bc13b70cc
+    sha256: 4acc7151cef5920d130f2e0a7615559cce8bfb037aeecb14d4d359ae3d9bc51b
   manager: conda
   name: pyparsing
   optional: false
   platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/noarch/pyparsing-3.1.0-pyhd8ed1ab_0.conda
-  version: 3.1.0
+  url: https://conda.anaconda.org/conda-forge/noarch/pyparsing-3.0.9-pyhd8ed1ab_0.tar.bz2
+  version: 3.0.9
 - category: main
   dependencies:
     python: '>=3.10,<3.11.0a0'
     python_abi: 3.10.* *_cp310
   hash:
     md5: 2de2b931546de39d852e5d21e58876c1
     sha256: 15c8cc139ffd7a9337aa40122c0f27abb15e5b7dc4d448dedb831e9aa797358f
@@ -9124,14 +9168,27 @@
   name: rfc3986-validator
   optional: false
   platform: osx-64
   url: https://conda.anaconda.org/conda-forge/noarch/rfc3986-validator-0.1.1-pyh9f0ad1d_0.tar.bz2
   version: 0.1.1
 - category: main
   dependencies:
+    python: '>=3.10,<3.11.0a0'
+    python_abi: 3.10.* *_cp310
+  hash:
+    md5: d27546735a054dd67e626b17ff07c089
+    sha256: fcd8c7a5272e2c678b0d3f7225758fe12e9b33b25371f5a02e6ee63387436297
+  manager: conda
+  name: ruamel.yaml.clib
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/osx-64/ruamel.yaml.clib-0.2.7-py310h90acd4f_1.conda
+  version: 0.2.7
+- category: main
+  dependencies:
     python: '>=3.7'
   hash:
     md5: 3b68bc43ec6baa48f7354a446267eefe
     sha256: 3ac44771fce01f19218bcdf3992e24984748048db69889a9df65abcc6a10e29b
   manager: conda
   name: setuptools
   optional: false
@@ -9346,22 +9403,22 @@
   platform: osx-64
   url: https://conda.anaconda.org/conda-forge/osx-64/typed-ast-1.5.4-py310h90acd4f_1.tar.bz2
   version: 1.5.4
 - category: main
   dependencies:
     python: '>=3.7'
   hash:
-    md5: 4a3014a4d107d15475d106b751c4e352
-    sha256: 90a8d56c8015af1575d504d5f77d95a806cd999fc178a06ab51a349f1f744672
+    md5: c39d6a09fe819de4951c2642629d9115
+    sha256: 6edd6d5be690be492712cb747b6d62707f0d0c34ef56eefc796d91e5a03187d1
   manager: conda
   name: typing_extensions
   optional: false
   platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.6.3-pyha770c72_0.conda
-  version: 4.6.3
+  url: https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.7.1-pyha770c72_0.conda
+  version: 4.7.1
 - category: main
   dependencies:
     python: '>=3.6.1'
   hash:
     md5: eb67e3cace64c66233e2d35949e20f92
     sha256: 9e3758b620397f56fb709f796969de436d63b7117897159619b87938e1f78739
   manager: conda
@@ -9431,21 +9488,21 @@
   platform: osx-64
   url: https://conda.anaconda.org/conda-forge/noarch/websocket-client-1.6.1-pyhd8ed1ab_0.conda
   version: 1.6.1
 - category: main
   dependencies:
     python: '>=3.7'
   hash:
-    md5: 49bb0d9e60ce1db25e151780331bb5f3
-    sha256: 79b4d29b0c004014a2abd5fc2c9fcd35cc6256222b960c2a317a27c4b0d8884d
+    md5: c95fac682453aeffa12db7ae5a721bec
+    sha256: e91cbb3c0ad9a9507dd030f5493831cb52da120329e0d0793711e8300a36db22
   manager: conda
   name: wheel
   optional: false
   platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/noarch/wheel-0.40.0-pyhd8ed1ab_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/wheel-0.40.0-pyhd8ed1ab_1.conda
   version: 0.40.0
 - category: main
   dependencies:
     python: '>=3.7'
   hash:
     md5: 2e9ebddf0b93d0fb203d0906b8052c4f
     sha256: a73d34f8169e206bccfb356c093ff5ced803b953bbcc1480ed27976f97598d68
@@ -9466,24 +9523,24 @@
   name: wrapt
   optional: false
   platform: osx-64
   url: https://conda.anaconda.org/conda-forge/osx-64/wrapt-1.15.0-py310h90acd4f_0.conda
   version: 1.15.0
 - category: main
   dependencies:
-    python: '>=3.7'
+    python: '>=3.8'
   hash:
-    md5: 13018819ca8f5b7cc675a8faf1f5fedf
-    sha256: 241de30545299be9bcea3addf8a2c22a3b3d4ba6730890e150ab690ac937a3d2
+    md5: 2da0451b54c4563c32490cb1b7cf68a1
+    sha256: 16d72127e150a3d5cbdc0b82c4069ef5be135c64bc99e71e7928507910669b41
   manager: conda
   name: zipp
   optional: false
   platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/noarch/zipp-3.15.0-pyhd8ed1ab_0.conda
-  version: 3.15.0
+  url: https://conda.anaconda.org/conda-forge/noarch/zipp-3.16.2-pyhd8ed1ab_0.conda
+  version: 3.16.2
 - category: main
   dependencies:
     pygments: ''
     python: '>=3.6'
   hash:
     md5: 46a2e6e3dfa718ce3492018d5a110dd6
     sha256: ce532e2da08fb2b77df281e3d42e2b2131641bdd6a6e8127f3718ae6860bd70d
@@ -9510,22 +9567,22 @@
   dependencies:
     exceptiongroup: ''
     idna: '>=2.8'
     python: '>=3.7'
     sniffio: '>=1.1'
     typing_extensions: ''
   hash:
-    md5: 2b35a85d654a47aac8f34c1bb6de7142
-    sha256: 863c11a6a0e937977229b405a16f6d43fff543dfe5b1a66da9c42ec0cbdaaf33
+    md5: 7b517e7a6f0790337906c055aa97ca49
+    sha256: 62637ac498bcf47783cbf4f48e9b09e4e2f5a6ad42f43ca8f632c353827b94f4
   manager: conda
   name: anyio
   optional: false
   platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/noarch/anyio-3.7.0-pyhd8ed1ab_1.conda
-  version: 3.7.0
+  url: https://conda.anaconda.org/conda-forge/noarch/anyio-3.7.1-pyhd8ed1ab_0.conda
+  version: 3.7.1
 - category: main
   dependencies:
     python: '>=3.5'
     six: ''
   hash:
     md5: bf7f54dd0f25c3f06ecb82a07341841a
     sha256: 7ed530efddd47a96c11197906b4008405b90e3bc2f4e0df722a36e0e6103fd9c
@@ -9730,39 +9787,39 @@
   dependencies:
     brotli: ''
     munkres: ''
     python: '>=3.10,<3.11.0a0'
     python_abi: 3.10.* *_cp310
     unicodedata2: '>=14.0.0'
   hash:
-    md5: 15dcc729f2102b4b64e0e6f53f2fb377
-    sha256: 92888a43be0f94b7110a73c1b2852119cd709c7b61196376dd82da8e48d9262f
+    md5: 2de0c6bd77a2ea8aa4e82943273c5dd3
+    sha256: 76ae3255902589a8076f76b4821c3e47e6622af9b2a8aba5ce432da5bc848632
   manager: conda
   name: fonttools
   optional: false
   platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/osx-64/fonttools-4.40.0-py310h6729b98_0.conda
-  version: 4.40.0
+  url: https://conda.anaconda.org/conda-forge/osx-64/fonttools-4.41.0-py310h6729b98_0.conda
+  version: 4.41.0
 - category: main
   dependencies:
     gettext: '>=0.21.1,<1.0a0'
-    glib-tools: 2.76.3 h7d26f99_0
+    glib-tools: 2.76.4 h7d26f99_0
     libcxx: '>=15.0.7'
-    libglib: 2.76.3 hc62aa5d_0
+    libglib: 2.76.4 hc62aa5d_0
     libzlib: '>=1.2.13,<1.3.0a0'
     python: '*'
   hash:
-    md5: a062952a59c0a26adb18899ac6472a7e
-    sha256: a143518370c1627707e6be19ec738116fd6e4a5838a42b8df0aa516615a016f4
+    md5: 4176982aebeacb4f6914ea5528dc2853
+    sha256: 415a4a82d9c4f0e9688025125c6e48b640e80ef7f2e6fb2077b5c9c062742f38
   manager: conda
   name: glib
   optional: false
   platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/osx-64/glib-2.76.3-h7d26f99_0.conda
-  version: 2.76.3
+  url: https://conda.anaconda.org/conda-forge/osx-64/glib-2.76.4-h7d26f99_0.conda
+  version: 2.76.4
 - category: main
   dependencies:
     gmp: '>=6.2.1,<7.0a0'
     mpc: '>=1.2.1,<2.0a0'
     mpfr: '>=4.1.0,<5.0a0'
     python: '>=3.10,<3.11.0a0'
     python_abi: 3.10.* *_cp310
@@ -9775,27 +9832,27 @@
   platform: osx-64
   url: https://conda.anaconda.org/conda-forge/osx-64/gmpy2-2.1.2-py310hb691cb2_1.tar.bz2
   version: 2.1.2
 - category: main
   dependencies:
     __osx: '>=10.13'
     libcxx: '>=15.0.7'
-    libgrpc: 1.56.0 he6801ca_2
+    libgrpc: 1.56.2 he6801ca_0
     libzlib: '>=1.2.13,<1.3.0a0'
     python: '>=3.10,<3.11.0a0'
     python_abi: 3.10.* *_cp310
   hash:
-    md5: 0ce1b3a5e4abf21c5a33e8d270ec2be2
-    sha256: 87bbaee723f135f6d58825206405e35e59af620cfff762ee8ba94c2194577396
+    md5: 6be89e336739268b0415850c065cc0d8
+    sha256: aa5b7029d95293f48b196cc22c7d7e457e1390387f4aeefb23f9c601d01076e6
   manager: conda
   name: grpcio
   optional: false
   platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/osx-64/grpcio-1.56.0-py310h0d4bf3c_2.conda
-  version: 1.56.0
+  url: https://conda.anaconda.org/conda-forge/osx-64/grpcio-1.56.2-py310h0d4bf3c_0.conda
+  version: 1.56.2
 - category: main
   dependencies:
     libaec: '>=1.0.6,<2.0a0'
     libcurl: '>=7.87.0,<9.0a0'
     libcxx: '>=13.0.1'
     libgfortran: 5.*
     libgfortran5: '>=9.5.0'
@@ -9811,35 +9868,35 @@
   url: https://conda.anaconda.org/conda-forge/osx-64/hdf5-1.12.2-nompi_h48135f9_101.conda
   version: 1.12.2
 - category: main
   dependencies:
     python: '>=3.8'
     zipp: '>=0.5'
   hash:
-    md5: ba3786c6846e46038fe60c785d46dc81
-    sha256: 1ffffc30dc67d8329d47c6d22de726cfd28d7ed236bca54f52fc0bdcd0a53fc7
+    md5: 4e9f59a060c3be52bc4ddc46ee9b6946
+    sha256: 2797ed927d65324309b6c630190d917b9f2111e0c217b721f80429aeb57f9fcf
   manager: conda
   name: importlib-metadata
   optional: false
   platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-6.7.0-pyha770c72_0.conda
-  version: 6.7.0
+  url: https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-6.8.0-pyha770c72_0.conda
+  version: 6.8.0
 - category: main
   dependencies:
-    python: '>=3.7'
+    python: '>=3.8'
     zipp: '>=3.1.0'
   hash:
-    md5: e5fd2260a231ee63b6969f4801082f2b
-    sha256: 091cca3e010f7a7353152f0abda2d68cfd83ddde80a15e974d9e18b2047e7be2
+    md5: a08b6be5bf18b9d2a927d3457750f82e
+    sha256: 94c1b2831c0f908ae56212d9aeb9c9173051d307682b4fedfd88fef774b0b8f7
   manager: conda
   name: importlib_resources
   optional: false
   platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/noarch/importlib_resources-5.12.0-pyhd8ed1ab_0.conda
-  version: 5.12.0
+  url: https://conda.anaconda.org/conda-forge/noarch/importlib_resources-6.0.0-pyhd8ed1ab_1.conda
+  version: 6.0.0
 - category: main
   dependencies:
     parso: '>=0.8.0,<0.9.0'
     python: '>=3.6'
   hash:
     md5: b5e695ef9c3f0d27d6cd96bf5adc9e07
     sha256: abe63ae6e1b13f83500608d94004cb8d485b264083511d77f79253e775cd546c
@@ -10207,14 +10264,29 @@
   name: rsa
   optional: false
   platform: osx-64
   url: https://conda.anaconda.org/conda-forge/noarch/rsa-4.9-pyhd8ed1ab_0.tar.bz2
   version: '4.9'
 - category: main
   dependencies:
+    python: '>=3.10,<3.11.0a0'
+    python_abi: 3.10.* *_cp310
+    ruamel.yaml.clib: '>=0.1.2'
+    setuptools: ''
+  hash:
+    md5: 4c87395e8169331108914e30ab46d2a4
+    sha256: 717052d56e07a042c283d2e8811aa7c6208241e51db91563c1ee52e85d376e7d
+  manager: conda
+  name: ruamel.yaml
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/osx-64/ruamel.yaml-0.17.32-py310h6729b98_0.conda
+  version: 0.17.32
+- category: main
+  dependencies:
     libcxx: '>=15.0.7'
     packaging: ''
     ply: ''
     python: '>=3.10,<3.11.0a0'
     python_abi: 3.10.* *_cp310
     tomli: ''
   hash:
@@ -10265,24 +10337,24 @@
   name: tqdm
   optional: false
   platform: osx-64
   url: https://conda.anaconda.org/conda-forge/noarch/tqdm-4.65.0-pyhd8ed1ab_1.conda
   version: 4.65.0
 - category: main
   dependencies:
-    typing_extensions: 4.6.3 pyha770c72_0
+    typing_extensions: 4.7.1 pyha770c72_0
   hash:
-    md5: 3876f650ed7d0f95d70fa4b647621909
-    sha256: d2334dab270e13182403cc3a394e3da8e7acb409e94059a6d9223d2ac053f90a
+    md5: f96688577f1faa58096d06a45136afa2
+    sha256: d5d19b8f5b275240c19616a46d67ec57250b3720ba88200da8c732c3fcbfc21d
   manager: conda
   name: typing-extensions
   optional: false
   platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.6.3-hd8ed1ab_0.conda
-  version: 4.6.3
+  url: https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.7.1-hd8ed1ab_0.conda
+  version: 4.7.1
 - category: main
   dependencies:
     markupsafe: '>=2.1.1'
     python: '>=3.8'
   hash:
     md5: 55fbbb3e67185820ee2007395bfe0073
     sha256: 28515f7ddb8a20f1436b9ac3a6ba2aa9be337995e4ee63c72d0f5d0efd6a2062
@@ -10325,22 +10397,22 @@
   dependencies:
     lazy-object-proxy: '>=1.4.0'
     python: '>=3.10,<3.11.0a0'
     python_abi: 3.10.* *_cp310
     typing-extensions: '>=4.0.0'
     wrapt: <2,>=1.11
   hash:
-    md5: 6f8c825da6f4eedc532a6d102220d0e0
-    sha256: 6c7bce2847f232fe7cc97e0ad5a7c45441f3a2d45740716510ee01a3bae32c7c
+    md5: 2812b75db400abe651a33b99a7173ee6
+    sha256: d7c9060e4f7ead4ed9d33722ed1736006ff60d61fac5c24884d5757c63f2d1fb
   manager: conda
   name: astroid
   optional: false
   platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/osx-64/astroid-2.15.5-py310h2ec42d9_0.conda
-  version: 2.15.5
+  url: https://conda.anaconda.org/conda-forge/osx-64/astroid-2.15.6-py310h2ec42d9_0.conda
+  version: 2.15.6
 - category: main
   dependencies:
     python: '>=3.6'
     typing-extensions: '>=3.6.5'
   hash:
     md5: 25e79f9a1133556671becbd65a170c78
     sha256: a08b78e6fadee1ffac0f255363d2a08a0c589c7403fd2a71c1c0b6aafd5e0737
@@ -10367,22 +10439,22 @@
 - category: main
   dependencies:
     cffi: '>=1.12'
     openssl: '>=3.1.1,<4.0a0'
     python: '>=3.10,<3.11.0a0'
     python_abi: 3.10.* *_cp310
   hash:
-    md5: f66541237ec50c9d89228ded177b8d65
-    sha256: 0d73ef9738465c357e40ad9f17d0bd5b266ed0c21191d177736074237c9d53ac
+    md5: f7f258c457df7e0617c2b92e24a7b47f
+    sha256: 458cf46565a728bbab0af7388a22d1561cc8bb5364675e1983f710fa0968dcb0
   manager: conda
   name: cryptography
   optional: false
   platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/osx-64/cryptography-41.0.1-py310ha1817de_0.conda
-  version: 41.0.1
+  url: https://conda.anaconda.org/conda-forge/osx-64/cryptography-41.0.2-py310ha1817de_0.conda
+  version: 41.0.2
 - category: main
   dependencies:
     python: '>=3.6'
     python-dateutil: '>=2.8.1'
   hash:
     md5: 6d8d61116031a3f5b1f32e7899785866
     sha256: 097d9b4c946b195800bc68f68393370049238509b08ef828c06fbf481bbc139c
@@ -10396,21 +10468,21 @@
   dependencies:
     gettext: '>=0.21.1,<1.0a0'
     glib: '>=2.76.3,<3.0a0'
     libcxx: '>=15.0.7'
     libglib: '>=2.76.3,<3.0a0'
     libiconv: '>=1.17,<2.0a0'
   hash:
-    md5: a24d0265742fe6614ca8d1186c0d8a42
-    sha256: 20014fd8c3a42094b8127f1a06c57c9c47115343fa721baae245b984def4ff60
+    md5: 659321735840756bc2c6ba7195ed9d8b
+    sha256: 362e945e55e729d11351b760622d25049272178ef1dc6f74c5d7e518ca3f2ed3
   manager: conda
   name: gstreamer
   optional: false
   platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/osx-64/gstreamer-1.22.4-h840fbdc_0.conda
+  url: https://conda.anaconda.org/conda-forge/osx-64/gstreamer-1.22.4-h840fbdc_1.conda
   version: 1.22.4
 - category: main
   dependencies:
     cairo: '>=1.16.0,<2.0a0'
     freetype: '>=2.12.1,<3.0a0'
     graphite2: ''
     icu: '>=70.1,<71.0a0'
@@ -10423,24 +10495,24 @@
   name: harfbuzz
   optional: false
   platform: osx-64
   url: https://conda.anaconda.org/conda-forge/osx-64/harfbuzz-6.0.0-h08f8713_0.conda
   version: 6.0.0
 - category: main
   dependencies:
-    importlib-metadata: '>=6.7.0,<6.7.1.0a0'
+    importlib-metadata: '>=6.8.0,<6.8.1.0a0'
   hash:
-    md5: 27a4cec373ec84d1c1aa02a1e37f8eaf
-    sha256: f46d34a06e63f220dd04f7ac211dd2b4812b6b8a9e851467cd2e0218174d2dfd
+    md5: b279b07ce18058034e5b3606ba103a8b
+    sha256: b96e01dc42d547d6d9ceb1c5b52a5232cc04e40153534350f702c3e0418a6b3f
   manager: conda
   name: importlib_metadata
   optional: false
   platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-6.7.0-hd8ed1ab_0.conda
-  version: 6.7.0
+  url: https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-6.8.0-hd8ed1ab_0.conda
+  version: 6.8.0
 - category: main
   dependencies:
     attrs: '>=17.4.0'
     importlib-metadata: ''
     importlib_resources: '>=1.4.0'
     pkgutil-resolve-name: '>=1.3.10'
     pyrsistent: '!=0.17.0,!=0.17.1,!=0.17.2,>=0.14.0'
@@ -10555,35 +10627,35 @@
     libblas: '>=3.9.0,<4.0a0'
     libcblas: '>=3.9.0,<4.0a0'
     libcxx: '>=15.0.7'
     liblapack: '>=3.9.0,<4.0a0'
     python: '>=3.10,<3.11.0a0'
     python_abi: 3.10.* *_cp310
   hash:
-    md5: 9accbca17b11eed20ee32b57189e9e66
-    sha256: b897d4d4ab581a22faba563c38981114bf16eb0eecc906b20421c96299def30f
+    md5: 525db32fd93b63f2f7ca3ece8576b9c8
+    sha256: 32fe99f86e998169999514fb7f96695fdec9215bd0e7061425c1b4e399ca2cae
   manager: conda
   name: numpy
   optional: false
   platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/osx-64/numpy-1.25.0-py310h7451ae0_0.conda
-  version: 1.25.0
+  url: https://conda.anaconda.org/conda-forge/osx-64/numpy-1.25.1-py310h7451ae0_0.conda
+  version: 1.25.1
 - category: main
   dependencies:
     python: '>=3.7'
     typing-extensions: '>=4.6.3'
   hash:
-    md5: 3e4aca765371893ad848397794600632
-    sha256: 5f382d0d3509784152506e0e022bb5a30d254555e809804491207196f890af67
+    md5: 044e7a1e0ad42c4e67110bd078150a63
+    sha256: 885611bd528abaf3e31bc0bfaad3a619cfe89db61d886b53c2a9ec9ff50edebe
   manager: conda
   name: platformdirs
   optional: false
   platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.8.0-pyhd8ed1ab_0.conda
-  version: 3.8.0
+  url: https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.9.1-pyhd8ed1ab_0.conda
+  version: 3.9.1
 - category: main
   dependencies:
     latexcodec: '>=1.0.4'
     python: '>=3.6'
     pyyaml: '>=3.01'
     setuptools: ''
     six: ''
@@ -10664,22 +10736,22 @@
 - category: main
   dependencies:
     greenlet: '!=0.4.17'
     python: '>=3.10,<3.11.0a0'
     python_abi: 3.10.* *_cp310
     typing-extensions: '>=4.2.0'
   hash:
-    md5: 2f7579944d2f1b682ad79c1de277368f
-    sha256: 89026e4549fa599e7db91a68a53cfa16983327e52ea661f1aadb5adccf59f71b
+    md5: 9560749662f11f766ce19db9fa6271a4
+    sha256: 9a4459fa103a68ff7bfe733f1f5af81fe31956fdbab87c062c1e0904c115c7fb
   manager: conda
   name: sqlalchemy
   optional: false
   platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/osx-64/sqlalchemy-2.0.17-py310h6729b98_0.conda
-  version: 2.0.17
+  url: https://conda.anaconda.org/conda-forge/osx-64/sqlalchemy-2.0.19-py310h6729b98_0.conda
+  version: 2.0.19
 - category: main
   dependencies:
     asttokens: ''
     executing: ''
     pure_eval: ''
     python: '>=3.5'
   hash:
@@ -10727,22 +10799,22 @@
     charset-normalizer: '>=2.0,<4.0'
     frozenlist: '>=1.1.1'
     multidict: '>=4.5,<7.0'
     python: '>=3.10,<3.11.0a0'
     python_abi: 3.10.* *_cp310
     yarl: '>=1.0,<2.0'
   hash:
-    md5: 513a7cdaa184e2856c358a57205d3837
-    sha256: 5def9e74e8217db10622b37b935d5a887ccea07c4245a0c7fc4711211d387055
+    md5: b91a4b8a80ba83d20ed0eabcc6949ebc
+    sha256: 4038817957ce83f536901968b86e665ac1bf5e642a2cc7de9082d12e29bcf53f
   manager: conda
   name: aiohttp
   optional: false
   platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/osx-64/aiohttp-3.8.4-py310h6729b98_1.conda
-  version: 3.8.4
+  url: https://conda.anaconda.org/conda-forge/osx-64/aiohttp-3.8.5-py310h6729b98_0.conda
+  version: 3.8.5
 - category: main
   dependencies:
     argon2-cffi-bindings: ''
     flit-core: '>=3.4,<4'
     python: '>=3.6'
   hash:
     md5: a0b402db58f73aaab8ee0ca1025a362e
@@ -10804,30 +10876,30 @@
   optional: false
   platform: osx-64
   url: https://conda.anaconda.org/conda-forge/osx-64/contourpy-1.1.0-py310h88cfcbd_0.conda
   version: 1.1.0
 - category: main
   dependencies:
     gettext: '>=0.21.1,<1.0a0'
-    gstreamer: 1.22.4 h840fbdc_0
+    gstreamer: 1.22.4 h840fbdc_1
     libcxx: '>=15.0.7'
     libglib: '>=2.76.3,<3.0a0'
     libogg: '>=1.3.4,<1.4.0a0'
     libopus: '>=1.3.1,<2.0a0'
     libpng: '>=1.6.39,<1.7.0a0'
     libvorbis: '>=1.3.7,<1.4.0a0'
     libzlib: '>=1.2.13,<1.3.0a0'
   hash:
-    md5: 3ddc9bb14daecff3a86233f07e0d472a
-    sha256: ef79b53e2a69ffba4fd089d461502049c955ca8d677aa7d5452b3dd87723521a
+    md5: 504bc1e992fc2d59e55cbd0102e117b0
+    sha256: ade088cd9e124e033f56926ab97012a9a0af186251d7d904005476900eb3da9d
   manager: conda
   name: gst-plugins-base
   optional: false
   platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/osx-64/gst-plugins-base-1.22.4-hb5d3a86_0.conda
+  url: https://conda.anaconda.org/conda-forge/osx-64/gst-plugins-base-1.22.4-hb5d3a86_1.conda
   version: 1.22.4
 - category: main
   dependencies:
     platformdirs: '>=2.5'
     python: '>=3.10,<3.11.0a0'
     python_abi: 3.10.* *_cp310
     traitlets: '>=5.3'
@@ -10856,14 +10928,29 @@
   name: jupyter_events
   optional: false
   platform: osx-64
   url: https://conda.anaconda.org/conda-forge/noarch/jupyter_events-0.6.3-pyhd8ed1ab_0.conda
   version: 0.6.3
 - category: main
   dependencies:
+    numpy: '>=1.19'
+    packaging: '>=17'
+    python: '>=3.10,<3.11.0a0'
+    python_abi: 3.10.* *_cp310
+  hash:
+    md5: 04ba9603c2c52981e403da2295df8bc5
+    sha256: 89903ed54d9024ae4205309a76db983505df6f582b8a33c29ae9e8aea30f478e
+  manager: conda
+  name: nibabel
+  optional: false
+  platform: osx-64
+  url: https://conda.anaconda.org/conda-forge/osx-64/nibabel-5.1.0-py310h2ec42d9_2.conda
+  version: 5.1.0
+- category: main
+  dependencies:
     blinker: ''
     cryptography: ''
     pyjwt: '>=1.0.0'
     python: '>=3.6'
   hash:
     md5: 8f882b197fd9c4941a787926baea4868
     sha256: 0cfd5146a91d3974f4abfc2a45de890371d510a77238fe553e036ec8c031dc5b
@@ -11071,47 +11158,47 @@
     __osx: '>=10.12'
     certifi: '>=2020.06.20'
     contourpy: '>=1.0.1'
     cycler: '>=0.10'
     fonttools: '>=4.22.0'
     freetype: '>=2.12.1,<3.0a0'
     kiwisolver: '>=1.0.1'
-    libcxx: '>=14.0.6'
+    libcxx: '>=15.0.7'
     numpy: '>=1.21.6,<2.0a0'
     packaging: '>=20.0'
     pillow: '>=6.2.0'
-    pyparsing: '>=2.3.1'
+    pyparsing: '>=2.3.1,<3.1'
     python: '>=3.10,<3.11.0a0'
     python-dateutil: '>=2.7'
     python_abi: 3.10.* *_cp310
   hash:
-    md5: 8b1caf6e250a7c8270711c301d8bcd2e
-    sha256: d65897175994c763913ee1871ff431234ef8264f05aaff5cfbb19187fd30a8cf
+    md5: ffc8dbf00f18c1ca9d3c02854cb72aee
+    sha256: ef3121ac09b07b94068226e624a86b0a4de536735109bb44af79954638fa0ba8
   manager: conda
   name: matplotlib-base
   optional: false
   platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/osx-64/matplotlib-base-3.7.1-py310he725631_0.conda
-  version: 3.7.1
+  url: https://conda.anaconda.org/conda-forge/osx-64/matplotlib-base-3.7.2-py310h475a17b_0.conda
+  version: 3.7.2
 - category: main
   dependencies:
     jsonschema: '>=2.6'
     jupyter_core: ''
     python: '>=3.8'
     python-fastjsonschema: ''
     traitlets: '>=5.1'
   hash:
-    md5: f525a01528c3eba1d381a232a6971c6a
-    sha256: 3c6be17e84dc71db605a9e088fa7af7d47edab45d15da8e2a2ab3f29ec5ec081
+    md5: 3ec35d84fc1775215061517eb4660693
+    sha256: d8b1ad3c219b39e5e325785606853ff1cd334769228490ac977b85aa95e94ba0
   manager: conda
   name: nbformat
   optional: false
   platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/noarch/nbformat-5.9.0-pyhd8ed1ab_0.conda
-  version: 5.9.0
+  url: https://conda.anaconda.org/conda-forge/noarch/nbformat-5.9.1-pyhd8ed1ab_0.conda
+  version: 5.9.1
 - category: main
   dependencies:
     prompt-toolkit: '>=3.0.39,<3.0.40.0a0'
   hash:
     md5: 4bbbe67d5df19db30f04b8e344dc9976
     sha256: 89f7fecc7355181dbc2ab851e668a2fce6aa4830b336a34c93b59bda93206270
   manager: conda
@@ -11244,27 +11331,27 @@
   name: ipython
   optional: false
   platform: osx-64
   url: https://conda.anaconda.org/conda-forge/noarch/ipython-8.14.0-pyhd1c38e8_0.conda
   version: 8.14.0
 - category: main
   dependencies:
-    matplotlib-base: '>=3.7.1,<3.7.2.0a0'
+    matplotlib-base: '>=3.7.2,<3.7.3.0a0'
     python: '>=3.10,<3.11.0a0'
     python_abi: 3.10.* *_cp310
     tornado: '>=5'
   hash:
-    md5: 958029c1236746d27149fca648c41cab
-    sha256: 8d51885c030f79fbb0984683e9a1b2e845119a85d9184eb2d5a123838cc82909
+    md5: 4fe2e1daa542b330507af9a2ca079d1c
+    sha256: a47920246485fdd4a9e0dadc04359a9264017f9b18c4b77cfe94213fe6a14c65
   manager: conda
   name: matplotlib
   optional: false
   platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/osx-64/matplotlib-3.7.1-py310h2ec42d9_0.conda
-  version: 3.7.1
+  url: https://conda.anaconda.org/conda-forge/osx-64/matplotlib-3.7.2-py310h2ec42d9_0.conda
+  version: 3.7.2
 - category: main
   dependencies:
     jupyter_client: '>=6.1.12'
     jupyter_core: '>=4.12,!=5.0.*'
     nbformat: '>=5.1'
     python: '>=3.7'
     traitlets: '>=5.3'
@@ -11384,22 +11471,22 @@
     python: '>=3.6'
     pyu2f: '>=0.1.5'
     requests: '>=2.20.0,<3.0.0dev'
     rsa: '>=3.1.4,<5'
     six: '>=1.9.0'
     urllib3: <2.0
   hash:
-    md5: 8c5dd8609d314721d990c1d1fd607f81
-    sha256: 6b097ca9b31961d6a983f81dc295012e9c99c4c1a5a83a93ab2fcc6528af428f
+    md5: 5583192796d1ebcf39b1e3e0958aa259
+    sha256: 1a75b167cb01f533c01716bc663d4859a0d55d47dd96eebb39b5aa4b51205b44
   manager: conda
   name: google-auth
   optional: false
   platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/noarch/google-auth-2.21.0-pyh1a96a4e_0.conda
-  version: 2.21.0
+  url: https://conda.anaconda.org/conda-forge/noarch/google-auth-2.22.0-pyh1a96a4e_0.conda
+  version: 2.22.0
 - category: main
   dependencies:
     __osx: ''
     appnope: ''
     comm: '>=0.1.1'
     debugpy: '>=1.6.5'
     ipython: '>=7.23.1'
@@ -11454,26 +11541,26 @@
     markupsafe: '>=2.0'
     mistune: '>=2.0.3,<4'
     nbclient: '>=0.5.0'
     nbformat: '>=5.1'
     packaging: ''
     pandocfilters: '>=1.4.1'
     pygments: '>=2.4.1'
-    python: '>=3.7'
+    python: '>=3.8'
     tinycss2: ''
     traitlets: '>=5.0'
   hash:
-    md5: 879782bde4bbdb4c7b5d4054504a20d5
-    sha256: cebfc8c620bdc950e92f72562d281fc57d696497e30bef5bc9e517be757b1c2f
+    md5: 32dde1678bb003c90d4bc0c2dbd21814
+    sha256: 76ad7689d35fe031459c422f142c9d8e7a02f6922049b7a0183fc70aaef02f0a
   manager: conda
   name: nbconvert-core
   optional: false
   platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/noarch/nbconvert-core-7.6.0-pyhd8ed1ab_0.conda
-  version: 7.6.0
+  url: https://conda.anaconda.org/conda-forge/noarch/nbconvert-core-7.7.1-pyhd8ed1ab_1.conda
+  version: 7.7.1
 - category: main
   dependencies:
     packaging: '>=20.0'
     platformdirs: '>=2.5.0'
     python: '>=3.7'
     requests: '>=2.19.0'
   hash:
@@ -11702,26 +11789,26 @@
   name: myst-parser
   optional: false
   platform: osx-64
   url: https://conda.anaconda.org/conda-forge/noarch/myst-parser-0.18.1-pyhd8ed1ab_0.tar.bz2
   version: 0.18.1
 - category: main
   dependencies:
-    nbconvert-core: 7.6.0 pyhd8ed1ab_0
+    nbconvert-core: 7.7.1 pyhd8ed1ab_1
     pandoc: ''
-    python: '>=3.7'
+    python: '>=3.8'
   hash:
-    md5: e8172ca42f2869bb90185c9356899e81
-    sha256: 07204ee7a7f429aa30c78897629c79859a60ef77fd1c2b9d9a1ad084c144a84f
+    md5: 796b056965d7146bcac082fa2a83943d
+    sha256: b5b2823e7951a5ba41b1020b7cce109fec7f2ebe540234bf8a17c54615c2f679
   manager: conda
   name: nbconvert-pandoc
   optional: false
   platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/noarch/nbconvert-pandoc-7.6.0-pyhd8ed1ab_0.conda
-  version: 7.6.0
+  url: https://conda.anaconda.org/conda-forge/noarch/nbconvert-pandoc-7.7.1-pyhd8ed1ab_1.conda
+  version: 7.7.1
 - category: main
   dependencies:
     accessible-pygments: ''
     babel: ''
     beautifulsoup4: ''
     docutils: '!=0.17.0'
     packaging: ''
@@ -12000,26 +12087,26 @@
   name: myst-nb
   optional: false
   platform: osx-64
   url: https://conda.anaconda.org/conda-forge/noarch/myst-nb-0.17.2-pyhd8ed1ab_0.conda
   version: 0.17.2
 - category: main
   dependencies:
-    nbconvert-core: 7.6.0 pyhd8ed1ab_0
-    nbconvert-pandoc: 7.6.0 pyhd8ed1ab_0
-    python: '>=3.7'
+    nbconvert-core: 7.7.1 pyhd8ed1ab_1
+    nbconvert-pandoc: 7.7.1 pyhd8ed1ab_1
+    python: '>=3.8'
   hash:
-    md5: 59976ee8df1c6f82c4aa94b5fd6b745e
-    sha256: c4fa59b7a23456c7488863b9521bfca2a62ed5061150402b7f66c6c8b3b332ea
+    md5: 95d9d1523df069792cd059f412be0d6e
+    sha256: c49a87861db316b322f919825820bc7193cbfa8a4a8b21b5ffe16a133644d400
   manager: conda
   name: nbconvert
   optional: false
   platform: osx-64
-  url: https://conda.anaconda.org/conda-forge/noarch/nbconvert-7.6.0-pyhd8ed1ab_0.conda
-  version: 7.6.0
+  url: https://conda.anaconda.org/conda-forge/noarch/nbconvert-7.7.1-pyhd8ed1ab_1.conda
+  version: 7.7.1
 - category: main
   dependencies:
     jupyter_server: '>=1.8,<3'
     python: '>=3.7'
   hash:
     md5: 67e0fe74c156267d9159e9133df7fd37
     sha256: f028d7ad1f2175cde307db08b60d07e371b9d6f035cfae6c81ea94b4c408c538
@@ -12853,25 +12940,26 @@
   name: double-conversion
   optional: false
   platform: win-64
   url: https://conda.anaconda.org/conda-forge/win-64/double-conversion-3.2.0-h63175ca_1.tar.bz2
   version: 3.2.0
 - category: main
   dependencies:
-    vc: '>=14.1,<15.0a0'
-    vs2015_runtime: '>=14.16.27012'
+    ucrt: '>=10.0.20348.0'
+    vc: '>=14.2,<15'
+    vc14_runtime: '>=14.29.30139'
   hash:
-    md5: 72fab4b0a033b718950cc5d930cbd1a6
-    sha256: 0adf15b86f2d130d7772b8a0792febb5e67a9eb2f63191701a94f686000e46d9
+    md5: 3671ee2bcd1d915690de5b1445fdf004
+    sha256: adcf12c65b6d1e8ef875ee2845f687957461a7869a1b1474cf6c4ac9024678df
   manager: conda
   name: eigen
   optional: false
   platform: win-64
-  url: https://conda.anaconda.org/conda-forge/win-64/eigen-3.4.0-h2d74725_0.tar.bz2
-  version: 3.4.0
+  url: https://conda.anaconda.org/conda-forge/win-64/eigen-3.4.1-h91493d7_0.conda
+  version: 3.4.1
 - category: main
   dependencies:
     ucrt: '>=10.0.20348.0'
     vc: '>=14.2,<15'
     vc14_runtime: '>=14.29.30139'
   hash:
     md5: 09196a7ba69b70d2124aff7b2763035d
@@ -13692,23 +13780,23 @@
   url: https://conda.anaconda.org/conda-forge/win-64/zlib-1.2.13-hcfcfb64_5.conda
   version: 1.2.13
 - category: main
   dependencies:
     libzlib: '>=1.2.13,<1.3.0a0'
     ucrt: '>=10.0.20348.0'
     vc: '>=14.2,<15'
-    vs2015_runtime: '>=14.29.30139'
+    vc14_runtime: '>=14.29.30139'
   hash:
-    md5: 62826565682d013b3e2346aaf7bded0e
-    sha256: ef23b2eb748b0b2139755e5a20d49a642340af1313017918dc91b4a4ce8f3bd9
+    md5: f3c3879d8cda1c5a6885435dd48a470e
+    sha256: 33e8fb73dee10740f00d4a450ad2d7f6d90692ca781480fa18fa70fd417d53ad
   manager: conda
   name: zstd
   optional: false
   platform: win-64
-  url: https://conda.anaconda.org/conda-forge/win-64/zstd-1.5.2-h12be248_6.conda
+  url: https://conda.anaconda.org/conda-forge/win-64/zstd-1.5.2-h12be248_7.conda
   version: 1.5.2
 - category: main
   dependencies:
     python: '>=3.6'
   hash:
     md5: dd5eed01874c75bebef810a2faec673e
     sha256: 1cc3eb4ee86271dfcfb0673cb7aa2632e43024b7f1324ca23689dcfbe0631b2f
@@ -13818,22 +13906,22 @@
   platform: win-64
   url: https://conda.anaconda.org/conda-forge/noarch/certifi-2023.5.7-pyhd8ed1ab_0.conda
   version: 2023.5.7
 - category: main
   dependencies:
     python: '>=3.7'
   hash:
-    md5: 7fcff9f6f123696e940bda77bd4d6551
-    sha256: 06cd371fc98f076797d6450f6f337cb679b1060c99680fb7e044591493333194
+    md5: 313516e9a4b08b12dfb1e1cd390a96e3
+    sha256: 0666a95fbbd2299008162e2126c009191e5953d1cad1878bf9f4d8d634af1dd4
   manager: conda
   name: charset-normalizer
   optional: false
   platform: win-64
-  url: https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-3.1.0-pyhd8ed1ab_0.conda
-  version: 3.1.0
+  url: https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-3.2.0-pyhd8ed1ab_0.conda
+  version: 3.2.0
 - category: main
   dependencies:
     python: '>=3.7'
   hash:
     md5: 3faab06a954c2a04039983f2c4a50d99
     sha256: 2c1b2e9755ce3102bca8d69e8f26e4f087ece73f50418186aee7c74bef8e1698
   manager: conda
@@ -14030,24 +14118,24 @@
   version: 2.12.1
 - category: main
   dependencies:
     python: '>=3.10,<3.11.0a0'
     python_abi: 3.10.* *_cp310
     ucrt: '>=10.0.20348.0'
     vc: '>=14.2,<15'
-    vs2015_runtime: '>=14.29.30139'
+    vc14_runtime: '>=14.29.30139'
   hash:
-    md5: 550271ca005a4c805cd7391cef008dc6
-    sha256: 1f88ceb482479902152030eaaa0a20e558d365e2968a94674770a7e8ff87486e
+    md5: 7eba3cb7b26fbaee485f63e84824c7cd
+    sha256: 0d53b0f82918e3ab4bdfe39dc2d0bbc51ba73ad5e243de4da15632730ae20dee
   manager: conda
   name: frozenlist
   optional: false
   platform: win-64
-  url: https://conda.anaconda.org/conda-forge/win-64/frozenlist-1.3.3-py310h8d17308_0.tar.bz2
-  version: 1.3.3
+  url: https://conda.anaconda.org/conda-forge/win-64/frozenlist-1.4.0-py310h8d17308_0.conda
+  version: 1.4.0
 - category: main
   dependencies:
     python: '>=3.8'
   hash:
     md5: 50ea2067ec92dfcc38b4f07992d7e235
     sha256: 0015e12d85b454ca8e09085e9e788a6156f4f1da1b270019cab2658381d60258
   manager: conda
@@ -14248,42 +14336,42 @@
     libiconv: '>=1.17,<2.0a0'
     libzlib: '>=1.2.13,<1.3.0a0'
     pcre2: '>=10.40,<10.41.0a0'
     ucrt: '>=10.0.20348.0'
     vc: '>=14.2,<15'
     vc14_runtime: '>=14.29.30139'
   hash:
-    md5: 4695e6acaf4790170161048d56cb51fc
-    sha256: 170d42dcf0c73f5846dfb0c4a241c065cd9830c644d98042f076f25c309e7571
+    md5: 8c3f24acdc0403eeb3fb42ab75e8a659
+    sha256: 4d7b96d0ed8b46df5ccd5de7e726c1ed81c9dc4526460e7608d9dbdbb8ac18f5
   manager: conda
   name: libglib
   optional: false
   platform: win-64
-  url: https://conda.anaconda.org/conda-forge/win-64/libglib-2.76.3-he8f3873_0.conda
-  version: 2.76.3
+  url: https://conda.anaconda.org/conda-forge/win-64/libglib-2.76.4-he8f3873_0.conda
+  version: 2.76.4
 - category: main
   dependencies:
     c-ares: '>=1.19.1,<2.0a0'
     libabseil: '>=20230125.3,<20230126.0a0'
     libprotobuf: '>=4.23.3,<4.23.4.0a0'
     libzlib: '>=1.2.13,<1.3.0a0'
     openssl: '>=3.1.1,<4.0a0'
     re2: '>=2023.3.2,<2023.3.3.0a0'
     ucrt: '>=10.0.20348.0'
     vc: '>=14.2,<15'
     vc14_runtime: '>=14.29.30139'
   hash:
-    md5: 44b832412b9a71277e67ecc52ffec4f2
-    sha256: 6a6791a8e6e68c36805ed83f6ad0929c20fcd5f3249cff5242f09a39e7f136fd
+    md5: 240221f7a200e718c242637e6c437b61
+    sha256: 42de23c2d63c3ab3d17ac145020c330340f4b1f2267692775e25ed93d85164eb
   manager: conda
   name: libgrpc
   optional: false
   platform: win-64
-  url: https://conda.anaconda.org/conda-forge/win-64/libgrpc-1.56.0-hea2d5f7_2.conda
-  version: 1.56.0
+  url: https://conda.anaconda.org/conda-forge/win-64/libgrpc-1.56.2-hea2d5f7_0.conda
+  version: 1.56.2
 - category: main
   dependencies:
     libxml2: '>=2.10.3,<2.11.0a0'
     pthreads-win32: ''
     ucrt: '>=10.0.20348.0'
     vc: '>=14.2,<15'
     vs2015_runtime: '>=14.29.30139'
@@ -14540,22 +14628,22 @@
   platform: win-64
   url: https://conda.anaconda.org/conda-forge/noarch/ply-3.11-py_1.tar.bz2
   version: '3.11'
 - category: main
   dependencies:
     python: '>=3.6'
   hash:
-    md5: 95c5be3c7cbd872509d16c216617fdab
-    sha256: eb11fd8b927d9c5ff9482cfbd6cd810a43a1351c44a288e9680542ea698a19a0
+    md5: 02153b6b760bbec00cfe9e4c97993d06
+    sha256: a149184fde856dba7968fc50ca89dbb07ebe84abd710d4076e2fada1b9399231
   manager: conda
   name: prometheus_client
   optional: false
   platform: win-64
-  url: https://conda.anaconda.org/conda-forge/noarch/prometheus_client-0.17.0-pyhd8ed1ab_0.conda
-  version: 0.17.0
+  url: https://conda.anaconda.org/conda-forge/noarch/prometheus_client-0.17.1-pyhd8ed1ab_0.conda
+  version: 0.17.1
 - category: main
   dependencies:
     python: '>=3.10,<3.11.0a0'
     python_abi: 3.10.* *_cp310
     ucrt: '>=10.0.20348.0'
     vc: '>=14.2,<15'
     vs2015_runtime: '>=14.29.30139'
@@ -14652,34 +14740,34 @@
   platform: win-64
   url: https://conda.anaconda.org/conda-forge/noarch/pygments-2.15.1-pyhd8ed1ab_0.conda
   version: 2.15.1
 - category: main
   dependencies:
     python: '>=3.6'
   hash:
-    md5: 99e28be5a278e2319834d7dc99e7bfdd
-    sha256: f3a64306fa0f405f10f4108d7ff42043d6fd393f940f9e98e395a3756687fc98
+    md5: 912c0194f898fdb783021fd25f913c31
+    sha256: 88ac94c42ade15113397e30d1831dd341399b5262fb5330b9240f915c33cd232
   manager: conda
   name: pyjwt
   optional: false
   platform: win-64
-  url: https://conda.anaconda.org/conda-forge/noarch/pyjwt-2.7.0-pyhd8ed1ab_0.conda
-  version: 2.7.0
+  url: https://conda.anaconda.org/conda-forge/noarch/pyjwt-2.8.0-pyhd8ed1ab_0.conda
+  version: 2.8.0
 - category: main
   dependencies:
     python: '>=3.6'
   hash:
-    md5: d3ed087d1f7f8f5590e8e87b57a8ce64
-    sha256: 18e3bd52c64f23bbc7c200fd2fc4152dd29423936dc43e8f129cb43f1af0136c
+    md5: e8fbc1b54b25f4b08281467bc13b70cc
+    sha256: 4acc7151cef5920d130f2e0a7615559cce8bfb037aeecb14d4d359ae3d9bc51b
   manager: conda
   name: pyparsing
   optional: false
   platform: win-64
-  url: https://conda.anaconda.org/conda-forge/noarch/pyparsing-3.1.0-pyhd8ed1ab_0.conda
-  version: 3.1.0
+  url: https://conda.anaconda.org/conda-forge/noarch/pyparsing-3.0.9-pyhd8ed1ab_0.tar.bz2
+  version: 3.0.9
 - category: main
   dependencies:
     python: '>=3.10,<3.11.0a0'
     python_abi: 3.10.* *_cp310
     ucrt: '>=10.0.20348.0'
     vc: '>=14.2,<15'
     vs2015_runtime: '>=14.29.30139'
@@ -14746,25 +14834,25 @@
   version: '304'
 - category: main
   dependencies:
     python: '>=3.10,<3.11.0a0'
     python_abi: 3.10.* *_cp310
     ucrt: '>=10.0.20348.0'
     vc: '>=14.2,<15'
-    vs2015_runtime: '>=14.29.30139'
+    vc14_runtime: '>=14.29.30139'
     winpty: ''
   hash:
-    md5: b0fb5ffdb72cb3b46bc9fdc163cf411d
-    sha256: 7adb8043a35dbd38ae0fbcac58f53c283e21ac61395de5028f905ce8e1548378
+    md5: 685cf7fe1b0724628476c991329017ad
+    sha256: 92145040d25738e56feb5c766eb6a613776ec574c4a3abb5eddc3cbe31d078da
   manager: conda
   name: pywinpty
   optional: false
   platform: win-64
-  url: https://conda.anaconda.org/conda-forge/win-64/pywinpty-2.0.10-py310h00ffb61_0.conda
-  version: 2.0.10
+  url: https://conda.anaconda.org/conda-forge/win-64/pywinpty-2.0.11-py310h00ffb61_0.conda
+  version: 2.0.11
 - category: main
   dependencies:
     python: '>=3.10,<3.11.0a0'
     python_abi: 3.10.* *_cp310
     ucrt: '>=10.0.20348.0'
     vc: '>=14.2,<15'
     vs2015_runtime: '>=14.29.30139'
@@ -14806,14 +14894,30 @@
   name: rfc3986-validator
   optional: false
   platform: win-64
   url: https://conda.anaconda.org/conda-forge/noarch/rfc3986-validator-0.1.1-pyh9f0ad1d_0.tar.bz2
   version: 0.1.1
 - category: main
   dependencies:
+    python: '>=3.10,<3.11.0a0'
+    python_abi: 3.10.* *_cp310
+    ucrt: '>=10.0.20348.0'
+    vc: '>=14.2,<15'
+    vs2015_runtime: '>=14.29.30139'
+  hash:
+    md5: e7cee92d4b0e9f8a68823d2501a87063
+    sha256: 42e99939c0f04e1a6a98de6f797ab48859e7d498d56f950939995ed42ed2c3d7
+  manager: conda
+  name: ruamel.yaml.clib
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/win-64/ruamel.yaml.clib-0.2.7-py310h8d17308_1.conda
+  version: 0.2.7
+- category: main
+  dependencies:
     python: '>=3.7'
   hash:
     md5: 3b68bc43ec6baa48f7354a446267eefe
     sha256: 3ac44771fce01f19218bcdf3992e24984748048db69889a9df65abcc6a10e29b
   manager: conda
   name: setuptools
   optional: false
@@ -15033,22 +15137,22 @@
   platform: win-64
   url: https://conda.anaconda.org/conda-forge/win-64/typed-ast-1.5.5-py310h8d17308_0.conda
   version: 1.5.5
 - category: main
   dependencies:
     python: '>=3.7'
   hash:
-    md5: 4a3014a4d107d15475d106b751c4e352
-    sha256: 90a8d56c8015af1575d504d5f77d95a806cd999fc178a06ab51a349f1f744672
+    md5: c39d6a09fe819de4951c2642629d9115
+    sha256: 6edd6d5be690be492712cb747b6d62707f0d0c34ef56eefc796d91e5a03187d1
   manager: conda
   name: typing_extensions
   optional: false
   platform: win-64
-  url: https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.6.3-pyha770c72_0.conda
-  version: 4.6.3
+  url: https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.7.1-pyha770c72_0.conda
+  version: 4.7.1
 - category: main
   dependencies:
     python: '>=3.6.1'
   hash:
     md5: eb67e3cace64c66233e2d35949e20f92
     sha256: 9e3758b620397f56fb709f796969de436d63b7117897159619b87938e1f78739
   manager: conda
@@ -15121,21 +15225,21 @@
   platform: win-64
   url: https://conda.anaconda.org/conda-forge/noarch/websocket-client-1.6.1-pyhd8ed1ab_0.conda
   version: 1.6.1
 - category: main
   dependencies:
     python: '>=3.7'
   hash:
-    md5: 49bb0d9e60ce1db25e151780331bb5f3
-    sha256: 79b4d29b0c004014a2abd5fc2c9fcd35cc6256222b960c2a317a27c4b0d8884d
+    md5: c95fac682453aeffa12db7ae5a721bec
+    sha256: e91cbb3c0ad9a9507dd030f5493831cb52da120329e0d0793711e8300a36db22
   manager: conda
   name: wheel
   optional: false
   platform: win-64
-  url: https://conda.anaconda.org/conda-forge/noarch/wheel-0.40.0-pyhd8ed1ab_0.conda
+  url: https://conda.anaconda.org/conda-forge/noarch/wheel-0.40.0-pyhd8ed1ab_1.conda
   version: 0.40.0
 - category: main
   dependencies:
     python: '>=3.7'
   hash:
     md5: 2e9ebddf0b93d0fb203d0906b8052c4f
     sha256: a73d34f8169e206bccfb356c093ff5ced803b953bbcc1480ed27976f97598d68
@@ -15257,24 +15361,24 @@
   name: xorg-xproto
   optional: false
   platform: win-64
   url: https://conda.anaconda.org/conda-forge/win-64/xorg-xproto-7.0.31-hcd874cb_1007.tar.bz2
   version: 7.0.31
 - category: main
   dependencies:
-    python: '>=3.7'
+    python: '>=3.8'
   hash:
-    md5: 13018819ca8f5b7cc675a8faf1f5fedf
-    sha256: 241de30545299be9bcea3addf8a2c22a3b3d4ba6730890e150ab690ac937a3d2
+    md5: 2da0451b54c4563c32490cb1b7cf68a1
+    sha256: 16d72127e150a3d5cbdc0b82c4069ef5be135c64bc99e71e7928507910669b41
   manager: conda
   name: zipp
   optional: false
   platform: win-64
-  url: https://conda.anaconda.org/conda-forge/noarch/zipp-3.15.0-pyhd8ed1ab_0.conda
-  version: 3.15.0
+  url: https://conda.anaconda.org/conda-forge/noarch/zipp-3.16.2-pyhd8ed1ab_0.conda
+  version: 3.16.2
 - category: main
   dependencies:
     pygments: ''
     python: '>=3.6'
   hash:
     md5: 46a2e6e3dfa718ce3492018d5a110dd6
     sha256: ce532e2da08fb2b77df281e3d42e2b2131641bdd6a6e8127f3718ae6860bd70d
@@ -15301,22 +15405,22 @@
   dependencies:
     exceptiongroup: ''
     idna: '>=2.8'
     python: '>=3.7'
     sniffio: '>=1.1'
     typing_extensions: ''
   hash:
-    md5: 2b35a85d654a47aac8f34c1bb6de7142
-    sha256: 863c11a6a0e937977229b405a16f6d43fff543dfe5b1a66da9c42ec0cbdaaf33
+    md5: 7b517e7a6f0790337906c055aa97ca49
+    sha256: 62637ac498bcf47783cbf4f48e9b09e4e2f5a6ad42f43ca8f632c353827b94f4
   manager: conda
   name: anyio
   optional: false
   platform: win-64
-  url: https://conda.anaconda.org/conda-forge/noarch/anyio-3.7.0-pyhd8ed1ab_1.conda
-  version: 3.7.0
+  url: https://conda.anaconda.org/conda-forge/noarch/anyio-3.7.1-pyhd8ed1ab_0.conda
+  version: 3.7.1
 - category: main
   dependencies:
     python: '>=3.5'
     six: ''
   hash:
     md5: bf7f54dd0f25c3f06ecb82a07341841a
     sha256: 7ed530efddd47a96c11197906b4008405b90e3bc2f4e0df722a36e0e6103fd9c
@@ -15418,22 +15522,22 @@
   version: 1.15.1
 - category: main
   dependencies:
     __win: ''
     colorama: ''
     python: '>=3.8'
   hash:
-    md5: 6b58680207b526c42dcff68b543803dd
-    sha256: 84e80a33e9a8e5398d3e97209366b57f635462a5b894f8076ec8c95e56672c44
+    md5: c1e57b6771510a3d2648ed6e76277391
+    sha256: 6fa8a7c644073b88ef3f857bb56f51efcf7c3852777a009187360f9a6bd1c606
   manager: conda
   name: click
   optional: false
   platform: win-64
-  url: https://conda.anaconda.org/conda-forge/noarch/click-8.1.3-win_pyhd8ed1ab_2.tar.bz2
-  version: 8.1.3
+  url: https://conda.anaconda.org/conda-forge/noarch/click-8.1.6-win_pyh7428d3b_0.conda
+  version: 8.1.6
 - category: main
   dependencies:
     python: '>=3.6'
     traitlets: '>=5.3'
   hash:
     md5: 168ae0f82cdf7505048e81054c7354e4
     sha256: 657e0a513c8705dc542c54c4c5234e813b7f4e2f412688796d611e83ddf132ea
@@ -15518,46 +15622,46 @@
   name: fontconfig
   optional: false
   platform: win-64
   url: https://conda.anaconda.org/conda-forge/win-64/fontconfig-2.14.2-hbde0cde_0.conda
   version: 2.14.2
 - category: main
   dependencies:
-    libglib: 2.76.3 he8f3873_0
+    libglib: 2.76.4 he8f3873_0
     libzlib: '>=1.2.13,<1.3.0a0'
     ucrt: '>=10.0.20348.0'
     vc: '>=14.2,<15'
     vc14_runtime: '>=14.29.30139'
   hash:
-    md5: 3015483cb3ffa200d51aac3c691fcda0
-    sha256: 10cc47bc9194e42ea984e437e3d99c794d5d6e7c5ac2994716054fcbcf65d33a
+    md5: 88237d3ddd338164196043cb7e927246
+    sha256: f90981fd787047c1b355bdaa9a981a5822152d3121f696d532ed29d51acc1507
   manager: conda
   name: glib-tools
   optional: false
   platform: win-64
-  url: https://conda.anaconda.org/conda-forge/win-64/glib-tools-2.76.3-h12be248_0.conda
-  version: 2.76.3
+  url: https://conda.anaconda.org/conda-forge/win-64/glib-tools-2.76.4-h12be248_0.conda
+  version: 2.76.4
 - category: main
   dependencies:
-    libgrpc: 1.56.0 hea2d5f7_2
+    libgrpc: 1.56.2 hea2d5f7_0
     libzlib: '>=1.2.13,<1.3.0a0'
     python: '>=3.10,<3.11.0a0'
     python_abi: 3.10.* *_cp310
     ucrt: '>=10.0.20348.0'
     vc: '>=14.2,<15'
     vc14_runtime: '>=14.29.30139'
   hash:
-    md5: c624ac3dd1ada404b8d8cc378bb60daf
-    sha256: b53354f228f80551ef7326cf108197c4a362334e5e1ef6695cd0532db87c99f0
+    md5: 1c43b1323746f119bfea36e689930225
+    sha256: 7a14fcbfbe24e7ce3bcb5e230c1c8d90ef919a0edfea9fb2cb405e54de9d8812
   manager: conda
   name: grpcio
   optional: false
   platform: win-64
-  url: https://conda.anaconda.org/conda-forge/win-64/grpcio-1.56.0-py310hb84602e_2.conda
-  version: 1.56.0
+  url: https://conda.anaconda.org/conda-forge/win-64/grpcio-1.56.2-py310hb84602e_0.conda
+  version: 1.56.2
 - category: main
   dependencies:
     libglib: '>=2.76.3,<3.0a0'
     ucrt: '>=10.0.20348.0'
     vc: '>=14.2,<15'
     vc14_runtime: '>=14.29.30139'
   hash:
@@ -15587,35 +15691,35 @@
   url: https://conda.anaconda.org/conda-forge/win-64/hdf5-1.12.2-nompi_h57737ce_101.conda
   version: 1.12.2
 - category: main
   dependencies:
     python: '>=3.8'
     zipp: '>=0.5'
   hash:
-    md5: ba3786c6846e46038fe60c785d46dc81
-    sha256: 1ffffc30dc67d8329d47c6d22de726cfd28d7ed236bca54f52fc0bdcd0a53fc7
+    md5: 4e9f59a060c3be52bc4ddc46ee9b6946
+    sha256: 2797ed927d65324309b6c630190d917b9f2111e0c217b721f80429aeb57f9fcf
   manager: conda
   name: importlib-metadata
   optional: false
   platform: win-64
-  url: https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-6.7.0-pyha770c72_0.conda
-  version: 6.7.0
+  url: https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-6.8.0-pyha770c72_0.conda
+  version: 6.8.0
 - category: main
   dependencies:
-    python: '>=3.7'
+    python: '>=3.8'
     zipp: '>=3.1.0'
   hash:
-    md5: e5fd2260a231ee63b6969f4801082f2b
-    sha256: 091cca3e010f7a7353152f0abda2d68cfd83ddde80a15e974d9e18b2047e7be2
+    md5: a08b6be5bf18b9d2a927d3457750f82e
+    sha256: 94c1b2831c0f908ae56212d9aeb9c9173051d307682b4fedfd88fef774b0b8f7
   manager: conda
   name: importlib_resources
   optional: false
   platform: win-64
-  url: https://conda.anaconda.org/conda-forge/noarch/importlib_resources-5.12.0-pyhd8ed1ab_0.conda
-  version: 5.12.0
+  url: https://conda.anaconda.org/conda-forge/noarch/importlib_resources-6.0.0-pyhd8ed1ab_1.conda
+  version: 6.0.0
 - category: main
   dependencies:
     parso: '>=0.8.0,<0.9.0'
     python: '>=3.6'
   hash:
     md5: b5e695ef9c3f0d27d6cd96bf5adc9e07
     sha256: abe63ae6e1b13f83500608d94004cb8d485b264083511d77f79253e775cd546c
@@ -15996,14 +16100,32 @@
   name: rsa
   optional: false
   platform: win-64
   url: https://conda.anaconda.org/conda-forge/noarch/rsa-4.9-pyhd8ed1ab_0.tar.bz2
   version: '4.9'
 - category: main
   dependencies:
+    python: '>=3.10,<3.11.0a0'
+    python_abi: 3.10.* *_cp310
+    ruamel.yaml.clib: '>=0.1.2'
+    setuptools: ''
+    ucrt: '>=10.0.20348.0'
+    vc: '>=14.2,<15'
+    vc14_runtime: '>=14.29.30139'
+  hash:
+    md5: c13c515dcc8f25ea5407630e172ed83c
+    sha256: 5f21b7fddaf2b82ee7ce2c313aa23029ec168907e4dc10c946c3cfdf9d9c7f90
+  manager: conda
+  name: ruamel.yaml
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/win-64/ruamel.yaml-0.17.32-py310h8d17308_0.conda
+  version: 0.17.32
+- category: main
+  dependencies:
     __win: ''
     python: '>=3.6'
     pywin32: ''
   hash:
     md5: c00d32dfa733d381b6a1908d0d67e0d7
     sha256: 55208c6b48d68dc9ad2e2cf81ab9dc6b8a1d607e67acf9115bdc7794accc84bc
   manager: conda
@@ -16098,24 +16220,24 @@
   name: tqdm
   optional: false
   platform: win-64
   url: https://conda.anaconda.org/conda-forge/noarch/tqdm-4.65.0-pyhd8ed1ab_1.conda
   version: 4.65.0
 - category: main
   dependencies:
-    typing_extensions: 4.6.3 pyha770c72_0
+    typing_extensions: 4.7.1 pyha770c72_0
   hash:
-    md5: 3876f650ed7d0f95d70fa4b647621909
-    sha256: d2334dab270e13182403cc3a394e3da8e7acb409e94059a6d9223d2ac053f90a
+    md5: f96688577f1faa58096d06a45136afa2
+    sha256: d5d19b8f5b275240c19616a46d67ec57250b3720ba88200da8c732c3fcbfc21d
   manager: conda
   name: typing-extensions
   optional: false
   platform: win-64
-  url: https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.6.3-hd8ed1ab_0.conda
-  version: 4.6.3
+  url: https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.7.1-hd8ed1ab_0.conda
+  version: 4.7.1
 - category: main
   dependencies:
     markupsafe: '>=2.1.1'
     python: '>=3.8'
   hash:
     md5: 55fbbb3e67185820ee2007395bfe0073
     sha256: 28515f7ddb8a20f1436b9ac3a6ba2aa9be337995e4ee63c72d0f5d0efd6a2062
@@ -16177,22 +16299,22 @@
   dependencies:
     lazy-object-proxy: '>=1.4.0'
     python: '>=3.10,<3.11.0a0'
     python_abi: 3.10.* *_cp310
     typing-extensions: '>=4.0.0'
     wrapt: <2,>=1.11
   hash:
-    md5: d8b37ae3e9ac63ddb024cea93df674aa
-    sha256: d3aa4a006149c3275a29c731509c287ae6cb51d7d65e74804276e6936f43f6d7
+    md5: a1e30c9be3eb810b8efdd581449983cc
+    sha256: 5e8eb649bb12a1e058883be6e37d357559c8ab46eb2aeffc2b401f4e5a621001
   manager: conda
   name: astroid
   optional: false
   platform: win-64
-  url: https://conda.anaconda.org/conda-forge/win-64/astroid-2.15.5-py310h5588dad_0.conda
-  version: 2.15.5
+  url: https://conda.anaconda.org/conda-forge/win-64/astroid-2.15.6-py310h5588dad_0.conda
+  version: 2.15.6
 - category: main
   dependencies:
     python: '>=3.6'
     typing-extensions: '>=3.6.5'
   hash:
     md5: 25e79f9a1133556671becbd65a170c78
     sha256: a08b78e6fadee1ffac0f255363d2a08a0c589c7403fd2a71c1c0b6aafd5e0737
@@ -16247,22 +16369,22 @@
     openssl: '>=3.1.1,<4.0a0'
     python: '>=3.10,<3.11.0a0'
     python_abi: 3.10.* *_cp310
     ucrt: '>=10.0.20348.0'
     vc: '>=14.2,<15'
     vc14_runtime: '>=14.29.30139'
   hash:
-    md5: dcd180d7b04ea819607366a35f323108
-    sha256: f7f15001093ef4bb3bce3898b7b945aed670e454318be33110f9aebbe689a0c3
+    md5: 507f1964c07ee129d1317e601a2bfb94
+    sha256: 42c22bc1372d12c4d1e2c9755f2d546e588f43f1117d78653b16137aa625bd4d
   manager: conda
   name: cryptography
   optional: false
   platform: win-64
-  url: https://conda.anaconda.org/conda-forge/win-64/cryptography-41.0.1-py310h6e82f81_0.conda
-  version: 41.0.1
+  url: https://conda.anaconda.org/conda-forge/win-64/cryptography-41.0.2-py310h6e82f81_0.conda
+  version: 41.0.2
 - category: main
   dependencies:
     aom: '>=3.5.0,<3.6.0a0'
     bzip2: '>=1.0.8,<2.0a0'
     dav1d: '>=1.2.0,<1.2.1.0a0'
     fontconfig: '>=2.14.2,<3.0a0'
     fonts-conda-ecosystem: ''
@@ -16293,22 +16415,22 @@
     python: '>=3.10,<3.11.0a0'
     python_abi: 3.10.* *_cp310
     ucrt: '>=10.0.20348.0'
     unicodedata2: '>=14.0.0'
     vc: '>=14.2,<15'
     vc14_runtime: '>=14.29.30139'
   hash:
-    md5: a18e1160ee09a9f5ac26b2ce965832f7
-    sha256: 417cbde320ed8a56796aac0913abb19c67156fb2429fa6b237a84591ff0a74a9
+    md5: 496704d1b32153ed96e60de270a3e2f4
+    sha256: 484cccfac21ddb4eef4daded8e95df485ee525fcc38f27efdafeb5d48c330cc9
   manager: conda
   name: fonttools
   optional: false
   platform: win-64
-  url: https://conda.anaconda.org/conda-forge/win-64/fonttools-4.40.0-py310h8d17308_0.conda
-  version: 4.40.0
+  url: https://conda.anaconda.org/conda-forge/win-64/fonttools-4.41.0-py310h8d17308_0.conda
+  version: 4.41.0
 - category: main
   dependencies:
     python: '>=3.6'
     python-dateutil: '>=2.8.1'
   hash:
     md5: 6d8d61116031a3f5b1f32e7899785866
     sha256: 097d9b4c946b195800bc68f68393370049238509b08ef828c06fbf481bbc139c
@@ -16317,42 +16439,42 @@
   optional: false
   platform: win-64
   url: https://conda.anaconda.org/conda-forge/noarch/ghp-import-2.1.0-pyhd8ed1ab_0.tar.bz2
   version: 2.1.0
 - category: main
   dependencies:
     gettext: '>=0.21.1,<1.0a0'
-    glib-tools: 2.76.3 h12be248_0
-    libglib: 2.76.3 he8f3873_0
+    glib-tools: 2.76.4 h12be248_0
+    libglib: 2.76.4 he8f3873_0
     libzlib: '>=1.2.13,<1.3.0a0'
     python: '*'
     ucrt: '>=10.0.20348.0'
     vc: '>=14.2,<15'
     vc14_runtime: '>=14.29.30139'
   hash:
-    md5: fa3f1af2dc70e0d00a755667a741fad3
-    sha256: 6c6f526cc153feeee786daf16f2790a8ff4478fde752b2d0d3619c884f00b898
+    md5: 4d7ae53ee4b7e08f3fbd1d3a7efd4812
+    sha256: 96457df6c2cb42ec32c25a135ca1232e740f21fe20216e54024df9274f5ae4ad
   manager: conda
   name: glib
   optional: false
   platform: win-64
-  url: https://conda.anaconda.org/conda-forge/win-64/glib-2.76.3-h12be248_0.conda
-  version: 2.76.3
+  url: https://conda.anaconda.org/conda-forge/win-64/glib-2.76.4-h12be248_0.conda
+  version: 2.76.4
 - category: main
   dependencies:
-    importlib-metadata: '>=6.7.0,<6.7.1.0a0'
+    importlib-metadata: '>=6.8.0,<6.8.1.0a0'
   hash:
-    md5: 27a4cec373ec84d1c1aa02a1e37f8eaf
-    sha256: f46d34a06e63f220dd04f7ac211dd2b4812b6b8a9e851467cd2e0218174d2dfd
+    md5: b279b07ce18058034e5b3606ba103a8b
+    sha256: b96e01dc42d547d6d9ceb1c5b52a5232cc04e40153534350f702c3e0418a6b3f
   manager: conda
   name: importlib_metadata
   optional: false
   platform: win-64
-  url: https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-6.7.0-hd8ed1ab_0.conda
-  version: 6.7.0
+  url: https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-6.8.0-hd8ed1ab_0.conda
+  version: 6.8.0
 - category: main
   dependencies:
     attrs: '>=17.4.0'
     importlib-metadata: ''
     importlib_resources: '>=1.4.0'
     pkgutil-resolve-name: '>=1.3.10'
     pyrsistent: '!=0.17.0,!=0.17.1,!=0.17.2,>=0.14.0'
@@ -16487,22 +16609,22 @@
   url: https://conda.anaconda.org/conda-forge/win-64/pillow-9.2.0-py310hd4fb230_3.tar.bz2
   version: 9.2.0
 - category: main
   dependencies:
     python: '>=3.7'
     typing-extensions: '>=4.6.3'
   hash:
-    md5: 3e4aca765371893ad848397794600632
-    sha256: 5f382d0d3509784152506e0e022bb5a30d254555e809804491207196f890af67
+    md5: 044e7a1e0ad42c4e67110bd078150a63
+    sha256: 885611bd528abaf3e31bc0bfaad3a619cfe89db61d886b53c2a9ec9ff50edebe
   manager: conda
   name: platformdirs
   optional: false
   platform: win-64
-  url: https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.8.0-pyhd8ed1ab_0.conda
-  version: 3.8.0
+  url: https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.9.1-pyhd8ed1ab_0.conda
+  version: 3.9.1
 - category: main
   dependencies:
     latexcodec: '>=1.0.4'
     python: '>=3.6'
     pyyaml: '>=3.01'
     setuptools: ''
     six: ''
@@ -16573,22 +16695,22 @@
     python: '>=3.10,<3.11.0a0'
     python_abi: 3.10.* *_cp310
     typing-extensions: '>=4.2.0'
     ucrt: '>=10.0.20348.0'
     vc: '>=14.2,<15'
     vc14_runtime: '>=14.29.30139'
   hash:
-    md5: 1a7ef45ab2cbed2272dc7bed9ee6f98a
-    sha256: 97cac75adba50a7fe35ae1abf29d5900e92f06f1ed08fc18ae5bfb4ea78175f1
+    md5: 4cfc2aca9d88ef166474d84cb9c51451
+    sha256: a459271587f425203f2664ee8b42d93ee0dbff46e49d611f03257ad25b1655d3
   manager: conda
   name: sqlalchemy
   optional: false
   platform: win-64
-  url: https://conda.anaconda.org/conda-forge/win-64/sqlalchemy-2.0.17-py310h8d17308_0.conda
-  version: 2.0.17
+  url: https://conda.anaconda.org/conda-forge/win-64/sqlalchemy-2.0.19-py310h8d17308_0.conda
+  version: 2.0.19
 - category: main
   dependencies:
     asttokens: ''
     executing: ''
     pure_eval: ''
     python: '>=3.5'
   hash:
@@ -16656,22 +16778,22 @@
     python: '>=3.10,<3.11.0a0'
     python_abi: 3.10.* *_cp310
     ucrt: '>=10.0.20348.0'
     vc: '>=14.2,<15'
     vc14_runtime: '>=14.29.30139'
     yarl: '>=1.0,<2.0'
   hash:
-    md5: c759aad020f1363a27088e6c621f4db1
-    sha256: 29265f10cc4b3a72a0f720b7fa975509a459df89cfc00ff3affdaa3dce709365
+    md5: cb4d6c6556ca7dfad7f75b1b371ecb30
+    sha256: 69805ed5b197795ed9e1457099b623df9eaffffe593c76a1a9b53ad09e281e22
   manager: conda
   name: aiohttp
   optional: false
   platform: win-64
-  url: https://conda.anaconda.org/conda-forge/win-64/aiohttp-3.8.4-py310h8d17308_1.conda
-  version: 3.8.4
+  url: https://conda.anaconda.org/conda-forge/win-64/aiohttp-3.8.5-py310h8d17308_0.conda
+  version: 3.8.5
 - category: main
   dependencies:
     argon2-cffi-bindings: ''
     flit-core: '>=3.4,<4'
     python: '>=3.6'
   hash:
     md5: a0b402db58f73aaab8ee0ca1025a362e
@@ -16708,21 +16830,21 @@
     glib: '>=2.76.3,<3.0a0'
     libglib: '>=2.76.3,<3.0a0'
     libiconv: '>=1.17,<2.0a0'
     ucrt: '>=10.0.20348.0'
     vc: '>=14.2,<15'
     vc14_runtime: '>=14.29.30139'
   hash:
-    md5: ead79af9af7587ca3f685fed4966a881
-    sha256: c8473fd20f328fcb1840ce402fc3876b004e14370cb9509ae0220ffad3fce14e
+    md5: 42f53931331420f6b748f91ef356a558
+    sha256: 5f9e74b2114872ed0ababbeaf5915a59729d1cc993a453de7584eaece1ddab91
   manager: conda
   name: gstreamer
   optional: false
   platform: win-64
-  url: https://conda.anaconda.org/conda-forge/win-64/gstreamer-1.22.4-hb4038d2_0.conda
+  url: https://conda.anaconda.org/conda-forge/win-64/gstreamer-1.22.4-hb4038d2_1.conda
   version: 1.22.4
 - category: main
   dependencies:
     cairo: '>=1.16.0,<2.0a0'
     freetype: '>=2.12.1,<3.0a0'
     graphite2: ''
     icu: '>=70.1,<71.0a0'
@@ -16919,30 +17041,30 @@
   optional: false
   platform: win-64
   url: https://conda.anaconda.org/conda-forge/noarch/flake8-black-0.3.6-pyhd8ed1ab_0.conda
   version: 0.3.6
 - category: main
   dependencies:
     gettext: '>=0.21.1,<1.0a0'
-    gstreamer: 1.22.4 hb4038d2_0
+    gstreamer: 1.22.4 hb4038d2_1
     libglib: '>=2.76.3,<3.0a0'
     libogg: '>=1.3.4,<1.4.0a0'
     libvorbis: '>=1.3.7,<1.4.0a0'
     libzlib: '>=1.2.13,<1.3.0a0'
     ucrt: '>=10.0.20348.0'
     vc: '>=14.2,<15'
     vc14_runtime: '>=14.29.30139'
   hash:
-    md5: 2c402e044af28ad8eccf03031c5c34c4
-    sha256: e173661c30f46d2baac980320cc53ce5f86c2d48994d895d39cdec7af825b878
+    md5: ce797dd3d60901f6260e84e84674c829
+    sha256: 796b63de19fa87c76583e0253e02796937d635d98701976390494589b5109d54
   manager: conda
   name: gst-plugins-base
   optional: false
   platform: win-64
-  url: https://conda.anaconda.org/conda-forge/win-64/gst-plugins-base-1.22.4-h001b923_0.conda
+  url: https://conda.anaconda.org/conda-forge/win-64/gst-plugins-base-1.22.4-h001b923_1.conda
   version: 1.22.4
 - category: main
   dependencies:
     importlib_metadata: '>=4.8.3'
     jupyter_core: '>=4.12,!=5.0.*'
     python: '>=3.8'
     python-dateutil: '>=2.8.2'
@@ -16986,22 +17108,22 @@
   dependencies:
     jsonschema: '>=2.6'
     jupyter_core: ''
     python: '>=3.8'
     python-fastjsonschema: ''
     traitlets: '>=5.1'
   hash:
-    md5: f525a01528c3eba1d381a232a6971c6a
-    sha256: 3c6be17e84dc71db605a9e088fa7af7d47edab45d15da8e2a2ab3f29ec5ec081
+    md5: 3ec35d84fc1775215061517eb4660693
+    sha256: d8b1ad3c219b39e5e325785606853ff1cd334769228490ac977b85aa95e94ba0
   manager: conda
   name: nbformat
   optional: false
   platform: win-64
-  url: https://conda.anaconda.org/conda-forge/noarch/nbformat-5.9.0-pyhd8ed1ab_0.conda
-  version: 5.9.0
+  url: https://conda.anaconda.org/conda-forge/noarch/nbformat-5.9.1-pyhd8ed1ab_0.conda
+  version: 5.9.1
 - category: main
   dependencies:
     cairo: '>=1.16.0,<2.0a0'
     fontconfig: '>=2.14.2,<3.0a0'
     fonts-conda-ecosystem: ''
     freetype: '>=2.12.1,<3.0a0'
     fribidi: '>=1.0.10,<2.0a0'
@@ -17180,22 +17302,22 @@
     liblapack: '>=3.9.0,<4.0a0'
     python: '>=3.10,<3.11.0a0'
     python_abi: 3.10.* *_cp310
     ucrt: '>=10.0.20348.0'
     vc: '>=14.2,<15'
     vc14_runtime: '>=14.29.30139'
   hash:
-    md5: 63be5dd380067c6db32243e6ca56e8e8
-    sha256: 2acd83d05b9095927dd7b147ac14140f13a97b45bdac1762d97f2009b2dfda77
+    md5: 922f75b8698c5b9909bf03c658898117
+    sha256: 25e07d23dd78641537082fd9b0c4183784fcc1d84c65f207d6e2e7ede7702c8f
   manager: conda
   name: numpy
   optional: false
   platform: win-64
-  url: https://conda.anaconda.org/conda-forge/win-64/numpy-1.25.0-py310hd02465a_0.conda
-  version: 1.25.0
+  url: https://conda.anaconda.org/conda-forge/win-64/numpy-1.25.1-py310hd02465a_0.conda
+  version: 1.25.1
 - category: main
   dependencies:
     gst-plugins-base: '>=1.22.0,<1.23.0a0'
     gstreamer: '>=1.22.0,<1.23.0a0'
     icu: '>=70.1,<71.0a0'
     jpeg: '>=9e,<10a'
     krb5: '>=1.20.1,<1.21.0a0'
@@ -17278,22 +17400,22 @@
     python: '>=3.6'
     pyu2f: '>=0.1.5'
     requests: '>=2.20.0,<3.0.0dev'
     rsa: '>=3.1.4,<5'
     six: '>=1.9.0'
     urllib3: <2.0
   hash:
-    md5: 8c5dd8609d314721d990c1d1fd607f81
-    sha256: 6b097ca9b31961d6a983f81dc295012e9c99c4c1a5a83a93ab2fcc6528af428f
+    md5: 5583192796d1ebcf39b1e3e0958aa259
+    sha256: 1a75b167cb01f533c01716bc663d4859a0d55d47dd96eebb39b5aa4b51205b44
   manager: conda
   name: google-auth
   optional: false
   platform: win-64
-  url: https://conda.anaconda.org/conda-forge/noarch/google-auth-2.21.0-pyh1a96a4e_0.conda
-  version: 2.21.0
+  url: https://conda.anaconda.org/conda-forge/noarch/google-auth-2.22.0-pyh1a96a4e_0.conda
+  version: 2.22.0
 - category: main
   dependencies:
     cairo: '>=1.16.0,<2.0a0'
     expat: '>=2.5.0,<3.0a0'
     getopt-win32: '>=0.1,<0.2.0a0'
     gts: '>=0.7.6,<0.8.0a0'
     libgd: '>=2.3.3,<2.4.0a0'
@@ -17369,26 +17491,41 @@
     markupsafe: '>=2.0'
     mistune: '>=2.0.3,<4'
     nbclient: '>=0.5.0'
     nbformat: '>=5.1'
     packaging: ''
     pandocfilters: '>=1.4.1'
     pygments: '>=2.4.1'
-    python: '>=3.7'
+    python: '>=3.8'
     tinycss2: ''
     traitlets: '>=5.0'
   hash:
-    md5: 879782bde4bbdb4c7b5d4054504a20d5
-    sha256: cebfc8c620bdc950e92f72562d281fc57d696497e30bef5bc9e517be757b1c2f
+    md5: 32dde1678bb003c90d4bc0c2dbd21814
+    sha256: 76ad7689d35fe031459c422f142c9d8e7a02f6922049b7a0183fc70aaef02f0a
   manager: conda
   name: nbconvert-core
   optional: false
   platform: win-64
-  url: https://conda.anaconda.org/conda-forge/noarch/nbconvert-core-7.6.0-pyhd8ed1ab_0.conda
-  version: 7.6.0
+  url: https://conda.anaconda.org/conda-forge/noarch/nbconvert-core-7.7.1-pyhd8ed1ab_1.conda
+  version: 7.7.1
+- category: main
+  dependencies:
+    numpy: '>=1.19'
+    packaging: '>=17'
+    python: '>=3.10,<3.11.0a0'
+    python_abi: 3.10.* *_cp310
+  hash:
+    md5: 9d814866ce7bef15844c53bf669a77d7
+    sha256: b298faffb20f17ae8adbed2fcbe3b5cdbd9a5243a85d77816f7e467f92902714
+  manager: conda
+  name: nibabel
+  optional: false
+  platform: win-64
+  url: https://conda.anaconda.org/conda-forge/win-64/nibabel-5.1.0-py310h5588dad_2.conda
+  version: 5.1.0
 - category: main
   dependencies:
     numpy: '>=1.21.6,<2.0a0'
     python: '>=3.10,<3.11.0a0'
     python-dateutil: '>=2.8.1'
     python_abi: 3.10.* *_cp310
     pytz: '>=2020.1'
@@ -17663,30 +17800,30 @@
     cycler: '>=0.10'
     fonttools: '>=4.22.0'
     freetype: '>=2.12.1,<3.0a0'
     kiwisolver: '>=1.0.1'
     numpy: '>=1.21.6,<2.0a0'
     packaging: '>=20.0'
     pillow: '>=6.2.0'
-    pyparsing: '>=2.3.1'
+    pyparsing: '>=2.3.1,<3.1'
     python: '>=3.10,<3.11.0a0'
     python-dateutil: '>=2.7'
     python_abi: 3.10.* *_cp310
     ucrt: '>=10.0.20348.0'
     vc: '>=14.2,<15'
-    vs2015_runtime: '>=14.29.30139'
+    vc14_runtime: '>=14.29.30139'
   hash:
-    md5: d8c42a72d04ad1b93ba7269e9949738e
-    sha256: 61975c0453d6e624c110cfec008eac14fb3fa268466a01f4257c6f280006c2fa
+    md5: f485fd7d59c2719f79aa4323caa5f1e3
+    sha256: 8a42826b6b9ca21817a5c100cbe5a85c62dac7f39284531d314e7836cd9ad939
   manager: conda
   name: matplotlib-base
   optional: false
   platform: win-64
-  url: https://conda.anaconda.org/conda-forge/win-64/matplotlib-base-3.7.1-py310h51140c5_0.conda
-  version: 3.7.1
+  url: https://conda.anaconda.org/conda-forge/win-64/matplotlib-base-3.7.2-py310h51140c5_0.conda
+  version: 3.7.2
 - category: main
   dependencies:
     docutils: '>=0.15,<0.20'
     jinja2: ''
     markdown-it-py: '>=1.0.0,<3.0.0'
     mdit-py-plugins: '>=0.3.1,<1'
     python: '>=3.7'
@@ -17700,26 +17837,26 @@
   name: myst-parser
   optional: false
   platform: win-64
   url: https://conda.anaconda.org/conda-forge/noarch/myst-parser-0.18.1-pyhd8ed1ab_0.tar.bz2
   version: 0.18.1
 - category: main
   dependencies:
-    nbconvert-core: 7.6.0 pyhd8ed1ab_0
+    nbconvert-core: 7.7.1 pyhd8ed1ab_1
     pandoc: ''
-    python: '>=3.7'
+    python: '>=3.8'
   hash:
-    md5: e8172ca42f2869bb90185c9356899e81
-    sha256: 07204ee7a7f429aa30c78897629c79859a60ef77fd1c2b9d9a1ad084c144a84f
+    md5: 796b056965d7146bcac082fa2a83943d
+    sha256: b5b2823e7951a5ba41b1020b7cce109fec7f2ebe540234bf8a17c54615c2f679
   manager: conda
   name: nbconvert-pandoc
   optional: false
   platform: win-64
-  url: https://conda.anaconda.org/conda-forge/noarch/nbconvert-pandoc-7.6.0-pyhd8ed1ab_0.conda
-  version: 7.6.0
+  url: https://conda.anaconda.org/conda-forge/noarch/nbconvert-pandoc-7.7.1-pyhd8ed1ab_1.conda
+  version: 7.7.1
 - category: main
   dependencies:
     accessible-pygments: ''
     babel: ''
     beautifulsoup4: ''
     docutils: '!=0.17.0'
     packaging: ''
@@ -17956,28 +18093,28 @@
   name: sphinxcontrib-jquery
   optional: false
   platform: win-64
   url: https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-jquery-4.1-pyhd8ed1ab_0.conda
   version: '4.1'
 - category: main
   dependencies:
-    matplotlib-base: '>=3.7.1,<3.7.2.0a0'
+    matplotlib-base: '>=3.7.2,<3.7.3.0a0'
     pyqt: '>=5.10'
     python: '>=3.10,<3.11.0a0'
     python_abi: 3.10.* *_cp310
     tornado: '>=5'
   hash:
-    md5: edfb6c85499499b014a09b8136e0fdbb
-    sha256: 697b9691c35244754ef8f67799c0c70ae4dd475a981eded17d0e5a22ff4b7971
+    md5: 5059435ea4238f449ace9c04387433bd
+    sha256: 5ff1cfee7bd663662c5152849c5611b33548dc25659559a6d30b756c9134bf75
   manager: conda
   name: matplotlib
   optional: false
   platform: win-64
-  url: https://conda.anaconda.org/conda-forge/win-64/matplotlib-3.7.1-py310h5588dad_0.conda
-  version: 3.7.1
+  url: https://conda.anaconda.org/conda-forge/win-64/matplotlib-3.7.2-py310h5588dad_0.conda
+  version: 3.7.2
 - category: main
   dependencies:
     importlib-metadata: ''
     ipykernel: ''
     ipython: ''
     jupyter-cache: '>=0.5.0,<0.7.0'
     myst-parser: '>=0.18.0,<0.19.0'
@@ -17994,26 +18131,26 @@
   name: myst-nb
   optional: false
   platform: win-64
   url: https://conda.anaconda.org/conda-forge/noarch/myst-nb-0.17.2-pyhd8ed1ab_0.conda
   version: 0.17.2
 - category: main
   dependencies:
-    nbconvert-core: 7.6.0 pyhd8ed1ab_0
-    nbconvert-pandoc: 7.6.0 pyhd8ed1ab_0
-    python: '>=3.7'
+    nbconvert-core: 7.7.1 pyhd8ed1ab_1
+    nbconvert-pandoc: 7.7.1 pyhd8ed1ab_1
+    python: '>=3.8'
   hash:
-    md5: 59976ee8df1c6f82c4aa94b5fd6b745e
-    sha256: c4fa59b7a23456c7488863b9521bfca2a62ed5061150402b7f66c6c8b3b332ea
+    md5: 95d9d1523df069792cd059f412be0d6e
+    sha256: c49a87861db316b322f919825820bc7193cbfa8a4a8b21b5ffe16a133644d400
   manager: conda
   name: nbconvert
   optional: false
   platform: win-64
-  url: https://conda.anaconda.org/conda-forge/noarch/nbconvert-7.6.0-pyhd8ed1ab_0.conda
-  version: 7.6.0
+  url: https://conda.anaconda.org/conda-forge/noarch/nbconvert-7.7.1-pyhd8ed1ab_1.conda
+  version: 7.7.1
 - category: main
   dependencies:
     jupyter_server: '>=1.8,<3'
     python: '>=3.7'
   hash:
     md5: 67e0fe74c156267d9159e9133df7fd37
     sha256: f028d7ad1f2175cde307db08b60d07e371b9d6f035cfae6c81ea94b4c408c538
```

### Comparing `hf-deepali-0.3.2/conda/environment.devenv.yml` & `hf-deepali-0.4.0/conda/environment.devenv.yml`

 * *Files 12% similar despite different names*

```diff
@@ -29,22 +29,23 @@
   - sphinx =4.5.0
   - sphinx-autoapi =2.1
   - sphinx-notfound-page =0.8
   - sphinx_rtd_theme =1.2
   # Main libraries
   - dacite =1.8
   - deprecation =2.1
+  - nibabel =5.1
   - numpy =1.25
   - pandas =1.5
   - pytorch =2.0,!=2.0.0  # ["osx" not in get_env("PLATFORM")]
   - pytorch-cuda =11.8  # ["osx" not in get_env("PLATFORM")]
   - pytorch::pytorch =2.0,!=2.0.0  # ["osx" in get_env("PLATFORM")]
   - pyyaml =6.0
+  - ruamel.yaml =0.17
   - SimpleITK =2.2
-  - typing-extensions =4.6
   # Utility libraries
   - boto3 =1.26
   - matplotlib =3.7
   - scipy =1.10
   - tensorboard =2.13
   - vtk =9.2
   # Examples / Tutorials
```

### Comparing `hf-deepali-0.3.2/conda/environment.linux-64.lock` & `hf-deepali-0.4.0/conda/environment.linux-64.lock`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Generated by conda-lock.
 # platform: linux-64
-# input_hash: 8bbc0023a299b67380a6493155cba6c46fd177739fbaea7c67b86663b42d8354
+# input_hash: c6bd68ba63788a00937c8cd1d91bb1e5813d242d7089005156ab1a663f53aee1
 @EXPLICIT
 https://conda.anaconda.org/conda-forge/linux-64/_libgcc_mutex-0.1-conda_forge.tar.bz2#d7c89558ba9fa0495403155b64376d81
 https://conda.anaconda.org/conda-forge/linux-64/ca-certificates-2023.5.7-hbcca054_0.conda#f5c65075fc34438d5b456c7f3f5ab695
 https://conda.anaconda.org/nvidia/linux-64/cuda-cudart-11.8.89-0.tar.bz2#b68c7ef3eda01e95d5903fb508c5e440
 https://conda.anaconda.org/nvidia/linux-64/cuda-cupti-11.8.87-0.tar.bz2#2f4b4933285400137cf029fef9a7daa6
 https://conda.anaconda.org/nvidia/linux-64/cuda-nvrtc-11.8.89-0.tar.bz2#f4af75ee32661708c979630cdb8f4987
 https://conda.anaconda.org/nvidia/linux-64/cuda-nvtx-11.8.86-0.tar.bz2#1825ffc3feb608f2752073935e90bb49
@@ -35,15 +35,15 @@
 https://conda.anaconda.org/conda-forge/linux-64/libgcc-ng-13.1.0-he5830b7_0.conda#cd93f779ff018dd85c7544c015c9db3c
 https://conda.anaconda.org/conda-forge/linux-64/alsa-lib-1.2.8-h166bdaf_0.tar.bz2#be733e69048951df1e4b4b7bb8c7666f
 https://conda.anaconda.org/conda-forge/linux-64/aom-3.5.0-h27087fc_0.tar.bz2#a08150fd2298460cd1fcccf626305642
 https://conda.anaconda.org/conda-forge/linux-64/attr-2.5.1-h166bdaf_1.tar.bz2#d9c69a24ad678ffce24c6543a0176b00
 https://conda.anaconda.org/conda-forge/linux-64/bzip2-1.0.8-h7f98852_4.tar.bz2#a1fd65c7ccbf10880423d82bca54eb54
 https://conda.anaconda.org/conda-forge/linux-64/c-ares-1.19.1-hd590300_0.conda#e8c18d865be43e2fb3f7a145b6adf1f5
 https://conda.anaconda.org/conda-forge/linux-64/double-conversion-3.2.0-h27087fc_1.tar.bz2#5a7e0df95874e7ffe8b7840907058563
-https://conda.anaconda.org/conda-forge/linux-64/eigen-3.4.0-h4bd325d_0.tar.bz2#61af675be1ebd2ab75ebc70b8687b84d
+https://conda.anaconda.org/conda-forge/linux-64/eigen-3.4.1-h00ab1b0_0.conda#c2acfc9bc0d0c53f83bbf0f582cb0e7a
 https://conda.anaconda.org/conda-forge/linux-64/fftw-3.3.10-nompi_hc118613_108.conda#6fa90698000b05dfe8ce6515794fe71a
 https://conda.anaconda.org/conda-forge/linux-64/fribidi-1.0.10-h36c2ea0_0.tar.bz2#ac7bc6a654f8f41b352b38f4051135f8
 https://conda.anaconda.org/conda-forge/linux-64/gettext-0.21.1-h27087fc_0.tar.bz2#14947d8770185e5153fdd04d4673ed37
 https://conda.anaconda.org/conda-forge/linux-64/giflib-5.2.1-h0b41bf4_3.conda#96f3b11872ef6fad973eac856cd2624f
 https://conda.anaconda.org/conda-forge/linux-64/gmp-6.2.1-h58526e2_0.tar.bz2#b94cf2db16066b242ebd26db2facbd56
 https://conda.anaconda.org/conda-forge/linux-64/graphite2-1.3.13-h58526e2_1001.tar.bz2#8c54672728e8ec6aa6db90cf2806d220
 https://conda.anaconda.org/conda-forge/linux-64/gstreamer-orc-0.4.34-hd590300_0.conda#7ea223fa114cc8134b8c4d398d3e5afe
@@ -119,44 +119,44 @@
 https://conda.anaconda.org/conda-forge/linux-64/libsqlite-3.42.0-h2797004_0.conda#fdaae20a1cf7cd62130a0973190a31b7
 https://conda.anaconda.org/conda-forge/linux-64/libssh2-1.11.0-h0841786_0.conda#1f5a58e686b13bcfde88b93f547d23fe
 https://conda.anaconda.org/conda-forge/linux-64/libvorbis-1.3.7-h9c3ff4c_0.tar.bz2#309dec04b70a3cc0f1e84a4013683bc0
 https://conda.anaconda.org/conda-forge/linux-64/libxcb-1.13-h7f98852_1004.tar.bz2#b3653fdc58d03face9724f602218a904
 https://conda.anaconda.org/conda-forge/linux-64/libxml2-2.10.3-hca2bb57_4.conda#bb808b654bdc3c783deaf107a2ffb503
 https://conda.anaconda.org/conda-forge/linux-64/libzip-1.9.2-hc929e4a_1.tar.bz2#5b122b50e738c4be5c3f2899f010d7cf
 https://conda.anaconda.org/conda-forge/linux-64/mpfr-4.2.0-hb012696_0.conda#14d87bdff2cbd3b1179a29fb316ed743
-https://conda.anaconda.org/conda-forge/linux-64/mysql-common-8.0.33-hf1915f5_1.conda#b241363e3b72bae6dfbd31e9fecf7d26
+https://conda.anaconda.org/conda-forge/linux-64/mysql-common-8.0.33-hf1915f5_2.conda#a55ff0ed12efd86cf3a3dfb750adb950
 https://conda.anaconda.org/conda-forge/linux-64/p11-kit-0.24.1-hc5aa10d_0.tar.bz2#56ee94e34b71742bbdfa832c974e47a8
 https://conda.anaconda.org/conda-forge/linux-64/pcre2-10.40-hc3806b6_0.tar.bz2#69e2c796349cd9b273890bee0febfe1b
 https://conda.anaconda.org/conda-forge/linux-64/readline-8.2-h8228510_1.conda#47d31b792659ce70f470b5c82fdfb7a4
 https://conda.anaconda.org/conda-forge/linux-64/tk-8.6.12-h27826a3_0.tar.bz2#5b8c42eb62e9fc961af70bdd6a26e168
 https://conda.anaconda.org/conda-forge/linux-64/xorg-fixesproto-5.0-h7f98852_1002.tar.bz2#65ad6e1eb4aed2b0611855aff05e04f6
 https://conda.anaconda.org/conda-forge/linux-64/xorg-libsm-1.2.3-hd9c2040_1000.tar.bz2#9e856f78d5c80d5a78f61e72d1d473a3
 https://conda.anaconda.org/conda-forge/linux-64/zeromq-4.3.4-h9c3ff4c_1.tar.bz2#21743a8d2ea0c8cfbbf8fe489b0347df
 https://conda.anaconda.org/conda-forge/linux-64/zlib-1.2.13-hd590300_5.conda#68c34ec6149623be41a1933ab996a209
-https://conda.anaconda.org/conda-forge/linux-64/zstd-1.5.2-h3eb15da_6.conda#6b63daed8feeca47be78f323e793d555
+https://conda.anaconda.org/conda-forge/linux-64/zstd-1.5.2-hfc55251_7.conda#32ae18eb2a687912fc9e92a501c0a11b
 https://conda.anaconda.org/conda-forge/linux-64/brotli-bin-1.0.9-h166bdaf_9.conda#d47dee1856d9cb955b8076eeff304a5b
 https://conda.anaconda.org/nvidia/linux-64/cuda-runtime-11.8.0-0.tar.bz2#3ca379d762f8d7bd727df9e2c9b30664
 https://conda.anaconda.org/conda-forge/linux-64/freetype-2.12.1-hca18f0e_1.conda#e1232042de76d24539a436d37597eb06
 https://conda.anaconda.org/conda-forge/linux-64/gl2ps-1.4.2-h0708190_0.tar.bz2#438718bf8921ac70956d919d0e2cc487
 https://conda.anaconda.org/conda-forge/linux-64/gnutls-3.7.8-hf3e180e_0.tar.bz2#cbe8e27140d67c3f30e01cfb642a6e7c
 https://conda.anaconda.org/conda-forge/linux-64/hdf4-4.2.15-h9772cbc_5.tar.bz2#ee08782aff2ff9b3291c967fa6bc7336
 https://conda.anaconda.org/conda-forge/linux-64/krb5-1.20.1-h81ceb04_0.conda#89a41adce7106749573d883b2f657d78
 https://conda.anaconda.org/conda-forge/linux-64/libgcrypt-1.10.1-h166bdaf_0.tar.bz2#f967fc95089cd247ceed56eda31de3a9
-https://conda.anaconda.org/conda-forge/linux-64/libglib-2.76.3-hebfc3b9_0.conda#a64f11b244b2c112cd3fa1cbe9493999
-https://conda.anaconda.org/conda-forge/linux-64/libgrpc-1.56.0-h3905398_2.conda#6cf9ef21c7ef12df628bf46ad67189d3
+https://conda.anaconda.org/conda-forge/linux-64/libglib-2.76.4-hebfc3b9_0.conda#c6f951789c888f7bbd2dd6858eab69de
+https://conda.anaconda.org/conda-forge/linux-64/libgrpc-1.56.2-h3905398_0.conda#a87e780f3d9cc7cf432e47ced83a67ce
 https://conda.anaconda.org/conda-forge/linux-64/libhwloc-2.9.1-hd6dc26d_0.conda#a3ede1b8e47f993ff1fe3908b23bb307
 https://conda.anaconda.org/conda-forge/linux-64/libllvm15-15.0.7-hadd5161_1.conda#17d91085ccf5934ce652cb448d0cb65a
 https://conda.anaconda.org/conda-forge/linux-64/libsndfile-1.2.0-hb75c966_0.conda#c648d19cd9c8625898d5d370414de7c7
 https://conda.anaconda.org/conda-forge/linux-64/libtheora-1.1.1-h7f98852_1005.tar.bz2#1a7c35f56343b7e9e8db20b296c7566c
 https://conda.anaconda.org/conda-forge/linux-64/libtiff-4.4.0-h82bc61c_5.conda#e712a63a21f9db647982971dc121cdcf
 https://conda.anaconda.org/conda-forge/linux-64/libudev1-253-h0b41bf4_1.conda#bb38b19a41bb94e8a19dbfb062d499c7
 https://conda.anaconda.org/conda-forge/linux-64/libxkbcommon-1.5.0-h79f4944_1.conda#04a39cdd663f295653fc143851830563
 https://conda.anaconda.org/conda-forge/linux-64/llvm-openmp-16.0.6-h4dfa4b3_0.conda#b096c85c415519259e731d8fb719a3ef
 https://conda.anaconda.org/conda-forge/linux-64/mpc-1.3.1-hfe3b2da_0.conda#289c71e83dc0daa7d4c81f04180778ca
-https://conda.anaconda.org/conda-forge/linux-64/mysql-libs-8.0.33-hca2cd23_1.conda#a04ac37f0659929f3ba0f33c7f3d750f
+https://conda.anaconda.org/conda-forge/linux-64/mysql-libs-8.0.33-hca2cd23_2.conda#b2f09078f50b9e859aca3f0dc1cc8b7e
 https://conda.anaconda.org/conda-forge/linux-64/nss-3.89-he45b914_0.conda#2745719a58eeaab6657256a3f142f099
 https://conda.anaconda.org/conda-forge/linux-64/pandoc-3.1.3-h32600fe_0.conda#8287aeb8462e2d4b235eff788e75919d
 https://conda.anaconda.org/conda-forge/linux-64/python-3.10.12-hd12c33a_0_cpython.conda#eb6f1df105f37daedd6dca78523baa75
 https://conda.anaconda.org/conda-forge/linux-64/sqlite-3.42.0-h2c6b66d_0.conda#1192f6ec654a5bc4ee1d64bdc4a3e5cc
 https://conda.anaconda.org/conda-forge/linux-64/xcb-util-0.4.0-h516909a_0.tar.bz2#a88ab22508ba067b689dc12696157cee
 https://conda.anaconda.org/conda-forge/linux-64/xcb-util-keysyms-0.4.0-h516909a_0.tar.bz2#d04a6285315c4f03ebaf37355be272f9
 https://conda.anaconda.org/conda-forge/linux-64/xcb-util-renderutil-0.3.9-h166bdaf_0.tar.bz2#732e22f1741bccea861f5668cf7342a7
@@ -168,37 +168,37 @@
 https://conda.anaconda.org/conda-forge/noarch/attrs-21.4.0-pyhd8ed1ab_0.tar.bz2#f70280205d7044c8b8358c8de3190e5d
 https://conda.anaconda.org/conda-forge/noarch/backcall-0.2.0-pyh9f0ad1d_0.tar.bz2#6006a6d08a3fa99268a2681c7fb55213
 https://conda.anaconda.org/conda-forge/noarch/backports-1.0-pyhd8ed1ab_3.conda#54ca2e08b3220c148a1d8329c2678e02
 https://conda.anaconda.org/conda-forge/noarch/blinker-1.6.2-pyhd8ed1ab_0.conda#2fb79ec81bad9492b6d59a06b3b647a4
 https://conda.anaconda.org/conda-forge/linux-64/brotli-1.0.9-h166bdaf_9.conda#4601544b4982ba1861fa9b9c607b2c06
 https://conda.anaconda.org/conda-forge/noarch/cachetools-5.3.1-pyhd8ed1ab_0.conda#60b5eb16d9a7a5482ba37f67aa49db5b
 https://conda.anaconda.org/conda-forge/noarch/certifi-2023.5.7-pyhd8ed1ab_0.conda#5d1b71c942b8421285934dad1d891ebc
-https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-3.1.0-pyhd8ed1ab_0.conda#7fcff9f6f123696e940bda77bd4d6551
-https://conda.anaconda.org/conda-forge/noarch/click-8.1.3-unix_pyhd8ed1ab_2.tar.bz2#20e4087407c7cb04a40817114b333dbf
+https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-3.2.0-pyhd8ed1ab_0.conda#313516e9a4b08b12dfb1e1cd390a96e3
+https://conda.anaconda.org/conda-forge/noarch/click-8.1.6-unix_pyh707e725_0.conda#64dbb3b205546691a61204d1cfb208e3
 https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.6-pyhd8ed1ab_0.tar.bz2#3faab06a954c2a04039983f2c4a50d99
 https://conda.anaconda.org/conda-forge/noarch/cycler-0.11.0-pyhd8ed1ab_0.tar.bz2#a50559fad0affdbb33729a68669ca1cb
 https://conda.anaconda.org/conda-forge/noarch/dataclasses-0.8-pyhc8e2a94_3.tar.bz2#a362b2124b06aad102e2ee4581acee7d
 https://conda.anaconda.org/conda-forge/linux-64/dbus-1.13.6-h5008d03_3.tar.bz2#ecfff944ba3960ecb334b9a2663d708d
 https://conda.anaconda.org/conda-forge/linux-64/debugpy-1.6.7-py310heca2aa9_0.conda#8ffb020d2b722c962f0b4f06a304f533
 https://conda.anaconda.org/conda-forge/noarch/decorator-5.1.1-pyhd8ed1ab_0.tar.bz2#43afe5ab04e35e17ba28649471dd7364
 https://conda.anaconda.org/conda-forge/noarch/defusedxml-0.7.1-pyhd8ed1ab_0.tar.bz2#961b3a227b437d82ad7054484cfa71b2
 https://conda.anaconda.org/conda-forge/linux-64/docutils-0.17.1-py310hff52083_3.tar.bz2#785160da087cf1d70e989afbb761f01c
 https://conda.anaconda.org/conda-forge/noarch/entrypoints-0.4-pyhd8ed1ab_0.tar.bz2#3cf04868fee0a029769bd41f4b2fbf2d
 https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.1.2-pyhd8ed1ab_0.conda#de4cb3384374e1411f0454edcf546cdb
 https://conda.anaconda.org/conda-forge/noarch/executing-1.2.0-pyhd8ed1ab_0.tar.bz2#4c1bc140e2be5c8ba6e3acab99e25c50
 https://conda.anaconda.org/conda-forge/noarch/filelock-3.12.2-pyhd8ed1ab_0.conda#53522ec72e6adae42bd373ef58357230
 https://conda.anaconda.org/conda-forge/noarch/flit-core-3.9.0-pyhd8ed1ab_0.conda#e8cfceef004266b259604c3faa2a0191
 https://conda.anaconda.org/conda-forge/linux-64/fontconfig-2.14.2-h14ed4e7_0.conda#0f69b688f52ff6da70bccb7ff7001d1d
-https://conda.anaconda.org/conda-forge/linux-64/frozenlist-1.3.3-py310h5764c6d_0.tar.bz2#25e1626333f9a0646579a162e7b174ee
+https://conda.anaconda.org/conda-forge/linux-64/frozenlist-1.4.0-py310h2372a71_0.conda#e239a69f354349af1117e336dd124067
 https://conda.anaconda.org/conda-forge/noarch/fsspec-2023.6.0-pyh1a96a4e_0.conda#50ea2067ec92dfcc38b4f07992d7e235
 https://conda.anaconda.org/conda-forge/linux-64/gdk-pixbuf-2.42.8-hff1cb4f_1.tar.bz2#a61c6312192e7c9de71548a6706a21e6
-https://conda.anaconda.org/conda-forge/linux-64/glib-tools-2.76.3-hfc55251_0.conda#8951eedf3cdf94dd733c1b5eee1f4880
+https://conda.anaconda.org/conda-forge/linux-64/glib-tools-2.76.4-hfc55251_0.conda#76ac435b8668f636a39fcb155c3543fd
 https://conda.anaconda.org/conda-forge/linux-64/gmpy2-2.1.2-py310h3ec546c_1.tar.bz2#73f6fa50c32ddd985cf5fba7b890a75c
 https://conda.anaconda.org/conda-forge/linux-64/greenlet-2.0.2-py310hc6cd4ac_1.conda#934c4eb3214284125eff6dd665e9568a
-https://conda.anaconda.org/conda-forge/linux-64/grpcio-1.56.0-py310h1b8f574_2.conda#78282ea7b261ed53a615faba16532e82
+https://conda.anaconda.org/conda-forge/linux-64/grpcio-1.56.2-py310h1b8f574_0.conda#0828bcffd8123a89f688e83ba95a356b
 https://conda.anaconda.org/conda-forge/linux-64/gts-0.7.6-h977cf35_4.conda#4d8df0b0db060d33c9a702ada998a8fe
 https://conda.anaconda.org/conda-forge/noarch/idna-3.4-pyhd8ed1ab_0.tar.bz2#34272b248891bddccc64479f9a7fffed
 https://conda.anaconda.org/conda-forge/noarch/imagesize-1.4.1-pyhd8ed1ab_0.tar.bz2#7de5386c8fea29e76b303f37dde4c352
 https://conda.anaconda.org/conda-forge/noarch/iniconfig-2.0.0-pyhd8ed1ab_0.conda#f800d2da156d08e289b14e87e43c1ae5
 https://conda.anaconda.org/conda-forge/noarch/ipython_genutils-0.2.0-py_1.tar.bz2#5071c982548b3a20caf70462f04f5287
 https://conda.anaconda.org/conda-forge/noarch/jmespath-1.0.1-pyhd8ed1ab_0.tar.bz2#2cfa3e1cf3fb51bb9b17acc5b5e9ea11
 https://conda.anaconda.org/conda-forge/noarch/jupyterlab_widgets-3.0.8-pyhd8ed1ab_0.conda#2bc3ca2f7387af385dd06706b4fb2d35
@@ -227,34 +227,35 @@
 https://conda.anaconda.org/conda-forge/noarch/pandocfilters-1.5.0-pyhd8ed1ab_0.tar.bz2#457c2c8c08e54905d6954e79cb5b5db9
 https://conda.anaconda.org/conda-forge/noarch/parso-0.8.3-pyhd8ed1ab_0.tar.bz2#17a565a0c3899244e938cdf417e7b094
 https://conda.anaconda.org/conda-forge/noarch/pathspec-0.11.1-pyhd8ed1ab_0.conda#dbb80d1e8dc2dba5c8b106dc0768ad45
 https://conda.anaconda.org/conda-forge/noarch/pickleshare-0.7.5-py_1003.tar.bz2#415f0ebb6198cc2801c73438a9fb5761
 https://conda.anaconda.org/conda-forge/noarch/pkgutil-resolve-name-1.3.10-pyhd8ed1ab_0.tar.bz2#89e3c7cdde7d3aaa2aee933b604dd07f
 https://conda.anaconda.org/conda-forge/noarch/pluggy-1.2.0-pyhd8ed1ab_0.conda#7263924c642d22e311d9e59b839f1b33
 https://conda.anaconda.org/conda-forge/noarch/ply-3.11-py_1.tar.bz2#7205635cd71531943440fbfe3b6b5727
-https://conda.anaconda.org/conda-forge/noarch/prometheus_client-0.17.0-pyhd8ed1ab_0.conda#95c5be3c7cbd872509d16c216617fdab
+https://conda.anaconda.org/conda-forge/noarch/prometheus_client-0.17.1-pyhd8ed1ab_0.conda#02153b6b760bbec00cfe9e4c97993d06
 https://conda.anaconda.org/conda-forge/linux-64/psutil-5.9.5-py310h1fa729e_0.conda#b0f0a014fc04012c05f39df15fe270ce
 https://conda.anaconda.org/conda-forge/noarch/ptyprocess-0.7.0-pyhd3deb0d_0.tar.bz2#359eeb6536da0e687af562ed265ec263
 https://conda.anaconda.org/conda-forge/noarch/pure_eval-0.2.2-pyhd8ed1ab_0.tar.bz2#6784285c7e55cb7212efabc79e4c2883
 https://conda.anaconda.org/conda-forge/noarch/pyasn1-0.4.8-py_0.tar.bz2#06d04c9f8f72ac77911db942eda24fb9
 https://conda.anaconda.org/conda-forge/noarch/pycodestyle-2.10.0-pyhd8ed1ab_0.conda#89843e4cc99c6a3fe5f4c86994cc8410
 https://conda.anaconda.org/conda-forge/noarch/pycparser-2.21-pyhd8ed1ab_0.tar.bz2#076becd9e05608f8dc72757d5f3a91ff
 https://conda.anaconda.org/conda-forge/noarch/pyflakes-3.0.1-pyhd8ed1ab_0.conda#44b7d77d96560c93e0e11437a3c35254
 https://conda.anaconda.org/conda-forge/noarch/pygments-2.15.1-pyhd8ed1ab_0.conda#d316679235612869eba305aa7d41d9bf
-https://conda.anaconda.org/conda-forge/noarch/pyjwt-2.7.0-pyhd8ed1ab_0.conda#99e28be5a278e2319834d7dc99e7bfdd
-https://conda.anaconda.org/conda-forge/noarch/pyparsing-3.1.0-pyhd8ed1ab_0.conda#d3ed087d1f7f8f5590e8e87b57a8ce64
+https://conda.anaconda.org/conda-forge/noarch/pyjwt-2.8.0-pyhd8ed1ab_0.conda#912c0194f898fdb783021fd25f913c31
+https://conda.anaconda.org/conda-forge/noarch/pyparsing-3.0.9-pyhd8ed1ab_0.tar.bz2#e8fbc1b54b25f4b08281467bc13b70cc
 https://conda.anaconda.org/conda-forge/linux-64/pyrsistent-0.19.3-py310h1fa729e_0.conda#f732bec05ecc2e302a868d971ae484e0
 https://conda.anaconda.org/conda-forge/noarch/pysocks-1.7.1-pyha2e5f31_6.tar.bz2#2a7de29fb590ca14b5243c4c812c8025
 https://conda.anaconda.org/conda-forge/noarch/python-fastjsonschema-2.17.1-pyhd8ed1ab_0.conda#dd4f393d857e9283eef2442234bd05e3
 https://conda.anaconda.org/conda-forge/noarch/python-json-logger-2.0.7-pyhd8ed1ab_0.conda#a61bf9ec79426938ff785eb69dbb1960
 https://conda.anaconda.org/pytorch/linux-64/pytorch-cuda-11.8-h7e8668a_5.tar.bz2#48e990086eb245cce92f09b45a34651e
 https://conda.anaconda.org/conda-forge/noarch/pytz-2023.3-pyhd8ed1ab_0.conda#d3076b483092a435832603243567bc31
 https://conda.anaconda.org/conda-forge/linux-64/pyyaml-6.0-py310h5764c6d_5.tar.bz2#9e68d2ff6d98737c855b65f48dd3c597
 https://conda.anaconda.org/conda-forge/linux-64/pyzmq-25.1.0-py310h5bbb5d0_0.conda#58017b4bb8fec6088a8b9ae44744ce4b
 https://conda.anaconda.org/conda-forge/noarch/rfc3986-validator-0.1.1-pyh9f0ad1d_0.tar.bz2#912a71cc01012ee38e6b90ddd561e36f
+https://conda.anaconda.org/conda-forge/linux-64/ruamel.yaml.clib-0.2.7-py310h1fa729e_1.conda#2f9b517412af46255cef5e53a22c264e
 https://conda.anaconda.org/conda-forge/noarch/send2trash-1.8.2-pyh41d4057_0.conda#ada5a17adcd10be4fc7e37e4166ba0e2
 https://conda.anaconda.org/conda-forge/noarch/setuptools-67.7.2-pyhd8ed1ab_0.conda#3b68bc43ec6baa48f7354a446267eefe
 https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2#e5f25f8dbc060e9a8d912e432202afc2
 https://conda.anaconda.org/conda-forge/noarch/sniffio-1.3.0-pyhd8ed1ab_0.tar.bz2#dd6cbc539e74cb1f430efbd4575b9303
 https://conda.anaconda.org/conda-forge/noarch/snowballstemmer-2.2.0-pyhd8ed1ab_0.tar.bz2#4d22a9315e78c6827f806065957d566e
 https://conda.anaconda.org/conda-forge/noarch/soupsieve-2.3.2.post1-pyhd8ed1ab_0.tar.bz2#146f4541d643d48fc8a75cacf69f03ae
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-applehelp-1.0.4-pyhd8ed1ab_0.conda#5a31a7d564f551d0e6dff52fd8cb5b16
@@ -267,51 +268,51 @@
 https://conda.anaconda.org/conda-forge/linux-64/tbb-2021.9.0-hf52228f_0.conda#f495e42d3d2020b025705625edf35490
 https://conda.anaconda.org/conda-forge/linux-64/tensorboard-data-server-0.7.0-py310h34c0648_0.conda#350fb40a1b4820cf02f546dfe6764fe9
 https://conda.anaconda.org/conda-forge/noarch/toml-0.10.2-pyhd8ed1ab_0.tar.bz2#f832c45a477c78bebd107098db465095
 https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2#5844808ffab9ebdb694585b50ba02a96
 https://conda.anaconda.org/conda-forge/linux-64/tornado-6.3.2-py310h2372a71_0.conda#1c510e74c87dc9b8fe1f7f9e8dbcef96
 https://conda.anaconda.org/conda-forge/noarch/traitlets-5.9.0-pyhd8ed1ab_0.conda#d0b4f5c87cd35ac3fb3d47b223263a64
 https://conda.anaconda.org/conda-forge/linux-64/typed-ast-1.5.5-py310h2372a71_0.conda#48d1b46a82b8b4fb6057711dd213977f
-https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.6.3-pyha770c72_0.conda#4a3014a4d107d15475d106b751c4e352
+https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.7.1-pyha770c72_0.conda#c39d6a09fe819de4951c2642629d9115
 https://conda.anaconda.org/conda-forge/noarch/typing_utils-0.1.0-pyhd8ed1ab_0.tar.bz2#eb67e3cace64c66233e2d35949e20f92
 https://conda.anaconda.org/conda-forge/noarch/uc-micro-py-1.0.1-pyhd8ed1ab_0.tar.bz2#3ddf6684d9b274a12c94e509ca45656c
 https://conda.anaconda.org/conda-forge/linux-64/unicodedata2-15.0.0-py310h5764c6d_0.tar.bz2#e972c5a1f472561cf4a91962cb01f4b4
 https://conda.anaconda.org/conda-forge/noarch/unidecode-1.3.6-pyhd8ed1ab_0.tar.bz2#e8f24401b17802df5f82f66a88cee29e
 https://conda.anaconda.org/conda-forge/noarch/webencodings-0.5.1-py_1.tar.bz2#3563be4c5611a44210d9ba0c16113136
 https://conda.anaconda.org/conda-forge/noarch/websocket-client-1.6.1-pyhd8ed1ab_0.conda#c34d9325a609381a0b0e8a5b4f325147
-https://conda.anaconda.org/conda-forge/noarch/wheel-0.40.0-pyhd8ed1ab_0.conda#49bb0d9e60ce1db25e151780331bb5f3
+https://conda.anaconda.org/conda-forge/noarch/wheel-0.40.0-pyhd8ed1ab_1.conda#c95fac682453aeffa12db7ae5a721bec
 https://conda.anaconda.org/conda-forge/noarch/widgetsnbextension-4.0.8-pyhd8ed1ab_0.conda#2e9ebddf0b93d0fb203d0906b8052c4f
 https://conda.anaconda.org/conda-forge/linux-64/wrapt-1.15.0-py310h1fa729e_0.conda#cbfdcc9c243ac7f080cf60833b482f97
 https://conda.anaconda.org/conda-forge/linux-64/xcb-util-image-0.4.0-h166bdaf_0.tar.bz2#c9b568bd804cb2903c6be6f5f68182e4
 https://conda.anaconda.org/conda-forge/linux-64/xorg-libxext-1.3.4-h0b41bf4_2.conda#82b6df12252e6f32402b96dacc656fec
 https://conda.anaconda.org/conda-forge/linux-64/xorg-libxfixes-5.0.3-h7f98852_1004.tar.bz2#e9a21aa4d5e3e5f1aed71e8cefd46b6a
 https://conda.anaconda.org/conda-forge/linux-64/xorg-libxrender-0.9.10-h7f98852_1003.tar.bz2#f59c1242cc1dd93e72c2ee2b360979eb
 https://conda.anaconda.org/conda-forge/linux-64/xorg-libxt-1.3.0-hd590300_0.conda#ab2044e8d87dda9f74652e8e084a5569
-https://conda.anaconda.org/conda-forge/noarch/zipp-3.15.0-pyhd8ed1ab_0.conda#13018819ca8f5b7cc675a8faf1f5fedf
+https://conda.anaconda.org/conda-forge/noarch/zipp-3.16.2-pyhd8ed1ab_0.conda#2da0451b54c4563c32490cb1b7cf68a1
 https://conda.anaconda.org/conda-forge/noarch/accessible-pygments-0.0.4-pyhd8ed1ab_0.conda#46a2e6e3dfa718ce3492018d5a110dd6
 https://conda.anaconda.org/conda-forge/noarch/aiosignal-1.3.1-pyhd8ed1ab_0.tar.bz2#d1e1eb7e21a9e2c74279d87dafb68156
-https://conda.anaconda.org/conda-forge/noarch/anyio-3.7.0-pyhd8ed1ab_1.conda#2b35a85d654a47aac8f34c1bb6de7142
+https://conda.anaconda.org/conda-forge/noarch/anyio-3.7.1-pyhd8ed1ab_0.conda#7b517e7a6f0790337906c055aa97ca49
 https://conda.anaconda.org/conda-forge/noarch/asttokens-2.2.1-pyhd8ed1ab_0.conda#bf7f54dd0f25c3f06ecb82a07341841a
 https://conda.anaconda.org/conda-forge/noarch/babel-2.12.1-pyhd8ed1ab_1.conda#ac432e732804a81ddcf29c92ead57cde
 https://conda.anaconda.org/conda-forge/noarch/backports.functools_lru_cache-1.6.5-pyhd8ed1ab_0.conda#6b1b907661838a75d067a22f87996b2e
 https://conda.anaconda.org/conda-forge/noarch/beautifulsoup4-4.12.2-pyha770c72_0.conda#a362ff7d976217f8fa78c0f1c4f59717
 https://conda.anaconda.org/conda-forge/noarch/bleach-6.0.0-pyhd8ed1ab_0.conda#d48b143d01385872a88ef8417e96c30e
 https://conda.anaconda.org/conda-forge/linux-64/cairo-1.16.0-ha61ee94_1014.tar.bz2#d1a88f3ed5b52e1024b80d4bcd26a7a0
 https://conda.anaconda.org/conda-forge/linux-64/cffi-1.15.1-py310h255011f_3.conda#800596144bb613cd7ac58b80900ce835
 https://conda.anaconda.org/conda-forge/noarch/comm-0.1.3-pyhd8ed1ab_0.conda#168ae0f82cdf7505048e81054c7354e4
 https://conda.anaconda.org/conda-forge/linux-64/curl-8.1.2-h409715c_0.conda#9f88cfb15b7d08b25880b138f91e0eb4
 https://conda.anaconda.org/conda-forge/noarch/dacite-1.8.0-pyhd8ed1ab_0.conda#3696792ba70ab3374320fe6041a82286
 https://conda.anaconda.org/conda-forge/noarch/deprecation-2.1.0-pyh9f0ad1d_0.tar.bz2#7b6747d7cc2076341029cff659669e8b
 https://conda.anaconda.org/conda-forge/noarch/flake8-6.0.0-pyhd8ed1ab_0.conda#e9345ba05d71742412b8aa6992ad9457
-https://conda.anaconda.org/conda-forge/linux-64/fonttools-4.40.0-py310h2372a71_0.conda#d3d83b419c81ac718a9221442707882b
+https://conda.anaconda.org/conda-forge/linux-64/fonttools-4.41.0-py310h2372a71_0.conda#606aea800172f81896b21cabc5575206
 https://conda.anaconda.org/conda-forge/linux-64/glew-2.1.0-h9c3ff4c_2.tar.bz2#fb05eb5c47590b247658243d27fc32f1
-https://conda.anaconda.org/conda-forge/linux-64/glib-2.76.3-hfc55251_0.conda#950e02f5665f5f4ff0437a6acba58798
+https://conda.anaconda.org/conda-forge/linux-64/glib-2.76.4-hfc55251_0.conda#dbcec5fd9c6c8be24b23575048755a59
 https://conda.anaconda.org/conda-forge/linux-64/hdf5-1.12.2-nompi_h4df4325_101.conda#162a25904af6586b234b2dd52ee99c61
-https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-6.7.0-pyha770c72_0.conda#ba3786c6846e46038fe60c785d46dc81
-https://conda.anaconda.org/conda-forge/noarch/importlib_resources-5.12.0-pyhd8ed1ab_0.conda#e5fd2260a231ee63b6969f4801082f2b
+https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-6.8.0-pyha770c72_0.conda#4e9f59a060c3be52bc4ddc46ee9b6946
+https://conda.anaconda.org/conda-forge/noarch/importlib_resources-6.0.0-pyhd8ed1ab_1.conda#a08b6be5bf18b9d2a927d3457750f82e
 https://conda.anaconda.org/conda-forge/noarch/jedi-0.18.2-pyhd8ed1ab_0.conda#b5e695ef9c3f0d27d6cd96bf5adc9e07
 https://conda.anaconda.org/conda-forge/noarch/jinja2-3.1.2-pyhd8ed1ab_1.tar.bz2#c8490ed5c70966d232fdd389d0dbed37
 https://conda.anaconda.org/conda-forge/noarch/jupyterlab_pygments-0.2.2-pyhd8ed1ab_0.tar.bz2#243f63592c8e449f40cd42eb5cf32f40
 https://conda.anaconda.org/conda-forge/noarch/latexcodec-2.0.1-pyh9f0ad1d_0.tar.bz2#8d67904973263afd2985ba56aa2d6bb4
 https://conda.anaconda.org/conda-forge/linux-64/libclang-15.0.7-default_h7634d5b_2.conda#1a4fe5162abe4a19b5a9dedf158a0ff9
 https://conda.anaconda.org/conda-forge/linux-64/libgd-2.3.3-h18fbbfe_3.tar.bz2#ea9758cf553476ddf75c789fdd239dc5
 https://conda.anaconda.org/conda-forge/linux-64/libva-2.18.0-h0b41bf4_0.conda#56e049224de34bbe0478aad422227942
@@ -331,51 +332,52 @@
 https://conda.anaconda.org/conda-forge/noarch/pyproject_hooks-1.0.0-pyhd8ed1ab_0.conda#21de50391d584eb7f4441b9de1ad773f
 https://conda.anaconda.org/conda-forge/noarch/pytest-7.3.2-pyhd8ed1ab_1.conda#f2465696f4396245eca4613f6e924796
 https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.8.2-pyhd8ed1ab_0.tar.bz2#dd999d1cc9f79e67dbb855c8924c7984
 https://conda.anaconda.org/conda-forge/noarch/pyu2f-0.1.5-pyhd8ed1ab_0.tar.bz2#caabbeaa83928d0c3e3949261daa18eb
 https://conda.anaconda.org/conda-forge/noarch/qtpy-2.3.1-pyhd8ed1ab_0.conda#10812eca3ec4ebaf3749e1960c208d43
 https://conda.anaconda.org/conda-forge/noarch/rfc3339-validator-0.1.4-pyhd8ed1ab_0.tar.bz2#fed45fc5ea0813240707998abe49f520
 https://conda.anaconda.org/conda-forge/noarch/rsa-4.9-pyhd8ed1ab_0.tar.bz2#03bf410858b2cefc267316408a77c436
+https://conda.anaconda.org/conda-forge/linux-64/ruamel.yaml-0.17.32-py310h2372a71_0.conda#9a03abf74d5069bda767c1bce7a41e0b
 https://conda.anaconda.org/conda-forge/linux-64/sip-6.7.9-py310hc6cd4ac_0.conda#a3217e1bff09702dfdfcb536825fc12d
 https://conda.anaconda.org/conda-forge/noarch/sympy-1.12-pypyh9d50eac_103.conda#2f7d6347d7acf6edf1ac7f2189f44c8f
 https://conda.anaconda.org/conda-forge/linux-64/tbb-devel-2021.9.0-hf52228f_0.conda#b44ecd26bd0318a9eef65705483c70bc
 https://conda.anaconda.org/conda-forge/noarch/terminado-0.17.1-pyh41d4057_0.conda#3788984d535770cad699efaeb6cb3037
 https://conda.anaconda.org/conda-forge/noarch/tinycss2-1.2.1-pyhd8ed1ab_0.tar.bz2#7234c9eefff659501cd2fe0d2ede4d48
 https://conda.anaconda.org/conda-forge/noarch/tqdm-4.65.0-pyhd8ed1ab_1.conda#ed792aff3acb977d09c7013358097f83
-https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.6.3-hd8ed1ab_0.conda#3876f650ed7d0f95d70fa4b647621909
+https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.7.1-hd8ed1ab_0.conda#f96688577f1faa58096d06a45136afa2
 https://conda.anaconda.org/conda-forge/noarch/werkzeug-2.3.6-pyhd8ed1ab_0.conda#55fbbb3e67185820ee2007395bfe0073
 https://conda.anaconda.org/conda-forge/linux-64/yarl-1.9.2-py310h2372a71_0.conda#73deaf595eb21f3e76a02ba1ae2edee6
 https://conda.anaconda.org/conda-forge/linux-64/argon2-cffi-bindings-21.2.0-py310h5764c6d_3.tar.bz2#12f70cd23e4ea88f913dba50b0f0aba0
-https://conda.anaconda.org/conda-forge/linux-64/astroid-2.15.5-py310hff52083_0.conda#1ed3ebb3837ac50a6bf762b44cf2315c
+https://conda.anaconda.org/conda-forge/linux-64/astroid-2.15.6-py310hff52083_0.conda#8ad02555d6ecdb8fd5f1963690c59699
 https://conda.anaconda.org/conda-forge/noarch/async-timeout-4.0.2-pyhd8ed1ab_0.tar.bz2#25e79f9a1133556671becbd65a170c78
 https://conda.anaconda.org/conda-forge/linux-64/brotlipy-0.7.0-py310h5764c6d_1005.tar.bz2#87669c3468dff637bbd0363bc0f895cf
-https://conda.anaconda.org/conda-forge/linux-64/cryptography-41.0.1-py310h75e40e8_0.conda#bd5501a8ae0df5ef36b9ed03035ebe3a
+https://conda.anaconda.org/conda-forge/linux-64/cryptography-41.0.2-py310h75e40e8_0.conda#3e80a669e7a1890ebb91370f2e818129
 https://conda.anaconda.org/conda-forge/linux-64/ffmpeg-5.1.2-gpl_h8dda1f0_106.conda#6845420373a9e260942bfbc5c786a4bb
 https://conda.anaconda.org/conda-forge/noarch/ghp-import-2.1.0-pyhd8ed1ab_0.tar.bz2#6d8d61116031a3f5b1f32e7899785866
 https://conda.anaconda.org/conda-forge/linux-64/gstreamer-1.22.0-h25f0c4b_2.conda#461541cb1b387c2a28ab6217f3d38502
 https://conda.anaconda.org/conda-forge/linux-64/harfbuzz-6.0.0-h8e241bc_0.conda#448fe40d2fed88ccf4d9ded37cbb2b38
-https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-6.7.0-hd8ed1ab_0.conda#27a4cec373ec84d1c1aa02a1e37f8eaf
+https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-6.8.0-hd8ed1ab_0.conda#b279b07ce18058034e5b3606ba103a8b
 https://conda.anaconda.org/conda-forge/noarch/jsonschema-4.17.3-pyhd8ed1ab_0.conda#723268a468177cd44568eb8f794e0d80
 https://conda.anaconda.org/conda-forge/noarch/jupyter_server_terminals-0.4.4-pyhd8ed1ab_1.conda#7c0965e1d4a0ee1529e8eaa03a78a5b3
 https://conda.anaconda.org/conda-forge/linux-64/libblas-3.9.0-16_linux64_mkl.tar.bz2#85f61af03fd291dae33150ffe89dc09a
 https://conda.anaconda.org/conda-forge/linux-64/libitk-5.3.0-hcedbc38_0.conda#85b4afd676357f69ab154096f1977884
 https://conda.anaconda.org/conda-forge/linux-64/libnetcdf-4.8.1-nompi_h261ec11_106.tar.bz2#9b25de670ce5753a33c18b1090d1d3bf
 https://conda.anaconda.org/conda-forge/noarch/markdown-3.4.3-pyhd8ed1ab_0.conda#89ed59ad509c05db6f5f2f573d499bfe
 https://conda.anaconda.org/conda-forge/noarch/mdit-py-plugins-0.4.0-pyhd8ed1ab_0.conda#6c5358a10873a15398b6f15f60cb5e1f
 https://conda.anaconda.org/conda-forge/linux-64/mkl-devel-2022.1.0-ha770c72_916.tar.bz2#69ba49e445f87aea2cba343a71a35ca2
-https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.8.0-pyhd8ed1ab_0.conda#3e4aca765371893ad848397794600632
+https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.9.1-pyhd8ed1ab_0.conda#044e7a1e0ad42c4e67110bd078150a63
 https://conda.anaconda.org/conda-forge/linux-64/pulseaudio-daemon-16.1-ha8d29e2_3.conda#34d9d75ca896f5919c372a34e25f23ea
 https://conda.anaconda.org/conda-forge/noarch/pybtex-0.24.0-pyhd8ed1ab_2.tar.bz2#2099b86a7399c44c0c61cdb6de6915ba
 https://conda.anaconda.org/conda-forge/linux-64/pyqt5-sip-12.11.0-py310heca2aa9_3.conda#3b1946b676534472ce65181dda0b9554
 https://conda.anaconda.org/conda-forge/noarch/python-build-0.10.0-pyhd8ed1ab_1.conda#0ab47ce574f6a8bcb9f2076436e7fedb
 https://conda.anaconda.org/conda-forge/noarch/setuptools-scm-7.1.0-pyhd8ed1ab_0.conda#6613dbb3b25cc648a107f33ca9f80fc1
-https://conda.anaconda.org/conda-forge/linux-64/sqlalchemy-2.0.17-py310h2372a71_0.conda#5addfcf598875b2e4febacbc98aa2d29
+https://conda.anaconda.org/conda-forge/linux-64/sqlalchemy-2.0.19-py310h2372a71_0.conda#2460f5ca3ab3265b80ee06a1d4b5b374
 https://conda.anaconda.org/conda-forge/noarch/stack_data-0.6.2-pyhd8ed1ab_0.conda#e7df0fdd404616638df5ece6e69ba7af
 https://conda.anaconda.org/conda-forge/noarch/wcwidth-0.2.6-pyhd8ed1ab_0.conda#078979d33523cb477bd1916ce41aacc9
-https://conda.anaconda.org/conda-forge/linux-64/aiohttp-3.8.4-py310h2372a71_1.conda#05d01d95b7838f86796b18a80fd42584
+https://conda.anaconda.org/conda-forge/linux-64/aiohttp-3.8.5-py310h2372a71_0.conda#0b05c509a96d0bf4bb424fe184170795
 https://conda.anaconda.org/conda-forge/noarch/argon2-cffi-21.3.0-pyhd8ed1ab_0.tar.bz2#a0b402db58f73aaab8ee0ca1025a362e
 https://conda.anaconda.org/conda-forge/noarch/black-22.3.0-pyhd8ed1ab_0.tar.bz2#7ecbfaae9a30b73c1a6e36e4a0debc03
 https://conda.anaconda.org/conda-forge/linux-64/gst-plugins-base-1.22.0-h4243ec0_2.conda#0d0c6604c8ac4ad5e51efa7bb58da05c
 https://conda.anaconda.org/conda-forge/linux-64/jupyter_core-5.3.1-py310hff52083_0.conda#63264f5a6dd5483475968016b614f525
 https://conda.anaconda.org/conda-forge/noarch/jupyter_events-0.6.3-pyhd8ed1ab_0.conda#d98c5196ab6ffeb0c2feca2912801353
 https://conda.anaconda.org/conda-forge/linux-64/libcblas-3.9.0-16_linux64_mkl.tar.bz2#361bf757b95488de76c4f123805742d3
 https://conda.anaconda.org/conda-forge/linux-64/liblapack-3.9.0-16_linux64_mkl.tar.bz2#a2f166748917d6d6e4707841ca1f519e
@@ -387,48 +389,49 @@
 https://conda.anaconda.org/conda-forge/noarch/pyopenssl-23.2.0-pyhd8ed1ab_1.conda#34f7d568bf59d18e3fef8c405cbece21
 https://conda.anaconda.org/conda-forge/linux-64/simpleitk-2.2.1-py310h2b9ea3a_1.conda#ec09bbee37ea5d3b6022bab2e9b4d5a4
 https://conda.anaconda.org/conda-forge/noarch/flake8-black-0.3.6-pyhd8ed1ab_0.conda#61649e6e9b39ac0c7d10938025f6fe4f
 https://conda.anaconda.org/conda-forge/linux-64/gtk2-2.24.33-h90689f9_2.tar.bz2#957a0255ab58aaf394a91725d73ab422
 https://conda.anaconda.org/conda-forge/noarch/jupyter_client-8.3.0-pyhd8ed1ab_0.conda#1d018ee4ab13217e2544f795eb0a6798
 https://conda.anaconda.org/conda-forge/linux-64/liblapacke-3.9.0-16_linux64_mkl.tar.bz2#44ccc4d4dca6a8d57fa17442bc64b5a1
 https://conda.anaconda.org/conda-forge/linux-64/librsvg-2.54.4-h7abd40a_0.tar.bz2#921e53675ed5ea352f022b79abab076a
-https://conda.anaconda.org/conda-forge/noarch/nbformat-5.9.0-pyhd8ed1ab_0.conda#f525a01528c3eba1d381a232a6971c6a
-https://conda.anaconda.org/conda-forge/linux-64/numpy-1.25.0-py310ha4c1d20_0.conda#03319f78e5c9c8d90c0110e2c6ed24f6
+https://conda.anaconda.org/conda-forge/noarch/nbformat-5.9.1-pyhd8ed1ab_0.conda#3ec35d84fc1775215061517eb4660693
+https://conda.anaconda.org/conda-forge/linux-64/numpy-1.25.1-py310ha4c1d20_0.conda#3810cbf2635cb1d0edb97715d4ad74e7
 https://conda.anaconda.org/conda-forge/noarch/prompt_toolkit-3.0.39-hd8ed1ab_0.conda#4bbbe67d5df19db30f04b8e344dc9976
 https://conda.anaconda.org/conda-forge/linux-64/qt-main-5.15.8-h5d23da1_6.conda#59c73debd9405771690ddbbad6c57b69
 https://conda.anaconda.org/conda-forge/noarch/urllib3-1.26.15-pyhd8ed1ab_0.conda#27db656619a55d727eaf5a6ece3d2fd6
 https://conda.anaconda.org/conda-forge/noarch/wslink-1.11.1-pyhd8ed1ab_0.conda#0d0113b67472cea3da288838ebc80acb
 https://conda.anaconda.org/conda-forge/linux-64/blas-devel-3.9.0-16_linux64_mkl.tar.bz2#3f92c1c9e1c0e183462c5071aa02cae1
 https://conda.anaconda.org/conda-forge/noarch/botocore-1.29.165-pyhd8ed1ab_0.conda#0f30016ea54215fdb883b8978340c9b7
 https://conda.anaconda.org/conda-forge/linux-64/contourpy-1.1.0-py310hd41b1e2_0.conda#684399f9ddc0b9d6f3b6164f6107098e
 https://conda.anaconda.org/conda-forge/linux-64/graphviz-7.0.5-h2e5815a_0.conda#96bf06b24d74a5bf826485e9032c9312
 https://conda.anaconda.org/conda-forge/noarch/ipython-8.14.0-pyh41d4057_0.conda#0a0b0d8177c4a209017b356439292db8
 https://conda.anaconda.org/conda-forge/noarch/nbclient-0.7.4-pyhd8ed1ab_0.conda#f7aa15f77d29b11caa1df1eb15383c59
+https://conda.anaconda.org/conda-forge/linux-64/nibabel-5.1.0-py310hff52083_2.conda#01c0095d68f52a2ebe4154974b668bef
 https://conda.anaconda.org/conda-forge/linux-64/pandas-1.5.3-py310h9b08913_1.conda#331c9dd2560aeb308e26f821280f19d0
 https://conda.anaconda.org/conda-forge/linux-64/pyqt-5.15.7-py310hab646b1_3.conda#d049da3204bf5ecb54a852b622f2d7d2
 https://conda.anaconda.org/conda-forge/noarch/requests-2.31.0-pyhd8ed1ab_0.conda#a30144e4156cdbb236f99ebb49828f8b
 https://conda.anaconda.org/conda-forge/linux-64/vtk-9.2.5-qt_py310hc895abb_200.conda#3462cb0fb18182f4203cdb6e73434a31
 https://conda.anaconda.org/conda-forge/linux-64/blas-2.116-mkl.tar.bz2#c196a26abf6b4f132c88828ab7c2231c
-https://conda.anaconda.org/conda-forge/noarch/google-auth-2.21.0-pyh1a96a4e_0.conda#8c5dd8609d314721d990c1d1fd607f81
+https://conda.anaconda.org/conda-forge/noarch/google-auth-2.22.0-pyh1a96a4e_0.conda#5583192796d1ebcf39b1e3e0958aa259
 https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.23.3-pyh71e2992_0.conda#482f0176a89f14e10a7d15f9f1980e36
 https://conda.anaconda.org/conda-forge/noarch/jupyter-cache-0.6.1-pyhd8ed1ab_0.conda#2e360820ae68e3d28e1a5a9d2714ca5c
-https://conda.anaconda.org/conda-forge/linux-64/matplotlib-base-3.7.1-py310he60537e_0.conda#68b2dd34c69d08b05a9db5e3596fe3ee
-https://conda.anaconda.org/conda-forge/noarch/nbconvert-core-7.6.0-pyhd8ed1ab_0.conda#879782bde4bbdb4c7b5d4054504a20d5
+https://conda.anaconda.org/conda-forge/linux-64/matplotlib-base-3.7.2-py310hf38f957_0.conda#9b55c9041c5a7f80f184a2cb05ec9663
+https://conda.anaconda.org/conda-forge/noarch/nbconvert-core-7.7.1-pyhd8ed1ab_1.conda#32dde1678bb003c90d4bc0c2dbd21814
 https://conda.anaconda.org/conda-forge/noarch/pooch-1.7.0-pyha770c72_3.conda#5936894aade8240c867d292aa0d980c6
 https://conda.anaconda.org/conda-forge/noarch/requests-oauthlib-1.3.1-pyhd8ed1ab_0.tar.bz2#61b279f051eef9c89d58f4d813e75e04
 https://conda.anaconda.org/conda-forge/noarch/s3transfer-0.6.1-pyhd8ed1ab_0.conda#b19a857ac845097e9c823c9f4d35f80e
 https://conda.anaconda.org/conda-forge/noarch/sphinx-4.5.0-pyh6c4a22f_0.tar.bz2#46b38d88c4270ff9ba78a89c83c66345
 https://conda.anaconda.org/conda-forge/noarch/boto3-1.26.165-pyhd8ed1ab_0.conda#b9a6316db67d5f2c8dbac2aeb24c6803
 https://conda.anaconda.org/conda-forge/noarch/google-auth-oauthlib-1.0.0-pyhd8ed1ab_1.conda#569e62e95b01b53e4ec7d9abe83b7385
 https://conda.anaconda.org/conda-forge/noarch/ipywidgets-8.0.7-pyhd8ed1ab_0.conda#4b0f4e8fe2a303e472674eae0340bdad
 https://conda.anaconda.org/conda-forge/noarch/jupyter_console-6.6.3-pyhd8ed1ab_0.conda#7cf6f52a66f8e3cd9d8b6c231262dcab
 https://conda.anaconda.org/conda-forge/noarch/jupyter_server-2.7.0-pyhd8ed1ab_0.conda#7488cd1f4d35a2af96faa765b7e5b2f0
-https://conda.anaconda.org/conda-forge/linux-64/matplotlib-3.7.1-py310hff52083_0.conda#c2b60c44d38d32779006a15c2581f0d1
+https://conda.anaconda.org/conda-forge/linux-64/matplotlib-3.7.2-py310hff52083_0.conda#7e454b4a61754714a4a4d183641374da
 https://conda.anaconda.org/conda-forge/noarch/myst-parser-0.18.1-pyhd8ed1ab_0.tar.bz2#bcfdf5c7d8bf5c6f6be7b4c66fff2eca
-https://conda.anaconda.org/conda-forge/noarch/nbconvert-pandoc-7.6.0-pyhd8ed1ab_0.conda#e8172ca42f2869bb90185c9356899e81
+https://conda.anaconda.org/conda-forge/noarch/nbconvert-pandoc-7.7.1-pyhd8ed1ab_1.conda#796b056965d7146bcac082fa2a83943d
 https://conda.anaconda.org/conda-forge/noarch/pydata-sphinx-theme-0.13.3-pyhd8ed1ab_0.conda#07aca5f2dea315dcc16680d6891e9056
 https://conda.anaconda.org/conda-forge/noarch/qtconsole-base-5.4.3-pyha770c72_0.conda#e0f5e8a6f9ea248e5c2d23efffff08f7
 https://conda.anaconda.org/conda-forge/linux-64/scipy-1.10.1-py310ha4c1d20_3.conda#0414d57832172f3cdcf56b5f053e177d
 https://conda.anaconda.org/conda-forge/noarch/sphinx-comments-0.0.3-pyh9f0ad1d_0.tar.bz2#2ae3ce35de0c1cec45c94182694f8d1b
 https://conda.anaconda.org/conda-forge/noarch/sphinx-copybutton-0.5.2-pyhd8ed1ab_0.conda#ac832cc43adc79118cf6e23f1f9b8995
 https://conda.anaconda.org/conda-forge/noarch/sphinx-design-0.3.0-pyhd8ed1ab_0.tar.bz2#83d1a712e6d2bab6b298b1d2f42ad355
 https://conda.anaconda.org/conda-forge/noarch/sphinx-external-toc-0.3.1-pyhd8ed1ab_0.conda#561bdf7b598d38e2962c46557bd1da12
@@ -438,15 +441,15 @@
 https://conda.anaconda.org/conda-forge/noarch/sphinx-thebe-0.2.1-pyhd8ed1ab_0.conda#8a4151bde2af98c6cbc42ee12b48eb7f
 https://conda.anaconda.org/conda-forge/noarch/sphinx-togglebutton-0.3.2-pyhd8ed1ab_0.tar.bz2#382738101934261ea7931d1460e64868
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-bibtex-2.5.0-pyhd8ed1ab_0.tar.bz2#b2e5c9aece936ebf9f26abdf71ddd74b
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-dotnetdomain-0.4-py_0.tar.bz2#fb61a7369f505b4bb98e1530c3e09f9f
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-golangdomain-0.2.0.dev0-py_0.tar.bz2#d1a73c192888d08cedec232602c22f32
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-jquery-4.1-pyhd8ed1ab_0.conda#914897066d5873acfb13e75705276ad1
 https://conda.anaconda.org/conda-forge/noarch/myst-nb-0.17.2-pyhd8ed1ab_0.conda#40190b7d06f86b63d28fa78aaa39c023
-https://conda.anaconda.org/conda-forge/noarch/nbconvert-7.6.0-pyhd8ed1ab_0.conda#59976ee8df1c6f82c4aa94b5fd6b745e
+https://conda.anaconda.org/conda-forge/noarch/nbconvert-7.7.1-pyhd8ed1ab_1.conda#95d9d1523df069792cd059f412be0d6e
 https://conda.anaconda.org/conda-forge/noarch/notebook-shim-0.2.3-pyhd8ed1ab_0.conda#67e0fe74c156267d9159e9133df7fd37
 https://conda.anaconda.org/conda-forge/noarch/qtconsole-5.4.3-pyhd8ed1ab_0.conda#3777f933bec5113d5a292de10b03d0f6
 https://conda.anaconda.org/conda-forge/noarch/sphinx-autoapi-2.1.0-pyhd8ed1ab_0.conda#6cb2b182390f837ce98737e92b9461f7
 https://conda.anaconda.org/conda-forge/noarch/sphinx-book-theme-1.0.1-pyhd8ed1ab_0.conda#1ef419576de2c51b6e3a5a393eb35cda
 https://conda.anaconda.org/conda-forge/noarch/sphinx_rtd_theme-1.2.2-pyha770c72_0.conda#5ef6aaf2cfb3b656cdadb431daed6a9f
 https://conda.anaconda.org/conda-forge/noarch/tensorboard-2.13.0-pyhd8ed1ab_0.conda#321151b2405f11ec6681a9a6f30822b4
 https://conda.anaconda.org/conda-forge/noarch/jupyter-book-0.15.1-pyhd8ed1ab_0.conda#f10d556d3b3dc0aeae6aee37c412ea60
```

### Comparing `hf-deepali-0.3.2/conda/environment.linux-64.yml` & `hf-deepali-0.4.0/conda/environment.linux-64.yml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Generated by conda-lock.
 # platform: linux-64
-# input_hash: 8bbc0023a299b67380a6493155cba6c46fd177739fbaea7c67b86663b42d8354
+# input_hash: c6bd68ba63788a00937c8cd1d91bb1e5813d242d7089005156ab1a663f53aee1
 
 channels:
   - conda-forge
   - pytorch
   - nvidia
   - nodefaults
 dependencies:
@@ -41,15 +41,15 @@
   - libgcc-ng=13.1.0=he5830b7_0
   - alsa-lib=1.2.8=h166bdaf_0
   - aom=3.5.0=h27087fc_0
   - attr=2.5.1=h166bdaf_1
   - bzip2=1.0.8=h7f98852_4
   - c-ares=1.19.1=hd590300_0
   - double-conversion=3.2.0=h27087fc_1
-  - eigen=3.4.0=h4bd325d_0
+  - eigen=3.4.1=h00ab1b0_0
   - fftw=3.3.10=nompi_hc118613_108
   - fribidi=1.0.10=h36c2ea0_0
   - gettext=0.21.1=h27087fc_0
   - giflib=5.2.1=h0b41bf4_3
   - gmp=6.2.1=h58526e2_0
   - graphite2=1.3.13=h58526e2_1001
   - gstreamer-orc=0.4.34=hd590300_0
@@ -125,44 +125,44 @@
   - libsqlite=3.42.0=h2797004_0
   - libssh2=1.11.0=h0841786_0
   - libvorbis=1.3.7=h9c3ff4c_0
   - libxcb=1.13=h7f98852_1004
   - libxml2=2.10.3=hca2bb57_4
   - libzip=1.9.2=hc929e4a_1
   - mpfr=4.2.0=hb012696_0
-  - mysql-common=8.0.33=hf1915f5_1
+  - mysql-common=8.0.33=hf1915f5_2
   - p11-kit=0.24.1=hc5aa10d_0
   - pcre2=10.40=hc3806b6_0
   - readline=8.2=h8228510_1
   - tk=8.6.12=h27826a3_0
   - xorg-fixesproto=5.0=h7f98852_1002
   - xorg-libsm=1.2.3=hd9c2040_1000
   - zeromq=4.3.4=h9c3ff4c_1
   - zlib=1.2.13=hd590300_5
-  - zstd=1.5.2=h3eb15da_6
+  - zstd=1.5.2=hfc55251_7
   - brotli-bin=1.0.9=h166bdaf_9
   - cuda-runtime=11.8.0=0
   - freetype=2.12.1=hca18f0e_1
   - gl2ps=1.4.2=h0708190_0
   - gnutls=3.7.8=hf3e180e_0
   - hdf4=4.2.15=h9772cbc_5
   - krb5=1.20.1=h81ceb04_0
   - libgcrypt=1.10.1=h166bdaf_0
-  - libglib=2.76.3=hebfc3b9_0
-  - libgrpc=1.56.0=h3905398_2
+  - libglib=2.76.4=hebfc3b9_0
+  - libgrpc=1.56.2=h3905398_0
   - libhwloc=2.9.1=hd6dc26d_0
   - libllvm15=15.0.7=hadd5161_1
   - libsndfile=1.2.0=hb75c966_0
   - libtheora=1.1.1=h7f98852_1005
   - libtiff=4.4.0=h82bc61c_5
   - libudev1=253=h0b41bf4_1
   - libxkbcommon=1.5.0=h79f4944_1
   - llvm-openmp=16.0.6=h4dfa4b3_0
   - mpc=1.3.1=hfe3b2da_0
-  - mysql-libs=8.0.33=hca2cd23_1
+  - mysql-libs=8.0.33=hca2cd23_2
   - nss=3.89=he45b914_0
   - pandoc=3.1.3=h32600fe_0
   - python=3.10.12=hd12c33a_0_cpython
   - sqlite=3.42.0=h2c6b66d_0
   - xcb-util=0.4.0=h516909a_0
   - xcb-util-keysyms=0.4.0=h516909a_0
   - xcb-util-renderutil=0.3.9=h166bdaf_0
@@ -174,37 +174,37 @@
   - attrs=21.4.0=pyhd8ed1ab_0
   - backcall=0.2.0=pyh9f0ad1d_0
   - backports=1.0=pyhd8ed1ab_3
   - blinker=1.6.2=pyhd8ed1ab_0
   - brotli=1.0.9=h166bdaf_9
   - cachetools=5.3.1=pyhd8ed1ab_0
   - certifi=2023.5.7=pyhd8ed1ab_0
-  - charset-normalizer=3.1.0=pyhd8ed1ab_0
-  - click=8.1.3=unix_pyhd8ed1ab_2
+  - charset-normalizer=3.2.0=pyhd8ed1ab_0
+  - click=8.1.6=unix_pyh707e725_0
   - colorama=0.4.6=pyhd8ed1ab_0
   - cycler=0.11.0=pyhd8ed1ab_0
   - dataclasses=0.8=pyhc8e2a94_3
   - dbus=1.13.6=h5008d03_3
   - debugpy=1.6.7=py310heca2aa9_0
   - decorator=5.1.1=pyhd8ed1ab_0
   - defusedxml=0.7.1=pyhd8ed1ab_0
   - docutils=0.17.1=py310hff52083_3
   - entrypoints=0.4=pyhd8ed1ab_0
   - exceptiongroup=1.1.2=pyhd8ed1ab_0
   - executing=1.2.0=pyhd8ed1ab_0
   - filelock=3.12.2=pyhd8ed1ab_0
   - flit-core=3.9.0=pyhd8ed1ab_0
   - fontconfig=2.14.2=h14ed4e7_0
-  - frozenlist=1.3.3=py310h5764c6d_0
+  - frozenlist=1.4.0=py310h2372a71_0
   - fsspec=2023.6.0=pyh1a96a4e_0
   - gdk-pixbuf=2.42.8=hff1cb4f_1
-  - glib-tools=2.76.3=hfc55251_0
+  - glib-tools=2.76.4=hfc55251_0
   - gmpy2=2.1.2=py310h3ec546c_1
   - greenlet=2.0.2=py310hc6cd4ac_1
-  - grpcio=1.56.0=py310h1b8f574_2
+  - grpcio=1.56.2=py310h1b8f574_0
   - gts=0.7.6=h977cf35_4
   - idna=3.4=pyhd8ed1ab_0
   - imagesize=1.4.1=pyhd8ed1ab_0
   - iniconfig=2.0.0=pyhd8ed1ab_0
   - ipython_genutils=0.2.0=py_1
   - jmespath=1.0.1=pyhd8ed1ab_0
   - jupyterlab_widgets=3.0.8=pyhd8ed1ab_0
@@ -233,34 +233,35 @@
   - pandocfilters=1.5.0=pyhd8ed1ab_0
   - parso=0.8.3=pyhd8ed1ab_0
   - pathspec=0.11.1=pyhd8ed1ab_0
   - pickleshare=0.7.5=py_1003
   - pkgutil-resolve-name=1.3.10=pyhd8ed1ab_0
   - pluggy=1.2.0=pyhd8ed1ab_0
   - ply=3.11=py_1
-  - prometheus_client=0.17.0=pyhd8ed1ab_0
+  - prometheus_client=0.17.1=pyhd8ed1ab_0
   - psutil=5.9.5=py310h1fa729e_0
   - ptyprocess=0.7.0=pyhd3deb0d_0
   - pure_eval=0.2.2=pyhd8ed1ab_0
   - pyasn1=0.4.8=py_0
   - pycodestyle=2.10.0=pyhd8ed1ab_0
   - pycparser=2.21=pyhd8ed1ab_0
   - pyflakes=3.0.1=pyhd8ed1ab_0
   - pygments=2.15.1=pyhd8ed1ab_0
-  - pyjwt=2.7.0=pyhd8ed1ab_0
-  - pyparsing=3.1.0=pyhd8ed1ab_0
+  - pyjwt=2.8.0=pyhd8ed1ab_0
+  - pyparsing=3.0.9=pyhd8ed1ab_0
   - pyrsistent=0.19.3=py310h1fa729e_0
   - pysocks=1.7.1=pyha2e5f31_6
   - python-fastjsonschema=2.17.1=pyhd8ed1ab_0
   - python-json-logger=2.0.7=pyhd8ed1ab_0
   - pytorch-cuda=11.8=h7e8668a_5
   - pytz=2023.3=pyhd8ed1ab_0
   - pyyaml=6.0=py310h5764c6d_5
   - pyzmq=25.1.0=py310h5bbb5d0_0
   - rfc3986-validator=0.1.1=pyh9f0ad1d_0
+  - ruamel.yaml.clib=0.2.7=py310h1fa729e_1
   - send2trash=1.8.2=pyh41d4057_0
   - setuptools=67.7.2=pyhd8ed1ab_0
   - six=1.16.0=pyh6c4a22f_0
   - sniffio=1.3.0=pyhd8ed1ab_0
   - snowballstemmer=2.2.0=pyhd8ed1ab_0
   - soupsieve=2.3.2.post1=pyhd8ed1ab_0
   - sphinxcontrib-applehelp=1.0.4=pyhd8ed1ab_0
@@ -273,51 +274,51 @@
   - tbb=2021.9.0=hf52228f_0
   - tensorboard-data-server=0.7.0=py310h34c0648_0
   - toml=0.10.2=pyhd8ed1ab_0
   - tomli=2.0.1=pyhd8ed1ab_0
   - tornado=6.3.2=py310h2372a71_0
   - traitlets=5.9.0=pyhd8ed1ab_0
   - typed-ast=1.5.5=py310h2372a71_0
-  - typing_extensions=4.6.3=pyha770c72_0
+  - typing_extensions=4.7.1=pyha770c72_0
   - typing_utils=0.1.0=pyhd8ed1ab_0
   - uc-micro-py=1.0.1=pyhd8ed1ab_0
   - unicodedata2=15.0.0=py310h5764c6d_0
   - unidecode=1.3.6=pyhd8ed1ab_0
   - webencodings=0.5.1=py_1
   - websocket-client=1.6.1=pyhd8ed1ab_0
-  - wheel=0.40.0=pyhd8ed1ab_0
+  - wheel=0.40.0=pyhd8ed1ab_1
   - widgetsnbextension=4.0.8=pyhd8ed1ab_0
   - wrapt=1.15.0=py310h1fa729e_0
   - xcb-util-image=0.4.0=h166bdaf_0
   - xorg-libxext=1.3.4=h0b41bf4_2
   - xorg-libxfixes=5.0.3=h7f98852_1004
   - xorg-libxrender=0.9.10=h7f98852_1003
   - xorg-libxt=1.3.0=hd590300_0
-  - zipp=3.15.0=pyhd8ed1ab_0
+  - zipp=3.16.2=pyhd8ed1ab_0
   - accessible-pygments=0.0.4=pyhd8ed1ab_0
   - aiosignal=1.3.1=pyhd8ed1ab_0
-  - anyio=3.7.0=pyhd8ed1ab_1
+  - anyio=3.7.1=pyhd8ed1ab_0
   - asttokens=2.2.1=pyhd8ed1ab_0
   - babel=2.12.1=pyhd8ed1ab_1
   - backports.functools_lru_cache=1.6.5=pyhd8ed1ab_0
   - beautifulsoup4=4.12.2=pyha770c72_0
   - bleach=6.0.0=pyhd8ed1ab_0
   - cairo=1.16.0=ha61ee94_1014
   - cffi=1.15.1=py310h255011f_3
   - comm=0.1.3=pyhd8ed1ab_0
   - curl=8.1.2=h409715c_0
   - dacite=1.8.0=pyhd8ed1ab_0
   - deprecation=2.1.0=pyh9f0ad1d_0
   - flake8=6.0.0=pyhd8ed1ab_0
-  - fonttools=4.40.0=py310h2372a71_0
+  - fonttools=4.41.0=py310h2372a71_0
   - glew=2.1.0=h9c3ff4c_2
-  - glib=2.76.3=hfc55251_0
+  - glib=2.76.4=hfc55251_0
   - hdf5=1.12.2=nompi_h4df4325_101
-  - importlib-metadata=6.7.0=pyha770c72_0
-  - importlib_resources=5.12.0=pyhd8ed1ab_0
+  - importlib-metadata=6.8.0=pyha770c72_0
+  - importlib_resources=6.0.0=pyhd8ed1ab_1
   - jedi=0.18.2=pyhd8ed1ab_0
   - jinja2=3.1.2=pyhd8ed1ab_1
   - jupyterlab_pygments=0.2.2=pyhd8ed1ab_0
   - latexcodec=2.0.1=pyh9f0ad1d_0
   - libclang=15.0.7=default_h7634d5b_2
   - libgd=2.3.3=h18fbbfe_3
   - libva=2.18.0=h0b41bf4_0
@@ -337,51 +338,52 @@
   - pyproject_hooks=1.0.0=pyhd8ed1ab_0
   - pytest=7.3.2=pyhd8ed1ab_1
   - python-dateutil=2.8.2=pyhd8ed1ab_0
   - pyu2f=0.1.5=pyhd8ed1ab_0
   - qtpy=2.3.1=pyhd8ed1ab_0
   - rfc3339-validator=0.1.4=pyhd8ed1ab_0
   - rsa=4.9=pyhd8ed1ab_0
+  - ruamel.yaml=0.17.32=py310h2372a71_0
   - sip=6.7.9=py310hc6cd4ac_0
   - sympy=1.12=pypyh9d50eac_103
   - tbb-devel=2021.9.0=hf52228f_0
   - terminado=0.17.1=pyh41d4057_0
   - tinycss2=1.2.1=pyhd8ed1ab_0
   - tqdm=4.65.0=pyhd8ed1ab_1
-  - typing-extensions=4.6.3=hd8ed1ab_0
+  - typing-extensions=4.7.1=hd8ed1ab_0
   - werkzeug=2.3.6=pyhd8ed1ab_0
   - yarl=1.9.2=py310h2372a71_0
   - argon2-cffi-bindings=21.2.0=py310h5764c6d_3
-  - astroid=2.15.5=py310hff52083_0
+  - astroid=2.15.6=py310hff52083_0
   - async-timeout=4.0.2=pyhd8ed1ab_0
   - brotlipy=0.7.0=py310h5764c6d_1005
-  - cryptography=41.0.1=py310h75e40e8_0
+  - cryptography=41.0.2=py310h75e40e8_0
   - ffmpeg=5.1.2=gpl_h8dda1f0_106
   - ghp-import=2.1.0=pyhd8ed1ab_0
   - gstreamer=1.22.0=h25f0c4b_2
   - harfbuzz=6.0.0=h8e241bc_0
-  - importlib_metadata=6.7.0=hd8ed1ab_0
+  - importlib_metadata=6.8.0=hd8ed1ab_0
   - jsonschema=4.17.3=pyhd8ed1ab_0
   - jupyter_server_terminals=0.4.4=pyhd8ed1ab_1
   - libblas=3.9.0=16_linux64_mkl
   - libitk=5.3.0=hcedbc38_0
   - libnetcdf=4.8.1=nompi_h261ec11_106
   - markdown=3.4.3=pyhd8ed1ab_0
   - mdit-py-plugins=0.4.0=pyhd8ed1ab_0
   - mkl-devel=2022.1.0=ha770c72_916
-  - platformdirs=3.8.0=pyhd8ed1ab_0
+  - platformdirs=3.9.1=pyhd8ed1ab_0
   - pulseaudio-daemon=16.1=ha8d29e2_3
   - pybtex=0.24.0=pyhd8ed1ab_2
   - pyqt5-sip=12.11.0=py310heca2aa9_3
   - python-build=0.10.0=pyhd8ed1ab_1
   - setuptools-scm=7.1.0=pyhd8ed1ab_0
-  - sqlalchemy=2.0.17=py310h2372a71_0
+  - sqlalchemy=2.0.19=py310h2372a71_0
   - stack_data=0.6.2=pyhd8ed1ab_0
   - wcwidth=0.2.6=pyhd8ed1ab_0
-  - aiohttp=3.8.4=py310h2372a71_1
+  - aiohttp=3.8.5=py310h2372a71_0
   - argon2-cffi=21.3.0=pyhd8ed1ab_0
   - black=22.3.0=pyhd8ed1ab_0
   - gst-plugins-base=1.22.0=h4243ec0_2
   - jupyter_core=5.3.1=py310hff52083_0
   - jupyter_events=0.6.3=pyhd8ed1ab_0
   - libcblas=3.9.0=16_linux64_mkl
   - liblapack=3.9.0=16_linux64_mkl
@@ -393,48 +395,49 @@
   - pyopenssl=23.2.0=pyhd8ed1ab_1
   - simpleitk=2.2.1=py310h2b9ea3a_1
   - flake8-black=0.3.6=pyhd8ed1ab_0
   - gtk2=2.24.33=h90689f9_2
   - jupyter_client=8.3.0=pyhd8ed1ab_0
   - liblapacke=3.9.0=16_linux64_mkl
   - librsvg=2.54.4=h7abd40a_0
-  - nbformat=5.9.0=pyhd8ed1ab_0
-  - numpy=1.25.0=py310ha4c1d20_0
+  - nbformat=5.9.1=pyhd8ed1ab_0
+  - numpy=1.25.1=py310ha4c1d20_0
   - prompt_toolkit=3.0.39=hd8ed1ab_0
   - qt-main=5.15.8=h5d23da1_6
   - urllib3=1.26.15=pyhd8ed1ab_0
   - wslink=1.11.1=pyhd8ed1ab_0
   - blas-devel=3.9.0=16_linux64_mkl
   - botocore=1.29.165=pyhd8ed1ab_0
   - contourpy=1.1.0=py310hd41b1e2_0
   - graphviz=7.0.5=h2e5815a_0
   - ipython=8.14.0=pyh41d4057_0
   - nbclient=0.7.4=pyhd8ed1ab_0
+  - nibabel=5.1.0=py310hff52083_2
   - pandas=1.5.3=py310h9b08913_1
   - pyqt=5.15.7=py310hab646b1_3
   - requests=2.31.0=pyhd8ed1ab_0
   - vtk=9.2.5=qt_py310hc895abb_200
   - blas=2.116=mkl
-  - google-auth=2.21.0=pyh1a96a4e_0
+  - google-auth=2.22.0=pyh1a96a4e_0
   - ipykernel=6.23.3=pyh71e2992_0
   - jupyter-cache=0.6.1=pyhd8ed1ab_0
-  - matplotlib-base=3.7.1=py310he60537e_0
-  - nbconvert-core=7.6.0=pyhd8ed1ab_0
+  - matplotlib-base=3.7.2=py310hf38f957_0
+  - nbconvert-core=7.7.1=pyhd8ed1ab_1
   - pooch=1.7.0=pyha770c72_3
   - requests-oauthlib=1.3.1=pyhd8ed1ab_0
   - s3transfer=0.6.1=pyhd8ed1ab_0
   - sphinx=4.5.0=pyh6c4a22f_0
   - boto3=1.26.165=pyhd8ed1ab_0
   - google-auth-oauthlib=1.0.0=pyhd8ed1ab_1
   - ipywidgets=8.0.7=pyhd8ed1ab_0
   - jupyter_console=6.6.3=pyhd8ed1ab_0
   - jupyter_server=2.7.0=pyhd8ed1ab_0
-  - matplotlib=3.7.1=py310hff52083_0
+  - matplotlib=3.7.2=py310hff52083_0
   - myst-parser=0.18.1=pyhd8ed1ab_0
-  - nbconvert-pandoc=7.6.0=pyhd8ed1ab_0
+  - nbconvert-pandoc=7.7.1=pyhd8ed1ab_1
   - pydata-sphinx-theme=0.13.3=pyhd8ed1ab_0
   - qtconsole-base=5.4.3=pyha770c72_0
   - scipy=1.10.1=py310ha4c1d20_3
   - sphinx-comments=0.0.3=pyh9f0ad1d_0
   - sphinx-copybutton=0.5.2=pyhd8ed1ab_0
   - sphinx-design=0.3.0=pyhd8ed1ab_0
   - sphinx-external-toc=0.3.1=pyhd8ed1ab_0
@@ -444,15 +447,15 @@
   - sphinx-thebe=0.2.1=pyhd8ed1ab_0
   - sphinx-togglebutton=0.3.2=pyhd8ed1ab_0
   - sphinxcontrib-bibtex=2.5.0=pyhd8ed1ab_0
   - sphinxcontrib-dotnetdomain=0.4=py_0
   - sphinxcontrib-golangdomain=0.2.0.dev0=py_0
   - sphinxcontrib-jquery=4.1=pyhd8ed1ab_0
   - myst-nb=0.17.2=pyhd8ed1ab_0
-  - nbconvert=7.6.0=pyhd8ed1ab_0
+  - nbconvert=7.7.1=pyhd8ed1ab_1
   - notebook-shim=0.2.3=pyhd8ed1ab_0
   - qtconsole=5.4.3=pyhd8ed1ab_0
   - sphinx-autoapi=2.1.0=pyhd8ed1ab_0
   - sphinx-book-theme=1.0.1=pyhd8ed1ab_0
   - sphinx_rtd_theme=1.2.2=pyha770c72_0
   - tensorboard=2.13.0=pyhd8ed1ab_0
   - jupyter-book=0.15.1=pyhd8ed1ab_0
```

### Comparing `hf-deepali-0.3.2/conda/environment.osx-64.lock` & `hf-deepali-0.4.0/conda/environment.osx-64.lock`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Generated by conda-lock.
 # platform: osx-64
-# input_hash: 1664d2c199c9cddb402252a38f5527d218754e954cbb25a82da7fecc8cbae3f6
+# input_hash: 533a7567b393584157366e71374225596e814fe74cfcb03642d3b4e184d58c87
 @EXPLICIT
 https://conda.anaconda.org/conda-forge/osx-64/bzip2-1.0.8-h0d85af4_4.tar.bz2#37edc4e6304ca87316e160f5ca0bd1b5
 https://conda.anaconda.org/conda-forge/osx-64/c-ares-1.19.1-h0dc2134_0.conda#b3e62631b4e1b9801477523ce1d6f355
 https://conda.anaconda.org/conda-forge/osx-64/ca-certificates-2023.5.7-h8857fd0_0.conda#b704e4b79ba0d887c4870b7b09d6a4df
 https://conda.anaconda.org/conda-forge/noarch/font-ttf-dejavu-sans-mono-2.37-hab24e00_0.tar.bz2#0c96522c6bdaed4b1566d11387caaf45
 https://conda.anaconda.org/conda-forge/noarch/font-ttf-inconsolata-3.000-h77eed37_0.tar.bz2#34893075a5c9e55cdafac56607368fc6
 https://conda.anaconda.org/conda-forge/noarch/font-ttf-source-code-pro-2.038-h77eed37_0.tar.bz2#4d59c254e01d9cde7957100457e2d5fb
@@ -41,15 +41,15 @@
 https://conda.anaconda.org/conda-forge/osx-64/x264-1!164.3095-h775f41a_2.tar.bz2#23e9c3180e2c0f9449bb042914ec2200
 https://conda.anaconda.org/conda-forge/osx-64/xorg-libxau-1.0.11-h0dc2134_0.conda#9566b4c29274125b0266d0177b5eb97b
 https://conda.anaconda.org/conda-forge/osx-64/xorg-libxdmcp-1.1.3-h35c211d_0.tar.bz2#86ac76d6bf1cbb9621943eb3bd9ae36e
 https://conda.anaconda.org/conda-forge/osx-64/xz-5.2.6-h775f41a_0.tar.bz2#a72f9d4ea13d55d745ff1ed594747f10
 https://conda.anaconda.org/conda-forge/osx-64/yaml-0.2.5-h0d85af4_2.tar.bz2#d7e08fcf8259d742156188e8762b4d20
 https://conda.anaconda.org/conda-forge/osx-64/aom-3.5.0-hf0c8a7f_0.tar.bz2#9110390ac33346f643e26051a92de5ce
 https://conda.anaconda.org/conda-forge/osx-64/double-conversion-3.2.0-hf0c8a7f_1.tar.bz2#3c2d7d657d83eac1507bc6fbab9eb297
-https://conda.anaconda.org/conda-forge/osx-64/eigen-3.4.0-h940c156_0.tar.bz2#f47a426ed1340c966f539c42187e3331
+https://conda.anaconda.org/conda-forge/osx-64/eigen-3.4.1-h1c7c39f_0.conda#4b30cbb5ec44b4ce28e92daac53f3132
 https://conda.anaconda.org/conda-forge/osx-64/expat-2.5.0-hf0c8a7f_1.conda#e12630038077877cbb6c7851e139c17c
 https://conda.anaconda.org/conda-forge/noarch/fonts-conda-forge-1-0.tar.bz2#f766549260d6815b0c52253f1fb1bb29
 https://conda.anaconda.org/conda-forge/osx-64/gettext-0.21.1-h8a4c099_0.tar.bz2#1e3aff29ce703d421c43f371ad676cc5
 https://conda.anaconda.org/conda-forge/osx-64/glew-2.1.0-h046ec9c_2.tar.bz2#6b753c8c7e4c46a8eb17b6f1781f958a
 https://conda.anaconda.org/conda-forge/osx-64/gmp-6.2.1-h2e338ed_0.tar.bz2#dedc96914428dae572a39e69ee2a392f
 https://conda.anaconda.org/conda-forge/osx-64/graphite2-1.3.13-h2e338ed_1001.tar.bz2#5f6e7f98caddd0fc2d345b207531814c
 https://conda.anaconda.org/conda-forge/osx-64/icu-70.1-h96cf925_0.tar.bz2#376635049e9b9b0bb875efd39dcd7b3b
@@ -79,35 +79,35 @@
 https://conda.anaconda.org/conda-forge/osx-64/readline-8.2-h9e318b2_1.conda#f17f77f2acf4d344734bda76829ce14e
 https://conda.anaconda.org/conda-forge/osx-64/svt-av1-1.4.1-hf0c8a7f_0.conda#86739428e1e1c8882fe14067a7ac371a
 https://conda.anaconda.org/conda-forge/osx-64/tbb-2021.9.0-hb8565cd_0.conda#6aedf8fdcdf5f2d7b4db21853a7d42ed
 https://conda.anaconda.org/conda-forge/osx-64/tk-8.6.12-h5dbffcc_0.tar.bz2#8e9480d9c47061db2ed1b4ecce519a7f
 https://conda.anaconda.org/conda-forge/osx-64/x265-3.5-hbb4e6a2_3.tar.bz2#a3bf3e95b7795871a6734a784400fcea
 https://conda.anaconda.org/conda-forge/osx-64/zeromq-4.3.4-he49afe7_1.tar.bz2#1972d732b123ed04b60fd21e94f0b178
 https://conda.anaconda.org/conda-forge/osx-64/zlib-1.2.13-h8a1eda9_5.conda#75a8a98b1c4671c5d2897975731da42d
-https://conda.anaconda.org/conda-forge/osx-64/zstd-1.5.2-hbc0c0cd_6.conda#40a188783d3c425bdccc9ae9104acbb8
+https://conda.anaconda.org/conda-forge/osx-64/zstd-1.5.2-h829000d_7.conda#b274ec4dbf15a6e20900e397610567a0
 https://conda.anaconda.org/conda-forge/osx-64/brotli-bin-1.0.9-hb7f2c08_9.conda#72c526f7ffa265473e6c75fd90605e52
 https://conda.anaconda.org/conda-forge/noarch/fonts-conda-ecosystem-1-0.tar.bz2#fee5683a3f04bd15cbd8318b096a27ab
 https://conda.anaconda.org/conda-forge/osx-64/freetype-2.12.1-h3f81eb7_1.conda#852224ea3e8991a8342228eab274840e
 https://conda.anaconda.org/conda-forge/osx-64/gl2ps-1.4.2-h4cff582_0.tar.bz2#a9e91533b95cd019d58f4b3ef9bbddf0
 https://conda.anaconda.org/conda-forge/osx-64/hdf4-4.2.15-h7aa5921_5.tar.bz2#a5e171d71c6b524409de40d81c098758
 https://conda.anaconda.org/conda-forge/osx-64/krb5-1.20.1-h049b76e_0.conda#db11fa2968ef0837288fe2d7f5b77a50
 https://conda.anaconda.org/conda-forge/osx-64/libclang-13.0.1-default_h255f2f3_1.conda#7ffe2879ebb140302889d22a1ec41d84
 https://conda.anaconda.org/conda-forge/osx-64/libgfortran-5.0.0-11_3_0_h97931a8_31.conda#97451338600bd9c5b535eb224ef6c471
-https://conda.anaconda.org/conda-forge/osx-64/libglib-2.76.3-hc62aa5d_0.conda#3687b3c1d257dec787418281cfc58358
+https://conda.anaconda.org/conda-forge/osx-64/libglib-2.76.4-hc62aa5d_0.conda#05c728fccc40277119bf94cf08e38384
 https://conda.anaconda.org/conda-forge/osx-64/libidn2-2.3.4-hb7f2c08_0.tar.bz2#bd109fd705b4ce40a62759129bc4ef5a
 https://conda.anaconda.org/conda-forge/osx-64/libnghttp2-1.52.0-he2ab024_0.conda#12ac7d100bf260263e30a019517f42a2
 https://conda.anaconda.org/conda-forge/osx-64/libprotobuf-4.23.3-h5feb325_0.conda#b9e780ed0d0a365ff10b8e83c64471ce
 https://conda.anaconda.org/conda-forge/osx-64/libssh2-1.11.0-hd019ec5_0.conda#ca3a72efba692c59a90d4b9fc0dfe774
 https://conda.anaconda.org/conda-forge/osx-64/libtheora-1.1.1-h0d85af4_1005.tar.bz2#e63b84ed4c2d84901332de92a98a2f2b
 https://conda.anaconda.org/conda-forge/osx-64/libtiff-4.4.0-h6268bbc_5.conda#551fc78ba147767ea5905d0746e2fbb5
 https://conda.anaconda.org/conda-forge/osx-64/libxml2-2.10.3-h201ad9d_4.conda#2101dd548f0601be252e27e48fa532fa
 https://conda.anaconda.org/conda-forge/osx-64/libzip-1.9.2-h6db710c_1.tar.bz2#ce732d37e479919f3d22b1ccdeb858ac
 https://conda.anaconda.org/conda-forge/osx-64/mkl-2022.1.0-h860c996_928.tar.bz2#98a4d58de0ba6e61ce46620b775c19ce
 https://conda.anaconda.org/conda-forge/osx-64/mpfr-4.2.0-h4f9bd69_0.conda#f48a2f4515be334c5cfeed82517b96e0
-https://conda.anaconda.org/conda-forge/osx-64/mysql-common-8.0.33-hc6116ba_1.conda#bfbfd93ef846f67d53f40bcf28b91621
+https://conda.anaconda.org/conda-forge/osx-64/mysql-common-8.0.33-hc6116ba_2.conda#6f1f77589d0af4e85e32f896d2a51f4e
 https://conda.anaconda.org/conda-forge/osx-64/nss-3.89-h78b00b3_0.conda#1eb1408ecae62d98a902636d46f5595c
 https://conda.anaconda.org/conda-forge/osx-64/python-3.10.12-had23ca6_0_cpython.conda#351b8aa0687f3510620cf06ad11229f4
 https://conda.anaconda.org/conda-forge/osx-64/sqlite-3.42.0-h2b0dec6_0.conda#6c22b83608a6e3bd324ab29d3092592f
 https://conda.anaconda.org/conda-forge/osx-64/tbb-devel-2021.9.0-hb8565cd_0.conda#23fd9e2cb5478ed8b6ba925a741af61b
 https://conda.anaconda.org/conda-forge/noarch/absl-py-1.4.0-pyhd8ed1ab_0.conda#dd5eed01874c75bebef810a2faec673e
 https://conda.anaconda.org/conda-forge/noarch/alabaster-0.7.13-pyhd8ed1ab_0.conda#06006184e203b61d3525f90de394471e
 https://conda.anaconda.org/conda-forge/noarch/appnope-0.1.3-pyhd8ed1ab_0.tar.bz2#54ac328d703bff191256ffa1183126d1
@@ -115,93 +115,94 @@
 https://conda.anaconda.org/conda-forge/noarch/attrs-21.4.0-pyhd8ed1ab_0.tar.bz2#f70280205d7044c8b8358c8de3190e5d
 https://conda.anaconda.org/conda-forge/noarch/backcall-0.2.0-pyh9f0ad1d_0.tar.bz2#6006a6d08a3fa99268a2681c7fb55213
 https://conda.anaconda.org/conda-forge/noarch/backports-1.0-pyhd8ed1ab_3.conda#54ca2e08b3220c148a1d8329c2678e02
 https://conda.anaconda.org/conda-forge/noarch/blinker-1.6.2-pyhd8ed1ab_0.conda#2fb79ec81bad9492b6d59a06b3b647a4
 https://conda.anaconda.org/conda-forge/osx-64/brotli-1.0.9-hb7f2c08_9.conda#53cff90f0cea22e13e5b791f0e5a8e7d
 https://conda.anaconda.org/conda-forge/noarch/cachetools-5.3.1-pyhd8ed1ab_0.conda#60b5eb16d9a7a5482ba37f67aa49db5b
 https://conda.anaconda.org/conda-forge/noarch/certifi-2023.5.7-pyhd8ed1ab_0.conda#5d1b71c942b8421285934dad1d891ebc
-https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-3.1.0-pyhd8ed1ab_0.conda#7fcff9f6f123696e940bda77bd4d6551
-https://conda.anaconda.org/conda-forge/noarch/click-8.1.3-unix_pyhd8ed1ab_2.tar.bz2#20e4087407c7cb04a40817114b333dbf
+https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-3.2.0-pyhd8ed1ab_0.conda#313516e9a4b08b12dfb1e1cd390a96e3
+https://conda.anaconda.org/conda-forge/noarch/click-8.1.6-unix_pyh707e725_0.conda#64dbb3b205546691a61204d1cfb208e3
 https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.6-pyhd8ed1ab_0.tar.bz2#3faab06a954c2a04039983f2c4a50d99
 https://conda.anaconda.org/conda-forge/noarch/cycler-0.11.0-pyhd8ed1ab_0.tar.bz2#a50559fad0affdbb33729a68669ca1cb
 https://conda.anaconda.org/conda-forge/noarch/dataclasses-0.8-pyhc8e2a94_3.tar.bz2#a362b2124b06aad102e2ee4581acee7d
 https://conda.anaconda.org/conda-forge/osx-64/debugpy-1.6.7-py310h7a76584_0.conda#549f7722839c44ee8a859fc0b94a5884
 https://conda.anaconda.org/conda-forge/noarch/decorator-5.1.1-pyhd8ed1ab_0.tar.bz2#43afe5ab04e35e17ba28649471dd7364
 https://conda.anaconda.org/conda-forge/noarch/defusedxml-0.7.1-pyhd8ed1ab_0.tar.bz2#961b3a227b437d82ad7054484cfa71b2
 https://conda.anaconda.org/conda-forge/osx-64/docutils-0.17.1-py310h2ec42d9_3.tar.bz2#69b3569d320b0fc940449fcc25b01e31
 https://conda.anaconda.org/conda-forge/noarch/entrypoints-0.4-pyhd8ed1ab_0.tar.bz2#3cf04868fee0a029769bd41f4b2fbf2d
 https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.1.2-pyhd8ed1ab_0.conda#de4cb3384374e1411f0454edcf546cdb
 https://conda.anaconda.org/conda-forge/noarch/executing-1.2.0-pyhd8ed1ab_0.tar.bz2#4c1bc140e2be5c8ba6e3acab99e25c50
 https://conda.anaconda.org/conda-forge/osx-64/fftw-3.3.10-nompi_h4fa670e_108.conda#39132ce6ed3180b42b54d40289cd4157
 https://conda.anaconda.org/conda-forge/noarch/filelock-3.12.2-pyhd8ed1ab_0.conda#53522ec72e6adae42bd373ef58357230
 https://conda.anaconda.org/conda-forge/noarch/flit-core-3.9.0-pyhd8ed1ab_0.conda#e8cfceef004266b259604c3faa2a0191
 https://conda.anaconda.org/conda-forge/osx-64/fontconfig-2.14.2-h5bb23bf_0.conda#86cc5867dfbee4178118392bae4a3c89
-https://conda.anaconda.org/conda-forge/osx-64/frozenlist-1.3.3-py310h90acd4f_0.tar.bz2#a3236ddc60f49384eba9348391293038
+https://conda.anaconda.org/conda-forge/osx-64/frozenlist-1.4.0-py310h6729b98_0.conda#f436715de06c55f25e12867550a3589a
 https://conda.anaconda.org/conda-forge/noarch/fsspec-2023.6.0-pyh1a96a4e_0.conda#50ea2067ec92dfcc38b4f07992d7e235
 https://conda.anaconda.org/conda-forge/osx-64/gdk-pixbuf-2.42.8-h3648f77_1.tar.bz2#f709a0451aa786175db4c3cfa2af35cc
-https://conda.anaconda.org/conda-forge/osx-64/glib-tools-2.76.3-h7d26f99_0.conda#43d414c01245d3655df3115c078b90d8
+https://conda.anaconda.org/conda-forge/osx-64/glib-tools-2.76.4-h7d26f99_0.conda#6a8b2c5e964467242058c27bace19c7f
 https://conda.anaconda.org/conda-forge/osx-64/gnutls-3.7.8-h207c4f0_0.tar.bz2#3886476538060824c0258316fd5bb828
 https://conda.anaconda.org/conda-forge/osx-64/greenlet-2.0.2-py310h9e9d8ca_1.conda#699b3a96666340fe9349c3547f047e29
 https://conda.anaconda.org/conda-forge/osx-64/gts-0.7.6-h53e17e3_4.conda#848cc963fcfbd063c7a023024aa3bec0
 https://conda.anaconda.org/conda-forge/noarch/idna-3.4-pyhd8ed1ab_0.tar.bz2#34272b248891bddccc64479f9a7fffed
 https://conda.anaconda.org/conda-forge/noarch/imagesize-1.4.1-pyhd8ed1ab_0.tar.bz2#7de5386c8fea29e76b303f37dde4c352
 https://conda.anaconda.org/conda-forge/noarch/iniconfig-2.0.0-pyhd8ed1ab_0.conda#f800d2da156d08e289b14e87e43c1ae5
 https://conda.anaconda.org/conda-forge/noarch/ipython_genutils-0.2.0-py_1.tar.bz2#5071c982548b3a20caf70462f04f5287
 https://conda.anaconda.org/conda-forge/noarch/jmespath-1.0.1-pyhd8ed1ab_0.tar.bz2#2cfa3e1cf3fb51bb9b17acc5b5e9ea11
 https://conda.anaconda.org/conda-forge/noarch/jupyterlab_widgets-3.0.8-pyhd8ed1ab_0.conda#2bc3ca2f7387af385dd06706b4fb2d35
 https://conda.anaconda.org/conda-forge/osx-64/kiwisolver-1.4.4-py310ha23aa8a_1.tar.bz2#cc358fb878ac593c60cea08b28ac7423
 https://conda.anaconda.org/conda-forge/osx-64/lazy-object-proxy-1.9.0-py310h90acd4f_0.conda#b0b1dc46dd92f49877ea8eecd56f2d00
 https://conda.anaconda.org/conda-forge/osx-64/lcms2-2.14-h90f4b2a_0.tar.bz2#e56c432e9a78c63692fa6bd076a15713
 https://conda.anaconda.org/conda-forge/osx-64/libblas-3.9.0-17_osx64_mkl.conda#e5d4b69958f8eb30b932828880b847f3
 https://conda.anaconda.org/conda-forge/osx-64/libcurl-8.1.2-hbee3ae8_0.conda#d51e337da844262f9033c9a26452520f
-https://conda.anaconda.org/conda-forge/osx-64/libgrpc-1.56.0-he6801ca_2.conda#46a189776f694d37c24c5c1fc301bf50
+https://conda.anaconda.org/conda-forge/osx-64/libgrpc-1.56.2-he6801ca_0.conda#c0bb2505f166b769ae3e1e01dce31fe9
 https://conda.anaconda.org/conda-forge/osx-64/libpq-15.3-h9dc22bb_1.conda#571aa9141d1a823202bb4cd794c939b0
 https://conda.anaconda.org/conda-forge/osx-64/libwebp-1.2.4-hfa4350a_0.tar.bz2#d3b5a56369701e6a11bf300ba3394391
 https://conda.anaconda.org/conda-forge/osx-64/loguru-0.7.0-py310h2ec42d9_0.conda#632a71feccc9f651c844c402efe61884
 https://conda.anaconda.org/conda-forge/osx-64/markupsafe-2.1.3-py310h6729b98_0.conda#b23ce1495527802905791489c3b1f129
 https://conda.anaconda.org/conda-forge/noarch/mccabe-0.7.0-pyhd8ed1ab_0.tar.bz2#34fc335fc50eef0b5ea708f2b5f54e0c
 https://conda.anaconda.org/conda-forge/noarch/mdurl-0.1.0-pyhd8ed1ab_0.tar.bz2#f8dab71fdc13b1bf29a01248b156d268
 https://conda.anaconda.org/conda-forge/noarch/mistune-3.0.0-pyhd8ed1ab_0.conda#c7d0ea64c37752ecbe6da458aee662d2
 https://conda.anaconda.org/conda-forge/osx-64/mkl-devel-2022.1.0-h694c41f_929.tar.bz2#041ceef009fe6d29cbd2555907c23ab3
 https://conda.anaconda.org/conda-forge/osx-64/mpc-1.3.1-h81bd1dd_0.conda#c752c0eb6c250919559172c011e5f65b
 https://conda.anaconda.org/conda-forge/noarch/mpmath-1.3.0-pyhd8ed1ab_0.conda#dbf6e2d89137da32fa6670f3bffc024e
 https://conda.anaconda.org/conda-forge/osx-64/multidict-6.0.4-py310h90acd4f_0.conda#0324181c4442d94c865cf9ae3b6a7fea
 https://conda.anaconda.org/conda-forge/noarch/munkres-1.1.4-pyh9f0ad1d_0.tar.bz2#2ba8498c1018c1e9c61eb99b973dfe19
 https://conda.anaconda.org/conda-forge/noarch/mypy_extensions-1.0.0-pyha770c72_0.conda#4eccaeba205f0aed9ac3a9ea58568ca3
-https://conda.anaconda.org/conda-forge/osx-64/mysql-libs-8.0.33-haa61052_1.conda#b1ba5ec2e4a774e8e4887f0f7592b574
+https://conda.anaconda.org/conda-forge/osx-64/mysql-libs-8.0.33-haa61052_2.conda#0e750706160c8e178864b890d3afd164
 https://conda.anaconda.org/conda-forge/noarch/nest-asyncio-1.5.6-pyhd8ed1ab_0.tar.bz2#7b868f21adde0d9b8b38f9c16836589b
 https://conda.anaconda.org/conda-forge/noarch/networkx-3.1-pyhd8ed1ab_0.conda#254f787d5068bc89f578bf63893ce8b4
 https://conda.anaconda.org/conda-forge/osx-64/openjpeg-2.5.0-h5d0d7b0_1.tar.bz2#be533cc782981a0ec5eed28aa618470a
 https://conda.anaconda.org/conda-forge/noarch/packaging-23.1-pyhd8ed1ab_0.conda#91cda59e66e1e4afe9476f8ef98f5c30
 https://conda.anaconda.org/conda-forge/noarch/pandocfilters-1.5.0-pyhd8ed1ab_0.tar.bz2#457c2c8c08e54905d6954e79cb5b5db9
 https://conda.anaconda.org/conda-forge/noarch/parso-0.8.3-pyhd8ed1ab_0.tar.bz2#17a565a0c3899244e938cdf417e7b094
 https://conda.anaconda.org/conda-forge/noarch/pathspec-0.11.1-pyhd8ed1ab_0.conda#dbb80d1e8dc2dba5c8b106dc0768ad45
 https://conda.anaconda.org/conda-forge/noarch/pickleshare-0.7.5-py_1003.tar.bz2#415f0ebb6198cc2801c73438a9fb5761
 https://conda.anaconda.org/conda-forge/noarch/pkgutil-resolve-name-1.3.10-pyhd8ed1ab_0.tar.bz2#89e3c7cdde7d3aaa2aee933b604dd07f
 https://conda.anaconda.org/conda-forge/noarch/pluggy-1.2.0-pyhd8ed1ab_0.conda#7263924c642d22e311d9e59b839f1b33
 https://conda.anaconda.org/conda-forge/noarch/ply-3.11-py_1.tar.bz2#7205635cd71531943440fbfe3b6b5727
-https://conda.anaconda.org/conda-forge/noarch/prometheus_client-0.17.0-pyhd8ed1ab_0.conda#95c5be3c7cbd872509d16c216617fdab
+https://conda.anaconda.org/conda-forge/noarch/prometheus_client-0.17.1-pyhd8ed1ab_0.conda#02153b6b760bbec00cfe9e4c97993d06
 https://conda.anaconda.org/conda-forge/osx-64/psutil-5.9.5-py310h90acd4f_0.conda#1111504c53989e065a98171156fc376a
 https://conda.anaconda.org/conda-forge/noarch/ptyprocess-0.7.0-pyhd3deb0d_0.tar.bz2#359eeb6536da0e687af562ed265ec263
 https://conda.anaconda.org/conda-forge/noarch/pure_eval-0.2.2-pyhd8ed1ab_0.tar.bz2#6784285c7e55cb7212efabc79e4c2883
 https://conda.anaconda.org/conda-forge/noarch/pyasn1-0.4.8-py_0.tar.bz2#06d04c9f8f72ac77911db942eda24fb9
 https://conda.anaconda.org/conda-forge/noarch/pycodestyle-2.10.0-pyhd8ed1ab_0.conda#89843e4cc99c6a3fe5f4c86994cc8410
 https://conda.anaconda.org/conda-forge/noarch/pycparser-2.21-pyhd8ed1ab_0.tar.bz2#076becd9e05608f8dc72757d5f3a91ff
 https://conda.anaconda.org/conda-forge/noarch/pyflakes-3.0.1-pyhd8ed1ab_0.conda#44b7d77d96560c93e0e11437a3c35254
 https://conda.anaconda.org/conda-forge/noarch/pygments-2.15.1-pyhd8ed1ab_0.conda#d316679235612869eba305aa7d41d9bf
-https://conda.anaconda.org/conda-forge/noarch/pyjwt-2.7.0-pyhd8ed1ab_0.conda#99e28be5a278e2319834d7dc99e7bfdd
-https://conda.anaconda.org/conda-forge/noarch/pyparsing-3.1.0-pyhd8ed1ab_0.conda#d3ed087d1f7f8f5590e8e87b57a8ce64
+https://conda.anaconda.org/conda-forge/noarch/pyjwt-2.8.0-pyhd8ed1ab_0.conda#912c0194f898fdb783021fd25f913c31
+https://conda.anaconda.org/conda-forge/noarch/pyparsing-3.0.9-pyhd8ed1ab_0.tar.bz2#e8fbc1b54b25f4b08281467bc13b70cc
 https://conda.anaconda.org/conda-forge/osx-64/pyrsistent-0.19.3-py310h90acd4f_0.conda#2de2b931546de39d852e5d21e58876c1
 https://conda.anaconda.org/conda-forge/noarch/pysocks-1.7.1-pyha2e5f31_6.tar.bz2#2a7de29fb590ca14b5243c4c812c8025
 https://conda.anaconda.org/conda-forge/noarch/python-fastjsonschema-2.17.1-pyhd8ed1ab_0.conda#dd4f393d857e9283eef2442234bd05e3
 https://conda.anaconda.org/conda-forge/noarch/python-json-logger-2.0.7-pyhd8ed1ab_0.conda#a61bf9ec79426938ff785eb69dbb1960
 https://conda.anaconda.org/conda-forge/noarch/pytz-2023.3-pyhd8ed1ab_0.conda#d3076b483092a435832603243567bc31
 https://conda.anaconda.org/conda-forge/osx-64/pyyaml-6.0-py310h90acd4f_5.tar.bz2#e0ba2009f52ccda088c63dedf0d1c5ec
 https://conda.anaconda.org/conda-forge/osx-64/pyzmq-25.1.0-py310h998be00_0.conda#d31ade96a299a26bcb59b74a9b3c1dd6
 https://conda.anaconda.org/conda-forge/noarch/rfc3986-validator-0.1.1-pyh9f0ad1d_0.tar.bz2#912a71cc01012ee38e6b90ddd561e36f
+https://conda.anaconda.org/conda-forge/osx-64/ruamel.yaml.clib-0.2.7-py310h90acd4f_1.conda#d27546735a054dd67e626b17ff07c089
 https://conda.anaconda.org/conda-forge/noarch/setuptools-67.7.2-pyhd8ed1ab_0.conda#3b68bc43ec6baa48f7354a446267eefe
 https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2#e5f25f8dbc060e9a8d912e432202afc2
 https://conda.anaconda.org/conda-forge/noarch/sniffio-1.3.0-pyhd8ed1ab_0.tar.bz2#dd6cbc539e74cb1f430efbd4575b9303
 https://conda.anaconda.org/conda-forge/noarch/snowballstemmer-2.2.0-pyhd8ed1ab_0.tar.bz2#4d22a9315e78c6827f806065957d566e
 https://conda.anaconda.org/conda-forge/noarch/soupsieve-2.3.2.post1-pyhd8ed1ab_0.tar.bz2#146f4541d643d48fc8a75cacf69f03ae
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-applehelp-1.0.4-pyhd8ed1ab_0.conda#5a31a7d564f551d0e6dff52fd8cb5b16
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-devhelp-1.0.2-py_0.tar.bz2#68e01cac9d38d0e717cd5c87bc3d2cc9
@@ -212,48 +213,48 @@
 https://conda.anaconda.org/conda-forge/noarch/tabulate-0.9.0-pyhd8ed1ab_1.tar.bz2#4759805cce2d914c38472f70bf4d8bcb
 https://conda.anaconda.org/conda-forge/osx-64/tensorboard-data-server-0.7.0-py310hdd0c95c_0.conda#a57f926841a85a41249ee67023498281
 https://conda.anaconda.org/conda-forge/noarch/toml-0.10.2-pyhd8ed1ab_0.tar.bz2#f832c45a477c78bebd107098db465095
 https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2#5844808ffab9ebdb694585b50ba02a96
 https://conda.anaconda.org/conda-forge/osx-64/tornado-6.3.2-py310h6729b98_0.conda#369ce2c5cd18205e4917f515b4052376
 https://conda.anaconda.org/conda-forge/noarch/traitlets-5.9.0-pyhd8ed1ab_0.conda#d0b4f5c87cd35ac3fb3d47b223263a64
 https://conda.anaconda.org/conda-forge/osx-64/typed-ast-1.5.4-py310h90acd4f_1.tar.bz2#189bf6e55cac449f8b34763502b18385
-https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.6.3-pyha770c72_0.conda#4a3014a4d107d15475d106b751c4e352
+https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.7.1-pyha770c72_0.conda#c39d6a09fe819de4951c2642629d9115
 https://conda.anaconda.org/conda-forge/noarch/typing_utils-0.1.0-pyhd8ed1ab_0.tar.bz2#eb67e3cace64c66233e2d35949e20f92
 https://conda.anaconda.org/conda-forge/noarch/uc-micro-py-1.0.1-pyhd8ed1ab_0.tar.bz2#3ddf6684d9b274a12c94e509ca45656c
 https://conda.anaconda.org/conda-forge/osx-64/unicodedata2-15.0.0-py310h90acd4f_0.tar.bz2#b62adca3645b3bbc46940d5b1833d59b
 https://conda.anaconda.org/conda-forge/noarch/unidecode-1.3.6-pyhd8ed1ab_0.tar.bz2#e8f24401b17802df5f82f66a88cee29e
 https://conda.anaconda.org/conda-forge/noarch/webencodings-0.5.1-py_1.tar.bz2#3563be4c5611a44210d9ba0c16113136
 https://conda.anaconda.org/conda-forge/noarch/websocket-client-1.6.1-pyhd8ed1ab_0.conda#c34d9325a609381a0b0e8a5b4f325147
-https://conda.anaconda.org/conda-forge/noarch/wheel-0.40.0-pyhd8ed1ab_0.conda#49bb0d9e60ce1db25e151780331bb5f3
+https://conda.anaconda.org/conda-forge/noarch/wheel-0.40.0-pyhd8ed1ab_1.conda#c95fac682453aeffa12db7ae5a721bec
 https://conda.anaconda.org/conda-forge/noarch/widgetsnbextension-4.0.8-pyhd8ed1ab_0.conda#2e9ebddf0b93d0fb203d0906b8052c4f
 https://conda.anaconda.org/conda-forge/osx-64/wrapt-1.15.0-py310h90acd4f_0.conda#f91dbc3c63e137a27a4de2964d56e6e3
-https://conda.anaconda.org/conda-forge/noarch/zipp-3.15.0-pyhd8ed1ab_0.conda#13018819ca8f5b7cc675a8faf1f5fedf
+https://conda.anaconda.org/conda-forge/noarch/zipp-3.16.2-pyhd8ed1ab_0.conda#2da0451b54c4563c32490cb1b7cf68a1
 https://conda.anaconda.org/conda-forge/noarch/accessible-pygments-0.0.4-pyhd8ed1ab_0.conda#46a2e6e3dfa718ce3492018d5a110dd6
 https://conda.anaconda.org/conda-forge/noarch/aiosignal-1.3.1-pyhd8ed1ab_0.tar.bz2#d1e1eb7e21a9e2c74279d87dafb68156
-https://conda.anaconda.org/conda-forge/noarch/anyio-3.7.0-pyhd8ed1ab_1.conda#2b35a85d654a47aac8f34c1bb6de7142
+https://conda.anaconda.org/conda-forge/noarch/anyio-3.7.1-pyhd8ed1ab_0.conda#7b517e7a6f0790337906c055aa97ca49
 https://conda.anaconda.org/conda-forge/noarch/asttokens-2.2.1-pyhd8ed1ab_0.conda#bf7f54dd0f25c3f06ecb82a07341841a
 https://conda.anaconda.org/conda-forge/noarch/babel-2.12.1-pyhd8ed1ab_1.conda#ac432e732804a81ddcf29c92ead57cde
 https://conda.anaconda.org/conda-forge/noarch/backports.functools_lru_cache-1.6.5-pyhd8ed1ab_0.conda#6b1b907661838a75d067a22f87996b2e
 https://conda.anaconda.org/conda-forge/noarch/beautifulsoup4-4.12.2-pyha770c72_0.conda#a362ff7d976217f8fa78c0f1c4f59717
 https://conda.anaconda.org/conda-forge/noarch/bleach-6.0.0-pyhd8ed1ab_0.conda#d48b143d01385872a88ef8417e96c30e
 https://conda.anaconda.org/conda-forge/osx-64/cairo-1.16.0-h904041c_1014.tar.bz2#2e7b4350178ed52bb6fd2b1ecbeeed4f
 https://conda.anaconda.org/conda-forge/osx-64/cffi-1.15.1-py310ha78151a_3.conda#652082e4a6cf9d26e43d0d362590c276
 https://conda.anaconda.org/conda-forge/noarch/comm-0.1.3-pyhd8ed1ab_0.conda#168ae0f82cdf7505048e81054c7354e4
 https://conda.anaconda.org/conda-forge/osx-64/curl-8.1.2-hbee3ae8_0.conda#6cc301a6c2ba26e29949818efdc133ca
 https://conda.anaconda.org/conda-forge/noarch/dacite-1.8.0-pyhd8ed1ab_0.conda#3696792ba70ab3374320fe6041a82286
 https://conda.anaconda.org/conda-forge/noarch/deprecation-2.1.0-pyh9f0ad1d_0.tar.bz2#7b6747d7cc2076341029cff659669e8b
 https://conda.anaconda.org/conda-forge/osx-64/ffmpeg-5.1.2-gpl_h8b4fe81_106.conda#3c62afa3457aeb6f058b40f1f41f772a
 https://conda.anaconda.org/conda-forge/noarch/flake8-6.0.0-pyhd8ed1ab_0.conda#e9345ba05d71742412b8aa6992ad9457
-https://conda.anaconda.org/conda-forge/osx-64/fonttools-4.40.0-py310h6729b98_0.conda#15dcc729f2102b4b64e0e6f53f2fb377
-https://conda.anaconda.org/conda-forge/osx-64/glib-2.76.3-h7d26f99_0.conda#a062952a59c0a26adb18899ac6472a7e
+https://conda.anaconda.org/conda-forge/osx-64/fonttools-4.41.0-py310h6729b98_0.conda#2de0c6bd77a2ea8aa4e82943273c5dd3
+https://conda.anaconda.org/conda-forge/osx-64/glib-2.76.4-h7d26f99_0.conda#4176982aebeacb4f6914ea5528dc2853
 https://conda.anaconda.org/conda-forge/osx-64/gmpy2-2.1.2-py310hb691cb2_1.tar.bz2#a495ede1fb673f39133b7c2628af7259
-https://conda.anaconda.org/conda-forge/osx-64/grpcio-1.56.0-py310h0d4bf3c_2.conda#0ce1b3a5e4abf21c5a33e8d270ec2be2
+https://conda.anaconda.org/conda-forge/osx-64/grpcio-1.56.2-py310h0d4bf3c_0.conda#6be89e336739268b0415850c065cc0d8
 https://conda.anaconda.org/conda-forge/osx-64/hdf5-1.12.2-nompi_h48135f9_101.conda#2ee4811ba5f72f7f12f69b3ec2d6cd96
-https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-6.7.0-pyha770c72_0.conda#ba3786c6846e46038fe60c785d46dc81
-https://conda.anaconda.org/conda-forge/noarch/importlib_resources-5.12.0-pyhd8ed1ab_0.conda#e5fd2260a231ee63b6969f4801082f2b
+https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-6.8.0-pyha770c72_0.conda#4e9f59a060c3be52bc4ddc46ee9b6946
+https://conda.anaconda.org/conda-forge/noarch/importlib_resources-6.0.0-pyhd8ed1ab_1.conda#a08b6be5bf18b9d2a927d3457750f82e
 https://conda.anaconda.org/conda-forge/noarch/jedi-0.18.2-pyhd8ed1ab_0.conda#b5e695ef9c3f0d27d6cd96bf5adc9e07
 https://conda.anaconda.org/conda-forge/noarch/jinja2-3.1.2-pyhd8ed1ab_1.tar.bz2#c8490ed5c70966d232fdd389d0dbed37
 https://conda.anaconda.org/conda-forge/noarch/jupyterlab_pygments-0.2.2-pyhd8ed1ab_0.tar.bz2#243f63592c8e449f40cd42eb5cf32f40
 https://conda.anaconda.org/conda-forge/noarch/latexcodec-2.0.1-pyh9f0ad1d_0.tar.bz2#8d67904973263afd2985ba56aa2d6bb4
 https://conda.anaconda.org/conda-forge/osx-64/libcblas-3.9.0-17_osx64_mkl.conda#5adcad22978f80fa101047022e79d9eb
 https://conda.anaconda.org/conda-forge/osx-64/libgd-2.3.3-h1e214de_3.tar.bz2#350af2b75c58dc16985fa97298469143
 https://conda.anaconda.org/conda-forge/osx-64/liblapack-3.9.0-17_osx64_mkl.conda#5557060dea295fcbb224be17b3947d16
@@ -272,102 +273,104 @@
 https://conda.anaconda.org/conda-forge/noarch/pyproject_hooks-1.0.0-pyhd8ed1ab_0.conda#21de50391d584eb7f4441b9de1ad773f
 https://conda.anaconda.org/conda-forge/noarch/pytest-7.3.2-pyhd8ed1ab_1.conda#f2465696f4396245eca4613f6e924796
 https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.8.2-pyhd8ed1ab_0.tar.bz2#dd999d1cc9f79e67dbb855c8924c7984
 https://conda.anaconda.org/conda-forge/noarch/pyu2f-0.1.5-pyhd8ed1ab_0.tar.bz2#caabbeaa83928d0c3e3949261daa18eb
 https://conda.anaconda.org/conda-forge/noarch/qtpy-2.3.1-pyhd8ed1ab_0.conda#10812eca3ec4ebaf3749e1960c208d43
 https://conda.anaconda.org/conda-forge/noarch/rfc3339-validator-0.1.4-pyhd8ed1ab_0.tar.bz2#fed45fc5ea0813240707998abe49f520
 https://conda.anaconda.org/conda-forge/noarch/rsa-4.9-pyhd8ed1ab_0.tar.bz2#03bf410858b2cefc267316408a77c436
+https://conda.anaconda.org/conda-forge/osx-64/ruamel.yaml-0.17.32-py310h6729b98_0.conda#4c87395e8169331108914e30ab46d2a4
 https://conda.anaconda.org/conda-forge/osx-64/sip-6.7.9-py310h9e9d8ca_0.conda#5aae43762f6fe7bbdd3e0e2bbd567999
 https://conda.anaconda.org/conda-forge/noarch/terminado-0.17.1-pyhd1c38e8_0.conda#046120b71d8896cb7faef78bfdbfee1e
 https://conda.anaconda.org/conda-forge/noarch/tinycss2-1.2.1-pyhd8ed1ab_0.tar.bz2#7234c9eefff659501cd2fe0d2ede4d48
 https://conda.anaconda.org/conda-forge/noarch/tqdm-4.65.0-pyhd8ed1ab_1.conda#ed792aff3acb977d09c7013358097f83
-https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.6.3-hd8ed1ab_0.conda#3876f650ed7d0f95d70fa4b647621909
+https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.7.1-hd8ed1ab_0.conda#f96688577f1faa58096d06a45136afa2
 https://conda.anaconda.org/conda-forge/noarch/werkzeug-2.3.6-pyhd8ed1ab_0.conda#55fbbb3e67185820ee2007395bfe0073
 https://conda.anaconda.org/conda-forge/osx-64/yarl-1.9.2-py310h6729b98_0.conda#f8a1c7107b3b661accf1a7d86c8fd4e1
 https://conda.anaconda.org/conda-forge/osx-64/argon2-cffi-bindings-21.2.0-py310h90acd4f_3.tar.bz2#952166ee5ce75092167a7385a4e243e3
-https://conda.anaconda.org/conda-forge/osx-64/astroid-2.15.5-py310h2ec42d9_0.conda#6f8c825da6f4eedc532a6d102220d0e0
+https://conda.anaconda.org/conda-forge/osx-64/astroid-2.15.6-py310h2ec42d9_0.conda#2812b75db400abe651a33b99a7173ee6
 https://conda.anaconda.org/conda-forge/noarch/async-timeout-4.0.2-pyhd8ed1ab_0.tar.bz2#25e79f9a1133556671becbd65a170c78
 https://conda.anaconda.org/conda-forge/osx-64/brotlipy-0.7.0-py310h90acd4f_1005.tar.bz2#63accc45f2b9ae1dad4db9cdfaa903b4
-https://conda.anaconda.org/conda-forge/osx-64/cryptography-41.0.1-py310ha1817de_0.conda#f66541237ec50c9d89228ded177b8d65
+https://conda.anaconda.org/conda-forge/osx-64/cryptography-41.0.2-py310ha1817de_0.conda#f7f258c457df7e0617c2b92e24a7b47f
 https://conda.anaconda.org/conda-forge/noarch/ghp-import-2.1.0-pyhd8ed1ab_0.tar.bz2#6d8d61116031a3f5b1f32e7899785866
-https://conda.anaconda.org/conda-forge/osx-64/gstreamer-1.22.4-h840fbdc_0.conda#a24d0265742fe6614ca8d1186c0d8a42
+https://conda.anaconda.org/conda-forge/osx-64/gstreamer-1.22.4-h840fbdc_1.conda#659321735840756bc2c6ba7195ed9d8b
 https://conda.anaconda.org/conda-forge/osx-64/harfbuzz-6.0.0-h08f8713_0.conda#3852d6ef7b77da3e81074a8e487e7df5
-https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-6.7.0-hd8ed1ab_0.conda#27a4cec373ec84d1c1aa02a1e37f8eaf
+https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-6.8.0-hd8ed1ab_0.conda#b279b07ce18058034e5b3606ba103a8b
 https://conda.anaconda.org/conda-forge/noarch/jsonschema-4.17.3-pyhd8ed1ab_0.conda#723268a468177cd44568eb8f794e0d80
 https://conda.anaconda.org/conda-forge/noarch/jupyter_server_terminals-0.4.4-pyhd8ed1ab_1.conda#7c0965e1d4a0ee1529e8eaa03a78a5b3
 https://conda.anaconda.org/conda-forge/osx-64/libitk-5.3.0-h10ab89a_0.conda#73b9bad009f8759bd1854cbc6deca726
 https://conda.anaconda.org/conda-forge/osx-64/liblapacke-3.9.0-17_osx64_mkl.conda#678af3918e54ac46249290a05e7e69b1
 https://conda.anaconda.org/conda-forge/osx-64/libnetcdf-4.8.1-nompi_hc61b76e_106.tar.bz2#502e31e4a400216854da4e9933fb21c2
 https://conda.anaconda.org/conda-forge/noarch/markdown-3.4.3-pyhd8ed1ab_0.conda#89ed59ad509c05db6f5f2f573d499bfe
 https://conda.anaconda.org/conda-forge/noarch/mdit-py-plugins-0.4.0-pyhd8ed1ab_0.conda#6c5358a10873a15398b6f15f60cb5e1f
-https://conda.anaconda.org/conda-forge/osx-64/numpy-1.25.0-py310h7451ae0_0.conda#9accbca17b11eed20ee32b57189e9e66
-https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.8.0-pyhd8ed1ab_0.conda#3e4aca765371893ad848397794600632
+https://conda.anaconda.org/conda-forge/osx-64/numpy-1.25.1-py310h7451ae0_0.conda#525db32fd93b63f2f7ca3ece8576b9c8
+https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.9.1-pyhd8ed1ab_0.conda#044e7a1e0ad42c4e67110bd078150a63
 https://conda.anaconda.org/conda-forge/noarch/pybtex-0.24.0-pyhd8ed1ab_2.tar.bz2#2099b86a7399c44c0c61cdb6de6915ba
 https://conda.anaconda.org/conda-forge/osx-64/pyobjc-framework-cocoa-9.2-py310hef2d279_0.conda#0874355241e82a01cd15c6e6b28c7187
 https://conda.anaconda.org/conda-forge/osx-64/pyqt5-sip-12.11.0-py310h415000c_3.conda#6c56916bf99c55b1f57a53ed689f2561
 https://conda.anaconda.org/conda-forge/noarch/python-build-0.10.0-pyhd8ed1ab_1.conda#0ab47ce574f6a8bcb9f2076436e7fedb
 https://conda.anaconda.org/conda-forge/noarch/setuptools-scm-7.1.0-pyhd8ed1ab_0.conda#6613dbb3b25cc648a107f33ca9f80fc1
-https://conda.anaconda.org/conda-forge/osx-64/sqlalchemy-2.0.17-py310h6729b98_0.conda#2f7579944d2f1b682ad79c1de277368f
+https://conda.anaconda.org/conda-forge/osx-64/sqlalchemy-2.0.19-py310h6729b98_0.conda#9560749662f11f766ce19db9fa6271a4
 https://conda.anaconda.org/conda-forge/noarch/stack_data-0.6.2-pyhd8ed1ab_0.conda#e7df0fdd404616638df5ece6e69ba7af
 https://conda.anaconda.org/conda-forge/noarch/sympy-1.12-pypyh9d50eac_103.conda#2f7d6347d7acf6edf1ac7f2189f44c8f
 https://conda.anaconda.org/conda-forge/noarch/wcwidth-0.2.6-pyhd8ed1ab_0.conda#078979d33523cb477bd1916ce41aacc9
-https://conda.anaconda.org/conda-forge/osx-64/aiohttp-3.8.4-py310h6729b98_1.conda#513a7cdaa184e2856c358a57205d3837
+https://conda.anaconda.org/conda-forge/osx-64/aiohttp-3.8.5-py310h6729b98_0.conda#b91a4b8a80ba83d20ed0eabcc6949ebc
 https://conda.anaconda.org/conda-forge/noarch/argon2-cffi-21.3.0-pyhd8ed1ab_0.tar.bz2#a0b402db58f73aaab8ee0ca1025a362e
 https://conda.anaconda.org/conda-forge/noarch/black-22.3.0-pyhd8ed1ab_0.tar.bz2#7ecbfaae9a30b73c1a6e36e4a0debc03
 https://conda.anaconda.org/conda-forge/osx-64/blas-devel-3.9.0-17_osx64_mkl.conda#b40b415e2be4d0d2a8d05d0f805240b7
 https://conda.anaconda.org/conda-forge/osx-64/contourpy-1.1.0-py310h88cfcbd_0.conda#0cfd4a8d0f1d785675d5e41e17c8b122
-https://conda.anaconda.org/conda-forge/osx-64/gst-plugins-base-1.22.4-hb5d3a86_0.conda#3ddc9bb14daecff3a86233f07e0d472a
+https://conda.anaconda.org/conda-forge/osx-64/gst-plugins-base-1.22.4-hb5d3a86_1.conda#504bc1e992fc2d59e55cbd0102e117b0
 https://conda.anaconda.org/conda-forge/osx-64/jupyter_core-5.3.1-py310h2ec42d9_0.conda#2df6b800f29e805b1453a5a32981b873
 https://conda.anaconda.org/conda-forge/noarch/jupyter_events-0.6.3-pyhd8ed1ab_0.conda#d98c5196ab6ffeb0c2feca2912801353
+https://conda.anaconda.org/conda-forge/osx-64/nibabel-5.1.0-py310h2ec42d9_2.conda#04ba9603c2c52981e403da2295df8bc5
 https://conda.anaconda.org/conda-forge/noarch/oauthlib-3.2.2-pyhd8ed1ab_0.tar.bz2#8f882b197fd9c4941a787926baea4868
 https://conda.anaconda.org/conda-forge/osx-64/pandas-1.5.3-py310hecf8f37_1.conda#116e61ed90d0332d30310b2210eb1db4
 https://conda.anaconda.org/conda-forge/osx-64/pango-1.50.14-hbd9bf65_0.conda#7de54d83e9c685b742e0a4d81b271de0
 https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.39-pyha770c72_0.conda#a4986c6bb5b0d05a38855b0880a5f425
 https://conda.anaconda.org/conda-forge/osx-64/pybtex-docutils-1.0.2-py310h2ec42d9_2.tar.bz2#7dac3c5087b676102bf38bd984499219
 https://conda.anaconda.org/conda-forge/noarch/pyopenssl-23.2.0-pyhd8ed1ab_1.conda#34f7d568bf59d18e3fef8c405cbece21
 https://conda.anaconda.org/conda-forge/noarch/send2trash-1.8.2-pyhd1c38e8_0.conda#2657c3de5371c571aef6678afb4aaadd
 https://conda.anaconda.org/conda-forge/osx-64/simpleitk-2.2.1-py310h4447650_1.conda#ca28f25ff59b4907686307195de35927
 https://conda.anaconda.org/conda-forge/osx-64/blas-2.117-mkl.conda#4c921079b5298ce08bb336fc025b96d7
 https://conda.anaconda.org/conda-forge/noarch/flake8-black-0.3.6-pyhd8ed1ab_0.conda#61649e6e9b39ac0c7d10938025f6fe4f
 https://conda.anaconda.org/conda-forge/osx-64/gtk2-2.24.33-h7c1209e_2.tar.bz2#307614630946527e302b7dd042a5cfa2
 https://conda.anaconda.org/conda-forge/noarch/jupyter_client-8.3.0-pyhd8ed1ab_0.conda#1d018ee4ab13217e2544f795eb0a6798
 https://conda.anaconda.org/conda-forge/osx-64/librsvg-2.54.4-h3d48ba6_0.tar.bz2#1a106d9119086f73b5f88c650f700210
-https://conda.anaconda.org/conda-forge/osx-64/matplotlib-base-3.7.1-py310he725631_0.conda#8b1caf6e250a7c8270711c301d8bcd2e
-https://conda.anaconda.org/conda-forge/noarch/nbformat-5.9.0-pyhd8ed1ab_0.conda#f525a01528c3eba1d381a232a6971c6a
+https://conda.anaconda.org/conda-forge/osx-64/matplotlib-base-3.7.2-py310h475a17b_0.conda#ffc8dbf00f18c1ca9d3c02854cb72aee
+https://conda.anaconda.org/conda-forge/noarch/nbformat-5.9.1-pyhd8ed1ab_0.conda#3ec35d84fc1775215061517eb4660693
 https://conda.anaconda.org/conda-forge/noarch/prompt_toolkit-3.0.39-hd8ed1ab_0.conda#4bbbe67d5df19db30f04b8e344dc9976
 https://conda.anaconda.org/conda-forge/osx-64/qt-main-5.15.8-h1d3b3f8_6.conda#5d816352174169f7ab45fb54a0fba4ed
 https://conda.anaconda.org/conda-forge/noarch/urllib3-1.26.15-pyhd8ed1ab_0.conda#27db656619a55d727eaf5a6ece3d2fd6
 https://conda.anaconda.org/conda-forge/noarch/wslink-1.11.1-pyhd8ed1ab_0.conda#0d0113b67472cea3da288838ebc80acb
 https://conda.anaconda.org/conda-forge/noarch/botocore-1.29.165-pyhd8ed1ab_0.conda#0f30016ea54215fdb883b8978340c9b7
 https://conda.anaconda.org/conda-forge/osx-64/graphviz-7.0.5-hc51f7b9_0.conda#589501e7b16648c032a537b6a0870dbe
 https://conda.anaconda.org/conda-forge/noarch/ipython-8.14.0-pyhd1c38e8_0.conda#f56fab4cea853c2248105b6cd7d79bf0
-https://conda.anaconda.org/conda-forge/osx-64/matplotlib-3.7.1-py310h2ec42d9_0.conda#958029c1236746d27149fca648c41cab
+https://conda.anaconda.org/conda-forge/osx-64/matplotlib-3.7.2-py310h2ec42d9_0.conda#4fe2e1daa542b330507af9a2ca079d1c
 https://conda.anaconda.org/conda-forge/noarch/nbclient-0.7.4-pyhd8ed1ab_0.conda#f7aa15f77d29b11caa1df1eb15383c59
 https://conda.anaconda.org/conda-forge/osx-64/pyqt-5.15.7-py310hdd03f62_3.conda#c652959992036327b71a2d5ff593cf72
 https://conda.anaconda.org/pytorch/osx-64/pytorch-2.0.1-py3.10_0.tar.bz2#527aa8793c545ed93288d32bb45d009d
 https://conda.anaconda.org/conda-forge/noarch/requests-2.31.0-pyhd8ed1ab_0.conda#a30144e4156cdbb236f99ebb49828f8b
 https://conda.anaconda.org/conda-forge/osx-64/vtk-9.2.5-qt_py310hea5b068_200.conda#8210705bd78317d38a376b01f6cfab46
-https://conda.anaconda.org/conda-forge/noarch/google-auth-2.21.0-pyh1a96a4e_0.conda#8c5dd8609d314721d990c1d1fd607f81
+https://conda.anaconda.org/conda-forge/noarch/google-auth-2.22.0-pyh1a96a4e_0.conda#5583192796d1ebcf39b1e3e0958aa259
 https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.23.3-pyh5fb750a_0.conda#00cfe411a8e07b8322185e573ae7c5a3
 https://conda.anaconda.org/conda-forge/noarch/jupyter-cache-0.6.1-pyhd8ed1ab_0.conda#2e360820ae68e3d28e1a5a9d2714ca5c
-https://conda.anaconda.org/conda-forge/noarch/nbconvert-core-7.6.0-pyhd8ed1ab_0.conda#879782bde4bbdb4c7b5d4054504a20d5
+https://conda.anaconda.org/conda-forge/noarch/nbconvert-core-7.7.1-pyhd8ed1ab_1.conda#32dde1678bb003c90d4bc0c2dbd21814
 https://conda.anaconda.org/conda-forge/noarch/pooch-1.7.0-pyha770c72_3.conda#5936894aade8240c867d292aa0d980c6
 https://conda.anaconda.org/conda-forge/noarch/requests-oauthlib-1.3.1-pyhd8ed1ab_0.tar.bz2#61b279f051eef9c89d58f4d813e75e04
 https://conda.anaconda.org/conda-forge/noarch/s3transfer-0.6.1-pyhd8ed1ab_0.conda#b19a857ac845097e9c823c9f4d35f80e
 https://conda.anaconda.org/conda-forge/noarch/sphinx-4.5.0-pyh6c4a22f_0.tar.bz2#46b38d88c4270ff9ba78a89c83c66345
 https://conda.anaconda.org/conda-forge/noarch/torchinfo-1.8.0-pyhd8ed1ab_0.conda#fba98fc95a945e2a6b93a77b39dd52dc
 https://conda.anaconda.org/conda-forge/noarch/torchmetrics-0.11.4-pyhd8ed1ab_0.conda#480cb2b6d502003e937d9e4326bc398f
 https://conda.anaconda.org/pytorch/osx-64/torchvision-0.15.2-py310_cpu.tar.bz2#5c3600915df5413045fc3335c7b66ece
 https://conda.anaconda.org/conda-forge/noarch/boto3-1.26.165-pyhd8ed1ab_0.conda#b9a6316db67d5f2c8dbac2aeb24c6803
 https://conda.anaconda.org/conda-forge/noarch/google-auth-oauthlib-1.0.0-pyhd8ed1ab_1.conda#569e62e95b01b53e4ec7d9abe83b7385
 https://conda.anaconda.org/conda-forge/noarch/ipywidgets-8.0.7-pyhd8ed1ab_0.conda#4b0f4e8fe2a303e472674eae0340bdad
 https://conda.anaconda.org/conda-forge/noarch/jupyter_console-6.6.3-pyhd8ed1ab_0.conda#7cf6f52a66f8e3cd9d8b6c231262dcab
 https://conda.anaconda.org/conda-forge/noarch/jupyter_server-2.7.0-pyhd8ed1ab_0.conda#7488cd1f4d35a2af96faa765b7e5b2f0
 https://conda.anaconda.org/conda-forge/noarch/myst-parser-0.18.1-pyhd8ed1ab_0.tar.bz2#bcfdf5c7d8bf5c6f6be7b4c66fff2eca
-https://conda.anaconda.org/conda-forge/noarch/nbconvert-pandoc-7.6.0-pyhd8ed1ab_0.conda#e8172ca42f2869bb90185c9356899e81
+https://conda.anaconda.org/conda-forge/noarch/nbconvert-pandoc-7.7.1-pyhd8ed1ab_1.conda#796b056965d7146bcac082fa2a83943d
 https://conda.anaconda.org/conda-forge/noarch/pydata-sphinx-theme-0.13.3-pyhd8ed1ab_0.conda#07aca5f2dea315dcc16680d6891e9056
 https://conda.anaconda.org/conda-forge/noarch/pytorch-lightning-2.0.4-pyhd8ed1ab_0.conda#ce9d626b181c6f8cceb5047f6a819f7d
 https://conda.anaconda.org/conda-forge/noarch/qtconsole-base-5.4.3-pyha770c72_0.conda#e0f5e8a6f9ea248e5c2d23efffff08f7
 https://conda.anaconda.org/conda-forge/osx-64/scipy-1.10.1-py310h3900cf1_3.conda#02fb6b5a4f5a89fecae4a11d6bc4a0b1
 https://conda.anaconda.org/conda-forge/noarch/sphinx-comments-0.0.3-pyh9f0ad1d_0.tar.bz2#2ae3ce35de0c1cec45c94182694f8d1b
 https://conda.anaconda.org/conda-forge/noarch/sphinx-copybutton-0.5.2-pyhd8ed1ab_0.conda#ac832cc43adc79118cf6e23f1f9b8995
 https://conda.anaconda.org/conda-forge/noarch/sphinx-design-0.3.0-pyhd8ed1ab_0.tar.bz2#83d1a712e6d2bab6b298b1d2f42ad355
@@ -378,15 +381,15 @@
 https://conda.anaconda.org/conda-forge/noarch/sphinx-thebe-0.2.1-pyhd8ed1ab_0.conda#8a4151bde2af98c6cbc42ee12b48eb7f
 https://conda.anaconda.org/conda-forge/noarch/sphinx-togglebutton-0.3.2-pyhd8ed1ab_0.tar.bz2#382738101934261ea7931d1460e64868
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-bibtex-2.5.0-pyhd8ed1ab_0.tar.bz2#b2e5c9aece936ebf9f26abdf71ddd74b
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-dotnetdomain-0.4-py_0.tar.bz2#fb61a7369f505b4bb98e1530c3e09f9f
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-golangdomain-0.2.0.dev0-py_0.tar.bz2#d1a73c192888d08cedec232602c22f32
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-jquery-4.1-pyhd8ed1ab_0.conda#914897066d5873acfb13e75705276ad1
 https://conda.anaconda.org/conda-forge/noarch/myst-nb-0.17.2-pyhd8ed1ab_0.conda#40190b7d06f86b63d28fa78aaa39c023
-https://conda.anaconda.org/conda-forge/noarch/nbconvert-7.6.0-pyhd8ed1ab_0.conda#59976ee8df1c6f82c4aa94b5fd6b745e
+https://conda.anaconda.org/conda-forge/noarch/nbconvert-7.7.1-pyhd8ed1ab_1.conda#95d9d1523df069792cd059f412be0d6e
 https://conda.anaconda.org/conda-forge/noarch/notebook-shim-0.2.3-pyhd8ed1ab_0.conda#67e0fe74c156267d9159e9133df7fd37
 https://conda.anaconda.org/conda-forge/noarch/qtconsole-5.4.3-pyhd8ed1ab_0.conda#3777f933bec5113d5a292de10b03d0f6
 https://conda.anaconda.org/conda-forge/noarch/sphinx-autoapi-2.1.0-pyhd8ed1ab_0.conda#6cb2b182390f837ce98737e92b9461f7
 https://conda.anaconda.org/conda-forge/noarch/sphinx-book-theme-1.0.1-pyhd8ed1ab_0.conda#1ef419576de2c51b6e3a5a393eb35cda
 https://conda.anaconda.org/conda-forge/noarch/sphinx_rtd_theme-1.2.2-pyha770c72_0.conda#5ef6aaf2cfb3b656cdadb431daed6a9f
 https://conda.anaconda.org/conda-forge/noarch/tensorboard-2.13.0-pyhd8ed1ab_0.conda#321151b2405f11ec6681a9a6f30822b4
 https://conda.anaconda.org/conda-forge/noarch/jupyter-book-0.15.1-pyhd8ed1ab_0.conda#f10d556d3b3dc0aeae6aee37c412ea60
```

### Comparing `hf-deepali-0.3.2/conda/environment.osx-64.yml` & `hf-deepali-0.4.0/conda/environment.osx-64.yml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Generated by conda-lock.
 # platform: osx-64
-# input_hash: 1664d2c199c9cddb402252a38f5527d218754e954cbb25a82da7fecc8cbae3f6
+# input_hash: 533a7567b393584157366e71374225596e814fe74cfcb03642d3b4e184d58c87
 
 channels:
   - conda-forge
   - pytorch
   - nvidia
   - nodefaults
 dependencies:
@@ -47,15 +47,15 @@
   - x264=1!164.3095=h775f41a_2
   - xorg-libxau=1.0.11=h0dc2134_0
   - xorg-libxdmcp=1.1.3=h35c211d_0
   - xz=5.2.6=h775f41a_0
   - yaml=0.2.5=h0d85af4_2
   - aom=3.5.0=hf0c8a7f_0
   - double-conversion=3.2.0=hf0c8a7f_1
-  - eigen=3.4.0=h940c156_0
+  - eigen=3.4.1=h1c7c39f_0
   - expat=2.5.0=hf0c8a7f_1
   - fonts-conda-forge=1=0
   - gettext=0.21.1=h8a4c099_0
   - glew=2.1.0=h046ec9c_2
   - gmp=6.2.1=h2e338ed_0
   - graphite2=1.3.13=h2e338ed_1001
   - icu=70.1=h96cf925_0
@@ -85,35 +85,35 @@
   - readline=8.2=h9e318b2_1
   - svt-av1=1.4.1=hf0c8a7f_0
   - tbb=2021.9.0=hb8565cd_0
   - tk=8.6.12=h5dbffcc_0
   - x265=3.5=hbb4e6a2_3
   - zeromq=4.3.4=he49afe7_1
   - zlib=1.2.13=h8a1eda9_5
-  - zstd=1.5.2=hbc0c0cd_6
+  - zstd=1.5.2=h829000d_7
   - brotli-bin=1.0.9=hb7f2c08_9
   - fonts-conda-ecosystem=1=0
   - freetype=2.12.1=h3f81eb7_1
   - gl2ps=1.4.2=h4cff582_0
   - hdf4=4.2.15=h7aa5921_5
   - krb5=1.20.1=h049b76e_0
   - libclang=13.0.1=default_h255f2f3_1
   - libgfortran=5.0.0=11_3_0_h97931a8_31
-  - libglib=2.76.3=hc62aa5d_0
+  - libglib=2.76.4=hc62aa5d_0
   - libidn2=2.3.4=hb7f2c08_0
   - libnghttp2=1.52.0=he2ab024_0
   - libprotobuf=4.23.3=h5feb325_0
   - libssh2=1.11.0=hd019ec5_0
   - libtheora=1.1.1=h0d85af4_1005
   - libtiff=4.4.0=h6268bbc_5
   - libxml2=2.10.3=h201ad9d_4
   - libzip=1.9.2=h6db710c_1
   - mkl=2022.1.0=h860c996_928
   - mpfr=4.2.0=h4f9bd69_0
-  - mysql-common=8.0.33=hc6116ba_1
+  - mysql-common=8.0.33=hc6116ba_2
   - nss=3.89=h78b00b3_0
   - python=3.10.12=had23ca6_0_cpython
   - sqlite=3.42.0=h2b0dec6_0
   - tbb-devel=2021.9.0=hb8565cd_0
   - absl-py=1.4.0=pyhd8ed1ab_0
   - alabaster=0.7.13=pyhd8ed1ab_0
   - appnope=0.1.3=pyhd8ed1ab_0
@@ -121,93 +121,94 @@
   - attrs=21.4.0=pyhd8ed1ab_0
   - backcall=0.2.0=pyh9f0ad1d_0
   - backports=1.0=pyhd8ed1ab_3
   - blinker=1.6.2=pyhd8ed1ab_0
   - brotli=1.0.9=hb7f2c08_9
   - cachetools=5.3.1=pyhd8ed1ab_0
   - certifi=2023.5.7=pyhd8ed1ab_0
-  - charset-normalizer=3.1.0=pyhd8ed1ab_0
-  - click=8.1.3=unix_pyhd8ed1ab_2
+  - charset-normalizer=3.2.0=pyhd8ed1ab_0
+  - click=8.1.6=unix_pyh707e725_0
   - colorama=0.4.6=pyhd8ed1ab_0
   - cycler=0.11.0=pyhd8ed1ab_0
   - dataclasses=0.8=pyhc8e2a94_3
   - debugpy=1.6.7=py310h7a76584_0
   - decorator=5.1.1=pyhd8ed1ab_0
   - defusedxml=0.7.1=pyhd8ed1ab_0
   - docutils=0.17.1=py310h2ec42d9_3
   - entrypoints=0.4=pyhd8ed1ab_0
   - exceptiongroup=1.1.2=pyhd8ed1ab_0
   - executing=1.2.0=pyhd8ed1ab_0
   - fftw=3.3.10=nompi_h4fa670e_108
   - filelock=3.12.2=pyhd8ed1ab_0
   - flit-core=3.9.0=pyhd8ed1ab_0
   - fontconfig=2.14.2=h5bb23bf_0
-  - frozenlist=1.3.3=py310h90acd4f_0
+  - frozenlist=1.4.0=py310h6729b98_0
   - fsspec=2023.6.0=pyh1a96a4e_0
   - gdk-pixbuf=2.42.8=h3648f77_1
-  - glib-tools=2.76.3=h7d26f99_0
+  - glib-tools=2.76.4=h7d26f99_0
   - gnutls=3.7.8=h207c4f0_0
   - greenlet=2.0.2=py310h9e9d8ca_1
   - gts=0.7.6=h53e17e3_4
   - idna=3.4=pyhd8ed1ab_0
   - imagesize=1.4.1=pyhd8ed1ab_0
   - iniconfig=2.0.0=pyhd8ed1ab_0
   - ipython_genutils=0.2.0=py_1
   - jmespath=1.0.1=pyhd8ed1ab_0
   - jupyterlab_widgets=3.0.8=pyhd8ed1ab_0
   - kiwisolver=1.4.4=py310ha23aa8a_1
   - lazy-object-proxy=1.9.0=py310h90acd4f_0
   - lcms2=2.14=h90f4b2a_0
   - libblas=3.9.0=17_osx64_mkl
   - libcurl=8.1.2=hbee3ae8_0
-  - libgrpc=1.56.0=he6801ca_2
+  - libgrpc=1.56.2=he6801ca_0
   - libpq=15.3=h9dc22bb_1
   - libwebp=1.2.4=hfa4350a_0
   - loguru=0.7.0=py310h2ec42d9_0
   - markupsafe=2.1.3=py310h6729b98_0
   - mccabe=0.7.0=pyhd8ed1ab_0
   - mdurl=0.1.0=pyhd8ed1ab_0
   - mistune=3.0.0=pyhd8ed1ab_0
   - mkl-devel=2022.1.0=h694c41f_929
   - mpc=1.3.1=h81bd1dd_0
   - mpmath=1.3.0=pyhd8ed1ab_0
   - multidict=6.0.4=py310h90acd4f_0
   - munkres=1.1.4=pyh9f0ad1d_0
   - mypy_extensions=1.0.0=pyha770c72_0
-  - mysql-libs=8.0.33=haa61052_1
+  - mysql-libs=8.0.33=haa61052_2
   - nest-asyncio=1.5.6=pyhd8ed1ab_0
   - networkx=3.1=pyhd8ed1ab_0
   - openjpeg=2.5.0=h5d0d7b0_1
   - packaging=23.1=pyhd8ed1ab_0
   - pandocfilters=1.5.0=pyhd8ed1ab_0
   - parso=0.8.3=pyhd8ed1ab_0
   - pathspec=0.11.1=pyhd8ed1ab_0
   - pickleshare=0.7.5=py_1003
   - pkgutil-resolve-name=1.3.10=pyhd8ed1ab_0
   - pluggy=1.2.0=pyhd8ed1ab_0
   - ply=3.11=py_1
-  - prometheus_client=0.17.0=pyhd8ed1ab_0
+  - prometheus_client=0.17.1=pyhd8ed1ab_0
   - psutil=5.9.5=py310h90acd4f_0
   - ptyprocess=0.7.0=pyhd3deb0d_0
   - pure_eval=0.2.2=pyhd8ed1ab_0
   - pyasn1=0.4.8=py_0
   - pycodestyle=2.10.0=pyhd8ed1ab_0
   - pycparser=2.21=pyhd8ed1ab_0
   - pyflakes=3.0.1=pyhd8ed1ab_0
   - pygments=2.15.1=pyhd8ed1ab_0
-  - pyjwt=2.7.0=pyhd8ed1ab_0
-  - pyparsing=3.1.0=pyhd8ed1ab_0
+  - pyjwt=2.8.0=pyhd8ed1ab_0
+  - pyparsing=3.0.9=pyhd8ed1ab_0
   - pyrsistent=0.19.3=py310h90acd4f_0
   - pysocks=1.7.1=pyha2e5f31_6
   - python-fastjsonschema=2.17.1=pyhd8ed1ab_0
   - python-json-logger=2.0.7=pyhd8ed1ab_0
   - pytz=2023.3=pyhd8ed1ab_0
   - pyyaml=6.0=py310h90acd4f_5
   - pyzmq=25.1.0=py310h998be00_0
   - rfc3986-validator=0.1.1=pyh9f0ad1d_0
+  - ruamel.yaml.clib=0.2.7=py310h90acd4f_1
   - setuptools=67.7.2=pyhd8ed1ab_0
   - six=1.16.0=pyh6c4a22f_0
   - sniffio=1.3.0=pyhd8ed1ab_0
   - snowballstemmer=2.2.0=pyhd8ed1ab_0
   - soupsieve=2.3.2.post1=pyhd8ed1ab_0
   - sphinxcontrib-applehelp=1.0.4=pyhd8ed1ab_0
   - sphinxcontrib-devhelp=1.0.2=py_0
@@ -218,48 +219,48 @@
   - tabulate=0.9.0=pyhd8ed1ab_1
   - tensorboard-data-server=0.7.0=py310hdd0c95c_0
   - toml=0.10.2=pyhd8ed1ab_0
   - tomli=2.0.1=pyhd8ed1ab_0
   - tornado=6.3.2=py310h6729b98_0
   - traitlets=5.9.0=pyhd8ed1ab_0
   - typed-ast=1.5.4=py310h90acd4f_1
-  - typing_extensions=4.6.3=pyha770c72_0
+  - typing_extensions=4.7.1=pyha770c72_0
   - typing_utils=0.1.0=pyhd8ed1ab_0
   - uc-micro-py=1.0.1=pyhd8ed1ab_0
   - unicodedata2=15.0.0=py310h90acd4f_0
   - unidecode=1.3.6=pyhd8ed1ab_0
   - webencodings=0.5.1=py_1
   - websocket-client=1.6.1=pyhd8ed1ab_0
-  - wheel=0.40.0=pyhd8ed1ab_0
+  - wheel=0.40.0=pyhd8ed1ab_1
   - widgetsnbextension=4.0.8=pyhd8ed1ab_0
   - wrapt=1.15.0=py310h90acd4f_0
-  - zipp=3.15.0=pyhd8ed1ab_0
+  - zipp=3.16.2=pyhd8ed1ab_0
   - accessible-pygments=0.0.4=pyhd8ed1ab_0
   - aiosignal=1.3.1=pyhd8ed1ab_0
-  - anyio=3.7.0=pyhd8ed1ab_1
+  - anyio=3.7.1=pyhd8ed1ab_0
   - asttokens=2.2.1=pyhd8ed1ab_0
   - babel=2.12.1=pyhd8ed1ab_1
   - backports.functools_lru_cache=1.6.5=pyhd8ed1ab_0
   - beautifulsoup4=4.12.2=pyha770c72_0
   - bleach=6.0.0=pyhd8ed1ab_0
   - cairo=1.16.0=h904041c_1014
   - cffi=1.15.1=py310ha78151a_3
   - comm=0.1.3=pyhd8ed1ab_0
   - curl=8.1.2=hbee3ae8_0
   - dacite=1.8.0=pyhd8ed1ab_0
   - deprecation=2.1.0=pyh9f0ad1d_0
   - ffmpeg=5.1.2=gpl_h8b4fe81_106
   - flake8=6.0.0=pyhd8ed1ab_0
-  - fonttools=4.40.0=py310h6729b98_0
-  - glib=2.76.3=h7d26f99_0
+  - fonttools=4.41.0=py310h6729b98_0
+  - glib=2.76.4=h7d26f99_0
   - gmpy2=2.1.2=py310hb691cb2_1
-  - grpcio=1.56.0=py310h0d4bf3c_2
+  - grpcio=1.56.2=py310h0d4bf3c_0
   - hdf5=1.12.2=nompi_h48135f9_101
-  - importlib-metadata=6.7.0=pyha770c72_0
-  - importlib_resources=5.12.0=pyhd8ed1ab_0
+  - importlib-metadata=6.8.0=pyha770c72_0
+  - importlib_resources=6.0.0=pyhd8ed1ab_1
   - jedi=0.18.2=pyhd8ed1ab_0
   - jinja2=3.1.2=pyhd8ed1ab_1
   - jupyterlab_pygments=0.2.2=pyhd8ed1ab_0
   - latexcodec=2.0.1=pyh9f0ad1d_0
   - libcblas=3.9.0=17_osx64_mkl
   - libgd=2.3.3=h1e214de_3
   - liblapack=3.9.0=17_osx64_mkl
@@ -278,102 +279,104 @@
   - pyproject_hooks=1.0.0=pyhd8ed1ab_0
   - pytest=7.3.2=pyhd8ed1ab_1
   - python-dateutil=2.8.2=pyhd8ed1ab_0
   - pyu2f=0.1.5=pyhd8ed1ab_0
   - qtpy=2.3.1=pyhd8ed1ab_0
   - rfc3339-validator=0.1.4=pyhd8ed1ab_0
   - rsa=4.9=pyhd8ed1ab_0
+  - ruamel.yaml=0.17.32=py310h6729b98_0
   - sip=6.7.9=py310h9e9d8ca_0
   - terminado=0.17.1=pyhd1c38e8_0
   - tinycss2=1.2.1=pyhd8ed1ab_0
   - tqdm=4.65.0=pyhd8ed1ab_1
-  - typing-extensions=4.6.3=hd8ed1ab_0
+  - typing-extensions=4.7.1=hd8ed1ab_0
   - werkzeug=2.3.6=pyhd8ed1ab_0
   - yarl=1.9.2=py310h6729b98_0
   - argon2-cffi-bindings=21.2.0=py310h90acd4f_3
-  - astroid=2.15.5=py310h2ec42d9_0
+  - astroid=2.15.6=py310h2ec42d9_0
   - async-timeout=4.0.2=pyhd8ed1ab_0
   - brotlipy=0.7.0=py310h90acd4f_1005
-  - cryptography=41.0.1=py310ha1817de_0
+  - cryptography=41.0.2=py310ha1817de_0
   - ghp-import=2.1.0=pyhd8ed1ab_0
-  - gstreamer=1.22.4=h840fbdc_0
+  - gstreamer=1.22.4=h840fbdc_1
   - harfbuzz=6.0.0=h08f8713_0
-  - importlib_metadata=6.7.0=hd8ed1ab_0
+  - importlib_metadata=6.8.0=hd8ed1ab_0
   - jsonschema=4.17.3=pyhd8ed1ab_0
   - jupyter_server_terminals=0.4.4=pyhd8ed1ab_1
   - libitk=5.3.0=h10ab89a_0
   - liblapacke=3.9.0=17_osx64_mkl
   - libnetcdf=4.8.1=nompi_hc61b76e_106
   - markdown=3.4.3=pyhd8ed1ab_0
   - mdit-py-plugins=0.4.0=pyhd8ed1ab_0
-  - numpy=1.25.0=py310h7451ae0_0
-  - platformdirs=3.8.0=pyhd8ed1ab_0
+  - numpy=1.25.1=py310h7451ae0_0
+  - platformdirs=3.9.1=pyhd8ed1ab_0
   - pybtex=0.24.0=pyhd8ed1ab_2
   - pyobjc-framework-cocoa=9.2=py310hef2d279_0
   - pyqt5-sip=12.11.0=py310h415000c_3
   - python-build=0.10.0=pyhd8ed1ab_1
   - setuptools-scm=7.1.0=pyhd8ed1ab_0
-  - sqlalchemy=2.0.17=py310h6729b98_0
+  - sqlalchemy=2.0.19=py310h6729b98_0
   - stack_data=0.6.2=pyhd8ed1ab_0
   - sympy=1.12=pypyh9d50eac_103
   - wcwidth=0.2.6=pyhd8ed1ab_0
-  - aiohttp=3.8.4=py310h6729b98_1
+  - aiohttp=3.8.5=py310h6729b98_0
   - argon2-cffi=21.3.0=pyhd8ed1ab_0
   - black=22.3.0=pyhd8ed1ab_0
   - blas-devel=3.9.0=17_osx64_mkl
   - contourpy=1.1.0=py310h88cfcbd_0
-  - gst-plugins-base=1.22.4=hb5d3a86_0
+  - gst-plugins-base=1.22.4=hb5d3a86_1
   - jupyter_core=5.3.1=py310h2ec42d9_0
   - jupyter_events=0.6.3=pyhd8ed1ab_0
+  - nibabel=5.1.0=py310h2ec42d9_2
   - oauthlib=3.2.2=pyhd8ed1ab_0
   - pandas=1.5.3=py310hecf8f37_1
   - pango=1.50.14=hbd9bf65_0
   - prompt-toolkit=3.0.39=pyha770c72_0
   - pybtex-docutils=1.0.2=py310h2ec42d9_2
   - pyopenssl=23.2.0=pyhd8ed1ab_1
   - send2trash=1.8.2=pyhd1c38e8_0
   - simpleitk=2.2.1=py310h4447650_1
   - blas=2.117=mkl
   - flake8-black=0.3.6=pyhd8ed1ab_0
   - gtk2=2.24.33=h7c1209e_2
   - jupyter_client=8.3.0=pyhd8ed1ab_0
   - librsvg=2.54.4=h3d48ba6_0
-  - matplotlib-base=3.7.1=py310he725631_0
-  - nbformat=5.9.0=pyhd8ed1ab_0
+  - matplotlib-base=3.7.2=py310h475a17b_0
+  - nbformat=5.9.1=pyhd8ed1ab_0
   - prompt_toolkit=3.0.39=hd8ed1ab_0
   - qt-main=5.15.8=h1d3b3f8_6
   - urllib3=1.26.15=pyhd8ed1ab_0
   - wslink=1.11.1=pyhd8ed1ab_0
   - botocore=1.29.165=pyhd8ed1ab_0
   - graphviz=7.0.5=hc51f7b9_0
   - ipython=8.14.0=pyhd1c38e8_0
-  - matplotlib=3.7.1=py310h2ec42d9_0
+  - matplotlib=3.7.2=py310h2ec42d9_0
   - nbclient=0.7.4=pyhd8ed1ab_0
   - pyqt=5.15.7=py310hdd03f62_3
   - pytorch=2.0.1=py3.10_0
   - requests=2.31.0=pyhd8ed1ab_0
   - vtk=9.2.5=qt_py310hea5b068_200
-  - google-auth=2.21.0=pyh1a96a4e_0
+  - google-auth=2.22.0=pyh1a96a4e_0
   - ipykernel=6.23.3=pyh5fb750a_0
   - jupyter-cache=0.6.1=pyhd8ed1ab_0
-  - nbconvert-core=7.6.0=pyhd8ed1ab_0
+  - nbconvert-core=7.7.1=pyhd8ed1ab_1
   - pooch=1.7.0=pyha770c72_3
   - requests-oauthlib=1.3.1=pyhd8ed1ab_0
   - s3transfer=0.6.1=pyhd8ed1ab_0
   - sphinx=4.5.0=pyh6c4a22f_0
   - torchinfo=1.8.0=pyhd8ed1ab_0
   - torchmetrics=0.11.4=pyhd8ed1ab_0
   - torchvision=0.15.2=py310_cpu
   - boto3=1.26.165=pyhd8ed1ab_0
   - google-auth-oauthlib=1.0.0=pyhd8ed1ab_1
   - ipywidgets=8.0.7=pyhd8ed1ab_0
   - jupyter_console=6.6.3=pyhd8ed1ab_0
   - jupyter_server=2.7.0=pyhd8ed1ab_0
   - myst-parser=0.18.1=pyhd8ed1ab_0
-  - nbconvert-pandoc=7.6.0=pyhd8ed1ab_0
+  - nbconvert-pandoc=7.7.1=pyhd8ed1ab_1
   - pydata-sphinx-theme=0.13.3=pyhd8ed1ab_0
   - pytorch-lightning=2.0.4=pyhd8ed1ab_0
   - qtconsole-base=5.4.3=pyha770c72_0
   - scipy=1.10.1=py310h3900cf1_3
   - sphinx-comments=0.0.3=pyh9f0ad1d_0
   - sphinx-copybutton=0.5.2=pyhd8ed1ab_0
   - sphinx-design=0.3.0=pyhd8ed1ab_0
@@ -384,15 +387,15 @@
   - sphinx-thebe=0.2.1=pyhd8ed1ab_0
   - sphinx-togglebutton=0.3.2=pyhd8ed1ab_0
   - sphinxcontrib-bibtex=2.5.0=pyhd8ed1ab_0
   - sphinxcontrib-dotnetdomain=0.4=py_0
   - sphinxcontrib-golangdomain=0.2.0.dev0=py_0
   - sphinxcontrib-jquery=4.1=pyhd8ed1ab_0
   - myst-nb=0.17.2=pyhd8ed1ab_0
-  - nbconvert=7.6.0=pyhd8ed1ab_0
+  - nbconvert=7.7.1=pyhd8ed1ab_1
   - notebook-shim=0.2.3=pyhd8ed1ab_0
   - qtconsole=5.4.3=pyhd8ed1ab_0
   - sphinx-autoapi=2.1.0=pyhd8ed1ab_0
   - sphinx-book-theme=1.0.1=pyhd8ed1ab_0
   - sphinx_rtd_theme=1.2.2=pyha770c72_0
   - tensorboard=2.13.0=pyhd8ed1ab_0
   - jupyter-book=0.15.1=pyhd8ed1ab_0
```

### Comparing `hf-deepali-0.3.2/conda/environment.win-64.lock` & `hf-deepali-0.4.0/conda/environment.win-64.lock`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Generated by conda-lock.
 # platform: win-64
-# input_hash: fe02ca598f6ebbae4e65d2a2d45af1db4913dae4b25d021473f905afc52e3198
+# input_hash: 6255d416b6866feefaa84cbaf27b3a7608f8bb60e8d5e51ca00574e0f3970f20
 @EXPLICIT
 https://conda.anaconda.org/conda-forge/win-64/ca-certificates-2023.5.7-h56e8100_0.conda#604212634bd8c4d6f20d44b946e8eedb
 https://conda.anaconda.org/conda-forge/win-64/cuda-cccl-impl-2.0.1-h57928b3_0.conda#6ddbe275ebb9ae875355baf8ade34b3f
 https://conda.anaconda.org/nvidia/win-64/cuda-cudart-11.8.89-0.tar.bz2#cd0f6ab42e0ccba5f6899c531ea193c1
 https://conda.anaconda.org/nvidia/win-64/cuda-cupti-11.8.87-0.tar.bz2#f18f6268a222d476c804d4adadd4926a
 https://conda.anaconda.org/nvidia/win-64/cuda-nvrtc-11.8.89-0.tar.bz2#d692bd090a4a9638ac15709cde2400da
 https://conda.anaconda.org/nvidia/win-64/cuda-nvtx-11.8.86-0.tar.bz2#7874207353c834d34217555785859dba
@@ -52,15 +52,15 @@
 https://conda.anaconda.org/conda-forge/win-64/vs2015_runtime-14.36.32532-h05e6639_17.conda#4618046c39f7c81861e53ded842e738a
 https://conda.anaconda.org/conda-forge/win-64/aom-3.5.0-h63175ca_0.tar.bz2#455524d2bf9625a42a1848c0d08ac063
 https://conda.anaconda.org/conda-forge/win-64/bzip2-1.0.8-h8ffe710_4.tar.bz2#7c03c66026944073040cb19a4f3ec3c9
 https://conda.anaconda.org/conda-forge/win-64/c-ares-1.19.1-hcfcfb64_0.conda#8aa74d9a74ed3a31d9ed38a387a8ca50
 https://conda.anaconda.org/nvidia/win-64/cuda-cudart-dev-11.8.89-0.tar.bz2#a4b0b3a1b7aa79ff39f6d3b1e7c62de3
 https://conda.anaconda.org/conda-forge/win-64/dav1d-1.2.0-hcfcfb64_0.conda#0ce7020bd3aadfb999f987d2b1cc0e25
 https://conda.anaconda.org/conda-forge/win-64/double-conversion-3.2.0-h63175ca_1.tar.bz2#d1b86ea3cf6e902694a592e6440b1fa5
-https://conda.anaconda.org/conda-forge/win-64/eigen-3.4.0-h2d74725_0.tar.bz2#72fab4b0a033b718950cc5d930cbd1a6
+https://conda.anaconda.org/conda-forge/win-64/eigen-3.4.1-h91493d7_0.conda#3671ee2bcd1d915690de5b1445fdf004
 https://conda.anaconda.org/conda-forge/win-64/fftw-3.3.10-nompi_h38027f0_108.conda#09196a7ba69b70d2124aff7b2763035d
 https://conda.anaconda.org/conda-forge/win-64/fribidi-1.0.10-h8d14728_0.tar.bz2#807e81d915f2bb2e49951648615241f6
 https://conda.anaconda.org/conda-forge/win-64/getopt-win32-0.1-h8ffe710_0.tar.bz2#9ac4874e2958f18e01c386649208fe40
 https://conda.anaconda.org/conda-forge/win-64/glew-2.1.0-h39d44d4_2.tar.bz2#840d21c1ee66b91af3d0211e7766393a
 https://conda.anaconda.org/conda-forge/win-64/graphite2-1.3.13-1000.tar.bz2#8fc0e04e5c852cadf2cad68b86a906ab
 https://conda.anaconda.org/conda-forge/win-64/icu-70.1-h0e60522_0.tar.bz2#64073396a905b6df895ab2489fae3847
 https://conda.anaconda.org/conda-forge/win-64/jpeg-9e-hcfcfb64_3.conda#824f1e030d224e9e376a4655032fdbc7
@@ -111,25 +111,25 @@
 https://conda.anaconda.org/conda-forge/win-64/libzip-1.9.2-h519de47_1.tar.bz2#9c3138e53e36c0c161a23d20db91297b
 https://conda.anaconda.org/conda-forge/win-64/m2w64-gcc-libs-5.3.0-7.tar.bz2#fe759119b8b3bfa720b8762c6fdc35de
 https://conda.anaconda.org/conda-forge/win-64/pcre2-10.40-h17e33f8_0.tar.bz2#2519de0d9620dc2bc7e19caf6867136d
 https://conda.anaconda.org/conda-forge/win-64/python-3.10.12-h4de0772_0_cpython.conda#14273454ca348a123ce09ab9d39c1a6e
 https://conda.anaconda.org/conda-forge/win-64/sqlite-3.42.0-hcfcfb64_0.conda#c505cc64dba674d4c419c0de772c8579
 https://conda.anaconda.org/conda-forge/win-64/zeromq-4.3.4-h0e60522_1.tar.bz2#e1aff0583dda5fb917eb3d2c1025aa80
 https://conda.anaconda.org/conda-forge/win-64/zlib-1.2.13-hcfcfb64_5.conda#a318e8622e11663f645cc7fa3260f462
-https://conda.anaconda.org/conda-forge/win-64/zstd-1.5.2-h12be248_6.conda#62826565682d013b3e2346aaf7bded0e
+https://conda.anaconda.org/conda-forge/win-64/zstd-1.5.2-h12be248_7.conda#f3c3879d8cda1c5a6885435dd48a470e
 https://conda.anaconda.org/conda-forge/noarch/absl-py-1.4.0-pyhd8ed1ab_0.conda#dd5eed01874c75bebef810a2faec673e
 https://conda.anaconda.org/conda-forge/noarch/alabaster-0.7.13-pyhd8ed1ab_0.conda#06006184e203b61d3525f90de394471e
 https://conda.anaconda.org/conda-forge/noarch/attrs-21.4.0-pyhd8ed1ab_0.tar.bz2#f70280205d7044c8b8358c8de3190e5d
 https://conda.anaconda.org/conda-forge/noarch/backcall-0.2.0-pyh9f0ad1d_0.tar.bz2#6006a6d08a3fa99268a2681c7fb55213
 https://conda.anaconda.org/conda-forge/noarch/backports-1.0-pyhd8ed1ab_3.conda#54ca2e08b3220c148a1d8329c2678e02
 https://conda.anaconda.org/conda-forge/noarch/blinker-1.6.2-pyhd8ed1ab_0.conda#2fb79ec81bad9492b6d59a06b3b647a4
 https://conda.anaconda.org/conda-forge/win-64/brotli-bin-1.0.9-hcfcfb64_9.conda#ba8ae6c24cf47da3fb73270e4f119f08
 https://conda.anaconda.org/conda-forge/noarch/cachetools-5.3.1-pyhd8ed1ab_0.conda#60b5eb16d9a7a5482ba37f67aa49db5b
 https://conda.anaconda.org/conda-forge/noarch/certifi-2023.5.7-pyhd8ed1ab_0.conda#5d1b71c942b8421285934dad1d891ebc
-https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-3.1.0-pyhd8ed1ab_0.conda#7fcff9f6f123696e940bda77bd4d6551
+https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-3.2.0-pyhd8ed1ab_0.conda#313516e9a4b08b12dfb1e1cd390a96e3
 https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.6-pyhd8ed1ab_0.tar.bz2#3faab06a954c2a04039983f2c4a50d99
 https://conda.anaconda.org/nvidia/win-64/cuda-libraries-dev-11.8.0-0.tar.bz2#4dceddb905013e47bee99757d42dfdd4
 https://conda.anaconda.org/nvidia/win-64/cuda-runtime-11.8.0-0.tar.bz2#9782ebd2dc96d2fd463c0d4a99254da6
 https://conda.anaconda.org/conda-forge/noarch/cycler-0.11.0-pyhd8ed1ab_0.tar.bz2#a50559fad0affdbb33729a68669ca1cb
 https://conda.anaconda.org/conda-forge/noarch/dataclasses-0.8-pyhc8e2a94_3.tar.bz2#a362b2124b06aad102e2ee4581acee7d
 https://conda.anaconda.org/conda-forge/win-64/debugpy-1.6.7-py310h00ffb61_0.conda#b7defb941402f3581384d16070ed1456
 https://conda.anaconda.org/conda-forge/noarch/decorator-5.1.1-pyhd8ed1ab_0.tar.bz2#43afe5ab04e35e17ba28649471dd7364
@@ -137,31 +137,31 @@
 https://conda.anaconda.org/conda-forge/win-64/docutils-0.17.1-py310h5588dad_3.tar.bz2#cdc0acfc953b7bd34229b7f229eae46a
 https://conda.anaconda.org/conda-forge/noarch/entrypoints-0.4-pyhd8ed1ab_0.tar.bz2#3cf04868fee0a029769bd41f4b2fbf2d
 https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.1.2-pyhd8ed1ab_0.conda#de4cb3384374e1411f0454edcf546cdb
 https://conda.anaconda.org/conda-forge/noarch/executing-1.2.0-pyhd8ed1ab_0.tar.bz2#4c1bc140e2be5c8ba6e3acab99e25c50
 https://conda.anaconda.org/conda-forge/noarch/filelock-3.12.2-pyhd8ed1ab_0.conda#53522ec72e6adae42bd373ef58357230
 https://conda.anaconda.org/conda-forge/noarch/flit-core-3.9.0-pyhd8ed1ab_0.conda#e8cfceef004266b259604c3faa2a0191
 https://conda.anaconda.org/conda-forge/win-64/freetype-2.12.1-h546665d_1.conda#1b513009cd012591f3fdc9e03a74ec0a
-https://conda.anaconda.org/conda-forge/win-64/frozenlist-1.3.3-py310h8d17308_0.tar.bz2#550271ca005a4c805cd7391cef008dc6
+https://conda.anaconda.org/conda-forge/win-64/frozenlist-1.4.0-py310h8d17308_0.conda#7eba3cb7b26fbaee485f63e84824c7cd
 https://conda.anaconda.org/conda-forge/noarch/fsspec-2023.6.0-pyh1a96a4e_0.conda#50ea2067ec92dfcc38b4f07992d7e235
 https://conda.anaconda.org/conda-forge/win-64/gl2ps-1.4.2-h0597ee9_0.tar.bz2#9f17f1b93f610b4bea2a256d528fe8f6
 https://conda.anaconda.org/conda-forge/win-64/greenlet-2.0.2-py310h00ffb61_1.conda#7535b10dbe0b5fbf63fede10a4f8666b
 https://conda.anaconda.org/conda-forge/win-64/hdf4-4.2.15-h1b1b6ef_5.tar.bz2#bfb6a2d82ef9a30455cc0900d89eed20
 https://conda.anaconda.org/conda-forge/noarch/idna-3.4-pyhd8ed1ab_0.tar.bz2#34272b248891bddccc64479f9a7fffed
 https://conda.anaconda.org/conda-forge/noarch/imagesize-1.4.1-pyhd8ed1ab_0.tar.bz2#7de5386c8fea29e76b303f37dde4c352
 https://conda.anaconda.org/conda-forge/noarch/iniconfig-2.0.0-pyhd8ed1ab_0.conda#f800d2da156d08e289b14e87e43c1ae5
 https://conda.anaconda.org/conda-forge/noarch/ipython_genutils-0.2.0-py_1.tar.bz2#5071c982548b3a20caf70462f04f5287
 https://conda.anaconda.org/conda-forge/noarch/jmespath-1.0.1-pyhd8ed1ab_0.tar.bz2#2cfa3e1cf3fb51bb9b17acc5b5e9ea11
 https://conda.anaconda.org/conda-forge/noarch/jupyterlab_widgets-3.0.8-pyhd8ed1ab_0.conda#2bc3ca2f7387af385dd06706b4fb2d35
 https://conda.anaconda.org/conda-forge/win-64/kiwisolver-1.4.4-py310h232114e_1.tar.bz2#c55fe943d5f212d49d27d08580f5a610
 https://conda.anaconda.org/conda-forge/win-64/lazy-object-proxy-1.9.0-py310h8d17308_0.conda#696baee03eafd09ed9c4ab6a095b620f
 https://conda.anaconda.org/conda-forge/win-64/libclang-15.0.7-default_h77d9078_2.conda#70188b1b3e0b1716405adab9050894d1
 https://conda.anaconda.org/conda-forge/win-64/libcurl-8.1.2-h68f0423_0.conda#94b9b7d0e882461fdb72d8d4e7441746
-https://conda.anaconda.org/conda-forge/win-64/libglib-2.76.3-he8f3873_0.conda#4695e6acaf4790170161048d56cb51fc
-https://conda.anaconda.org/conda-forge/win-64/libgrpc-1.56.0-hea2d5f7_2.conda#44b832412b9a71277e67ecc52ffec4f2
+https://conda.anaconda.org/conda-forge/win-64/libglib-2.76.4-he8f3873_0.conda#8c3f24acdc0403eeb3fb42ab75e8a659
+https://conda.anaconda.org/conda-forge/win-64/libgrpc-1.56.2-hea2d5f7_0.conda#240221f7a200e718c242637e6c437b61
 https://conda.anaconda.org/conda-forge/win-64/libhwloc-2.9.1-h51c2c0f_0.conda#8ec5920f3ed67faa0264a36c0b533ed0
 https://conda.anaconda.org/conda-forge/win-64/libtiff-4.4.0-hc4f729c_5.conda#fe00c2f95c1215e355c34094b00480d7
 https://conda.anaconda.org/conda-forge/win-64/markupsafe-2.1.3-py310h8d17308_0.conda#e6deeae9d0dac4d17c6ef2fa62b3efff
 https://conda.anaconda.org/conda-forge/noarch/mccabe-0.7.0-pyhd8ed1ab_0.tar.bz2#34fc335fc50eef0b5ea708f2b5f54e0c
 https://conda.anaconda.org/conda-forge/noarch/mdurl-0.1.0-pyhd8ed1ab_0.tar.bz2#f8dab71fdc13b1bf29a01248b156d268
 https://conda.anaconda.org/conda-forge/noarch/mistune-3.0.0-pyhd8ed1ab_0.conda#c7d0ea64c37752ecbe6da458aee662d2
 https://conda.anaconda.org/conda-forge/noarch/mpmath-1.3.0-pyhd8ed1ab_0.conda#dbf6e2d89137da32fa6670f3bffc024e
@@ -174,34 +174,35 @@
 https://conda.anaconda.org/conda-forge/noarch/pandocfilters-1.5.0-pyhd8ed1ab_0.tar.bz2#457c2c8c08e54905d6954e79cb5b5db9
 https://conda.anaconda.org/conda-forge/noarch/parso-0.8.3-pyhd8ed1ab_0.tar.bz2#17a565a0c3899244e938cdf417e7b094
 https://conda.anaconda.org/conda-forge/noarch/pathspec-0.11.1-pyhd8ed1ab_0.conda#dbb80d1e8dc2dba5c8b106dc0768ad45
 https://conda.anaconda.org/conda-forge/noarch/pickleshare-0.7.5-py_1003.tar.bz2#415f0ebb6198cc2801c73438a9fb5761
 https://conda.anaconda.org/conda-forge/noarch/pkgutil-resolve-name-1.3.10-pyhd8ed1ab_0.tar.bz2#89e3c7cdde7d3aaa2aee933b604dd07f
 https://conda.anaconda.org/conda-forge/noarch/pluggy-1.2.0-pyhd8ed1ab_0.conda#7263924c642d22e311d9e59b839f1b33
 https://conda.anaconda.org/conda-forge/noarch/ply-3.11-py_1.tar.bz2#7205635cd71531943440fbfe3b6b5727
-https://conda.anaconda.org/conda-forge/noarch/prometheus_client-0.17.0-pyhd8ed1ab_0.conda#95c5be3c7cbd872509d16c216617fdab
+https://conda.anaconda.org/conda-forge/noarch/prometheus_client-0.17.1-pyhd8ed1ab_0.conda#02153b6b760bbec00cfe9e4c97993d06
 https://conda.anaconda.org/conda-forge/win-64/psutil-5.9.5-py310h8d17308_0.conda#9f98965e4f7dc2e4eb84abd50406d3a0
 https://conda.anaconda.org/conda-forge/win-64/pthread-stubs-0.4-hcd874cb_1001.tar.bz2#a1f820480193ea83582b13249a7e7bd9
 https://conda.anaconda.org/conda-forge/noarch/pure_eval-0.2.2-pyhd8ed1ab_0.tar.bz2#6784285c7e55cb7212efabc79e4c2883
 https://conda.anaconda.org/conda-forge/noarch/pyasn1-0.4.8-py_0.tar.bz2#06d04c9f8f72ac77911db942eda24fb9
 https://conda.anaconda.org/conda-forge/noarch/pycodestyle-2.10.0-pyhd8ed1ab_0.conda#89843e4cc99c6a3fe5f4c86994cc8410
 https://conda.anaconda.org/conda-forge/noarch/pycparser-2.21-pyhd8ed1ab_0.tar.bz2#076becd9e05608f8dc72757d5f3a91ff
 https://conda.anaconda.org/conda-forge/noarch/pyflakes-3.0.1-pyhd8ed1ab_0.conda#44b7d77d96560c93e0e11437a3c35254
 https://conda.anaconda.org/conda-forge/noarch/pygments-2.15.1-pyhd8ed1ab_0.conda#d316679235612869eba305aa7d41d9bf
-https://conda.anaconda.org/conda-forge/noarch/pyjwt-2.7.0-pyhd8ed1ab_0.conda#99e28be5a278e2319834d7dc99e7bfdd
-https://conda.anaconda.org/conda-forge/noarch/pyparsing-3.1.0-pyhd8ed1ab_0.conda#d3ed087d1f7f8f5590e8e87b57a8ce64
+https://conda.anaconda.org/conda-forge/noarch/pyjwt-2.8.0-pyhd8ed1ab_0.conda#912c0194f898fdb783021fd25f913c31
+https://conda.anaconda.org/conda-forge/noarch/pyparsing-3.0.9-pyhd8ed1ab_0.tar.bz2#e8fbc1b54b25f4b08281467bc13b70cc
 https://conda.anaconda.org/conda-forge/win-64/pyrsistent-0.19.3-py310h8d17308_0.conda#ddba6aad7d1857d16675d41a6e8b0224
 https://conda.anaconda.org/conda-forge/noarch/python-fastjsonschema-2.17.1-pyhd8ed1ab_0.conda#dd4f393d857e9283eef2442234bd05e3
 https://conda.anaconda.org/conda-forge/noarch/python-json-logger-2.0.7-pyhd8ed1ab_0.conda#a61bf9ec79426938ff785eb69dbb1960
 https://conda.anaconda.org/conda-forge/noarch/pytz-2023.3-pyhd8ed1ab_0.conda#d3076b483092a435832603243567bc31
 https://conda.anaconda.org/conda-forge/win-64/pywin32-304-py310h00ffb61_2.tar.bz2#e1401844b4f4ec959e099452a953e764
-https://conda.anaconda.org/conda-forge/win-64/pywinpty-2.0.10-py310h00ffb61_0.conda#b0fb5ffdb72cb3b46bc9fdc163cf411d
+https://conda.anaconda.org/conda-forge/win-64/pywinpty-2.0.11-py310h00ffb61_0.conda#685cf7fe1b0724628476c991329017ad
 https://conda.anaconda.org/conda-forge/win-64/pyyaml-6.0-py310h8d17308_5.tar.bz2#d0daf3eed98dd2bf4337ed08d8011eb8
 https://conda.anaconda.org/conda-forge/win-64/pyzmq-25.1.0-py310hcd737a0_0.conda#75b926fbf2e2c67eb5210c68e1ac8f18
 https://conda.anaconda.org/conda-forge/noarch/rfc3986-validator-0.1.1-pyh9f0ad1d_0.tar.bz2#912a71cc01012ee38e6b90ddd561e36f
+https://conda.anaconda.org/conda-forge/win-64/ruamel.yaml.clib-0.2.7-py310h8d17308_1.conda#e7cee92d4b0e9f8a68823d2501a87063
 https://conda.anaconda.org/conda-forge/noarch/setuptools-67.7.2-pyhd8ed1ab_0.conda#3b68bc43ec6baa48f7354a446267eefe
 https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2#e5f25f8dbc060e9a8d912e432202afc2
 https://conda.anaconda.org/conda-forge/noarch/sniffio-1.3.0-pyhd8ed1ab_0.tar.bz2#dd6cbc539e74cb1f430efbd4575b9303
 https://conda.anaconda.org/conda-forge/noarch/snowballstemmer-2.2.0-pyhd8ed1ab_0.tar.bz2#4d22a9315e78c6827f806065957d566e
 https://conda.anaconda.org/conda-forge/noarch/soupsieve-2.3.2.post1-pyhd8ed1ab_0.tar.bz2#146f4541d643d48fc8a75cacf69f03ae
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-applehelp-1.0.4-pyhd8ed1ab_0.conda#5a31a7d564f551d0e6dff52fd8cb5b16
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-devhelp-1.0.2-py_0.tar.bz2#68e01cac9d38d0e717cd5c87bc3d2cc9
@@ -212,56 +213,56 @@
 https://conda.anaconda.org/conda-forge/noarch/tabulate-0.9.0-pyhd8ed1ab_1.tar.bz2#4759805cce2d914c38472f70bf4d8bcb
 https://conda.anaconda.org/conda-forge/win-64/tensorboard-data-server-0.7.0-py310h5588dad_0.conda#1aa33e391e578ec1f6b23d10e005aa2e
 https://conda.anaconda.org/conda-forge/noarch/toml-0.10.2-pyhd8ed1ab_0.tar.bz2#f832c45a477c78bebd107098db465095
 https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2#5844808ffab9ebdb694585b50ba02a96
 https://conda.anaconda.org/conda-forge/win-64/tornado-6.3.2-py310h8d17308_0.conda#6cd035ff75b46eb8ae7403b3dded2def
 https://conda.anaconda.org/conda-forge/noarch/traitlets-5.9.0-pyhd8ed1ab_0.conda#d0b4f5c87cd35ac3fb3d47b223263a64
 https://conda.anaconda.org/conda-forge/win-64/typed-ast-1.5.5-py310h8d17308_0.conda#a2ac0e6c5a06b35dea207c3d77f94f74
-https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.6.3-pyha770c72_0.conda#4a3014a4d107d15475d106b751c4e352
+https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.7.1-pyha770c72_0.conda#c39d6a09fe819de4951c2642629d9115
 https://conda.anaconda.org/conda-forge/noarch/typing_utils-0.1.0-pyhd8ed1ab_0.tar.bz2#eb67e3cace64c66233e2d35949e20f92
 https://conda.anaconda.org/conda-forge/noarch/uc-micro-py-1.0.1-pyhd8ed1ab_0.tar.bz2#3ddf6684d9b274a12c94e509ca45656c
 https://conda.anaconda.org/conda-forge/win-64/unicodedata2-15.0.0-py310h8d17308_0.tar.bz2#5d14ba562f7740b64be9c8059498cfbf
 https://conda.anaconda.org/conda-forge/noarch/unidecode-1.3.6-pyhd8ed1ab_0.tar.bz2#e8f24401b17802df5f82f66a88cee29e
 https://conda.anaconda.org/conda-forge/noarch/webencodings-0.5.1-py_1.tar.bz2#3563be4c5611a44210d9ba0c16113136
 https://conda.anaconda.org/conda-forge/noarch/websocket-client-1.6.1-pyhd8ed1ab_0.conda#c34d9325a609381a0b0e8a5b4f325147
-https://conda.anaconda.org/conda-forge/noarch/wheel-0.40.0-pyhd8ed1ab_0.conda#49bb0d9e60ce1db25e151780331bb5f3
+https://conda.anaconda.org/conda-forge/noarch/wheel-0.40.0-pyhd8ed1ab_1.conda#c95fac682453aeffa12db7ae5a721bec
 https://conda.anaconda.org/conda-forge/noarch/widgetsnbextension-4.0.8-pyhd8ed1ab_0.conda#2e9ebddf0b93d0fb203d0906b8052c4f
 https://conda.anaconda.org/conda-forge/noarch/win32_setctime-1.1.0-pyhd8ed1ab_0.tar.bz2#dc80c0c2b01f7d6d6d5df4b63ef54f17
 https://conda.anaconda.org/conda-forge/noarch/win_inet_pton-1.1.0-pyhd8ed1ab_6.tar.bz2#30878ecc4bd36e8deeea1e3c151b2e0b
 https://conda.anaconda.org/conda-forge/win-64/wrapt-1.15.0-py310h8d17308_0.conda#2ec4d850e6fbe1da9971a7bb801a1ebd
 https://conda.anaconda.org/conda-forge/win-64/xorg-kbproto-1.0.7-hcd874cb_1002.tar.bz2#8d11c1dac4756ca57e78c1bfe173bba4
 https://conda.anaconda.org/conda-forge/win-64/xorg-libice-1.0.10-hcd874cb_0.tar.bz2#8f45beee385cb67e42d6732bdb1b6a40
 https://conda.anaconda.org/conda-forge/win-64/xorg-libxau-1.0.11-hcd874cb_0.conda#c46ba8712093cb0114404ae8a7582e1a
 https://conda.anaconda.org/conda-forge/win-64/xorg-libxdmcp-1.1.3-hcd874cb_0.tar.bz2#46878ebb6b9cbd8afcf8088d7ef00ece
 https://conda.anaconda.org/conda-forge/win-64/xorg-xextproto-7.3.0-hcd874cb_1003.conda#6e6c2639620e436bddb7c040cd4f3adb
 https://conda.anaconda.org/conda-forge/win-64/xorg-xproto-7.0.31-hcd874cb_1007.tar.bz2#88f3c65d2ad13826a9e0b162063be023
-https://conda.anaconda.org/conda-forge/noarch/zipp-3.15.0-pyhd8ed1ab_0.conda#13018819ca8f5b7cc675a8faf1f5fedf
+https://conda.anaconda.org/conda-forge/noarch/zipp-3.16.2-pyhd8ed1ab_0.conda#2da0451b54c4563c32490cb1b7cf68a1
 https://conda.anaconda.org/conda-forge/noarch/accessible-pygments-0.0.4-pyhd8ed1ab_0.conda#46a2e6e3dfa718ce3492018d5a110dd6
 https://conda.anaconda.org/conda-forge/noarch/aiosignal-1.3.1-pyhd8ed1ab_0.tar.bz2#d1e1eb7e21a9e2c74279d87dafb68156
-https://conda.anaconda.org/conda-forge/noarch/anyio-3.7.0-pyhd8ed1ab_1.conda#2b35a85d654a47aac8f34c1bb6de7142
+https://conda.anaconda.org/conda-forge/noarch/anyio-3.7.1-pyhd8ed1ab_0.conda#7b517e7a6f0790337906c055aa97ca49
 https://conda.anaconda.org/conda-forge/noarch/asttokens-2.2.1-pyhd8ed1ab_0.conda#bf7f54dd0f25c3f06ecb82a07341841a
 https://conda.anaconda.org/conda-forge/noarch/babel-2.12.1-pyhd8ed1ab_1.conda#ac432e732804a81ddcf29c92ead57cde
 https://conda.anaconda.org/conda-forge/noarch/backports.functools_lru_cache-1.6.5-pyhd8ed1ab_0.conda#6b1b907661838a75d067a22f87996b2e
 https://conda.anaconda.org/conda-forge/noarch/beautifulsoup4-4.12.2-pyha770c72_0.conda#a362ff7d976217f8fa78c0f1c4f59717
 https://conda.anaconda.org/conda-forge/noarch/bleach-6.0.0-pyhd8ed1ab_0.conda#d48b143d01385872a88ef8417e96c30e
 https://conda.anaconda.org/conda-forge/win-64/brotli-1.0.9-hcfcfb64_9.conda#5275e2634840f6d156934a16b7c0c813
 https://conda.anaconda.org/conda-forge/win-64/cffi-1.15.1-py310h628cb3f_3.conda#b7ca236d34501eb6a70691c1e29a0234
-https://conda.anaconda.org/conda-forge/noarch/click-8.1.3-win_pyhd8ed1ab_2.tar.bz2#6b58680207b526c42dcff68b543803dd
+https://conda.anaconda.org/conda-forge/noarch/click-8.1.6-win_pyh7428d3b_0.conda#c1e57b6771510a3d2648ed6e76277391
 https://conda.anaconda.org/conda-forge/noarch/comm-0.1.3-pyhd8ed1ab_0.conda#168ae0f82cdf7505048e81054c7354e4
 https://conda.anaconda.org/conda-forge/win-64/curl-8.1.2-h68f0423_0.conda#fc67d347f9eaa7922fd7bc26bfa5419b
 https://conda.anaconda.org/conda-forge/noarch/dacite-1.8.0-pyhd8ed1ab_0.conda#3696792ba70ab3374320fe6041a82286
 https://conda.anaconda.org/conda-forge/noarch/deprecation-2.1.0-pyh9f0ad1d_0.tar.bz2#7b6747d7cc2076341029cff659669e8b
 https://conda.anaconda.org/conda-forge/noarch/flake8-6.0.0-pyhd8ed1ab_0.conda#e9345ba05d71742412b8aa6992ad9457
 https://conda.anaconda.org/conda-forge/win-64/fontconfig-2.14.2-hbde0cde_0.conda#08767992f1a4f1336a257af1241034bd
-https://conda.anaconda.org/conda-forge/win-64/glib-tools-2.76.3-h12be248_0.conda#3015483cb3ffa200d51aac3c691fcda0
-https://conda.anaconda.org/conda-forge/win-64/grpcio-1.56.0-py310hb84602e_2.conda#c624ac3dd1ada404b8d8cc378bb60daf
+https://conda.anaconda.org/conda-forge/win-64/glib-tools-2.76.4-h12be248_0.conda#88237d3ddd338164196043cb7e927246
+https://conda.anaconda.org/conda-forge/win-64/grpcio-1.56.2-py310hb84602e_0.conda#1c43b1323746f119bfea36e689930225
 https://conda.anaconda.org/conda-forge/win-64/gts-0.7.6-h6b5321d_4.conda#a41f14768d5e377426ad60c613f2923b
 https://conda.anaconda.org/conda-forge/win-64/hdf5-1.12.2-nompi_h57737ce_101.conda#3e2b84f2f7bcf6915d1baa21e5b1a862
-https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-6.7.0-pyha770c72_0.conda#ba3786c6846e46038fe60c785d46dc81
-https://conda.anaconda.org/conda-forge/noarch/importlib_resources-5.12.0-pyhd8ed1ab_0.conda#e5fd2260a231ee63b6969f4801082f2b
+https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-6.8.0-pyha770c72_0.conda#4e9f59a060c3be52bc4ddc46ee9b6946
+https://conda.anaconda.org/conda-forge/noarch/importlib_resources-6.0.0-pyhd8ed1ab_1.conda#a08b6be5bf18b9d2a927d3457750f82e
 https://conda.anaconda.org/conda-forge/noarch/jedi-0.18.2-pyhd8ed1ab_0.conda#b5e695ef9c3f0d27d6cd96bf5adc9e07
 https://conda.anaconda.org/conda-forge/noarch/jinja2-3.1.2-pyhd8ed1ab_1.tar.bz2#c8490ed5c70966d232fdd389d0dbed37
 https://conda.anaconda.org/conda-forge/noarch/jupyterlab_pygments-0.2.2-pyhd8ed1ab_0.tar.bz2#243f63592c8e449f40cd42eb5cf32f40
 https://conda.anaconda.org/conda-forge/noarch/latexcodec-2.0.1-pyh9f0ad1d_0.tar.bz2#8d67904973263afd2985ba56aa2d6bb4
 https://conda.anaconda.org/conda-forge/win-64/lcms2-2.14-h90d422f_0.tar.bz2#a0deec92aa16fca7bf5a6717d05f88ee
 https://conda.anaconda.org/conda-forge/win-64/libxcb-1.13-hcd874cb_1004.tar.bz2#a6d7fd030532378ecb6ba435cd9f8234
 https://conda.anaconda.org/conda-forge/noarch/lightning-utilities-0.9.0-pyhd8ed1ab_0.conda#c71f7ec8b80a536e58b979299b230251
@@ -280,112 +281,114 @@
 https://conda.anaconda.org/conda-forge/noarch/pytest-7.3.2-pyhd8ed1ab_1.conda#f2465696f4396245eca4613f6e924796
 https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.8.2-pyhd8ed1ab_0.tar.bz2#dd999d1cc9f79e67dbb855c8924c7984
 https://conda.anaconda.org/pytorch/win-64/pytorch-cuda-11.8-h24eeafa_5.tar.bz2#6c31007cf6837eac42629e117ef1d947
 https://conda.anaconda.org/conda-forge/noarch/pyu2f-0.1.5-pyhd8ed1ab_0.tar.bz2#caabbeaa83928d0c3e3949261daa18eb
 https://conda.anaconda.org/conda-forge/noarch/qtpy-2.3.1-pyhd8ed1ab_0.conda#10812eca3ec4ebaf3749e1960c208d43
 https://conda.anaconda.org/conda-forge/noarch/rfc3339-validator-0.1.4-pyhd8ed1ab_0.tar.bz2#fed45fc5ea0813240707998abe49f520
 https://conda.anaconda.org/conda-forge/noarch/rsa-4.9-pyhd8ed1ab_0.tar.bz2#03bf410858b2cefc267316408a77c436
+https://conda.anaconda.org/conda-forge/win-64/ruamel.yaml-0.17.32-py310h8d17308_0.conda#c13c515dcc8f25ea5407630e172ed83c
 https://conda.anaconda.org/conda-forge/noarch/send2trash-1.8.2-pyh08f2357_0.conda#c00d32dfa733d381b6a1908d0d67e0d7
 https://conda.anaconda.org/conda-forge/win-64/sip-6.7.9-py310h00ffb61_0.conda#a249b5eefc4c36146ade59e2b237b7fd
 https://conda.anaconda.org/conda-forge/noarch/sympy-1.12-pyh04b8f61_3.conda#6af285473a6a49ea8068e0b5b28ed7de
 https://conda.anaconda.org/conda-forge/win-64/tbb-2021.9.0-h91493d7_0.conda#6aa3f1becefeaa00a4d2a79b2a478aee
 https://conda.anaconda.org/conda-forge/noarch/terminado-0.17.0-pyh08f2357_0.tar.bz2#0152a609d5748ed9887d195b1e61a6c9
 https://conda.anaconda.org/conda-forge/noarch/tinycss2-1.2.1-pyhd8ed1ab_0.tar.bz2#7234c9eefff659501cd2fe0d2ede4d48
 https://conda.anaconda.org/conda-forge/noarch/tqdm-4.65.0-pyhd8ed1ab_1.conda#ed792aff3acb977d09c7013358097f83
-https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.6.3-hd8ed1ab_0.conda#3876f650ed7d0f95d70fa4b647621909
+https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.7.1-hd8ed1ab_0.conda#f96688577f1faa58096d06a45136afa2
 https://conda.anaconda.org/conda-forge/noarch/werkzeug-2.3.6-pyhd8ed1ab_0.conda#55fbbb3e67185820ee2007395bfe0073
 https://conda.anaconda.org/conda-forge/win-64/xorg-libsm-1.2.3-hcd874cb_1000.tar.bz2#76a765e735668a9922da3d58e746a7a6
 https://conda.anaconda.org/conda-forge/win-64/yarl-1.9.2-py310h8d17308_0.conda#0dfd2f264553d751449a0585d030adf7
 https://conda.anaconda.org/conda-forge/win-64/argon2-cffi-bindings-21.2.0-py310h8d17308_3.tar.bz2#3f6daa76891876a933722b5c9ee7dcaa
-https://conda.anaconda.org/conda-forge/win-64/astroid-2.15.5-py310h5588dad_0.conda#d8b37ae3e9ac63ddb024cea93df674aa
+https://conda.anaconda.org/conda-forge/win-64/astroid-2.15.6-py310h5588dad_0.conda#a1e30c9be3eb810b8efdd581449983cc
 https://conda.anaconda.org/conda-forge/noarch/async-timeout-4.0.2-pyhd8ed1ab_0.tar.bz2#25e79f9a1133556671becbd65a170c78
 https://conda.anaconda.org/conda-forge/win-64/brotlipy-0.7.0-py310h8d17308_1005.tar.bz2#6cb010e0fa21d7b606a13038a89ccbc2
 https://conda.anaconda.org/conda-forge/win-64/cairo-1.16.0-hd694305_1014.tar.bz2#91f08ed9ff25a969ddd06237454dae0d
-https://conda.anaconda.org/conda-forge/win-64/cryptography-41.0.1-py310h6e82f81_0.conda#dcd180d7b04ea819607366a35f323108
+https://conda.anaconda.org/conda-forge/win-64/cryptography-41.0.2-py310h6e82f81_0.conda#507f1964c07ee129d1317e601a2bfb94
 https://conda.anaconda.org/conda-forge/win-64/ffmpeg-5.1.2-gpl_h5037a79_109.conda#57b15431095a5632832088a38b7318b7
-https://conda.anaconda.org/conda-forge/win-64/fonttools-4.40.0-py310h8d17308_0.conda#a18e1160ee09a9f5ac26b2ce965832f7
+https://conda.anaconda.org/conda-forge/win-64/fonttools-4.41.0-py310h8d17308_0.conda#496704d1b32153ed96e60de270a3e2f4
 https://conda.anaconda.org/conda-forge/noarch/ghp-import-2.1.0-pyhd8ed1ab_0.tar.bz2#6d8d61116031a3f5b1f32e7899785866
-https://conda.anaconda.org/conda-forge/win-64/glib-2.76.3-h12be248_0.conda#fa3f1af2dc70e0d00a755667a741fad3
-https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-6.7.0-hd8ed1ab_0.conda#27a4cec373ec84d1c1aa02a1e37f8eaf
+https://conda.anaconda.org/conda-forge/win-64/glib-2.76.4-h12be248_0.conda#4d7ae53ee4b7e08f3fbd1d3a7efd4812
+https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-6.8.0-hd8ed1ab_0.conda#b279b07ce18058034e5b3606ba103a8b
 https://conda.anaconda.org/conda-forge/noarch/jsonschema-4.17.3-pyhd8ed1ab_0.conda#723268a468177cd44568eb8f794e0d80
 https://conda.anaconda.org/conda-forge/noarch/jupyter_server_terminals-0.4.4-pyhd8ed1ab_1.conda#7c0965e1d4a0ee1529e8eaa03a78a5b3
 https://conda.anaconda.org/conda-forge/win-64/libitk-5.3.0-h6e1890f_0.conda#705a9011eeac84184b34f157ca927ec0
 https://conda.anaconda.org/conda-forge/win-64/libnetcdf-4.8.1-nompi_h8c042bf_106.tar.bz2#90515eee0f7575b5fd296b6ba8d91dae
 https://conda.anaconda.org/conda-forge/noarch/markdown-3.4.3-pyhd8ed1ab_0.conda#89ed59ad509c05db6f5f2f573d499bfe
 https://conda.anaconda.org/conda-forge/noarch/mdit-py-plugins-0.4.0-pyhd8ed1ab_0.conda#6c5358a10873a15398b6f15f60cb5e1f
 https://conda.anaconda.org/conda-forge/win-64/mkl-2022.1.0-h6a75c08_874.tar.bz2#2ff89a7337a9636029b4db9466e9f8e3
 https://conda.anaconda.org/conda-forge/win-64/pillow-9.2.0-py310hd4fb230_3.tar.bz2#96a1ddd65392fb64636dd8311f862e14
-https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.8.0-pyhd8ed1ab_0.conda#3e4aca765371893ad848397794600632
+https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.9.1-pyhd8ed1ab_0.conda#044e7a1e0ad42c4e67110bd078150a63
 https://conda.anaconda.org/conda-forge/noarch/pybtex-0.24.0-pyhd8ed1ab_2.tar.bz2#2099b86a7399c44c0c61cdb6de6915ba
 https://conda.anaconda.org/conda-forge/win-64/pyqt5-sip-12.11.0-py310h00ffb61_3.conda#a4c757150f616bae079bc08cea956138
 https://conda.anaconda.org/conda-forge/noarch/python-build-0.10.0-pyhd8ed1ab_1.conda#0ab47ce574f6a8bcb9f2076436e7fedb
 https://conda.anaconda.org/conda-forge/noarch/setuptools-scm-7.1.0-pyhd8ed1ab_0.conda#6613dbb3b25cc648a107f33ca9f80fc1
-https://conda.anaconda.org/conda-forge/win-64/sqlalchemy-2.0.17-py310h8d17308_0.conda#1a7ef45ab2cbed2272dc7bed9ee6f98a
+https://conda.anaconda.org/conda-forge/win-64/sqlalchemy-2.0.19-py310h8d17308_0.conda#4cfc2aca9d88ef166474d84cb9c51451
 https://conda.anaconda.org/conda-forge/noarch/stack_data-0.6.2-pyhd8ed1ab_0.conda#e7df0fdd404616638df5ece6e69ba7af
 https://conda.anaconda.org/conda-forge/win-64/tbb-devel-2021.9.0-h91493d7_0.conda#ece1b712d5d6c96f916ec0f11e52b391
 https://conda.anaconda.org/conda-forge/noarch/wcwidth-0.2.6-pyhd8ed1ab_0.conda#078979d33523cb477bd1916ce41aacc9
 https://conda.anaconda.org/conda-forge/win-64/xorg-libx11-1.8.4-hcd874cb_0.conda#ebdb02b455647e13fa697da89d9bdf84
-https://conda.anaconda.org/conda-forge/win-64/aiohttp-3.8.4-py310h8d17308_1.conda#c759aad020f1363a27088e6c621f4db1
+https://conda.anaconda.org/conda-forge/win-64/aiohttp-3.8.5-py310h8d17308_0.conda#cb4d6c6556ca7dfad7f75b1b371ecb30
 https://conda.anaconda.org/conda-forge/noarch/argon2-cffi-21.3.0-pyhd8ed1ab_0.tar.bz2#a0b402db58f73aaab8ee0ca1025a362e
 https://conda.anaconda.org/conda-forge/noarch/black-22.3.0-pyhd8ed1ab_0.tar.bz2#7ecbfaae9a30b73c1a6e36e4a0debc03
-https://conda.anaconda.org/conda-forge/win-64/gstreamer-1.22.4-hb4038d2_0.conda#ead79af9af7587ca3f685fed4966a881
+https://conda.anaconda.org/conda-forge/win-64/gstreamer-1.22.4-hb4038d2_1.conda#42f53931331420f6b748f91ef356a558
 https://conda.anaconda.org/conda-forge/win-64/harfbuzz-6.0.0-he256f1b_0.conda#15422d4ff786ed835173cfb8e6735679
 https://conda.anaconda.org/conda-forge/win-64/jupyter_core-5.3.1-py310h5588dad_0.conda#39614170bdabdaa7531cb1dc2846c37c
 https://conda.anaconda.org/conda-forge/noarch/jupyter_events-0.6.3-pyhd8ed1ab_0.conda#d98c5196ab6ffeb0c2feca2912801353
 https://conda.anaconda.org/conda-forge/win-64/libblas-3.9.0-17_win64_mkl.conda#9e42ac6b256b96bfaa19f829c25940e8
 https://conda.anaconda.org/conda-forge/win-64/mkl-devel-2022.1.0-h57928b3_875.tar.bz2#6319a06307af296c1dfae93687c283b2
 https://conda.anaconda.org/conda-forge/noarch/oauthlib-3.2.2-pyhd8ed1ab_0.tar.bz2#8f882b197fd9c4941a787926baea4868
 https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.39-pyha770c72_0.conda#a4986c6bb5b0d05a38855b0880a5f425
 https://conda.anaconda.org/conda-forge/win-64/pybtex-docutils-1.0.2-py310h5588dad_2.tar.bz2#a69da1e6eb6ce9a7794d379a54e06990
 https://conda.anaconda.org/conda-forge/noarch/pyopenssl-23.2.0-pyhd8ed1ab_1.conda#34f7d568bf59d18e3fef8c405cbece21
 https://conda.anaconda.org/conda-forge/win-64/simpleitk-2.2.1-py310hcf936e6_1.conda#39ff6e62452d8ccdbc0bdfe8566932f5
 https://conda.anaconda.org/conda-forge/win-64/xorg-libxext-1.3.4-hcd874cb_2.conda#2aa695ac3c56193fd8d526e3b511e021
 https://conda.anaconda.org/conda-forge/win-64/xorg-libxt-1.3.0-hcd874cb_0.conda#f7db1a67cd97a9bd0f59ee6997a77159
 https://conda.anaconda.org/conda-forge/noarch/flake8-black-0.3.6-pyhd8ed1ab_0.conda#61649e6e9b39ac0c7d10938025f6fe4f
-https://conda.anaconda.org/conda-forge/win-64/gst-plugins-base-1.22.4-h001b923_0.conda#2c402e044af28ad8eccf03031c5c34c4
+https://conda.anaconda.org/conda-forge/win-64/gst-plugins-base-1.22.4-h001b923_1.conda#ce797dd3d60901f6260e84e84674c829
 https://conda.anaconda.org/conda-forge/noarch/jupyter_client-8.3.0-pyhd8ed1ab_0.conda#1d018ee4ab13217e2544f795eb0a6798
 https://conda.anaconda.org/conda-forge/win-64/libcblas-3.9.0-17_win64_mkl.conda#768b2c3be666ecf9e62f939ea919f819
 https://conda.anaconda.org/conda-forge/win-64/liblapack-3.9.0-17_win64_mkl.conda#278121fe8f0d65d496998aa290f36322
-https://conda.anaconda.org/conda-forge/noarch/nbformat-5.9.0-pyhd8ed1ab_0.conda#f525a01528c3eba1d381a232a6971c6a
+https://conda.anaconda.org/conda-forge/noarch/nbformat-5.9.1-pyhd8ed1ab_0.conda#3ec35d84fc1775215061517eb4660693
 https://conda.anaconda.org/conda-forge/win-64/pango-1.50.14-hdffb7b3_0.conda#a613f324e0f213238baec720d5c4ed00
 https://conda.anaconda.org/conda-forge/noarch/prompt_toolkit-3.0.39-hd8ed1ab_0.conda#4bbbe67d5df19db30f04b8e344dc9976
 https://conda.anaconda.org/conda-forge/noarch/urllib3-1.26.15-pyhd8ed1ab_0.conda#27db656619a55d727eaf5a6ece3d2fd6
 https://conda.anaconda.org/conda-forge/noarch/wslink-1.11.1-pyhd8ed1ab_0.conda#0d0113b67472cea3da288838ebc80acb
 https://conda.anaconda.org/conda-forge/win-64/xorg-libxpm-3.5.16-hcd874cb_0.conda#e74445e2a4ad70fc358ae2bf87c20f41
 https://conda.anaconda.org/conda-forge/noarch/botocore-1.29.165-pyhd8ed1ab_0.conda#0f30016ea54215fdb883b8978340c9b7
 https://conda.anaconda.org/conda-forge/noarch/ipython-8.14.0-pyh08f2357_0.conda#1fc684c1de5475383790ada5627c5430
 https://conda.anaconda.org/conda-forge/win-64/libgd-2.3.3-h891f43f_3.tar.bz2#0d66b24e1ba733a75df08e0af6f20be1
 https://conda.anaconda.org/conda-forge/win-64/liblapacke-3.9.0-17_win64_mkl.conda#6c98bb1c41479063f089459dcdedcecb
 https://conda.anaconda.org/conda-forge/noarch/nbclient-0.7.4-pyhd8ed1ab_0.conda#f7aa15f77d29b11caa1df1eb15383c59
-https://conda.anaconda.org/conda-forge/win-64/numpy-1.25.0-py310hd02465a_0.conda#63be5dd380067c6db32243e6ca56e8e8
+https://conda.anaconda.org/conda-forge/win-64/numpy-1.25.1-py310hd02465a_0.conda#922f75b8698c5b9909bf03c658898117
 https://conda.anaconda.org/conda-forge/win-64/qt-main-5.15.8-h720456b_6.conda#3047b05190091b66cf60017b8968a562
 https://conda.anaconda.org/conda-forge/noarch/requests-2.31.0-pyhd8ed1ab_0.conda#a30144e4156cdbb236f99ebb49828f8b
 https://conda.anaconda.org/conda-forge/win-64/blas-devel-3.9.0-17_win64_mkl.conda#bfcbcc96906ca944d944eb4ae340371a
 https://conda.anaconda.org/conda-forge/win-64/contourpy-1.1.0-py310h232114e_0.conda#4079a644cfc3b1fbd72571dc0a87ea33
-https://conda.anaconda.org/conda-forge/noarch/google-auth-2.21.0-pyh1a96a4e_0.conda#8c5dd8609d314721d990c1d1fd607f81
+https://conda.anaconda.org/conda-forge/noarch/google-auth-2.22.0-pyh1a96a4e_0.conda#5583192796d1ebcf39b1e3e0958aa259
 https://conda.anaconda.org/conda-forge/win-64/graphviz-7.0.6-h51cb2cd_0.conda#136eb298a1c96b07f935dd0525fbd11c
 https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.23.3-pyh6817e22_0.conda#b71d6766fc67ea676f75d121965da056
 https://conda.anaconda.org/conda-forge/noarch/jupyter-cache-0.6.1-pyhd8ed1ab_0.conda#2e360820ae68e3d28e1a5a9d2714ca5c
-https://conda.anaconda.org/conda-forge/noarch/nbconvert-core-7.6.0-pyhd8ed1ab_0.conda#879782bde4bbdb4c7b5d4054504a20d5
+https://conda.anaconda.org/conda-forge/noarch/nbconvert-core-7.7.1-pyhd8ed1ab_1.conda#32dde1678bb003c90d4bc0c2dbd21814
+https://conda.anaconda.org/conda-forge/win-64/nibabel-5.1.0-py310h5588dad_2.conda#9d814866ce7bef15844c53bf669a77d7
 https://conda.anaconda.org/conda-forge/win-64/pandas-1.5.3-py310h1c4a608_1.conda#3e3b61b47b88cf649025e67223bee77f
 https://conda.anaconda.org/conda-forge/noarch/pooch-1.7.0-pyha770c72_3.conda#5936894aade8240c867d292aa0d980c6
 https://conda.anaconda.org/conda-forge/win-64/pyqt-5.15.7-py310h1fd54f2_3.conda#4012c5ed74c63b82c344e38cf3e68a26
 https://conda.anaconda.org/conda-forge/noarch/requests-oauthlib-1.3.1-pyhd8ed1ab_0.tar.bz2#61b279f051eef9c89d58f4d813e75e04
 https://conda.anaconda.org/conda-forge/noarch/s3transfer-0.6.1-pyhd8ed1ab_0.conda#b19a857ac845097e9c823c9f4d35f80e
 https://conda.anaconda.org/conda-forge/noarch/sphinx-4.5.0-pyh6c4a22f_0.tar.bz2#46b38d88c4270ff9ba78a89c83c66345
 https://conda.anaconda.org/conda-forge/win-64/vtk-9.2.5-qt_py310h2fd250f_200.conda#fccf10ecfe3ea51109abdd5354071823
 https://conda.anaconda.org/conda-forge/win-64/blas-2.117-mkl.conda#a6b489be6ddbc3259df7cc8a440b8950
 https://conda.anaconda.org/conda-forge/noarch/boto3-1.26.165-pyhd8ed1ab_0.conda#b9a6316db67d5f2c8dbac2aeb24c6803
 https://conda.anaconda.org/conda-forge/noarch/google-auth-oauthlib-1.0.0-pyhd8ed1ab_1.conda#569e62e95b01b53e4ec7d9abe83b7385
 https://conda.anaconda.org/conda-forge/noarch/ipywidgets-8.0.7-pyhd8ed1ab_0.conda#4b0f4e8fe2a303e472674eae0340bdad
 https://conda.anaconda.org/conda-forge/noarch/jupyter_console-6.6.3-pyhd8ed1ab_0.conda#7cf6f52a66f8e3cd9d8b6c231262dcab
 https://conda.anaconda.org/conda-forge/noarch/jupyter_server-2.7.0-pyhd8ed1ab_0.conda#7488cd1f4d35a2af96faa765b7e5b2f0
-https://conda.anaconda.org/conda-forge/win-64/matplotlib-base-3.7.1-py310h51140c5_0.conda#d8c42a72d04ad1b93ba7269e9949738e
+https://conda.anaconda.org/conda-forge/win-64/matplotlib-base-3.7.2-py310h51140c5_0.conda#f485fd7d59c2719f79aa4323caa5f1e3
 https://conda.anaconda.org/conda-forge/noarch/myst-parser-0.18.1-pyhd8ed1ab_0.tar.bz2#bcfdf5c7d8bf5c6f6be7b4c66fff2eca
-https://conda.anaconda.org/conda-forge/noarch/nbconvert-pandoc-7.6.0-pyhd8ed1ab_0.conda#e8172ca42f2869bb90185c9356899e81
+https://conda.anaconda.org/conda-forge/noarch/nbconvert-pandoc-7.7.1-pyhd8ed1ab_1.conda#796b056965d7146bcac082fa2a83943d
 https://conda.anaconda.org/conda-forge/noarch/pydata-sphinx-theme-0.13.3-pyhd8ed1ab_0.conda#07aca5f2dea315dcc16680d6891e9056
 https://conda.anaconda.org/conda-forge/noarch/qtconsole-base-5.4.3-pyha770c72_0.conda#e0f5e8a6f9ea248e5c2d23efffff08f7
 https://conda.anaconda.org/conda-forge/win-64/scipy-1.10.1-py310h578b7cb_3.conda#d44c1bad75bb3e4d40066b3d3dd718ed
 https://conda.anaconda.org/conda-forge/noarch/sphinx-comments-0.0.3-pyh9f0ad1d_0.tar.bz2#2ae3ce35de0c1cec45c94182694f8d1b
 https://conda.anaconda.org/conda-forge/noarch/sphinx-copybutton-0.5.2-pyhd8ed1ab_0.conda#ac832cc43adc79118cf6e23f1f9b8995
 https://conda.anaconda.org/conda-forge/noarch/sphinx-design-0.3.0-pyhd8ed1ab_0.tar.bz2#83d1a712e6d2bab6b298b1d2f42ad355
 https://conda.anaconda.org/conda-forge/noarch/sphinx-external-toc-0.3.1-pyhd8ed1ab_0.conda#561bdf7b598d38e2962c46557bd1da12
@@ -394,17 +397,17 @@
 https://conda.anaconda.org/conda-forge/noarch/sphinx-notfound-page-0.8.3-pyhd8ed1ab_0.tar.bz2#6159b3d4402dc5746022e66c7ccd2b92
 https://conda.anaconda.org/conda-forge/noarch/sphinx-thebe-0.2.1-pyhd8ed1ab_0.conda#8a4151bde2af98c6cbc42ee12b48eb7f
 https://conda.anaconda.org/conda-forge/noarch/sphinx-togglebutton-0.3.2-pyhd8ed1ab_0.tar.bz2#382738101934261ea7931d1460e64868
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-bibtex-2.5.0-pyhd8ed1ab_0.tar.bz2#b2e5c9aece936ebf9f26abdf71ddd74b
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-dotnetdomain-0.4-py_0.tar.bz2#fb61a7369f505b4bb98e1530c3e09f9f
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-golangdomain-0.2.0.dev0-py_0.tar.bz2#d1a73c192888d08cedec232602c22f32
 https://conda.anaconda.org/conda-forge/noarch/sphinxcontrib-jquery-4.1-pyhd8ed1ab_0.conda#914897066d5873acfb13e75705276ad1
-https://conda.anaconda.org/conda-forge/win-64/matplotlib-3.7.1-py310h5588dad_0.conda#edfb6c85499499b014a09b8136e0fdbb
+https://conda.anaconda.org/conda-forge/win-64/matplotlib-3.7.2-py310h5588dad_0.conda#5059435ea4238f449ace9c04387433bd
 https://conda.anaconda.org/conda-forge/noarch/myst-nb-0.17.2-pyhd8ed1ab_0.conda#40190b7d06f86b63d28fa78aaa39c023
-https://conda.anaconda.org/conda-forge/noarch/nbconvert-7.6.0-pyhd8ed1ab_0.conda#59976ee8df1c6f82c4aa94b5fd6b745e
+https://conda.anaconda.org/conda-forge/noarch/nbconvert-7.7.1-pyhd8ed1ab_1.conda#95d9d1523df069792cd059f412be0d6e
 https://conda.anaconda.org/conda-forge/noarch/notebook-shim-0.2.3-pyhd8ed1ab_0.conda#67e0fe74c156267d9159e9133df7fd37
 https://conda.anaconda.org/pytorch/win-64/pytorch-2.0.1-py3.10_cuda11.8_cudnn8_0.tar.bz2#798f578b07f4a959d587c98dc922d051
 https://conda.anaconda.org/conda-forge/noarch/qtconsole-5.4.3-pyhd8ed1ab_0.conda#3777f933bec5113d5a292de10b03d0f6
 https://conda.anaconda.org/conda-forge/noarch/sphinx-autoapi-2.1.0-pyhd8ed1ab_0.conda#6cb2b182390f837ce98737e92b9461f7
 https://conda.anaconda.org/conda-forge/noarch/sphinx-book-theme-1.0.1-pyhd8ed1ab_0.conda#1ef419576de2c51b6e3a5a393eb35cda
 https://conda.anaconda.org/conda-forge/noarch/sphinx_rtd_theme-1.2.2-pyha770c72_0.conda#5ef6aaf2cfb3b656cdadb431daed6a9f
 https://conda.anaconda.org/conda-forge/noarch/tensorboard-2.13.0-pyhd8ed1ab_0.conda#321151b2405f11ec6681a9a6f30822b4
```

### Comparing `hf-deepali-0.3.2/conda/environment.win-64.yml` & `hf-deepali-0.4.0/conda/environment.win-64.yml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Generated by conda-lock.
 # platform: win-64
-# input_hash: fe02ca598f6ebbae4e65d2a2d45af1db4913dae4b25d021473f905afc52e3198
+# input_hash: 6255d416b6866feefaa84cbaf27b3a7608f8bb60e8d5e51ca00574e0f3970f20
 
 channels:
   - conda-forge
   - pytorch
   - nvidia
   - nodefaults
 dependencies:
@@ -58,15 +58,15 @@
   - vs2015_runtime=14.36.32532=h05e6639_17
   - aom=3.5.0=h63175ca_0
   - bzip2=1.0.8=h8ffe710_4
   - c-ares=1.19.1=hcfcfb64_0
   - cuda-cudart-dev=11.8.89=0
   - dav1d=1.2.0=hcfcfb64_0
   - double-conversion=3.2.0=h63175ca_1
-  - eigen=3.4.0=h2d74725_0
+  - eigen=3.4.1=h91493d7_0
   - fftw=3.3.10=nompi_h38027f0_108
   - fribidi=1.0.10=h8d14728_0
   - getopt-win32=0.1=h8ffe710_0
   - glew=2.1.0=h39d44d4_2
   - graphite2=1.3.13=1000
   - icu=70.1=h0e60522_0
   - jpeg=9e=hcfcfb64_3
@@ -117,25 +117,25 @@
   - libzip=1.9.2=h519de47_1
   - m2w64-gcc-libs=5.3.0=7
   - pcre2=10.40=h17e33f8_0
   - python=3.10.12=h4de0772_0_cpython
   - sqlite=3.42.0=hcfcfb64_0
   - zeromq=4.3.4=h0e60522_1
   - zlib=1.2.13=hcfcfb64_5
-  - zstd=1.5.2=h12be248_6
+  - zstd=1.5.2=h12be248_7
   - absl-py=1.4.0=pyhd8ed1ab_0
   - alabaster=0.7.13=pyhd8ed1ab_0
   - attrs=21.4.0=pyhd8ed1ab_0
   - backcall=0.2.0=pyh9f0ad1d_0
   - backports=1.0=pyhd8ed1ab_3
   - blinker=1.6.2=pyhd8ed1ab_0
   - brotli-bin=1.0.9=hcfcfb64_9
   - cachetools=5.3.1=pyhd8ed1ab_0
   - certifi=2023.5.7=pyhd8ed1ab_0
-  - charset-normalizer=3.1.0=pyhd8ed1ab_0
+  - charset-normalizer=3.2.0=pyhd8ed1ab_0
   - colorama=0.4.6=pyhd8ed1ab_0
   - cuda-libraries-dev=11.8.0=0
   - cuda-runtime=11.8.0=0
   - cycler=0.11.0=pyhd8ed1ab_0
   - dataclasses=0.8=pyhc8e2a94_3
   - debugpy=1.6.7=py310h00ffb61_0
   - decorator=5.1.1=pyhd8ed1ab_0
@@ -143,31 +143,31 @@
   - docutils=0.17.1=py310h5588dad_3
   - entrypoints=0.4=pyhd8ed1ab_0
   - exceptiongroup=1.1.2=pyhd8ed1ab_0
   - executing=1.2.0=pyhd8ed1ab_0
   - filelock=3.12.2=pyhd8ed1ab_0
   - flit-core=3.9.0=pyhd8ed1ab_0
   - freetype=2.12.1=h546665d_1
-  - frozenlist=1.3.3=py310h8d17308_0
+  - frozenlist=1.4.0=py310h8d17308_0
   - fsspec=2023.6.0=pyh1a96a4e_0
   - gl2ps=1.4.2=h0597ee9_0
   - greenlet=2.0.2=py310h00ffb61_1
   - hdf4=4.2.15=h1b1b6ef_5
   - idna=3.4=pyhd8ed1ab_0
   - imagesize=1.4.1=pyhd8ed1ab_0
   - iniconfig=2.0.0=pyhd8ed1ab_0
   - ipython_genutils=0.2.0=py_1
   - jmespath=1.0.1=pyhd8ed1ab_0
   - jupyterlab_widgets=3.0.8=pyhd8ed1ab_0
   - kiwisolver=1.4.4=py310h232114e_1
   - lazy-object-proxy=1.9.0=py310h8d17308_0
   - libclang=15.0.7=default_h77d9078_2
   - libcurl=8.1.2=h68f0423_0
-  - libglib=2.76.3=he8f3873_0
-  - libgrpc=1.56.0=hea2d5f7_2
+  - libglib=2.76.4=he8f3873_0
+  - libgrpc=1.56.2=hea2d5f7_0
   - libhwloc=2.9.1=h51c2c0f_0
   - libtiff=4.4.0=hc4f729c_5
   - markupsafe=2.1.3=py310h8d17308_0
   - mccabe=0.7.0=pyhd8ed1ab_0
   - mdurl=0.1.0=pyhd8ed1ab_0
   - mistune=3.0.0=pyhd8ed1ab_0
   - mpmath=1.3.0=pyhd8ed1ab_0
@@ -180,34 +180,35 @@
   - pandocfilters=1.5.0=pyhd8ed1ab_0
   - parso=0.8.3=pyhd8ed1ab_0
   - pathspec=0.11.1=pyhd8ed1ab_0
   - pickleshare=0.7.5=py_1003
   - pkgutil-resolve-name=1.3.10=pyhd8ed1ab_0
   - pluggy=1.2.0=pyhd8ed1ab_0
   - ply=3.11=py_1
-  - prometheus_client=0.17.0=pyhd8ed1ab_0
+  - prometheus_client=0.17.1=pyhd8ed1ab_0
   - psutil=5.9.5=py310h8d17308_0
   - pthread-stubs=0.4=hcd874cb_1001
   - pure_eval=0.2.2=pyhd8ed1ab_0
   - pyasn1=0.4.8=py_0
   - pycodestyle=2.10.0=pyhd8ed1ab_0
   - pycparser=2.21=pyhd8ed1ab_0
   - pyflakes=3.0.1=pyhd8ed1ab_0
   - pygments=2.15.1=pyhd8ed1ab_0
-  - pyjwt=2.7.0=pyhd8ed1ab_0
-  - pyparsing=3.1.0=pyhd8ed1ab_0
+  - pyjwt=2.8.0=pyhd8ed1ab_0
+  - pyparsing=3.0.9=pyhd8ed1ab_0
   - pyrsistent=0.19.3=py310h8d17308_0
   - python-fastjsonschema=2.17.1=pyhd8ed1ab_0
   - python-json-logger=2.0.7=pyhd8ed1ab_0
   - pytz=2023.3=pyhd8ed1ab_0
   - pywin32=304=py310h00ffb61_2
-  - pywinpty=2.0.10=py310h00ffb61_0
+  - pywinpty=2.0.11=py310h00ffb61_0
   - pyyaml=6.0=py310h8d17308_5
   - pyzmq=25.1.0=py310hcd737a0_0
   - rfc3986-validator=0.1.1=pyh9f0ad1d_0
+  - ruamel.yaml.clib=0.2.7=py310h8d17308_1
   - setuptools=67.7.2=pyhd8ed1ab_0
   - six=1.16.0=pyh6c4a22f_0
   - sniffio=1.3.0=pyhd8ed1ab_0
   - snowballstemmer=2.2.0=pyhd8ed1ab_0
   - soupsieve=2.3.2.post1=pyhd8ed1ab_0
   - sphinxcontrib-applehelp=1.0.4=pyhd8ed1ab_0
   - sphinxcontrib-devhelp=1.0.2=py_0
@@ -218,56 +219,56 @@
   - tabulate=0.9.0=pyhd8ed1ab_1
   - tensorboard-data-server=0.7.0=py310h5588dad_0
   - toml=0.10.2=pyhd8ed1ab_0
   - tomli=2.0.1=pyhd8ed1ab_0
   - tornado=6.3.2=py310h8d17308_0
   - traitlets=5.9.0=pyhd8ed1ab_0
   - typed-ast=1.5.5=py310h8d17308_0
-  - typing_extensions=4.6.3=pyha770c72_0
+  - typing_extensions=4.7.1=pyha770c72_0
   - typing_utils=0.1.0=pyhd8ed1ab_0
   - uc-micro-py=1.0.1=pyhd8ed1ab_0
   - unicodedata2=15.0.0=py310h8d17308_0
   - unidecode=1.3.6=pyhd8ed1ab_0
   - webencodings=0.5.1=py_1
   - websocket-client=1.6.1=pyhd8ed1ab_0
-  - wheel=0.40.0=pyhd8ed1ab_0
+  - wheel=0.40.0=pyhd8ed1ab_1
   - widgetsnbextension=4.0.8=pyhd8ed1ab_0
   - win32_setctime=1.1.0=pyhd8ed1ab_0
   - win_inet_pton=1.1.0=pyhd8ed1ab_6
   - wrapt=1.15.0=py310h8d17308_0
   - xorg-kbproto=1.0.7=hcd874cb_1002
   - xorg-libice=1.0.10=hcd874cb_0
   - xorg-libxau=1.0.11=hcd874cb_0
   - xorg-libxdmcp=1.1.3=hcd874cb_0
   - xorg-xextproto=7.3.0=hcd874cb_1003
   - xorg-xproto=7.0.31=hcd874cb_1007
-  - zipp=3.15.0=pyhd8ed1ab_0
+  - zipp=3.16.2=pyhd8ed1ab_0
   - accessible-pygments=0.0.4=pyhd8ed1ab_0
   - aiosignal=1.3.1=pyhd8ed1ab_0
-  - anyio=3.7.0=pyhd8ed1ab_1
+  - anyio=3.7.1=pyhd8ed1ab_0
   - asttokens=2.2.1=pyhd8ed1ab_0
   - babel=2.12.1=pyhd8ed1ab_1
   - backports.functools_lru_cache=1.6.5=pyhd8ed1ab_0
   - beautifulsoup4=4.12.2=pyha770c72_0
   - bleach=6.0.0=pyhd8ed1ab_0
   - brotli=1.0.9=hcfcfb64_9
   - cffi=1.15.1=py310h628cb3f_3
-  - click=8.1.3=win_pyhd8ed1ab_2
+  - click=8.1.6=win_pyh7428d3b_0
   - comm=0.1.3=pyhd8ed1ab_0
   - curl=8.1.2=h68f0423_0
   - dacite=1.8.0=pyhd8ed1ab_0
   - deprecation=2.1.0=pyh9f0ad1d_0
   - flake8=6.0.0=pyhd8ed1ab_0
   - fontconfig=2.14.2=hbde0cde_0
-  - glib-tools=2.76.3=h12be248_0
-  - grpcio=1.56.0=py310hb84602e_2
+  - glib-tools=2.76.4=h12be248_0
+  - grpcio=1.56.2=py310hb84602e_0
   - gts=0.7.6=h6b5321d_4
   - hdf5=1.12.2=nompi_h57737ce_101
-  - importlib-metadata=6.7.0=pyha770c72_0
-  - importlib_resources=5.12.0=pyhd8ed1ab_0
+  - importlib-metadata=6.8.0=pyha770c72_0
+  - importlib_resources=6.0.0=pyhd8ed1ab_1
   - jedi=0.18.2=pyhd8ed1ab_0
   - jinja2=3.1.2=pyhd8ed1ab_1
   - jupyterlab_pygments=0.2.2=pyhd8ed1ab_0
   - latexcodec=2.0.1=pyh9f0ad1d_0
   - lcms2=2.14=h90d422f_0
   - libxcb=1.13=hcd874cb_1004
   - lightning-utilities=0.9.0=pyhd8ed1ab_0
@@ -286,112 +287,114 @@
   - pytest=7.3.2=pyhd8ed1ab_1
   - python-dateutil=2.8.2=pyhd8ed1ab_0
   - pytorch-cuda=11.8=h24eeafa_5
   - pyu2f=0.1.5=pyhd8ed1ab_0
   - qtpy=2.3.1=pyhd8ed1ab_0
   - rfc3339-validator=0.1.4=pyhd8ed1ab_0
   - rsa=4.9=pyhd8ed1ab_0
+  - ruamel.yaml=0.17.32=py310h8d17308_0
   - send2trash=1.8.2=pyh08f2357_0
   - sip=6.7.9=py310h00ffb61_0
   - sympy=1.12=pyh04b8f61_3
   - tbb=2021.9.0=h91493d7_0
   - terminado=0.17.0=pyh08f2357_0
   - tinycss2=1.2.1=pyhd8ed1ab_0
   - tqdm=4.65.0=pyhd8ed1ab_1
-  - typing-extensions=4.6.3=hd8ed1ab_0
+  - typing-extensions=4.7.1=hd8ed1ab_0
   - werkzeug=2.3.6=pyhd8ed1ab_0
   - xorg-libsm=1.2.3=hcd874cb_1000
   - yarl=1.9.2=py310h8d17308_0
   - argon2-cffi-bindings=21.2.0=py310h8d17308_3
-  - astroid=2.15.5=py310h5588dad_0
+  - astroid=2.15.6=py310h5588dad_0
   - async-timeout=4.0.2=pyhd8ed1ab_0
   - brotlipy=0.7.0=py310h8d17308_1005
   - cairo=1.16.0=hd694305_1014
-  - cryptography=41.0.1=py310h6e82f81_0
+  - cryptography=41.0.2=py310h6e82f81_0
   - ffmpeg=5.1.2=gpl_h5037a79_109
-  - fonttools=4.40.0=py310h8d17308_0
+  - fonttools=4.41.0=py310h8d17308_0
   - ghp-import=2.1.0=pyhd8ed1ab_0
-  - glib=2.76.3=h12be248_0
-  - importlib_metadata=6.7.0=hd8ed1ab_0
+  - glib=2.76.4=h12be248_0
+  - importlib_metadata=6.8.0=hd8ed1ab_0
   - jsonschema=4.17.3=pyhd8ed1ab_0
   - jupyter_server_terminals=0.4.4=pyhd8ed1ab_1
   - libitk=5.3.0=h6e1890f_0
   - libnetcdf=4.8.1=nompi_h8c042bf_106
   - markdown=3.4.3=pyhd8ed1ab_0
   - mdit-py-plugins=0.4.0=pyhd8ed1ab_0
   - mkl=2022.1.0=h6a75c08_874
   - pillow=9.2.0=py310hd4fb230_3
-  - platformdirs=3.8.0=pyhd8ed1ab_0
+  - platformdirs=3.9.1=pyhd8ed1ab_0
   - pybtex=0.24.0=pyhd8ed1ab_2
   - pyqt5-sip=12.11.0=py310h00ffb61_3
   - python-build=0.10.0=pyhd8ed1ab_1
   - setuptools-scm=7.1.0=pyhd8ed1ab_0
-  - sqlalchemy=2.0.17=py310h8d17308_0
+  - sqlalchemy=2.0.19=py310h8d17308_0
   - stack_data=0.6.2=pyhd8ed1ab_0
   - tbb-devel=2021.9.0=h91493d7_0
   - wcwidth=0.2.6=pyhd8ed1ab_0
   - xorg-libx11=1.8.4=hcd874cb_0
-  - aiohttp=3.8.4=py310h8d17308_1
+  - aiohttp=3.8.5=py310h8d17308_0
   - argon2-cffi=21.3.0=pyhd8ed1ab_0
   - black=22.3.0=pyhd8ed1ab_0
-  - gstreamer=1.22.4=hb4038d2_0
+  - gstreamer=1.22.4=hb4038d2_1
   - harfbuzz=6.0.0=he256f1b_0
   - jupyter_core=5.3.1=py310h5588dad_0
   - jupyter_events=0.6.3=pyhd8ed1ab_0
   - libblas=3.9.0=17_win64_mkl
   - mkl-devel=2022.1.0=h57928b3_875
   - oauthlib=3.2.2=pyhd8ed1ab_0
   - prompt-toolkit=3.0.39=pyha770c72_0
   - pybtex-docutils=1.0.2=py310h5588dad_2
   - pyopenssl=23.2.0=pyhd8ed1ab_1
   - simpleitk=2.2.1=py310hcf936e6_1
   - xorg-libxext=1.3.4=hcd874cb_2
   - xorg-libxt=1.3.0=hcd874cb_0
   - flake8-black=0.3.6=pyhd8ed1ab_0
-  - gst-plugins-base=1.22.4=h001b923_0
+  - gst-plugins-base=1.22.4=h001b923_1
   - jupyter_client=8.3.0=pyhd8ed1ab_0
   - libcblas=3.9.0=17_win64_mkl
   - liblapack=3.9.0=17_win64_mkl
-  - nbformat=5.9.0=pyhd8ed1ab_0
+  - nbformat=5.9.1=pyhd8ed1ab_0
   - pango=1.50.14=hdffb7b3_0
   - prompt_toolkit=3.0.39=hd8ed1ab_0
   - urllib3=1.26.15=pyhd8ed1ab_0
   - wslink=1.11.1=pyhd8ed1ab_0
   - xorg-libxpm=3.5.16=hcd874cb_0
   - botocore=1.29.165=pyhd8ed1ab_0
   - ipython=8.14.0=pyh08f2357_0
   - libgd=2.3.3=h891f43f_3
   - liblapacke=3.9.0=17_win64_mkl
   - nbclient=0.7.4=pyhd8ed1ab_0
-  - numpy=1.25.0=py310hd02465a_0
+  - numpy=1.25.1=py310hd02465a_0
   - qt-main=5.15.8=h720456b_6
   - requests=2.31.0=pyhd8ed1ab_0
   - blas-devel=3.9.0=17_win64_mkl
   - contourpy=1.1.0=py310h232114e_0
-  - google-auth=2.21.0=pyh1a96a4e_0
+  - google-auth=2.22.0=pyh1a96a4e_0
   - graphviz=7.0.6=h51cb2cd_0
   - ipykernel=6.23.3=pyh6817e22_0
   - jupyter-cache=0.6.1=pyhd8ed1ab_0
-  - nbconvert-core=7.6.0=pyhd8ed1ab_0
+  - nbconvert-core=7.7.1=pyhd8ed1ab_1
+  - nibabel=5.1.0=py310h5588dad_2
   - pandas=1.5.3=py310h1c4a608_1
   - pooch=1.7.0=pyha770c72_3
   - pyqt=5.15.7=py310h1fd54f2_3
   - requests-oauthlib=1.3.1=pyhd8ed1ab_0
   - s3transfer=0.6.1=pyhd8ed1ab_0
   - sphinx=4.5.0=pyh6c4a22f_0
   - vtk=9.2.5=qt_py310h2fd250f_200
   - blas=2.117=mkl
   - boto3=1.26.165=pyhd8ed1ab_0
   - google-auth-oauthlib=1.0.0=pyhd8ed1ab_1
   - ipywidgets=8.0.7=pyhd8ed1ab_0
   - jupyter_console=6.6.3=pyhd8ed1ab_0
   - jupyter_server=2.7.0=pyhd8ed1ab_0
-  - matplotlib-base=3.7.1=py310h51140c5_0
+  - matplotlib-base=3.7.2=py310h51140c5_0
   - myst-parser=0.18.1=pyhd8ed1ab_0
-  - nbconvert-pandoc=7.6.0=pyhd8ed1ab_0
+  - nbconvert-pandoc=7.7.1=pyhd8ed1ab_1
   - pydata-sphinx-theme=0.13.3=pyhd8ed1ab_0
   - qtconsole-base=5.4.3=pyha770c72_0
   - scipy=1.10.1=py310h578b7cb_3
   - sphinx-comments=0.0.3=pyh9f0ad1d_0
   - sphinx-copybutton=0.5.2=pyhd8ed1ab_0
   - sphinx-design=0.3.0=pyhd8ed1ab_0
   - sphinx-external-toc=0.3.1=pyhd8ed1ab_0
@@ -400,17 +403,17 @@
   - sphinx-notfound-page=0.8.3=pyhd8ed1ab_0
   - sphinx-thebe=0.2.1=pyhd8ed1ab_0
   - sphinx-togglebutton=0.3.2=pyhd8ed1ab_0
   - sphinxcontrib-bibtex=2.5.0=pyhd8ed1ab_0
   - sphinxcontrib-dotnetdomain=0.4=py_0
   - sphinxcontrib-golangdomain=0.2.0.dev0=py_0
   - sphinxcontrib-jquery=4.1=pyhd8ed1ab_0
-  - matplotlib=3.7.1=py310h5588dad_0
+  - matplotlib=3.7.2=py310h5588dad_0
   - myst-nb=0.17.2=pyhd8ed1ab_0
-  - nbconvert=7.6.0=pyhd8ed1ab_0
+  - nbconvert=7.7.1=pyhd8ed1ab_1
   - notebook-shim=0.2.3=pyhd8ed1ab_0
   - pytorch=2.0.1=py3.10_cuda11.8_cudnn8_0
   - qtconsole=5.4.3=pyhd8ed1ab_0
   - sphinx-autoapi=2.1.0=pyhd8ed1ab_0
   - sphinx-book-theme=1.0.1=pyhd8ed1ab_0
   - sphinx_rtd_theme=1.2.2=pyha770c72_0
   - tensorboard=2.13.0=pyhd8ed1ab_0
```

### Comparing `hf-deepali-0.3.2/docker/Dockerfile` & `hf-deepali-0.4.0/docker/Dockerfile`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-ARG BASE_IMAGE=ubuntu:22.04
+ARG BASE_IMAGE
 FROM $BASE_IMAGE
 
 ARG DEBIAN_FRONTEND=noninteractive
 ENV TZ=Etc/UTC
 
 # Packages
 #
```

### Comparing `hf-deepali-0.3.2/docker/build` & `hf-deepali-0.4.0/docker/build`

 * *Files 19% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     --conda|--conda-version) conda_version="$2"; shift; ;;
     *) error "invalid argument $1"
   esac
   shift
 done
 
 [ -n "$tag" ] || tag="deepali:$USER"
-[ -n "$base_image" ] || base_image="ubuntu:22.04"
+[ -n "$base_image" ] || base_image="nvidia/cuda:11.8.0-cudnn8-runtime-ubuntu22.04"
 [ -n "$conda_version" ] || conda_version="22.9.0-3"
 [ -n "$python_version" ] || python_version="3.10.8"
 
 if [ -z "$version" ]; then
   version=$(cd "$PROJECT_DIR" && python -m setuptools_scm)
   if [ $? -ne 0 ]; then
     echo "setuptools_scm must be installed in Python environment used to build this Docker image. Alternatively, use --version to specify a deepali version string." 1>&2
```

### Comparing `hf-deepali-0.3.2/docker/run` & `hf-deepali-0.4.0/docker/run`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.2/docs/_citations.bib` & `hf-deepali-0.4.0/docs/_citations.bib`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.2/docs/_config.yml` & `hf-deepali-0.4.0/docs/_config.yml`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.2/docs/_images/logo.png` & `hf-deepali-0.4.0/docs/_images/logo.png`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.2/docs/_toc.yml` & `hf-deepali-0.4.0/docs/_toc.yml`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 
 format: jb-book
 root: index
 parts:
 - caption: Basics
   chapters:
   - file: basics/installation
-  - file: basics/example-page
 - caption: Tutorials
   chapters:
   - file: tutorials/pairwise-registration-intro
 - caption: Reference
   chapters:
   - file: reference/core/index
     sections:
@@ -42,9 +41,10 @@
   - file: reference/api/deepali/losses/index
   - file: reference/api/deepali/modules/index
   - file: reference/api/deepali/networks/index
   - file: reference/api/deepali/spatial/index
   - file: reference/api/deepali/utils/index
 - caption: Contributing
   chapters:
+  - file: basics/example-page
   - file: tutorials/example-notebook
   - file: tutorials/example-myst-notebook
```

### Comparing `hf-deepali-0.3.2/docs/basics/example-page.md` & `hf-deepali-0.4.0/docs/basics/example-page.md`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.2/docs/basics/installation.md` & `hf-deepali-0.4.0/docs/basics/installation.md`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.2/docs/index.md` & `hf-deepali-0.4.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.2/docs/reference/core/flow.md` & `hf-deepali-0.4.0/docs/reference/core/flow.md`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.2/docs/reference/core/image.md` & `hf-deepali-0.4.0/docs/reference/core/image.md`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.2/docs/reference/data/transforms.md` & `hf-deepali-0.4.0/docs/reference/data/transforms.md`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.2/docs/reference/spatial/common.md` & `hf-deepali-0.4.0/docs/reference/spatial/common.md`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.2/docs/reference/spatial/composite.md` & `hf-deepali-0.4.0/docs/reference/spatial/composite.md`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.2/docs/reference/utils/index.md` & `hf-deepali-0.4.0/docs/reference/utils/index.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,45 +1,34 @@
 # Miscellaneous utilities
 
 ```{eval-rst}
 .. automodule:: deepali.utils
     :noindex:
 ```
 
-## Command-line interfaces
-
-```{eval-rst}
-.. automodule:: deepali.utils.cli
-    :noindex:
-```
-
-```{admonition} Under construction
-In the meantime, please refer to {mod}`deepali.utils.cli`.
-```
-
 ## TensorBoard
 
 ```{eval-rst}
 .. automodule:: deepali.utils.tensorboard
     :noindex:
 ```
 
 ```{admonition} Under construction
 In the meantime, please refer to {mod}`deepali.utils.tensorboard`.
 ```
 
 ## SimpleITK interfaces
 
 ```{eval-rst}
-.. automodule:: deepali.utils.sitk
+.. automodule:: deepali.utils.simpleitk
     :noindex:
 ```
 
 ```{admonition} Under construction
-In the meantime, please refer to {mod}`deepali.utils.sitk`.
+In the meantime, please refer to {mod}`deepali.utils.simpleitk`.
 ```
 
 ## VTK interfaces
 
 ```{eval-rst}
 .. automodule:: deepali.utils.vtk
     :noindex:
```

### Comparing `hf-deepali-0.3.2/docs/tutorials/example-myst-notebook.md` & `hf-deepali-0.4.0/docs/tutorials/example-myst-notebook.md`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.2/docs/tutorials/example-notebook.ipynb` & `hf-deepali-0.4.0/docs/tutorials/example-notebook.ipynb`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.2/docs/tutorials/pairwise-registration-intro.ipynb` & `hf-deepali-0.4.0/docs/tutorials/pairwise-registration-intro.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.998359126984127%*

 * *Differences: {"'cells'": "{3: {'source': {insert: [(1, '    from deepali.core.environ import "*

 * *            "cuda_visible_devices\\n'), (6, '    from deepali.core.environ import "*

 * *            "cuda_visible_devices')], delete: [6, 1]}}, 7: {'source': {delete: [2]}}}",*

 * * "'metadata'": "{'language_info': {'version': '3.10.11'}}"}*

```diff
@@ -39,20 +39,20 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "try:\n",
-                "    from deepali.utils.cli import cuda_visible_devices\n",
+                "    from deepali.core.environ import cuda_visible_devices\n",
                 "except ImportError:\n",
                 "    if not os.getenv(\"COLAB_RELEASE_TAG\"):\n",
                 "        raise\n",
                 "    !git clone https://github.com/BioMedIA/deepali.git && pip install ./deepali\n",
-                "    from deepali.utils.cli import cuda_visible_devices"
+                "    from deepali.core.environ import cuda_visible_devices"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -86,15 +86,14 @@
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "from torchvision.datasets import MNIST\n",
                 "from torchvision.transforms import ToTensor\n",
                 "\n",
-                "\n",
                 "with io.capture_output() as captured:  # type: ignore[reportPrivateImportUsage]\n",
                 "    mnist = MNIST(root=\"data\", download=True, transform=ToTensor())"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
@@ -954,14 +953,14 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.12"
+            "version": "3.10.11"
         },
         "orig_nbformat": 4
     },
     "nbformat": 4,
     "nbformat_minor": 2
 }
```

### Comparing `hf-deepali-0.3.2/examples/ffd/README.md` & `hf-deepali-0.4.0/examples/ffd/README.md`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.2/examples/ffd/engine.py` & `hf-deepali-0.4.0/examples/ffd/engine.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.2/examples/ffd/hooks.py` & `hf-deepali-0.4.0/examples/ffd/hooks.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.2/examples/ffd/losses.py` & `hf-deepali-0.4.0/examples/ffd/losses.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.2/examples/ffd/optim.py` & `hf-deepali-0.4.0/examples/ffd/optim.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.2/examples/ffd/pairwise.py` & `hf-deepali-0.4.0/examples/ffd/pairwise.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.2/examples/ffd/params.yaml` & `hf-deepali-0.4.0/examples/ffd/params.yaml`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.2/examples/ffd/register.py` & `hf-deepali-0.4.0/examples/ffd/register.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,20 +9,21 @@
 import json
 import yaml
 
 import torch
 import torch.cuda
 from torch import Tensor
 
-from deepali.core import Grid, PathStr, unlink_or_mkdir
+from deepali.core.argparse import ArgumentParser, Args, main_func
+from deepali.core.environ import cuda_visible_devices
+from deepali.core.grid import Grid
+from deepali.core.logging import configure_logging
+from deepali.core.pathlib import PathStr, unlink_or_mkdir
 from deepali.data import Image
 from deepali.modules import TransformImage
-from deepali.utils.cli import ArgumentParser, Args, main_func
-from deepali.utils.cli import configure_logging, cuda_visible_devices
-from deepali.utils.cli import filter_warning_of_experimental_named_tensors_feature
 
 from .pairwise import register_pairwise
 
 log = logging.getLogger()
 
 
 def parser(**kwargs) -> ArgumentParser:
@@ -93,15 +94,14 @@
         if not torch.cuda.is_available():
             log.error("Cannot use --device 'cuda' when torch.cuda.is_available() is False")
             return 1
         gpu_ids = cuda_visible_devices()
         if len(gpu_ids) != 1:
             log.error("CUDA_VISIBLE_DEVICES must be set to one GPU")
             return 1
-    filter_warning_of_experimental_named_tensors_feature()
     return 0
 
 
 def func(args: Args) -> int:
     r"""Execute registration given parsed arguments."""
     config = load_config(args.config)
     device = torch.device("cuda:0" if args.device == "cuda" else "cpu")
```

### Comparing `hf-deepali-0.3.2/examples/istn/models/__init__.py` & `hf-deepali-0.4.0/examples/istn/models/__init__.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.2/examples/istn/models/itn.py` & `hf-deepali-0.4.0/examples/istn/models/itn.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.2/examples/istn/models/stn.py` & `hf-deepali-0.4.0/examples/istn/models/stn.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 import math
 from typing import Dict, List, Optional, Sequence, Tuple, Union, overload
 
 import torch
 from torch import Tensor, Size
 from torch.nn import Module, ModuleList, ReLU, Sequential, Upsample
 
-from deepali.core import Device, PathStr, ScalarOrTuple, functional as U, unlink_or_mkdir
+from deepali.core import Device, PathStr, ScalarOrTuple, functional as U
+from deepali.core.pathlib import unlink_or_mkdir
 from deepali.networks.layers import Conv2d, Conv3d, ConvLayer, Linear, convolution, pooling
 from deepali.networks.utils import module_output_size
 from deepali.spatial import TransformConfig, has_affine_component, has_nonrigid_component
 
 
 @dataclass
 class SpatialTransformerConfig(TransformConfig):
```

### Comparing `hf-deepali-0.3.2/examples/istn/params.yaml` & `hf-deepali-0.4.0/examples/istn/params.yaml`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.2/examples/istn/train.py` & `hf-deepali-0.4.0/examples/istn/train.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,21 +26,23 @@
 from torch.nn import Module, Sequential, functional as F
 from torch.optim import Adam, Optimizer
 from torch.optim.lr_scheduler import ExponentialLR
 from torch.utils.data import DataLoader, Dataset, Subset
 from torch.utils.data.distributed import DistributedSampler
 from torch.utils.tensorboard import SummaryWriter
 
-from deepali.core import DataclassConfig, functional as U, unlink_or_mkdir
+from deepali.core import functional as U
+from deepali.core.config import DataclassConfig
+from deepali.core.pathlib import unlink_or_mkdir
 from deepali.data import ImageBatch, ImageDataset, ImageDatasetConfig, Partition
 from deepali.data import collate_samples, prepare_batch
 from deepali.data.transforms import CastImage, ResizeImage
 from deepali.modules import ToImmutableOutput
-from deepali.utils.cli import LOG_FORMAT, LogLevel, cuda_visible_devices
-from deepali.utils.cli import filter_warning_of_experimental_named_tensors_feature
+from deepali.core.environ import cuda_visible_devices
+from deepali.core.logging import LOG_FORMAT, LogLevel
 from deepali.utils.ignite import handlers as H
 from deepali.utils.ignite.output_transforms import get_output_transform
 from deepali.utils.ignite.score_functions import negative_loss_score_function
 
 from models import ImageAndSpatialTransformerConfig as ModelConfig
 from models import ImageAndSpatialTransformerNetwork, create_istn
 
@@ -192,15 +194,14 @@
     log_dir: Path,
     log_level: Union[int, LogLevel],
     now_dt: str,
     trained_model_path: Optional[str] = None,
     detect_anomaly: bool = False,
 ) -> None:
     r"""Run model training in local distributed process."""
-    filter_warning_of_experimental_named_tensors_feature()
 
     rank = idist.get_rank()
     seed = config.train.random_seed + rank
     logger = setup_logger("train", level=int(log_level), format=LOG_FORMAT, distributed_rank=rank)
 
     logger.info(
         f"distributed backend={idist.backend()}, seed={seed}"
```

### Comparing `hf-deepali-0.3.2/pyproject.toml` & `hf-deepali-0.4.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -38,25 +38,26 @@
 dynamic = ["version"]
 
 dependencies = [
     "dacite",
     "deprecation",
     "pandas",
     "pyyaml",
-    "SimpleITK>=2.0",
+    "ruamel.yaml",
     "torch>=1.9",
     "typing-extensions",
 ]
 
 [project.optional-dependencies]
 all = [
     "hf-deepali[utils,tests]"
 ]
 utils = [
     "boto3",
+    "nibabel",
     "numpy",
     "scipy",
     "SimpleITK>=2.0",
     "vtk>=9.0",
 ]
 tests = [
     "pytest",
```

### Comparing `hf-deepali-0.3.2/src/deepali/core/_kornia.py` & `hf-deepali-0.4.0/src/deepali/core/_kornia.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.2/src/deepali/core/affine.py` & `hf-deepali-0.4.0/src/deepali/core/affine.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from typing import Optional, Union
 
 import torch
 from torch import Tensor
 
 from .linalg import homogeneous_transform
 from .tensor import as_float_tensor, atleast_1d, cat_scalars
-from .types import Array, Device, Scalar, Shape
+from .typing import Array, Device, DType, Scalar, Shape
 
 
 __all__ = (
     "affine_rotation_matrix",
     "apply_transform",
     "euler_rotation_matrix",
     "euler_rotation_angles",
@@ -84,15 +84,15 @@
     return matrix
 
 
 def identity_transform(
     shape: Union[int, Shape],
     *args,
     homogeneous: bool = False,
-    dtype: Optional[torch.dtype] = None,
+    dtype: Optional[DType] = None,
     device: Optional[Device] = None,
 ) -> Tensor:
     r"""Create homogeneous coordinate transformation matrix of identity mapping.
 
     Args:
         shape: Shape of non-homogeneous point coordinates tensor ``(..., D)``, where the size of the
             last dimension corresponds to the number of spatial dimensions.
@@ -118,15 +118,15 @@
     return euler_rotation_matrix(*args, **kwargs)
 
 
 def euler_rotation_matrix(
     angles: Union[Scalar, Array],
     order: Optional[str] = None,
     homogeneous: bool = False,
-    dtype: Optional[torch.dtype] = None,
+    dtype: Optional[DType] = None,
     device: Optional[Device] = None,
 ) -> Tensor:
     r"""Euler rotation matrices.
 
     Args:
         angles: Scalar rotation angle for a 2D rotation, or the three angles (alpha, beta, gamma)
             for an extrinsic rotation in the specified `order`. The argument can be a tensor of
@@ -335,15 +335,15 @@
         raise ValueError(f"euler_rotation_order() invalid argument '{arg}'")
     return order
 
 
 def scaling_transform(
     scales: Union[Scalar, Array],
     homogeneous: bool = False,
-    dtype: Optional[torch.dtype] = None,
+    dtype: Optional[DType] = None,
     device: Optional[Device] = None,
 ) -> Tensor:
     r"""Scaling matrices.
 
     Args:
         scales: Tensor of anisotropic scaling factors of shape ``(..., D)``.
         homogeneous: Whether to return homogeneous transformation matrices.
@@ -364,15 +364,15 @@
     matrix[..., J, J] = scales_
     return matrix
 
 
 def shear_matrix(
     angles: Union[Scalar, Array],
     homogeneous: bool = False,
-    dtype: Optional[torch.dtype] = None,
+    dtype: Optional[DType] = None,
     device: Optional[Device] = None,
 ) -> Tensor:
     r"""Shear matrices.
 
     Args:
         angles: Tensor of anisotropic shear angles in radians of shape ``(..., N)``,
             where ``N=(D * (D - 1)) / 2`` with ``D`` denoting the number of spatial dimensions.
@@ -406,15 +406,15 @@
     matrix[..., K[0], K[1]] = torch.tan(angles_)
     return matrix
 
 
 def translation(
     offset: Union[Scalar, Array],
     homogeneous: bool = False,
-    dtype: Optional[torch.dtype] = None,
+    dtype: Optional[DType] = None,
     device: Optional[Device] = None,
 ) -> Tensor:
     r"""Translation offsets / matrices.
 
     Args:
         offset: Translation vectors of shape ``(..., D)`` or ``(..., D, 1)``.
         homogeneous: Whether to return homogeneous transformation matrices.
```

### Comparing `hf-deepali-0.3.2/src/deepali/core/bspline.py` & `hf-deepali-0.4.0/src/deepali/core/bspline.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 from .enum import PaddingMode, SpatialDim, SpatialDimArg
 from .grid import Grid
 from .image import conv, conv1d
 from .itertools import is_even_permutation
 from .kernels import cubic_bspline1d
 from .tensor import move_dim
-from .types import ScalarOrTuple
+from .typing import DType, ScalarOrTuple
 
 
 @overload
 def cubic_bspline_control_point_grid_size(size: int, stride: int) -> int:
     ...
 
 
@@ -85,34 +85,34 @@
     )
 
 
 @overload
 def bspline_interpolation_weights(
     degree: int,
     stride: int,
-    dtype: Optional[torch.dtype] = None,
+    dtype: Optional[DType] = None,
     device: Optional[torch.device] = None,
 ) -> Tensor:
     ...
 
 
 @overload
 def bspline_interpolation_weights(
     degree: int,
     stride: Sequence[int],
-    dtype: Optional[torch.dtype] = None,
+    dtype: Optional[DType] = None,
     device: Optional[torch.device] = None,
 ) -> Tuple[Tensor, ...]:
     ...
 
 
 def bspline_interpolation_weights(
     degree: int,
     stride: ScalarOrTuple[int],
-    dtype: Optional[torch.dtype] = None,
+    dtype: Optional[DType] = None,
     device: Optional[torch.device] = None,
 ) -> Union[Tensor, Tuple[Tensor, ...]]:
     r"""Compute B-spline interpolation weights."""
     # Adapted from MIRTK ComputeBSplineIndicesAndWeights() at
     # https://github.com/BioMedIA/MIRTK/blob/877917b1b3ec9e602f7395dbbb1270e4334fc311/Modules/Numerics/include/mirtk/BSpline.h#L670-L789
     if degree == 3:
         return cubic_bspline_interpolation_weights(stride, dtype=dtype, device=device)
@@ -172,44 +172,44 @@
     return kernels
 
 
 @overload
 def cubic_bspline_interpolation_weights(
     stride: int,
     derivative: int = 0,
-    dtype: Optional[torch.dtype] = None,
+    dtype: Optional[DType] = None,
     device: Optional[torch.device] = None,
 ) -> Tensor:
     ...
 
 
 @overload
 def cubic_bspline_interpolation_weights(
     stride: int,
     derivative: Sequence[int],
-    dtype: Optional[torch.dtype] = None,
+    dtype: Optional[DType] = None,
     device: Optional[torch.device] = None,
 ) -> Tuple[Tensor, ...]:
     ...
 
 
 @overload
 def cubic_bspline_interpolation_weights(
     stride: Sequence[int],
     derivative: ScalarOrTuple[int] = 0,
-    dtype: Optional[torch.dtype] = None,
+    dtype: Optional[DType] = None,
     device: Optional[torch.device] = None,
 ) -> Tuple[Tensor, ...]:
     ...
 
 
 def cubic_bspline_interpolation_weights(
     stride: ScalarOrTuple[int],
     derivative: ScalarOrTuple[int] = 0,
-    dtype: Optional[torch.dtype] = None,
+    dtype: Optional[DType] = None,
     device: Optional[torch.device] = None,
 ) -> Union[Tensor, Tuple[Tensor, ...]]:
     r"""Compute cubic B-spline interpolation weights."""
     kernels = {}
     return_single_tensor = isinstance(stride, int) and isinstance(derivative, int)
     if isinstance(stride, int):
         stride = [stride] * (len(derivative) if isinstance(derivative, Sequence) else 1)
```

### Comparing `hf-deepali-0.3.2/src/deepali/core/config.py` & `hf-deepali-0.4.0/src/deepali/core/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,18 +4,21 @@
 
 from dataclasses import asdict, fields
 from pathlib import Path
 from typing import Any, Dict, Mapping, Optional, Sequence, TypeVar, Type
 
 import dacite
 import json
-import yaml
 
-from .path import abspath_template
-from .types import PathStr, is_path_str_field
+# PyYAML does not support YAML 1.2, which is required by DVC for example
+# (cf. https://github.com/iterative/dvc/issues/8466#issuecomment-1290757564)
+from ruamel.yaml import YAML
+
+from .pathlib import PathStr, abspath_template
+from .typing import is_path_str_field
 
 
 T = TypeVar("T", bound="DataclassConfig")
 
 
 class DataclassConfig(object):
     r"""Base class of configuration data classes."""
@@ -38,23 +41,21 @@
         config._finalize(parent)
         return config
 
     @classmethod
     def from_path(cls: Type[T], path: PathStr, section: Optional[str] = None) -> T:
         r"""Load configuration from file."""
         path = Path(path).absolute()
-        text = path.read_text()
-        if path.suffix == ".json":
-            config = json.loads(text)
-        elif path.suffix in (".yml", ".yaml"):
-            config = yaml.load(text, Loader=yaml.SafeLoader)
-        else:
-            raise ValueError(
-                f"{cls.__name__}.from_path() 'path' has unsupported suffix {path.suffix}"
-            )
+        if path.suffix not in (".json", ".yaml", ".yml"):
+            raise ValueError(f"{cls.__name__}.write() 'path' has unsupported suffix {path.suffix}")
+        with path.open("rt") as fp:
+            if path.suffix == ".json":
+                config = json.load(fp)
+            else:
+                config = YAML(typ="safe").load(fp)
         if config is None:
             config = {}
         if section is None:
             section = cls.section()
         if section:
             for key in section.split("."):
                 config = config.get(key, {})
@@ -63,26 +64,26 @@
     @classmethod
     def read(cls: Type[T], path: PathStr, section: Optional[str] = None) -> T:
         r"""Load configuration from file."""
         return cls.from_path(path, section=section)
 
     def write(self, path: PathStr) -> None:
         r"""Write configuration to file."""
-        path = Path(path).absolute()
         config = self.asdict()
-        if path.suffix == ".json":
-            text = json.dumps(config)
-        elif path.suffix in (".yml", ".yaml"):
-            text = yaml.safe_dump(config)
-        else:
+        path = Path(path).absolute()
+        if path.suffix not in (".json", ".yaml", ".yml"):
             raise ValueError(
                 f"{type(self).__name__}.write() 'path' has unsupported suffix {path.suffix}"
             )
         path.parent.mkdir(parents=True, exist_ok=True)
-        path.write_text(text)
+        with path.open("wt") as fp:
+            if path.suffix == ".json":
+                json.dump(config, fp)
+            else:
+                YAML(typ="safe").dump(config, fp)
 
     def asdict(self) -> Dict[str, Any]:
         r"""Get configuration dictionary."""
         return asdict(self)
 
     def _finalize(self: T, parent: Optional[Path] = None) -> None:
         r"""Finalize parameters after loading these from input file."""
```

### Comparing `hf-deepali-0.3.2/src/deepali/core/cube.py` & `hf-deepali-0.4.0/src/deepali/core/cube.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 import torch
 from torch import Tensor
 
 from .grid import ALIGN_CORNERS, Axes, Grid
 from .linalg import hmm, homogeneous_matrix, homogeneous_transform
 from .tensor import as_tensor, cat_scalars
-from .types import Array, Device, DType, Shape, Size
+from .typing import Array, Device, Shape, Size
 
 
 class Cube(object):
     r"""Bounding box oriented in world space which defines a normalized domain.
 
     Coordinates of points within this domain can be either with respect to the world coordinate
     system or the cube defined by the bounding box where coordinate axes are parallel to the
@@ -191,15 +191,15 @@
 
     @property
     def ndim(self) -> int:
         r"""Number of cube dimensions."""
         return len(self._extent)
 
     @property
-    def dtype(self) -> DType:
+    def dtype(self) -> torch.dtype:
         r"""Get data type of cube attribute tensors."""
         return self._extent.dtype
 
     @property
     def device(self) -> Device:
         r"""Get device on which cube attribute tensors are stored."""
         return self._extent.device
```

### Comparing `hf-deepali-0.3.2/src/deepali/core/enum.py` & `hf-deepali-0.4.0/src/deepali/core/enum.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.2/src/deepali/core/flow.py` & `hf-deepali-0.4.0/src/deepali/core/flow.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from . import affine as A
 from .enum import PaddingMode, Sampling
 from .grid import ALIGN_CORNERS, Grid
 from .image import check_sample_grid, grid_reshape, grid_sample
 from .image import spatial_derivatives
 from .image import _image_size, zeros_image
 from .tensor import move_dim
-from .types import Array, Device, Scalar, Shape, Size
+from .typing import Array, Device, DType, Scalar, Shape, Size
 
 
 def affine_flow(matrix: Tensor, grid: Union[Grid, Tensor], channels_last: bool = False) -> Tensor:
     r"""Compute dense flow field from homogeneous transformation.
 
     Args:
         matrix: Homogeneous coordinate transformation matrices of shape ``(N, D, 1)`` (translation),
@@ -427,13 +427,13 @@
 
 
 def zeros_flow(
     size: Optional[Union[int, Size, Grid]] = None,
     shape: Optional[Shape] = None,
     num: int = 1,
     named: bool = False,
-    dtype: Optional[torch.dtype] = None,
+    dtype: Optional[DType] = None,
     device: Optional[Device] = None,
 ) -> Tensor:
     r"""Create batch of flow fields filled with zeros for given image batch size or grid."""
     size = _image_size("zeros_flow", size, shape)
     return zeros_image(size, num=num, channels=len(size), named=named, dtype=dtype, device=device)
```

### Comparing `hf-deepali-0.3.2/src/deepali/core/functional.py` & `hf-deepali-0.4.0/src/deepali/core/functional.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,14 +114,16 @@
 from .pointset import denormalize_grid
 from .pointset import normalize_grid
 from .pointset import polyline_directions
 from .pointset import polyline_tangents
 from .pointset import transform_grid
 from .pointset import transform_points
 
+from .random import multinomial
+
 
 __all__ = (
     # Basic tensor functions
     "abspow",
     "as_tensor",
     "as_float_tensor",
     "as_one_hot_tensor",
@@ -130,14 +132,16 @@
     "batched_index_select",
     "max_difference",
     "move_dim",
     "round_decimals",
     "threshold",
     "unravel_coords",
     "unravel_index",
+    # Random sampling
+    "multinomial",
     # Linear algebra/geometry
     "affine_flow",
     "affine_rotation_matrix",
     "affine_transform_points",
     "affine_transform_vectors",
     "angle_axis_to_rotation_matrix",
     "angle_axis_to_quaternion",
```

### Comparing `hf-deepali-0.3.2/src/deepali/core/grid.py` & `hf-deepali-0.4.0/src/deepali/core/grid.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,16 +22,16 @@
     # At runtime, cyclical import resolved by Grid.cube() instead
     from .cube import Cube
 
 from .enum import SpatialDim, SpatialDimArg
 from .math import round_decimals
 from .linalg import homogeneous_transform, homogeneous_matrix, hmm
 from .tensor import as_tensor, cat_scalars
-from .types import Array, Device, PathStr, ScalarOrTuple, Shape, Size
-from .types import is_int_dtype
+from .typing import Array, Device, DType, PathStr, ScalarOrTuple, Shape, Size
+from .typing import is_int_dtype
 
 
 ALIGN_CORNERS = True
 r"""By default, grid corner points define the domain within which the data is defined.
 
 The normalized coordinates with respect to the grid cube are thus in [-1, 1] between
 the first and last grid points (grid cell center points). This is such that when a
@@ -969,15 +969,15 @@
         self,
         dim: Optional[int] = None,
         center: bool = False,
         normalize: bool = True,
         align_corners: Optional[bool] = None,
         channels_last: bool = True,
         flip: bool = False,
-        dtype: Optional[torch.dtype] = None,
+        dtype: Optional[DType] = None,
         device: Optional[Device] = None,
     ) -> Tensor:
         r"""Get tensor of grid point coordinates.
 
         Args:
             dim: Return coordinates for specified dimension, where ``dim=0`` refers to
                 the first grid dimension, i.e., the ``x`` axis.
@@ -1054,15 +1054,15 @@
         if not flip:  # default order (x, ...) requires flipping stacked meshgrid coords
             coords = torch.flip(coords, dims=(channels_dim,))
         return coords
 
     def points(
         self,
         axes: Axes = Axes.WORLD,
-        dtype: Optional[torch.dtype] = None,
+        dtype: Optional[DType] = None,
         device: Optional[Device] = None,
     ) -> Tensor:
         r"""Tensor of grid point coordinates with respect to specified coordinate axes."""
         axes = Axes(axes)
         coords = self.coords(
             normalize=(axes is Axes.CUBE),
             align_corners=False,
```

### Comparing `hf-deepali-0.3.2/src/deepali/core/image.py` & `hf-deepali-0.4.0/src/deepali/core/image.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from .enum import PaddingMode, Sampling
 from .enum import SpatialDim, SpatialDimArg, SpatialDerivativeKeys
 from .grid import ALIGN_CORNERS, Axes, Grid, grid_transform_points
 from .kernels import gaussian1d, gaussian1d_I
 from .nnutils import same_padding, stride_minus_kernel_padding
 from .random import multinomial
 from .tensor import as_tensor, cat_scalars, move_dim
-from .types import Array, Device, Scalar, ScalarOrTuple, Size, Shape, is_float_dtype
+from .typing import Array, Device, DType, Scalar, ScalarOrTuple, Size, Shape, is_float_dtype
 
 
 def avg_pool(
     data: Tensor,
     kernel_size: ScalarOrTuple[int],
     stride: Optional[ScalarOrTuple[int]] = None,
     padding: Optional[ScalarOrTuple[int]] = 0,
@@ -298,15 +298,15 @@
     kernel: Tensor,
     dim: int = -1,
     stride: int = 1,
     dilation: int = 1,
     padding: Union[PaddingMode, str, int] = None,
     output_padding: Optional[int] = None,
     transpose: bool = False,
-    dtype: Optional[torch.dtype] = None,
+    dtype: Optional[DType] = None,
 ) -> Tensor:
     r"""Convolve data with 1-dimensional kernel along specified dimension."""
     if not isinstance(data, Tensor):
         raise TypeError("conv1d() 'data' must be torch.Tensor")
     if data.ndim < 3:
         raise ValueError("conv1d() 'data' must have shape (N, C, ..., X)")
     if not isinstance(kernel, Tensor):
@@ -1348,15 +1348,15 @@
 
 def rescale(
     data: Tensor,
     min: Optional[Scalar] = None,
     max: Optional[Scalar] = None,
     data_min: Optional[Scalar] = None,
     data_max: Optional[Scalar] = None,
-    dtype: Optional[torch.dtype] = None,
+    dtype: Optional[DType] = None,
 ) -> Tensor:
     r"""Linearly rescale values to specified output interval.
 
     Args:
         data: Input tensor.
         min: Minimum value of output tensor. Use ``data_min`` if ``None``.
         max: Maximum value of output tensor. Use ``data_max`` if ``None``.
@@ -1687,15 +1687,15 @@
     size: Optional[Union[int, Size, Grid]] = None,
     shape: Optional[Shape] = None,
     num: Optional[int] = None,
     center: Optional[Sequence[int]] = None,
     radius: Optional[float] = None,
     sigma: float = 0,
     x_max: Optional[Union[float, Sequence[float]]] = None,
-    dtype: Optional[torch.dtype] = None,
+    dtype: Optional[DType] = None,
     device: Optional[Device] = None,
 ) -> Tensor:
     r"""Synthetic image of a circle.
 
     Args:
         size: Spatial size in the order ``(X, Y)``.
         shape: Spatial size in the order ``(Y, X)``.
@@ -1750,15 +1750,15 @@
     shape: Optional[Shape] = None,
     num: Optional[int] = None,
     center: Optional[Sequence[float]] = None,
     radius: Optional[float] = None,
     width: Optional[float] = None,
     sigma: float = 0,
     x_max: Union[float, Sequence[float]] = 5,
-    dtype: Optional[torch.dtype] = None,
+    dtype: Optional[DType] = None,
     device: Optional[Device] = None,
 ) -> Tensor:
     r"""Synthetic C-shaped image.
 
     Args:
         size: Spatial size in the order ``(X, Y)``.
         shape: Spatial size in the order ``(Y, X)``.
@@ -1804,15 +1804,15 @@
 
 
 def empty_image(
     size: Optional[Union[int, Size, Grid]] = None,
     shape: Optional[Shape] = None,
     num: Optional[int] = None,
     channels: Optional[int] = None,
-    dtype: Optional[torch.dtype] = None,
+    dtype: Optional[DType] = None,
     device: Optional[Device] = None,
 ) -> Tensor:
     """Create new batch of uninitalized image data.
 
     Args:
         size: Spatial size in the order ``(X, ...)``.
         shape: Spatial size in the order ``(..., X)``.
@@ -1832,15 +1832,15 @@
 
 def grid_image(
     size: Optional[Union[int, Size, Grid]] = None,
     shape: Optional[Shape] = None,
     num: Optional[int] = None,
     stride: Optional[Union[int, Sequence[int]]] = None,
     inverted: bool = False,
-    dtype: Optional[torch.dtype] = None,
+    dtype: Optional[DType] = None,
     device: Optional[Device] = None,
 ) -> Tensor:
     """Create batch of regularly spaced grid images.
 
     Args:
         size: Spatial size in the order ``(X, ...)``.
         shape: Spatial size in the order ``(..., X)``.
@@ -1878,15 +1878,15 @@
 
 
 def ones_image(
     size: Optional[Union[int, Size, Grid]] = None,
     shape: Optional[Shape] = None,
     num: Optional[int] = None,
     channels: Optional[int] = None,
-    dtype: Optional[torch.dtype] = None,
+    dtype: Optional[DType] = None,
     device: Optional[Device] = None,
 ) -> Tensor:
     """Create new batch of image data filled with ones.
 
     Args:
         size: Spatial size in the order ``(X, ...)``.
         shape: Spatial size in the order ``(..., X)``.
@@ -1905,15 +1905,15 @@
 
 
 def zeros_image(
     size: Optional[Union[int, Size, Grid]] = None,
     shape: Optional[Shape] = None,
     num: Optional[int] = None,
     channels: Optional[int] = None,
-    dtype: Optional[torch.dtype] = None,
+    dtype: Optional[DType] = None,
     device: Optional[Device] = None,
 ) -> Tensor:
     """Create new batch of image data filled with zeros.
 
     Args:
         size: Spatial size in the order ``(X, ...)``.
         shape: Spatial size in the order ``(..., X)``.
```

### Comparing `hf-deepali-0.3.2/src/deepali/core/itertools.py` & `hf-deepali-0.4.0/src/deepali/core/itertools.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.2/src/deepali/core/kernels.py` & `hf-deepali-0.4.0/src/deepali/core/kernels.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 import torch
 from torch import Tensor
 import torch.nn.functional as F
 
 from .linalg import tensordot
 from .tensor import as_tensor, cat_scalars
-from .types import Array, Device, Scalar
+from .typing import Array, Device, DType, Scalar
 
 
 def bspline1d(stride: int, order: int = 4) -> Tensor:
     r"""B-spline kernel of given order for specified control point spacing.
 
     Implementation adopted from AirLab:
     https://github.com/airlab-unibas/airlab/blob/80c9d487c012892c395d63c6d937a67303c321d1/airlab/utils/kernelFunction.py#L218
@@ -63,15 +63,15 @@
         return -t + 2
 
 
 def cubic_bspline(
     stride: Union[int, Sequence[int]],
     *args: int,
     derivative: int = 0,
-    dtype: Optional[torch.dtype] = None,
+    dtype: Optional[DType] = None,
     device: Optional[Device] = None,
 ):
     r"""Get n-dimensional cubic B-spline kernel.
 
     Args:
         stride: Spacing between control points with respect to original (upsampled) image grid.
         derivative: Order of cubic B-spline derivative.
@@ -96,15 +96,15 @@
         return cubic_bspline3d(stride_, derivative=derivative, dtype=dtype, device=device)
     raise NotImplementedError(f"cubic_bspline() {D}-dimensional kernel")
 
 
 def cubic_bspline1d(
     stride: Union[int, Sequence[int]],
     derivative: int = 0,
-    dtype: Optional[torch.dtype] = None,
+    dtype: Optional[DType] = None,
     device: Optional[Device] = None,
 ) -> Tensor:
     r"""Cubic B-spline kernel for specified control point spacing.
 
     Args:
         stride: Spacing between control points with respect to original (upsampled) image grid.
         derivative: Order of cubic B-spline derivative.
@@ -126,15 +126,15 @@
     return kernel.to(device)
 
 
 def cubic_bspline2d(
     stride: Union[int, Sequence[int]],
     *args: int,
     derivative: int = 0,
-    dtype: Optional[torch.dtype] = None,
+    dtype: Optional[DType] = None,
     device: Optional[Device] = None,
 ) -> Tensor:
     r"""Cubic B-spline kernel for specified control point spacing.
 
     Args:
         stride: Spacing between control points with respect to original (upsampled) image grid.
         derivative: Order of cubic B-spline derivative.
@@ -158,15 +158,15 @@
     return kernel.to(device)
 
 
 def cubic_bspline3d(
     stride: Union[int, Sequence[int]],
     *args: int,
     derivative: int = 0,
-    dtype: Optional[torch.dtype] = None,
+    dtype: Optional[DType] = None,
     device: Optional[Device] = None,
 ) -> Tensor:
     r"""Cubic B-spline kernel for specified control point spacing.
 
     Args:
         stride: Spacing between control points with respect to original (upsampled) image grid.
         derivative: Order of cubic B-spline derivative.
@@ -220,15 +220,15 @@
     return radius
 
 
 def gaussian(
     sigma: Union[Scalar, Array],
     *args: Scalar,
     normalize: bool = True,
-    dtype: Optional[torch.dtype] = None,
+    dtype: Optional[DType] = None,
     device: Optional[Device] = None,
 ):
     r"""Get n-dimensional Gaussian kernel."""
     sigma_ = cat_scalars(sigma, *args, dtype=dtype, device=torch.device("cpu"))
     if not torch.is_floating_point(sigma_):
         if dtype is not None:
             raise TypeError("Gaussian kernel dtype must be floating point type")
@@ -249,15 +249,15 @@
 
 
 def gaussian1d(
     sigma: Scalar,
     radius: Optional[Union[int, Tensor]] = None,
     scale: Optional[Scalar] = None,
     normalize: bool = True,
-    dtype: Optional[torch.dtype] = None,
+    dtype: Optional[DType] = None,
     device: Optional[Device] = None,
 ) -> Tensor:
     r"""Get 1-dimensional Gaussian kernel."""
     sigma = as_tensor(sigma, device="cpu")
     if sigma.ndim != 0:
         raise ValueError("gaussian1d() 'sigma' must be scalar")
     if sigma.lt(0):
@@ -285,15 +285,15 @@
         kernel = as_tensor(scale, dtype=dtype, device=device)
     return kernel
 
 
 def gaussian1d_I(
     sigma: Scalar,
     normalize: bool = True,
-    dtype: Optional[torch.dtype] = None,
+    dtype: Optional[DType] = None,
     device: Optional[Device] = None,
 ) -> Tensor:
     r"""Get 1st order derivative of 1-dimensional Gaussian kernel."""
     if torch.is_tensor(sigma):
         sigma_ = as_tensor(sigma)  # satisfy static type checker
         if sigma_.ndim != 0:
             raise ValueError("gaussian1d() 'sigma' must be scalar")
```

### Comparing `hf-deepali-0.3.2/src/deepali/core/linalg.py` & `hf-deepali-0.4.0/src/deepali/core/linalg.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from typing import Optional, Sequence, Tuple, Union
 
 import torch
 import torch.nn.functional as F
 from torch import Tensor
 
 from .tensor import as_tensor
-from .types import Device
+from .typing import Device, DType
 
 from ._kornia import (
     angle_axis_to_rotation_matrix,
     angle_axis_to_quaternion,
     rotation_matrix_to_angle_axis,
     rotation_matrix_to_quaternion,
     quaternion_to_angle_axis,
@@ -53,15 +53,15 @@
 
     AFFINE = "affine"  # Square affine transformation matrix.
     HOMOGENEOUS = "homogeneous"  # Full homogeneous transformation matrix.
     TRANSLATION = "translation"  # Translation vector.
 
 
 def as_homogeneous_tensor(
-    tensor: Tensor, dtype: Optional[torch.dtype] = None, device: Optional[Device] = None
+    tensor: Tensor, dtype: Optional[DType] = None, device: Optional[Device] = None
 ) -> Tuple[Tensor, HomogeneousTensorType]:
     r"""Convert tensor to homogeneous coordinate transformation."""
     tensor_ = as_tensor(tensor, dtype=dtype, device=device)
     if tensor_.ndim == 0:
         raise ValueError("Expected at least 1-dimensional 'tensor'")
     if tensor_.ndim == 1:
         tensor_ = tensor_.unsqueeze(1)
@@ -73,15 +73,15 @@
         type_ = HomogeneousTensorType.HOMOGENEOUS
     else:
         raise ValueError(f"Invalid homogeneous 'tensor' shape {tensor_.shape}")
     return tensor_, type_
 
 
 def as_homogeneous_matrix(
-    tensor: Tensor, dtype: Optional[torch.dtype] = None, device: Optional[Device] = None
+    tensor: Tensor, dtype: Optional[DType] = None, device: Optional[Device] = None
 ) -> Tensor:
     r"""Convert tensor to homogeneous coordinate transformation matrix.
 
     Args:
         tensor: Tensor of translations of shape ``(D,)`` or ``(..., D, 1)``, tensor of square affine
             matrices of shape ``(..., D, D)``, or tensor of homogeneous transformation matrices of
             shape ``(..., D, D + 1)``.
@@ -338,15 +338,15 @@
         a, a_type = c, c_type
     return a
 
 
 def homogeneous_matrix(
     tensor: Tensor,
     offset: Optional[Tensor] = None,
-    dtype: Optional[torch.dtype] = None,
+    dtype: Optional[DType] = None,
     device: Optional[Device] = None,
 ) -> Tensor:
     r"""Convert square matrix or vector to homogeneous coordinate transformation matrix.
 
     Args:
         tensor: Tensor of translations of shape ``(D,)`` or ``(..., D, 1)``, tensor of square affine
             matrices of shape ``(..., D, D)``, or tensor of homogeneous transformation matrices of
```

### Comparing `hf-deepali-0.3.2/src/deepali/core/math.py` & `hf-deepali-0.4.0/src/deepali/core/math.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 r"""Basic math operations with tensors."""
 
 from typing import Optional, Union
 
 import torch
 from torch import Tensor
 
-from .types import Scalar
+from .typing import Scalar
 
 
 def abspow(x: Tensor, exponent: Union[int, float]) -> Tensor:
     r"""Compute ``abs(x)**exponent``."""
     if exponent == 1:
         return x.abs()
     return x.abs().pow(exponent)
```

### Comparing `hf-deepali-0.3.2/src/deepali/core/nnutils.py` & `hf-deepali-0.4.0/src/deepali/core/nnutils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from collections import namedtuple
 from typing import Any, Iterable, Mapping, NamedTuple, Optional, Sequence, Tuple, Union, overload
 
 import torch
 from torch import Size, Tensor
 
-from .types import ScalarOrTuple
+from .typing import ScalarOrTuple
 
 
 def get_namedtuple_item(self: NamedTuple, arg: Union[int, str]) -> Any:
     if isinstance(arg, str):
         return getattr(self, arg)
     return self[arg]
```

### Comparing `hf-deepali-0.3.2/src/deepali/core/pointset.py` & `hf-deepali-0.4.0/src/deepali/core/pointset.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.2/src/deepali/core/tensor.py` & `hf-deepali-0.4.0/src/deepali/core/tensor.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 from logging import Logger
 from typing import Callable, Optional, Tuple, Union
 
 import torch
 from torch import Tensor
 
-from .types import Array, Device, Scalar
+from .typing import Array, Device, DType, Scalar
 
 
 def as_tensor(
-    arg: Union[Scalar, Array], dtype: Optional[torch.dtype] = None, device: Optional[Device] = None
+    arg: Union[Scalar, Array], dtype: Optional[DType] = None, device: Optional[Device] = None
 ) -> Tensor:
     r"""Create tensor from array if argument is not of type torch.Tensor.
 
     Unlike ``torch.as_tensor()``, this function preserves the tensor device if ``device=None``.
 
     """
     if device is None and isinstance(arg, Tensor):
@@ -30,15 +30,15 @@
     return arr_
 
 
 def as_one_hot_tensor(
     tensor: Tensor,
     num_classes: int,
     ignore_index: Optional[int] = None,
-    dtype: Optional[torch.dtype] = None,
+    dtype: Optional[DType] = None,
 ) -> Tensor:
     r"""Converts label image to one-hot encoding of multi-class segmentation.
 
     Adapted from: https://github.com/wolny/pytorch-3dunet
 
     Args:
         tensor: Input tensor of shape ``(N, 1, ..., X)`` or ``(N, C, ..., X)``.
@@ -83,26 +83,26 @@
     result = torch.zeros(shape, dtype=dtype).to(inputs.device).scatter_(1, inputs, 1)
     # bring back the ignore_index in the result
     result[mask] = ignore_index
     return result
 
 
 def atleast_1d(
-    arr: Array, dtype: Optional[torch.dtype] = None, device: Optional[Device] = None
+    arr: Array, dtype: Optional[DType] = None, device: Optional[Device] = None
 ) -> Tensor:
     r"""Convert array-like argument to 1- or more-dimensional PyTorch tensor."""
     arr_ = as_tensor(arr, dtype=dtype, device=device)
     return arr_.unsqueeze(0) if arr_.ndim == 0 else arr_
 
 
 def cat_scalars(
     arg: Union[Scalar, Array],
     *args: Scalar,
     num: int = 0,
-    dtype: Optional[torch.dtype] = None,
+    dtype: Optional[DType] = None,
     device: Optional[Device] = None,
 ) -> Tensor:
     r"""Join arguments into single 1-dimensional tensor.
 
     This auxiliary function is used by ``Grid``, ``Image``, and ``ImageBatch`` to support
     method arguments for different spatial dimensions as either scalar constant, list
     of scalar ``*args``, or single ``Array`` argument. If a single argument of type ``Array``
```

### Comparing `hf-deepali-0.3.2/src/deepali/data/__init__.py` & `hf-deepali-0.4.0/src/deepali/data/__init__.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.2/src/deepali/data/collate.py` & `hf-deepali-0.4.0/src/deepali/data/collate.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from dataclasses import is_dataclass
 from pathlib import Path
 from typing import Any, List, Mapping, NamedTuple, Sequence, overload
 
 import torch
 from torch.utils.data.dataloader import default_collate
 
-from ..core.types import Batch, Dataclass, Sample, is_namedtuple
+from deepali.core.typing import Batch, Dataclass, Sample, is_namedtuple
 
 from .flow import FlowField, FlowFields
 from .image import Image, ImageBatch
 from .sample import sample_field_names, sample_field_value
 from .sample import replace_all_sample_field_values
```

### Comparing `hf-deepali-0.3.2/src/deepali/data/dataset.py` & `hf-deepali-0.4.0/src/deepali/data/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 from typing import Mapping, Optional, Union, Sequence, TypeVar, overload
 
 import pandas as pd
 
 from torch.nn import Sequential
 from torch.utils.data import Dataset as TorchDataset, Subset
 
-from ..core.config import DataclassConfig
-from ..core.types import PathStr, Sample, is_namedtuple, is_path_str
+from deepali.core.config import DataclassConfig
+from deepali.core.typing import PathStr, Sample, is_namedtuple, is_path_str
 
 from .transforms import Transform
 from .transforms.image import ImageTransformConfig
 from .transforms.image import image_transforms, prepend_read_image_transform
 
 
 __all__ = (
```

### Comparing `hf-deepali-0.3.2/src/deepali/data/flow.py` & `hf-deepali-0.4.0/src/deepali/data/flow.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 
 from typing import Any, Optional, Sequence, Type, TypeVar, Union, overload
 
 import torch
 from torch import Tensor
 from torch.nn import functional as F
 
-from ..core.enum import PaddingMode, Sampling
-from ..core import flow as U
-from ..core.grid import Axes, Grid, grid_transform_vectors
-from ..core.tensor import move_dim
-from ..core.types import Array, Device, DType, EllipsisType, PathStr, Scalar
+from deepali.core import flow as U
+from deepali.core.enum import PaddingMode, Sampling
+from deepali.core.grid import ALIGN_CORNERS, Axes, Grid, grid_transform_vectors
+from deepali.core.tensor import move_dim
+from deepali.core.typing import Array, Device, DType, EllipsisType, PathStr, Scalar
 
 from .image import Image, ImageBatch
 
 
 TFlowField = TypeVar("TFlowField", bound="FlowField")
 TFlowFields = TypeVar("TFlowFields", bound="FlowFields")
 
@@ -489,31 +489,49 @@
             return self._axes
         batch = self.batch()
         batch = batch.axes(axes)
         return batch[0]
 
     @classmethod
     def from_sitk(
-        cls: Type[TFlowField], image: "sitk.Image", axes: Optional[Axes] = None
+        cls: Type[TFlowField],
+        image: "sitk.Image",
+        axes: Optional[Axes] = None,
+        align_corners: bool = ALIGN_CORNERS,
+        dtype: Optional[DType] = None,
+        device: Optional[Device] = None,
     ) -> TFlowField:
         r"""Create vector field from ``SimpleITK.Image``."""
-        image = super().from_sitk(image)
+        image = Image.from_sitk(image, align_corners=align_corners, dtype=dtype, device=device)
         return cls.from_image(image, axes=axes or Axes.WORLD)
 
     def sitk(self: TFlowField, axes: Optional[Axes] = None) -> "sitk.Image":
         r"""Create ``SimpleITK.Image`` from this vector field."""
-        disp: TFlowField = self.detach()
+        disp: FlowField = self.detach()
         disp = disp.axes(axes or Axes.WORLD)
         return Image.sitk(disp)
 
     @classmethod
-    def read(cls: Type[TFlowField], path: PathStr, axes: Optional[Axes] = None) -> TFlowField:
+    def read(
+        cls: Type[TFlowField],
+        path: PathStr,
+        axes: Optional[Axes] = None,
+        align_corners: bool = ALIGN_CORNERS,
+        dtype: Optional[DType] = None,
+        device: Optional[Device] = None,
+    ) -> TFlowField:
         r"""Read image data from file."""
-        image = cls._read_sitk(path)
-        return cls.from_sitk(image, axes)
+        image = Image.read(path, align_corners=align_corners, dtype=dtype, device=device)
+        return cls.from_image(image, axes=axes or Axes.WORLD)
+
+    def write(self, path: PathStr, axes: Optional[Axes] = None, compress: bool = True) -> None:
+        r"""Write flow field data to file."""
+        disp: FlowField = self.detach()
+        disp = disp.axes(axes or Axes.WORLD)
+        Image.write(disp, path, compress=compress)
 
     def curl(self: TFlowField, mode: str = "central") -> Image:
         r"""Compute curl of vector field."""
         batch = self.batch()
         rotvec = batch.curl(mode=mode)
         return rotvec[0]
```

### Comparing `hf-deepali-0.3.2/src/deepali/data/image.py` & `hf-deepali-0.4.0/src/deepali/data/image.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,33 +1,27 @@
 r"""Image tensors."""
 
 from __future__ import annotations
 
-from typing import Any, Dict, Optional, Sequence, Tuple, Type, TypeVar, Union, overload
+from typing import Any, Dict, Generator, Optional, Sequence, Tuple, Type, TypeVar, Union, overload
 
 import numpy as np
 import torch
 from torch import Tensor
 from torch.nn import functional as F
 
-try:
-    import SimpleITK as sitk
-    from ..utils.sitk.torch import image_from_tensor, tensor_from_image
-    from ..utils.sitk.imageio import read_image
-except ImportError:
-    sitk = None
-
-from ..core.cube import Cube
-from ..core.enum import PaddingMode, Sampling, SpatialDimArg
-from ..core.grid import ALIGN_CORNERS, Axes, Grid, grid_transform_points
-from ..core import image as U
-from ..core.itertools import zip_longest_repeat_last
-from ..core.path import unlink_or_mkdir
-from ..core.tensor import cat_scalars
-from ..core.types import Array, Device, DType, EllipsisType, PathStr, Scalar, ScalarOrTuple, Size
+from deepali.core.cube import Cube
+from deepali.core.enum import PaddingMode, Sampling, SpatialDimArg
+from deepali.core.grid import ALIGN_CORNERS, Axes, Grid, grid_transform_points
+from deepali.core import image as U
+from deepali.core.itertools import zip_longest_repeat_last
+from deepali.core.tensor import cat_scalars
+from deepali.core.typing import Array, Device, DType, EllipsisType
+from deepali.core.typing import PathUri, Scalar, ScalarOrTuple, Size
+from deepali.utils.imageio import read_image, write_image
 
 from .tensor import DataTensor
 
 Domain = Cube
 
 TImage = TypeVar("TImage", bound="Image")
 TImageBatch = TypeVar("TImageBatch", bound="ImageBatch")
@@ -199,14 +193,31 @@
                 )
             assert all(isinstance(d, Tensor) for d in data)
             assert all(isinstance(g, (tuple, list)) for g in grid)
             assert all(len(d) == len(g) for d, g in zip(data, grid))
             return tuple(cls._torch_function_result(func, d, g) for d, g in zip(data, grid))
         return cls._torch_function_result(func, data, grid)
 
+    @classmethod
+    def from_images(cls: Type[TImageBatch], images: Sequence[Image]) -> TImageBatch:
+        r"""Create image batch from sequence of images."""
+        if not all(isinstance(image, DataTensor) for image in images):
+            raise TypeError(f"{cls.__name__}.from_images() 'images' must be Image sequence")
+        data = torch.cat([image.tensor().unsqueeze(0) for image in images], dim=0)
+        grid = [image.grid() for image in images]
+        return cls(data, grid)
+
+    def append(self: TImageBatch, other: ImageBatch) -> TImageBatch:
+        r"""Append data from another image batch to data of this batch."""
+        if not isinstance(other, ImageBatch):
+            raise TypeError(f"{type(self).__name__}.append() 'other' must be ImageBatch")
+        data = torch.cat([self.tensor(), other.tensor()], dim=0)
+        grid = self.grids() + other.grids()
+        return self._make_instance(data, grid)
+
     def cube(self: TImageBatch, n: int = 0) -> Cube:
         r"""Get cube of n-th image in batch defining its normalized coordinates space with respect to the world."""
         return self._grid[n].cube()
 
     def cubes(self: TImageBatch) -> Tuple[Cube, ...]:
         r"""Get cubes of all images which define their normalized coordinates spaces with respect to the world."""
         return tuple(grid.cube() for grid in self._grid)
@@ -360,14 +371,20 @@
             if data.ndim < 3:
                 return data
             return self._make_subitem(data, grid)
         elif data.ndim < 4:
             return data
         return self._make_instance(data, grid)
 
+    def __iter__(self) -> Generator[Image, None, None]:
+        r"""Generator to iterate over images in batch."""
+        for index in range(len(self)):
+            data = self.tensor().narrow(0, index, 1).squeeze_(0)
+            yield self._make_subitem(data, self._grid[index])
+
     @property
     def sdim(self: TImageBatch) -> int:
         r"""Number of spatial dimensions."""
         return self.ndim - 2
 
     @property
     def nchannels(self: TImageBatch) -> int:
@@ -1111,60 +1128,73 @@
         return self.shape[0]
 
     @classmethod
     def from_sitk(
         cls: Type[TImage],
         image: "sitk.Image",
         align_corners: bool = ALIGN_CORNERS,
-        dtype: Optional[torch.dtype] = None,
+        dtype: Optional[DType] = None,
         device: Optional[Device] = None,
     ) -> TImage:
         r"""Create image from ``SimpleITK.Image`` instance."""
-        if sitk is None:
+        try:
+            from deepali.utils.simpleitk.torch import tensor_from_image
+        except ImportError:
             raise RuntimeError(f"{cls.__name__}.from_sitk() requires SimpleITK")
         data = tensor_from_image(image, dtype=dtype, device=device)
         grid = Grid.from_sitk(image, align_corners=align_corners)
         return cls(data, grid)
 
     def sitk(self: TImage) -> "sitk.Image":
         r"""Create ``SimpleITK.Image`` from this image."""
-        if sitk is None:
+        try:
+            from deepali.utils.simpleitk.torch import image_from_tensor
+        except ImportError:
             raise RuntimeError(f"{type(self).__name__}.sitk() requires SimpleITK")
         grid = self._grid
         origin = grid.origin().tolist()
         spacing = grid.spacing().tolist()
         direction = grid.direction().flatten().tolist()
         return image_from_tensor(self, origin=origin, spacing=spacing, direction=direction)
 
     @classmethod
-    def read(
+    def from_uri(
         cls: Type[TImage],
-        path: PathStr,
+        uri: str,
         align_corners: bool = ALIGN_CORNERS,
-        dtype: Optional[torch.dtype] = None,
+        dtype: Optional[DType] = None,
         device: Optional[Device] = None,
     ) -> TImage:
-        r"""Read image data from file."""
-        image = cls._read_sitk(path)
-        return cls.from_sitk(image, align_corners=align_corners, dtype=dtype, device=device)
+        r"""Create image from data stored at a given URI."""
+        return cls.read(uri, align_corners=align_corners, dtype=dtype, device=device)
+
+    def to_uri(
+        self: TImage,
+        uri: str,
+        compress: bool = True,
+    ) -> TImage:
+        r"""Save image data to file object at given URI."""
+        self.write(uri, compress=compress)
 
     @classmethod
-    def _read_sitk(cls, path: PathStr) -> "sitk.Image":
-        r"""Read SimpleITK.Image from file path."""
-        if sitk is None:
-            raise RuntimeError(f"{cls.__name__}.read() requires SimpleITK")
-        return read_image(path)
+    def read(
+        cls: Type[TImage],
+        path: PathUri,
+        align_corners: bool = ALIGN_CORNERS,
+        dtype: Optional[DType] = None,
+        device: Optional[Device] = None,
+    ) -> TImage:
+        r"""Read image data from file."""
+        data, grid = read_image(path)
+        grid = grid.align_corners_(align_corners)
+        return cls(data, grid, dtype=dtype, device=device)
 
-    def write(self: TImage, path: PathStr, compress: bool = True) -> None:
+    def write(self: TImage, path: PathUri, compress: bool = True) -> None:
         r"""Write image data to file."""
-        if sitk is None:
-            raise RuntimeError(f"{type(self).__name__}.write() requires SimpleITK")
-        image = self.sitk()
-        path = unlink_or_mkdir(path)
-        sitk.WriteImage(image, str(path), compress)
+        write_image(self.tensor(), self.grid(), path, compress=compress)
 
     def normalize(
         self: TImage,
         mode: str = "unit",
         min: Optional[float] = None,
         max: Optional[float] = None,
     ) -> TImage:
```

### Comparing `hf-deepali-0.3.2/src/deepali/data/partition.py` & `hf-deepali-0.4.0/src/deepali/data/partition.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.2/src/deepali/data/prepare.py` & `hf-deepali-0.4.0/src/deepali/data/prepare.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from collections import abc
 from dataclasses import is_dataclass
 from typing import Any, Mapping, NamedTuple, Optional, Sequence, Union, overload
 
 import torch
 from torch import Tensor
 
-from ..core.types import Batch, Dataclass, Device, is_namedtuple
+from deepali.core.typing import Batch, Dataclass, Device, is_namedtuple
 
 from .sample import sample_field_names, sample_field_value
 from .sample import replace_all_sample_field_values
 
 
 __all__ = ("prepare_batch",)
```

### Comparing `hf-deepali-0.3.2/src/deepali/data/sample.py` & `hf-deepali-0.4.0/src/deepali/data/sample.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 r"""Functions for dealing with dataset sample collections."""
 
 from copy import copy as shallowcopy
 from collections import OrderedDict
 from dataclasses import fields, is_dataclass
 from typing import Any, Mapping, Sequence, Tuple
 
-from ..core.types import Sample, is_namedtuple
+from deepali.core.typing import Sample, is_namedtuple
 
 
 __all__ = (
     "Sample",
     "sample_field_names",
     "sample_field_value",
     "replace_all_sample_field_values",
```

### Comparing `hf-deepali-0.3.2/src/deepali/data/sampler.py` & `hf-deepali-0.4.0/src/deepali/data/sampler.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.2/src/deepali/data/tensor.py` & `hf-deepali-0.4.0/src/deepali/data/tensor.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 from collections import OrderedDict
 from typing import Optional, Type, TypeVar
 
 import torch
 import torch.utils.hooks
 from torch import Tensor
 
-from ..core.tensor import as_tensor
-from ..core.types import Array, Device, DType
+from deepali.core.tensor import as_tensor
+from deepali.core.typing import Array, Device, DType
 
 
 T = TypeVar("T", bound="DataTensor")
 
 
 __all__ = ("DataTensor",)
```

### Comparing `hf-deepali-0.3.2/src/deepali/data/transforms/__init__.py` & `hf-deepali-0.4.0/src/deepali/data/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.2/src/deepali/data/transforms/image.py` & `hf-deepali-0.4.0/src/deepali/data/transforms/image.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 from pathlib import Path
 from typing import List, Mapping, Optional, Sequence, Union
 
 import torch
 from torch import Tensor
 from torch.nn import Module
 
-from ...core.enum import PaddingMode, Sampling
-from ...core.types import PathStr, ScalarOrTuple
-from ..image import Image
+from deepali.core.enum import PaddingMode, Sampling
+from deepali.core.typing import DeviceStr, DTypeStr, PathUri, ScalarOrTuple
 
+from ..image import Image
 from .item import ItemTransform, ItemwiseTransform
 
 
 __all__ = (
     "AvgPoolImage",
     "CastImage",
     "CenterCropImage",
@@ -74,15 +74,15 @@
             + f" count_include_pad={self.count_include_pad})"
         )
 
 
 class CastImage(ItemwiseTransform, Module):
     r"""Cast image data to specified type."""
 
-    def __init__(self, dtype: Union[torch.dtype, str]) -> None:
+    def __init__(self, dtype: DTypeStr) -> None:
         super().__init__()
         if isinstance(dtype, str):
             attr = dtype
             dtype = getattr(torch, attr, None)
             if dtype is None:
                 raise ValueError(
                     f"{type(self).__name__}() module torch has no 'dtype' named torch.{attr}"
@@ -239,29 +239,29 @@
 
 
 class ReadImage(ItemwiseTransform, Module):
     r"""Read image data from file path."""
 
     def __init__(
         self,
-        dtype: Optional[Union[torch.dtype, str]] = None,
-        device: Optional[Union[str, torch.device]] = None,
+        dtype: Optional[DTypeStr] = None,
+        device: Optional[DeviceStr] = None,
     ) -> None:
         super().__init__()
         if isinstance(dtype, str):
             attr = dtype
             dtype = getattr(torch, attr, None)
             if dtype is None:
                 raise ValueError(f"ReadImage() module torch has no 'dtype' named torch.{attr}")
         if dtype is not None and not isinstance(dtype, torch.dtype):
             raise TypeError("ReadImage() 'dtype' must by None or torch.dtype")
         self.dtype = dtype
         self.device = torch.device(device or "cpu")
 
-    def forward(self, path: PathStr) -> Image:
+    def forward(self, path: PathUri) -> Image:
         if not isinstance(path, (str, Path)):
             raise TypeError(f"{type(self).__name__}() 'path' must be Path or str")
         image = Image.read(path, dtype=self.dtype, device=self.device)
         return image
 
     def __repr__(self) -> str:
         return type(self).__name__ + f"(dtype={self.dtype}, device='{self.device!s}')"
```

### Comparing `hf-deepali-0.3.2/src/deepali/data/transforms/item.py` & `hf-deepali-0.4.0/src/deepali/data/transforms/item.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 from collections.abc import KeysView
 from copy import copy as shallowcopy, deepcopy
 from dataclasses import is_dataclass, fields
 from typing import Any, Callable, Iterable, Mapping, Optional, Union
 
 from torch.nn import Module
 
-from ...core.types import RE_OUTPUT_KEY_INDEX, is_namedtuple
+from deepali.core.collections import re_output_key_index
+from deepali.core.typing import is_namedtuple
 
 
 __all__ = ("ItemTransform", "ItemwiseTransform")
 
 
 class ItemTransform(Module):
     r"""Transform only specified item/field of dict, named tuple, tuple, list, or dataclass."""
@@ -70,15 +71,15 @@
             keys = set(self.key)
         else:
             keys = [self.key]
         for key in keys:
             if isinstance(key, int):
                 data = self._apply_index(data, key)
             elif isinstance(key, str):
-                key = RE_OUTPUT_KEY_INDEX.sub(r".\1", key)
+                key = re_output_key_index.sub(r".\1", key)
                 data = self._apply_key(data, key)
             else:
                 raise TypeError(f"{type(self).__name__}() 'key' must be None, int, or str")
         return data
 
     def _apply_all(self, data: Any) -> Any:
         r"""Transform all leaf items."""
```

### Comparing `hf-deepali-0.3.2/src/deepali/losses/__init__.py` & `hf-deepali-0.4.0/src/deepali/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.2/src/deepali/losses/base.py` & `hf-deepali-0.4.0/src/deepali/losses/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 from abc import ABCMeta, abstractmethod
 from collections import OrderedDict
 from typing import Any, Dict, Mapping, Optional, Sequence, Union
 
 from torch import Tensor
 from torch.nn import Module, ModuleDict, ModuleList
 
-from ..core.math import max_difference
-from ..core.types import ScalarOrTuple
+from deepali.core.math import max_difference
+from deepali.core.typing import ScalarOrTuple
 
 
 RegistrationResult = Dict[str, Any]
 RegistrationLosses = Union[Module, ModuleDict, ModuleList, Mapping[str, Module], Sequence[Module]]
 
 
 class RegistrationLoss(Module, metaclass=ABCMeta):
```

### Comparing `hf-deepali-0.3.2/src/deepali/losses/flow.py` & `hf-deepali-0.4.0/src/deepali/losses/flow.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 from __future__ import annotations
 
 from typing import Optional, Union
 
 import torch
 from torch import Tensor
 
-from ..core.types import Shape
+from deepali.core.typing import Shape
 
-from .base import DisplacementLoss
 from . import functional as L
+from .base import DisplacementLoss
 
 
 class _SpatialDerivativesLoss(DisplacementLoss):
     r"""Base class of regularization terms based on spatial derivatives of dense displacements."""
 
     def __init__(
         self,
@@ -170,15 +170,15 @@
         super().__init__(mode=mode, sigma=sigma, reduction=reduction)
         self.material_name = material_name
         self.first_parameter = first_parameter
         self.second_parameter = second_parameter
         self.poissons_ratio = poissons_ratio
         self.youngs_modulus = youngs_modulus
         self.shear_modulus = shear_modulus
-    
+
     def forward(self, u: Tensor) -> Tensor:
         r"""Evaluate regularization loss for given transformation."""
         spacing = self._spacing(u.shape)
         return L.elasticity_loss(
             u,
             spacing=spacing,
             mode=self.mode,
```

### Comparing `hf-deepali-0.3.2/src/deepali/losses/functional.py` & `hf-deepali-0.4.0/src/deepali/losses/functional.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 import math
 
 import torch
 from torch import Tensor
 from torch.nn.functional import binary_cross_entropy_with_logits, logsigmoid
 import torch.nn.functional as F
 
-from ..core.bspline import evaluate_cubic_bspline
-from ..core.enum import SpatialDerivativeKeys, SpatialDim
-from ..core.grid import Grid
-from ..core.image import avg_pool, dot_channels, rand_sample, spatial_derivatives
-from ..core.flow import denormalize_flow
-from ..core.pointset import transform_grid
-from ..core.pointset import transform_points
-from ..core.tensor import as_one_hot_tensor, move_dim
-from ..core.types import Array, ScalarOrTuple
+from deepali.core.bspline import evaluate_cubic_bspline
+from deepali.core.enum import SpatialDerivativeKeys, SpatialDim
+from deepali.core.grid import Grid
+from deepali.core.image import avg_pool, dot_channels, rand_sample, spatial_derivatives
+from deepali.core.flow import denormalize_flow
+from deepali.core.pointset import transform_grid
+from deepali.core.pointset import transform_points
+from deepali.core.tensor import as_one_hot_tensor, move_dim
+from deepali.core.typing import Array, ScalarOrTuple
 
 
 __all__ = (
     "balanced_binary_cross_entropy_with_logits",
     "binary_cross_entropy_with_logits",
     "label_smoothing",
     "dice_score",
```

### Comparing `hf-deepali-0.3.2/src/deepali/losses/image.py` & `hf-deepali-0.4.0/src/deepali/losses/image.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 r"""Image dissimilarity measures."""
 
 from typing import Optional, Union
 
 from torch import Tensor
 
-from ..core import functional as U
-from ..core.types import ScalarOrTuple
+from deepali.core import functional as U
+from deepali.core.typing import ScalarOrTuple
 
+from . import functional as L
 from .base import NormalizedPairwiseImageLoss
 from .base import PairwiseImageLoss
-from . import functional as L
 
 
 class Dice(PairwiseImageLoss):
     r"""Generalized Sorensen-Dice similarity coefficient."""
 
     def __init__(self, epsilon: float = 1e-15) -> None:
         super().__init__()
```

### Comparing `hf-deepali-0.3.2/src/deepali/losses/params.py` & `hf-deepali-0.4.0/src/deepali/losses/params.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.2/src/deepali/losses/pointset.py` & `hf-deepali-0.4.0/src/deepali/losses/pointset.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 r"""Point set distance terms."""
 
 import torch
 import torch.linalg
 from torch import Tensor
 
-from ..core import functional as U
+from deepali.core import functional as U
 
 from .base import PointSetDistance
 
 
 class ClosestPointDistance(PointSetDistance):
     r"""Average closest point distance."""
```

### Comparing `hf-deepali-0.3.2/src/deepali/modules/__init__.py` & `hf-deepali-0.4.0/src/deepali/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.2/src/deepali/modules/basic.py` & `hf-deepali-0.4.0/src/deepali/modules/basic.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 r"""Basic tensor operations."""
 
 from typing import Any, Mapping, Optional, Sequence, Union
 
 from torch import Tensor
 from torch.nn import Module
 
-from ..core import functional as U
-from ..core.enum import PaddingMode
-from ..core.types import ScalarOrTuple
+from deepali.core import functional as U
+from deepali.core.enum import PaddingMode
+from deepali.core.typing import ScalarOrTuple
 
 
 class GetItem(Module):
     r"""Get item at specified input tensor sequence index or with given dictionary key."""
 
     def __init__(self, key: Any) -> None:
         r"""Set item index or key.
```

### Comparing `hf-deepali-0.3.2/src/deepali/modules/flow.py` & `hf-deepali-0.4.0/src/deepali/modules/flow.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 from copy import copy as shallow_copy
 from typing import Optional
 
 from torch import Tensor
 from torch.nn import Module
 
-from ..core import functional as U
-from ..core import ALIGN_CORNERS
+from deepali.core import ALIGN_CORNERS
+from deepali.core import functional as U
 
 
 class ExpFlow(Module):
     r"""Layer that computes exponential map of flow field."""
 
     def __init__(
         self,
```

### Comparing `hf-deepali-0.3.2/src/deepali/modules/image.py` & `hf-deepali-0.4.0/src/deepali/modules/image.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 
 from pkg_resources import parse_version
 
 import torch
 from torch import Tensor
 from torch.nn import Module, functional as F
 
-from ..core import functional as U
-from ..core.enum import PaddingMode
-from ..core.kernels import gaussian1d
-from ..core.types import ScalarOrTuple
+from deepali.core import functional as U
+from deepali.core.enum import PaddingMode
+from deepali.core.kernels import gaussian1d
+from deepali.core.typing import ScalarOrTuple
 
 
 class FilterImage(Module):
     r"""Convoles an image with a predefined filter kernel."""
 
     def __init__(
         self,
```

### Comparing `hf-deepali-0.3.2/src/deepali/modules/lambd.py` & `hf-deepali-0.4.0/src/deepali/modules/lambd.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.2/src/deepali/modules/mixins.py` & `hf-deepali-0.4.0/src/deepali/modules/mixins.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.2/src/deepali/modules/output.py` & `hf-deepali-0.4.0/src/deepali/modules/output.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 r"""Output conversion modules."""
 
 from typing import Mapping, Sequence, Union
 
 from torch import Tensor
 from torch.nn import Module
 
-from ..core.nnutils import as_immutable_container
+from deepali.core.nnutils import as_immutable_container
 
 
 class ToImmutableOutput(Module):
     r"""Convert input to immutable output container.
 
     For use with ``torch.utils.tensorboard.SummaryWriter.add_graph`` when model output is list or dict.
     See error message: "Encountering a dict at the output of the tracer might cause the trace to be incorrect,
```

### Comparing `hf-deepali-0.3.2/src/deepali/modules/sample.py` & `hf-deepali-0.4.0/src/deepali/modules/sample.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 r"""Modules for sampling of image data, e.g., after spatial transformation."""
 
 from typing import Dict, Mapping, Optional, Tuple, Union, cast, overload
 
 from torch import Tensor
 from torch.nn import Module
 
-from ..core import functional as U
-from ..core.enum import PaddingMode, Sampling
-from ..core.grid import Axes, Grid, grid_points_transform
-from ..core.linalg import homogeneous_matmul, homogeneous_transform
-from ..core.types import Scalar
+from deepali.core import functional as U
+from deepali.core.enum import PaddingMode, Sampling
+from deepali.core.grid import Axes, Grid, grid_points_transform
+from deepali.core.linalg import homogeneous_matmul, homogeneous_transform
+from deepali.core.typing import Scalar
 
 
 class SampleImage(Module):
     r"""Sample images at grid points."""
 
     def __init__(
         self,
```

### Comparing `hf-deepali-0.3.2/src/deepali/modules/utilities.py` & `hf-deepali-0.4.0/src/deepali/modules/utilities.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.2/src/deepali/networks/__init__.py` & `hf-deepali-0.4.0/src/deepali/networks/__init__.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.2/src/deepali/networks/blocks/residual.py` & `hf-deepali-0.4.0/src/deepali/networks/blocks/residual.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 from __future__ import annotations
 
 from typing import Any, Mapping, Optional, Union
 
 import torch
 from torch.nn import Identity, Module, Sequential, init
 
-from ...core.enum import PaddingMode
-from ...core.types import ScalarOrTuple
+from deepali.core.enum import PaddingMode
+from deepali.core.typing import ScalarOrTuple
 
 from ..layers.acti import ActivationArg, activation
 from ..layers.conv import ConvLayer, convolution, same_padding
 from ..layers.norm import NormArg
 from ..layers.join import JoinLayer
 
 from .skip import SkipConnection, SkipFunc
```

### Comparing `hf-deepali-0.3.2/src/deepali/networks/blocks/skip.py` & `hf-deepali-0.4.0/src/deepali/networks/blocks/skip.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 r"""Sequential network layers with skip connections."""
 
 from typing import Any, Callable, Mapping, Union, overload
 
 from torch import Tensor
 from torch.nn import Identity, Module, ModuleDict, Sequential
 
-from ...modules.mixins import ReprWithCrossReferences
+from deepali.modules.mixins import ReprWithCrossReferences
+
 from ..layers.join import JoinFunc, join_func
 
 
 # fmt: off
 __all__ = (
     "DenseBlock",
     "Shortcut",
```

### Comparing `hf-deepali-0.3.2/src/deepali/networks/layers/__init__.py` & `hf-deepali-0.4.0/src/deepali/networks/layers/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 r"""Basic network modules, usually with learnable parameters."""
 
-from ...modules import Pad
-from ...modules import Reshape
-from ...modules import View
+from deepali.modules import Pad
+from deepali.modules import Reshape
+from deepali.modules import View
 
 from .acti import Activation
 from .acti import ActivationArg
 from .acti import ActivationFunc
 from .acti import activation
 from .acti import is_activation
```

### Comparing `hf-deepali-0.3.2/src/deepali/networks/layers/acti.py` & `hf-deepali-0.4.0/src/deepali/networks/layers/acti.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.2/src/deepali/networks/layers/conv.py` & `hf-deepali-0.4.0/src/deepali/networks/layers/conv.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,22 +9,18 @@
 
 from torch.nn import Module, init
 from torch.nn.modules import Sequential
 from torch.nn.modules import Conv1d as _Conv1d, ConvTranspose1d as _ConvTranspose1d
 from torch.nn.modules import Conv2d as _Conv2d, ConvTranspose2d as _ConvTranspose2d
 from torch.nn.modules import Conv3d as _Conv3d, ConvTranspose3d as _ConvTranspose3d
 
-from ...core.enum import PaddingMode
-from ...core.nnutils import same_padding
-from ...core.nnutils import stride_minus_kernel_padding
-from ...core.types import ScalarOrTuple
-from ...core.types import ScalarOrTuple1d
-from ...core.types import ScalarOrTuple2d
-from ...core.types import ScalarOrTuple3d
-from ...modules import ReprWithCrossReferences
+from deepali.core.enum import PaddingMode
+from deepali.core.nnutils import same_padding, stride_minus_kernel_padding
+from deepali.core.typing import ScalarOrTuple, ScalarOrTuple1d, ScalarOrTuple2d, ScalarOrTuple3d
+from deepali.modules import ReprWithCrossReferences
 
 from .acti import ActivationArg, activation
 from .norm import NormArg, normalization
 
 
 __all__ = (
     "Conv1d",
```

### Comparing `hf-deepali-0.3.2/src/deepali/networks/layers/join.py` & `hf-deepali-0.4.0/src/deepali/networks/layers/join.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.2/src/deepali/networks/layers/linear.py` & `hf-deepali-0.4.0/src/deepali/networks/layers/linear.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.2/src/deepali/networks/layers/norm.py` & `hf-deepali-0.4.0/src/deepali/networks/layers/norm.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.2/src/deepali/networks/layers/pool.py` & `hf-deepali-0.4.0/src/deepali/networks/layers/pool.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.2/src/deepali/networks/layers/upsample.py` & `hf-deepali-0.4.0/src/deepali/networks/layers/upsample.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,19 +16,19 @@
 from enum import Enum
 from typing import Optional, Sequence, Union
 
 import torch
 from torch import Tensor, nn
 from torch.nn import Module, Sequential, Identity
 
-from ...core.enum import PaddingMode, Sampling
-from ...core.grid import ALIGN_CORNERS
-from ...core.nnutils import upsample_padding, upsample_output_padding
-from ...core.types import ScalarOrTuple
-from ...modules import Pad
+from deepali.core.enum import PaddingMode, Sampling
+from deepali.core.grid import ALIGN_CORNERS
+from deepali.core.nnutils import upsample_padding, upsample_output_padding
+from deepali.core.typing import ScalarOrTuple
+from deepali.modules import Pad
 
 from .conv import convolution
 from .pool import pooling
 
 
 __all__ = ("Upsample", "UpsampleMode", "SubpixelUpsample")
 
@@ -96,15 +96,14 @@
 
         if out_channels is None:
             out_channels = in_channels
         upsample_mode = UpsampleMode.DECONV if mode == "default" else UpsampleMode(mode)
         padding_mode = PaddingMode(padding_mode).conv_mode(spatial_dims)
 
         if upsample_mode == UpsampleMode.DECONV:
-
             if not in_channels:
                 raise ValueError(
                     f"{type(self).__name__}() 'in_channels' required in {upsample_mode.value!r} mode"
                 )
 
             if isinstance(scale_factor, (int, float)):
                 scale_factor = (scale_factor,) * spatial_dims
@@ -149,15 +148,14 @@
                 init=init,
                 bias=bias,
                 transposed=True,
             )
             self.add_module("deconv", deconv)
 
         elif upsample_mode == UpsampleMode.INTERPOLATE:
-
             if pre_conv == "default":
                 if in_channels is None or in_channels == out_channels:
                     pre_conv = None
                 else:
                     if kernel_size is None:
                         kernel_size = 1
                     if isinstance(kernel_size, int):
@@ -200,15 +198,14 @@
             mode = Sampling(sampling).interpolate_mode(spatial_dims)
             upsample = nn.Upsample(
                 scale_factor=scale_factor, mode=mode, align_corners=align_corners
             )
             self.add_module("interpolate", upsample)
 
         elif upsample_mode == UpsampleMode.PIXELSHUFFLE:
-
             try:
                 scale_factor_ = int(scale_factor)
             except TypeError:
                 raise TypeError(
                     f"{type(self).__name__}() 'scale_factor' must be int for {upsample_mode.value!r} mode"
                 )
```

### Comparing `hf-deepali-0.3.2/src/deepali/networks/resnet.py` & `hf-deepali-0.4.0/src/deepali/networks/resnet.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,19 +10,19 @@
 from __future__ import annotations
 
 from dataclasses import dataclass
 from typing import Any, Callable, Mapping, Optional, Sequence, Type, Union
 
 from torch.nn import Flatten, Module, Sequential, init
 
-from ..core.config import DataclassConfig
-from ..core.enum import PaddingMode
-from ..core.itertools import zip_longest_repeat_last
-from ..core.types import ScalarOrTuple
-from ..modules import ReprWithCrossReferences
+from deepali.core.config import DataclassConfig
+from deepali.core.enum import PaddingMode
+from deepali.core.itertools import zip_longest_repeat_last
+from deepali.core.typing import ScalarOrTuple
+from deepali.modules import ReprWithCrossReferences
 
 from .blocks import ResidualUnit
 from .layers import ActivationArg, NormArg, ConvLayer, Linear, Upsample, pooling
 from .layers import is_batch_norm, is_convolution, is_group_norm
 
 
 # fmt: off
```

### Comparing `hf-deepali-0.3.2/src/deepali/networks/unet.py` & `hf-deepali-0.4.0/src/deepali/networks/unet.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from dataclasses import dataclass, field
 from typing import Callable, Iterable, Mapping, NamedTuple, Optional, Sequence, Tuple, Type, Union
 from typing import Dict, List
 
 from torch import Tensor
 from torch.nn import Identity, Module, ModuleDict, Sequential
 
-from ..core.config import DataclassConfig
-from ..core.enum import PaddingMode
-from ..core.image import crop
-from ..core.itertools import repeat_last
-from ..core.nnutils import as_immutable_container
-from ..core.types import ListOrTuple, ScalarOrTuple
-from ..modules import GetItem, ReprWithCrossReferences
+from deepali.core.config import DataclassConfig
+from deepali.core.enum import PaddingMode
+from deepali.core.image import crop
+from deepali.core.itertools import repeat_last
+from deepali.core.nnutils import as_immutable_container
+from deepali.core.typing import ListOrTuple, ScalarOrTuple
+from deepali.modules import GetItem, ReprWithCrossReferences
 
 from .blocks import ResidualUnit
 from .layers import ActivationArg, ConvLayer, JoinLayer, NormArg, PoolLayer
 from .layers import Upsample, UpsampleMode
 from .utils import module_output_size
```

### Comparing `hf-deepali-0.3.2/src/deepali/networks/utils.py` & `hf-deepali-0.4.0/src/deepali/networks/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,15 @@
 import torch
 from torch import Tensor, nn
 from torch.nn import Module
 
-from ..core.nnutils import conv_output_size
-from ..core.nnutils import conv_transposed_output_size
-from ..core.nnutils import pad_output_size
-from ..core.nnutils import pool_output_size
-from ..core.nnutils import unpool_output_size
-from ..core.nnutils import upsample_output_size
-from ..core.types import ScalarOrTuple
+from deepali.core.nnutils import conv_output_size, conv_transposed_output_size
+from deepali.core.nnutils import pad_output_size, upsample_output_size
+from deepali.core.nnutils import pool_output_size, unpool_output_size
+from deepali.core.typing import ScalarOrTuple
 
 from .layers import Pad
 from .blocks import SkipConnection
 from .layers import is_activation
 from .layers import is_norm_layer
```

### Comparing `hf-deepali-0.3.2/src/deepali/spatial/__init__.py` & `hf-deepali-0.4.0/src/deepali/spatial/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 and :attr:`.Axes.CUBE` otherwise.
 
 """
 
 import sys
 from typing import Any, Optional
 
-from ..core.grid import Grid
+from deepali.core.grid import Grid
 
 # Base classes for type comparison and annotation
 from .base import LinearTransform  # noqa
 from .base import NonRigidTransform  # noqa
 from .base import ReadOnlyParameters  # noqa
 from .base import SpatialTransform
```

### Comparing `hf-deepali-0.3.2/src/deepali/spatial/base.py` & `hf-deepali-0.4.0/src/deepali/spatial/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 r"""Base classes of spatial coordinate transformations."""
 
 from __future__ import annotations
 
 from abc import ABCMeta, abstractmethod
 from copy import copy as shallow_copy
-from typing import Optional, Tuple, TypeVar, Union, overload
-from typing_extensions import final
+from typing import Optional, Tuple, TypeVar, Union, final, overload
 
 import torch
 import torch.optim
 from torch import Tensor
 from torch.nn import Module
 import torch.nn.functional as F
 
-from ..core import functional as U
-from ..core.grid import Axes, Grid
-from ..core.linalg import as_homogeneous_matrix
-from ..core.types import Device
-from ..data.flow import FlowFields
-from ..modules import DeviceProperty
+from deepali.core import functional as U
+from deepali.core.grid import Axes, Grid
+from deepali.core.linalg import as_homogeneous_matrix
+from deepali.core.typing import Device
+from deepali.data.flow import FlowFields
+from deepali.modules import DeviceProperty
 
 
 TSpatialTransform = TypeVar("TSpatialTransform", bound="SpatialTransform")
 TLinearTransform = TypeVar("TLinearTransform", bound="LinearTransform")
 TNonRigidTransform = TypeVar("TNonRigidTransform", bound="NonRigidTransform")
```

### Comparing `hf-deepali-0.3.2/src/deepali/spatial/bspline.py` & `hf-deepali-0.4.0/src/deepali/spatial/bspline.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 from copy import copy as shallow_copy
 from typing import cast, overload
 from typing import Callable, List, Optional, Sequence, Tuple, TypeVar, Union
 
 import torch
 from torch import Size, Tensor
 
-from ..core import kernels as K
-from ..core import functional as U
-from ..core.enum import SpatialDim
-from ..core.grid import Grid
-from ..core.types import ScalarOrTuple
-from ..modules import ExpFlow
+from deepali.core import kernels as K
+from deepali.core import functional as U
+from deepali.core.enum import SpatialDim
+from deepali.core.grid import Grid
+from deepali.core.typing import ScalarOrTuple
+from deepali.modules import ExpFlow
 
 from .base import NonRigidTransform
 from .parametric import ParametricTransform
 
 
 TBSplineTransform = TypeVar("TBSplineTransform", bound="BSplineTransform")
```

### Comparing `hf-deepali-0.3.2/src/deepali/spatial/composite.py` & `hf-deepali-0.4.0/src/deepali/spatial/composite.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 from collections import OrderedDict
 from typing import Iterable, Optional, Tuple, TypeVar, Union, overload
 
 import torch
 from torch import Tensor
 from torch.nn import ModuleDict
 
-from ..core.grid import Axes, Grid, grid_transform_points
-from ..core.linalg import as_homogeneous_matrix, homogeneous_matmul
-from ..core.tensor import move_dim
+from deepali.core.grid import Axes, Grid, grid_transform_points
+from deepali.core.linalg import as_homogeneous_matrix, homogeneous_matmul
+from deepali.core.tensor import move_dim
 
 from .base import SpatialTransform
 
 
 TCompositeTransform = TypeVar("TCompositeTransform", bound="CompositeTransform")
```

### Comparing `hf-deepali-0.3.2/src/deepali/spatial/generic.py` & `hf-deepali-0.4.0/src/deepali/spatial/generic.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,21 +6,21 @@
 from pathlib import Path
 from typing import Callable, Dict, List, Mapping, Optional, Union
 
 import torch
 from torch import Tensor
 from torch.nn import ModuleDict
 
-from ..core.affine import euler_rotation_angles
-from ..core.affine import euler_rotation_matrix
-from ..core.config import DataclassConfig
-from ..core.grid import Grid
-from ..core.linalg import quaternion_to_rotation_matrix
-from ..core.linalg import rotation_matrix_to_quaternion
-from ..core.types import ScalarOrTuple
+from deepali.core.affine import euler_rotation_angles
+from deepali.core.affine import euler_rotation_matrix
+from deepali.core.config import DataclassConfig
+from deepali.core.grid import Grid
+from deepali.core.linalg import quaternion_to_rotation_matrix
+from deepali.core.linalg import rotation_matrix_to_quaternion
+from deepali.core.typing import ScalarOrTuple
 
 from .bspline import FreeFormDeformation, StationaryVelocityFreeFormDeformation
 from .composite import SequentialTransform
 from .linear import AnisotropicScaling, EulerRotation, QuaternionRotation
 from .linear import HomogeneousTransform, Shearing, Translation
 from .nonrigid import DisplacementFieldTransform, StationaryVelocityFieldTransform
```

### Comparing `hf-deepali-0.3.2/src/deepali/spatial/linear.py` & `hf-deepali-0.4.0/src/deepali/spatial/linear.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,20 +6,20 @@
 import math
 from typing import Callable, Optional, Union
 
 import torch
 from torch import Size, Tensor
 from torch.nn import init
 
-from ..core import affine as U
-from ..core.grid import Grid
-from ..core.linalg import normalize_quaternion
-from ..core.linalg import quaternion_to_rotation_matrix
-from ..core.linalg import rotation_matrix_to_quaternion
-from ..core.tensor import as_float_tensor
+from deepali.core import affine as U
+from deepali.core.grid import Grid
+from deepali.core.linalg import normalize_quaternion
+from deepali.core.linalg import quaternion_to_rotation_matrix
+from deepali.core.linalg import rotation_matrix_to_quaternion
+from deepali.core.tensor import as_float_tensor
 
 from .base import LinearTransform
 from .composite import SequentialTransform
 from .parametric import InvertibleParametricTransform
 
 
 class HomogeneousTransform(InvertibleParametricTransform, LinearTransform):
```

### Comparing `hf-deepali-0.3.2/src/deepali/spatial/nonrigid.py` & `hf-deepali-0.4.0/src/deepali/spatial/nonrigid.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 from copy import copy as shallow_copy
 import math
 from typing import Callable, Optional, Sequence, TypeVar, Union, cast
 
 import torch
 from torch import Size, Tensor
 
-from ..core import functional as U
-from ..core.grid import Axes, Grid
-from ..data.flow import FlowFields
-from ..modules import ExpFlow
+from deepali.core import functional as U
+from deepali.core.grid import Axes, Grid
+from deepali.data.flow import FlowFields
+from deepali.modules import ExpFlow
 
 from .base import NonRigidTransform
 from .parametric import ParametricTransform
 
 
 TDenseVectorFieldTransform = TypeVar(
     "TDenseVectorFieldTransform", bound="DenseVectorFieldTransform"
```

### Comparing `hf-deepali-0.3.2/src/deepali/spatial/parametric.py` & `hf-deepali-0.4.0/src/deepali/spatial/parametric.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 from copy import copy as shallow_copy
 from typing import Callable, Optional, Union, cast, overload
 
 import torch
 from torch import Size, Tensor
 from torch.nn import Parameter, init
 
-from ..core.grid import Grid
+from deepali.core.grid import Grid
 
 from .base import ReadOnlyParameters, TSpatialTransform
 
 
 class ParametricTransform:
     r"""Mix-in for spatial transformations that have (optimizable) parameters."""
```

### Comparing `hf-deepali-0.3.2/src/deepali/spatial/transformer.py` & `hf-deepali-0.4.0/src/deepali/spatial/transformer.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,18 +9,18 @@
 
 from copy import copy as shallow_copy
 from typing import Dict, Optional, Tuple, TypeVar, Union, cast, overload
 
 from torch import Tensor
 from torch.nn import Module
 
-from ..core.enum import PaddingMode, Sampling
-from ..core.grid import Axes, Grid
-from ..core.types import Scalar
-from ..modules import SampleImage
+from deepali.core.enum import PaddingMode, Sampling
+from deepali.core.grid import Axes, Grid
+from deepali.core.typing import Scalar
+from deepali.modules import SampleImage
 
 from .base import SpatialTransform
 
 
 TSpatialTransformer = TypeVar("TSpatialTransformer", bound="SpatialTransformer")
 
 
@@ -120,15 +120,15 @@
         align_centers: bool = False,
         flip_coords: bool = False,
     ) -> None:
         r"""Initialize spatial image transformer.
 
         Args:
             transform: Spatial coordinate transformation which is applied to ``target`` grid points.
-            target: Sampling grid of output images. If ``None``, use ``transform.axes()``.
+            target: Sampling grid of output images. If ``None``, use ``transform.grid()``.
             source: Sampling grid of input images. If ``None``, use ``target``.
             sampling: Image interpolation mode.
             padding: Image extrapolation mode or scalar out-of-domain value.
             align_centers: Whether to implicitly align the ``target`` and ``source`` centers.
                 If ``True``, only the affine component of the target to source transformation
                 is applied after the spatial grid ``transform``. If ``False``, also the
                 translation of grid center points is considered.
```

### Comparing `hf-deepali-0.3.2/src/deepali/utils/aws/resource.py` & `hf-deepali-0.4.0/src/deepali/utils/storage.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,449 +1,381 @@
 r"""Interface for resources stored locally, remotely, or in cloud storage."""
 
 from __future__ import annotations
 
 from copy import deepcopy
-import os
 from pathlib import Path
 import re
 import shutil
-from typing import Any, Generator, Optional, TypeVar, Union
+from typing import Generator, Optional, TypeVar, cast
 from urllib.parse import urlsplit
 
-PathStr = Union[Path, str]
-PathUri = Union[Path, str]
+from deepali.core.pathlib import PathStr, PathUri, to_uri, unlink_or_mkdir
 
 
-# See https://mypy.readthedocs.io/en/latest/generics.html#generic-methods-and-generic-self for the use
-# of `T` to annotate `self`. Many methods of `Resource` return `self` and we want those return values
-# to be the type of the subclass, not the looser type of `Resource`.
-T = TypeVar("T", bound="Resource")
+__all__ = (
+    "LocalObject",
+    "StorageObject",
+    "copy_file",
+)
 
 
-class Resource(object):
+TStorageObject = TypeVar("TStorageObject", bound="StorageObject")
+
+
+class StorageObject(object):
     r"""Interface for storage objects.
 
     This base class can be used for storage objects that are only stored locally.
-    The base implementations of the ``Resource`` interface functions reflect this use
-    case, where ``Resource("/path/to/file")`` represents such local path object.
-    The factory function ``Resource.from_uri`` is recommended for creating concrete
-    instances of ``Resource`` or one of its subclasses. To create a resource instance
-    for a local file path, use ``Resource.from_uri("file:///path/to/file")``.
-    An S3 object resource is created by ``Resource.from_uri("s3://bucket/key")``.
-    By using the ``Resource`` interface when writing tools that read and write
+    The base implementations of the ``StorageObject`` interface functions reflect this
+    use case, where ``StorageObject("/path/to/file")`` represents such local path object.
+    The factory function ``StorageObject.from_uri`` is recommended for creating concrete
+    instances of ``StorageObject`` or one of its subclasses. To create a resource instance
+    for a local file path, use ``StorageObject.from_uri("file:///path/to/file")``.
+    An S3 object resource is created by ``StorageObject.from_uri("s3://bucket/key")``.
+    By using the ``StorageObject`` interface when writing tools that read and write
     from either local, remote, or cloud storage, the tool CLI can create these
     resource instances from input argument URIs or local file path strings
     without URI scheme, i.e., without "file://" prefix. The consumer or producer
     of a resource object can either directly read/write the object data using
     the ``read_(bytes|text)`` and/or ``write_(bytes|text)`` functions, or
     download/upload the storage object to/from a local file path using the
     ``pull`` and ``push`` operations. Note that these operations directly interact
-    with the local storage if the resource instance is of base type ``Resource``,
+    with the local storage if the resource instance is of base type ``StorageObject``,
     rather than a remote or cloud storage specific subclass. The ``pull`` and ``push``
     operations should be preferred over ``read`` and ``write`` if the resource data
     is accessed multiple times, in order to take advantage of the local temporary
     copy of the resource object. Otherwise, system IO operations can be saved by
     using the direct ``read`` and ``write`` operations instead.
 
-    Additionally, the ``Resource.release`` function should be called by tools when
-    a resource is no longer required to indicate that the local copy of this resource
-    can be removed. If the resource object itself represents a local ``Resource``,
-    the release operation has no effect. To ensure that the ``release`` function is
-    called also in case of an exception, the ``Resource`` class implements the context
-    manager interface functions ``__enter__`` and ``__exit__``.
+    Additionally, the ``StorageObject.release()`` function should be called by tools
+    when a resource is no longer required to indicate that the local copy of this
+    resource can be removed. If the resource object itself represents a local
+    ``StorageObject``, the release operation has no effect. To ensure that the ``release``
+    function is called also in case of an exception, the ``StorageObject`` class
+    implements the context manager interface functions ``__enter__`` and ``__exit__``.
 
-    Example usage with resource context:
+    Example usage with storage object context:
 
     .. code-block:: python
 
-        with Resource.from_uri("s3://bucket/key") as res:
+        with StorageObject.from_uri("s3://bucket/key") as obj:
             # request download to local storage
-            path = res.pull().path
+            path = obj.pull().path
             # use local storage object referenced by path
         # local copy of storage object has been deleted
 
     The above is equivalent to using a try-finally block:
 
     .. code-block:: python
 
-        res = Resource.from_uri("s3://bucket/key")
+        obj = StorageObject.from_uri("s3://bucket/key")
         try:
-            path = res.pull().path
+            path = obj.pull().path
             # use local storage object referenced by path
         finally:
             # delete local copy of storage object
-            res.release()
+            obj.release()
 
     Usage of the ``with`` statement is recommended.
 
     Nesting of contexts for a resource object is possible and post-pones the
     invocation of the ``release`` operation until the outermost context has
     been left. This is accomplished by using a counter that is increment by
     ``__enter__``, and decremented again by ``__exit__``.
 
-    It should be noted that ``Resource`` operations are generally not thread-safe,
-    and actual consumers of resource objects should require the main thread to
-    deal with obtaining, downloading (if ``pull`` is used), and releasing a resource.
-    For different resources from remote storage (e.g., AWS S3), when using multiple
-    processes (threads), the main process (thread) must initialize the default client
-    connection (e.g., using ``S3Client.init_default()``) before spawning processes.
+    It should be noted that ``StorageObject`` operations are generally not thread-safe,
+    and actual consumers of resource objects should require the main thread to deal with
+    obtaining, downloading (if ``pull`` is used), and releasing a resource. For different
+    resources from remote storage (e.g., AWS S3), when using multiple processes (threads),
+    the main process (thread) must initialize the default client connection (e.g., using
+    ``S3Client.init_default()``) before spawning processes.
 
     """
 
-    def __init__(self: T, path: PathStr) -> None:
+    def __init__(self, path: PathStr) -> None:
         r"""Initialize storage object.
 
         Args:
             path (str, pathlib.Path): Local path of storage object.
 
         """
         self._path = Path(path).absolute()
         self._depth = 0
 
-    def __enter__(self: T) -> T:
+    def __enter__(self: TStorageObject) -> TStorageObject:
         r"""Enter context."""
         self._depth = max(1, self._depth + 1)
         return self
 
-    def __exit__(self: T, *exc) -> None:
+    def __exit__(self, *exc) -> None:
         r"""Release resource when leaving outermost context."""
         self._depth = max(0, self._depth - 1)
         if self._depth == 0:
             self.release()
 
     @staticmethod
-    def from_path(*args: Optional[PathStr]) -> Resource:
+    def from_path(*args: Optional[PathStr]) -> StorageObject:
         r"""Create storage object from path or URI.
 
         Args:
             args: Path or URI components. The last absolute path or URI is the base to which
                 subsequent arguments are appended. Any ``None`` value is ignored. See also ``to_uri()``.
 
         Returns:
             obj (Resource): Instance of concrete type representing the referenced storage object.
 
         """
-        return Resource.from_uri(to_uri(args))
+        return StorageObject.from_uri(to_uri(*args))
 
     @staticmethod
-    def from_uri(uri: str) -> Resource:
+    def from_uri(uri: str) -> StorageObject:
         r"""Create storage object from URI.
 
         Args:
             uri: URI of storage object.
 
         Returns:
-            obj (Resource): Instance of concrete type representing the referenced storage object.
+            Instance of concrete type representing the referenced storage object.
 
         """
         res = urlsplit(uri, scheme="file")
         if res.scheme == "file":
             match = re.match(r"/+([a-zA-Z]:.*)", res.path)
             path = match.group(1) if match else res.path
-            return Resource(Path("/" + res.netloc + "/" + path if res.netloc else path))
+            return LocalObject(Path("/" + res.netloc + "/" + path if res.netloc else path))
         if res.scheme == "s3":
             # DO NOT import at module level to avoid cyclical import!
-            from .s3.object import S3Object
+            from .aws.s3.object import S3Object
 
-            return S3Object.from_uri(uri)
+            return cast(StorageObject, S3Object.from_uri(uri))
         raise ValueError("Invalid or unsupported storage object URI: %s", uri)
 
     @property
-    def uri(self: T) -> str:
+    def uri(self) -> str:
         r"""
         Returns:
             uri (str): URI of storage object.
 
         """
         return self.path.as_uri()
 
     @property
-    def path(self: T) -> Path:
+    def path(self) -> Path:
         r"""Get absolute local path of storage object."""
         return self._path
 
     @property
-    def name(self: T) -> str:
+    def name(self) -> str:
         r"""Name of storage object including file name extension, excluding directory path."""
         return self.path.name
 
-    def with_path(self: T, path) -> T:
+    def with_path(self: TStorageObject, path) -> TStorageObject:
         r"""Create copy of storage object reference with modified ``path``.
 
         Args:
             path (str, pathlib.Path): New local path of storage object.
 
         Returns:
-            self: New storage object reference with modified ``path`` property.
+            New storage object reference with modified ``path`` property.
 
         """
         obj = deepcopy(self)
         obj._path = Path(path).absolute()
         return obj
 
-    def with_properties(self: T, **kwargs) -> T:
+    def with_properties(self: TStorageObject, **kwargs) -> TStorageObject:
         r"""Create copy of storage object reference with modified properties.
 
         Args:
             **kwargs: New property values. Only specified properties are changed.
 
         Returns:
-            self: New storage object reference with modified properties.
+            New storage object reference with modified properties.
 
         """
         obj = deepcopy(self)
         for name, value in kwargs.items():
             setattr(obj, name, value)
         return obj
 
-    def exists(self: T) -> bool:
+    def exists(self) -> bool:
         r"""Whether object exists in storage."""
         return self.path.exists()
 
-    def is_file(self: T) -> bool:
+    def is_file(self) -> bool:
         r"""Whether storage object represents a file."""
         return self.path.is_file()
 
-    def is_dir(self: T) -> bool:
+    def is_dir(self) -> bool:
         r"""Whether storage object represents a directory."""
         return self.path.is_dir()
 
-    def iterdir(self: T, prefix: Optional[str] = None) -> Generator[T, None, None]:
+    def iterdir(
+        self: TStorageObject, prefix: Optional[str] = None
+    ) -> Generator[TStorageObject, None, None]:
         r"""List storage objects within directory, excluding subfolder contents.
 
         Args:
             prefix: Name prefix.
 
         Returns:
-            iterable: Generator of storage objects.
+            Generator of storage objects.
 
         """
-        assert type(self) is Resource, "must be implemented by subclass"
+        assert type(self) is StorageObject, "must be implemented by subclass"
         for path in self.path.iterdir():
             if not prefix or path.name.startswith(prefix):
-                yield Resource(path)
+                yield cast(TStorageObject, StorageObject(path))
 
-    def pull(self: T, force: bool = False) -> T:
+    def pull(self: TStorageObject, force: bool = False) -> TStorageObject:
         r"""Download content of storage object to local path.
 
         Args:
             force (bool): Whether to force download even if local path already exists.
 
         Returns:
-            self: This storage object.
+            This storage object.
 
         """
         return self
 
-    def push(self: T, force: bool = False) -> T:
+    def push(self: TStorageObject, force: bool = False) -> TStorageObject:
         r"""Upload content of local path to storage object.
 
         Args:
             force (bool): Whether to force upload even if storage object already exists.
 
         Returns:
-            self: This storage object.
+            This storage object.
 
         """
         return self
 
-    def read_bytes(self: T) -> bytes:
+    def read_bytes(self) -> bytes:
         r"""Read file content from local path if it exists, or referenced storage object otherwise.
 
         Returns:
-            data (bytes): Binary file content of storage object.
+            Binary file content of storage object.
 
         """
         return self.pull().path.read_bytes()
 
-    def write_bytes(self: T, data: bytes) -> T:
+    def write_bytes(self: TStorageObject, data: bytes) -> TStorageObject:
         r"""Write bytes to storage object.
 
         Args:
-            data (bytes): Binary data to write.
+            data: Binary data to write.
 
         Returns:
-            self: This storage object.
+            This storage object.
 
         """
-        self.path.parent.mkdir(parents=True, exist_ok=True)
+        try:
+            self.path.unlink()
+        except FileNotFoundError:
+            self.path.parent.mkdir(parents=True, exist_ok=True)
         self.path.write_bytes(data)
         return self.push()
 
-    def read_text(self: T, encoding: Optional[str] = None) -> str:
+    def read_text(self, encoding: Optional[str] = None) -> str:
         r"""Read text file content from local path if it exists, or referenced storage object otherwise.
 
         Args:
-            encoding (str): Text encoding.
+            encoding: Text encoding.
 
         Returns:
-            text (str): Decoded text file content of storage object.
+            Decoded text file content of storage object.
 
         """
         return self.pull().path.read_text()
 
-    def write_text(self: T, text: str, encoding: Optional[str] = None) -> T:
+    def write_text(
+        self: TStorageObject, text: str, encoding: Optional[str] = None
+    ) -> TStorageObject:
         r"""Write text to storage object.
 
         Args:
-            text (str): Text to write.
-            encoding (str): Text encoding.
+            text: Text to write.
+            encoding: Text encoding.
 
         Returns:
-            self: This storage object.
+            This storage object.
 
         """
-        self.path.parent.mkdir(parents=True, exist_ok=True)
+        try:
+            self.path.unlink()
+        except FileNotFoundError:
+            self.path.parent.mkdir(parents=True, exist_ok=True)
         self.path.write_text(text, encoding=encoding)
         return self.push()
 
-    def rmdir(self: T) -> T:
+    def rmdir(self: TStorageObject) -> TStorageObject:
         r"""Remove directory both locally and from remote storage."""
         try:
             shutil.rmtree(self.path)
         except FileNotFoundError:
             pass
         return self
 
-    def unlink(self: T) -> T:
+    def unlink(self: TStorageObject) -> TStorageObject:
         r"""Remove file both locally and from remote storage."""
         try:
             self.path.unlink()
         except FileNotFoundError:
             pass
         return self
 
-    def delete(self: T) -> T:
+    def delete(self: TStorageObject) -> TStorageObject:
         r"""Remove object both locally and from remote storage."""
         try:
             self.rmdir()
         except NotADirectoryError:
             self.unlink()
         return self
 
-    def release(self: T) -> T:
+    def release(self: TStorageObject) -> TStorageObject:
         r"""Release local temporary copy of storage object.
 
         Only remove local copy of storage object. When the storage object
-        is only stored locally, i.e., self is not a subclass of Resource,
-        but of type ``Resource``, this operation does nothing.
+        is only stored locally, i.e., self is not a subclass of StorageObject,
+        but of type ``StorageObject``, this operation does nothing.
 
         """
-        if type(self) is not Resource:
+        if type(self) is not StorageObject:
             try:
                 shutil.rmtree(self.path)
             except FileNotFoundError:
                 pass
             except NotADirectoryError:
                 try:
                     self.path.unlink()
                 except FileNotFoundError:
                     pass
         return self
 
-    def __str__(self: T) -> str:
+    def __str__(self) -> str:
         r"""Get human-readable string representation of storage object reference."""
         return self.uri
 
-    def __repr__(self: T) -> str:
+    def __repr__(self) -> str:
         r"""Get human-readable string representation of storage object reference."""
         return type(self).__name__ + "(path='{}')".format(self.path)
 
 
-def is_absolute(path: Union[Path, str]) -> bool:
-    r"""Check whether given path string or URI is absolute."""
-    if is_uri(path):
-        return True
-    return Path(path).is_absolute()
-
-
-def is_uri(arg: Any) -> bool:
-    r"""Check whether a given argument is a URI."""
-    if isinstance(arg, Path):
-        return False
-    if isinstance(arg, str):
-        # Windows path with drive letter
-        if os.name == "nt" and re.match(r"([a-zA-Z]):[/\\](.*)", arg):
-            return False
-        return re.match(r"([a-zA-Z0-9]+)://(.*)", arg) is not None
-    return False
-
-
-def to_uri(*args: Optional[PathStr]) -> str:
-    r"""Create valid URI from resource paths.
-
-    Args:
-        args: Local path components or an already valid URI. The last absolute path or URI in this
-            list of arguments is the base path or URI prefix for subsequent relative paths which
-            are appended to this base to construct the URI. Any ``None`` values are ignored.
-
-    Returns:
-        Valid URI.
-
-    """
-    args = [arg for arg in args if arg is not None]
-    for i, arg in enumerate(reversed(args)):
-        if is_uri(arg):
-            base = str(arg)
-            args = args[len(args) - i :]
-            break
-        elif Path(arg).is_absolute():
-            base = Path(arg)
-            args = args[len(args) - i :]
-            break
-    else:
-        base = Path.cwd()
-    if isinstance(base, Path):
-        uri = local_path_uri(base.joinpath(*args))
-    else:
-        uri = norm_uri(f"{base}/{'/'.join(args)}" if args else base)
-    return uri
-
-
-def norm_uri(uri: str) -> str:
-    r"""Normalize URI.
-
-    Args:
-        uri: A valid URI string.
-
-    Returns:
-        Normalized URI string.
+class LocalObject(StorageObject):
+    r"""Local storage object."""
 
-    """
-    match = re.match(r"(?P<scheme>[a-zA-Z0-9]+)://(?P<path>.*)", uri)
-    if not match:
-        raise ValueError(f"norm_uri() 'uri' is not a valid URI: {uri}")
-    scheme = match["scheme"].lower()
-    path = re.sub("^/+", "", re.sub(r"[/\\]{1,}", "/", match["path"]))
-    # Local file URI
-    if scheme == "file":
-        if os.name != "nt" or re.match(r"(?P<drive>[a-zA-Z]):[/\\]", path) is None:
-            path = "/" + path
-        return "file://" + path
-    # AWS S3 object URI
-    if scheme == "s3":
-        return "s3://" + path
-    # Other URI
-    return urlsplit(uri, scheme="file").geturl()
-
-
-def local_path_uri(arg: PathStr) -> str:
-    r"""Create valid URI from local path.
-
-    Unlike Path.as_uri(), this function does not escape special characters as used in format template strings.
-
-    Args:
-        arg: Local path.
+    def release(self: TStorageObject) -> TStorageObject:
+        r"""Release local temporary copy of storage object."""
+        return self
 
-    Returns:
-        Valid URI.
 
-    """
-    uri = norm_uri(f"file://{Path(arg).absolute()}")
-    if uri.endswith("/"):
-        # Trailing forward slashes are removed by Path already, but trailing backward slashes are
-        # only converted to a single forward slash by norm_uri(), not removed by Path. To produce
-        # a consistent result regardless of whether forward or backward slashes are used, remove
-        # any remaining trailing slash even if it could signify a directory.
-        uri = uri[:-1]
-    return uri
+def copy_file(src: PathStr, dst: PathUri) -> StorageObject:
+    r"""Copy local file to specified path or URI."""
+    obj = StorageObject.from_uri(to_uri(dst))
+    if isinstance(obj, LocalObject):
+        path = unlink_or_mkdir(obj.path)
+        shutil.copy2(src, path)
+    else:
+        obj.with_path(src).push(force=True)
+    return obj
```

### Comparing `hf-deepali-0.3.2/src/deepali/utils/aws/s3/client.py` & `hf-deepali-0.4.0/src/deepali/utils/aws/s3/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,17 +5,19 @@
 from contextlib import contextmanager
 from enum import Enum
 import io
 from pathlib import Path
 from typing import Any, Callable, Dict, Generator, List, Optional, Set, Tuple, Union
 
 import boto3
+from botocore.exceptions import ClientError
 
 from .config import S3Config
 
+S3ClientError = ClientError
 PathStr = Union[Path, str]
 
 
 def match_all(key: str) -> bool:
     r"""Default 'match' function used by 'S3Client.download_files()'."""
     return True
 
@@ -94,19 +96,29 @@
         r"""Initialize S3 client.
 
         Args:
             config: Client configuration.
             **kwargs: Individual client configuration settings.
 
         """
-        super().__init__()
         if config is None:
             config = S3Config()
         self._config = config._replace(**kwargs)
         self._client = None
+        self._depth = 0
+
+    @property
+    def exceptions(self):
+        r"""Get boto3 exceptions for connected client."""
+        if self._client is None:
+            raise AssertionError(
+                f"{type(self).__name__} must be connected to access exceptions."
+                " Mabye use botocore.exceptions module instead."
+            )
+        return self._client.exceptions
 
     @classmethod
     def from_arg(cls, arg: Union[S3Config, S3Client, Dict[str, Any], None]) -> S3Client:
         r"""Get client instance given function argument.
 
         Args:
             arg: Function argument.
@@ -123,24 +135,14 @@
         if isinstance(arg, S3Config):
             return cls(arg)
         if isinstance(arg, dict):
             return cls(**arg)
         return cls.default()
 
     @property
-    def exceptions(self):
-        r"""Get boto3 exceptions for connected client."""
-        if self._client is None:
-            raise AssertionError(
-                f"{type(self).__name__} must be connected to access exceptions."
-                " Mabye use botocore.exceptions module instead."
-            )
-        return self._client.exceptions
-
-    @property
     def config(self) -> S3Config:
         r"""Get client configuration object."""
         return self._config
 
     @property
     def ops(self) -> Set[S3Client.Operation]:
         r"""Get list of permissible client operations."""
@@ -319,15 +321,16 @@
         """
         assert not self.is_closed(), "client connection required"
         assert bucket, "S3 bucket must be specified"
         assert key, "S3 object key must be specified"
         if S3Client.Operation.READ not in self.ops:
             raise PermissionError("S3 client has no read permissions")
         buffer = io.BytesIO()
-        self._client.download_fileobj(Bucket=bucket, Key=key, Fileobj=buffer)
+        config = self._config.transfer_config()
+        self._client.download_fileobj(Bucket=bucket, Key=key, Fileobj=buffer, Config=config)
         return buffer.getvalue()
 
     def write_bytes(self, bucket: str, key: str, data: bytes) -> None:
         r"""Upload binary object data.
 
         Args:
             bucket: Bucket name.
@@ -340,15 +343,16 @@
         """
         assert not self.is_closed(), "client connection required"
         assert bucket, "S3 bucket must be specified"
         assert key, "S3 object key must be specified"
         if S3Client.Operation.WRITE not in self.ops:
             raise PermissionError("S3 client has no write permissions")
         buffer = io.BytesIO(data)
-        self._client.upload_fileobj(Fileobj=buffer, Bucket=bucket, Key=key)
+        config = self._config.transfer_config()
+        self._client.upload_fileobj(Fileobj=buffer, Bucket=bucket, Key=key, Config=config)
 
     def read_text(self, bucket: str, key: str, encoding: Optional[str] = None) -> str:
         r"""Download text file content.
 
         Args:
             bucket: Bucket name.
             key: S3 object key.
@@ -494,19 +498,15 @@
                 "Use overwrite=True to force overwriting "
                 + "existing S3 object '{k}' in bucket {b}".format(k=key, b=bucket)
             )
         path = Path(path).absolute()
         self.write_bytes(bucket=bucket, key=key, data=path.read_bytes())
 
     def upload_files(
-        self,
-        path: PathStr,
-        bucket: str,
-        prefix: Optional[str] = None,
-        overwrite: bool = True,
+        self, path: PathStr, bucket: str, prefix: Optional[str] = None, overwrite: bool = True
     ) -> Tuple[int, int]:
         r"""Upload local directory to S3.
 
         Args:
             path: Local directory path.
             bucket: Bucket name.
             prefix: Common S3 object key prefix. If ``None`` or empty string,
@@ -584,22 +584,21 @@
 
         """
         assert not self.is_closed(), "client connection required"
         assert bucket, "S3 bucket must be specified"
         if S3Client.Operation.DELETE not in self.ops:
             raise PermissionError("S3 client has no permission to delete objects")
         count = 0
-        token = None
+        list_kwargs = {"Bucket": bucket, "Prefix": prefix}
+        del_kwargs = {"Bucket": bucket, "Delete": {"Objects": []}}
         while True:
-            resp = self._client.list_objects_v2(
-                Bucket=bucket, Prefix=prefix, ContinuationToken=token
-            )
-            count += len(
-                self._client.delete_objects(Bucket=bucket, Delete=dict(Objects=resp["Contents"]))[
-                    "Deleted"
-                ]
-            )
+            list_resp = self._client.list_objects_v2(**list_kwargs)
+            del_kwargs["Delete"]["Objects"] = [
+                {"Key": obj["Key"]} for obj in list_resp.get("Contents", [])
+            ]
+            if del_kwargs["Delete"]["Objects"]:
+                count += len(self._client.delete_objects(**del_kwargs)["Deleted"])
             try:
-                token = resp["NextContinuationToken"]
+                list_resp["ContinuationToken"] = list_resp["NextContinuationToken"]
             except KeyError:
                 break
         return count
```

### Comparing `hf-deepali-0.3.2/src/deepali/utils/aws/s3/object.py` & `hf-deepali-0.4.0/src/deepali/utils/aws/s3/object.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,25 @@
-r"""Representation of objects stored in AWS Simple Storage Service (S3)."""
+r"""Reference objects stored in AWS Simple Storage Service (S3)."""
 
 from __future__ import annotations
 
 import re
 
 from copy import deepcopy
 from pathlib import Path
 from tempfile import gettempdir
 from typing import Generator, Optional
 
+from deepali.core.pathlib import PathStr, to_uri
+from deepali.utils.storage import StorageObject
+
 from .client import S3Client
-from ..resource import PathStr, Resource
 
 
-class S3Object(Resource):
+class S3Object(StorageObject):
     r"""Object stored in AWS Simple Storage Service (S3)."""
 
     def __init__(self, bucket: str, key: str, path: PathStr = None) -> None:
         r"""Initialize AWS S3 object.
 
         Args:
             bucket: Name of AWS S3 bucket containing this object.
@@ -74,26 +76,40 @@
         Returns:
             path: Absolute path of local copy of S3 object.
 
         """
         key = S3Object.normkey(key)
         if key.startswith("/"):
             key = key[1:]
-        return Path(gettempdir()).joinpath("deepali", "cache", "s3", bucket, key)
+        return Path(gettempdir()).joinpath("deepali", "data", "s3", bucket, key)
 
     def reset_path(self) -> S3Object:
         r"""Reset ``path`` to ``default_path`` for given ``bucket`` and ``key``.
 
         Returns:
             self: This instance.
 
         """
         self._path = self.default_path(bucket=self.bucket, key=self.key)
         return self
 
+    @staticmethod
+    def from_path(*args: Optional[PathStr]) -> S3Object:
+        r"""Create storage object from path or URI.
+
+        Args:
+            args: Path or URI components. The last absolute path or URI is the base to which
+                subsequent arguments are appended. Any ``None`` value is ignored. See also ``to_uri()``.
+
+        Returns:
+            obj (Resource): Instance of concrete type representing the referenced storage object.
+
+        """
+        return S3Object.from_uri(to_uri(*args))
+
     @classmethod
     def from_uri(cls, uri: str) -> S3Object:
         r"""Create AWS S3 object from URI.
 
         Args:
             uri: URI of S3 object. Must start with 's3://' followed by the bucket name.
                 The remainder of the URI represents the object key, excluding the forward
@@ -175,15 +191,15 @@
         r"""Whether AWS S3 object exists and represents a file."""
         return not self.key.endswith("/") and self.exists()
 
     def is_dir(self) -> bool:
         r"""Whether AWS S3 object exists and represents a directory."""
         return self.key.endswith("/") and self.exists()
 
-    def iterdir(self, prefix: str = None) -> Generator[Resource, None, None]:
+    def iterdir(self, prefix: str = None) -> Generator[S3Object, None, None]:
         r"""List S3 objects within directory, excluding subfolder contents.
 
         Args:
             prefix: Name prefix.
 
         Returns:
             iterable: Generator of S3 objects.
@@ -231,15 +247,20 @@
 
         """
         if self.key.endswith("/"):
             self.s3.upload_files(
                 bucket=self.bucket, prefix=self.key, path=self.path, overwrite=force
             )
         else:
-            self.s3.upload_file(bucket=self.bucket, key=self.key, path=self.path, overwrite=force)
+            try:
+                self.s3.upload_file(
+                    bucket=self.bucket, key=self.key, path=self.path, overwrite=force
+                )
+            except FileExistsError:
+                pass
         return self
 
     def read_bytes(self) -> bytes:
         r"""Read file content from local path if it exists, or corresponding S3 object otherwise.
 
         Returns:
             Binary file content of storage object.
```

### Comparing `hf-deepali-0.3.2/src/deepali/utils/cli/argparse.py` & `hf-deepali-0.4.0/src/deepali/core/argparse.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,114 @@
-r"""Utility functions for creating argparse based command line interfaces."""
+r"""Utility functions for creating argparse based command-line interfaces.
+
+In order to implement a CLI module, first define an argument parser by implementing
+a ``parser()`` function within the module which instantiates an ``ArgumentParser``
+with the respective command-line arguments of the CLI module.
+
+.. code::
+
+    def parser(*args, **kwargs) -> ArgumentParser:
+        ...
+
+Next, implement the main function of the CLI module. To indicate that this function
+receives already parsed command-line arguments, and in accordance with the respective
+attribute of an argparse subparsers, this function must be named ``func()``. In addition,
+an ``init()`` function can optionally be defined. It can be used, for example, to
+configure the loggers and to set environment variables before ``func()`` is invoked.
+These initialization steps can also be done in ``func()``, but by splitting these out
+into ``init()`` it is possible to implement a CLI module which calls the ``func()`` of
+other CLI modules without repeating these initialization steps. The return value of
+``init()`` and ``func()`` must be the exit code of the program.
+
+.. code::
+
+    logger = logging.getLogger()
+
+    def init(args: ParsedArguments) -> int:
+        configure_logging(args, logger)
+        init_omp_num_threads(args.threads)
+
+    def func(args: ParsedArguments) -> int:
+        ...
+        return 0
+
+The above functions are sufficient to implement a CLI module. Finally, the description
+of the CLI module which is printed as part of the default help output should be given
+as docstring at the top of the module.
+
+Lastly, an actual ``main()`` function which invokes the CLI module has to be defined
+and either be called explicitly when ``__name__ == "__main__"``, or in a special module
+file named ``__main__.py`` which is executed by the Python interpreter when the package
+containing the CLI module is being executed using ``python -m``.
+
+The ``main_func()`` closure can be used to implement a script for a single CLI, i.e.,
+
+.. code::
+
+    main = main_func(parser, func, init=init)
+
+    if __name__ == "__main__":
+        sys.exit(main())
+
+The ``entry_point()`` closure can be used to implement a script which can invoke multiple CLIs.
+Which CLI is being executed depends on the subcommand name. Subcommands can further be nested.
+An example of such nested subcommands is given by ``conda``, e.g., ``conda env config vars set``.
+This can be implemented using the ``entry_point()`` defined by this module as follows.
+
+Implement the CLI module ``conda/env/config/vars/set.py`` which must define the ``parser()`` and
+``func()`` function as detailed above. Then copy the following code into ``conda/__main__.py``
+
+.. code::
+
+    import sys
+
+    from hfresearch.cli.argparse import entry_point
+
+    main = entry_point(
+        package=__name__,
+        path=__path__,
+        description="...",
+        subcommands=["env.config.vars.set"],
+    )
+
+    sys.exit(main())
+
+The ``subcommands`` keyword argument is optional. If not specified, ``entry_point()`` will
+auto-discover the available CLI modules when ``--help`` is requested. By specifying the
+available subcommands explicitly, the help output is generated faster.
+
+"""
 
 import argparse
 import inspect
 import os
 import sys
-import logging
 from typing import Any, Callable, Dict, Iterable, List, Optional, Sequence, Union
 from typing_extensions import Protocol
 from collections import namedtuple
 from importlib import import_module
 from pkgutil import walk_packages
 from pkg_resources import DistributionNotFound, get_distribution
 
+from .psutil import memory_limit
+from .typing import BoolStr
+
 
 ParsedArguments = argparse.Namespace  # for type annotations
 UnknownArguments = List[str]
 
+Args = ParsedArguments
+
 
 STANDARD_ARGUMENTS_GROUP_TITLE = "Standard arguments"
 
+# Valid values for arguments of type BoolStr
+TRUE = (True, "1", "yes", "on", "true", "True", "TRUE")
+FALSE = (False, "0", "no", "off", "false", "False", "FALSE")
+
 
 class HelpFormatter(argparse.ArgumentDefaultsHelpFormatter):
     # See: https://stackoverflow.com/a/35848313
 
     def add_usage(self, usage, actions, groups, prefix=None):
         if prefix is None:
             prefix = "Usage: "
@@ -124,18 +210,14 @@
         else:
             prog = os.path.basename(sys.argv[0])
         try:
             version = get_distribution(dist).version
         except DistributionNotFound:
             version = None
 
-        # Loggers
-        log = logging.getLogger(dist)
-        log.addHandler(logging.StreamHandler())
-
         # Main parser
         mainparser = ArgumentParser(
             prog=prog, description=description, add_help=True, version=version
         )
         subparsers = mainparser.add_subparsers()
 
         default_options_parser = ArgumentParser(add_help=False)
@@ -151,18 +233,14 @@
             group.add_argument(
                 "--version",
                 action="version",
                 version="%(prog)s " + version,
                 help="Show program version number and exit.",
             )
 
-        common_options_parser = ArgumentParser(add_help=False)
-        group = common_options_parser.add_argument_group(STANDARD_ARGUMENTS_GROUP_TITLE)
-        group.add_argument("--log-level", default="INFO", help="Set logging level.")
-
         # Discover CLIs
         CommandInfo = namedtuple("CommandInfo", ["module", "commands"])
 
         def find_commands(name: str, path: List[str]) -> Dict[str, CommandInfo]:
             commands = {}
             module_infos = [
                 (basename, ispkg)
@@ -171,16 +249,15 @@
             ]
             for basename, ispkg in module_infos:
                 module_name = ".".join([name, basename])
                 command_name = basename.replace("_", "-")
                 commands[command_name] = CommandInfo(
                     module=module_name,
                     commands=find_commands(
-                        name=module_name,
-                        path=[os.path.join(prefix, basename) for prefix in path],
+                        name=module_name, path=[os.path.join(prefix, basename) for prefix in path]
                     )
                     if ispkg
                     else None,
                 )
             return commands
 
         if subcommands:
@@ -228,23 +305,21 @@
                 if command_info.commands is None:
                     parser_fn = getattr(module, "parser")
                     parser = parser_fn(add_help=False)
                     func = getattr(module, "func")
                     func = _func_wrapper(func=func, init=getattr(module, "init", None))
                     subparsers.add_parser(
                         command_name,
-                        parents=[parser, default_options_parser, common_options_parser],
+                        parents=[parser, default_options_parser],
                         help=parser.description,
                     ).set_defaults(func=func)
                 else:
                     add_commands(
                         subparsers.add_parser(
-                            command_name,
-                            parents=[default_options_parser],
-                            help=module.__doc__,
+                            command_name, parents=[default_options_parser], help=module.__doc__
                         ).add_subparsers(),
                         command_info.commands,
                         argv[1:],
                     )
             else:
                 for command_name, command_info in commands.items():
                     subparsers.add_parser(
@@ -255,20 +330,18 @@
 
         add_commands(subparsers, commands, argv)
 
         # Parse command arguments and call requested subcommand function
         args, unknown = mainparser.parse_known_args(argv)
 
         if hasattr(args, "func"):
-            log.setLevel(args.log_level)
-            log.info("")  # Make the console output stand out
             try:
                 exit_code = args.func(args, unknown)
             except KeyboardInterrupt:
-                log.debug("Execution interrupted by user")
+                sys.stderr.write("Interrupted by user\n")
                 exit_code = 1
         else:
             mainparser.print_usage()
             exit_code = 1
 
         return exit_code
 
@@ -321,16 +394,15 @@
         return exit_code
 
     # Return closure
     return main
 
 
 def _func_wrapper(
-    func: Callable[[ParsedArguments], int],
-    init: Callable[[ParsedArguments], int] = None,
+    func: Callable[[ParsedArguments], int], init: Callable[[ParsedArguments], int] = None
 ) -> Callable[[ParsedArguments], int]:
     r"""Wrap command 'init' and 'func' callables."""
 
     nparams = len(inspect.signature(func).parameters)
     assert nparams == 1 or nparams == 2, "func() must have one or two parameters"
 
     def call_init_then_func(args: ParsedArguments, unknown: UnknownArguments = []) -> int:
@@ -353,7 +425,43 @@
     r"""Get Python package name given CLI module __name__."""
     parts = []
     for part in module.split("."):
         if part in ("app", "apps", "cli"):
             break
         parts.append(part)
     return ".".join(parts)
+
+
+def bool_from_arg(arg: BoolStr) -> bool:
+    r"""Convert string argument to boolean value."""
+    if arg in TRUE:
+        return True
+    if arg in FALSE:
+        return False
+    raise ValueError("bool_from_arg() 'arg' must be valid boolean string argument")
+
+
+def memory_from_arg(arg: Union[int, str, None]) -> int:
+    r"""Parse --memory option argument.
+
+    Args:
+        arg: Amount of memory. If None, returns the total available memory.
+
+    Returns:
+        Amount of memory in number of bytes.
+
+    """
+    if arg is None:
+        return memory_limit()
+    if isinstance(arg, int):
+        return arg
+    if not isinstance(arg, str):
+        raise TypeError("memory_from_arg() 'arg' must be int or str")
+    if arg.endswith("B"):
+        return int(arg[:-1])
+    if arg.endswith("K"):
+        return int(float(arg[:-1]) * 1024)
+    if arg.endswith("M"):
+        return int(float(arg[:-1]) * 1024**2)
+    if arg.endswith("G"):
+        return int(float(arg[:-1]) * 1024**3)
+    return int(arg)
```

### Comparing `hf-deepali-0.3.2/src/deepali/utils/cli/environ.py` & `hf-deepali-0.4.0/src/deepali/core/environ.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-r"""Auxiliary functions relating to parsing or setting up environment variables."""
+r"""Utilities for parsing and setting up of common environment variables."""
 
 import os
 import re
 from typing import Optional, Tuple
 
 
 def cuda_visible_devices() -> Tuple[int, ...]:
@@ -32,13 +32,34 @@
     r"""Check if CUDA_VISIBLE_DEVICES environment variable is set."""
     gpu_ids = cuda_visible_devices()
     if num and len(gpu_ids) != num:
         raise RuntimeError(f"CUDA_VISIBLE_DEVICES must be set to {num} GPUs")
     return len(gpu_ids)
 
 
+def init_num_threads(threads: int) -> None:
+    r"""Set environment variables used to limit number of process threads."""
+    if threads < 0:
+        raise ValueError("init_num_threads() 'threads' must not be negative")
+    threads = max(1, int(threads))
+    for env in (
+        "ITK_GLOBAL_DEFAULT_NUMBER_OF_THREADS",
+        "MKL_NUM_THREADS",
+        "NUMEXPR_NUM_THREADS",
+        "OMP_NUM_THREADS",
+    ):
+        os.environ[env] = str(threads)
+    try:
+        import SimpleITK as sitk
+
+        sitk.ProcessObject.SetGlobalDefaultNumberOfThreads(threads)
+    except ImportError:
+        pass
+
+
 def init_omp_num_threads(threads: Optional[int] = None, default: int = 1) -> int:
+    r"""Set environment variable OMP_NUM_THREADS to limit number of process threads."""
     if threads is None or threads < 0:
         threads = os.environ.get("OMP_NUM_THREADS", default)
     threads = max(1, int(threads))
     os.environ["OMP_NUM_THREADS"] = str(threads)
     return threads
```

### Comparing `hf-deepali-0.3.2/src/deepali/utils/ignite/handlers.py` & `hf-deepali-0.4.0/src/deepali/utils/ignite/handlers.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 from ignite.engine import Engine, Events, State
 from torch import Tensor
 from torch.nn.modules import Module
 from torch.optim.optimizer import Optimizer
 from torch.utils.data import BatchSampler, DataLoader
 from torch.utils.tensorboard import SummaryWriter
 
-from ...core import RE_OUTPUT_KEY_INDEX
-from ..tensorboard import escape_channel_index_format_string, add_summary_images
+from deepali.core.collections import re_output_key_index
+from deepali.utils.tensorboard import escape_channel_index_format_string, add_summary_images
 
 
 def clamp_learning_rate(
     engine: Engine,
     optimizer: Optimizer,
     min_learning_rate: Optional[float] = None,
     max_learning_rate: Optional[float] = None,
@@ -230,18 +230,18 @@
     elif callable(channel_offset):
         channel_offset_value = channel_offset(engine)
     elif channel_offset is not False:
         raise TypeError("write_summary_images() 'channel_offset' must be bool or callable")
     # Format tag strings
     prefix = format_tag(prefix or "")
     if isinstance(names, dict):
-        names = {RE_OUTPUT_KEY_INDEX.sub(r".\1", name): tag for name, tag in names.items()}
+        names = {re_output_key_index.sub(r".\1", name): tag for name, tag in names.items()}
         names = {name: format_tag(tag) for name, tag in names.items()}
     elif names is not None:
-        names = {RE_OUTPUT_KEY_INDEX.sub(r".\1", name) for name in names}
+        names = {re_output_key_index.sub(r".\1", name) for name in names}
         names = {format_tag(name) for name in names}
     # Input batch
     batch = engine.state.batch
     if isinstance(batch, Tensor):
         batch = {"batch": batch}
     batch = filter_images(batch)
     add_summary_images(
```

### Comparing `hf-deepali-0.3.2/src/deepali/utils/ignite/metrics/average_loss.py` & `hf-deepali-0.4.0/src/deepali/utils/ignite/metrics/average_loss.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.2/src/deepali/utils/ignite/metrics/binary_classification.py` & `hf-deepali-0.4.0/src/deepali/utils/ignite/metrics/binary_classification.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.2/src/deepali/utils/ignite/metrics/multilabel_classification.py` & `hf-deepali-0.4.0/src/deepali/utils/ignite/metrics/multilabel_classification.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.2/src/deepali/utils/ignite/output_transforms.py` & `hf-deepali-0.4.0/src/deepali/utils/ignite/output_transforms.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,17 +3,18 @@
 from typing import Callable, Optional, Sequence, Tuple, Union
 
 from ignite.engine import Engine
 
 import torch
 from torch import Tensor
 
-from ...core.image import grid_reshape
-from ...core.tensor import as_one_hot_tensor
-from ...core import ALIGN_CORNERS, TensorCollection, get_tensor
+from deepali.core import ALIGN_CORNERS
+from deepali.core.collections import TensorCollection, get_tensor
+from deepali.core.image import grid_reshape
+from deepali.core.tensor import as_one_hot_tensor
 
 
 def get_output_transform(key: str) -> Callable[[TensorCollection], Tensor]:
     r"""Get tensor at specified nested engine output map key entry."""
 
     def output_transform(output: TensorCollection) -> Tensor:
         return get_tensor(output, key)
@@ -37,15 +38,14 @@
     Returns:
         y_pred: Tensor of one-hot encoded predictions with shape ``(N, 2, ..., X)``.
         y: Tensor of target labels with shape ``(N, ..., X)``.
 
     """
 
     def output_transform(output: TensorCollection) -> Tuple[Tensor, Tensor]:
-
         dtype = torch.int32
         y_pred_tensor = get_tensor(output, y_pred)
         y_tensor = get_tensor(output, y)
         assert y_tensor.ndim == y_pred_tensor.ndim
         assert y_tensor.shape[1] == 1
         if y_tensor.shape[0] == 1 and y_pred_tensor.shape[0] > 1:
             y_tensor = y_tensor.expand(y_pred_tensor.shape[0:1] + y_tensor.shape[1:])
```

### Comparing `hf-deepali-0.3.2/src/deepali/utils/ignite/score_functions.py` & `hf-deepali-0.4.0/src/deepali/utils/ignite/score_functions.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from typing import Mapping
 
 from ignite.engine import Engine
 
 from torch import Tensor
 
-from ...core import get_tensor
+from deepali.core.collections import get_tensor
 
 
 def negative_loss_score_function(engine: Engine, key: str = "loss") -> Tensor:
     r"""Get negated loss value from ``engine.state.output``."""
     output = engine.state.output
     if isinstance(output, Mapping):
         loss = get_tensor(output, key)
```

### Comparing `hf-deepali-0.3.2/src/deepali/utils/sitk/grid.py` & `hf-deepali-0.4.0/src/deepali/utils/simpleitk/grid.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,298 +1,345 @@
-r"""Auxiliary functions for working with oriented image data."""
+r"""Attributes of data sampling grid oriented in space."""
 
 import itertools
-from pathlib import Path
-from typing import Sequence, Tuple, Union, Optional
+from typing import Sequence, Tuple, TypeVar, Union, Optional
 
 import numpy as np
+from numpy.typing import ArrayLike, NDArray
 import SimpleITK as sitk
 
-Coords = Union[np.ndarray, Sequence[float]]
 
+TGridAttrs = TypeVar("TGridAttrs", bound="GridAttrs")
 
-class Grid(object):
-    r"""Finite and discrete image sampling grid oriented in world space."""
+
+class GridAttrs(object):
+    r"""Attributes of a regular data sampling grid oriented in world space."""
 
     __slots__ = ["_size", "origin", "spacing", "direction"]
 
     def __init__(
         self,
-        size: Tuple[Union[int, float], ...],
-        origin: Optional[Tuple[float, ...]] = None,
-        spacing: Optional[Tuple[float, ...]] = None,
-        direction: Optional[Tuple[float, ...]] = None,
-    ):
+        size: Sequence[Union[float, int]],
+        center: Optional[Sequence[float]] = None,
+        origin: Optional[Sequence[float]] = None,
+        spacing: Optional[Sequence[float]] = None,
+        direction: Optional[Union[Sequence[float], Sequence[Sequence[float]]]] = None,
+    ) -> None:
+        r"""Initialize grid attributes.
+
+        Note that the order of spatial dimensions of the attributes is ``(X, ...)``,
+        whereas the data arrays often are given in reverse order, i.e., the shape of a
+        corresponding data array is ``(..., X)``.
+
+        Args:
+            size: Size of spatial grid dimensions. The length determines the number of dimensions.
+            center: Grid center point coordinates in world space along each dimension.
+            origin: World coordinates of grid point with index zero along each dimension.
+            spacing: Spacing between grid points along each dimension.
+            direction: Direction cosines. Must be a square matrix, but can be flattened.
+
+        """
         ndim = len(size)
-        if origin is None:
-            origin = (0.0,) * ndim
-        elif not isinstance(origin, tuple):
-            origin = tuple(origin)
         if spacing is None:
             spacing = (1.0,) * ndim
         elif not isinstance(spacing, tuple):
             spacing = tuple(spacing)
         if direction is None:
             direction = np.eye(ndim, ndim)
-        if isinstance(direction, np.ndarray):
-            direction = direction.flatten().astype(float)
-        if not isinstance(direction, tuple):
-            direction = tuple(direction)
-        self._size = tuple(
-            float(n) for n in size
-        )  # store as float s.t., grid.down().up() restores original grid
+        direction = tuple(float(x) for x in np.asanyarray(direction).flatten())
+        if origin is None:
+            if center is None:
+                origin = (0.0,) * ndim
+            else:
+                offset = np.array(0.5 * n if n > 0 else 0 for n in self._int_size(size))
+                rotation = np.array(self.direction).reshape(ndim, ndim)
+                scaling = np.diag(spacing)
+                coords: NDArray = np.asanyarray(center) - np.matmul(rotation @ scaling, offset)
+                origin = tuple(float(x) for x in coords)
+        elif center is not None:
+            raise ValueError("Grid() 'center' and 'origin' are mutually exclusive")
+        elif not isinstance(origin, tuple):
+            origin = tuple(origin)
+        # store grid size as float such that grid.down().up() restores original grid
+        self._size = tuple(float(n) for n in size)
         self.origin = origin
         self.spacing = spacing
         self.direction = direction
 
     @property
+    def center(self) -> Tuple[float, ...]:
+        r"""Get grid center point coordinates in world space."""
+        offset = np.array(0.5 * n if n > 0 else 0 for n in self.size)
+        coords: NDArray = self.origin + np.matmul(self.transform[:-1, :-1], offset)
+        return tuple(float(x) for x in coords)
+
+    @property
     def ndim(self) -> int:
-        """Number of image grid dimensions."""
+        r"""Number of spatial grid dimensions."""
         return len(self.shape)
 
     @property
-    def npts(self) -> int:
-        """Total number of image grid points."""
+    def npoints(self) -> int:
+        r"""Total number of grid points."""
         return int(np.prod(self.size))
 
     @staticmethod
     def _int_size(size) -> Tuple[int, ...]:
         """Get grid size from internal floating point representation."""
         return tuple([int(n + 0.5) if n > 1 or n <= 0 else 1 for n in size])
 
     @property
     def size(self) -> Tuple[int, ...]:
-        """Size of image data array."""
+        r"""Size of sampling grid with spatial dimensions in the order (X, ...)."""
         return self._int_size(self._size)
 
     @property
     def shape(self) -> Tuple[int, ...]:
-        """Shape of image data array."""
+        r"""Shape of sampling grid with spatial dimensions in the order (..., X)."""
         return tuple(reversed(self.size))
 
-    @classmethod
-    def from_file(cls, path: Union[Path, str]):
-        reader = sitk.ImageFileReader()
-        reader.SetFileName(str(path))
-        reader.ReadImageInformation()
-        return cls.from_reader(reader)
-
-    @classmethod
-    def from_reader(cls, reader: sitk.ImageFileReader):
-        return cls(
-            size=reader.GetSize(),
-            origin=reader.GetOrigin(),
-            spacing=reader.GetSpacing(),
-            direction=reader.GetDirection(),
-        )
-
-    @classmethod
-    def from_image(cls, image: sitk.Image):
-        return cls(
-            size=image.GetSize(),
-            origin=image.GetOrigin(),
-            spacing=image.GetSpacing(),
-            direction=image.GetDirection(),
-        )
-
-    def zeros_image(self, dtype: int = sitk.sitkInt16, channels: int = 1):
-        r"""Create empty image from grid."""
-        img = sitk.Image(self.size, dtype, channels)
-        img.SetOrigin(self.origin)
-        img.SetDirection(self.direction)
-        img.SetSpacing(self.spacing)
-        return img
-
-    def with_margin(self, margin: int):
-        """Create new image grid with an additional margin along each grid axis."""
+    def with_margin(self: TGridAttrs, margin: Union[int, None]) -> TGridAttrs:
+        r"""Create new image grid with an additional margin along each grid axis."""
         if not margin:
             return self
-        return self.__class__(
+        cls = type(self)
+        return cls(
             size=tuple(n + 2 * margin for n in self._size),
             origin=self.index_to_physical_space((-margin,) * self.ndim),
             spacing=self.spacing,
             direction=self.direction,
         )
 
-    def with_spacing(self, *args: float):
-        """Create new image grid with specified spacing."""
+    def with_spacing(self: TGridAttrs, *args: float) -> TGridAttrs:
+        r"""Create new image grid with specified spacing."""
+        cls = type(self)
         spacing = np.asarray(*args)
         assert 0 <= spacing.ndim <= 1
         if spacing.ndim == 0:
             spacing = spacing.repeat(self.ndim)
         assert spacing.size == self.ndim
         cur_size = np.asarray(self._size)
         cur_spacing = np.asarray(self.spacing)
         size = cur_size * cur_spacing / spacing
         shift = 0.5 * (np.round(cur_size) - np.round(size) * spacing / cur_spacing)
         origin = self.index_to_physical_space(shift)
-        return self.__class__(size=size, origin=origin, spacing=spacing, direction=self.direction)
+        return cls(size=size, origin=origin, spacing=spacing, direction=self.direction)
 
-    def down(self, levels: int = 1):
-        """Create new image grid of half the size."""
+    def down(self: TGridAttrs, levels: int = 1) -> TGridAttrs:
+        r"""Create new sampling grid of half the size while preserving grid extent."""
+        cls = type(self)
         size = self._size
         for _ in range(levels):
             size = tuple(n / 2 for n in size)
         cur_size = self.size
         new_size = self._int_size(size)
         spacing = tuple(
             self.spacing[i] * cur_size[i] / new_size[i] if new_size[i] > 0 else self.spacing[i]
             for i in range(self.ndim)
         )
-        return self.__class__(size=size, spacing=spacing)
+        return cls(size=size, center=self.center, spacing=spacing, direction=self.direction)
 
-    def up(self, levels: int = 1):
-        """Create new image grid of double the size."""
+    def up(self: TGridAttrs, levels: int = 1) -> TGridAttrs:
+        r"""Create new sampling grid of double the size while preserving grid extent."""
+        cls = type(self)
         size = self._size
         for _ in range(levels):
             size = tuple(2 * n for n in size)
         cur_size = self.size
         new_size = self._int_size(size)
         spacing = tuple(
             self.spacing[i] * cur_size[i] / new_size[i] if new_size[i] > 0 else self.spacing[i]
             for i in range(self.ndim)
         )
-        return self.__class__(size=size, spacing=spacing)
+        return cls(size=size, center=self.center, spacing=spacing, direction=self.direction)
 
     @property
     def dcm(self) -> np.ndarray:
-        """Get direction cosine matrix."""
+        r"""Get direction cosine matrix."""
         return np.array(self.direction).reshape(self.ndim, self.ndim)
 
     @property
     def transform(self) -> np.ndarray:
-        """Get homogeneous coordinate transformation from image grid to world space."""
+        r"""Get homogeneous coordinate transformation from image grid to world space."""
         rotation = self.dcm
         scaling = np.diag(self.spacing)
         matrix = homogeneous_matrix(rotation @ scaling)
         matrix[0:-1, -1] = self.origin
         return matrix
 
     @property
     def inverse_transform(self) -> np.ndarray:
-        """Get homogeneous coordinate transformation from world space to image grid."""
+        r"""Get homogeneous coordinate transformation from world space to image grid."""
         rotation = self.dcm.T
         scaling = np.diag([1 / s for s in self.spacing])
         translation = translation_matrix([-t for t in self.origin])
         return homogeneous_matrix(scaling @ rotation) @ translation
 
     @property
     def indices(self) -> np.ndarray:
-        """Get array of image grid point coordinates in image space."""
+        r"""Get array of image grid point coordinates in image space."""
         return np.flip(
             np.stack(
                 np.meshgrid(*[np.arange(arg) for arg in self.shape], indexing="ij"),
                 axis=self.ndim,
             ),
             axis=-1,
         )
 
     def axis_indices(self, axis: int) -> np.ndarray:
-        """Get array of image grid indices along specified axis."""
+        r"""Get array of image grid indices along specified axis."""
         return np.arange(self.shape[axis])
 
     @property
     def points(self) -> np.ndarray:
-        """Get array of image grid point coordinates in world space."""
+        r"""Get array of image grid point coordinates in world space."""
         return self.index_to_physical_space(self.indices)
 
     @property
     def coords(self) -> Tuple[np.ndarray, ...]:
-        """Get 1D arrays of grid point coordinates along each axis."""
+        r"""Get 1D arrays of grid point coordinates along each axis."""
         return tuple(self.axis_coords(axis) for axis in range(self.ndim))
 
     def axis_coords(self, axis: int) -> np.ndarray:
-        """Get array of image grid point coordinates in world space along specified axis."""
+        r"""Get array of image grid point coordinates in world space along specified axis."""
         indices = [[0]] * self.ndim
         indices[axis] = [index for index in range(self.shape[axis])]
         mesh = np.stack(np.meshgrid(*indices, indexing="ij"), axis=self.ndim)
         return self.index_to_physical_space(mesh)[..., axis].flatten()
 
     @property
     def corners(self) -> np.ndarray:
-        """Get corners of image domain in world space."""
+        r"""Get corners of image domain in world space."""
         limits = []
         for axis in range(self.ndim):
             limits.append((0, self.shape[axis]))
         corners = [tuple(reversed(indices)) for indices in itertools.product(*limits)]
         return self.index_to_physical_space(corners)
 
-    def index_to_physical_space(self, points: Coords) -> np.ndarray:
-        """Map point coordinates from image to world space."""
+    def index_to_physical_space(self, points: ArrayLike) -> np.ndarray:
+        r"""Map point coordinates from image to world space.
+
+        Args:
+            points: Input voxel indices as n-dimensional array of shape ``(..., D)``.
+                The input can be both integral or floating point indices.
+
+        Returns:
+            World coordinates of the indexed grid locations.
+
+        """
         return transform_point(self.transform, points)
 
-    def physical_space_to_index(self, points: Coords) -> np.ndarray:
-        """Map point coordinates from world to discrete image space."""
-        return np.round(self.physical_space_to_continuous_index(points)).astype(int)
+    def physical_space_to_index(self, points: ArrayLike) -> np.ndarray:
+        r"""Map point coordinates from world to discrete image space.
+
+        Args:
+            points: World coordinates of input points given as n-dimensional array of shape ``(..., D)``.
+
+        Returns:
+            Integral indices of nearest grid points.
+
+        """
+        index: np.ndarray = np.round(self.physical_space_to_continuous_index(points))
+        return index.astype(int)
 
-    def physical_space_to_continuous_index(self, points: Coords) -> np.ndarray:
-        """Map point coordinates from world to continuous image space."""
+    def physical_space_to_continuous_index(self, points: ArrayLike) -> np.ndarray:
+        r"""Map point coordinates from world to continuous image space.
+
+        Args:
+            points: World coordinates of input points given as n-dimensional array of shape ``(..., D)``.
+
+        Returns:
+            Indices of grid locations as floating point values.
+
+        """
         # Round to avoid 1e-15, 1e-17, -1e-14,... as representations for zero, s.t.,
         # indices == physical_space_to_continuous_index(index_to_physical_space(indices))
         return np.round(transform_point(self.inverse_transform, points), decimals=12)
 
     def __repr__(self) -> str:
         return (
-            self.__class__.__name__
-            + "(size={size}, origin={origin}, spacing={spacing}, direction={direction})".format(
-                size=self.size,
-                origin=self.origin,
-                spacing=self.spacing,
-                direction=self.direction,
-            )
+            f"{type(self).__name__}("
+            f"size={self.size}"
+            f", origin={self.origin}"
+            f", spacing={self.spacing}"
+            f", direction={self.direction}"
+            ")"
         )
 
 
+def image_grid_attributes(image: sitk.Image) -> GridAttrs:
+    r"""Get image sampling grid attributes."""
+    return GridAttrs(
+        size=image.GetSize(),
+        origin=image.GetOrigin(),
+        spacing=image.GetSpacing(),
+        direction=image.GetDirection(),
+    )
+
+
 def homogeneous_coords(point: np.ndarray, ndim: int = None, copy: bool = True) -> np.ndarray:
-    """Create array with homogeneous point coordinates."""
+    r"""Create array of homogeneous point coordinates from D-dimensional point set.
+
+    Args:
+        point: Input point or point set as array of shape ``(..., D)``.
+        ndim: Expected number of spatial dimensions. If specified, and the input ``point``
+            array is of shape ``(..., ndim + 1)``, the input point array is returned
+            without adding an additional dimension.
+        copy: Whether to copy the input ``point`` array when ``ndim`` is specified and
+            the shape of the input array is ``(..., ndim + 1)``.
+
+    Returns:
+        Array of homogeneous coordinates with shape ``(..., D + 1)``.
+
+    """
     if ndim is not None:
         if point.shape[-1] == ndim + 1:
             return np.copy(point) if copy else point
         assert point.shape[-1] == ndim
     # Creating new array with submatrix assignment is faster than np.hstack!
     pts = np.ones(point.shape[0:-1] + (point.shape[-1] + 1,), dtype=point.dtype)
     pts[..., :-1] = point
     return pts
 
 
 def homogeneous_matrix(transform: np.ndarray, ndim: int = None, copy: bool = True) -> np.ndarray:
-    """Create homogeneous transformation matrix from affine coordinate transformation."""
+    r"""Create homogeneous transformation matrix from affine coordinate transformation."""
     assert transform.ndim == 2
     rows, cols = transform.shape
     if ndim is None:
         ndim = rows
         assert (
             transform.shape[1] == ndim or transform.shape[1] == ndim + 1
         ), "transform.shape={}".format(transform.shape)
     elif rows == ndim + 1 and cols == ndim + 1:
         return np.copy(transform) if copy else transform
     matrix = np.eye(ndim + 1, ndim + 1, dtype=transform.dtype)
     matrix[0:rows, 0:cols] = transform
     return matrix
 
 
-def translation_matrix(displacement: Sequence[float]) -> np.ndarray:
-    """Create translation matrix for homogeneous coordinates."""
-    displacement = np.asanyarray(displacement)
-    assert displacement.ndim == 1
-    matrix = np.eye(displacement.size + 1)
-    matrix[0:-1, -1] = displacement
+def translation_matrix(displacement: ArrayLike) -> np.ndarray:
+    r"""Create translation matrix for homogeneous coordinates."""
+    arg = np.asanyarray(displacement)
+    assert arg.ndim == 1
+    matrix = np.eye(arg.size + 1)
+    matrix[0:-1, -1] = arg
     return matrix
 
 
-def transform_point(matrix: np.ndarray, point: np.ndarray) -> np.ndarray:
-    """Transform one or more points given a transformation matrix."""
-    pts = np.asanyarray(point)
-    dim = pts.shape[-1]
+def transform_point(matrix: np.ndarray, point: ArrayLike) -> np.ndarray:
+    r"""Transform one or more points given a transformation matrix."""
+    arg = np.asanyarray(point)
+    dim = arg.shape[-1]
     mat = homogeneous_matrix(matrix, ndim=dim, copy=False)
-    x = pts.reshape(-1, dim)
-    y = np.matmul(x, mat[0:-1, 0:-1].T) + np.expand_dims(mat[0:-1, -1], axis=0)
-    return y.reshape(pts.shape)
+    x = arg.reshape(-1, dim)
+    y: np.ndarray = np.matmul(x, mat[0:-1, 0:-1].T) + np.expand_dims(mat[0:-1, -1], axis=0)
+    return y.reshape(arg.shape)
 
 
-def transform_vector(matrix: np.ndarray, vector: np.ndarray) -> np.ndarray:
-    """Transform one or more vectors given a transformation matrix."""
-    vec = np.asanyarray(vector)
-    dim = vec.shape[-1]
-    v = vec.reshape(-1, dim)
-    u = np.matmul(v, matrix[0:dim, 0:dim].T)
-    return u.reshape(vec.shape)
+def transform_vector(matrix: np.ndarray, vector: ArrayLike) -> np.ndarray:
+    r"""Transform one or more vectors given a transformation matrix."""
+    arg = np.asanyarray(vector)
+    dim = arg.shape[-1]
+    v = arg.reshape(-1, dim)
+    u: np.ndarray = np.matmul(v, matrix[0:dim, 0:dim].T)
+    return u.reshape(arg.shape)
```

### Comparing `hf-deepali-0.3.2/src/deepali/utils/sitk/numpy.py` & `hf-deepali-0.4.0/src/deepali/utils/simpleitk/numpy.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.2/src/deepali/utils/sitk/sample.py` & `hf-deepali-0.4.0/src/deepali/utils/simpleitk/sample.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 
 import numpy as np
 import scipy.interpolate
 import scipy.ndimage
 import scipy.spatial
 import SimpleITK as sitk
 
-from .grid import Grid
+from .grid import GridAttrs, image_grid_attributes
 
 
 def resample_image(
     image: sitk.Image,
-    reference: Union[Grid, sitk.Image],
+    reference: Union[GridAttrs, sitk.Image],
     interpolator: int = sitk.sitkLinear,
     padding_value: float = 0,
 ) -> sitk.Image:
     r"""Interpolate image values at grid points of reference image.
 
     Args:
         image: Scalar or vector-valued image to evaluate at the specified points.
@@ -89,15 +89,15 @@
     # )
 
 
 def interpolate_ndimage(
     image: sitk.Image, points: np.ndarray, padding_value: float = 0, order: int = 1
 ) -> np.ndarray:
     r"""Use ``scipy.ndimage.map_coordinates`` to interpolate image."""
-    grid = Grid.from_image(image)
+    grid = image_grid_attributes(image)
     idxs = np.moveaxis(grid.physical_space_to_continuous_index(points), -1, 0)
     idxs = np.flip(idxs, axis=0)
     vals = sitk.GetArrayViewFromImage(image)
     nval = image.GetNumberOfComponentsPerPixel()
     if nval > 1:
         out = np.stack(
             [
@@ -112,15 +112,15 @@
 
 
 def interpolate_regular_grid(
     image: sitk.Image, points: np.ndarray, padding_value: float = 0
 ) -> np.ndarray:
     r"""Use ``scipy.interpolate.RegularGridInterpolator`` to interpolate image data."""
     size = points.shape[0:-1]
-    grid = Grid.from_image(image)
+    grid = image_grid_attributes(image)
     vals = sitk.GetArrayViewFromImage(image)
     nval = image.GetNumberOfComponentsPerPixel()
     idxs = grid.physical_space_to_continuous_index(points.reshape(-1, grid.ndim))
     idxs = np.flip(idxs, axis=-1)
     coords = tuple(np.arange(vals.shape[axis]) for axis in range(grid.ndim))
     if nval > 1:
         out = []
@@ -143,15 +143,15 @@
 
     This method should only be used for comparison. The used Delaunay triangulation
     is not suited for interpolating image data sampled on a regular grid.
 
     Use ``warp_image`` (for regularly spaced ``points``) or ``interpolate_image``.
     """
     size = points.shape[0:-1]
-    grid = Grid.from_image(image)
+    grid = image_grid_attributes(image)
     tess = scipy.spatial.qhull.Delaunay(grid.points.reshape(-1, grid.ndim))
     vals = sitk.GetArrayViewFromImage(image)
     nval = image.GetNumberOfComponentsPerPixel()
     coor = points.reshape(-1, grid.ndim)
     if nval > 1:
         out = []
         for c in range(nval):
```

### Comparing `hf-deepali-0.3.2/src/deepali/utils/sitk/torch.py` & `hf-deepali-0.4.0/src/deepali/utils/simpleitk/torch.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.2/src/deepali/utils/tensorboard.py` & `hf-deepali-0.4.0/src/deepali/utils/tensorboard.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import re
 from typing import Callable, Optional, Union
 
 from torch import Tensor
 from torch.utils.tensorboard import SummaryWriter
 
 from ..core.image import normalize_image
-from ..core.types import TensorCollection
+from ..core.typing import TensorCollection
 
 
 RE_CHANNEL_INDEX = re.compile(r"\{c(:[^}]+)?\}")
 
 
 def escape_channel_index_format_string(tag: str) -> str:
     r"""Escape image channel index format before str.format() call."""
```

### Comparing `hf-deepali-0.3.2/src/deepali/utils/vtk/idlist.py` & `hf-deepali-0.4.0/src/deepali/utils/vtk/idlist.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.2/src/deepali/utils/vtk/image.py` & `hf-deepali-0.4.0/src/deepali/utils/vtk/image.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,16 @@
     vtkImageStencilToImage,
     vtkMatrixToLinearTransform,
     vtkPolyData,
     vtkPolyDataToImageStencil,
     vtkTransformPolyDataFilter,
 )
 
-from ..sitk.grid import Grid  # TODO: Make Grid independent of SimpleITK
+from deepali.core.grid import Grid
+
 from .numpy import numpy_to_vtk_matrix4x4
 
 
 def surface_mesh_grid(*mesh: vtkPolyData, resolution: Optional[float] = None) -> Grid:
     r"""Compute image grid for given surface mesh discretization with specified resolution."""
     # Common bounds of mesh points
     #
@@ -38,30 +39,32 @@
         origin=bounds[0::2] + 0.5 * resolution,
         spacing=np.asarray([resolution] * 3),
     )
 
 
 def surface_image_stencil(mesh: vtkPolyData, grid: Grid) -> vtkImageStencilData:
     r"""Convert vtkPolyData surface mesh to image stencil."""
+    max_index = [n - 1 for n in grid.size().tolist()]
+
     rot = np.eye(4, dtype=np.float)
     rot[:3, :3] = np.array(grid.direction).reshape(3, 3)
     rot = numpy_to_vtk_matrix4x4(rot)
 
     transform = vtkMatrixToLinearTransform()
     transform.SetInput(rot)
 
     transformer = vtkTransformPolyDataFilter()
     transformer.SetInputData(mesh)
     transformer.SetTransform(transform)
 
     converter = vtkPolyDataToImageStencil()
     converter.SetInputConnection(transformer.GetOutputPort())
-    converter.SetOutputOrigin(grid.origin)
-    converter.SetOutputSpacing(grid.spacing)
-    converter.SetOutputWholeExtent([0, grid.size[0] - 1, 0, grid.size[1] - 1, 0, grid.size[2] - 1])
+    converter.SetOutputOrigin(grid.origin().tolist())
+    converter.SetOutputSpacing(grid.spacing().tolist())
+    converter.SetOutputWholeExtent([0, max_index[0], 0, max_index[1], 0, max_index[2]])
     converter.Update()
 
     stencil = vtkImageStencilData()
     stencil.DeepCopy(converter.GetOutput())
     return stencil
```

### Comparing `hf-deepali-0.3.2/src/deepali/utils/vtk/numpy.py` & `hf-deepali-0.4.0/src/deepali/utils/vtk/numpy.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.2/src/deepali/utils/vtk/polydataio.py` & `hf-deepali-0.4.0/src/deepali/utils/vtk/polydataio.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,120 +1,126 @@
 r"""Auxiliary functions for working with vtkPolyData."""
 
 from io import StringIO
-from pathlib import Path
-from typing import List, Tuple, Union
+from typing import List, Tuple
 
 import numpy as np
 
 from vtk import vtkCellArray, vtkPoints, vtkPolyData
+from vtk import vtkOBJReader, vtkOBJWriter
 from vtk import vtkPLYReader, vtkPLYWriter
 from vtk import vtkXMLPolyDataReader, vtkXMLPolyDataWriter
 from vtk import vtkPolyDataReader, vtkPolyDataWriter
 
-from .numpy import vtk_to_numpy_array, vtk_to_numpy_points
+from deepali.core.pathlib import PathUri
+from deepali.utils.storage import StorageObject
 
-PathStr = Union[Path, str]
+from .numpy import vtk_to_numpy_array, vtk_to_numpy_points
 
 
-def read_polydata(path: PathStr) -> vtkPolyData:
+def read_polydata(path: PathUri) -> vtkPolyData:
     r"""Read vtkPolyData from specified file."""
-    path = Path(path).absolute()
-    if not path.is_file():
-        raise FileNotFoundError(str(path))
-    suffix = path.suffix.lower()
-    if suffix == ".off":
-        return read_polydata_off(path)
-    elif suffix == ".ply":
-        reader = vtkPLYReader()
-    elif suffix == ".vtp":
-        reader = vtkXMLPolyDataReader()
-    elif suffix == ".vtk":
-        reader = vtkPolyDataReader()
-    else:
-        raise ValueError("Unsupported file name extension: {}".format(suffix))
-    reader.SetFileName(str(path))
-    reader.Update()
-    polydata = vtkPolyData()
-    polydata.DeepCopy(reader.GetOutput())
+    with StorageObject.from_path(path) as obj:
+        if not obj.is_file():
+            raise FileNotFoundError(f"File not found: {obj.uri}")
+        obj = obj.pull()
+        if not obj.path.is_file():
+            raise FileNotFoundError(f"File not found: {obj.path}")
+        suffix = obj.path.suffix.lower()
+        if suffix == ".off":
+            return read_polydata_off(obj.path)
+        if suffix == ".obj":
+            reader = vtkOBJReader()
+        elif suffix == ".ply":
+            reader = vtkPLYReader()
+        elif suffix == ".vtp":
+            reader = vtkXMLPolyDataReader()
+        elif suffix == ".vtk":
+            reader = vtkPolyDataReader()
+        else:
+            raise ValueError("Unsupported file name extension: {}".format(suffix))
+        reader.SetFileName(str(obj.path))
+        reader.Update()
+        polydata = vtkPolyData()
+        polydata.DeepCopy(reader.GetOutput())
     return polydata
 
 
-def read_off(path: PathStr) -> Tuple[List[List[float]], List[List[int]]]:
+def read_off(path: PathUri) -> Tuple[List[List[float]], List[List[int]]]:
     r"""Read values from .off file."""
-    data = Path(path).read_text()
+    with StorageObject.from_path(path) as obj:
+        data = obj.read_text()
     stream = StringIO(data)
     magic = stream.readline().strip()
     if magic not in ("OFF", "CNOFF"):
         raise ValueError(f"Invalid OFF file header: {path}")
     header = tuple([int(s) for s in stream.readline().strip().split(" ")])
     n_verts, n_faces = header[:2]
     verts = [[float(s) for s in stream.readline().strip().split(" ")] for _ in range(n_verts)]
     faces = [[int(s) for s in stream.readline().strip().split(" ")] for _ in range(n_faces)]
     assert len(verts) == n_verts, f"Expected {n_verts} vertices, found only {len(verts)}"
     assert len(faces) == n_faces, f"Expected {n_faces} vertices, found only {len(faces)}"
     return verts, faces
 
 
-def read_polydata_off(path: PathStr) -> vtkPolyData:
+def read_polydata_off(path: PathUri) -> vtkPolyData:
     r"""Read vtkPolyData from .off file."""
     verts, faces = read_off(path)
     points = vtkPoints()
     polys = vtkCellArray()
     for vert in verts:
         points.InsertNextPoint(vert[:3])
     for poly in faces:
         polys.InsertNextCell(poly[0], poly[1 : 1 + poly[0]])
     output = vtkPolyData()
     output.SetPoints(points)
     output.SetPolys(polys)
     return output
 
 
-def write_polydata(polydata: vtkPolyData, path: PathStr):
+def write_polydata(polydata: vtkPolyData, path: PathUri):
     r"""Write vtkPolyData to specified file in XML format."""
-    path = Path(path).absolute()
-    suffix = path.suffix.lower()
-    if suffix == ".off":
-        write_polydata_off(polydata, path)
-        return
-    if suffix == ".ply":
-        writer = vtkPLYWriter()
-        writer.SetFileTypeToBinary()
-    elif suffix == ".vtp":
-        writer = vtkXMLPolyDataWriter()
-    elif suffix == ".vtk":
-        writer = vtkPolyDataWriter()
-    else:
-        raise ValueError("Unsupported file name extension: {}".format(suffix))
-    try:
-        path.unlink()  # in case of protected symlink to DVC cache
-    except FileNotFoundError:
-        path.parent.mkdir(parents=True, exist_ok=True)
-    writer.SetFileName(str(path))
-    writer.SetInputData(polydata)
-    writer.Update()
+    with StorageObject.from_path(path) as obj:
+        suffix = obj.path.suffix.lower()
+        if suffix == ".off":
+            write_polydata_off(polydata, obj.path)
+            return
+        if suffix == ".obj":
+            writer = vtkOBJWriter()
+        elif suffix == ".ply":
+            writer = vtkPLYWriter()
+            writer.SetFileTypeToBinary()
+        elif suffix == ".vtp":
+            writer = vtkXMLPolyDataWriter()
+        elif suffix == ".vtk":
+            writer = vtkPolyDataWriter()
+        else:
+            raise ValueError("Unsupported file name extension: {}".format(suffix))
+        try:
+            obj.path.unlink()  # in case of protected symlink to DVC cache
+        except FileNotFoundError:
+            obj.path.parent.mkdir(parents=True, exist_ok=True)
+        writer.SetFileName(str(obj.path))
+        writer.SetInputData(polydata)
+        writer.Update()
+        obj.push(force=True)
 
 
-def write_polydata_off(polydata: vtkPolyData, path: PathStr):
+def write_polydata_off(polydata: vtkPolyData, path: PathUri):
     r"""Write vtkPolyData to specified file in OFF format."""
-    path = Path(path).absolute()
-
-    try:
-        path.unlink()  # in case of protected symlink to DVC cache
-    except FileNotFoundError:
-        path.parent.mkdir(parents=True, exist_ok=True)
-
     verts = vtk_to_numpy_points(polydata)
 
     F = polydata.GetPolys().GetNumberOfCells()
     faces = vtk_to_numpy_array(polydata.GetPolys().GetData())
     assert faces.ndim == 1
     if len(faces) / F != 4:
         raise ValueError("write_polydata_off() only supports triangulated surface meshes")
     faces = faces.reshape(-1, 4)
 
-    with path.open(mode="wt") as fp:
-        fp.write("OFF\n")
-        fp.write(f"{len(verts)} {len(faces)} 0\n")
-        np.savetxt(fp, verts, delimiter=" ", newline="\n", header="", footer="")
-        np.savetxt(fp, faces, delimiter=" ", newline="\n", header="", footer="", fmt="%d")
+    stream = StringIO()
+    stream.write("OFF\n")
+    stream.write(f"{len(verts)} {len(faces)} 0\n")
+    np.savetxt(stream, verts, delimiter=" ", newline="\n", header="", footer="")
+    np.savetxt(stream, faces, delimiter=" ", newline="\n", header="", footer="", fmt="%d")
+
+    with StorageObject.from_path(path) as obj:
+        obj.write_text(stream.getvalue())
```

### Comparing `hf-deepali-0.3.2/src/deepali/utils/vtk/simpleitk.py` & `hf-deepali-0.4.0/src/deepali/utils/vtk/simpleitk.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,17 +13,18 @@
     VTK_UNSIGNED_SHORT,
     VTK_UNSIGNED_LONG,
     VTK_UNSIGNED_LONG_LONG,
     VTK_FLOAT,
     VTK_DOUBLE,
 )
 
+from deepali.utils.simpleitk.grid import GridAttrs
+from deepali.utils.simpleitk.sample import interpolate_ndimage
+
 from .numpy import numpy_to_vtk_array, vtk_to_numpy_array, vtk_to_numpy_points
-from ..sitk.grid import Grid
-from ..sitk.sample import interpolate_ndimage
 
 
 VTK_DATA_TYPE_FROM_SITK_PIXEL_ID = {
     sitk.sitkInt8: VTK_CHAR,
     sitk.sitkInt16: VTK_SHORT,
     sitk.sitkInt32: VTK_LONG,
     sitk.sitkInt64: VTK_LONG_LONG,
@@ -100,18 +101,18 @@
         points = apply_warp_field_to_points(
             warp_field, pointset.GetPoints(), is_def_field=is_def_field
         )
         output.SetPoints(points)
     return output
 
 
-def image_data_grid(data: vtkImageData) -> Grid:
+def image_data_grid(data: vtkImageData) -> GridAttrs:
     r"""Create image grid from vtkImageData object."""
     extent = data.GetExtent()
-    return Grid(
+    return GridAttrs(
         size=(
             extent[1] - extent[0] + 1,
             extent[3] - extent[2] + 1,
             extent[5] - extent[4] + 1,
         ),
         origin=data.GetOrigin(),
         spacing=data.GetSpacing(),
@@ -157,15 +158,15 @@
     importer.SetDataExtentToWholeExtent()
     importer.UpdateWholeExtent()
     output = vtkImageData()
     output.DeepCopy(importer.GetOutput())
     return output
 
 
-def sitk_image_from_vtk_image(image: vtkImageData, grid: Optional[Grid] = None) -> sitk.Image:
+def sitk_image_from_vtk_image(image: vtkImageData, grid: Optional[GridAttrs] = None) -> sitk.Image:
     r"""Create SimpleITK image from vtkImageData."""
     if image.GetNumberOfScalarComponents() != 1:
         raise NotImplementedError("sitk_image_from_vtk_image() only supports scalar 'image'")
     data = image.GetPointData().GetScalars()
     data = vtk_to_numpy_array(data)
     data = data.reshape(tuple(reversed(grid.size)))
     output = sitk.GetImageFromArray(data)
```

### Comparing `hf-deepali-0.3.2/src/hf_deepali.egg-info/PKG-INFO` & `hf-deepali-0.4.0/src/hf_deepali.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hf-deepali
-Version: 0.3.2
+Version: 0.4.0
 Summary: Image, point set, and surface registration library for PyTorch.
 Maintainer-email: Andreas Schuh <andreas.schuh@imperial.ac.uk>
 License: Apache-2.0
 Project-URL: Homepage, https://biomedia.github.io/deepali
 Project-URL: Repository, https://github.com/BioMedIA/deepali.git
 Project-URL: Bug Tracker, https://github.com/BioMedIA/deepali/issues
 Keywords: medical-imaging,image-registration,spatial-transformer-networks
```

### Comparing `hf-deepali-0.3.2/src/hf_deepali.egg-info/SOURCES.txt` & `hf-deepali-0.4.0/src/hf_deepali.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 .dockerignore
 .flake8
 .gitignore
+CITATION.cff
 CODE_OF_CONDUCT.md
 CONTRIBUTING.md
 LICENSE
 README.md
 TODO
 pyproject.toml
 pyrightconfig.json
@@ -74,32 +75,38 @@
 examples/istn/train.py
 examples/istn/models/__init__.py
 examples/istn/models/itn.py
 examples/istn/models/stn.py
 src/deepali/core/__init__.py
 src/deepali/core/_kornia.py
 src/deepali/core/affine.py
+src/deepali/core/argparse.py
 src/deepali/core/bspline.py
+src/deepali/core/collections.py
 src/deepali/core/config.py
 src/deepali/core/cube.py
 src/deepali/core/enum.py
+src/deepali/core/environ.py
 src/deepali/core/flow.py
 src/deepali/core/functional.py
 src/deepali/core/grid.py
 src/deepali/core/image.py
 src/deepali/core/itertools.py
 src/deepali/core/kernels.py
 src/deepali/core/linalg.py
+src/deepali/core/logging.py
 src/deepali/core/math.py
 src/deepali/core/nnutils.py
-src/deepali/core/path.py
+src/deepali/core/pathlib.py
 src/deepali/core/pointset.py
+src/deepali/core/psutil.py
 src/deepali/core/random.py
+src/deepali/core/tempfile.py
 src/deepali/core/tensor.py
-src/deepali/core/types.py
+src/deepali/core/typing.py
 src/deepali/data/__init__.py
 src/deepali/data/collate.py
 src/deepali/data/dataset.py
 src/deepali/data/flow.py
 src/deepali/data/image.py
 src/deepali/data/partition.py
 src/deepali/data/prepare.py
@@ -149,40 +156,40 @@
 src/deepali/spatial/generic.py
 src/deepali/spatial/image.py
 src/deepali/spatial/linear.py
 src/deepali/spatial/nonrigid.py
 src/deepali/spatial/parametric.py
 src/deepali/spatial/transformer.py
 src/deepali/utils/__init__.py
+src/deepali/utils/ipython.py
+src/deepali/utils/storage.py
 src/deepali/utils/tensorboard.py
 src/deepali/utils/aws/__init__.py
-src/deepali/utils/aws/resource.py
 src/deepali/utils/aws/s3/__init__.py
 src/deepali/utils/aws/s3/client.py
 src/deepali/utils/aws/s3/config.py
 src/deepali/utils/aws/s3/object.py
-src/deepali/utils/cli/__init__.py
-src/deepali/utils/cli/argparse.py
-src/deepali/utils/cli/environ.py
-src/deepali/utils/cli/logging.py
-src/deepali/utils/cli/warnings.py
 src/deepali/utils/ignite/__init__.py
 src/deepali/utils/ignite/handlers.py
 src/deepali/utils/ignite/output_transforms.py
 src/deepali/utils/ignite/score_functions.py
 src/deepali/utils/ignite/metrics/__init__.py
 src/deepali/utils/ignite/metrics/average_loss.py
 src/deepali/utils/ignite/metrics/binary_classification.py
 src/deepali/utils/ignite/metrics/multilabel_classification.py
-src/deepali/utils/sitk/__init__.py
-src/deepali/utils/sitk/grid.py
-src/deepali/utils/sitk/imageio.py
-src/deepali/utils/sitk/numpy.py
-src/deepali/utils/sitk/sample.py
-src/deepali/utils/sitk/torch.py
+src/deepali/utils/imageio/__init__.py
+src/deepali/utils/imageio/meta.py
+src/deepali/utils/imageio/nifti.py
+src/deepali/utils/imageio/sitk.py
+src/deepali/utils/simpleitk/__init__.py
+src/deepali/utils/simpleitk/grid.py
+src/deepali/utils/simpleitk/imageio.py
+src/deepali/utils/simpleitk/numpy.py
+src/deepali/utils/simpleitk/sample.py
+src/deepali/utils/simpleitk/torch.py
 src/deepali/utils/vtk/__init__.py
 src/deepali/utils/vtk/idlist.py
 src/deepali/utils/vtk/image.py
 src/deepali/utils/vtk/numpy.py
 src/deepali/utils/vtk/polydataio.py
 src/deepali/utils/vtk/simpleitk.py
 src/hf_deepali.egg-info/PKG-INFO
@@ -199,8 +206,9 @@
 tests/test_core_random.py
 tests/test_core_tensor_utils.py
 tests/test_data_flow.py
 tests/test_data_image.py
 tests/test_network_blocks.py
 tests/test_network_layers.py
 tests/test_network_resnet.py
-tests/test_network_unet.py
+tests/test_network_unet.py
+tests/test_utils_imageio_meta.py
```

### Comparing `hf-deepali-0.3.2/tests/_test_core_bspline.py` & `hf-deepali-0.4.0/tests/_test_core_bspline.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.2/tests/test_core_bspline.py` & `hf-deepali-0.4.0/tests/test_core_bspline.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.2/tests/test_core_cube.py` & `hf-deepali-0.4.0/tests/test_core_cube.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.2/tests/test_core_grid.py` & `hf-deepali-0.4.0/tests/test_core_grid.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import pytest
 
 import numpy as np
 import torch
 from torch import Tensor
 
-from deepali.core.grid import Grid
 from deepali.core import affine as A
+from deepali.core.grid import Grid
 
 
 @pytest.fixture
 def default_angle() -> Tensor:
     return torch.deg2rad(torch.tensor(33.0))
```

### Comparing `hf-deepali-0.3.2/tests/test_core_image_utils.py` & `hf-deepali-0.4.0/tests/test_core_image_utils.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 
 import pytest
 import torch
 from torch import Tensor
 
-from deepali.core import Grid
 from deepali.core import functional as U
+from deepali.core import Grid
 
 
 def test_fill_border():
     image = torch.zeros((2, 1, 7, 5), dtype=torch.float)
 
     result = U.fill_border(image, margin=1, value=1)
     assert isinstance(result, Tensor)
```

### Comparing `hf-deepali-0.3.2/tests/test_core_random.py` & `hf-deepali-0.4.0/tests/test_core_random.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.2/tests/test_core_tensor_utils.py` & `hf-deepali-0.4.0/tests/test_core_tensor_utils.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.2/tests/test_data_flow.py` & `hf-deepali-0.4.0/tests/test_data_flow.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.2/tests/test_data_image.py` & `hf-deepali-0.4.0/tests/test_data_image.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.2/tests/test_network_blocks.py` & `hf-deepali-0.4.0/tests/test_network_blocks.py`

 * *Files identical despite different names*

### Comparing `hf-deepali-0.3.2/tests/test_network_layers.py` & `hf-deepali-0.4.0/tests/test_network_layers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 r"""Test basic network layers."""
 
 import pytest
 
 import torch
 from torch import Tensor, nn
 
-from deepali.core.enum import PaddingMode
+from deepali.core import PaddingMode
 from deepali.networks.layers import Activation, activation
 from deepali.networks.layers import Conv2d, Conv3d, ConvLayer, convolution, conv_module
 from deepali.networks.layers import JoinLayer, join_func
 from deepali.networks.layers import LambdaLayer
 from deepali.networks.layers import NormLayer, normalization, norm_layer
```

### Comparing `hf-deepali-0.3.2/tests/test_network_unet.py` & `hf-deepali-0.4.0/tests/test_network_unet.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Tuple
 
 import pytest
 
 import torch
 from torch import Tensor
 
-from deepali.core.types import is_namedtuple
+from deepali.core.typing import is_namedtuple
 from deepali.networks.layers import convolution
 from deepali.networks.unet import UNet, UNetConfig, last_num_channels
 
 
 @pytest.fixture(scope="function")
 def input_tensor(request) -> Tensor:
     if request.param == 2:
```

