# Comparing `tmp/hist-2.6.3.tar.gz` & `tmp/hist-2.7.0.tar.gz`

## Comparing `hist-2.6.3.tar` & `hist-2.7.0.tar`

### file list

```diff
@@ -1,134 +1,146 @@
--rw-r--r--   0        0        0     3319 2020-02-02 00:00:00.000000 hist-2.6.3/.all-contributorsrc
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 hist-2.6.3/.flake8
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 hist-2.6.3/.git_archival.txt
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 hist-2.6.3/.gitattributes
--rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 hist-2.6.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 hist-2.6.3/.readthedocs.yml
--rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 hist-2.6.3/CITATION.cff
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 hist-2.6.3/dev-environment.yml
--rw-r--r--   0        0        0     2057 2020-02-02 00:00:00.000000 hist-2.6.3/noxfile.py
--rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 hist-2.6.3/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 hist-2.6.3/.github/dependabot.yml
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 hist-2.6.3/.github/labeler.yml
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 hist-2.6.3/.github/ISSUE_TEMPLATE/bug-report.md
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 hist-2.6.3/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 hist-2.6.3/.github/ISSUE_TEMPLATE/docs-improvements.md
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 hist-2.6.3/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 hist-2.6.3/.github/ISSUE_TEMPLATE/support.md
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 hist-2.6.3/.github/matchers/pylint.json
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 hist-2.6.3/.github/workflows/cd.yml
--rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 hist-2.6.3/.github/workflows/ci.yml
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 hist-2.6.3/.github/workflows/pr.yml
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 hist-2.6.3/binder/postBuild
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 hist-2.6.3/docs/Makefile
--rw-r--r--   0        0        0     2781 2020-02-02 00:00:00.000000 hist-2.6.3/docs/banner_slides.md
--rw-r--r--   0        0        0     7953 2020-02-02 00:00:00.000000 hist-2.6.3/docs/changelog.md
--rw-r--r--   0        0        0     3158 2020-02-02 00:00:00.000000 hist-2.6.3/docs/conf.py
--rw-r--r--   0        0        0     4187 2020-02-02 00:00:00.000000 hist-2.6.3/docs/index.rst
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 hist-2.6.3/docs/make.bat
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 hist-2.6.3/docs/support.rst
--rw-r--r--   0        0        0     3093 2020-02-02 00:00:00.000000 hist-2.6.3/docs/_images/axis_category.png
--rw-r--r--   0        0        0     5696 2020-02-02 00:00:00.000000 hist-2.6.3/docs/_images/axis_circular.png
--rw-r--r--   0        0        0     2349 2020-02-02 00:00:00.000000 hist-2.6.3/docs/_images/axis_integer.png
--rw-r--r--   0        0        0     2352 2020-02-02 00:00:00.000000 hist-2.6.3/docs/_images/axis_regular.png
--rw-r--r--   0        0        0     2599 2020-02-02 00:00:00.000000 hist-2.6.3/docs/_images/axis_variable.png
--rw-r--r--   0        0        0   278047 2020-02-02 00:00:00.000000 hist-2.6.3/docs/_images/banner.gif
--rw-r--r--   0        0        0    21774 2020-02-02 00:00:00.000000 hist-2.6.3/docs/_images/ex_hist_density.png
--rw-r--r--   0        0        0    62092 2020-02-02 00:00:00.000000 hist-2.6.3/docs/_images/fullplot_example.png
--rw-r--r--   0        0        0    18389 2020-02-02 00:00:00.000000 hist-2.6.3/docs/_images/histlogo.png
--rw-r--r--   0        0        0    94683 2020-02-02 00:00:00.000000 hist-2.6.3/docs/_images/histlogo.svg
--rw-r--r--   0        0        0    17543 2020-02-02 00:00:00.000000 hist-2.6.3/docs/_images/histogram_design.png
--rw-r--r--   0        0        0   301669 2020-02-02 00:00:00.000000 hist-2.6.3/docs/_images/pieplot_example.png
--rw-r--r--   0        0        0   114661 2020-02-02 00:00:00.000000 hist-2.6.3/docs/_images/ratioplot_example.png
--rw-r--r--   0        0        0    14396 2020-02-02 00:00:00.000000 hist-2.6.3/docs/_images/stackplot_example.png
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 hist-2.6.3/docs/_src/images/.gitignore
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 hist-2.6.3/docs/_src/images/Makefile
--rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 hist-2.6.3/docs/_src/images/axis_category.tex
--rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 hist-2.6.3/docs/_src/images/axis_circular.tex
--rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 hist-2.6.3/docs/_src/images/axis_integer.tex
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 hist-2.6.3/docs/_src/images/axis_regular.tex
--rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 hist-2.6.3/docs/_src/images/axis_variable.tex
--rw-r--r--   0        0        0     5903 2020-02-02 00:00:00.000000 hist-2.6.3/docs/examples/HistDemo.ipynb
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 hist-2.6.3/docs/reference/hist.accumulators.rst
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 hist-2.6.3/docs/reference/hist.axestuple.rst
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 hist-2.6.3/docs/reference/hist.axis.rst
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 hist-2.6.3/docs/reference/hist.basehist.rst
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 hist-2.6.3/docs/reference/hist.classichist.rst
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 hist-2.6.3/docs/reference/hist.dask.rst
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 hist-2.6.3/docs/reference/hist.hist.rst
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 hist-2.6.3/docs/reference/hist.intervals.rst
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 hist-2.6.3/docs/reference/hist.namedhist.rst
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 hist-2.6.3/docs/reference/hist.numpy.rst
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 hist-2.6.3/docs/reference/hist.rst
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 hist-2.6.3/docs/reference/hist.stack.rst
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 hist-2.6.3/docs/reference/hist.storage.rst
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 hist-2.6.3/docs/reference/hist.tag.rst
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 hist-2.6.3/docs/reference/hist.version.rst
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 hist-2.6.3/docs/reference/modules.rst
--rw-r--r--   0        0        0     5217 2020-02-02 00:00:00.000000 hist-2.6.3/docs/user-guide/accumulators.rst
--rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 hist-2.6.3/docs/user-guide/analyses.rst
--rw-r--r--   0        0        0     7468 2020-02-02 00:00:00.000000 hist-2.6.3/docs/user-guide/axes.rst
--rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 hist-2.6.3/docs/user-guide/indexing.rst
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 hist-2.6.3/docs/user-guide/installation.rst
--rw-r--r--   0        0        0     3906 2020-02-02 00:00:00.000000 hist-2.6.3/docs/user-guide/numpy.rst
--rw-r--r--   0        0        0     5669 2020-02-02 00:00:00.000000 hist-2.6.3/docs/user-guide/quickstart.rst
--rw-r--r--   0        0        0     3620 2020-02-02 00:00:00.000000 hist-2.6.3/docs/user-guide/storages.rst
--rw-r--r--   0        0        0     2782 2020-02-02 00:00:00.000000 hist-2.6.3/docs/user-guide/subclassing.rst
--rw-r--r--   0        0        0    17488 2020-02-02 00:00:00.000000 hist-2.6.3/docs/user-guide/notebooks/Histogram.ipynb
--rw-r--r--   0        0        0     3904 2020-02-02 00:00:00.000000 hist-2.6.3/docs/user-guide/notebooks/Interpolation.ipynb
--rw-r--r--   0        0        0     8905 2020-02-02 00:00:00.000000 hist-2.6.3/docs/user-guide/notebooks/Plots.ipynb
--rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 hist-2.6.3/docs/user-guide/notebooks/Reprs.ipynb
--rw-r--r--   0        0        0    19154 2020-02-02 00:00:00.000000 hist-2.6.3/docs/user-guide/notebooks/SVGHistogram.ipynb
--rw-r--r--   0        0        0     5872 2020-02-02 00:00:00.000000 hist-2.6.3/docs/user-guide/notebooks/Stack.ipynb
--rw-r--r--   0        0        0     3929 2020-02-02 00:00:00.000000 hist-2.6.3/docs/user-guide/notebooks/Transform.ipynb
--rw-r--r--   0        0        0    50193 2020-02-02 00:00:00.000000 hist-2.6.3/notebooks/HistLogo.ipynb
--rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 hist-2.6.3/notebooks/axestuple-setattr.ipynb
--rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 hist-2.6.3/src/hist/__init__.py
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 hist-2.6.3/src/hist/accumulators.py
--rw-r--r--   0        0        0     2834 2020-02-02 00:00:00.000000 hist-2.6.3/src/hist/axestuple.py
--rw-r--r--   0        0        0    18693 2020-02-02 00:00:00.000000 hist-2.6.3/src/hist/basehist.py
--rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 hist-2.6.3/src/hist/classichist.py
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 hist-2.6.3/src/hist/hist.py
--rw-r--r--   0        0        0     6926 2020-02-02 00:00:00.000000 hist-2.6.3/src/hist/intervals.py
--rw-r--r--   0        0        0     2708 2020-02-02 00:00:00.000000 hist-2.6.3/src/hist/namedhist.py
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 hist-2.6.3/src/hist/numpy.py
--rw-r--r--   0        0        0    22956 2020-02-02 00:00:00.000000 hist-2.6.3/src/hist/plot.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hist-2.6.3/src/hist/py.typed
--rw-r--r--   0        0        0    11131 2020-02-02 00:00:00.000000 hist-2.6.3/src/hist/quick_construct.py
--rw-r--r--   0        0        0     5888 2020-02-02 00:00:00.000000 hist-2.6.3/src/hist/stack.py
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 hist-2.6.3/src/hist/storage.py
--rw-r--r--   0        0        0     5426 2020-02-02 00:00:00.000000 hist-2.6.3/src/hist/svgplots.py
--rw-r--r--   0        0        0     2335 2020-02-02 00:00:00.000000 hist-2.6.3/src/hist/svgutils.py
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 hist-2.6.3/src/hist/tag.py
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 hist-2.6.3/src/hist/typing.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 hist-2.6.3/src/hist/version.py
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 hist-2.6.3/src/hist/version.pyi
--rw-r--r--   0        0        0     6107 2020-02-02 00:00:00.000000 hist-2.6.3/src/hist/axis/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hist-2.6.3/src/hist/axis/py.typed
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 hist-2.6.3/src/hist/axis/transform.py
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 hist-2.6.3/src/hist/dask/__init__.py
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 hist-2.6.3/src/hist/dask/hist.py
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 hist-2.6.3/src/hist/dask/namedhist.py
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 hist-2.6.3/tests/conftest.py
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 hist-2.6.3/tests/test_axestuple.py
--rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 hist-2.6.3/tests/test_axis.py
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 hist-2.6.3/tests/test_bh.py
--rw-r--r--   0        0        0     4189 2020-02-02 00:00:00.000000 hist-2.6.3/tests/test_dask.py
--rw-r--r--   0        0        0    27523 2020-02-02 00:00:00.000000 hist-2.6.3/tests/test_general.py
--rw-r--r--   0        0        0     6204 2020-02-02 00:00:00.000000 hist-2.6.3/tests/test_intervals.py
--rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 hist-2.6.3/tests/test_mock_plot.py
--rw-r--r--   0        0        0    25285 2020-02-02 00:00:00.000000 hist-2.6.3/tests/test_named.py
--rw-r--r--   0        0        0    19787 2020-02-02 00:00:00.000000 hist-2.6.3/tests/test_plot.py
--rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 hist-2.6.3/tests/test_profile.py
--rw-r--r--   0        0        0     2706 2020-02-02 00:00:00.000000 hist-2.6.3/tests/test_reprs.py
--rw-r--r--   0        0        0    12142 2020-02-02 00:00:00.000000 hist-2.6.3/tests/test_stacks.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 hist-2.6.3/tests/test_version.py
--rw-r--r--   0        0        0    20789 2020-02-02 00:00:00.000000 hist-2.6.3/tests/baseline/test_image_plot_pull.png
--rw-r--r--   0        0        0    19242 2020-02-02 00:00:00.000000 hist-2.6.3/tests/baseline/test_image_plot_ratio_callable.png
--rw-r--r--   0        0        0    13830 2020-02-02 00:00:00.000000 hist-2.6.3/tests/baseline/test_image_plot_ratio_hist.png
--rw-r--r--   0        0        0    18456 2020-02-02 00:00:00.000000 hist-2.6.3/tests/baseline/test_plot1d_auto_handling.png
--rw-r--r--   0        0        0     2148 2020-02-02 00:00:00.000000 hist-2.6.3/.gitignore
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 hist-2.6.3/LICENSE
--rw-r--r--   0        0        0    12721 2020-02-02 00:00:00.000000 hist-2.6.3/README.md
--rw-r--r--   0        0        0     4829 2020-02-02 00:00:00.000000 hist-2.6.3/pyproject.toml
--rw-r--r--   0        0        0    16926 2020-02-02 00:00:00.000000 hist-2.6.3/PKG-INFO
+-rw-r--r--   0        0        0     3319 2020-02-02 00:00:00.000000 hist-2.7.0/.all-contributorsrc
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 hist-2.7.0/.git_archival.txt
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 hist-2.7.0/.gitattributes
+-rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 hist-2.7.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 hist-2.7.0/.readthedocs.yml
+-rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 hist-2.7.0/CITATION.cff
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 hist-2.7.0/dev-environment.yml
+-rw-r--r--   0        0        0     2530 2020-02-02 00:00:00.000000 hist-2.7.0/noxfile.py
+-rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 hist-2.7.0/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 hist-2.7.0/.github/dependabot.yml
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 hist-2.7.0/.github/labeler.yml
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 hist-2.7.0/.github/ISSUE_TEMPLATE/bug-report.md
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 hist-2.7.0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 hist-2.7.0/.github/ISSUE_TEMPLATE/docs-improvements.md
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 hist-2.7.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 hist-2.7.0/.github/ISSUE_TEMPLATE/support.md
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 hist-2.7.0/.github/matchers/pylint.json
+-rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 hist-2.7.0/.github/workflows/cd.yml
+-rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 hist-2.7.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 hist-2.7.0/.github/workflows/pr.yml
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 hist-2.7.0/binder/postBuild
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 hist-2.7.0/docs/Makefile
+-rw-r--r--   0        0        0     2785 2020-02-02 00:00:00.000000 hist-2.7.0/docs/banner_slides.md
+-rw-r--r--   0        0        0     8422 2020-02-02 00:00:00.000000 hist-2.7.0/docs/changelog.md
+-rw-r--r--   0        0        0     2707 2020-02-02 00:00:00.000000 hist-2.7.0/docs/conf.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 hist-2.7.0/docs/contributing.md
+-rw-r--r--   0        0        0     4205 2020-02-02 00:00:00.000000 hist-2.7.0/docs/index.rst
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 hist-2.7.0/docs/make.bat
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 hist-2.7.0/docs/support.rst
+-rw-r--r--   0        0        0     3093 2020-02-02 00:00:00.000000 hist-2.7.0/docs/_images/axis_category.png
+-rw-r--r--   0        0        0     5696 2020-02-02 00:00:00.000000 hist-2.7.0/docs/_images/axis_circular.png
+-rw-r--r--   0        0        0     2349 2020-02-02 00:00:00.000000 hist-2.7.0/docs/_images/axis_integer.png
+-rw-r--r--   0        0        0     2352 2020-02-02 00:00:00.000000 hist-2.7.0/docs/_images/axis_regular.png
+-rw-r--r--   0        0        0     2599 2020-02-02 00:00:00.000000 hist-2.7.0/docs/_images/axis_variable.png
+-rw-r--r--   0        0        0   278047 2020-02-02 00:00:00.000000 hist-2.7.0/docs/_images/banner.gif
+-rw-r--r--   0        0        0    21774 2020-02-02 00:00:00.000000 hist-2.7.0/docs/_images/ex_hist_density.png
+-rw-r--r--   0        0        0    62092 2020-02-02 00:00:00.000000 hist-2.7.0/docs/_images/fullplot_example.png
+-rw-r--r--   0        0        0    18389 2020-02-02 00:00:00.000000 hist-2.7.0/docs/_images/histlogo.png
+-rw-r--r--   0        0        0    94683 2020-02-02 00:00:00.000000 hist-2.7.0/docs/_images/histlogo.svg
+-rw-r--r--   0        0        0    17543 2020-02-02 00:00:00.000000 hist-2.7.0/docs/_images/histogram_design.png
+-rw-r--r--   0        0        0   301669 2020-02-02 00:00:00.000000 hist-2.7.0/docs/_images/pieplot_example.png
+-rw-r--r--   0        0        0   114661 2020-02-02 00:00:00.000000 hist-2.7.0/docs/_images/ratioplot_example.png
+-rw-r--r--   0        0        0    14396 2020-02-02 00:00:00.000000 hist-2.7.0/docs/_images/stackplot_example.png
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 hist-2.7.0/docs/_src/images/.gitignore
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 hist-2.7.0/docs/_src/images/Makefile
+-rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 hist-2.7.0/docs/_src/images/axis_category.tex
+-rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 hist-2.7.0/docs/_src/images/axis_circular.tex
+-rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 hist-2.7.0/docs/_src/images/axis_integer.tex
+-rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 hist-2.7.0/docs/_src/images/axis_regular.tex
+-rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 hist-2.7.0/docs/_src/images/axis_variable.tex
+-rw-r--r--   0        0        0     5913 2020-02-02 00:00:00.000000 hist-2.7.0/docs/examples/HistDemo.ipynb
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 hist-2.7.0/docs/reference/hist.accumulators.rst
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 hist-2.7.0/docs/reference/hist.axestuple.rst
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 hist-2.7.0/docs/reference/hist.axis.rst
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 hist-2.7.0/docs/reference/hist.axis.transform.rst
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 hist-2.7.0/docs/reference/hist.basehist.rst
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 hist-2.7.0/docs/reference/hist.classichist.rst
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 hist-2.7.0/docs/reference/hist.dask.hist.rst
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 hist-2.7.0/docs/reference/hist.dask.namedhist.rst
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 hist-2.7.0/docs/reference/hist.dask.rst
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 hist-2.7.0/docs/reference/hist.hist.rst
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 hist-2.7.0/docs/reference/hist.intervals.rst
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 hist-2.7.0/docs/reference/hist.namedhist.rst
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 hist-2.7.0/docs/reference/hist.numpy.rst
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 hist-2.7.0/docs/reference/hist.plot.rst
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 hist-2.7.0/docs/reference/hist.quick_construct.rst
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 hist-2.7.0/docs/reference/hist.rst
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 hist-2.7.0/docs/reference/hist.stack.rst
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 hist-2.7.0/docs/reference/hist.storage.rst
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 hist-2.7.0/docs/reference/hist.svgplots.rst
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 hist-2.7.0/docs/reference/hist.svgutils.rst
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 hist-2.7.0/docs/reference/hist.tag.rst
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 hist-2.7.0/docs/reference/hist.version.rst
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 hist-2.7.0/docs/reference/modules.rst
+-rw-r--r--   0        0        0     5217 2020-02-02 00:00:00.000000 hist-2.7.0/docs/user-guide/accumulators.rst
+-rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 hist-2.7.0/docs/user-guide/analyses.rst
+-rw-r--r--   0        0        0     7451 2020-02-02 00:00:00.000000 hist-2.7.0/docs/user-guide/axes.rst
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 hist-2.7.0/docs/user-guide/cli.rst
+-rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 hist-2.7.0/docs/user-guide/indexing.rst
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 hist-2.7.0/docs/user-guide/installation.rst
+-rw-r--r--   0        0        0     3915 2020-02-02 00:00:00.000000 hist-2.7.0/docs/user-guide/numpy.rst
+-rw-r--r--   0        0        0     5662 2020-02-02 00:00:00.000000 hist-2.7.0/docs/user-guide/quickstart.rst
+-rw-r--r--   0        0        0     3586 2020-02-02 00:00:00.000000 hist-2.7.0/docs/user-guide/storages.rst
+-rw-r--r--   0        0        0     2784 2020-02-02 00:00:00.000000 hist-2.7.0/docs/user-guide/subclassing.rst
+-rw-r--r--   0        0        0    17498 2020-02-02 00:00:00.000000 hist-2.7.0/docs/user-guide/notebooks/Histogram.ipynb
+-rw-r--r--   0        0        0     3908 2020-02-02 00:00:00.000000 hist-2.7.0/docs/user-guide/notebooks/Interpolation.ipynb
+-rw-r--r--   0        0        0     8945 2020-02-02 00:00:00.000000 hist-2.7.0/docs/user-guide/notebooks/Plots.ipynb
+-rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 hist-2.7.0/docs/user-guide/notebooks/Reprs.ipynb
+-rw-r--r--   0        0        0    18737 2020-02-02 00:00:00.000000 hist-2.7.0/docs/user-guide/notebooks/SVGHistogram.ipynb
+-rw-r--r--   0        0        0     5882 2020-02-02 00:00:00.000000 hist-2.7.0/docs/user-guide/notebooks/Stack.ipynb
+-rw-r--r--   0        0        0     3853 2020-02-02 00:00:00.000000 hist-2.7.0/docs/user-guide/notebooks/Transform.ipynb
+-rw-r--r--   0        0        0    50203 2020-02-02 00:00:00.000000 hist-2.7.0/notebooks/HistLogo.ipynb
+-rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 hist-2.7.0/notebooks/axestuple-setattr.ipynb
+-rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 hist-2.7.0/src/hist/__init__.py
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 hist-2.7.0/src/hist/accumulators.py
+-rw-r--r--   0        0        0     2291 2020-02-02 00:00:00.000000 hist-2.7.0/src/hist/axestuple.py
+-rw-r--r--   0        0        0    22056 2020-02-02 00:00:00.000000 hist-2.7.0/src/hist/basehist.py
+-rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 hist-2.7.0/src/hist/classichist.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 hist-2.7.0/src/hist/hist.py
+-rw-r--r--   0        0        0     4130 2020-02-02 00:00:00.000000 hist-2.7.0/src/hist/interop.py
+-rw-r--r--   0        0        0     6893 2020-02-02 00:00:00.000000 hist-2.7.0/src/hist/intervals.py
+-rw-r--r--   0        0        0     5187 2020-02-02 00:00:00.000000 hist-2.7.0/src/hist/namedhist.py
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 hist-2.7.0/src/hist/numpy.py
+-rw-r--r--   0        0        0    23008 2020-02-02 00:00:00.000000 hist-2.7.0/src/hist/plot.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hist-2.7.0/src/hist/py.typed
+-rw-r--r--   0        0        0    11131 2020-02-02 00:00:00.000000 hist-2.7.0/src/hist/quick_construct.py
+-rw-r--r--   0        0        0     5902 2020-02-02 00:00:00.000000 hist-2.7.0/src/hist/stack.py
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 hist-2.7.0/src/hist/storage.py
+-rw-r--r--   0        0        0     5426 2020-02-02 00:00:00.000000 hist-2.7.0/src/hist/svgplots.py
+-rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 hist-2.7.0/src/hist/svgutils.py
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 hist-2.7.0/src/hist/tag.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 hist-2.7.0/src/hist/version.py
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 hist-2.7.0/src/hist/version.pyi
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hist-2.7.0/src/hist/_compat/__init__.py
+-rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 hist-2.7.0/src/hist/_compat/builtins.py
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 hist-2.7.0/src/hist/_compat/typing.py
+-rw-r--r--   0        0        0     6018 2020-02-02 00:00:00.000000 hist-2.7.0/src/hist/axis/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hist-2.7.0/src/hist/axis/py.typed
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 hist-2.7.0/src/hist/axis/transform.py
+-rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 hist-2.7.0/src/hist/dask/__init__.py
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 hist-2.7.0/src/hist/dask/hist.py
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 hist-2.7.0/src/hist/dask/namedhist.py
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 hist-2.7.0/tests/conftest.py
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 hist-2.7.0/tests/test_axestuple.py
+-rw-r--r--   0        0        0     2078 2020-02-02 00:00:00.000000 hist-2.7.0/tests/test_axis.py
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 hist-2.7.0/tests/test_bh.py
+-rw-r--r--   0        0        0     4217 2020-02-02 00:00:00.000000 hist-2.7.0/tests/test_dask.py
+-rw-r--r--   0        0        0    28170 2020-02-02 00:00:00.000000 hist-2.7.0/tests/test_general.py
+-rw-r--r--   0        0        0    11430 2020-02-02 00:00:00.000000 hist-2.7.0/tests/test_interop.py
+-rw-r--r--   0        0        0     6204 2020-02-02 00:00:00.000000 hist-2.7.0/tests/test_intervals.py
+-rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 hist-2.7.0/tests/test_mock_plot.py
+-rw-r--r--   0        0        0    25239 2020-02-02 00:00:00.000000 hist-2.7.0/tests/test_named.py
+-rw-r--r--   0        0        0    19787 2020-02-02 00:00:00.000000 hist-2.7.0/tests/test_plot.py
+-rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 hist-2.7.0/tests/test_profile.py
+-rw-r--r--   0        0        0     2714 2020-02-02 00:00:00.000000 hist-2.7.0/tests/test_reprs.py
+-rw-r--r--   0        0        0    12162 2020-02-02 00:00:00.000000 hist-2.7.0/tests/test_stacks.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 hist-2.7.0/tests/test_version.py
+-rw-r--r--   0        0        0    20789 2020-02-02 00:00:00.000000 hist-2.7.0/tests/baseline/test_image_plot_pull.png
+-rw-r--r--   0        0        0    19242 2020-02-02 00:00:00.000000 hist-2.7.0/tests/baseline/test_image_plot_ratio_callable.png
+-rw-r--r--   0        0        0    13830 2020-02-02 00:00:00.000000 hist-2.7.0/tests/baseline/test_image_plot_ratio_hist.png
+-rw-r--r--   0        0        0    19403 2020-02-02 00:00:00.000000 hist-2.7.0/tests/baseline/test_plot1d_auto_handling.png
+-rw-r--r--   0        0        0     2148 2020-02-02 00:00:00.000000 hist-2.7.0/.gitignore
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 hist-2.7.0/LICENSE
+-rw-r--r--   0        0        0    12885 2020-02-02 00:00:00.000000 hist-2.7.0/README.md
+-rw-r--r--   0        0        0     5725 2020-02-02 00:00:00.000000 hist-2.7.0/pyproject.toml
+-rw-r--r--   0        0        0    16961 2020-02-02 00:00:00.000000 hist-2.7.0/PKG-INFO
```

### Comparing `hist-2.6.3/.all-contributorsrc` & `hist-2.7.0/.all-contributorsrc`

 * *Files identical despite different names*

### Comparing `hist-2.6.3/.pre-commit-config.yaml` & `hist-2.7.0/.pre-commit-config.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -1,99 +1,71 @@
 ci:
   autoupdate_commit_msg: "chore: update pre-commit hooks"
   autofix_commit_msg: "style: pre-commit fixes"
 
 repos:
 - repo: https://github.com/psf/black
-  rev: 22.12.0
+  rev: 23.7.0
   hooks:
   - id: black-jupyter
 
+- repo: https://github.com/asottile/blacken-docs
+  rev: "1.15.0"
+  hooks:
+  - id: blacken-docs
+    additional_dependencies: [black==23.7.0]
+
 - repo: https://github.com/pre-commit/pre-commit-hooks
   rev: v4.4.0
   hooks:
   - id: check-added-large-files
   - id: check-case-conflict
   - id: check-merge-conflict
   - id: check-symlinks
   - id: check-yaml
   - id: debug-statements
   - id: end-of-file-fixer
   - id: mixed-line-ending
   - id: requirements-txt-fixer
   - id: trailing-whitespace
 
-- repo: https://github.com/PyCQA/isort
-  rev: 5.11.4
-  hooks:
-  - id: isort
-    args: ["-a", "from __future__ import annotations"]
-
-- repo: https://github.com/asottile/pyupgrade
-  rev: v3.3.1
-  hooks:
-  - id: pyupgrade
-    args: [--py37-plus]
-
-- repo: https://github.com/asottile/setup-cfg-fmt
-  rev: v2.2.0
+- repo: https://github.com/astral-sh/ruff-pre-commit
+  rev: v0.0.278
   hooks:
-  - id: setup-cfg-fmt
+  - id: ruff
+    args: ["--fix", "--show-fixes"]
 
 # Notebook formatting
 - repo: https://github.com/nbQA-dev/nbQA
-  rev: 1.6.1
+  rev: 1.7.0
   hooks:
-  - id: nbqa-pyupgrade
-    additional_dependencies: [pyupgrade==2.31.1]
-    args: ["--py37-plus"]
-
-- repo: https://github.com/asottile/yesqa
-  rev: v1.4.0
-  hooks:
-  - id: yesqa
-    additional_dependencies: &flake8-dependencies
-    - flake8-bugbear
-
-- repo: https://github.com/pycqa/flake8
-  rev: 6.0.0
-  hooks:
-  - id: flake8
-    exclude: docs/conf.py
-    additional_dependencies: *flake8-dependencies
+  - id: nbqa-ruff
+    additional_dependencies: [ruff==0.0.255]
+    args: ["--extend-ignore=B008,T20,I002,E402", "--fix", "--show-fixes"]
 
 - repo: https://github.com/pre-commit/mirrors-mypy
-  rev: v0.991
+  rev: v1.4.1
   hooks:
   - id: mypy
     files: ^src
     args: []
-    additional_dependencies: ["numpy~=1.23.0", "matplotlib>=3.4", "boost-histogram~=1.3.1", "uhi~=0.3.1"]
-
-- repo: https://github.com/mgedmin/check-manifest
-  rev: "0.49"
-  hooks:
-  - id: check-manifest
-    stages: [manual]
+    additional_dependencies: ["numpy~=1.24.0", "matplotlib>=3.4", "boost-histogram~=1.3.1", "uhi~=0.3.1", "pandas-stubs>=2.0.1.230501"]
 
 - repo: https://github.com/codespell-project/codespell
-  rev: v2.2.2
+  rev: v2.2.5
   hooks:
   - id: codespell
     args: ["-Lhist,gaus,nd"]
     exclude: ^notebooks/HistLogo.ipynb$
 
 - repo: https://github.com/pre-commit/pygrep-hooks
-  rev: v1.9.0
+  rev: v1.10.0
   hooks:
-  - id: python-check-blanket-noqa
-  - id: python-check-blanket-type-ignore
-  - id: python-no-log-warn
   - id: python-use-type-annotations
   - id: rst-backticks
   - id: rst-directive-colons
   - id: rst-inline-touching-normal
 
 - repo: https://github.com/shellcheck-py/shellcheck-py
-  rev: v0.9.0.2
+  rev: v0.9.0.5
   hooks:
   - id: shellcheck
```

### Comparing `hist-2.6.3/CITATION.cff` & `hist-2.7.0/CITATION.cff`

 * *Files identical despite different names*

### Comparing `hist-2.6.3/noxfile.py` & `hist-2.7.0/noxfile.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+import argparse
 import shutil
 import sys
 from pathlib import Path
 
 import nox
 
 ALL_PYTHONS = ["3.7", "3.8", "3.9", "3.10", "3.11"]
@@ -25,15 +26,15 @@
 
 @nox.session
 def pylint(session: nox.Session) -> None:
     """
     Run pylint.
     """
 
-    session.install("pylint~=2.15.0")
+    session.install("pylint~=2.16.0")
     session.install("-e", ".")
     session.run("pylint", "src", *session.posargs)
 
 
 @nox.session(python=ALL_PYTHONS, reuse_venv=True)
 def tests(session):
     """
@@ -54,32 +55,52 @@
         session.error(
             "Must be run from Linux, images will be slightly different on macOS"
         )
     session.run("pytest", "--mpl-generate-path=tests/baseline", *session.posargs)
 
 
 @nox.session(reuse_venv=True)
-def docs(session):
+def docs(session: nox.Session) -> None:
     """
-    Build the docs. Pass "serve" to serve.
+    Build the docs. Pass "--serve" to serve.
     """
 
+    parser = argparse.ArgumentParser()
+    parser.add_argument("--serve", action="store_true", help="Serve after building")
+    args = parser.parse_args(session.posargs)
+
     session.install("-e", ".[docs]")
     session.chdir("docs")
     session.run("sphinx-build", "-M", "html", ".", "_build")
 
-    if session.posargs:
-        if "serve" in session.posargs:
-            print("Launching docs at http://localhost:8001/ - use Ctrl-C to quit")
-            session.run("python", "-m", "http.server", "8001", "-d", "_build/html")
-        else:
-            print("Unsupported argument to docs")
+    if args.serve:
+        print("Launching docs at http://localhost:8000/ - use Ctrl-C to quit")
+        session.run("python", "-m", "http.server", "8000", "-d", "_build/html")
 
 
-@nox.session
+@nox.session(reuse_venv=True)
+def build_api_docs(session: nox.Session) -> None:
+    """
+    Build (regenerate) API docs.
+    """
+
+    session.install("sphinx")
+    session.chdir("docs")
+    session.run(
+        "sphinx-apidoc",
+        "-o",
+        "reference/",
+        "--separate",
+        "--force",
+        "--module-first",
+        "../src/hist",
+    )
+
+
+@nox.session(reuse_venv=True)
 def build(session):
     """
     Build an SDist and wheel.
     """
 
     build_p = DIR.joinpath("build")
     if build_p.exists():
```

### Comparing `hist-2.6.3/.github/CONTRIBUTING.md` & `hist-2.7.0/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `hist-2.6.3/.github/ISSUE_TEMPLATE/feature_request.md` & `hist-2.7.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `hist-2.6.3/.github/matchers/pylint.json` & `hist-2.7.0/.github/matchers/pylint.json`

 * *Files identical despite different names*

### Comparing `hist-2.6.3/.github/workflows/cd.yml` & `hist-2.7.0/.github/workflows/cd.yml`

 * *Files 12% similar despite different names*

```diff
@@ -7,15 +7,15 @@
       - main
   release:
     types:
     - published
 
 jobs:
   dist:
-    runs-on: ubuntu-20.04
+    runs-on: ubuntu-22.04
     steps:
     - uses: actions/checkout@v3
       with:
         fetch-depth: 0
 
     - name: Build SDist & wheel
       run: pipx run --spec build pyproject-build
@@ -35,11 +35,11 @@
 
     steps:
     - uses: actions/download-artifact@v3
       with:
         name: artifact
         path: dist
 
-    - uses: pypa/gh-action-pypi-publish@v1.6.4
+    - uses: pypa/gh-action-pypi-publish@release/v1
       with:
         user: __token__
         password: ${{ secrets.pypi_password }}
```

### Comparing `hist-2.6.3/.github/workflows/ci.yml` & `hist-2.7.0/.github/workflows/ci.yml`

 * *Files 12% similar despite different names*

```diff
@@ -5,14 +5,18 @@
   push:
     branches:
       - main
 
 env:
   FORCE_COLOR: 3
 
+concurrency:
+  group: ${ github.workflow }-${ github.ref }
+  cancel-in-progress: true
+
 jobs:
   pre-commit:
     runs-on: ubuntu-latest
     steps:
     - uses: actions/checkout@v3
     - uses: actions/setup-python@v4
       with:
```

### Comparing `hist-2.6.3/docs/Makefile` & `hist-2.7.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `hist-2.6.3/docs/banner_slides.md` & `hist-2.7.0/docs/banner_slides.md`

 * *Files 2% similar despite different names*

```diff
@@ -12,35 +12,33 @@
 Converted to GIF with ezgif.com, 300 ms delay time.
 -->
 
 ```python
 import hist
 
 # Make a histogram
-h = hist.Hist(
-    hist.axes.Regular(10, 0, 1, name="x")
-)
+h = hist.Hist(hist.axes.Regular(10, 0, 1, name="x"))
 
 # Fill it with events
-h.fill(x=[.2, .3, .6, .9])
+h.fill(x=[0.2, 0.3, 0.6, 0.9])
 
 # Compute the sum
 total = h.sum()
 ```
 
 # QuickConstruct
 
 ```python
 from hist import Hist
 
 # Make a histogram
 h = Hist.new.Reg(10, 0, 1, name="x").Double()
 
 # Fill it with events
-h.fill(x=[.2, .3, .6, .9])
+h.fill(x=[0.2, 0.3, 0.6, 0.9])
 
 # Compute the sum
 total = h.sum()
 ```
 
 # Plotting: plot_full
 
@@ -62,15 +60,15 @@
 \end{center}
 
 
 # Advanced Indexing
 
 ```python
 # Slice in data coordinates
-sliced_h = h[.5j:1.5j]
+sliced_h = h[0.5j:1.5j]
 
 # Sum over and rebin easily
 smaller_1d = h_2d[sum, 2j]
 
 # Set and access easily
 h[...] = np.asarray(prebinned)
 
@@ -133,14 +131,15 @@
 * Means
 * Weighted Means
 
 Supports the UHI `PlottableHistogram` protocol!
 
 ```python
 import mplhep
+
 mplhep.histplot(h)
 ```
 
 
 
 # NumPy compatibility
```

### Comparing `hist-2.6.3/docs/changelog.md` & `hist-2.7.0/docs/changelog.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,29 @@
 # Changelog
 
+
+## Version 2.7.0
+
+Features:
+
+* Add a function to integrate axes
+  [#505](https://github.com/scikit-hep/hist/pull/505)
+* Add `fill_flattened` support
+  [#474](https://github.com/scikit-hep/hist/pull/474)
+
+Various other items:
+
+* Move linting to using Ruff
+  [#475](https://github.com/scikit-hep/hist/pull/475)
+* `Self` & `_compat`
+  [#479](https://github.com/scikit-hep/hist/pull/479)
+* Rework and rerun docs API
+  [#481](https://github.com/scikit-hep/hist/pull/481)
+
+
 ## Version 2.6.3
 
 * Experimental dask support
   [#471](https://github.com/scikit-hep/hist/pull/471)
 * Some minor cleanups from refurb
   [#453](https://github.com/scikit-hep/hist/pull/453)
```

### Comparing `hist-2.6.3/docs/conf.py` & `hist-2.7.0/docs/conf.py`

 * *Files 23% similar despite different names*

```diff
@@ -4,55 +4,55 @@
 # list see the documentation:
 # https://www.sphinx-doc.org/en/master/usage/configuration.html
 
 from __future__ import annotations
 
 # Warning: do not change the path here. To use autodoc, you need to install the
 # package first.
-import os
-import shutil
-import sys
-from pathlib import Path
-
 from pkg_resources import get_distribution
 
-DIR = Path(__file__).parent.resolve()
-BASEDIR = DIR.parent
-
-sys.path.append(str(BASEDIR / "src/hist"))
-
 # -- Project information -----------------------------------------------------
 
 project = "Hist"
-copyright = "2020-2021, Henry Schreiner"
+copyright = "2020, Henry Schreiner"
 author = "Henry Schreiner and Nino Lau"
 version = get_distribution("hist").version
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
-    "sphinx.ext.autodoc",
+    "myst_parser",
     "nbsphinx",
+    "sphinx.ext.autodoc",
     "sphinx.ext.mathjax",
     "sphinx.ext.napoleon",
     "sphinx_copybutton",
-    "myst_parser",
+    "sphinxcontrib.programoutput",
 ]
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ["_templates"]
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This pattern also affects html_static_path and html_extra_path.
-exclude_patterns = ["_build", "**.ipynb_checkpoints", "Thumbs.db", ".DS_Store", ".env"]
+exclude_patterns = [
+    "**.ipynb_checkpoints",
+    ".DS_Store",
+    ".env",
+    "user-guide/notebooks/SVGHistogram.ipynb",
+    "Thumbs.db",
+    "_build",
+    "banner_slides.md",
+    "build",
+]
 
 
 # -- Options for HTML output -------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 #
@@ -87,28 +87,7 @@
 
 nbsphinx_execute_arguments = [
     "--InlineBackend.figure_formats={'png2x'}",
     "--InlineBackend.rc=figure.dpi=96",
 ]
 
 nbsphinx_kernel_name = "python3"
-
-
-def prepare(app):
-    outer = BASEDIR / ".github"
-    inner = DIR
-    contributing = "CONTRIBUTING.md"
-    shutil.copy(outer / contributing, inner / "contributing.md")
-
-
-def clean_up(app, exception):
-    inner = DIR
-    os.unlink(inner / "contributing.md")
-
-
-def setup(app):
-
-    # Copy the file in
-    app.connect("builder-inited", prepare)
-
-    # Clean up the generated file
-    app.connect("build-finished", clean_up)
```

### Comparing `hist-2.6.3/docs/index.rst` & `hist-2.7.0/docs/index.rst`

 * *Files 1% similar despite different names*

```diff
@@ -34,14 +34,15 @@
    user-guide/notebooks/Plots
    user-guide/analyses
    user-guide/numpy
    user-guide/subclassing
    user-guide/notebooks/Histogram
    user-guide/notebooks/Stack
    user-guide/notebooks/Interpolation
+   user-guide/cli
 
 .. toctree::
    :maxdepth: 2
    :titlesonly:
    :caption: Developers
    :glob:
```

### Comparing `hist-2.6.3/docs/make.bat` & `hist-2.7.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `hist-2.6.3/docs/support.rst` & `hist-2.7.0/docs/support.rst`

 * *Files identical despite different names*

### Comparing `hist-2.6.3/docs/_images/axis_category.png` & `hist-2.7.0/docs/_images/axis_category.png`

 * *Files identical despite different names*

### Comparing `hist-2.6.3/docs/_images/axis_circular.png` & `hist-2.7.0/docs/_images/axis_circular.png`

 * *Files identical despite different names*

### Comparing `hist-2.6.3/docs/_images/axis_integer.png` & `hist-2.7.0/docs/_images/axis_integer.png`

 * *Files identical despite different names*

### Comparing `hist-2.6.3/docs/_images/axis_regular.png` & `hist-2.7.0/docs/_images/axis_regular.png`

 * *Files identical despite different names*

### Comparing `hist-2.6.3/docs/_images/axis_variable.png` & `hist-2.7.0/docs/_images/axis_variable.png`

 * *Files identical despite different names*

### Comparing `hist-2.6.3/docs/_images/banner.gif` & `hist-2.7.0/docs/_images/banner.gif`

 * *Files identical despite different names*

### Comparing `hist-2.6.3/docs/_images/ex_hist_density.png` & `hist-2.7.0/docs/_images/ex_hist_density.png`

 * *Files identical despite different names*

### Comparing `hist-2.6.3/docs/_images/fullplot_example.png` & `hist-2.7.0/docs/_images/fullplot_example.png`

 * *Files identical despite different names*

### Comparing `hist-2.6.3/docs/_images/histlogo.png` & `hist-2.7.0/docs/_images/histlogo.png`

 * *Files identical despite different names*

### Comparing `hist-2.6.3/docs/_images/histlogo.svg` & `hist-2.7.0/docs/_images/histlogo.svg`

 * *Files identical despite different names*

### Comparing `hist-2.6.3/docs/_images/histogram_design.png` & `hist-2.7.0/docs/_images/histogram_design.png`

 * *Files identical despite different names*

### Comparing `hist-2.6.3/docs/_images/pieplot_example.png` & `hist-2.7.0/docs/_images/pieplot_example.png`

 * *Files identical despite different names*

### Comparing `hist-2.6.3/docs/_images/ratioplot_example.png` & `hist-2.7.0/docs/_images/ratioplot_example.png`

 * *Files identical despite different names*

### Comparing `hist-2.6.3/docs/_images/stackplot_example.png` & `hist-2.7.0/docs/_images/stackplot_example.png`

 * *Files identical despite different names*

### Comparing `hist-2.6.3/docs/_src/images/axis_category.tex` & `hist-2.7.0/docs/_src/images/axis_category.tex`

 * *Files identical despite different names*

### Comparing `hist-2.6.3/docs/_src/images/axis_circular.tex` & `hist-2.7.0/docs/_src/images/axis_circular.tex`

 * *Files identical despite different names*

### Comparing `hist-2.6.3/docs/_src/images/axis_integer.tex` & `hist-2.7.0/docs/_src/images/axis_integer.tex`

 * *Files identical despite different names*

### Comparing `hist-2.6.3/docs/_src/images/axis_regular.tex` & `hist-2.7.0/docs/_src/images/axis_regular.tex`

 * *Files identical despite different names*

### Comparing `hist-2.6.3/docs/_src/images/axis_variable.tex` & `hist-2.7.0/docs/_src/images/axis_variable.tex`

 * *Files identical despite different names*

### Comparing `hist-2.6.3/docs/examples/HistDemo.ipynb` & `hist-2.7.0/docs/examples/HistDemo.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9996323529411765%*

 * *Differences: {"'cells'": "{4: {'source': ['import numpy as np\\n', '\\n', 'from hist import Hist']}}"}*

```diff
@@ -32,16 +32,17 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "from hist import Hist\n",
-                "import numpy as np"
+                "import numpy as np\n",
+                "\n",
+                "from hist import Hist"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "We can use the classic constructors from boost-histogram, but let's use the new QuickConstruct system instead:"
```

### Comparing `hist-2.6.3/docs/user-guide/accumulators.rst` & `hist-2.7.0/docs/user-guide/accumulators.rst`

 * *Files identical despite different names*

### Comparing `hist-2.6.3/docs/user-guide/analyses.rst` & `hist-2.7.0/docs/user-guide/analyses.rst`

 * *Files identical despite different names*

### Comparing `hist-2.6.3/docs/user-guide/axes.rst` & `hist-2.7.0/docs/user-guide/axes.rst`

 * *Files 8% similar despite different names*

```diff
@@ -180,28 +180,33 @@
 
 One use for an IntCategory axis is for an IntEnum:
 
 .. code-block:: python3
 
     import enum
 
+
     class MyEnum(enum.IntEnum):
         a = 1
         b = 5
 
+
     my_enum_axis = hist.axis.IntEnum(list(MyEnum), underflow=False, overflow=False)
 
 
 You can sort the Categorty axes via ``.sort()`` method:
 
 .. code-block:: python3
 
-    h = Hist(axis.IntCategory([3, 1, 2], label="Number"), axis.StrCategory(["Teacher", "Police", "Artist"], label="Profession"))
-    h.sort(0).axes[0] # IntCategory([1, 2, 3], label='Number')
-    h.sort(1, reverse=True).axes[1] # StrCategory(['Teacher', 'Police', 'Artist'], label='Profession')
+    h = Hist(
+        axis.IntCategory([3, 1, 2], label="Number"),
+        axis.StrCategory(["Teacher", "Police", "Artist"], label="Profession"),
+    )
+    # Sort Number axis increasing and Profession axis decreasing
+    h1 = h.sort("Number").sort("Profession", reverse=True)
 
 
 .. py:function:: hist.axis.StrCategory([str1, ...], name, label, metadata="", growth=False)
    :noindex:
 
    You can put strings in a category axis as well. The fill method supports lists or arrays of strings
    to allow this to be filled.
```

### Comparing `hist-2.6.3/docs/user-guide/indexing.rst` & `hist-2.7.0/docs/user-guide/indexing.rst`

 * *Files identical despite different names*

### Comparing `hist-2.6.3/docs/user-guide/installation.rst` & `hist-2.7.0/docs/user-guide/installation.rst`

 * *Files identical despite different names*

### Comparing `hist-2.6.3/docs/user-guide/numpy.rst` & `hist-2.7.0/docs/user-guide/numpy.rst`

 * *Files 10% similar despite different names*

```diff
@@ -37,21 +37,23 @@
 If you try the following in an IPython session, you will get:
 
 .. code-block:: python3
 
    import numpy as np
    import hist
 
-   norm_vals = np.concatenate([
-       np.random.normal(loc=5, scale=1, size=1_000_000),
-       np.random.normal(loc=2, scale=.2, size=200_000),
-       np.random.normal(loc=8, scale=.2, size=200_000),
-   ])
+   norm_vals = np.concatenate(
+       [
+           np.random.normal(loc=5, scale=1, size=1_000_000),
+           np.random.normal(loc=2, scale=0.2, size=200_000),
+           np.random.normal(loc=8, scale=0.2, size=200_000),
+       ]
+   )
 
-.. code-block:: python3
+.. code-block:: ipython
 
    %%timeit
    bins, edges = np.histogram(norm_vals, bins=100, range=(0, 10))
 
 .. code-block:: text
 
    17.4 ms ± 2.64 ms per loop (mean ± std. dev. of 7 runs, 100 loops each)
@@ -60,15 +62,15 @@
 density, widths, and more, or in some cases you can change the
 computation call itself to add ``density=``, or use the matching
 function inside Matplotlib, and the API is different if you want 2D or
 ND histograms. But if you already use NumPy histograms and you really
 don’t want to rewrite your code, hist has adaptors for the
 three histogram functions in NumPy:
 
-.. code-block:: python3
+.. code-block:: ipython
 
    %%timeit
    bins, edges = hist.numpy.histogram(norm_vals, bins=100, range=(0, 10))
 
 .. code-block:: text
 
    7.3 ms ± 55.7 µs per loop (mean ± std. dev. of 7 runs, 100 loops each)
@@ -91,32 +93,29 @@
 
 
 2D Histogram example
 ^^^^^^^^^^^^^^^^^^^^
 
 .. code-block:: python3
 
-   data  = np.random.multivariate_normal(
-       (0, 0),
-       ((1, 0),(0, .5)),
-       10_000_000).T.copy()
+   data = np.random.multivariate_normal((0, 0), ((1, 0), (0, 0.5)), 10_000_000).T.copy()
 
 We can check the performance against NumPy again; NumPy does not do well
 with regular spaced bins in more than 1D:
 
-.. code-block:: python3
+.. code-block:: ipython
 
    %%timeit
    np.histogram2d(*data, bins=(400, 200), range=((-2, 2), (-1, 1)))
 
 .. code-block:: text
 
    1.31 s ± 17.3 ms per loop (mean ± std. dev. of 7 runs, 1 loop each)
 
-.. code-block:: python3
+.. code-block:: ipython
 
    %%timeit
    hist.numpy.histogram2d(*data, bins=(400, 200), range=((-2, 2), (-1, 1)))
 
 .. code-block:: text
 
    101 ms ± 117 µs per loop (mean ± std. dev. of 7 runs, 10 loops each)
```

### Comparing `hist-2.6.3/docs/user-guide/quickstart.rst` & `hist-2.7.0/docs/user-guide/quickstart.rst`

 * *Files 1% similar despite different names*

```diff
@@ -42,16 +42,15 @@
 Note that you have to specify the storage at the end (but this does make it easier to use ``Weight`` or other useful storages).
 
 The exact same syntax is used any number of dimensions:
 
 .. code-block:: python3
 
    hist3D = (
-        Hist.new
-       .Regular(10, 0, 100, circular=True, name="x")
+       Hist.new.Regular(10, 0, 100, circular=True, name="x")
        .Regular(10, 0.0, 10.0, name="y")
        .Variable([1, 2, 3, 4, 5, 5.5, 6], name="z")
        .Weight()
    )
 
 See :ref:`usage-axes` and :ref:`usage-transforms`.
 
@@ -81,15 +80,15 @@
 .. code-block:: python3
 
     h = Hist(
         hist.axis.Regular(10, 0, 1, name="x"),
         hist.axis.Regular(10, 0, 1, name="y"),
         hist.axis.Regular(10, 0, 1, name="z"),
     )
-    mini = h[1:5, .2j:.9j, sum]
+    mini = h[1:5, 0.2j:0.9j, sum]
     # Will be 4 bins x 7 bins
 
 See :ref:`usage-indexing`.
 
 .. _accessing-the-contents:
 
 Accessing the contents
```

### Comparing `hist-2.6.3/docs/user-guide/storages.rst` & `hist-2.7.0/docs/user-guide/storages.rst`

 * *Files 3% similar despite different names*

```diff
@@ -90,19 +90,15 @@
 
     1
     3
 
 .. code-block:: python3
 
     # Method 2
-    h = (
-        Hist.new.Reg(10, 0, 1, name="x")
-        .Int64()
-        .fill([0.5, 0.5])
-    )
+    h = Hist.new.Reg(10, 0, 1, name="x").Int64().fill([0.5, 0.5])
 
     print(h[0.5j])
 
 .. code-block:: text
 
     2
```

### Comparing `hist-2.6.3/docs/user-guide/subclassing.rst` & `hist-2.7.0/docs/user-guide/subclassing.rst`

 * *Files 0% similar despite different names*

```diff
@@ -9,17 +9,19 @@
 When you subclass, you will need to add a family. Any object can be used - the module for your library is a good choice if you only have one "family" of histograms. Hist uses ``hist``, Boost-histogram uses ``boost_histogram``. You can use anything you want, though; a custom tag object like ``MY_FAMILY = object()`` works well too. It just has to support ``is``, and be the exact same object on all your subclasses.
 
 .. code-block:: python3
 
     import hist
     import my_package
 
+
     class Histogram(hist.Hist, family=my_package):
         ...
 
+
     class Regular(hist.axis.Regular, family=my_package):
         ...
 
 If you only override ``Histogram``, you can leave off the ``family=`` argument, or set it to ``None``. It will generate a private ``object()`` in this case. You must add an explicit family to ``Histogram`` if you subclass any further components.
 
 If you use Mixins, special care needs to be taken if you need a left-acting
 Mixin, since class keywords are handled via ``super()`` left to right. This is
```

### Comparing `hist-2.6.3/docs/user-guide/notebooks/Histogram.ipynb` & `hist-2.7.0/docs/user-guide/notebooks/Histogram.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9994897959183673%*

 * *Differences: {"'cells'": "{4: {'source': ['import hist\\n', 'from hist import Hist']}, 43: {'source': ['import "*

 * *            "dask.array as da\\n', '\\n', 'import hist.dask as dah']}}"}*

```diff
@@ -38,16 +38,16 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "from hist import Hist\n",
-                "import hist"
+                "import hist\n",
+                "from hist import Hist"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "#### Standard method:"
@@ -506,16 +506,17 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "import hist.dask as dah\n",
-                "import dask.array as da"
+                "import dask.array as da\n",
+                "\n",
+                "import hist.dask as dah"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Hist\n",
```

### Comparing `hist-2.6.3/docs/user-guide/notebooks/Interpolation.ipynb` & `hist-2.7.0/docs/user-guide/notebooks/Interpolation.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999263468013468%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(2, 'import numpy as np\\n'), (3, 'from scipy import "*

 * *            "interpolate\\n'), (4, '\\n'), (5, 'from hist import Hist')], delete: [4, 2, 1]}}}"}*

```diff
@@ -16,18 +16,19 @@
             "cell_type": "code",
             "execution_count": null,
             "id": "6d3cc20c",
             "metadata": {},
             "outputs": [],
             "source": [
                 "# Make the necessary imports.\n",
-                "from scipy import interpolate\n",
-                "from hist import Hist, axis\n",
                 "import matplotlib.pyplot as plt\n",
-                "import numpy as np"
+                "import numpy as np\n",
+                "from scipy import interpolate\n",
+                "\n",
+                "from hist import Hist"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "c960dff2",
             "metadata": {},
```

### Comparing `hist-2.6.3/docs/user-guide/notebooks/Plots.ipynb` & `hist-2.7.0/docs/user-guide/notebooks/Plots.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9975260416666667%*

 * *Differences: {"'cells'": "{0: {'source': ['# Plots {#usage-plotting}'], 'attachments': OrderedDict()}, 2: "*

 * *            "{'source': ['import hist\\n', 'from hist import Hist']}}"}*

```diff
@@ -1,14 +1,15 @@
 {
     "cells": [
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "# Plots"
+                "# Plots {#usage-plotting}"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "One of the most amazing feature of hist is it's powerful plotting family. Here you can see how to plot Hist."
@@ -16,16 +17,16 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "from hist import Hist\n",
-                "import hist"
+                "import hist\n",
+                "from hist import Hist"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
```

### Comparing `hist-2.6.3/docs/user-guide/notebooks/Reprs.ipynb` & `hist-2.7.0/docs/user-guide/notebooks/Reprs.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9979166666666667%*

 * *Differences: {"'cells'": "{1: {'source': ['import numpy as np\\n', '\\n', 'from hist import Hist']}}"}*

```diff
@@ -11,16 +11,17 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "from hist import Hist\n",
-                "import numpy as np"
+                "import numpy as np\n",
+                "\n",
+                "from hist import Hist"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
```

### Comparing `hist-2.6.3/docs/user-guide/notebooks/SVGHistogram.ipynb` & `hist-2.7.0/docs/user-guide/notebooks/SVGHistogram.ipynb`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9988765009855163%*

 * *Differences: {"'cells'": '{2: {\'source\': {insert: [(25, \'        return f"<{self.start}/>"\')], delete: [26, '*

 * *            "25]}}, 4: {'source': {delete: [13, 12, 11, 10]}}, 9: {'source': {insert: [(2, 'import "*

 * *            "operator\\n'), (3, 'import textwrap\\n'), (4, '\\n'), (5, 'import boost_histogram as "*

 * *            "bh\\n'), (6, 'import numpy as np\\n'), (7, '\\n')], delete: [4, 2, 1, 0]}}, 10: "*

 * *            "{'source': {insert: [(6, '            return plot_hist_1d_c(self)._repr_svg_()\\n'), "*

 * *            "(7 […]*

```diff
@@ -41,16 +41,15 @@
                 "        return self.name + ending\n",
                 "\n",
                 "    def __str__(self):\n",
                 "        if self.contents:\n",
                 "            return \"<{self.start}>\\n{contents}\\n</{self.name}>\".format(\n",
                 "                self=self, contents=\"\\n\".join(str(s) for s in self.contents)\n",
                 "            )\n",
-                "        else:\n",
-                "            return f\"<{self.start}/>\""
+                "        return f\"<{self.start}/>\""
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Now let's add classes that exactly correspond to the `XML` tags:"
@@ -71,18 +70,14 @@
                 "    pass\n",
                 "\n",
                 "\n",
                 "class line(XML):\n",
                 "    pass\n",
                 "\n",
                 "\n",
-                "class rect(XML):\n",
-                "    pass\n",
-                "\n",
-                "\n",
                 "class ellipse(XML):\n",
                 "    pass\n",
                 "\n",
                 "\n",
                 "class polygon(XML):\n",
                 "    pass\n",
                 "\n",
@@ -136,20 +131,22 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "import textwrap\n",
-                "import numpy as np\n",
-                "import boost_histogram as bh\n",
                 "import functools\n",
-                "import operator\n",
                 "import math\n",
+                "import operator\n",
+                "import textwrap\n",
+                "\n",
+                "import boost_histogram as bh\n",
+                "import numpy as np\n",
+                "\n",
                 "import hist"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
@@ -157,20 +154,18 @@
             "source": [
                 "class Histogram(hist.Hist):\n",
                 "    def _repr_svg_(self):\n",
                 "        # This can be _repr_html_ instead, too - would make adding text easier/nicer\n",
                 "        if self.ndim == 1:\n",
                 "            if not self.axes[0].traits.circular:\n",
                 "                return plot_hist_1d(self)._repr_svg_()\n",
-                "            else:\n",
-                "                return plot_hist_1d_c(self)._repr_svg_()\n",
-                "        elif self.ndim == 2:\n",
+                "            return plot_hist_1d_c(self)._repr_svg_()\n",
+                "        if self.ndim == 2:\n",
                 "            return plot_hist_2d(self)._repr_svg_()\n",
-                "        else:\n",
-                "            return plot_hist_md(self)._repr_svg_()"
+                "        return plot_hist_md(self)._repr_svg_()"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Now let's make a svg plotting function:\n",
@@ -197,15 +192,14 @@
                 "        right_edge,\n",
                 "        pad_x=0,\n",
                 "        pad_y=0,\n",
                 "        opacity=1,\n",
                 "        stroke_width=2,\n",
                 "    ):\n",
                 "        width = right_edge - left_edge\n",
-                "        center_y = height / 2.0\n",
                 "        top_y = y\n",
                 "\n",
                 "        height = height * (1 - 2 * pad_y)\n",
                 "        top_y = top_y * (1 - 2 * pad_y) + pad_y\n",
                 "        left_edge = left_edge * (1 - 2 * pad_x) + pad_x\n",
                 "        width = width * (1 - 2 * pad_x)\n",
                 "        color = int(opacity * 255)\n",
@@ -225,18 +219,15 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "def plot_hist_1d(hi):\n",
                 "    assert hi.ndim == 1\n",
                 "    assert not hi.axes[0].traits.circular\n",
                 "\n",
-                "    if len(hi.axes[0]) > 40:\n",
-                "        h = hi[:: bh.rebin(len(hi.axes[0]) // 20)]\n",
-                "    else:\n",
-                "        h = hi\n",
+                "    h = hi[:: bh.rebin(len(hi.axes[0]) // 20)] if len(hi.axes[0]) > 40 else hi\n",
                 "\n",
                 "    (edges,) = h.axes.edges\n",
                 "    norm_edges = (edges - edges[0]) / (edges[-1] - edges[0])\n",
                 "    norm_vals = h.view()\n",
                 "\n",
                 "    if not h.empty():\n",
                 "        norm_vals /= functools.reduce(operator.mul, h.axes.widths) / h.sum()\n",
@@ -453,31 +444,30 @@
                 "                    style=\"fill:white;stroke-width:3;stroke:rgb(0,0,0)\",\n",
                 "                )\n",
                 "            )\n",
                 "        )\n",
                 "\n",
                 "    polylines = [\n",
                 "        polyline(\n",
-                "            points=\"\"\n",
-                "            + f\"{3*20}, {3*20+105} \"\n",
-                "            + f\"{3*20+30}, {3*20+105} \"\n",
-                "            + f\"{3*20+30}, {3*20+95} \"\n",
-                "            + f\"{3*20+40}, {3*20+95} \"\n",
-                "            + f\"{3*20+40}, {3*20+70} \"\n",
-                "            + f\"{3*20+50}, {3*20+70} \"\n",
-                "            + f\"{3*20+50}, {3*20+52} \"\n",
-                "            + f\"{3*20+60}, {3*20+52} \"\n",
-                "            + f\"{3*20+60}, {3*20+45} \"\n",
-                "            + f\"{3*20+70}, {3*20+45} \"\n",
-                "            + f\"{3*20+70}, {3*20+65} \"\n",
-                "            + f\"{3*20+80}, {3*20+65} \"\n",
-                "            + f\"{3*20+80}, {3*20+95} \"\n",
-                "            + f\"{3*20+90}, {3*20+95} \"\n",
-                "            + f\"{3*20+90}, {3*20+105} \"\n",
-                "            + f\"{3*20+120}, {3*20+105} \",\n",
+                "            points=f\"{3*20}, {3*20+105} \"\n",
+                "            f\"{3*20+30}, {3*20+105} \"\n",
+                "            f\"{3*20+30}, {3*20+95} \"\n",
+                "            f\"{3*20+40}, {3*20+95} \"\n",
+                "            f\"{3*20+40}, {3*20+70} \"\n",
+                "            f\"{3*20+50}, {3*20+70} \"\n",
+                "            f\"{3*20+50}, {3*20+52} \"\n",
+                "            f\"{3*20+60}, {3*20+52} \"\n",
+                "            f\"{3*20+60}, {3*20+45} \"\n",
+                "            f\"{3*20+70}, {3*20+45} \"\n",
+                "            f\"{3*20+70}, {3*20+65} \"\n",
+                "            f\"{3*20+80}, {3*20+65} \"\n",
+                "            f\"{3*20+80}, {3*20+95} \"\n",
+                "            f\"{3*20+90}, {3*20+95} \"\n",
+                "            f\"{3*20+90}, {3*20+105} \"\n",
+                "            f\"{3*20+120}, {3*20+105} \",\n",
                 "            style=\"fill:none;stroke:black;stroke-width:2\",\n",
                 "        ),\n",
                 "    ]\n",
                 "\n",
                 "    names = \"\"\n",
                 "    for i in range(hi.ndim):\n",
                 "        names += str(hi.axes[i].name or hi.axes[i].label)\n",
@@ -529,36 +519,31 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "def plot_hist_1d_c(hi):\n",
                 "    assert hi.ndim == 1\n",
                 "    assert hi.axes[0].traits.circular\n",
                 "\n",
-                "    if len(hi.axes[0]) > 40:\n",
-                "        h = hi[:: bh.rebin(len(hi.axes[0]) // 20)]\n",
-                "    else:\n",
-                "        h = hi\n",
+                "    h = hi[:: bh.rebin(len(hi.axes[0]) // 20)] if len(hi.axes[0]) > 40 else hi\n",
                 "\n",
                 "    (edges,) = h.axes.edges\n",
-                "    norm_edges = (edges - edges[0]) / (edges[-1] - edges[0])\n",
                 "    norm_vals = h.view()\n",
                 "\n",
                 "    if not h.empty():\n",
                 "        norm_vals /= functools.reduce(operator.mul, h.axes.widths) / h.sum()\n",
                 "        norm_vals /= np.max(norm_vals)\n",
                 "\n",
                 "    polygons = []\n",
                 "    ang = math.pi * 2 / (len(edges) - 1)\n",
                 "    for i in range(len(edges) - 1):\n",
                 "        polygons.append(\n",
                 "            polygon(\n",
-                "                points=\"\"\n",
-                "                + \"150, 125 \"\n",
-                "                + f\"{150+100*norm_vals[i] * math.cos(i * ang)}, {125+100*norm_vals[i] * math.sin(i * ang)} \"\n",
-                "                + f\"{150+100*norm_vals[i] * math.cos((i+1) * ang)}, {125+100*norm_vals[i] * math.sin((i+1) * ang)} \",\n",
+                "                points=\"150, 125 \"\n",
+                "                f\"{150+100*norm_vals[i] * math.cos(i * ang)}, {125+100*norm_vals[i] * math.sin(i * ang)} \"\n",
+                "                f\"{150+100*norm_vals[i] * math.cos((i+1) * ang)}, {125+100*norm_vals[i] * math.sin((i+1) * ang)} \",\n",
                 "                style=\"fill:none;stroke:black;stroke-width:2\",\n",
                 "            )\n",
                 "        )\n",
                 "\n",
                 "    circles = [\n",
                 "        circle(\n",
                 "            cx=\"150\",\n",
@@ -587,15 +572,16 @@
                 "            x=140,\n",
                 "            y=125 + 100 * max(norm_vals),\n",
                 "            style=\"font-family: monospace\",\n",
                 "        ),\n",
                 "    ]\n",
                 "\n",
                 "    return svg(*polygons, *texts, *circles, width=800, height=250)\n",
-                "    pass"
+                "    pass\n",
+                "    return None"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
```

### Comparing `hist-2.6.3/docs/user-guide/notebooks/Stack.ipynb` & `hist-2.7.0/docs/user-guide/notebooks/Stack.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998081140350877%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(1, 'import numpy as np\\n'), (2, '\\n'), (3, 'import "*

 * *            "hist\\n'), (4, 'from hist import Hist\\n')], delete: [2, 1, 0]}}}"}*

```diff
@@ -15,18 +15,19 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "2ce95976",
             "metadata": {},
             "outputs": [],
             "source": [
-                "from hist import Hist\n",
-                "import hist\n",
-                "import numpy as np\n",
                 "import matplotlib.pyplot as plt\n",
+                "import numpy as np\n",
+                "\n",
+                "import hist\n",
+                "from hist import Hist\n",
                 "\n",
                 "ax = hist.axis.Regular(25, -5, 5, flow=False, name=\"x\")\n",
                 "cax = hist.axis.StrCategory([\"signal\", \"upper\", \"lower\"], name=\"c\")\n",
                 "full_hist = Hist(ax, cax)\n",
                 "\n",
                 "full_hist.fill(x=np.random.normal(size=600), c=\"signal\")\n",
                 "full_hist.fill(x=2 * np.random.normal(size=500) + 2, c=\"upper\")\n",
```

### Comparing `hist-2.6.3/docs/user-guide/notebooks/Transform.ipynb` & `hist-2.7.0/docs/user-guide/notebooks/Transform.ipynb`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.992890625%*

 * *Differences: {"'cells'": "{0: {'source': ['# Transform {#usage-transforms}\\n'], 'attachments': OrderedDict()}, "*

 * *            "3: {'source': {insert: [(2, '\\n'), (3, 'import numpy as np\\n'), (4, '\\n'), (5, "*

 * *            "'import hist\\n'), (6, 'from hist import Hist')], delete: [4, 1, 0]}}}"}*

```diff
@@ -1,18 +1,15 @@
 {
     "cells": [
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "# Transform\n",
-                "\n",
-                "```warning\n",
-                "The hist package is still under active development, the usage and contents are in flux.\n",
-                "```"
+                "# Transform {#usage-transforms}\n"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Based on [boost-histogram](https://github.com/scikit-hep/boost-histogram)'s Transform, hist provides a powerful transform system on Regular axes that allows you to provide a functional form for the conversion between a regular spacing and the actual bin edges. The following transforms are built in:\n",
@@ -34,19 +31,21 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "import hist\n",
-                "from hist import Hist\n",
                 "import ctypes\n",
                 "import math\n",
-                "import numpy as np"
+                "\n",
+                "import numpy as np\n",
+                "\n",
+                "import hist\n",
+                "from hist import Hist"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
```

### Comparing `hist-2.6.3/notebooks/HistLogo.ipynb` & `hist-2.7.0/notebooks/HistLogo.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9995659722222222%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(1, 'import numpy as np\\n'), (6, '\\n')], delete: [5]}}}"}*

```diff
@@ -14,19 +14,20 @@
             "cell_type": "code",
             "execution_count": 1,
             "id": "professional-order",
             "metadata": {},
             "outputs": [],
             "source": [
                 "import matplotlib.pyplot as plt\n",
+                "import numpy as np\n",
                 "import PIL.Image\n",
                 "import PIL.ImageDraw\n",
                 "import PIL.ImageFilter\n",
                 "import PIL.ImageFont\n",
-                "import numpy as np\n",
+                "\n",
                 "import hist"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 2,
             "id": "confidential-usage",
```

### Comparing `hist-2.6.3/notebooks/axestuple-setattr.ipynb` & `hist-2.7.0/notebooks/axestuple-setattr.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9986979166666667%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(0, 'from hist import Hist\\n')], delete: [0]}}}"}*

```diff
@@ -13,15 +13,15 @@
         {
             "cell_type": "code",
             "execution_count": 1,
             "id": "64ab1f7d-0a8d-4ffa-bff2-e9e5268995f7",
             "metadata": {},
             "outputs": [],
             "source": [
-                "from hist import axis, Hist\n",
+                "from hist import Hist\n",
                 "\n",
                 "h = Hist.new.Reg(50, -3, 3, name=\"X\").Reg(50, -3, 3, name=\"Y\").Double()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 2,
```

### Comparing `hist-2.6.3/src/hist/__init__.py` & `hist-2.7.0/src/hist/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from types import ModuleType
 
 from . import accumulators, axis, numpy, storage, tag
 from .basehist import BaseHist
 from .hist import Hist
 from .namedhist import NamedHist
 from .stack import Stack
-from .tag import (  # pylint: disable=redefined-builtin
+from .tag import (
     loc,
     overflow,
     rebin,
     sum,
     underflow,
 )
 
@@ -48,13 +48,12 @@
 
 
 def __dir__() -> tuple[str, ...]:
     return __all__
 
 
 def __getattr__(name: str) -> ModuleType:
-
     if name == "axes":
         msg = f"Misspelling error, '{name}' should be 'axis'"
-        warnings.warn(msg)
+        warnings.warn(msg, stacklevel=2)
         return axis
     raise AttributeError(f"module {__name__} has no attribute {name}")
```

### Comparing `hist-2.6.3/src/hist/axestuple.py` & `hist-2.7.0/src/hist/axestuple.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,16 @@
 from __future__ import annotations
 
-import sys
 import warnings
-from collections.abc import Iterable, Iterator
+from collections.abc import Iterable
 from typing import Any
 
 from boost_histogram.axis import ArrayTuple, AxesTuple
 
-if sys.version_info < (3, 10):
-    import builtins
-    import itertools
-
-    # pylint: disable-next=redefined-builtin
-    def zip(*iterables: Any, strict: bool = False) -> Iterator[tuple[Any, ...]]:
-        if strict:
-            marker = object()
-            for each in itertools.zip_longest(*iterables, fillvalue=marker):
-                for val in each:
-                    if val is marker:
-                        raise ValueError("zip() arguments are not the same length")
-                yield each
-        else:
-            yield from builtins.zip(*iterables)
-
+from ._compat.builtins import zip
 
 __all__ = ("NamedAxesTuple", "AxesTuple", "ArrayTuple")
 
 
 def __dir__() -> tuple[str, ...]:
     return __all__
 
@@ -70,15 +54,15 @@
 
         disallowed_names = {"weight", "sample", "threads"}
         for ax in self:
             if ax.name in disallowed_names:
                 disallowed_warning = (
                     f"{ax.name} is a protected keyword and cannot be used as axis name"
                 )
-                warnings.warn(disallowed_warning)
+                warnings.warn(disallowed_warning, stacklevel=2)
 
         valid_names = [ax.name for ax in self if ax.name]
         if len(valid_names) != len(set(valid_names)):
             raise KeyError(
                 f"{self.__class__.__name__} instance cannot contain axes with duplicated names"
             )
```

### Comparing `hist-2.6.3/src/hist/basehist.py` & `hist-2.7.0/src/hist/basehist.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 from __future__ import annotations
 
 import functools
 import operator
 import typing
 import warnings
-from typing import Any, Callable, Iterator, Mapping, Sequence, Tuple, TypeVar, Union
+from typing import Any, Callable, Iterator, Mapping, Sequence, Tuple, Union
 
 import boost_histogram as bh
 import histoprint
 import numpy as np
 
 import hist
 
+from . import interop
+from ._compat.typing import ArrayLike, Protocol, Self, SupportsIndex
 from .axestuple import NamedAxesTuple
 from .axis import AxisProtocol
 from .quick_construct import MetaConstructor
 from .storage import Storage
 from .svgplots import html_hist, svg_hist_1d, svg_hist_1d_c, svg_hist_2d
-from .typing import ArrayLike, Protocol, SupportsIndex
 
 if typing.TYPE_CHECKING:
     from builtins import ellipsis
 
     import matplotlib.axes
     from mplhep.plot import Hist1DArtists, Hist2DArtists
 
@@ -48,17 +49,14 @@
         else "linestyle"
         if k == "ls"
         else k: v
         for k, v in kwargs.items()
     }
 
 
-T = TypeVar("T", bound="BaseHist")
-
-
 class BaseHist(bh.Histogram, metaclass=MetaConstructor, family=hist):
     __slots__ = ()
 
     def __init__(
         self,
         *args: AxisProtocol | Storage | str | tuple[int, float, float],
         storage: Storage | str | None = None,
@@ -92,26 +90,26 @@
             if storage_str == "Atomicint64":
                 storage_str = "AtomicInt64"
             elif storage_str == "Weightedmean":
                 storage_str = "WeightedMean"
             storage = getattr(bh.storage, storage_str)()
         elif isinstance(storage, type):
             msg = f"Please use '{storage.__name__}()' instead of '{storage.__name__}'"
-            warnings.warn(msg)
+            warnings.warn(msg, stacklevel=2)
             storage = storage()
 
         super().__init__(*args, storage=storage, metadata=metadata)  # type: ignore[call-overload]
 
         disallowed_names = {"weight", "sample", "threads"}
         for ax in self.axes:
             if ax.name in disallowed_names:
                 disallowed_warning = (
                     f"{ax.name} is a protected keyword and cannot be used as axis name"
                 )
-                warnings.warn(disallowed_warning)
+                warnings.warn(disallowed_warning, stacklevel=2)
 
         valid_names = [ax.name for ax in self.axes if ax.name]
         if len(valid_names) != len(set(valid_names)):
             raise KeyError(
                 f"{self.__class__.__name__} instance cannot contain axes with duplicated names"
             )
         for i, ax in enumerate(self.axes):
@@ -137,26 +135,24 @@
 
         return NamedAxesTuple(self._axis(i) for i in range(self.ndim))
 
     def _repr_html_(self) -> str | None:
         if self.size == 0:
             return None
 
-        if self.ndim == 1:
-            if len(self.axes[0]) <= 1000:
-                return str(
-                    html_hist(
-                        self,
-                        svg_hist_1d_c if self.axes[0].traits.circular else svg_hist_1d,
-                    )
+        if self.ndim == 1 and len(self.axes[0]) <= 1000:
+            return str(
+                html_hist(
+                    self,
+                    svg_hist_1d_c if self.axes[0].traits.circular else svg_hist_1d,
                 )
+            )
 
-        if self.ndim == 2:
-            if len(self.axes[0]) <= 200 and len(self.axes[1]) <= 200:
-                return str(html_hist(self, svg_hist_2d))
+        if self.ndim == 2 and len(self.axes[0]) <= 200 and len(self.axes[1]) <= 200:
+            return str(html_hist(self, svg_hist_2d))
 
         return None
 
     def _name_to_index(self, name: str) -> int:
         """
             Transform axis name to axis index, given axis name, return axis \
             index.
@@ -165,21 +161,21 @@
             if name == axis.name:
                 return index
 
         raise ValueError(f"The axis name {name} could not be found")
 
     @classmethod
     def from_columns(
-        cls: type[T],
+        cls,
         data: Mapping[str, ArrayLike],
         axes: Sequence[str | AxisProtocol],
         *,
         weight: str | None = None,
         storage: hist.storage.Storage = hist.storage.Double(),  # noqa: B008
-    ) -> T:
+    ) -> Self:
         axes_list: list[Any] = []
         for ax in axes:
             if isinstance(ax, str):
                 assert ax in data, f"{ax} must be present in data={list(data)}"
                 cats = set(data[ax])  # type: ignore[arg-type]
                 if all(isinstance(a, str) for a in cats):
                     axes_list.append(hist.axis.StrCategory(sorted(cats), name=ax))  # type: ignore[arg-type]
@@ -197,29 +193,29 @@
         weight_arr = data[weight] if weight else None
 
         self = cls(*axes_list, storage=storage)
         data_list = {x.name: data[x.name] for x in axes_list}
         self.fill(**data_list, weight=weight_arr)  # type: ignore[arg-type]
         return self
 
-    def project(self: T, *args: int | str) -> T | float | bh.accumulators.Accumulator:
+    def project(self, *args: int | str) -> Self | float | bh.accumulators.Accumulator:
         """
         Projection of axis idx.
         """
         int_args = [self._name_to_index(a) if isinstance(a, str) else a for a in args]
         return super().project(*int_args)
 
     def fill(
-        self: T,
+        self,
         *args: ArrayLike,
         weight: ArrayLike | None = None,
         sample: ArrayLike | None = None,
         threads: int | None = None,
         **kwargs: ArrayLike,
-    ) -> T:
+    ) -> Self:
         """
         Insert data into the histogram using names and indices, return
         a Hist object.
         """
 
         data_dict = {
             self._name_to_index(k) if isinstance(k, str) else k: v
@@ -231,30 +227,96 @@
                 "All axes must be accounted for in fill, you may have used a disallowed name in the axes"
             )
 
         data = (data_dict[i] for i in range(len(args), self.ndim))
 
         return super().fill(*args, *data, weight=weight, sample=sample, threads=threads)
 
+    def fill_flattened(
+        self: Self,
+        *args: Any,
+        weight: Any | None = None,
+        sample: Any | None = None,
+        threads: int | None = None,
+        **kwargs: Any,
+    ) -> Self:
+        axis_names = {ax.name for ax in self.axes}
+
+        non_user_kwargs = {}
+        if weight is not None:
+            non_user_kwargs["weight"] = weight
+        if sample is not None:
+            non_user_kwargs["sample"] = sample
+
+        # Single arguments are either arrays for single-dimensional histograms, or
+        # structures for multi-dimensional hists that must first be unpacked
+        if len(args) == 1 and not kwargs:
+            (arg,) = args
+            destructured = interop.destructure(arg)
+            # Try to unpack the array, if it's valid to do so, i.e. is the Awkward Array a record array?
+            if destructured is None:
+                # Can't unpack, fall back on broadcasting single array (to flatten and convert)
+                broadcast = interop.broadcast_and_flatten(
+                    (arg, *non_user_kwargs.values())
+                )
+                # Partition out non-user args
+                user_args_broadcast = broadcast[:1]
+                user_kwargs_broadcast = {}
+                non_user_kwargs_broadcast = dict(
+                    zip(non_user_kwargs.keys(), broadcast[1:])
+                )
+            else:
+                # Result must be broadcast, so unpack and rebuild
+                broadcast = interop.broadcast_and_flatten(
+                    (*destructured.values(), *non_user_kwargs.values())
+                )
+                # Partition into user and non-user args
+                user_args_broadcast = ()
+                user_kwargs_broadcast = {
+                    k: v
+                    for k, v in zip(destructured, broadcast[: len(destructured)])
+                    if k in axis_names
+                }
+                non_user_kwargs_broadcast = dict(
+                    zip(non_user_kwargs, broadcast[len(destructured) :])
+                )
+        # Multiple args: broadcast and flatten!
+        else:
+            inputs = (*args, *kwargs.values(), *non_user_kwargs)
+            broadcast = interop.broadcast_and_flatten(inputs)
+            user_args_broadcast = broadcast[: len(args)]
+            user_kwargs_broadcast = dict(
+                zip(kwargs, broadcast[len(args) : len(args) + len(kwargs)])
+            )
+            non_user_kwargs_broadcast = dict(
+                zip(non_user_kwargs, broadcast[len(args) + len(kwargs) :])
+            )
+        return self.fill(
+            *user_args_broadcast,
+            **user_kwargs_broadcast,
+            threads=threads,
+            **non_user_kwargs_broadcast,
+        )
+
     def sort(
-        self: T,
+        self,
         axis: int | str,
         key: (
             Callable[[int], SupportsLessThan] | Callable[[str], SupportsLessThan] | None
         ) = None,
         reverse: bool = False,
-    ) -> T:
+    ) -> Self:
         """
         Sort a categorical axis.
         """
 
         with warnings.catch_warnings():
             warnings.simplefilter("ignore")
             sorted_cats = sorted(self.axes[axis], key=key, reverse=reverse)
-            # This can only return T, not float, etc., so we ignore the extra types here
+            # This can only return Self, not float, etc., so we ignore the extra types here
             return self[{axis: [bh.loc(x) for x in sorted_cats]}]  # type: ignore[dict-item, return-value]
 
     def _loc_shortcut(self, x: Any) -> Any:
         """
         Convert some specific indices to location.
         """
 
@@ -311,16 +373,16 @@
 
         if not isinstance(index, tuple):
             index = (index,)  # type: ignore[assignment]
 
         return tuple(self._loc_shortcut(v) for v in index)  # type: ignore[union-attr, union-attr, union-attr, union-attr]
 
     def __getitem__(  # type: ignore[override]
-        self: T, index: IndexingExpr
-    ) -> T | float | bh.accumulators.Accumulator:
+        self, index: IndexingExpr
+    ) -> Self | float | bh.accumulators.Accumulator:
         """
         Get histogram item.
         """
 
         return super().__getitem__(self._index_transform(index))
 
     def __setitem__(  # type: ignore[override]
@@ -328,15 +390,15 @@
     ) -> None:
         """
         Set histogram item.
         """
 
         return super().__setitem__(self._index_transform(index), value)
 
-    def profile(self: T, axis: int | str) -> T:
+    def profile(self, axis: int | str) -> Self:
         """
         Returns a profile (Mean/WeightedMean) histogram from a normal histogram
         with N-1 axes. The axis given is profiled over and removed from the
         final histogram.
         """
 
         if self.kind != bh.Kind.COUNT:
@@ -510,15 +572,14 @@
 
     def plot_pie(
         self,
         *,
         ax: matplotlib.axes.Axes | None = None,
         **kwargs: Any,
     ) -> Any:
-
         from hist import plot
 
         return plot.plot_pie(self, ax=ax, **kwargs)
 
     def stack(self, axis: int | str) -> hist.stack.Stack:
         """
         Returns a stack from a normal histogram axes.
@@ -529,14 +590,30 @@
             self[{axis: i}] for i in range(len(self.axes[axis]))
         ]
         for name, h in zip(self.axes[axis], stack_histograms):
             h.name = name
 
         return hist.stack.Stack(*stack_histograms)
 
+    def integrate(
+        self,
+        name: int | str,
+        i_or_list: InnerIndexing | list[str | int] | None = None,
+        j: InnerIndexing | None = None,
+    ) -> Self | float | bh.accumulators.Accumulator:
+        if isinstance(i_or_list, list):
+            with warnings.catch_warnings():
+                warnings.simplefilter("ignore")
+
+                # TODO: We could teach the typing system that list always returns Self type
+                selection: Self = self[{name: i_or_list}]  # type: ignore[assignment, dict-item]
+                return selection[{name: slice(0, len(i_or_list), sum)}]
+
+        return self[{name: slice(i_or_list, j, sum)}]
+
     def sum(self, flow: bool = False) -> float | bh.accumulators.Accumulator:
         """
         Compute the sum over the histogram bins (optionally including the flow bins).
         """
         # TODO: This method will go away once we can guarantee a modern boost-histogram (1.3.2 or better)
         if any(x == 0 for x in (self.axes.extent if flow else self.axes.size)):
             storage = self.storage_type
```

### Comparing `hist-2.6.3/src/hist/classichist.py` & `hist-2.7.0/src/hist/classichist.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 import argparse
 import shutil
 import sys
+from pathlib import Path
 
 import boost_histogram as bh
 from histoprint import print_hist
 
 import hist
 
 
@@ -23,19 +24,19 @@
         help="maximum screen width",
         default=shutil.get_terminal_size()[0],
     )
     parser.add_argument("-t", "--label", type=str, help="label for plot")
     parser.add_argument("-o", "--output-image", type=str, help="save image to file")
     args = parser.parse_args()
 
-    print(
+    print(  # noqa: T201
         "Classic hist interface - please use histoprint instead; this supports multiple file formats and much more!"
     )
 
-    with open(args.input, encoding="utf-8") if args.input else sys.stdin as f:
+    with Path(args.input).open(encoding="utf-8") if args.input else sys.stdin as f:
         values = [float(v) for v in f]
 
     h = bh.numpy.histogram(values, bins=args.buckets, histogram=hist.Hist)
 
     if args.output_image:
         import matplotlib.pyplot as plt
```

### Comparing `hist-2.6.3/src/hist/intervals.py` & `hist-2.7.0/src/hist/intervals.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from __future__ import annotations
 
 from typing import Any
 
 import numpy as np
 
-from .typing import Literal
+from ._compat.typing import Literal
 
 try:
     from scipy import stats
 except ModuleNotFoundError:
     from sys import stderr
 
-    print(
+    print(  # noqa: T201
         "hist.intervals requires scipy. Please install hist[plot] or manually install scipy.",
         file=stderr,
     )
     raise
 
 __all__ = ("poisson_interval", "clopper_pearson_interval", "ratio_uncertainty")
 
@@ -70,16 +70,15 @@
         counts: np.typing.NDArray[Any] = values / scale
         interval_min = scale * stats.chi2.ppf((1 - coverage) / 2, 2 * counts) / 2.0
         interval_min[values == 0.0] = 0.0  # chi2.ppf produces NaN for values=0
         interval_max = (
             scale * stats.chi2.ppf((1 + coverage) / 2, 2 * (counts + 1)) / 2.0
         )
         interval_max[values == 0.0] = np.nan
-    interval = np.stack((interval_min, interval_max))
-    return interval  # type: ignore[no-any-return]
+    return np.stack((interval_min, interval_max))
 
 
 def clopper_pearson_interval(
     num: np.typing.NDArray[Any],
     denom: np.typing.NDArray[Any],
     coverage: float | None = None,
 ) -> np.typing.NDArray[Any]:
```

### Comparing `hist-2.6.3/src/hist/plot.py` & `hist-2.7.0/src/hist/plot.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,23 +4,23 @@
 import sys
 from typing import Any, Callable, Iterable, NamedTuple, Union
 
 import numpy as np
 
 import hist
 
-from .typing import Literal
+from ._compat.typing import Literal
 
 try:
     import matplotlib.axes
     import matplotlib.pyplot as plt
     from matplotlib import patches, transforms
     from mplhep.plot import Hist1DArtists, Hist2DArtists, hist2dplot, histplot
 except ModuleNotFoundError:
-    print(
+    print(  # noqa: T201
         "Hist requires mplhep to plot, either install hist[plot] or mplhep",
         file=sys.stderr,
     )
     raise
 
 __all__ = (
     "hist2dplot",
@@ -118,15 +118,15 @@
             continue
         if ix < len(g) - 1 and g[ix + 1][1] in {".", "("}:
             continue
         varnames.append(tokval)
     varnames = list(OrderedDict.fromkeys([name for name in varnames if name != "x"]))
     lambdastr = f"lambda x,{','.join(varnames)}: {expr}"
     # pylint: disable-next=eval-used
-    return eval(lambdastr)  # type: ignore[no-any-return]
+    return eval(lambdastr)  # type: ignore[no-any-return]  # noqa: PGH001
 
 
 def _curve_fit_wrapper(
     func: Callable[..., Any],
     xdata: np.typing.NDArray[Any],
     ydata: np.typing.NDArray[Any],
     yerr: np.typing.NDArray[Any],
@@ -136,15 +136,15 @@
     Wrapper around `scipy.optimize.curve_fit`. Initial parameters (`p0`)
     can be set in the function definition with defaults for kwargs
     (e.g., `func = lambda x,a=1.,b=2.: x+a+b`, will feed `p0 = [1.,2.]` to `curve_fit`)
     """
     try:
         from scipy.optimize import curve_fit, minimize
     except ModuleNotFoundError:
-        print(_PLT_MISSING_MSG, file=sys.stderr)
+        print(_PLT_MISSING_MSG, file=sys.stderr)  # noqa: T201
         raise
 
     params = list(inspect.signature(func).parameters.values())
     p0 = [
         1 if arg.default is inspect.Parameter.empty else arg.default
         for arg in params[1:]
     ]
@@ -158,15 +158,15 @@
         absolute_sigma=True,
         p0=p0,
     )
     if likelihood:
         try:
             from iminuit import Minuit
         except ModuleNotFoundError:
-            print(_PLT_MISSING_MSG, file=sys.stderr)
+            print(_PLT_MISSING_MSG, file=sys.stderr)  # noqa: T201
             raise
         from scipy.special import gammaln
 
         def fnll(v: Iterable[np.typing.NDArray[Any]]) -> float:
             ypred = func(xdata, *v)
             if (ypred <= 0.0).any():
                 return 1e6
@@ -694,15 +694,14 @@
 
 def plot_pie(
     self: hist.BaseHist,
     *,
     ax: matplotlib.axes.Axes | None = None,
     **kwargs: Any,
 ) -> Any:
-
     if ax is None:
         fig = plt.gcf()
         ax = fig.add_subplot(111)
 
     data = self.density()
 
     labels = [str(get_center(x)) for x in self.axes[0]]
@@ -713,20 +712,18 @@
 def plot_stack(
     self: hist.stack.Stack,
     *,
     ax: matplotlib.axes.Axes | None = None,
     legend: bool | None = False,
     **kwargs: Any,
 ) -> Any:
-
     if self[0].ndim != 1:
         raise NotImplementedError("Please project to 1D before calling plot")
 
-    if "label" not in kwargs:
-        if all(h.name is not None for h in self):
-            kwargs["label"] = [h.name for h in self]
+    if "label" not in kwargs and all(h.name is not None for h in self):
+        kwargs["label"] = [h.name for h in self]
 
     ret = histplot(list(self), ax=ax, **kwargs)
     final_ax = ret[0].stairs.axes
     _plot_keywords_wrapper(final_ax, legend=legend)
 
     return ret
```

### Comparing `hist-2.6.3/src/hist/quick_construct.py` & `hist-2.7.0/src/hist/quick_construct.py`

 * *Files identical despite different names*

### Comparing `hist-2.6.3/src/hist/stack.py` & `hist-2.7.0/src/hist/stack.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 from __future__ import annotations
 
 import copy
 import typing
-from typing import Any, Iterator, TypeVar
+from typing import Any, Iterator
 
 import histoprint
 import numpy as np
 
+from ._compat.typing import Self
 from .axestuple import NamedAxesTuple
 from .basehist import BaseHist
 
 if typing.TYPE_CHECKING:
-    import matplotlib
+    import matplotlib as mpl
 
 
 __all__ = ("Stack",)
 
-T = TypeVar("T", bound="Stack")
-
 
 class Stack:
     def __init__(
         self,
         *args: BaseHist,
     ) -> None:
         """
@@ -38,22 +37,22 @@
 
         first_axes = args[0].axes
         for a in args[1:]:
             if first_axes != a.axes:
                 raise ValueError("The Histogram axes don't match")
 
     @classmethod
-    def from_iter(cls: type[T], iterable: typing.Iterable[BaseHist]) -> T:
+    def from_iter(cls, iterable: typing.Iterable[BaseHist]) -> Self:
         """
         Create a Stack from an iterable of histograms.
         """
         return cls(*iterable)
 
     @classmethod
-    def from_dict(cls: type[T], d: typing.Mapping[str, BaseHist]) -> T:
+    def from_dict(cls, d: typing.Mapping[str, BaseHist]) -> Self:
         """
         Create a Stack from a dictionary of histograms. The keys of the
         dictionary are used as names.
         """
 
         new_dict = {k: copy.copy(h) for k, h in d.items()}
         for k, h in new_dict.items():
@@ -73,29 +72,29 @@
         raise IndexError(f"Name not found: {name}")
 
     @typing.overload
     def __getitem__(self, val: int | str) -> BaseHist:
         ...
 
     @typing.overload
-    def __getitem__(self: T, val: slice) -> T:
+    def __getitem__(self, val: slice) -> Self:
         ...
 
-    def __getitem__(self: T, val: int | slice | str) -> BaseHist | T:
+    def __getitem__(self, val: int | slice | str) -> BaseHist | Self:
         if isinstance(val, str):
             val = self._get_index(val)
         if isinstance(val, slice):
             my_slice = slice(
                 self._get_index(val.start), self._get_index(val.stop), val.step
             )
             return self.__class__(*self._stack.__getitem__(my_slice))
 
         return self._stack.__getitem__(val)
 
-    def __setitem__(self: T, key: int | str, value: BaseHist) -> None:
+    def __setitem__(self, key: int | str, value: BaseHist) -> None:
         """
         Set a histogram in the Stack. Checks the axes of the histogram, they must match.
         """
         if not isinstance(value, BaseHist):
             raise ValueError("The value should be a histogram")
         if isinstance(key, str):
             key = self._get_index(key)
@@ -120,88 +119,87 @@
             return False
         return self._stack == other._stack
 
     @property
     def axes(self) -> NamedAxesTuple:
         return self._stack[0].axes
 
-    def plot(self, *, ax: matplotlib.axes.Axes | None = None, **kwargs: Any) -> Any:
+    def plot(self, *, ax: mpl.axes.Axes | None = None, **kwargs: Any) -> Any:
         """
         Plot method for Stack object.
         """
 
         import hist.plot
 
         return hist.plot.plot_stack(self, ax=ax, **kwargs)
 
-    def show(self, **kwargs: Any) -> Any:
+    def show(self, **kwargs: object) -> Any:
         """
         Pretty print the stacked histograms to the console.
         """
-        if "labels" not in kwargs:
-            if all(h.name is not None for h in self):
-                kwargs["labels"] = [h.name for h in self]
+        if "labels" not in kwargs and all(h.name is not None for h in self):
+            kwargs["labels"] = [h.name for h in self]
 
         return histoprint.print_hist(list(self), stack=True, **kwargs)
 
-    def __mul__(self: T, other: float) -> T:
+    def __mul__(self, other: float) -> Self:
         """
         Multiply the Stack by a scalar.
         """
         return self.__class__(*(h * other for h in self))
 
-    def __imul__(self: T, other: float) -> T:
+    def __imul__(self, other: float) -> Self:
         """
         Multiply each histogram in the Stack by a scalar.
         """
         for h in self:
-            h *= other
+            h *= other  # noqa: PLW2901
         return self
 
-    def __rmul__(self: T, other: float) -> T:
+    def __rmul__(self, other: float) -> Self:
         """
         Multiply the Stack by a scalar.
         """
         return self.__mul__(other)
 
-    def __add__(self: T, other: float | np.typing.NDArray[Any]) -> T:
+    def __add__(self, other: float | np.typing.NDArray[Any]) -> Self:
         """
         Add a scalar or array to the Stack.
         """
         return self.__class__(*(h + other for h in self))
 
-    def __iadd__(self: T, other: float | np.typing.NDArray[Any]) -> T:
+    def __iadd__(self, other: float | np.typing.NDArray[Any]) -> Self:
         """
         Add a scalar or array to the Stack.
         """
         for h in self:
-            h += other
+            h += other  # noqa: PLW2901
         return self
 
-    def __radd__(self: T, other: float | np.typing.NDArray[Any]) -> T:
+    def __radd__(self, other: float | np.typing.NDArray[Any]) -> Self:
         """
         Add a scalar or array to the Stack.
         """
         return self.__add__(other)
 
-    def __sub__(self: T, other: float | np.typing.NDArray[Any]) -> T:
+    def __sub__(self, other: float | np.typing.NDArray[Any]) -> Self:
         """
         Subtract a scalar or array to the Stack.
         """
         return self.__class__(*(h - other for h in self))
 
-    def __isub__(self: T, other: float | np.typing.NDArray[Any]) -> T:
+    def __isub__(self, other: float | np.typing.NDArray[Any]) -> Self:
         """
         Subtract a scalar or array to the Stack.
         """
         for h in self:
-            h -= other
+            h -= other  # noqa: PLW2901
         return self
 
-    def project(self: T, *args: int | str) -> T:
+    def project(self, *args: int | str) -> Self:
         """
         Project the Stack onto a new axes.
         """
         return self.__class__(*(h.project(*args) for h in self))  # type: ignore[arg-type]
 
 
 def __dir__() -> tuple[str, ...]:
```

### Comparing `hist-2.6.3/src/hist/svgplots.py` & `hist-2.7.0/src/hist/svgplots.py`

 * *Files identical despite different names*

### Comparing `hist-2.6.3/src/hist/svgutils.py` & `hist-2.7.0/src/hist/svgutils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 from __future__ import annotations
 
-from typing import TypeVar
-
-from .typing import Protocol
+from ._compat.typing import Protocol, Self
 
 
 class SupportsStr(Protocol):
     def __str__(self) -> str:
         ...
 
 
@@ -62,33 +60,30 @@
     pass
 
 
 class div(XML):
     pass
 
 
-T = TypeVar("T", bound="rect")
-
-
 class rect(XML):
     @classmethod
     def pad(
-        cls: type[T],
+        cls,
         x: float,
         y: float,
         scale_x: float,
         scale_y: float,
         height: float,
         left_edge: float,
         right_edge: float,
         pad_x: float = 0,
         pad_y: float = 0,
         opacity: float = 1,
         stroke_width: float = 2,
-    ) -> T:
+    ) -> Self:
         width = right_edge - left_edge
         top_y = y
 
         height *= 1 - 2 * pad_y
         top_y = top_y * (1 - 2 * pad_y) + pad_y
         width = width * (1 - 2 * pad_x)
         color = int(opacity * 255)
```

### Comparing `hist-2.6.3/src/hist/typing.py` & `hist-2.7.0/src/hist/_compat/typing.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,20 +4,25 @@
 from typing import TYPE_CHECKING, Any
 
 if sys.version_info < (3, 8):
     from typing_extensions import Literal, Protocol, SupportsIndex
 else:
     from typing import Literal, Protocol, SupportsIndex
 
+if sys.version_info < (3, 11):
+    from typing_extensions import Self
+else:
+    from typing import Self
+
 if TYPE_CHECKING:
     from numpy import ufunc as Ufunc
     from numpy.typing import ArrayLike
 else:
     ArrayLike = Any
     Ufunc = Any
 
 
-__all__ = ("Literal", "Protocol", "SupportsIndex", "Ufunc", "ArrayLike")
+__all__ = ["Literal", "Protocol", "SupportsIndex", "Ufunc", "ArrayLike", "Self"]
 
 
-def __dir__() -> tuple[str, ...]:
+def __dir__() -> list[str]:
     return __all__
```

### Comparing `hist-2.6.3/src/hist/axis/__init__.py` & `hist-2.7.0/src/hist/axis/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,17 @@
 from __future__ import annotations
 
-import sys
 from typing import Any, Iterable
 
 import boost_histogram.axis as bha
 
 import hist
-from hist.axestuple import ArrayTuple, NamedAxesTuple
-
-if sys.version_info >= (3, 8):
-    from typing import Protocol
-else:
-    from typing_extensions import Protocol
 
+from .._compat.typing import Protocol
+from ..axestuple import ArrayTuple, NamedAxesTuple
 from . import transform
 
 __all__ = (
     "AxisProtocol",
     "AxesMixin",
     "Regular",
     "Variable",
```

### Comparing `hist-2.6.3/tests/conftest.py` & `hist-2.7.0/tests/conftest.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,30 +9,30 @@
     import hist.dask as dah
 except ImportError:
     dah = None
 
 
 @pytest.fixture(params=[Hist, BaseHist, NamedHist])
 def named_hist(request):
-    yield request.param
+    return request.param
 
 
 @pytest.fixture(params=[Hist, BaseHist])
 def unnamed_hist(request):
-    yield request.param
+    return request.param
 
 
 dask_params_named = []
 dask_params_unnamed = []
 if dah is not None:
     dask_params_named = [dah.Hist, dah.NamedHist]
     dask_params_unnamed = [dah.Hist]
 
 
 @pytest.fixture(params=dask_params_named)
 def named_dask_hist(request):
-    yield request.param
+    return request.param
 
 
 @pytest.fixture(params=dask_params_unnamed)
 def unnamed_dask_hist(request):
-    yield request.param
+    return request.param
```

### Comparing `hist-2.6.3/tests/test_axestuple.py` & `hist-2.7.0/tests/test_axestuple.py`

 * *Files identical despite different names*

### Comparing `hist-2.6.3/tests/test_axis.py` & `hist-2.7.0/tests/test_axis.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,14 +54,13 @@
     )
     assert axis.Integer(0, 8, flow=False, overflow=True) == axis.Integer(
         0, 8, underflow=False
     )
 
 
 def test_axis_disallowed_names():
-
     with pytest.warns(UserWarning):
         hist.Hist(axis.Regular(10, 0, 10, name="weight"))
     with pytest.warns(UserWarning):
         hist.Hist(axis.Regular(10, 0, 10, name="sample"))
     with pytest.warns(UserWarning):
         hist.Hist(axis.Regular(10, 0, 10, name="threads"))
```

### Comparing `hist-2.6.3/tests/test_bh.py` & `hist-2.7.0/tests/test_bh.py`

 * *Files identical despite different names*

### Comparing `hist-2.6.3/tests/test_dask.py` & `hist-2.7.0/tests/test_dask.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,18 +55,20 @@
         control.fill(strcat="testcat1", intcat=1, x=xTc[0], y=xTc[1], z=xTc[2])
         control.fill(strcat="testcat2", intcat=2, x=xTc[0], y=xTc[1], z=xTc[2])
 
     assert np.allclose(h.counts(), control.counts())
     if use_weights:
         assert np.allclose(h.variances(), control.variances())
 
-    assert len(h.axes[0]) == 2 and len(control.axes[0]) == 2
+    assert len(h.axes[0]) == 2
+    assert len(control.axes[0]) == 2
     assert all(cx == hx for cx, hx in zip(control.axes[0], h.axes[0]))
 
-    assert len(h.axes[1]) == 2 and len(control.axes[1]) == 2
+    assert len(h.axes[1]) == 2
+    assert len(control.axes[1]) == 2
     assert all(cx == hx for cx, hx in zip(control.axes[1], h.axes[1]))
 
 
 @pytest.mark.parametrize("use_weights", [True, False])
 def test_named_5D_strcat_intcat_rectangular(named_dask_hist, use_weights):
     x = da.random.standard_normal(size=(2000, 3), chunks=(400, 3))
     if use_weights:
@@ -112,12 +114,14 @@
         control.fill(strcat="testcat1", intcat=1, x=xTc[0], y=xTc[1], z=xTc[2])
         control.fill(strcat="testcat2", intcat=2, x=xTc[0], y=xTc[1], z=xTc[2])
 
     assert np.allclose(h.counts(), control.counts())
     if use_weights:
         assert np.allclose(h.variances(), control.variances())
 
-    assert len(h.axes[0]) == 2 and len(control.axes[0]) == 2
+    assert len(h.axes[0]) == 2
+    assert len(control.axes[0]) == 2
     assert all(cx == hx for cx, hx in zip(control.axes[0], h.axes[0]))
 
-    assert len(h.axes[1]) == 2 and len(control.axes[1]) == 2
+    assert len(h.axes[1]) == 2
+    assert len(control.axes[1]) == 2
     assert all(cx == hx for cx, hx in zip(control.axes[1], h.axes[1]))
```

### Comparing `hist-2.6.3/tests/test_general.py` & `hist-2.7.0/tests/test_general.py`

 * *Files 2% similar despite different names*

```diff
@@ -660,17 +660,16 @@
         Hist.new.Reg(24, 1, 5).Func(ftype(math.log), ftype(math.exp))
 
     # wrong value raises uncatchable warning
     # Hist.new.Func(
     #     4, -1, 5, forward=ftype(math.log), inverse=ftype(math.log)
     # ).Double()
 
-    with pytest.raises(ValueError):
-        with pytest.warns(RuntimeWarning):
-            Hist.new.Func(4, -1, 5, forward=ftype(np.log), inverse=ftype(np.log))
+    with pytest.raises(ValueError), pytest.warns(RuntimeWarning):
+        Hist.new.Func(4, -1, 5, forward=ftype(np.log), inverse=ftype(np.log))
 
     # lack args
     with pytest.raises(TypeError):
         Hist.new.Func(4, 1, 5)
 
 
 def test_hist_proxy_matches(named_hist):
@@ -684,16 +683,15 @@
     """
 
     h = Hist.new.Reg(10, 0, 1, name="x").Double().fill([0.5, 0.5])
     assert h[0.5j] == 2
 
     assert type(h) == Hist
 
-    with pytest.raises(AttributeError):
-        Hist().new
+    assert not hasattr(Hist(), "new")
 
     h = (
         Hist.new.Reg(10, 0, 1, name="x")
         .Reg(10, 0, 1, name="y")
         .Double()
         .fill([0.5, 0.5], [0.2, 0.6])
     )
@@ -834,36 +832,36 @@
     )
 
     with pytest.raises(TypeError):
         named_hist.from_columns(columns, (axis.Integer(1, 5), "y"), weight="data")
 
 
 def test_from_array(named_hist):
-    h = Hist(
+    h = named_hist(
         axis.Regular(10, 1, 2, name="A"),
         axis.Regular(7, 1, 3, name="B"),
         data=np.ones((10, 7)),
     )
     assert h.values() == approx(np.ones((10, 7)))
     assert h.sum() == approx(70)
     assert h.sum(flow=True) == approx(70)
 
-    h = Hist(
+    h = named_hist(
         axis.Regular(10, 1, 2, name="A"),
         axis.Regular(7, 1, 3, name="B"),
         data=np.ones((12, 9)),
     )
 
     assert h.values(flow=False) == approx(np.ones((10, 7)))
     assert h.values(flow=True) == approx(np.ones((12, 9)))
     assert h.sum() == approx(70)
     assert h.sum(flow=True) == approx(12 * 9)
 
     with pytest.raises(ValueError):
-        h = Hist(
+        h = named_hist(
             axis.Regular(10, 1, 2, name="A"),
             axis.Regular(7, 1, 3, name="B"),
             data=np.ones((11, 9)),
         )
 
 
 def test_sum_empty_axis():
@@ -921,7 +919,37 @@
 def test_quick_construct_direct():
     h = hist.new.IntCat([4, 1, 2]).StrCat(["AB", "BCC", "BC"]).Double()
     assert tuple(h.sort(0).axes[0]) == (1, 2, 4)
     assert tuple(h.sort(0, reverse=True).axes[0]) == (4, 2, 1)
     assert tuple(h.sort(0, key=lambda x: -x).axes[0]) == (4, 2, 1)
     assert tuple(h.sort(1).axes[1]) == ("AB", "BC", "BCC")
     assert tuple(h.sort(1, reverse=True).axes[1]) == ("BCC", "BC", "AB")
+
+
+def test_integrate():
+    h = (
+        hist.new.IntCat([4, 1, 2], name="x")
+        .StrCat(["AB", "BCC", "BC"], name="y")
+        .Int(1, 10, name="z")
+        .Int64()
+    )
+    h.fill(4, "AB", 1)
+    h.fill(4, "BCC", 2)
+    h.fill(4, "BC", 4)
+    h.fill(4, "X", 8)
+
+    h.fill(2, "aAB", 3)
+    h.fill(2, "BCC", 5)
+    h.fill(2, "AB", 2)
+    h.fill(2, "X", 1)
+
+    h.fill(1, "AB", 3)
+    h.fill(1, "BCC", 1)
+    h.fill(1, "BC", 5)
+    h.fill(1, "X", 2)
+
+    h1 = h.integrate("y", ["AB", "BC"]).integrate("z")
+    h2 = h.integrate("y", ["AB", "BC", "BCC"]).integrate("z")
+
+    assert h1[{"x": 4j}] == 2
+    assert h1[{"x": 2j}] == 1
+    assert h2[{"x": 1j}] == 3
```

### Comparing `hist-2.6.3/tests/test_intervals.py` & `hist-2.7.0/tests/test_intervals.py`

 * *Files identical despite different names*

### Comparing `hist-2.6.3/tests/test_mock_plot.py` & `hist-2.7.0/tests/test_mock_plot.py`

 * *Files identical despite different names*

### Comparing `hist-2.6.3/tests/test_named.py` & `hist-2.7.0/tests/test_named.py`

 * *Files 0% similar despite different names*

```diff
@@ -701,19 +701,18 @@
         NamedHist.new.Reg(24, 1, 5, name="x").Func(ftype(math.log), ftype(math.exp))
 
     # Uncatchable warning
     # assert NamedHist.new.Func(
     #     4, -1, 5, name="x", forward=ftype(math.log), inverse=ftype(math.log)
     # )
 
-    with pytest.raises(ValueError):
-        with pytest.warns(RuntimeWarning):
-            NamedHist.new.Func(
-                4, -1, 5, name="x", forward=ftype(np.log), inverse=ftype(np.log)
-            )
+    with pytest.raises(ValueError), pytest.warns(RuntimeWarning):
+        NamedHist.new.Func(
+            4, -1, 5, name="x", forward=ftype(np.log), inverse=ftype(np.log)
+        )
 
     # lack args
     with pytest.raises(TypeError):
         NamedHist.new.Func(4, 1, 5, name="x")
 
 
 def test_named_hist_proxy():
@@ -722,16 +721,15 @@
     """
 
     h = NamedHist.new.Reg(10, 0, 1, name="x").Double().fill(x=[0.5, 0.5])
     assert h[0.5j] == 2
 
     assert type(h) is NamedHist
 
-    with pytest.raises(AttributeError):
-        NamedHist().new
+    assert not hasattr(NamedHist(), "new")
 
     h = (
         NamedHist.new.Reg(10, 0, 1, name="x")
         .Reg(10, 0, 1, name="y")
         .Double()
         .fill(x=[0.5, 0.5], y=[0.2, 0.6])
     )
```

### Comparing `hist-2.6.3/tests/test_plot.py` & `hist-2.7.0/tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `hist-2.6.3/tests/test_profile.py` & `hist-2.7.0/tests/test_profile.py`

 * *Files identical despite different names*

### Comparing `hist-2.6.3/tests/test_reprs.py` & `hist-2.7.0/tests/test_reprs.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,107 +1,97 @@
 from __future__ import annotations
 
-from hist import Hist, Stack, axis
+from hist import Stack, axis
 
 
 def test_1D_empty_repr(named_hist):
-
     h = named_hist.new.Reg(10, -1, 1, name="x", label="y").Double()
     html = h._repr_html_()
     assert html
     assert "name='x'" in repr(h)
     assert "label='y'" in repr(h)
 
 
 def test_1D_var_empty_repr(named_hist):
-
     h = named_hist.new.Var(range(10), name="x", label="y").Double()
     html = h._repr_html_()
     assert html
     assert "name='x'" in repr(h)
     assert "label='y'" in repr(h)
 
 
 def test_1D_int_empty_repr(named_hist):
-
     h = named_hist.new.Int(-9, 9, name="x", label="y").Double()
     html = h._repr_html_()
     assert html
     assert "name='x'" in repr(h)
     assert "label='y'" in repr(h)
 
 
 def test_1D_intcat_empty_repr(named_hist):
-
     h = named_hist.new.IntCat([1, 3, 5], name="x", label="y").Double()
     html = h._repr_html_()
     assert html
     assert "name='x'" in repr(h)
     assert "label='y'" in repr(h)
 
 
 def test_1D_strcat_empty_repr(named_hist):
-
     h = named_hist.new.StrCat(["1", "3", "5"], name="x", label="y").Double()
     html = h._repr_html_()
     assert html
     assert "name='x'" in repr(h)
     assert "label='y'" in repr(h)
 
 
 def test_2D_empty_repr(named_hist):
-
     h = (
         named_hist.new.Reg(10, -1, 1, name="x", label="y")
         .Int(0, 15, name="p", label="q")
         .Double()
     )
     html = h._repr_html_()
     assert html
     assert "name='x'" in repr(h)
     assert "name='p'" in repr(h)
     assert "label='y'" in repr(h)
     assert "label='q'" in repr(h)
 
 
 def test_1D_circ_empty_repr(named_hist):
-
     h = named_hist.new.Reg(10, -1, 1, circular=True, name="R", label="r").Double()
     html = h._repr_html_()
     assert html
     assert "name='R'" in repr(h)
     assert "label='r'" in repr(h)
 
 
 def test_ND_empty_repr(named_hist):
-
     h = (
         named_hist.new.Reg(10, -1, 1, name="x", label="y")
         .Reg(12, -3, 3, name="p", label="q")
         .Reg(15, -2, 4, name="a", label="b")
         .Double()
     )
     html = h._repr_html_()
     assert html is None
 
 
 def test_empty_mega_repr(named_hist):
-
     h = named_hist.new.Reg(1001, -1, 1, name="x").Double()
     html = h._repr_html_()
     assert html is None
 
     h = named_hist.new.Reg(201, -1, 1, name="x").Reg(100, 0, 1, name="y").Double()
     html = h._repr_html_()
     assert html is None
 
 
 def test_stack_repr(named_hist):
-
     a1 = axis.Regular(
         50, -5, 5, name="A", label="a [unit]", underflow=False, overflow=False
     )
     a2 = axis.Regular(
         50, -5, 5, name="A", label="a [unit]", underflow=False, overflow=False
     )
-    assert "name='A'" in repr(Stack(Hist(a1), Hist(a2)))
-    assert "label='a [unit]'" in repr(Stack(Hist(a1), Hist(a2)))
+    assert "name='A'" in repr(Stack(named_hist(a1), named_hist(a2)))
+    assert "label='a [unit]'" in repr(Stack(named_hist(a1), named_hist(a2)))
```

### Comparing `hist-2.6.3/tests/test_stacks.py` & `hist-2.7.0/tests/test_stacks.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 
 import numpy as np
 import pytest
 from pytest import approx
 
 from hist import Hist, NamedHist, Stack, axis
 
+np.random.seed(42)
+
 # different histograms here!
 reg_ax = axis.Regular(10, 0, 1)
 boo_ax = axis.Boolean()
 var_ax = axis.Variable(range(-3, 3))
 int_ax = axis.Integer(-3, 3)
 int_cat_ax = axis.IntCategory(range(-3, 3))
 str_cat_ax = axis.StrCategory(["F", "T"])
```

### Comparing `hist-2.6.3/tests/baseline/test_image_plot_pull.png` & `hist-2.7.0/tests/baseline/test_image_plot_pull.png`

 * *Files identical despite different names*

### Comparing `hist-2.6.3/tests/baseline/test_image_plot_ratio_callable.png` & `hist-2.7.0/tests/baseline/test_image_plot_ratio_callable.png`

 * *Files identical despite different names*

### Comparing `hist-2.6.3/tests/baseline/test_image_plot_ratio_hist.png` & `hist-2.7.0/tests/baseline/test_image_plot_ratio_hist.png`

 * *Files identical despite different names*

### Comparing `hist-2.6.3/.gitignore` & `hist-2.7.0/.gitignore`

 * *Files identical despite different names*

### Comparing `hist-2.6.3/LICENSE` & `hist-2.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hist-2.6.3/README.md` & `hist-2.7.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -59,14 +59,16 @@
   - Histogram arguments (like `data=`) can go in the storage.
 
 - Extended Histogram features:
   - Direct support for `.name` and `.label`, like axes.
   - `.density()` computes the density as an array.
   - `.profile(remove_ax)` can convert a ND COUNT histogram into a (N-1)D MEAN histogram.
   - `.sort(axis)` supports sorting a histogram by a categorical axis. Optionally takes a function to sort by.
+  - `.fill_flattened(...)` will flatten and fill, including support for AwkwardArray.
+  - `.integrate(...)`, which takes the opposite arguments as `.project`.
 
 - Hist implements UHI+; an extension to the UHI (Unified Histogram Indexing) system designed for import-free interactivity:
   - Uses `j` suffix to switch to data coordinates in access or slices.
   - Uses `j` suffix on slices to rebin.
   - Strings can be used directly to index into string category axes.
 
 - Quick plotting routines encourage exploration:
@@ -93,29 +95,28 @@
 ## Usage
 
 ```python
 from hist import Hist
 
 # Quick construction, no other imports needed:
 h = (
-  Hist.new
-  .Reg(10, 0 ,1, name="x", label="x-axis")
-  .Var(range(10), name="y", label="y-axis")
-  .Int64()
+    Hist.new.Reg(10, 0, 1, name="x", label="x-axis")
+    .Var(range(10), name="y", label="y-axis")
+    .Int64()
 )
 
 # Filling by names is allowed:
 h.fill(y=[1, 4, 6], x=[3, 5, 2])
 
 # Names can be used to manipulate the histogram:
 h.project("x")
 h[{"y": 0.5j + 3, "x": 5j}]
 
 # You can access data coordinates or rebin with a `j` suffix:
-h[.3j:, ::2j] # x from .3 to the end, y is rebinned by 2
+h[0.3j:, ::2j]  # x from .3 to the end, y is rebinned by 2
 
 # Elegant plotting functions:
 h.plot()
 h.plot2d_full()
 h.plot_pull(Callable)
 ```
```

### Comparing `hist-2.6.3/pyproject.toml` & `hist-2.7.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     "dask-histogram",
 ]
 requires-python = ">=3.7"
 dependencies = [
     "boost-histogram~=1.3.1",
     "histoprint>=2.2.0",
     "numpy>=1.14.5",
-    'typing-extensions>=3.7;python_version<"3.8"',
+    'typing-extensions>=4;python_version<"3.11"',
 ]
 dynamic = ["version"]
 
 [project.scripts]
 hist = "hist.classichist:main"
 
 [project.urls]
@@ -56,54 +56,54 @@
 mpl = [
     "matplotlib >=3.0",
     "mplhep >=0.2.16",
 ]
 plot = [
     "matplotlib >=3.0",
     "mplhep >=0.2.16",
-    "scipy >=1.4; python_version<'3.11'",
-    "iminuit >=2; python_version<'3.11'",
+    "scipy >=1.4",
+    "iminuit >=2",
 ]
 dask = [
-    "dask[dataframe] >=2022; python_version>'3.7'",
-    "dask_histogram >=2023.1; python_version>'3.7'"
+    "dask[dataframe] >=2022; python_version>='3.8'",
+    "dask_histogram >=2023.1; python_version>='3.8'"
 ]
 test = [
     "pytest >=6",
     "pytest-mpl >=0.12",
-    "dask[dataframe] >=2022; python_version>'3.7'",
-    "dask_histogram >=2023.1; python_version>'3.7'",
+    "dask[dataframe] >=2022; python_version>='3.8'",
+    "dask_histogram >=2023.1; python_version>='3.8'",
 ]
 dev = [
     "pytest >=6",
     "pytest-mpl >=0.12",
     "matplotlib >=3.0",
     "mplhep >=0.2.16",
-    "scipy >=1.4; python_version<'3.11'",
+    "scipy >=1.4",
     "iminuit >=2; python_version<'3.11'",
     "ipykernel",
-    "dask[dataframe] >=2022; python_version>'3.7'",
-    "dask_histogram >=2023.1; python_version>'3.7'",
+    "dask[dataframe] >=2022; python_version>='3.8'",
+    "dask_histogram >=2023.1; python_version>='3.8'",
 ]
 docs = [
     "pytest >=6",
     "pytest-mpl >=0.12",
     "matplotlib >=3.0",
     "mplhep >=0.2.16",
-    "scipy >=1.4; python_version<'3.11'",
-    "iminuit >=2; python_version<'3.11'",
+    "scipy >=1.4",
+    "iminuit >=2",
     "ipython_genutils",
     "graphviz >=0.20.1",
-    "dask[dataframe] >=2022; python_version>'3.7'",
-    "dask_histogram >=2023.1; python_version>'3.7'",
+    "dask[dataframe] >=2022; python_version>='3.8'",
+    "dask_histogram >=2023.1; python_version>='3.8'",
     "nbsphinx",
-    "Sphinx >=3.0.0",
+    "sphinx >=3.0.0",
     "sphinx_copybutton",
-    "sphinx_rtd_theme >=0.5.0",
     "sphinx_book_theme >=0.0.38",
+    "sphinxcontrib-programoutput",
     "ipython",
     "ipykernel",
     "pillow",
     "uncertainties>=3",
     "myst_parser>=0.14",
 ]
 
@@ -120,20 +120,14 @@
 required_plugins = ["pytest-mpl"]
 log_cli_level = "DEBUG"
 filterwarnings = [
     "error",
     "ignore::matplotlib._api.deprecation.MatplotlibDeprecationWarning"
 ]
 
-[tool.nbqa.mutate]
-pyupgrade = 1
-
-[tool.isort]
-profile = "black"
-
 [tool.mypy]
 warn_unused_configs = true
 files = "src"
 python_version = "3.8"
 strict = true
 show_error_codes = true
 enable_error_code = ["ignore-without-code", "truthy-bool"]
@@ -177,8 +171,43 @@
   "too-many-statements",
   "wrong-import-position",
   "duplicate-code",
   "import-outside-toplevel",
   "import-error",
   "disallowed-name",
   "cyclic-import",
+  "redefined-builtin",
 ]
+
+[tool.ruff]
+select = [
+  "E", "F", "W", # flake8
+  "B",  "B904",  # flake8-bugbear
+  "I",           # isort
+  "ARG",         # flake8-unused-arguments
+  "C4",          # flake8-comprehensions
+  "ICN",         # flake8-import-conventions
+  "ISC",         # flake8-implicit-str-concat
+  "PGH",         # pygrep-hooks
+  "PIE",         # flake8-pie
+  "PL",          # pylint
+  "PT",          # flake8-pytest-style
+  "PTH",         # flake8-use-pathlib
+  "RET",         # flake8-return
+  "RUF",         # Ruff-specific
+  "SIM",         # flake8-simplify
+  "T20",         # flake8-print
+  "UP",          # pyupgrade
+  "YTT",         # flake8-2020
+]
+extend-ignore = ["PLR", "E501", "PT011", "PT013", "PT004", "B017"]
+typing-modules = ["hist._compat.typing"]
+src = ["src"]
+unfixable = ["T20", "F841"]
+exclude = []
+isort.required-imports = ["from __future__ import annotations"]
+flake8-unused-arguments.ignore-variadic-names = true
+
+[tool.ruff.per-file-ignores]
+"tests/test_plot.py" = ["B008"]
+"docs/conf.py" = ["ARG001", "PTH"]
+"noxfile.py" = ["T20"]
```

### Comparing `hist-2.6.3/PKG-INFO` & `hist-2.7.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hist
-Version: 2.6.3
+Version: 2.7.0
 Summary: Hist classes and utilities
 Project-URL: Homepage, https://github.com/scikit-hep/hist
 Project-URL: Documentation, https://hist.readthedocs.io/
 Project-URL: Bug Tracker, https://github.com/scikit-hep/hist/issues
 Project-URL: Discussions, https://github.com/scikit-hep/hist/discussions
 Project-URL: Changelog, https://hist.readthedocs.io/en/latest/changelog.html
 Author-email: Henry Schreiner <henry.schreiner@cern.ch>
@@ -29,60 +29,60 @@
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Requires-Dist: boost-histogram~=1.3.1
 Requires-Dist: histoprint>=2.2.0
 Requires-Dist: numpy>=1.14.5
-Requires-Dist: typing-extensions>=3.7; python_version < '3.8'
+Requires-Dist: typing-extensions>=4; python_version < '3.11'
 Provides-Extra: dask
-Requires-Dist: dask-histogram>=2023.1; python_version > '3.7' and extra == 'dask'
-Requires-Dist: dask[dataframe]>=2022; python_version > '3.7' and extra == 'dask'
+Requires-Dist: dask-histogram>=2023.1; python_version >= '3.8' and extra == 'dask'
+Requires-Dist: dask[dataframe]>=2022; python_version >= '3.8' and extra == 'dask'
 Provides-Extra: dev
-Requires-Dist: dask-histogram>=2023.1; python_version > '3.7' and extra == 'dev'
-Requires-Dist: dask[dataframe]>=2022; python_version > '3.7' and extra == 'dev'
+Requires-Dist: dask-histogram>=2023.1; python_version >= '3.8' and extra == 'dev'
+Requires-Dist: dask[dataframe]>=2022; python_version >= '3.8' and extra == 'dev'
 Requires-Dist: iminuit>=2; python_version < '3.11' and extra == 'dev'
 Requires-Dist: ipykernel; extra == 'dev'
 Requires-Dist: matplotlib>=3.0; extra == 'dev'
 Requires-Dist: mplhep>=0.2.16; extra == 'dev'
 Requires-Dist: pytest-mpl>=0.12; extra == 'dev'
 Requires-Dist: pytest>=6; extra == 'dev'
-Requires-Dist: scipy>=1.4; python_version < '3.11' and extra == 'dev'
+Requires-Dist: scipy>=1.4; extra == 'dev'
 Provides-Extra: docs
-Requires-Dist: dask-histogram>=2023.1; python_version > '3.7' and extra == 'docs'
-Requires-Dist: dask[dataframe]>=2022; python_version > '3.7' and extra == 'docs'
+Requires-Dist: dask-histogram>=2023.1; python_version >= '3.8' and extra == 'docs'
+Requires-Dist: dask[dataframe]>=2022; python_version >= '3.8' and extra == 'docs'
 Requires-Dist: graphviz>=0.20.1; extra == 'docs'
-Requires-Dist: iminuit>=2; python_version < '3.11' and extra == 'docs'
+Requires-Dist: iminuit>=2; extra == 'docs'
 Requires-Dist: ipykernel; extra == 'docs'
 Requires-Dist: ipython; extra == 'docs'
 Requires-Dist: ipython-genutils; extra == 'docs'
 Requires-Dist: matplotlib>=3.0; extra == 'docs'
 Requires-Dist: mplhep>=0.2.16; extra == 'docs'
 Requires-Dist: myst-parser>=0.14; extra == 'docs'
 Requires-Dist: nbsphinx; extra == 'docs'
 Requires-Dist: pillow; extra == 'docs'
 Requires-Dist: pytest-mpl>=0.12; extra == 'docs'
 Requires-Dist: pytest>=6; extra == 'docs'
-Requires-Dist: scipy>=1.4; python_version < '3.11' and extra == 'docs'
+Requires-Dist: scipy>=1.4; extra == 'docs'
 Requires-Dist: sphinx-book-theme>=0.0.38; extra == 'docs'
 Requires-Dist: sphinx-copybutton; extra == 'docs'
-Requires-Dist: sphinx-rtd-theme>=0.5.0; extra == 'docs'
 Requires-Dist: sphinx>=3.0.0; extra == 'docs'
+Requires-Dist: sphinxcontrib-programoutput; extra == 'docs'
 Requires-Dist: uncertainties>=3; extra == 'docs'
 Provides-Extra: mpl
 Requires-Dist: matplotlib>=3.0; extra == 'mpl'
 Requires-Dist: mplhep>=0.2.16; extra == 'mpl'
 Provides-Extra: plot
-Requires-Dist: iminuit>=2; python_version < '3.11' and extra == 'plot'
+Requires-Dist: iminuit>=2; extra == 'plot'
 Requires-Dist: matplotlib>=3.0; extra == 'plot'
 Requires-Dist: mplhep>=0.2.16; extra == 'plot'
-Requires-Dist: scipy>=1.4; python_version < '3.11' and extra == 'plot'
+Requires-Dist: scipy>=1.4; extra == 'plot'
 Provides-Extra: test
-Requires-Dist: dask-histogram>=2023.1; python_version > '3.7' and extra == 'test'
-Requires-Dist: dask[dataframe]>=2022; python_version > '3.7' and extra == 'test'
+Requires-Dist: dask-histogram>=2023.1; python_version >= '3.8' and extra == 'test'
+Requires-Dist: dask[dataframe]>=2022; python_version >= '3.8' and extra == 'test'
 Requires-Dist: pytest-mpl>=0.12; extra == 'test'
 Requires-Dist: pytest>=6; extra == 'test'
 Description-Content-Type: text/markdown
 
 <img alt="histogram" width="200" src="https://raw.githubusercontent.com/scikit-hep/hist/main/docs/_images/histlogo.png"/>
 
 # Hist
@@ -144,14 +144,16 @@
   - Histogram arguments (like `data=`) can go in the storage.
 
 - Extended Histogram features:
   - Direct support for `.name` and `.label`, like axes.
   - `.density()` computes the density as an array.
   - `.profile(remove_ax)` can convert a ND COUNT histogram into a (N-1)D MEAN histogram.
   - `.sort(axis)` supports sorting a histogram by a categorical axis. Optionally takes a function to sort by.
+  - `.fill_flattened(...)` will flatten and fill, including support for AwkwardArray.
+  - `.integrate(...)`, which takes the opposite arguments as `.project`.
 
 - Hist implements UHI+; an extension to the UHI (Unified Histogram Indexing) system designed for import-free interactivity:
   - Uses `j` suffix to switch to data coordinates in access or slices.
   - Uses `j` suffix on slices to rebin.
   - Strings can be used directly to index into string category axes.
 
 - Quick plotting routines encourage exploration:
@@ -178,29 +180,28 @@
 ## Usage
 
 ```python
 from hist import Hist
 
 # Quick construction, no other imports needed:
 h = (
-  Hist.new
-  .Reg(10, 0 ,1, name="x", label="x-axis")
-  .Var(range(10), name="y", label="y-axis")
-  .Int64()
+    Hist.new.Reg(10, 0, 1, name="x", label="x-axis")
+    .Var(range(10), name="y", label="y-axis")
+    .Int64()
 )
 
 # Filling by names is allowed:
 h.fill(y=[1, 4, 6], x=[3, 5, 2])
 
 # Names can be used to manipulate the histogram:
 h.project("x")
 h[{"y": 0.5j + 3, "x": 5j}]
 
 # You can access data coordinates or rebin with a `j` suffix:
-h[.3j:, ::2j] # x from .3 to the end, y is rebinned by 2
+h[0.3j:, ::2j]  # x from .3 to the end, y is rebinned by 2
 
 # Elegant plotting functions:
 h.plot()
 h.plot2d_full()
 h.plot_pull(Callable)
 ```
```

