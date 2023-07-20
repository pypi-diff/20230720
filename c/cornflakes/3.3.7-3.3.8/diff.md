# Comparing `tmp/cornflakes-3.3.7.tar.gz` & `tmp/cornflakes-3.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cornflakes-3.3.7.tar", max compression
+gzip compressed data, was "cornflakes-3.3.8.tar", max compression
```

## Comparing `cornflakes-3.3.7.tar` & `cornflakes-3.3.8.tar`

### file list

```diff
@@ -1,1015 +1,1025 @@
--rwxr-xr-x   0        0        0    11310 2023-07-05 20:19:15.777308 cornflakes-3.3.7/LICENSE
--rwxr-xr-x   0        0        0     4022 2023-07-05 20:19:15.777308 cornflakes-3.3.7/README.rst
--rwxr-xr-x   0        0        0     6769 2023-07-05 20:19:15.777308 cornflakes-3.3.7/build.py
--rwxr-xr-x   0        0        0     1139 2023-07-05 20:19:15.777308 cornflakes-3.3.7/cornflakes/__init__.py
--rwxr-xr-x   0        0        0      116 2023-07-05 20:19:15.777308 cornflakes-3.3.7/cornflakes/__main__.py
--rwxr-xr-x   0        0        0      251 2023-07-05 20:19:15.777308 cornflakes-3.3.7/cornflakes/builder/__init__.py
--rwxr-xr-x   0        0        0     4806 2023-07-05 20:19:15.777308 cornflakes-3.3.7/cornflakes/builder/_generate_config_module.py
--rw-r--r--   0        0        0     2575 2023-07-05 20:19:15.777308 cornflakes-3.3.7/cornflakes/builder/_generate_enum_module.py
--rw-r--r--   0        0        0     2714 2023-07-05 20:19:15.777308 cornflakes-3.3.7/cornflakes/cli/__init__.py
--rwxr-xr-x   0        0        0      541 2023-07-05 20:19:15.777308 cornflakes-3.3.7/cornflakes/common/__init__.py
--rwxr-xr-x   0        0        0     1583 2023-07-05 20:19:15.777308 cornflakes-3.3.7/cornflakes/common/_default_ca_path.py
--rwxr-xr-x   0        0        0      254 2023-07-05 20:19:15.777308 cornflakes-3.3.7/cornflakes/common/_extract_var_names.py
--rw-r--r--   0        0        0     2245 2023-07-05 20:19:15.777308 cornflakes-3.3.7/cornflakes/common/_patch_module.py
--rwxr-xr-x   0        0        0      817 2023-07-05 20:19:15.777308 cornflakes-3.3.7/cornflakes/common/_type_to_str.py
--rwxr-xr-x   0        0        0     3044 2023-07-05 20:19:15.777308 cornflakes-3.3.7/cornflakes/common/_types.py
--rwxr-xr-x   0        0        0      731 2023-07-05 20:19:15.777308 cornflakes-3.3.7/cornflakes/decorator/__init__.py
--rwxr-xr-x   0        0        0     1065 2023-07-05 20:19:15.777308 cornflakes-3.3.7/cornflakes/decorator/_add_dataclass_slots.py
--rw-r--r--   0        0        0      778 2023-07-05 20:19:15.777308 cornflakes-3.3.7/cornflakes/decorator/_funcat.py
--rw-r--r--   0        0        0     2486 2023-07-05 20:19:15.777308 cornflakes-3.3.7/cornflakes/decorator/_indexer.py
--rw-r--r--   0        0        0     5799 2023-07-05 20:19:15.777308 cornflakes-3.3.7/cornflakes/decorator/_wrap_kwargs.py
--rw-r--r--   0        0        0      395 2023-07-05 20:19:15.777308 cornflakes-3.3.7/cornflakes/decorator/_wrap_partial.py
--rwxr-xr-x   0        0        0      673 2023-07-05 20:19:15.777308 cornflakes-3.3.7/cornflakes/decorator/click/__init__.py
--rwxr-xr-x   0        0        0     3574 2023-07-05 20:19:15.777308 cornflakes-3.3.7/cornflakes/decorator/click/_click_cli.py
--rwxr-xr-x   0        0        0      450 2023-07-05 20:19:15.777308 cornflakes-3.3.7/cornflakes/decorator/click/options/__init__.py
--rwxr-xr-x   0        0        0     2896 2023-07-05 20:19:15.777308 cornflakes-3.3.7/cornflakes/decorator/click/options/_auto_option.py
--rwxr-xr-x   0        0        0     1338 2023-07-05 20:19:15.777308 cornflakes-3.3.7/cornflakes/decorator/click/options/_bg_process.py
--rwxr-xr-x   0        0        0      593 2023-07-05 20:19:15.777308 cornflakes-3.3.7/cornflakes/decorator/click/options/_global.py
--rwxr-xr-x   0        0        0      849 2023-07-05 20:19:15.777308 cornflakes-3.3.7/cornflakes/decorator/click/options/_verbose.py
--rwxr-xr-x   0        0        0     2484 2023-07-05 20:19:15.777308 cornflakes-3.3.7/cornflakes/decorator/click/rich/__init__.py
--rwxr-xr-x   0        0        0      385 2023-07-05 20:19:15.777308 cornflakes-3.3.7/cornflakes/decorator/click/rich/_rich_argument.py
--rwxr-xr-x   0        0        0    23838 2023-07-05 20:19:15.777308 cornflakes-3.3.7/cornflakes/decorator/click/rich/_rich_click.py
--rwxr-xr-x   0        0        0     1907 2023-07-05 20:19:15.777308 cornflakes-3.3.7/cornflakes/decorator/click/rich/_rich_command.py
--rwxr-xr-x   0        0        0     4907 2023-07-05 20:19:15.777308 cornflakes-3.3.7/cornflakes/decorator/click/rich/_rich_config.py
--rwxr-xr-x   0        0        0     1804 2023-07-05 20:19:15.777308 cornflakes-3.3.7/cornflakes/decorator/click/rich/_rich_global_option_wrapper.py
--rwxr-xr-x   0        0        0     3034 2023-07-05 20:19:15.777308 cornflakes-3.3.7/cornflakes/decorator/click/rich/_rich_group.py
--rwxr-xr-x   0        0        0      343 2023-07-05 20:19:15.777308 cornflakes-3.3.7/cornflakes/decorator/config/__init__.py
--rwxr-xr-x   0        0        0     3992 2023-07-05 20:19:15.777308 cornflakes-3.3.7/cornflakes/decorator/config/_config.py
--rwxr-xr-x   0        0        0     1849 2023-07-05 20:19:15.777308 cornflakes-3.3.7/cornflakes/decorator/config/_config_group.py
--rwxr-xr-x   0        0        0     7790 2023-07-05 20:19:15.777308 cornflakes-3.3.7/cornflakes/decorator/config/_load_config.py
--rwxr-xr-x   0        0        0     3094 2023-07-05 20:19:15.777308 cornflakes-3.3.7/cornflakes/decorator/config/_load_config_group.py
--rwxr-xr-x   0        0        0      360 2023-07-05 20:19:15.777308 cornflakes-3.3.7/cornflakes/decorator/config/_write_config.py
--rwxr-xr-x   0        0        0      920 2023-07-05 20:19:15.777308 cornflakes-3.3.7/cornflakes/decorator/config/dict.py
--rwxr-xr-x   0        0        0     3344 2023-07-05 20:19:15.777308 cornflakes-3.3.7/cornflakes/decorator/config/ini.py
--rwxr-xr-x   0        0        0     2170 2023-07-05 20:19:15.777308 cornflakes-3.3.7/cornflakes/decorator/config/yaml.py
--rw-r--r--   0        0        0      293 2023-07-05 20:19:15.777308 cornflakes-3.3.7/cornflakes/decorator/dataclass/__init__.py
--rwxr-xr-x   0        0        0     9156 2023-07-05 20:19:15.777308 cornflakes-3.3.7/cornflakes/decorator/dataclass/_dataclass.py
--rwxr-xr-x   0        0        0     8215 2023-07-05 20:19:15.777308 cornflakes-3.3.7/cornflakes/decorator/dataclass/_enforce_types.py
--rwxr-xr-x   0        0        0    19011 2023-07-05 20:19:15.777308 cornflakes-3.3.7/cornflakes/decorator/dataclass/_field.py
--rwxr-xr-x   0        0        0     3341 2023-07-05 20:19:15.777308 cornflakes-3.3.7/cornflakes/decorator/dataclass/helper.py
--rw-r--r--   0        0        0      141 2023-07-05 20:19:15.777308 cornflakes-3.3.7/cornflakes/decorator/dataclass/validator/__init__.py
--rw-r--r--   0        0        0    24661 2023-07-05 20:19:15.777308 cornflakes-3.3.7/cornflakes/decorator/dataclass/validator/url.py
--rw-r--r--   0        0        0      151 2023-07-05 20:19:15.777308 cornflakes-3.3.7/cornflakes/decorator/datalite/__init__.py
--rw-r--r--   0        0        0     8315 2023-07-05 20:19:15.777308 cornflakes-3.3.7/cornflakes/decorator/datalite/commons.py
--rw-r--r--   0        0        0      539 2023-07-05 20:19:15.777308 cornflakes-3.3.7/cornflakes/decorator/datalite/constraints.py
--rw-r--r--   0        0        0     3758 2023-07-05 20:19:15.777308 cornflakes-3.3.7/cornflakes/decorator/datalite/datalite_decorator.py
--rw-r--r--   0        0        0     6372 2023-07-05 20:19:15.777308 cornflakes-3.3.7/cornflakes/decorator/datalite/fetch.py
--rw-r--r--   0        0        0     4638 2023-07-05 20:19:15.777308 cornflakes-3.3.7/cornflakes/decorator/datalite/mass_actions.py
--rw-r--r--   0        0        0     6295 2023-07-05 20:19:15.777308 cornflakes-3.3.7/cornflakes/decorator/datalite/migrations.py
--rw-r--r--   0        0        0     1555 2023-07-05 20:19:15.777308 cornflakes-3.3.7/cornflakes/decorator/datalite/type_mapping.py
--rw-r--r--   0        0        0     1869 2023-07-05 20:19:15.777308 cornflakes-3.3.7/cornflakes/decorator/string_builder.py
--rwxr-xr-x   0        0        0     7901 2023-07-05 20:19:15.777308 cornflakes-3.3.7/cornflakes/decorator/types.py
--rwxr-xr-x   0        0        0      189 2023-07-05 20:19:15.777308 cornflakes-3.3.7/cornflakes/logging/__init__.py
--rwxr-xr-x   0        0        0     6489 2023-07-05 20:19:15.777308 cornflakes-3.3.7/cornflakes/logging/logger.py
--rw-r--r--   0        0        0      207 2023-07-05 20:19:15.777308 cornflakes-3.3.7/cornflakes/packaging/__init__.py
--rw-r--r--   0        0        0     2479 2023-07-05 20:19:15.777308 cornflakes-3.3.7/cornflakes/packaging/bump_version.py
--rw-r--r--   0        0        0     1940 2023-07-05 20:19:15.777308 cornflakes-3.3.7/cornflakes/packaging/update_deps.py
--rwxr-xr-x   0        0        0      110 2023-07-05 20:19:15.781308 cornflakes-3.3.7/cornflakes/parser/__init__.py
--rwxr-xr-x   0        0        0     5091 2023-07-05 20:19:15.781308 cornflakes-3.3.7/cornflakes/parser/_yaml.py
--rw-r--r--   0        0        0       57 2023-07-05 20:19:15.781308 cornflakes-3.3.7/cornflakes/py.typed
--rw-r--r--   0        0        0     6261 2023-07-05 20:19:15.781308 cornflakes-3.3.7/inst/_cornflakes/bindings.cpp
--rw-r--r--   0        0        0      422 2023-07-05 20:19:15.781308 cornflakes-3.3.7/inst/_cornflakes/bindings.hpp
--rw-r--r--   0        0        0     3914 2023-07-05 20:19:15.781308 cornflakes-3.3.7/inst/_cornflakes/cross_endian.h
--rwxr-xr-x   0        0        0   129827 2023-07-05 20:19:15.781308 cornflakes-3.3.7/inst/_cornflakes/datetime_utils.hpp
--rwxr-xr-x   0        0        0     2667 2023-07-05 20:19:15.781308 cornflakes-3.3.7/inst/_cornflakes/digest.cpp
--rw-r--r--   0        0        0      805 2023-07-05 20:19:15.781308 cornflakes-3.3.7/inst/_cornflakes/digest.hpp
--rw-r--r--   0        0        0    18739 2023-07-05 20:19:15.781308 cornflakes-3.3.7/inst/_cornflakes/ini.cpp
--rw-r--r--   0        0        0     1032 2023-07-05 20:19:15.781308 cornflakes-3.3.7/inst/_cornflakes/ini.hpp
--rw-r--r--   0        0        0    28105 2023-07-05 20:19:15.781308 cornflakes-3.3.7/inst/_cornflakes/string_operations.cpp
--rw-r--r--   0        0        0     9263 2023-07-05 20:19:15.781308 cornflakes-3.3.7/inst/_cornflakes/string_operations.hpp
--rw-r--r--   0        0        0     2831 2023-07-05 20:19:15.781308 cornflakes-3.3.7/inst/_cornflakes/system_operations.cpp
--rwxr-xr-x   0        0        0     1201 2023-07-05 20:19:15.781308 cornflakes-3.3.7/inst/_cornflakes/system_operations.hpp
--rw-r--r--   0        0        0       52 2023-07-05 20:19:16.197314 cornflakes-3.3.7/inst/ext/hash-library/.git
--rw-r--r--   0        0        0      861 2023-07-05 20:19:17.573333 cornflakes-3.3.7/inst/ext/hash-library/LICENSE
--rw-r--r--   0        0        0    29030 2023-07-05 20:19:17.573333 cornflakes-3.3.7/inst/ext/hash-library/crc32.cpp
--rw-r--r--   0        0        0     1736 2023-07-05 20:19:17.573333 cornflakes-3.3.7/inst/ext/hash-library/crc32.h
--rw-r--r--   0        0        0     3163 2023-07-05 20:19:17.573333 cornflakes-3.3.7/inst/ext/hash-library/digest.cpp
--rw-r--r--   0        0        0      723 2023-07-05 20:19:17.573333 cornflakes-3.3.7/inst/ext/hash-library/hash.h
--rw-r--r--   0        0        0     2726 2023-07-05 20:19:17.573333 cornflakes-3.3.7/inst/ext/hash-library/hmac.h
--rw-r--r--   0        0        0     8204 2023-07-05 20:19:17.573333 cornflakes-3.3.7/inst/ext/hash-library/keccak.cpp
--rw-r--r--   0        0        0     2103 2023-07-05 20:19:17.573333 cornflakes-3.3.7/inst/ext/hash-library/keccak.h
--rw-r--r--   0        0        0    10806 2023-07-05 20:19:17.573333 cornflakes-3.3.7/inst/ext/hash-library/md5.cpp
--rw-r--r--   0        0        0     1921 2023-07-05 20:19:17.573333 cornflakes-3.3.7/inst/ext/hash-library/md5.h
--rw-r--r--   0        0        0     1758 2023-07-05 20:19:17.573333 cornflakes-3.3.7/inst/ext/hash-library/readme.md
--rw-r--r--   0        0        0     8393 2023-07-05 20:19:17.573333 cornflakes-3.3.7/inst/ext/hash-library/sha1.cpp
--rw-r--r--   0        0        0     1940 2023-07-05 20:19:17.573333 cornflakes-3.3.7/inst/ext/hash-library/sha1.h
--rw-r--r--   0        0        0    14195 2023-07-05 20:19:17.573333 cornflakes-3.3.7/inst/ext/hash-library/sha256.cpp
--rw-r--r--   0        0        0     1968 2023-07-05 20:19:17.573333 cornflakes-3.3.7/inst/ext/hash-library/sha256.h
--rw-r--r--   0        0        0     8175 2023-07-05 20:19:17.573333 cornflakes-3.3.7/inst/ext/hash-library/sha3.cpp
--rw-r--r--   0        0        0     2051 2023-07-05 20:19:17.573333 cornflakes-3.3.7/inst/ext/hash-library/sha3.h
--rw-r--r--   0        0        0     1611 2023-07-05 20:19:17.573333 cornflakes-3.3.7/inst/ext/hash-library/tests/github-issue2.cpp
--rw-r--r--   0        0        0      405 2023-07-05 20:19:17.573333 cornflakes-3.3.7/inst/ext/hash-library/tests/github-issue6.cpp
--rw-r--r--   0        0        0    47981 2023-07-05 20:19:17.573333 cornflakes-3.3.7/inst/ext/hash-library/tests/tests.cpp
--rw-r--r--   0        0        0     1271 2023-07-05 20:19:18.321343 cornflakes-3.3.7/inst/ext/pybind11/.appveyor.yml
--rw-r--r--   0        0        0      996 2023-07-05 20:19:18.321343 cornflakes-3.3.7/inst/ext/pybind11/.clang-format
--rw-r--r--   0        0        0     2605 2023-07-05 20:19:18.321343 cornflakes-3.3.7/inst/ext/pybind11/.clang-tidy
--rw-r--r--   0        0        0     2196 2023-07-05 20:19:18.321343 cornflakes-3.3.7/inst/ext/pybind11/.cmake-format.yaml
--rw-r--r--   0        0        0     1308 2023-07-05 20:19:18.321343 cornflakes-3.3.7/inst/ext/pybind11/.codespell-ignore-lines
--rw-r--r--   0        0        0       48 2023-07-05 20:19:16.765322 cornflakes-3.3.7/inst/ext/pybind11/.git
--rw-r--r--   0        0        0       18 2023-07-05 20:19:18.321343 cornflakes-3.3.7/inst/ext/pybind11/.gitattributes
--rw-r--r--   0        0        0      182 2023-07-05 20:19:18.321343 cornflakes-3.3.7/inst/ext/pybind11/.github/CODEOWNERS
--rw-r--r--   0        0        0    15284 2023-07-05 20:19:18.321343 cornflakes-3.3.7/inst/ext/pybind11/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0     2561 2023-07-05 20:19:18.321343 cornflakes-3.3.7/inst/ext/pybind11/.github/ISSUE_TEMPLATE/bug-report.yml
--rw-r--r--   0        0        0      328 2023-07-05 20:19:18.321343 cornflakes-3.3.7/inst/ext/pybind11/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      162 2023-07-05 20:19:18.321343 cornflakes-3.3.7/inst/ext/pybind11/.github/dependabot.yml
--rw-r--r--   0        0        0      116 2023-07-05 20:19:18.321343 cornflakes-3.3.7/inst/ext/pybind11/.github/labeler.yml
--rw-r--r--   0        0        0       50 2023-07-05 20:19:18.321343 cornflakes-3.3.7/inst/ext/pybind11/.github/labeler_merged.yml
--rw-r--r--   0        0        0      668 2023-07-05 20:19:18.321343 cornflakes-3.3.7/inst/ext/pybind11/.github/matchers/pylint.json
--rw-r--r--   0        0        0      645 2023-07-05 20:19:18.321343 cornflakes-3.3.7/inst/ext/pybind11/.github/pull_request_template.md
--rw-r--r--   0        0        0    32023 2023-07-05 20:19:18.321343 cornflakes-3.3.7/inst/ext/pybind11/.github/workflows/ci.yml
--rw-r--r--   0        0        0     2127 2023-07-05 20:19:18.321343 cornflakes-3.3.7/inst/ext/pybind11/.github/workflows/configure.yml
--rw-r--r--   0        0        0     1460 2023-07-05 20:19:18.321343 cornflakes-3.3.7/inst/ext/pybind11/.github/workflows/format.yml
--rw-r--r--   0        0        0      559 2023-07-05 20:19:18.321343 cornflakes-3.3.7/inst/ext/pybind11/.github/workflows/labeler.yml
--rw-r--r--   0        0        0     2558 2023-07-05 20:19:18.321343 cornflakes-3.3.7/inst/ext/pybind11/.github/workflows/pip.yml
--rw-r--r--   0        0        0     2865 2023-07-05 20:19:18.321343 cornflakes-3.3.7/inst/ext/pybind11/.github/workflows/upstream.yml
--rw-r--r--   0        0        0      502 2023-07-05 20:19:18.321343 cornflakes-3.3.7/inst/ext/pybind11/.gitignore
--rw-r--r--   0        0        0     3588 2023-07-05 20:19:18.321343 cornflakes-3.3.7/inst/ext/pybind11/.pre-commit-config.yaml
--rw-r--r--   0        0        0       62 2023-07-05 20:19:18.321343 cornflakes-3.3.7/inst/ext/pybind11/.readthedocs.yml
--rw-r--r--   0        0        0    11983 2023-07-05 20:19:18.321343 cornflakes-3.3.7/inst/ext/pybind11/CMakeLists.txt
--rw-r--r--   0        0        0     1684 2023-07-05 20:19:18.321343 cornflakes-3.3.7/inst/ext/pybind11/LICENSE
--rw-r--r--   0        0        0      235 2023-07-05 20:19:18.325343 cornflakes-3.3.7/inst/ext/pybind11/MANIFEST.in
--rw-r--r--   0        0        0     7686 2023-07-05 20:19:18.325343 cornflakes-3.3.7/inst/ext/pybind11/README.rst
--rw-r--r--   0        0        0      607 2023-07-05 20:19:18.325343 cornflakes-3.3.7/inst/ext/pybind11/docs/Doxyfile
--rw-r--r--   0        0        0     7417 2023-07-05 20:19:18.325343 cornflakes-3.3.7/inst/ext/pybind11/docs/Makefile
--rw-r--r--   0        0        0       37 2023-07-05 20:19:18.325343 cornflakes-3.3.7/inst/ext/pybind11/docs/_static/css/custom.css
--rw-r--r--   0        0        0     3937 2023-07-05 20:19:18.325343 cornflakes-3.3.7/inst/ext/pybind11/docs/advanced/cast/chrono.rst
--rw-r--r--   0        0        0     3429 2023-07-05 20:19:18.325343 cornflakes-3.3.7/inst/ext/pybind11/docs/advanced/cast/custom.rst
--rw-r--r--   0        0        0    14283 2023-07-05 20:19:18.325343 cornflakes-3.3.7/inst/ext/pybind11/docs/advanced/cast/eigen.rst
--rw-r--r--   0        0        0     3889 2023-07-05 20:19:18.325343 cornflakes-3.3.7/inst/ext/pybind11/docs/advanced/cast/functional.rst
--rw-r--r--   0        0        0     1556 2023-07-05 20:19:18.325343 cornflakes-3.3.7/inst/ext/pybind11/docs/advanced/cast/index.rst
--rw-r--r--   0        0        0    12371 2023-07-05 20:19:18.325343 cornflakes-3.3.7/inst/ext/pybind11/docs/advanced/cast/overview.rst
--rw-r--r--   0        0        0     9586 2023-07-05 20:19:18.325343 cornflakes-3.3.7/inst/ext/pybind11/docs/advanced/cast/stl.rst
--rw-r--r--   0        0        0     8863 2023-07-05 20:19:18.325343 cornflakes-3.3.7/inst/ext/pybind11/docs/advanced/cast/strings.rst
--rw-r--r--   0        0        0    47796 2023-07-05 20:19:18.325343 cornflakes-3.3.7/inst/ext/pybind11/docs/advanced/classes.rst
--rw-r--r--   0        0        0     8453 2023-07-05 20:19:18.325343 cornflakes-3.3.7/inst/ext/pybind11/docs/advanced/embedding.rst
--rw-r--r--   0        0        0    17796 2023-07-05 20:19:18.325343 cornflakes-3.3.7/inst/ext/pybind11/docs/advanced/exceptions.rst
--rw-r--r--   0        0        0    26729 2023-07-05 20:19:18.325343 cornflakes-3.3.7/inst/ext/pybind11/docs/advanced/functions.rst
--rw-r--r--   0        0        0    15651 2023-07-05 20:19:18.325343 cornflakes-3.3.7/inst/ext/pybind11/docs/advanced/misc.rst
--rw-r--r--   0        0        0      278 2023-07-05 20:19:18.325343 cornflakes-3.3.7/inst/ext/pybind11/docs/advanced/pycpp/index.rst
--rw-r--r--   0        0        0    17161 2023-07-05 20:19:18.325343 cornflakes-3.3.7/inst/ext/pybind11/docs/advanced/pycpp/numpy.rst
--rw-r--r--   0        0        0     9030 2023-07-05 20:19:18.325343 cornflakes-3.3.7/inst/ext/pybind11/docs/advanced/pycpp/object.rst
--rw-r--r--   0        0        0     5710 2023-07-05 20:19:18.325343 cornflakes-3.3.7/inst/ext/pybind11/docs/advanced/pycpp/utilities.rst
--rw-r--r--   0        0        0     6377 2023-07-05 20:19:18.325343 cornflakes-3.3.7/inst/ext/pybind11/docs/advanced/smart_ptrs.rst
--rw-r--r--   0        0        0     9240 2023-07-05 20:19:18.325343 cornflakes-3.3.7/inst/ext/pybind11/docs/basics.rst
--rw-r--r--   0        0        0     2856 2023-07-05 20:19:18.325343 cornflakes-3.3.7/inst/ext/pybind11/docs/benchmark.py
--rw-r--r--   0        0        0     3168 2023-07-05 20:19:18.325343 cornflakes-3.3.7/inst/ext/pybind11/docs/benchmark.rst
--rw-r--r--   0        0        0   114174 2023-07-05 20:19:18.325343 cornflakes-3.3.7/inst/ext/pybind11/docs/changelog.rst
--rw-r--r--   0        0        0    16380 2023-07-05 20:19:18.325343 cornflakes-3.3.7/inst/ext/pybind11/docs/classes.rst
--rw-r--r--   0        0        0      273 2023-07-05 20:19:18.325343 cornflakes-3.3.7/inst/ext/pybind11/docs/cmake/index.rst
--rw-r--r--   0        0        0    25777 2023-07-05 20:19:18.325343 cornflakes-3.3.7/inst/ext/pybind11/docs/compiling.rst
--rw-r--r--   0        0        0    11574 2023-07-05 20:19:18.325343 cornflakes-3.3.7/inst/ext/pybind11/docs/conf.py
--rw-r--r--   0        0        0    13177 2023-07-05 20:19:18.325343 cornflakes-3.3.7/inst/ext/pybind11/docs/faq.rst
--rw-r--r--   0        0        0      613 2023-07-05 20:19:18.325343 cornflakes-3.3.7/inst/ext/pybind11/docs/index.rst
--rw-r--r--   0        0        0     3277 2023-07-05 20:19:18.325343 cornflakes-3.3.7/inst/ext/pybind11/docs/installing.rst
--rw-r--r--   0        0        0     3079 2023-07-05 20:19:18.325343 cornflakes-3.3.7/inst/ext/pybind11/docs/limitations.rst
--rw-r--r--   0        0        0    61034 2023-07-05 20:19:18.325343 cornflakes-3.3.7/inst/ext/pybind11/docs/pybind11-logo.png
--rw-r--r--   0        0        0    44653 2023-07-05 20:19:18.329343 cornflakes-3.3.7/inst/ext/pybind11/docs/pybind11_vs_boost_python1.png
--rw-r--r--   0        0        0    87708 2023-07-05 20:19:18.329343 cornflakes-3.3.7/inst/ext/pybind11/docs/pybind11_vs_boost_python1.svg
--rw-r--r--   0        0        0    41121 2023-07-05 20:19:18.329343 cornflakes-3.3.7/inst/ext/pybind11/docs/pybind11_vs_boost_python2.png
--rw-r--r--   0        0        0    85853 2023-07-05 20:19:18.329343 cornflakes-3.3.7/inst/ext/pybind11/docs/pybind11_vs_boost_python2.svg
--rw-r--r--   0        0        0     2647 2023-07-05 20:19:18.329343 cornflakes-3.3.7/inst/ext/pybind11/docs/reference.rst
--rw-r--r--   0        0        0     4414 2023-07-05 20:19:18.329343 cornflakes-3.3.7/inst/ext/pybind11/docs/release.rst
--rw-r--r--   0        0        0      149 2023-07-05 20:19:18.329343 cornflakes-3.3.7/inst/ext/pybind11/docs/requirements.txt
--rw-r--r--   0        0        0    23489 2023-07-05 20:19:18.329343 cornflakes-3.3.7/inst/ext/pybind11/docs/upgrade.rst
--rw-r--r--   0        0        0    23959 2023-07-05 20:19:18.329343 cornflakes-3.3.7/inst/ext/pybind11/include/pybind11/attr.h
--rw-r--r--   0        0        0     7069 2023-07-05 20:19:18.329343 cornflakes-3.3.7/inst/ext/pybind11/include/pybind11/buffer_info.h
--rw-r--r--   0        0        0    65952 2023-07-05 20:19:18.329343 cornflakes-3.3.7/inst/ext/pybind11/include/pybind11/cast.h
--rw-r--r--   0        0        0     8458 2023-07-05 20:19:18.329343 cornflakes-3.3.7/inst/ext/pybind11/include/pybind11/chrono.h
--rw-r--r--   0        0        0      120 2023-07-05 20:19:18.329343 cornflakes-3.3.7/inst/ext/pybind11/include/pybind11/common.h
--rw-r--r--   0        0        0     2096 2023-07-05 20:19:18.329343 cornflakes-3.3.7/inst/ext/pybind11/include/pybind11/complex.h
--rw-r--r--   0        0        0    28518 2023-07-05 20:19:18.329343 cornflakes-3.3.7/inst/ext/pybind11/include/pybind11/detail/class.h
--rw-r--r--   0        0        0    52990 2023-07-05 20:19:18.329343 cornflakes-3.3.7/inst/ext/pybind11/include/pybind11/detail/common.h
--rw-r--r--   0        0        0     5491 2023-07-05 20:19:18.329343 cornflakes-3.3.7/inst/ext/pybind11/include/pybind11/detail/descr.h
--rw-r--r--   0        0        0    17869 2023-07-05 20:19:18.329343 cornflakes-3.3.7/inst/ext/pybind11/include/pybind11/detail/init.h
--rw-r--r--   0        0        0    26498 2023-07-05 20:19:18.329343 cornflakes-3.3.7/inst/ext/pybind11/include/pybind11/detail/internals.h
--rw-r--r--   0        0        0    42613 2023-07-05 20:19:18.329343 cornflakes-3.3.7/inst/ext/pybind11/include/pybind11/detail/type_caster_base.h
--rw-r--r--   0        0        0     1625 2023-07-05 20:19:18.329343 cornflakes-3.3.7/inst/ext/pybind11/include/pybind11/detail/typeid.h
--rw-r--r--   0        0        0    31450 2023-07-05 20:19:18.329343 cornflakes-3.3.7/inst/ext/pybind11/include/pybind11/eigen/matrix.h
--rw-r--r--   0        0        0    18140 2023-07-05 20:19:18.333343 cornflakes-3.3.7/inst/ext/pybind11/include/pybind11/eigen/tensor.h
--rw-r--r--   0        0        0      316 2023-07-05 20:19:18.329343 cornflakes-3.3.7/inst/ext/pybind11/include/pybind11/eigen.h
--rw-r--r--   0        0        0    13475 2023-07-05 20:19:18.333343 cornflakes-3.3.7/inst/ext/pybind11/include/pybind11/embed.h
--rw-r--r--   0        0        0     4731 2023-07-05 20:19:18.333343 cornflakes-3.3.7/inst/ext/pybind11/include/pybind11/eval.h
--rw-r--r--   0        0        0     5002 2023-07-05 20:19:18.333343 cornflakes-3.3.7/inst/ext/pybind11/include/pybind11/functional.h
--rw-r--r--   0        0        0     8262 2023-07-05 20:19:18.333343 cornflakes-3.3.7/inst/ext/pybind11/include/pybind11/gil.h
--rw-r--r--   0        0        0     8862 2023-07-05 20:19:18.333343 cornflakes-3.3.7/inst/ext/pybind11/include/pybind11/iostream.h
--rw-r--r--   0        0        0    79416 2023-07-05 20:19:18.333343 cornflakes-3.3.7/inst/ext/pybind11/include/pybind11/numpy.h
--rw-r--r--   0        0        0     9103 2023-07-05 20:19:18.333343 cornflakes-3.3.7/inst/ext/pybind11/include/pybind11/operators.h
--rw-r--r--   0        0        0     2734 2023-07-05 20:19:18.333343 cornflakes-3.3.7/inst/ext/pybind11/include/pybind11/options.h
--rw-r--r--   0        0        0   126420 2023-07-05 20:19:18.333343 cornflakes-3.3.7/inst/ext/pybind11/include/pybind11/pybind11.h
--rw-r--r--   0        0        0    94641 2023-07-05 20:19:18.333343 cornflakes-3.3.7/inst/ext/pybind11/include/pybind11/pytypes.h
--rw-r--r--   0        0        0     4185 2023-07-05 20:19:18.333343 cornflakes-3.3.7/inst/ext/pybind11/include/pybind11/stl/filesystem.h
--rw-r--r--   0        0        0    15399 2023-07-05 20:19:18.333343 cornflakes-3.3.7/inst/ext/pybind11/include/pybind11/stl.h
--rw-r--r--   0        0        0    29824 2023-07-05 20:19:18.333343 cornflakes-3.3.7/inst/ext/pybind11/include/pybind11/stl_bind.h
--rw-r--r--   0        0        0     2765 2023-07-05 20:19:18.333343 cornflakes-3.3.7/inst/ext/pybind11/noxfile.py
--rw-r--r--   0        0        0      429 2023-07-05 20:19:18.333343 cornflakes-3.3.7/inst/ext/pybind11/pybind11/__init__.py
--rw-r--r--   0        0        0     1544 2023-07-05 20:19:18.333343 cornflakes-3.3.7/inst/ext/pybind11/pybind11/__main__.py
--rw-r--r--   0        0        0      233 2023-07-05 20:19:18.333343 cornflakes-3.3.7/inst/ext/pybind11/pybind11/_version.py
--rw-r--r--   0        0        0     1207 2023-07-05 20:19:18.333343 cornflakes-3.3.7/inst/ext/pybind11/pybind11/commands.py
--rw-r--r--   0        0        0        0 2023-07-05 20:19:18.333343 cornflakes-3.3.7/inst/ext/pybind11/pybind11/py.typed
--rw-r--r--   0        0        0    17631 2023-07-05 20:19:18.333343 cornflakes-3.3.7/inst/ext/pybind11/pybind11/setup_helpers.py
--rw-r--r--   0        0        0     2316 2023-07-05 20:19:18.333343 cornflakes-3.3.7/inst/ext/pybind11/pyproject.toml
--rw-r--r--   0        0        0     1452 2023-07-05 20:19:18.333343 cornflakes-3.3.7/inst/ext/pybind11/setup.cfg
--rw-r--r--   0        0        0     4877 2023-07-05 20:19:18.333343 cornflakes-3.3.7/inst/ext/pybind11/setup.py
--rw-r--r--   0        0        0    21675 2023-07-05 20:19:18.333343 cornflakes-3.3.7/inst/ext/pybind11/tests/CMakeLists.txt
--rw-r--r--   0        0        0     5625 2023-07-05 20:19:18.333343 cornflakes-3.3.7/inst/ext/pybind11/tests/conftest.py
--rw-r--r--   0        0        0    11736 2023-07-05 20:19:18.333343 cornflakes-3.3.7/inst/ext/pybind11/tests/constructor_stats.h
--rw-r--r--   0        0        0     3578 2023-07-05 20:19:18.333343 cornflakes-3.3.7/inst/ext/pybind11/tests/cross_module_gil_utils.cpp
--rw-r--r--   0        0        0     1776 2023-07-05 20:19:18.333343 cornflakes-3.3.7/inst/ext/pybind11/tests/cross_module_interleaved_error_already_set.cpp
--rw-r--r--   0        0        0      396 2023-07-05 20:19:18.333343 cornflakes-3.3.7/inst/ext/pybind11/tests/eigen_tensor_avoid_stl_array.cpp
--rw-r--r--   0        0        0      926 2023-07-05 20:19:18.333343 cornflakes-3.3.7/inst/ext/pybind11/tests/env.py
--rw-r--r--   0        0        0        0 2023-07-05 20:19:18.333343 cornflakes-3.3.7/inst/ext/pybind11/tests/extra_python_package/pytest.ini
--rw-r--r--   0        0        0     8294 2023-07-05 20:19:18.333343 cornflakes-3.3.7/inst/ext/pybind11/tests/extra_python_package/test_files.py
--rw-r--r--   0        0        0        0 2023-07-05 20:19:18.333343 cornflakes-3.3.7/inst/ext/pybind11/tests/extra_setuptools/pytest.ini
--rw-r--r--   0        0        0     4153 2023-07-05 20:19:18.337343 cornflakes-3.3.7/inst/ext/pybind11/tests/extra_setuptools/test_setuphelper.py
--rw-r--r--   0        0        0     2847 2023-07-05 20:19:18.337343 cornflakes-3.3.7/inst/ext/pybind11/tests/local_bindings.h
--rw-r--r--   0        0        0     5743 2023-07-05 20:19:18.337343 cornflakes-3.3.7/inst/ext/pybind11/tests/object.h
--rw-r--r--   0        0        0     6264 2023-07-05 20:19:18.337343 cornflakes-3.3.7/inst/ext/pybind11/tests/pybind11_cross_module_tests.cpp
--rw-r--r--   0        0        0     4517 2023-07-05 20:19:18.337343 cornflakes-3.3.7/inst/ext/pybind11/tests/pybind11_tests.cpp
--rw-r--r--   0        0        0     2685 2023-07-05 20:19:18.337343 cornflakes-3.3.7/inst/ext/pybind11/tests/pybind11_tests.h
--rw-r--r--   0        0        0      768 2023-07-05 20:19:18.337343 cornflakes-3.3.7/inst/ext/pybind11/tests/pytest.ini
--rw-r--r--   0        0        0      600 2023-07-05 20:19:18.337343 cornflakes-3.3.7/inst/ext/pybind11/tests/requirements.txt
--rw-r--r--   0        0        0      855 2023-07-05 20:19:18.337343 cornflakes-3.3.7/inst/ext/pybind11/tests/test_async.cpp
--rw-r--r--   0        0        0      536 2023-07-05 20:19:18.337343 cornflakes-3.3.7/inst/ext/pybind11/tests/test_async.py
--rw-r--r--   0        0        0     8567 2023-07-05 20:19:18.337343 cornflakes-3.3.7/inst/ext/pybind11/tests/test_buffers.cpp
--rw-r--r--   0        0        0     4848 2023-07-05 20:19:18.337343 cornflakes-3.3.7/inst/ext/pybind11/tests/test_buffers.py
--rw-r--r--   0        0        0    16025 2023-07-05 20:19:18.337343 cornflakes-3.3.7/inst/ext/pybind11/tests/test_builtin_casters.cpp
--rw-r--r--   0        0        0    17243 2023-07-05 20:19:18.337343 cornflakes-3.3.7/inst/ext/pybind11/tests/test_builtin_casters.py
--rw-r--r--   0        0        0     4118 2023-07-05 20:19:18.337343 cornflakes-3.3.7/inst/ext/pybind11/tests/test_call_policies.cpp
--rw-r--r--   0        0        0     6549 2023-07-05 20:19:18.337343 cornflakes-3.3.7/inst/ext/pybind11/tests/test_call_policies.py
--rw-r--r--   0        0        0    10858 2023-07-05 20:19:18.337343 cornflakes-3.3.7/inst/ext/pybind11/tests/test_callbacks.cpp
--rw-r--r--   0        0        0     6796 2023-07-05 20:19:18.337343 cornflakes-3.3.7/inst/ext/pybind11/tests/test_callbacks.py
--rw-r--r--   0        0        0     3370 2023-07-05 20:19:18.337343 cornflakes-3.3.7/inst/ext/pybind11/tests/test_chrono.cpp
--rw-r--r--   0        0        0     5691 2023-07-05 20:19:18.337343 cornflakes-3.3.7/inst/ext/pybind11/tests/test_chrono.py
--rw-r--r--   0        0        0    24874 2023-07-05 20:19:18.337343 cornflakes-3.3.7/inst/ext/pybind11/tests/test_class.cpp
--rw-r--r--   0        0        0    14757 2023-07-05 20:19:18.337343 cornflakes-3.3.7/inst/ext/pybind11/tests/test_class.py
--rw-r--r--   0        0        0     2639 2023-07-05 20:19:18.337343 cornflakes-3.3.7/inst/ext/pybind11/tests/test_cmake_build/CMakeLists.txt
--rw-r--r--   0        0        0      673 2023-07-05 20:19:18.337343 cornflakes-3.3.7/inst/ext/pybind11/tests/test_cmake_build/embed.cpp
--rw-r--r--   0        0        0     1171 2023-07-05 20:19:18.337343 cornflakes-3.3.7/inst/ext/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt
--rw-r--r--   0        0        0     1293 2023-07-05 20:19:18.337343 cornflakes-3.3.7/inst/ext/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt
--rw-r--r--   0        0        0     1685 2023-07-05 20:19:18.337343 cornflakes-3.3.7/inst/ext/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt
--rw-r--r--   0        0        0      152 2023-07-05 20:19:18.337343 cornflakes-3.3.7/inst/ext/pybind11/tests/test_cmake_build/main.cpp
--rw-r--r--   0        0        0     1353 2023-07-05 20:19:18.337343 cornflakes-3.3.7/inst/ext/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt
--rw-r--r--   0        0        0     1163 2023-07-05 20:19:18.337343 cornflakes-3.3.7/inst/ext/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt
--rw-r--r--   0        0        0     1368 2023-07-05 20:19:18.337343 cornflakes-3.3.7/inst/ext/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt
--rw-r--r--   0        0        0      198 2023-07-05 20:19:18.337343 cornflakes-3.3.7/inst/ext/pybind11/tests/test_cmake_build/test.py
--rw-r--r--   0        0        0     3831 2023-07-05 20:19:18.337343 cornflakes-3.3.7/inst/ext/pybind11/tests/test_const_name.cpp
--rw-r--r--   0        0        0      593 2023-07-05 20:19:18.337343 cornflakes-3.3.7/inst/ext/pybind11/tests/test_const_name.py
--rw-r--r--   0        0        0     5615 2023-07-05 20:19:18.337343 cornflakes-3.3.7/inst/ext/pybind11/tests/test_constants_and_functions.cpp
--rw-r--r--   0        0        0     1498 2023-07-05 20:19:18.337343 cornflakes-3.3.7/inst/ext/pybind11/tests/test_constants_and_functions.py
--rw-r--r--   0        0        0    10886 2023-07-05 20:19:18.337343 cornflakes-3.3.7/inst/ext/pybind11/tests/test_copy_move.cpp
--rw-r--r--   0        0        0     4796 2023-07-05 20:19:18.337343 cornflakes-3.3.7/inst/ext/pybind11/tests/test_copy_move.py
--rw-r--r--   0        0        0     7280 2023-07-05 20:19:18.337343 cornflakes-3.3.7/inst/ext/pybind11/tests/test_custom_type_casters.cpp
--rw-r--r--   0        0        0     3992 2023-07-05 20:19:18.337343 cornflakes-3.3.7/inst/ext/pybind11/tests/test_custom_type_casters.py
--rw-r--r--   0        0        0     1259 2023-07-05 20:19:18.337343 cornflakes-3.3.7/inst/ext/pybind11/tests/test_custom_type_setup.cpp
--rw-r--r--   0        0        0     1091 2023-07-05 20:19:18.337343 cornflakes-3.3.7/inst/ext/pybind11/tests/test_custom_type_setup.py
--rw-r--r--   0        0        0     4557 2023-07-05 20:19:18.337343 cornflakes-3.3.7/inst/ext/pybind11/tests/test_docstring_options.cpp
--rw-r--r--   0        0        0     2423 2023-07-05 20:19:18.337343 cornflakes-3.3.7/inst/ext/pybind11/tests/test_docstring_options.py
--rw-r--r--   0        0        0    19350 2023-07-05 20:19:18.337343 cornflakes-3.3.7/inst/ext/pybind11/tests/test_eigen_matrix.cpp
--rw-r--r--   0        0        0    29028 2023-07-05 20:19:18.337343 cornflakes-3.3.7/inst/ext/pybind11/tests/test_eigen_matrix.py
--rw-r--r--   0        0        0      473 2023-07-05 20:19:18.337343 cornflakes-3.3.7/inst/ext/pybind11/tests/test_eigen_tensor.cpp
--rw-r--r--   0        0        0    10590 2023-07-05 20:19:18.337343 cornflakes-3.3.7/inst/ext/pybind11/tests/test_eigen_tensor.inl
--rw-r--r--   0        0        0     9414 2023-07-05 20:19:18.337343 cornflakes-3.3.7/inst/ext/pybind11/tests/test_eigen_tensor.py
--rw-r--r--   0        0        0     1798 2023-07-05 20:19:18.337343 cornflakes-3.3.7/inst/ext/pybind11/tests/test_embed/CMakeLists.txt
--rw-r--r--   0        0        0     1315 2023-07-05 20:19:18.337343 cornflakes-3.3.7/inst/ext/pybind11/tests/test_embed/catch.cpp
--rw-r--r--   0        0        0      543 2023-07-05 20:19:18.337343 cornflakes-3.3.7/inst/ext/pybind11/tests/test_embed/external_module.cpp
--rw-r--r--   0        0        0    17410 2023-07-05 20:19:18.337343 cornflakes-3.3.7/inst/ext/pybind11/tests/test_embed/test_interpreter.cpp
--rw-r--r--   0        0        0      237 2023-07-05 20:19:18.337343 cornflakes-3.3.7/inst/ext/pybind11/tests/test_embed/test_interpreter.py
--rw-r--r--   0        0        0      275 2023-07-05 20:19:18.337343 cornflakes-3.3.7/inst/ext/pybind11/tests/test_embed/test_trampoline.py
--rw-r--r--   0        0        0     5722 2023-07-05 20:19:18.337343 cornflakes-3.3.7/inst/ext/pybind11/tests/test_enum.cpp
--rw-r--r--   0        0        0     8939 2023-07-05 20:19:18.337343 cornflakes-3.3.7/inst/ext/pybind11/tests/test_enum.py
--rw-r--r--   0        0        0     3168 2023-07-05 20:19:18.337343 cornflakes-3.3.7/inst/ext/pybind11/tests/test_eval.cpp
--rw-r--r--   0        0        0     1143 2023-07-05 20:19:18.337343 cornflakes-3.3.7/inst/ext/pybind11/tests/test_eval.py
--rw-r--r--   0        0        0      119 2023-07-05 20:19:18.337343 cornflakes-3.3.7/inst/ext/pybind11/tests/test_eval_call.py
--rw-r--r--   0        0        0    12082 2023-07-05 20:19:18.337343 cornflakes-3.3.7/inst/ext/pybind11/tests/test_exceptions.cpp
--rw-r--r--   0        0        0      399 2023-07-05 20:19:18.337343 cornflakes-3.3.7/inst/ext/pybind11/tests/test_exceptions.h
--rw-r--r--   0        0        0    13001 2023-07-05 20:19:18.337343 cornflakes-3.3.7/inst/ext/pybind11/tests/test_exceptions.py
--rw-r--r--   0        0        0    18155 2023-07-05 20:19:18.337343 cornflakes-3.3.7/inst/ext/pybind11/tests/test_factory_constructors.cpp
--rw-r--r--   0        0        0    16491 2023-07-05 20:19:18.337343 cornflakes-3.3.7/inst/ext/pybind11/tests/test_factory_constructors.py
--rw-r--r--   0        0        0     5311 2023-07-05 20:19:18.337343 cornflakes-3.3.7/inst/ext/pybind11/tests/test_gil_scoped.cpp
--rw-r--r--   0        0        0     8507 2023-07-05 20:19:18.337343 cornflakes-3.3.7/inst/ext/pybind11/tests/test_gil_scoped.py
--rw-r--r--   0        0        0     3960 2023-07-05 20:19:18.337343 cornflakes-3.3.7/inst/ext/pybind11/tests/test_iostream.cpp
--rw-r--r--   0        0        0     7202 2023-07-05 20:19:18.341343 cornflakes-3.3.7/inst/ext/pybind11/tests/test_iostream.py
--rw-r--r--   0        0        0     9444 2023-07-05 20:19:18.341343 cornflakes-3.3.7/inst/ext/pybind11/tests/test_kwargs_and_defaults.cpp
--rw-r--r--   0        0        0    13600 2023-07-05 20:19:18.341343 cornflakes-3.3.7/inst/ext/pybind11/tests/test_kwargs_and_defaults.py
--rw-r--r--   0        0        0     4401 2023-07-05 20:19:18.341343 cornflakes-3.3.7/inst/ext/pybind11/tests/test_local_bindings.cpp
--rw-r--r--   0        0        0     8054 2023-07-05 20:19:18.341343 cornflakes-3.3.7/inst/ext/pybind11/tests/test_local_bindings.py
--rw-r--r--   0        0        0    21388 2023-07-05 20:19:18.341343 cornflakes-3.3.7/inst/ext/pybind11/tests/test_methods_and_attributes.cpp
--rw-r--r--   0        0        0    18105 2023-07-05 20:19:18.341343 cornflakes-3.3.7/inst/ext/pybind11/tests/test_methods_and_attributes.py
--rw-r--r--   0        0        0     4121 2023-07-05 20:19:18.341343 cornflakes-3.3.7/inst/ext/pybind11/tests/test_modules.cpp
--rw-r--r--   0        0        0     3963 2023-07-05 20:19:18.341343 cornflakes-3.3.7/inst/ext/pybind11/tests/test_modules.py
--rw-r--r--   0        0        0    12305 2023-07-05 20:19:18.341343 cornflakes-3.3.7/inst/ext/pybind11/tests/test_multiple_inheritance.cpp
--rw-r--r--   0        0        0    11874 2023-07-05 20:19:18.341343 cornflakes-3.3.7/inst/ext/pybind11/tests/test_multiple_inheritance.py
--rw-r--r--   0        0        0    19861 2023-07-05 20:19:18.341343 cornflakes-3.3.7/inst/ext/pybind11/tests/test_numpy_array.cpp
--rw-r--r--   0        0        0    20414 2023-07-05 20:19:18.341343 cornflakes-3.3.7/inst/ext/pybind11/tests/test_numpy_array.py
--rw-r--r--   0        0        0    21114 2023-07-05 20:19:18.341343 cornflakes-3.3.7/inst/ext/pybind11/tests/test_numpy_dtypes.cpp
--rw-r--r--   0        0        0    14272 2023-07-05 20:19:18.341343 cornflakes-3.3.7/inst/ext/pybind11/tests/test_numpy_dtypes.py
--rw-r--r--   0        0        0     4487 2023-07-05 20:19:18.341343 cornflakes-3.3.7/inst/ext/pybind11/tests/test_numpy_vectorize.cpp
--rw-r--r--   0        0        0     9658 2023-07-05 20:19:18.341343 cornflakes-3.3.7/inst/ext/pybind11/tests/test_numpy_vectorize.py
--rw-r--r--   0        0        0     2777 2023-07-05 20:19:18.341343 cornflakes-3.3.7/inst/ext/pybind11/tests/test_opaque_types.cpp
--rw-r--r--   0        0        0     1847 2023-07-05 20:19:18.341343 cornflakes-3.3.7/inst/ext/pybind11/tests/test_opaque_types.py
--rw-r--r--   0        0        0     9132 2023-07-05 20:19:18.341343 cornflakes-3.3.7/inst/ext/pybind11/tests/test_operator_overloading.cpp
--rw-r--r--   0        0        0     4332 2023-07-05 20:19:18.341343 cornflakes-3.3.7/inst/ext/pybind11/tests/test_operator_overloading.py
--rw-r--r--   0        0        0     6719 2023-07-05 20:19:18.341343 cornflakes-3.3.7/inst/ext/pybind11/tests/test_pickling.cpp
--rw-r--r--   0        0        0     2720 2023-07-05 20:19:18.341343 cornflakes-3.3.7/inst/ext/pybind11/tests/test_pickling.py
--rw-r--r--   0        0        0    30750 2023-07-05 20:19:18.341343 cornflakes-3.3.7/inst/ext/pybind11/tests/test_pytypes.cpp
--rw-r--r--   0        0        0    23629 2023-07-05 20:19:18.341343 cornflakes-3.3.7/inst/ext/pybind11/tests/test_pytypes.py
--rw-r--r--   0        0        0    21153 2023-07-05 20:19:18.341343 cornflakes-3.3.7/inst/ext/pybind11/tests/test_sequences_and_iterators.cpp
--rw-r--r--   0        0        0     8039 2023-07-05 20:19:18.341343 cornflakes-3.3.7/inst/ext/pybind11/tests/test_sequences_and_iterators.py
--rw-r--r--   0        0        0    18898 2023-07-05 20:19:18.341343 cornflakes-3.3.7/inst/ext/pybind11/tests/test_smart_ptr.cpp
--rw-r--r--   0        0        0     9530 2023-07-05 20:19:18.341343 cornflakes-3.3.7/inst/ext/pybind11/tests/test_smart_ptr.py
--rw-r--r--   0        0        0    21587 2023-07-05 20:19:18.341343 cornflakes-3.3.7/inst/ext/pybind11/tests/test_stl.cpp
--rw-r--r--   0        0        0    12232 2023-07-05 20:19:18.341343 cornflakes-3.3.7/inst/ext/pybind11/tests/test_stl.py
--rw-r--r--   0        0        0     4622 2023-07-05 20:19:18.341343 cornflakes-3.3.7/inst/ext/pybind11/tests/test_stl_binders.cpp
--rw-r--r--   0        0        0     9138 2023-07-05 20:19:18.341343 cornflakes-3.3.7/inst/ext/pybind11/tests/test_stl_binders.py
--rw-r--r--   0        0        0     4617 2023-07-05 20:19:18.341343 cornflakes-3.3.7/inst/ext/pybind11/tests/test_tagbased_polymorphic.cpp
--rw-r--r--   0        0        0      741 2023-07-05 20:19:18.341343 cornflakes-3.3.7/inst/ext/pybind11/tests/test_tagbased_polymorphic.py
--rw-r--r--   0        0        0     1855 2023-07-05 20:19:18.341343 cornflakes-3.3.7/inst/ext/pybind11/tests/test_thread.cpp
--rw-r--r--   0        0        0      826 2023-07-05 20:19:18.341343 cornflakes-3.3.7/inst/ext/pybind11/tests/test_thread.py
--rw-r--r--   0        0        0      603 2023-07-05 20:19:18.341343 cornflakes-3.3.7/inst/ext/pybind11/tests/test_union.cpp
--rw-r--r--   0        0        0      148 2023-07-05 20:19:18.341343 cornflakes-3.3.7/inst/ext/pybind11/tests/test_union.py
--rw-r--r--   0        0        0    22991 2023-07-05 20:19:18.341343 cornflakes-3.3.7/inst/ext/pybind11/tests/test_virtual_functions.cpp
--rw-r--r--   0        0        0    12913 2023-07-05 20:19:18.341343 cornflakes-3.3.7/inst/ext/pybind11/tests/test_virtual_functions.py
--rw-r--r--   0        0        0     3226 2023-07-05 20:19:18.341343 cornflakes-3.3.7/inst/ext/pybind11/tests/valgrind-numpy-scipy.supp
--rw-r--r--   0        0        0     2657 2023-07-05 20:19:18.341343 cornflakes-3.3.7/inst/ext/pybind11/tests/valgrind-python.supp
--rw-r--r--   0        0        0     2449 2023-07-05 20:19:18.341343 cornflakes-3.3.7/inst/ext/pybind11/tools/FindCatch.cmake
--rw-r--r--   0        0        0     3105 2023-07-05 20:19:18.341343 cornflakes-3.3.7/inst/ext/pybind11/tools/FindEigen3.cmake
--rw-r--r--   0        0        0    11190 2023-07-05 20:19:18.341343 cornflakes-3.3.7/inst/ext/pybind11/tools/FindPythonLibsNew.cmake
--rw-r--r--   0        0        0      817 2023-07-05 20:19:18.341343 cornflakes-3.3.7/inst/ext/pybind11/tools/JoinPaths.cmake
--rwxr-xr-x   0        0        0     1423 2023-07-05 20:19:18.341343 cornflakes-3.3.7/inst/ext/pybind11/tools/check-style.sh
--rw-r--r--   0        0        0      952 2023-07-05 20:19:18.341343 cornflakes-3.3.7/inst/ext/pybind11/tools/cmake_uninstall.cmake.in
--rw-r--r--   0        0        0     1117 2023-07-05 20:19:18.341343 cornflakes-3.3.7/inst/ext/pybind11/tools/codespell_ignore_lines_from_errors.py
--rw-r--r--   0        0        0     1031 2023-07-05 20:19:18.341343 cornflakes-3.3.7/inst/ext/pybind11/tools/libsize.py
--rwxr-xr-x   0        0        0     1311 2023-07-05 20:19:18.341343 cornflakes-3.3.7/inst/ext/pybind11/tools/make_changelog.py
--rw-r--r--   0        0        0      196 2023-07-05 20:19:18.341343 cornflakes-3.3.7/inst/ext/pybind11/tools/pybind11.pc.in
--rw-r--r--   0        0        0    14033 2023-07-05 20:19:18.345343 cornflakes-3.3.7/inst/ext/pybind11/tools/pybind11Common.cmake
--rw-r--r--   0        0        0     6930 2023-07-05 20:19:18.345343 cornflakes-3.3.7/inst/ext/pybind11/tools/pybind11Config.cmake.in
--rw-r--r--   0        0        0     8960 2023-07-05 20:19:18.345343 cornflakes-3.3.7/inst/ext/pybind11/tools/pybind11NewTools.cmake
--rw-r--r--   0        0        0     8361 2023-07-05 20:19:18.345343 cornflakes-3.3.7/inst/ext/pybind11/tools/pybind11Tools.cmake
--rw-r--r--   0        0        0       94 2023-07-05 20:19:18.345343 cornflakes-3.3.7/inst/ext/pybind11/tools/pyproject.toml
--rw-r--r--   0        0        0     2104 2023-07-05 20:19:18.345343 cornflakes-3.3.7/inst/ext/pybind11/tools/setup_global.py.in
--rw-r--r--   0        0        0     1234 2023-07-05 20:19:18.345343 cornflakes-3.3.7/inst/ext/pybind11/tools/setup_main.py.in
--rw-r--r--   0        0        0       49 2023-07-05 20:19:17.249328 cornflakes-3.3.7/inst/ext/rapidjson/.git
--rw-r--r--   0        0        0      450 2023-07-05 20:19:19.025352 cornflakes-3.3.7/inst/ext/rapidjson/.gitattributes
--rw-r--r--   0        0        0      404 2023-07-05 20:19:19.029353 cornflakes-3.3.7/inst/ext/rapidjson/.gitignore
--rw-r--r--   0        0        0      104 2023-07-05 20:19:19.029353 cornflakes-3.3.7/inst/ext/rapidjson/.gitmodules
--rw-r--r--   0        0        0     6312 2023-07-05 20:19:19.029353 cornflakes-3.3.7/inst/ext/rapidjson/.travis.yml
--rw-r--r--   0        0        0     6818 2023-07-05 20:19:19.029353 cornflakes-3.3.7/inst/ext/rapidjson/CHANGELOG.md
--rw-r--r--   0        0        0    10429 2023-07-05 20:19:19.029353 cornflakes-3.3.7/inst/ext/rapidjson/CMakeLists.txt
--rw-r--r--   0        0        0      828 2023-07-05 20:19:19.029353 cornflakes-3.3.7/inst/ext/rapidjson/CMakeModules/FindGTestSrc.cmake
--rw-r--r--   0        0        0      229 2023-07-05 20:19:19.029353 cornflakes-3.3.7/inst/ext/rapidjson/RapidJSON.pc.in
--rw-r--r--   0        0        0      983 2023-07-05 20:19:19.029353 cornflakes-3.3.7/inst/ext/rapidjson/RapidJSONConfig.cmake.in
--rw-r--r--   0        0        0      469 2023-07-05 20:19:19.029353 cornflakes-3.3.7/inst/ext/rapidjson/RapidJSONConfigVersion.cmake.in
--rw-r--r--   0        0        0     2662 2023-07-05 20:19:19.029353 cornflakes-3.3.7/inst/ext/rapidjson/appveyor.yml
--rw-r--r--   0        0        0        5 2023-07-05 20:19:19.029353 cornflakes-3.3.7/inst/ext/rapidjson/bin/data/abcde.txt
--rw-r--r--   0        0        0      603 2023-07-05 20:19:19.029353 cornflakes-3.3.7/inst/ext/rapidjson/bin/data/glossary.json
--rw-r--r--   0        0        0      898 2023-07-05 20:19:19.029353 cornflakes-3.3.7/inst/ext/rapidjson/bin/data/menu.json
--rw-r--r--   0        0        0      103 2023-07-05 20:19:19.029353 cornflakes-3.3.7/inst/ext/rapidjson/bin/data/readme.txt
--rw-r--r--   0        0        0   687491 2023-07-05 20:19:19.029353 cornflakes-3.3.7/inst/ext/rapidjson/bin/data/sample.json
--rw-r--r--   0        0        0     3554 2023-07-05 20:19:19.029353 cornflakes-3.3.7/inst/ext/rapidjson/bin/data/webapp.json
--rw-r--r--   0        0        0      626 2023-07-05 20:19:19.029353 cornflakes-3.3.7/inst/ext/rapidjson/bin/data/widget.json
--rw-r--r--   0        0        0     4375 2023-07-05 20:19:19.029353 cornflakes-3.3.7/inst/ext/rapidjson/bin/draft-04/schema
--rw-r--r--   0        0        0      368 2023-07-05 20:19:19.029353 cornflakes-3.3.7/inst/ext/rapidjson/bin/encodings/utf16be.json
--rw-r--r--   0        0        0      370 2023-07-05 20:19:19.029353 cornflakes-3.3.7/inst/ext/rapidjson/bin/encodings/utf16bebom.json
--rw-r--r--   0        0        0      368 2023-07-05 20:19:19.029353 cornflakes-3.3.7/inst/ext/rapidjson/bin/encodings/utf16le.json
--rw-r--r--   0        0        0      370 2023-07-05 20:19:19.029353 cornflakes-3.3.7/inst/ext/rapidjson/bin/encodings/utf16lebom.json
--rw-r--r--   0        0        0      736 2023-07-05 20:19:19.029353 cornflakes-3.3.7/inst/ext/rapidjson/bin/encodings/utf32be.json
--rw-r--r--   0        0        0      740 2023-07-05 20:19:19.029353 cornflakes-3.3.7/inst/ext/rapidjson/bin/encodings/utf32bebom.json
--rw-r--r--   0        0        0      736 2023-07-05 20:19:19.029353 cornflakes-3.3.7/inst/ext/rapidjson/bin/encodings/utf32le.json
--rw-r--r--   0        0        0      740 2023-07-05 20:19:19.029353 cornflakes-3.3.7/inst/ext/rapidjson/bin/encodings/utf32lebom.json
--rw-r--r--   0        0        0      322 2023-07-05 20:19:19.029353 cornflakes-3.3.7/inst/ext/rapidjson/bin/encodings/utf8.json
--rw-r--r--   0        0        0      325 2023-07-05 20:19:19.029353 cornflakes-3.3.7/inst/ext/rapidjson/bin/encodings/utf8bom.json
--rw-r--r--   0        0        0       60 2023-07-05 20:19:19.029353 cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonchecker/fail1.json
--rw-r--r--   0        0        0       58 2023-07-05 20:19:19.029353 cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonchecker/fail10.json
--rw-r--r--   0        0        0       29 2023-07-05 20:19:19.029353 cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonchecker/fail11.json
--rw-r--r--   0        0        0       31 2023-07-05 20:19:19.029353 cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonchecker/fail12.json
--rw-r--r--   0        0        0       43 2023-07-05 20:19:19.029353 cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonchecker/fail13.json
--rw-r--r--   0        0        0       31 2023-07-05 20:19:19.029353 cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonchecker/fail14.json
--rw-r--r--   0        0        0       34 2023-07-05 20:19:19.029353 cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonchecker/fail15.json
--rw-r--r--   0        0        0        8 2023-07-05 20:19:19.029353 cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonchecker/fail16.json
--rw-r--r--   0        0        0       34 2023-07-05 20:19:19.029353 cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonchecker/fail17.json
--rw-r--r--   0        0        0       50 2023-07-05 20:19:19.029353 cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonchecker/fail18.json
--rw-r--r--   0        0        0       22 2023-07-05 20:19:19.029353 cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonchecker/fail19.json
--rw-r--r--   0        0        0       17 2023-07-05 20:19:19.029353 cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonchecker/fail2.json
--rw-r--r--   0        0        0       23 2023-07-05 20:19:19.029353 cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonchecker/fail20.json
--rw-r--r--   0        0        0       32 2023-07-05 20:19:19.029353 cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonchecker/fail21.json
--rw-r--r--   0        0        0       33 2023-07-05 20:19:19.029353 cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonchecker/fail22.json
--rw-r--r--   0        0        0       20 2023-07-05 20:19:19.029353 cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonchecker/fail23.json
--rw-r--r--   0        0        0       16 2023-07-05 20:19:19.029353 cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonchecker/fail24.json
--rw-r--r--   0        0        0       29 2023-07-05 20:19:19.029353 cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonchecker/fail25.json
--rw-r--r--   0        0        0       38 2023-07-05 20:19:19.029353 cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonchecker/fail26.json
--rw-r--r--   0        0        0       14 2023-07-05 20:19:19.029353 cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonchecker/fail27.json
--rw-r--r--   0        0        0       15 2023-07-05 20:19:19.029353 cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonchecker/fail28.json
--rw-r--r--   0        0        0        4 2023-07-05 20:19:19.029353 cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonchecker/fail29.json
--rw-r--r--   0        0        0       37 2023-07-05 20:19:19.029353 cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonchecker/fail3.json
--rw-r--r--   0        0        0        5 2023-07-05 20:19:19.029353 cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonchecker/fail30.json
--rw-r--r--   0        0        0        7 2023-07-05 20:19:19.029353 cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonchecker/fail31.json
--rw-r--r--   0        0        0       40 2023-07-05 20:19:19.033352 cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonchecker/fail32.json
--rw-r--r--   0        0        0       12 2023-07-05 20:19:19.033352 cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonchecker/fail33.json
--rw-r--r--   0        0        0       16 2023-07-05 20:19:19.033352 cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonchecker/fail4.json
--rw-r--r--   0        0        0       24 2023-07-05 20:19:19.033352 cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonchecker/fail5.json
--rw-r--r--   0        0        0       26 2023-07-05 20:19:19.033352 cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonchecker/fail6.json
--rw-r--r--   0        0        0       26 2023-07-05 20:19:19.033352 cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonchecker/fail7.json
--rw-r--r--   0        0        0       16 2023-07-05 20:19:19.033352 cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonchecker/fail8.json
--rw-r--r--   0        0        0       22 2023-07-05 20:19:19.033352 cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonchecker/fail9.json
--rw-r--r--   0        0        0     1441 2023-07-05 20:19:19.033352 cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonchecker/pass1.json
--rw-r--r--   0        0        0       52 2023-07-05 20:19:19.033352 cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonchecker/pass2.json
--rw-r--r--   0        0        0      148 2023-07-05 20:19:19.033352 cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonchecker/pass3.json
--rw-r--r--   0        0        0      173 2023-07-05 20:19:19.033352 cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonchecker/readme.txt
--rw-r--r--   0        0        0        5 2023-07-05 20:19:19.033352 cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonschema/.gitignore
--rw-r--r--   0        0        0       98 2023-07-05 20:19:19.033352 cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonschema/.travis.yml
--rw-r--r--   0        0        0     1057 2023-07-05 20:19:19.033352 cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonschema/LICENSE
--rw-r--r--   0        0        0     4787 2023-07-05 20:19:19.033352 cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonschema/README.md
--rwxr-xr-x   0        0        0     9059 2023-07-05 20:19:19.033352 cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonschema/bin/jsonschema_suite
--rw-r--r--   0        0        0       25 2023-07-05 20:19:19.033352 cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonschema/remotes/folder/folderInteger.json
--rw-r--r--   0        0        0       25 2023-07-05 20:19:19.033352 cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonschema/remotes/integer.json
--rw-r--r--   0        0        0      110 2023-07-05 20:19:19.033352 cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonschema/remotes/subSchemas.json
--rw-r--r--   0        0        0     2257 2023-07-05 20:19:19.033352 cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonschema/tests/draft3/additionalItems.json
--rw-r--r--   0        0        0     2745 2023-07-05 20:19:19.033352 cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonschema/tests/draft3/additionalProperties.json
--rw-r--r--   0        0        0     1273 2023-07-05 20:19:19.033352 cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonschema/tests/draft3/default.json
--rw-r--r--   0        0        0     2989 2023-07-05 20:19:19.033352 cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonschema/tests/draft3/dependencies.json
--rw-r--r--   0        0        0     1936 2023-07-05 20:19:19.033352 cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonschema/tests/draft3/disallow.json
--rw-r--r--   0        0        0     1544 2023-07-05 20:19:19.033352 cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonschema/tests/draft3/divisibleBy.json
--rw-r--r--   0        0        0     1964 2023-07-05 20:19:19.033352 cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonschema/tests/draft3/enum.json
--rw-r--r--   0        0        0     2591 2023-07-05 20:19:19.033352 cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonschema/tests/draft3/extends.json
--rw-r--r--   0        0        0     1136 2023-07-05 20:19:19.033352 cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonschema/tests/draft3/items.json
--rw-r--r--   0        0        0      706 2023-07-05 20:19:19.033352 cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonschema/tests/draft3/maxItems.json
--rw-r--r--   0        0        0      895 2023-07-05 20:19:19.033352 cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonschema/tests/draft3/maxLength.json
--rw-r--r--   0        0        0     1063 2023-07-05 20:19:19.033352 cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonschema/tests/draft3/maximum.json
--rw-r--r--   0        0        0      693 2023-07-05 20:19:19.033352 cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonschema/tests/draft3/minItems.json
--rw-r--r--   0        0        0      886 2023-07-05 20:19:19.033352 cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonschema/tests/draft3/minLength.json
--rw-r--r--   0        0        0     1063 2023-07-05 20:19:19.033352 cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonschema/tests/draft3/minimum.json
--rw-r--r--   0        0        0     3075 2023-07-05 20:19:19.033352 cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonschema/tests/draft3/optional/bignum.json
--rw-r--r--   0        0        0     6751 2023-07-05 20:19:19.033352 cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonschema/tests/draft3/optional/format.json
--rw-r--r--   0        0        0      463 2023-07-05 20:19:19.033352 cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonschema/tests/draft3/optional/jsregex.json
--rw-r--r--   0        0        0      384 2023-07-05 20:19:19.033352 cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonschema/tests/draft3/optional/zeroTerminatedFloats.json
--rw-r--r--   0        0        0      857 2023-07-05 20:19:19.033352 cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonschema/tests/draft3/pattern.json
--rw-r--r--   0        0        0     3365 2023-07-05 20:19:19.033352 cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonschema/tests/draft3/patternProperties.json
--rw-r--r--   0        0        0     2881 2023-07-05 20:19:19.033352 cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonschema/tests/draft3/properties.json
--rw-r--r--   0        0        0     4385 2023-07-05 20:19:19.033352 cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonschema/tests/draft3/ref.json
--rw-r--r--   0        0        0     1961 2023-07-05 20:19:19.033352 cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonschema/tests/draft3/refRemote.json
--rw-r--r--   0        0        0     1282 2023-07-05 20:19:19.033352 cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonschema/tests/draft3/required.json
--rw-r--r--   0        0        0    13217 2023-07-05 20:19:19.033352 cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonschema/tests/draft3/type.json
--rw-r--r--   0        0        0     2613 2023-07-05 20:19:19.033352 cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonschema/tests/draft3/uniqueItems.json
--rw-r--r--   0        0        0     2282 2023-07-05 20:19:19.033352 cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonschema/tests/draft4/additionalItems.json
--rw-r--r--   0        0        0     2745 2023-07-05 20:19:19.033352 cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonschema/tests/draft4/additionalProperties.json
--rw-r--r--   0        0        0     3025 2023-07-05 20:19:19.033352 cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonschema/tests/draft4/allOf.json
--rw-r--r--   0        0        0     1608 2023-07-05 20:19:19.033352 cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonschema/tests/draft4/anyOf.json
--rw-r--r--   0        0        0     1273 2023-07-05 20:19:19.033352 cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonschema/tests/draft4/default.json
--rw-r--r--   0        0        0      854 2023-07-05 20:19:19.033352 cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonschema/tests/draft4/definitions.json
--rw-r--r--   0        0        0     3139 2023-07-05 20:19:19.033352 cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonschema/tests/draft4/dependencies.json
--rw-r--r--   0        0        0     1975 2023-07-05 20:19:19.033352 cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonschema/tests/draft4/enum.json
--rw-r--r--   0        0        0     1136 2023-07-05 20:19:19.033352 cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonschema/tests/draft4/items.json
--rw-r--r--   0        0        0      706 2023-07-05 20:19:19.033352 cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonschema/tests/draft4/maxItems.json
--rw-r--r--   0        0        0      896 2023-07-05 20:19:19.033352 cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonschema/tests/draft4/maxLength.json
--rw-r--r--   0        0        0      759 2023-07-05 20:19:19.033352 cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonschema/tests/draft4/maxProperties.json
--rw-r--r--   0        0        0     1063 2023-07-05 20:19:19.033352 cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonschema/tests/draft4/maximum.json
--rw-r--r--   0        0        0      693 2023-07-05 20:19:19.033352 cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonschema/tests/draft4/minItems.json
--rw-r--r--   0        0        0      886 2023-07-05 20:19:19.033352 cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonschema/tests/draft4/minLength.json
--rw-r--r--   0        0        0      725 2023-07-05 20:19:19.033352 cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonschema/tests/draft4/minProperties.json
--rw-r--r--   0        0        0     1063 2023-07-05 20:19:19.033352 cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonschema/tests/draft4/minimum.json
--rw-r--r--   0        0        0     1525 2023-07-05 20:19:19.033352 cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonschema/tests/draft4/multipleOf.json
--rw-r--r--   0        0        0     2266 2023-07-05 20:19:19.033352 cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonschema/tests/draft4/not.json
--rw-r--r--   0        0        0     1607 2023-07-05 20:19:19.033352 cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonschema/tests/draft4/oneOf.json
--rw-r--r--   0        0        0     3075 2023-07-05 20:19:19.033352 cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonschema/tests/draft4/optional/bignum.json
--rw-r--r--   0        0        0     4608 2023-07-05 20:19:19.033352 cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonschema/tests/draft4/optional/format.json
--rw-r--r--   0        0        0      384 2023-07-05 20:19:19.033352 cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonschema/tests/draft4/optional/zeroTerminatedFloats.json
--rw-r--r--   0        0        0      857 2023-07-05 20:19:19.033352 cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonschema/tests/draft4/pattern.json
--rw-r--r--   0        0        0     3365 2023-07-05 20:19:19.033352 cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonschema/tests/draft4/patternProperties.json
--rw-r--r--   0        0        0     2881 2023-07-05 20:19:19.033352 cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonschema/tests/draft4/properties.json
--rw-r--r--   0        0        0     4366 2023-07-05 20:19:19.033352 cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonschema/tests/draft4/ref.json
--rw-r--r--   0        0        0     1961 2023-07-05 20:19:19.033352 cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonschema/tests/draft4/refRemote.json
--rw-r--r--   0        0        0      923 2023-07-05 20:19:19.033352 cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonschema/tests/draft4/required.json
--rw-r--r--   0        0        0     9298 2023-07-05 20:19:19.033352 cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonschema/tests/draft4/type.json
--rw-r--r--   0        0        0     2613 2023-07-05 20:19:19.033352 cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonschema/tests/draft4/uniqueItems.json
--rw-r--r--   0        0        0      134 2023-07-05 20:19:19.033352 cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonschema/tox.ini
--rw-r--r--   0        0        0    30003 2023-07-05 20:19:19.033352 cornflakes-3.3.7/inst/ext/rapidjson/bin/types/alotofkeys.json
--rw-r--r--   0        0        0      849 2023-07-05 20:19:19.033352 cornflakes-3.3.7/inst/ext/rapidjson/bin/types/booleans.json
--rw-r--r--   0        0        0     1698 2023-07-05 20:19:19.033352 cornflakes-3.3.7/inst/ext/rapidjson/bin/types/floats.json
--rw-r--r--   0        0        0     4202 2023-07-05 20:19:19.033352 cornflakes-3.3.7/inst/ext/rapidjson/bin/types/guids.json
--rw-r--r--   0        0        0     1098 2023-07-05 20:19:19.033352 cornflakes-3.3.7/inst/ext/rapidjson/bin/types/integers.json
--rw-r--r--   0        0        0    15142 2023-07-05 20:19:19.033352 cornflakes-3.3.7/inst/ext/rapidjson/bin/types/mixed.json
--rw-r--r--   0        0        0      802 2023-07-05 20:19:19.033352 cornflakes-3.3.7/inst/ext/rapidjson/bin/types/nulls.json
--rw-r--r--   0        0        0    33764 2023-07-05 20:19:19.033352 cornflakes-3.3.7/inst/ext/rapidjson/bin/types/paragraphs.json
--rw-r--r--   0        0        0       86 2023-07-05 20:19:19.033352 cornflakes-3.3.7/inst/ext/rapidjson/bin/types/readme.txt
--rw-r--r--   0        0        0     3150 2023-07-05 20:19:19.033352 cornflakes-3.3.7/inst/ext/rapidjson/bin/unittestschema/address.json
--rw-r--r--   0        0        0       84 2023-07-05 20:19:19.033352 cornflakes-3.3.7/inst/ext/rapidjson/bin/unittestschema/allOf_address.json
--rw-r--r--   0        0        0       84 2023-07-05 20:19:19.033352 cornflakes-3.3.7/inst/ext/rapidjson/bin/unittestschema/anyOf_address.json
--rw-r--r--   0        0        0     1315 2023-07-05 20:19:19.033352 cornflakes-3.3.7/inst/ext/rapidjson/bin/unittestschema/idandref.json
--rw-r--r--   0        0        0       84 2023-07-05 20:19:19.033352 cornflakes-3.3.7/inst/ext/rapidjson/bin/unittestschema/oneOf_address.json
--rw-r--r--   0        0        0     2175 2023-07-05 20:19:19.033352 cornflakes-3.3.7/inst/ext/rapidjson/contrib/natvis/LICENSE
--rw-r--r--   0        0        0      678 2023-07-05 20:19:19.033352 cornflakes-3.3.7/inst/ext/rapidjson/contrib/natvis/README.md
--rw-r--r--   0        0        0     2729 2023-07-05 20:19:19.033352 cornflakes-3.3.7/inst/ext/rapidjson/contrib/natvis/rapidjson.natvis
--rw-r--r--   0        0        0     1052 2023-07-05 20:19:19.033352 cornflakes-3.3.7/inst/ext/rapidjson/doc/CMakeLists.txt
--rw-r--r--   0        0        0   103393 2023-07-05 20:19:19.037353 cornflakes-3.3.7/inst/ext/rapidjson/doc/Doxyfile.in
--rw-r--r--   0        0        0   103478 2023-07-05 20:19:19.037353 cornflakes-3.3.7/inst/ext/rapidjson/doc/Doxyfile.zh-cn.in
--rw-r--r--   0        0        0      912 2023-07-05 20:19:19.037353 cornflakes-3.3.7/inst/ext/rapidjson/doc/diagram/architecture.dot
--rw-r--r--   0        0        0    16569 2023-07-05 20:19:19.037353 cornflakes-3.3.7/inst/ext/rapidjson/doc/diagram/architecture.png
--rw-r--r--   0        0        0     2239 2023-07-05 20:19:19.037353 cornflakes-3.3.7/inst/ext/rapidjson/doc/diagram/insituparsing.dot
--rw-r--r--   0        0        0    37281 2023-07-05 20:19:19.037353 cornflakes-3.3.7/inst/ext/rapidjson/doc/diagram/insituparsing.png
--rw-r--r--   0        0        0     1915 2023-07-05 20:19:19.037353 cornflakes-3.3.7/inst/ext/rapidjson/doc/diagram/iterative-parser-states-diagram.dot
--rw-r--r--   0        0        0    92378 2023-07-05 20:19:19.037353 cornflakes-3.3.7/inst/ext/rapidjson/doc/diagram/iterative-parser-states-diagram.png
--rw-r--r--   0        0        0      176 2023-07-05 20:19:19.037353 cornflakes-3.3.7/inst/ext/rapidjson/doc/diagram/makefile
--rw-r--r--   0        0        0      935 2023-07-05 20:19:19.037353 cornflakes-3.3.7/inst/ext/rapidjson/doc/diagram/move1.dot
--rw-r--r--   0        0        0    16081 2023-07-05 20:19:19.037353 cornflakes-3.3.7/inst/ext/rapidjson/doc/diagram/move1.png
--rw-r--r--   0        0        0     1502 2023-07-05 20:19:19.037353 cornflakes-3.3.7/inst/ext/rapidjson/doc/diagram/move2.dot
--rw-r--r--   0        0        0    41517 2023-07-05 20:19:19.037353 cornflakes-3.3.7/inst/ext/rapidjson/doc/diagram/move2.png
--rw-r--r--   0        0        0     1454 2023-07-05 20:19:19.037353 cornflakes-3.3.7/inst/ext/rapidjson/doc/diagram/move3.dot
--rw-r--r--   0        0        0    36371 2023-07-05 20:19:19.037353 cornflakes-3.3.7/inst/ext/rapidjson/doc/diagram/move3.png
--rw-r--r--   0        0        0     1427 2023-07-05 20:19:19.037353 cornflakes-3.3.7/inst/ext/rapidjson/doc/diagram/normalparsing.dot
--rw-r--r--   0        0        0    32887 2023-07-05 20:19:19.037353 cornflakes-3.3.7/inst/ext/rapidjson/doc/diagram/normalparsing.png
--rw-r--r--   0        0        0     1435 2023-07-05 20:19:19.037353 cornflakes-3.3.7/inst/ext/rapidjson/doc/diagram/simpledom.dot
--rw-r--r--   0        0        0    43670 2023-07-05 20:19:19.037353 cornflakes-3.3.7/inst/ext/rapidjson/doc/diagram/simpledom.png
--rw-r--r--   0        0        0     1456 2023-07-05 20:19:19.037353 cornflakes-3.3.7/inst/ext/rapidjson/doc/diagram/tutorial.dot
--rw-r--r--   0        0        0    44634 2023-07-05 20:19:19.037353 cornflakes-3.3.7/inst/ext/rapidjson/doc/diagram/tutorial.png
--rw-r--r--   0        0        0     1775 2023-07-05 20:19:19.037353 cornflakes-3.3.7/inst/ext/rapidjson/doc/diagram/utilityclass.dot
--rw-r--r--   0        0        0    99993 2023-07-05 20:19:19.037353 cornflakes-3.3.7/inst/ext/rapidjson/doc/diagram/utilityclass.png
--rw-r--r--   0        0        0    15464 2023-07-05 20:19:19.037353 cornflakes-3.3.7/inst/ext/rapidjson/doc/dom.md
--rw-r--r--   0        0        0    15393 2023-07-05 20:19:19.037353 cornflakes-3.3.7/inst/ext/rapidjson/doc/dom.zh-cn.md
--rw-r--r--   0        0        0     6708 2023-07-05 20:19:19.037353 cornflakes-3.3.7/inst/ext/rapidjson/doc/encoding.md
--rw-r--r--   0        0        0     6860 2023-07-05 20:19:19.037353 cornflakes-3.3.7/inst/ext/rapidjson/doc/encoding.zh-cn.md
--rw-r--r--   0        0        0    15364 2023-07-05 20:19:19.037353 cornflakes-3.3.7/inst/ext/rapidjson/doc/faq.md
--rw-r--r--   0        0        0    15030 2023-07-05 20:19:19.041353 cornflakes-3.3.7/inst/ext/rapidjson/doc/faq.zh-cn.md
--rw-r--r--   0        0        0     5063 2023-07-05 20:19:19.041353 cornflakes-3.3.7/inst/ext/rapidjson/doc/features.md
--rw-r--r--   0        0        0     4805 2023-07-05 20:19:19.041353 cornflakes-3.3.7/inst/ext/rapidjson/doc/features.zh-cn.md
--rw-r--r--   0        0        0    22426 2023-07-05 20:19:19.041353 cornflakes-3.3.7/inst/ext/rapidjson/doc/internals.md
--rw-r--r--   0        0        0    21956 2023-07-05 20:19:19.041353 cornflakes-3.3.7/inst/ext/rapidjson/doc/internals.zh-cn.md
--rw-r--r--   0        0        0     5259 2023-07-05 20:19:19.041353 cornflakes-3.3.7/inst/ext/rapidjson/doc/logo/rapidjson.png
--rw-r--r--   0        0        0     4230 2023-07-05 20:19:19.041353 cornflakes-3.3.7/inst/ext/rapidjson/doc/logo/rapidjson.svg
--rw-r--r--   0        0        0     6090 2023-07-05 20:19:19.041353 cornflakes-3.3.7/inst/ext/rapidjson/doc/misc/DoxygenLayout.xml
--rw-r--r--   0        0        0     6572 2023-07-05 20:19:19.041353 cornflakes-3.3.7/inst/ext/rapidjson/doc/misc/doxygenextra.css
--rw-r--r--   0        0        0      256 2023-07-05 20:19:19.041353 cornflakes-3.3.7/inst/ext/rapidjson/doc/misc/footer.html
--rw-r--r--   0        0        0     1137 2023-07-05 20:19:19.041353 cornflakes-3.3.7/inst/ext/rapidjson/doc/misc/header.html
--rw-r--r--   0        0        0      363 2023-07-05 20:19:19.041353 cornflakes-3.3.7/inst/ext/rapidjson/doc/npm.md
--rw-r--r--   0        0        0     1268 2023-07-05 20:19:19.041353 cornflakes-3.3.7/inst/ext/rapidjson/doc/performance.md
--rw-r--r--   0        0        0     1236 2023-07-05 20:19:19.041353 cornflakes-3.3.7/inst/ext/rapidjson/doc/performance.zh-cn.md
--rw-r--r--   0        0        0     8883 2023-07-05 20:19:19.041353 cornflakes-3.3.7/inst/ext/rapidjson/doc/pointer.md
--rw-r--r--   0        0        0     8532 2023-07-05 20:19:19.041353 cornflakes-3.3.7/inst/ext/rapidjson/doc/pointer.zh-cn.md
--rw-r--r--   0        0        0    21276 2023-07-05 20:19:19.041353 cornflakes-3.3.7/inst/ext/rapidjson/doc/sax.md
--rw-r--r--   0        0        0    19967 2023-07-05 20:19:19.041353 cornflakes-3.3.7/inst/ext/rapidjson/doc/sax.zh-cn.md
--rw-r--r--   0        0        0    18222 2023-07-05 20:19:19.041353 cornflakes-3.3.7/inst/ext/rapidjson/doc/schema.md
--rw-r--r--   0        0        0     9765 2023-07-05 20:19:19.041353 cornflakes-3.3.7/inst/ext/rapidjson/doc/schema.zh-cn.md
--rw-r--r--   0        0        0    14531 2023-07-05 20:19:19.041353 cornflakes-3.3.7/inst/ext/rapidjson/doc/stream.md
--rw-r--r--   0        0        0    14325 2023-07-05 20:19:19.041353 cornflakes-3.3.7/inst/ext/rapidjson/doc/stream.zh-cn.md
--rw-r--r--   0        0        0    22121 2023-07-05 20:19:19.041353 cornflakes-3.3.7/inst/ext/rapidjson/doc/tutorial.md
--rw-r--r--   0        0        0    21546 2023-07-05 20:19:19.041353 cornflakes-3.3.7/inst/ext/rapidjson/doc/tutorial.zh-cn.md
--rw-r--r--   0        0        0      229 2023-07-05 20:19:19.041353 cornflakes-3.3.7/inst/ext/rapidjson/docker/debian/Dockerfile
--rw-r--r--   0        0        0      982 2023-07-05 20:19:19.041353 cornflakes-3.3.7/inst/ext/rapidjson/example/CMakeLists.txt
--rw-r--r--   0        0        0     7130 2023-07-05 20:19:19.041353 cornflakes-3.3.7/inst/ext/rapidjson/example/archiver/archiver.cpp
--rw-r--r--   0        0        0     3567 2023-07-05 20:19:19.041353 cornflakes-3.3.7/inst/ext/rapidjson/example/archiver/archiver.h
--rw-r--r--   0        0        0     6862 2023-07-05 20:19:19.041353 cornflakes-3.3.7/inst/ext/rapidjson/example/archiver/archivertest.cpp
--rw-r--r--   0        0        0     2577 2023-07-05 20:19:19.041353 cornflakes-3.3.7/inst/ext/rapidjson/example/capitalize/capitalize.cpp
--rw-r--r--   0        0        0     1015 2023-07-05 20:19:19.041353 cornflakes-3.3.7/inst/ext/rapidjson/example/condense/condense.cpp
--rw-r--r--   0        0        0     4979 2023-07-05 20:19:19.041353 cornflakes-3.3.7/inst/ext/rapidjson/example/filterkey/filterkey.cpp
--rw-r--r--   0        0        0     5946 2023-07-05 20:19:19.041353 cornflakes-3.3.7/inst/ext/rapidjson/example/filterkeydom/filterkeydom.cpp
--rw-r--r--   0        0        0     6022 2023-07-05 20:19:19.041353 cornflakes-3.3.7/inst/ext/rapidjson/example/jsonx/jsonx.cpp
--rw-r--r--   0        0        0     9461 2023-07-05 20:19:19.041353 cornflakes-3.3.7/inst/ext/rapidjson/example/lookaheadparser/lookaheadparser.cpp
--rw-r--r--   0        0        0     2814 2023-07-05 20:19:19.041353 cornflakes-3.3.7/inst/ext/rapidjson/example/messagereader/messagereader.cpp
--rw-r--r--   0        0        0     5150 2023-07-05 20:19:19.041353 cornflakes-3.3.7/inst/ext/rapidjson/example/parsebyparts/parsebyparts.cpp
--rw-r--r--   0        0        0     1019 2023-07-05 20:19:19.041353 cornflakes-3.3.7/inst/ext/rapidjson/example/pretty/pretty.cpp
--rw-r--r--   0        0        0     2245 2023-07-05 20:19:19.041353 cornflakes-3.3.7/inst/ext/rapidjson/example/prettyauto/prettyauto.cpp
--rw-r--r--   0        0        0     8706 2023-07-05 20:19:19.041353 cornflakes-3.3.7/inst/ext/rapidjson/example/schemavalidator/schemavalidator.cpp
--rw-r--r--   0        0        0     4590 2023-07-05 20:19:19.041353 cornflakes-3.3.7/inst/ext/rapidjson/example/serialize/serialize.cpp
--rw-r--r--   0        0        0      685 2023-07-05 20:19:19.041353 cornflakes-3.3.7/inst/ext/rapidjson/example/simpledom/simpledom.cpp
--rw-r--r--   0        0        0     2259 2023-07-05 20:19:19.041353 cornflakes-3.3.7/inst/ext/rapidjson/example/simplepullreader/simplepullreader.cpp
--rw-r--r--   0        0        0     1868 2023-07-05 20:19:19.041353 cornflakes-3.3.7/inst/ext/rapidjson/example/simplereader/simplereader.cpp
--rw-r--r--   0        0        0     1031 2023-07-05 20:19:19.041353 cornflakes-3.3.7/inst/ext/rapidjson/example/simplewriter/simplewriter.cpp
--rw-r--r--   0        0        0     1610 2023-07-05 20:19:19.041353 cornflakes-3.3.7/inst/ext/rapidjson/example/sortkeys/sortkeys.cpp
--rw-r--r--   0        0        0      943 2023-07-05 20:19:19.041353 cornflakes-3.3.7/inst/ext/rapidjson/example/traverseaspointer.cpp
--rw-r--r--   0        0        0     6263 2023-07-05 20:19:19.041353 cornflakes-3.3.7/inst/ext/rapidjson/example/tutorial/tutorial.cpp
--rw-r--r--   0        0        0    22592 2023-07-05 20:19:19.041353 cornflakes-3.3.7/inst/ext/rapidjson/include/rapidjson/allocators.h
--rw-r--r--   0        0        0     2260 2023-07-05 20:19:19.041353 cornflakes-3.3.7/inst/ext/rapidjson/include/rapidjson/cursorstreamwrapper.h
--rw-r--r--   0        0        0   133763 2023-07-05 20:19:19.045353 cornflakes-3.3.7/inst/ext/rapidjson/include/rapidjson/document.h
--rw-r--r--   0        0        0    10660 2023-07-05 20:19:19.045353 cornflakes-3.3.7/inst/ext/rapidjson/include/rapidjson/encodedstream.h
--rw-r--r--   0        0        0    29260 2023-07-05 20:19:19.045353 cornflakes-3.3.7/inst/ext/rapidjson/include/rapidjson/encodings.h
--rw-r--r--   0        0        0    13025 2023-07-05 20:19:19.045353 cornflakes-3.3.7/inst/ext/rapidjson/include/rapidjson/error/en.h
--rw-r--r--   0        0        0    13353 2023-07-05 20:19:19.045353 cornflakes-3.3.7/inst/ext/rapidjson/include/rapidjson/error/error.h
--rw-r--r--   0        0        0     2980 2023-07-05 20:19:19.045353 cornflakes-3.3.7/inst/ext/rapidjson/include/rapidjson/filereadstream.h
--rw-r--r--   0        0        0     3125 2023-07-05 20:19:19.045353 cornflakes-3.3.7/inst/ext/rapidjson/include/rapidjson/filewritestream.h
--rw-r--r--   0        0        0     4013 2023-07-05 20:19:19.045353 cornflakes-3.3.7/inst/ext/rapidjson/include/rapidjson/fwd.h
--rw-r--r--   0        0        0     9271 2023-07-05 20:19:19.045353 cornflakes-3.3.7/inst/ext/rapidjson/include/rapidjson/internal/biginteger.h
--rw-r--r--   0        0        0     2045 2023-07-05 20:19:19.045353 cornflakes-3.3.7/inst/ext/rapidjson/include/rapidjson/internal/clzll.h
--rw-r--r--   0        0        0    11559 2023-07-05 20:19:19.045353 cornflakes-3.3.7/inst/ext/rapidjson/include/rapidjson/internal/diyfp.h
--rw-r--r--   0        0        0     8473 2023-07-05 20:19:19.045353 cornflakes-3.3.7/inst/ext/rapidjson/include/rapidjson/internal/dtoa.h
--rw-r--r--   0        0        0     2973 2023-07-05 20:19:19.045353 cornflakes-3.3.7/inst/ext/rapidjson/include/rapidjson/internal/ieee754.h
--rw-r--r--   0        0        0    10110 2023-07-05 20:19:19.045353 cornflakes-3.3.7/inst/ext/rapidjson/include/rapidjson/internal/itoa.h
--rw-r--r--   0        0        0     6620 2023-07-05 20:19:19.045353 cornflakes-3.3.7/inst/ext/rapidjson/include/rapidjson/internal/meta.h
--rw-r--r--   0        0        0     3574 2023-07-05 20:19:19.045353 cornflakes-3.3.7/inst/ext/rapidjson/include/rapidjson/internal/pow10.h
--rw-r--r--   0        0        0    26120 2023-07-05 20:19:19.045353 cornflakes-3.3.7/inst/ext/rapidjson/include/rapidjson/internal/regex.h
--rw-r--r--   0        0        0     7163 2023-07-05 20:19:19.045353 cornflakes-3.3.7/inst/ext/rapidjson/include/rapidjson/internal/stack.h
--rw-r--r--   0        0        0     2726 2023-07-05 20:19:19.045353 cornflakes-3.3.7/inst/ext/rapidjson/include/rapidjson/internal/strfunc.h
--rw-r--r--   0        0        0     9045 2023-07-05 20:19:19.045353 cornflakes-3.3.7/inst/ext/rapidjson/include/rapidjson/internal/strtod.h
--rw-r--r--   0        0        0     1398 2023-07-05 20:19:19.045353 cornflakes-3.3.7/inst/ext/rapidjson/include/rapidjson/internal/swap.h
--rw-r--r--   0        0        0     4061 2023-07-05 20:19:19.045353 cornflakes-3.3.7/inst/ext/rapidjson/include/rapidjson/istreamwrapper.h
--rw-r--r--   0        0        0     2539 2023-07-05 20:19:19.045353 cornflakes-3.3.7/inst/ext/rapidjson/include/rapidjson/memorybuffer.h
--rw-r--r--   0        0        0     2646 2023-07-05 20:19:19.045353 cornflakes-3.3.7/inst/ext/rapidjson/include/rapidjson/memorystream.h
--rw-r--r--   0        0        0     8372 2023-07-05 20:19:19.045353 cornflakes-3.3.7/inst/ext/rapidjson/include/rapidjson/msinttypes/inttypes.h
--rw-r--r--   0        0        0     9386 2023-07-05 20:19:19.045353 cornflakes-3.3.7/inst/ext/rapidjson/include/rapidjson/msinttypes/stdint.h
--rw-r--r--   0        0        0     2310 2023-07-05 20:19:19.045353 cornflakes-3.3.7/inst/ext/rapidjson/include/rapidjson/ostreamwrapper.h
--rw-r--r--   0        0        0    63132 2023-07-05 20:19:19.045353 cornflakes-3.3.7/inst/ext/rapidjson/include/rapidjson/pointer.h
--rw-r--r--   0        0        0    10518 2023-07-05 20:19:19.045353 cornflakes-3.3.7/inst/ext/rapidjson/include/rapidjson/prettywriter.h
--rw-r--r--   0        0        0    25585 2023-07-05 20:19:19.045353 cornflakes-3.3.7/inst/ext/rapidjson/include/rapidjson/rapidjson.h
--rw-r--r--   0        0        0    94332 2023-07-05 20:19:19.045353 cornflakes-3.3.7/inst/ext/rapidjson/include/rapidjson/reader.h
--rw-r--r--   0        0        0   146796 2023-07-05 20:19:19.049353 cornflakes-3.3.7/inst/ext/rapidjson/include/rapidjson/schema.h
--rw-r--r--   0        0        0     6732 2023-07-05 20:19:19.049353 cornflakes-3.3.7/inst/ext/rapidjson/include/rapidjson/stream.h
--rw-r--r--   0        0        0     3972 2023-07-05 20:19:19.049353 cornflakes-3.3.7/inst/ext/rapidjson/include/rapidjson/stringbuffer.h
--rw-r--r--   0        0        0    19752 2023-07-05 20:19:19.049353 cornflakes-3.3.7/inst/ext/rapidjson/include/rapidjson/uri.h
--rw-r--r--   0        0        0    26856 2023-07-05 20:19:19.049353 cornflakes-3.3.7/inst/ext/rapidjson/include/rapidjson/writer.h
--rw-r--r--   0        0        0       94 2023-07-05 20:19:19.049353 cornflakes-3.3.7/inst/ext/rapidjson/include_dirs.js
--rw-r--r--   0        0        0      355 2023-07-05 20:19:19.049353 cornflakes-3.3.7/inst/ext/rapidjson/library.json
--rw-r--r--   0        0        0     5152 2023-07-05 20:19:19.049353 cornflakes-3.3.7/inst/ext/rapidjson/license.txt
--rw-r--r--   0        0        0      561 2023-07-05 20:19:19.049353 cornflakes-3.3.7/inst/ext/rapidjson/package.json
--rw-r--r--   0        0        0     3407 2023-07-05 20:19:19.049353 cornflakes-3.3.7/inst/ext/rapidjson/rapidjson.autopkg
--rw-r--r--   0        0        0    11146 2023-07-05 20:19:19.049353 cornflakes-3.3.7/inst/ext/rapidjson/readme.md
--rw-r--r--   0        0        0     8795 2023-07-05 20:19:19.049353 cornflakes-3.3.7/inst/ext/rapidjson/readme.zh-cn.md
--rw-r--r--   0        0        0      491 2023-07-05 20:19:19.049353 cornflakes-3.3.7/inst/ext/rapidjson/test/CMakeLists.txt
--rw-r--r--   0        0        0      834 2023-07-05 20:19:19.049353 cornflakes-3.3.7/inst/ext/rapidjson/test/perftest/CMakeLists.txt
--rw-r--r--   0        0        0    35467 2023-07-05 20:19:19.049353 cornflakes-3.3.7/inst/ext/rapidjson/test/perftest/misctest.cpp
--rw-r--r--   0        0        0      975 2023-07-05 20:19:19.049353 cornflakes-3.3.7/inst/ext/rapidjson/test/perftest/perftest.cpp
--rw-r--r--   0        0        0     5756 2023-07-05 20:19:19.049353 cornflakes-3.3.7/inst/ext/rapidjson/test/perftest/perftest.h
--rw-r--r--   0        0        0     4456 2023-07-05 20:19:19.049353 cornflakes-3.3.7/inst/ext/rapidjson/test/perftest/platformtest.cpp
--rw-r--r--   0        0        0    16302 2023-07-05 20:19:19.049353 cornflakes-3.3.7/inst/ext/rapidjson/test/perftest/rapidjsontest.cpp
--rw-r--r--   0        0        0     7218 2023-07-05 20:19:19.049353 cornflakes-3.3.7/inst/ext/rapidjson/test/perftest/schematest.cpp
--rw-r--r--   0        0        0     3060 2023-07-05 20:19:19.049353 cornflakes-3.3.7/inst/ext/rapidjson/test/unittest/CMakeLists.txt
--rw-r--r--   0        0        0     9040 2023-07-05 20:19:19.049353 cornflakes-3.3.7/inst/ext/rapidjson/test/unittest/allocatorstest.cpp
--rw-r--r--   0        0        0     4420 2023-07-05 20:19:19.049353 cornflakes-3.3.7/inst/ext/rapidjson/test/unittest/bigintegertest.cpp
--rw-r--r--   0        0        0     1092 2023-07-05 20:19:19.049353 cornflakes-3.3.7/inst/ext/rapidjson/test/unittest/clzlltest.cpp
--rw-r--r--   0        0        0     3733 2023-07-05 20:19:19.049353 cornflakes-3.3.7/inst/ext/rapidjson/test/unittest/cursorstreamwrappertest.cpp
--rw-r--r--   0        0        0    21279 2023-07-05 20:19:19.049353 cornflakes-3.3.7/inst/ext/rapidjson/test/unittest/documenttest.cpp
--rw-r--r--   0        0        0     3441 2023-07-05 20:19:19.049353 cornflakes-3.3.7/inst/ext/rapidjson/test/unittest/dtoatest.cpp
--rw-r--r--   0        0        0    12004 2023-07-05 20:19:19.049353 cornflakes-3.3.7/inst/ext/rapidjson/test/unittest/encodedstreamtest.cpp
--rw-r--r--   0        0        0    19344 2023-07-05 20:19:19.049353 cornflakes-3.3.7/inst/ext/rapidjson/test/unittest/encodingstest.cpp
--rw-r--r--   0        0        0     4389 2023-07-05 20:19:19.049353 cornflakes-3.3.7/inst/ext/rapidjson/test/unittest/filestreamtest.cpp
--rw-r--r--   0        0        0     5837 2023-07-05 20:19:19.049353 cornflakes-3.3.7/inst/ext/rapidjson/test/unittest/fwdtest.cpp
--rw-r--r--   0        0        0     5419 2023-07-05 20:19:19.049353 cornflakes-3.3.7/inst/ext/rapidjson/test/unittest/istreamwrappertest.cpp
--rw-r--r--   0        0        0     3956 2023-07-05 20:19:19.049353 cornflakes-3.3.7/inst/ext/rapidjson/test/unittest/itoatest.cpp
--rw-r--r--   0        0        0     4753 2023-07-05 20:19:19.049353 cornflakes-3.3.7/inst/ext/rapidjson/test/unittest/jsoncheckertest.cpp
--rw-r--r--   0        0        0     2401 2023-07-05 20:19:19.049353 cornflakes-3.3.7/inst/ext/rapidjson/test/unittest/namespacetest.cpp
--rw-r--r--   0        0        0     2481 2023-07-05 20:19:19.049353 cornflakes-3.3.7/inst/ext/rapidjson/test/unittest/ostreamwrappertest.cpp
--rw-r--r--   0        0        0     1457 2023-07-05 20:19:19.049353 cornflakes-3.3.7/inst/ext/rapidjson/test/unittest/platformtest.cpp
--rw-r--r--   0        0        0    62776 2023-07-05 20:19:19.049353 cornflakes-3.3.7/inst/ext/rapidjson/test/unittest/pointertest.cpp
--rw-r--r--   0        0        0    10350 2023-07-05 20:19:19.049353 cornflakes-3.3.7/inst/ext/rapidjson/test/unittest/prettywritertest.cpp
--rw-r--r--   0        0        0    98539 2023-07-05 20:19:19.049353 cornflakes-3.3.7/inst/ext/rapidjson/test/unittest/readertest.cpp
--rw-r--r--   0        0        0    17263 2023-07-05 20:19:19.049353 cornflakes-3.3.7/inst/ext/rapidjson/test/unittest/regextest.cpp
--rw-r--r--   0        0        0   150825 2023-07-05 20:19:19.049353 cornflakes-3.3.7/inst/ext/rapidjson/test/unittest/schematest.cpp
--rw-r--r--   0        0        0     7121 2023-07-05 20:19:19.049353 cornflakes-3.3.7/inst/ext/rapidjson/test/unittest/simdtest.cpp
--rw-r--r--   0        0        0     1316 2023-07-05 20:19:19.049353 cornflakes-3.3.7/inst/ext/rapidjson/test/unittest/strfunctest.cpp
--rw-r--r--   0        0        0     5544 2023-07-05 20:19:19.049353 cornflakes-3.3.7/inst/ext/rapidjson/test/unittest/stringbuffertest.cpp
--rw-r--r--   0        0        0     4256 2023-07-05 20:19:19.049353 cornflakes-3.3.7/inst/ext/rapidjson/test/unittest/strtodtest.cpp
--rw-r--r--   0        0        0     1527 2023-07-05 20:19:19.053353 cornflakes-3.3.7/inst/ext/rapidjson/test/unittest/unittest.cpp
--rw-r--r--   0        0        0     3979 2023-07-05 20:19:19.053353 cornflakes-3.3.7/inst/ext/rapidjson/test/unittest/unittest.h
--rw-r--r--   0        0        0    28512 2023-07-05 20:19:19.053353 cornflakes-3.3.7/inst/ext/rapidjson/test/unittest/uritest.cpp
--rw-r--r--   0        0        0    57574 2023-07-05 20:19:19.053353 cornflakes-3.3.7/inst/ext/rapidjson/test/unittest/valuetest.cpp
--rw-r--r--   0        0        0    17932 2023-07-05 20:19:19.053353 cornflakes-3.3.7/inst/ext/rapidjson/test/unittest/writertest.cpp
--rw-r--r--   0        0        0      369 2023-07-05 20:19:19.053353 cornflakes-3.3.7/inst/ext/rapidjson/test/valgrind.supp
--rw-r--r--   0        0        0       80 2023-07-05 20:19:19.653361 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/.git
--rw-r--r--   0        0        0      595 2023-07-05 20:19:20.917378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/.gitignore
--rw-r--r--   0        0        0     2591 2023-07-05 20:19:20.917378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/.travis.yml
--rw-r--r--   0        0        0     4940 2023-07-05 20:19:20.917378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/BUILD.bazel
--rw-r--r--   0        0        0     1220 2023-07-05 20:19:20.917378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/CMakeLists.txt
--rw-r--r--   0        0        0     6738 2023-07-05 20:19:20.917378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/CONTRIBUTING.md
--rw-r--r--   0        0        0     1475 2023-07-05 20:19:20.917378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/LICENSE
--rw-r--r--   0        0        0      315 2023-07-05 20:19:20.917378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/Makefile.am
--rw-r--r--   0        0        0     4501 2023-07-05 20:19:20.917378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/README.md
--rw-r--r--   0        0        0      213 2023-07-05 20:19:20.917378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/WORKSPACE
--rw-r--r--   0        0        0     3405 2023-07-05 20:19:20.917378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/appveyor.yml
--rwxr-xr-x   0        0        0     1751 2023-07-05 20:19:20.917378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/ci/build-linux-autotools.sh
--rwxr-xr-x   0        0        0     1674 2023-07-05 20:19:20.917378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/ci/build-linux-bazel.sh
--rwxr-xr-x   0        0        0     1922 2023-07-05 20:19:20.917378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/ci/env-linux.sh
--rwxr-xr-x   0        0        0     1852 2023-07-05 20:19:20.917378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/ci/env-osx.sh
--rwxr-xr-x   0        0        0     2220 2023-07-05 20:19:20.917378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/ci/get-nprocessors.sh
--rwxr-xr-x   0        0        0     2229 2023-07-05 20:19:20.917378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/ci/install-linux.sh
--rwxr-xr-x   0        0        0     1688 2023-07-05 20:19:20.917378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/ci/install-osx.sh
--rwxr-xr-x   0        0        0     2093 2023-07-05 20:19:20.917378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/ci/log-config.sh
--rwxr-xr-x   0        0        0     1310 2023-07-05 20:19:20.917378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/ci/travis.sh
--rw-r--r--   0        0        0      461 2023-07-05 20:19:20.917378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/configure.ac
--rw-r--r--   0        0        0     5559 2023-07-05 20:19:20.917378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/CHANGES
--rw-r--r--   0        0        0     9463 2023-07-05 20:19:20.917378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/CMakeLists.txt
--rw-r--r--   0        0        0     1369 2023-07-05 20:19:20.917378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/CONTRIBUTORS
--rw-r--r--   0        0        0     1475 2023-07-05 20:19:20.917378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/LICENSE
--rw-r--r--   0        0        0     7627 2023-07-05 20:19:20.917378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/Makefile.am
--rw-r--r--   0        0        0    13045 2023-07-05 20:19:20.917378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/README.md
--rw-r--r--   0        0        0        0 2023-07-05 20:19:20.917378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/build-aux/.keep
--rw-r--r--   0        0        0      336 2023-07-05 20:19:20.917378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/cmake/gmock.pc.in
--rw-r--r--   0        0        0      343 2023-07-05 20:19:20.917378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/cmake/gmock_main.pc.in
--rw-r--r--   0        0        0     6260 2023-07-05 20:19:20.917378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/configure.ac
--rw-r--r--   0        0        0    28266 2023-07-05 20:19:20.917378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/docs/CheatSheet.md
--rw-r--r--   0        0        0   128053 2023-07-05 20:19:20.921378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/docs/CookBook.md
--rw-r--r--   0        0        0     9924 2023-07-05 20:19:20.921378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/docs/DesignDoc.md
--rw-r--r--   0        0        0      838 2023-07-05 20:19:20.921378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/docs/Documentation.md
--rw-r--r--   0        0        0    30079 2023-07-05 20:19:20.921378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/docs/ForDummies.md
--rw-r--r--   0        0        0    23329 2023-07-05 20:19:20.921378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/docs/FrequentlyAskedQuestions.md
--rw-r--r--   0        0        0     1528 2023-07-05 20:19:20.921378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/docs/KnownIssues.md
--rw-r--r--   0        0        0    42948 2023-07-05 20:19:20.921378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/include/gmock/gmock-actions.h
--rw-r--r--   0        0        0     5820 2023-07-05 20:19:20.921378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/include/gmock/gmock-cardinalities.h
--rw-r--r--   0        0        0   114405 2023-07-05 20:19:20.921378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/include/gmock/gmock-generated-actions.h
--rw-r--r--   0        0        0    27848 2023-07-05 20:19:20.921378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/include/gmock/gmock-generated-actions.h.pump
--rw-r--r--   0        0        0    74779 2023-07-05 20:19:20.921378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/include/gmock/gmock-generated-function-mockers.h
--rw-r--r--   0        0        0    11740 2023-07-05 20:19:20.921378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/include/gmock/gmock-generated-function-mockers.h.pump
--rw-r--r--   0        0        0    90816 2023-07-05 20:19:20.921378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/include/gmock/gmock-generated-matchers.h
--rw-r--r--   0        0        0    21921 2023-07-05 20:19:20.921378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/include/gmock/gmock-generated-matchers.h.pump
--rw-r--r--   0        0        0    18419 2023-07-05 20:19:20.921378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/include/gmock/gmock-generated-nice-strict.h
--rw-r--r--   0        0        0     6598 2023-07-05 20:19:20.921378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/include/gmock/gmock-generated-nice-strict.h.pump
--rw-r--r--   0        0        0   190280 2023-07-05 20:19:20.925378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/include/gmock/gmock-matchers.h
--rw-r--r--   0        0        0     9377 2023-07-05 20:19:20.925378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/include/gmock/gmock-more-actions.h
--rw-r--r--   0        0        0     3357 2023-07-05 20:19:20.925378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/include/gmock/gmock-more-matchers.h
--rw-r--r--   0        0        0    72839 2023-07-05 20:19:20.925378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/include/gmock/gmock-spec-builders.h
--rw-r--r--   0        0        0     3683 2023-07-05 20:19:20.925378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/include/gmock/gmock.h
--rw-r--r--   0        0        0      329 2023-07-05 20:19:20.925378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/include/gmock/internal/custom/gmock-generated-actions.h
--rw-r--r--   0        0        0      415 2023-07-05 20:19:20.925378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/include/gmock/internal/custom/gmock-generated-actions.h.pump
--rw-r--r--   0        0        0     2000 2023-07-05 20:19:20.925378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/include/gmock/internal/custom/gmock-matchers.h
--rw-r--r--   0        0        0     2159 2023-07-05 20:19:20.925378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/include/gmock/internal/custom/gmock-port.h
--rw-r--r--   0        0        0    11633 2023-07-05 20:19:20.925378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/include/gmock/internal/gmock-generated-internal-utils.h
--rw-r--r--   0        0        0     4926 2023-07-05 20:19:20.925378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/include/gmock/internal/gmock-generated-internal-utils.h.pump
--rw-r--r--   0        0        0    22618 2023-07-05 20:19:20.925378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/include/gmock/internal/gmock-internal-utils.h
--rw-r--r--   0        0        0     3867 2023-07-05 20:19:20.925378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/include/gmock/internal/gmock-port.h
--rw-r--r--   0        0        0     3681 2023-07-05 20:19:20.925378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/make/Makefile
--rw-r--r--   0        0        0     1788 2023-07-05 20:19:20.925378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/msvc/2005/gmock.sln
--rw-r--r--   0        0        0     3993 2023-07-05 20:19:20.925378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/msvc/2005/gmock.vcproj
--rw-r--r--   0        0        0      349 2023-07-05 20:19:20.925378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/msvc/2005/gmock_config.vsprops
--rw-r--r--   0        0        0     3992 2023-07-05 20:19:20.925378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/msvc/2005/gmock_main.vcproj
--rw-r--r--   0        0        0     4251 2023-07-05 20:19:20.925378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/msvc/2005/gmock_test.vcproj
--rw-r--r--   0        0        0     2751 2023-07-05 20:19:20.925378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/msvc/2010/gmock.sln
--rw-r--r--   0        0        0     8485 2023-07-05 20:19:20.925378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/msvc/2010/gmock.vcxproj
--rw-r--r--   0        0        0      697 2023-07-05 20:19:20.925378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/msvc/2010/gmock_config.props
--rw-r--r--   0        0        0     8722 2023-07-05 20:19:20.925378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/msvc/2010/gmock_main.vcxproj
--rw-r--r--   0        0        0     9648 2023-07-05 20:19:20.925378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/msvc/2010/gmock_test.vcxproj
--rw-r--r--   0        0        0     2698 2023-07-05 20:19:20.925378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/msvc/2015/gmock.sln
--rw-r--r--   0        0        0     8274 2023-07-05 20:19:20.925378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/msvc/2015/gmock.vcxproj
--rw-r--r--   0        0        0      677 2023-07-05 20:19:20.925378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/msvc/2015/gmock_config.props
--rw-r--r--   0        0        0     8505 2023-07-05 20:19:20.925378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/msvc/2015/gmock_main.vcxproj
--rw-r--r--   0        0        0     9406 2023-07-05 20:19:20.925378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/msvc/2015/gmock_test.vcxproj
--rwxr-xr-x   0        0        0     8658 2023-07-05 20:19:20.925378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/scripts/fuse_gmock_files.py
--rw-r--r--   0        0        0    11386 2023-07-05 20:19:20.925378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/scripts/generator/LICENSE
--rw-r--r--   0        0        0     1327 2023-07-05 20:19:20.925378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/scripts/generator/README
--rw-r--r--   0        0        0     4216 2023-07-05 20:19:20.929378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/scripts/generator/README.cppclean
--rwxr-xr-x   0        0        0        0 2023-07-05 20:19:20.929378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/scripts/generator/cpp/__init__.py
--rwxr-xr-x   0        0        0    62772 2023-07-05 20:19:20.929378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/scripts/generator/cpp/ast.py
--rwxr-xr-x   0        0        0     8293 2023-07-05 20:19:20.929378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/scripts/generator/cpp/gmock_class.py
--rwxr-xr-x   0        0        0    11356 2023-07-05 20:19:20.929378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/scripts/generator/cpp/gmock_class_test.py
--rwxr-xr-x   0        0        0     2004 2023-07-05 20:19:20.929378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/scripts/generator/cpp/keywords.py
--rwxr-xr-x   0        0        0     9752 2023-07-05 20:19:20.929378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/scripts/generator/cpp/tokenize.py
--rwxr-xr-x   0        0        0     1153 2023-07-05 20:19:20.929378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/scripts/generator/cpp/utils.py
--rwxr-xr-x   0        0        0     1091 2023-07-05 20:19:20.929378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/scripts/generator/gmock_gen.py
--rwxr-xr-x   0        0        0    11167 2023-07-05 20:19:20.929378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/scripts/gmock-config.in
--rwxr-xr-x   0        0        0    24131 2023-07-05 20:19:20.929378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/scripts/gmock_doctor.py
--rwxr-xr-x   0        0        0    51024 2023-07-05 20:19:20.929378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/scripts/upload.py
--rwxr-xr-x   0        0        0     2833 2023-07-05 20:19:20.929378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/scripts/upload_gmock.py
--rw-r--r--   0        0        0     2150 2023-07-05 20:19:20.929378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/src/gmock-all.cc
--rw-r--r--   0        0        0     5300 2023-07-05 20:19:20.929378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/src/gmock-cardinalities.cc
--rw-r--r--   0        0        0     7665 2023-07-05 20:19:20.929378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/src/gmock-internal-utils.cc
--rw-r--r--   0        0        0    21845 2023-07-05 20:19:20.929378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/src/gmock-matchers.cc
--rw-r--r--   0        0        0    32771 2023-07-05 20:19:20.929378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/src/gmock-spec-builders.cc
--rw-r--r--   0        0        0     7930 2023-07-05 20:19:20.929378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/src/gmock.cc
--rw-r--r--   0        0        0     2593 2023-07-05 20:19:20.929378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/src/gmock_main.cc
--rw-r--r--   0        0        0     3159 2023-07-05 20:19:20.929378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/test/BUILD.bazel
--rw-r--r--   0        0        0    50479 2023-07-05 20:19:20.929378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/test/gmock-actions_test.cc
--rw-r--r--   0        0        0    12329 2023-07-05 20:19:20.929378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/test/gmock-cardinalities_test.cc
--rw-r--r--   0        0        0    41272 2023-07-05 20:19:20.929378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/test/gmock-generated-actions_test.cc
--rw-r--r--   0        0        0    20021 2023-07-05 20:19:20.929378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/test/gmock-generated-function-mockers_test.cc
--rw-r--r--   0        0        0     5320 2023-07-05 20:19:20.929378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/test/gmock-generated-internal-utils_test.cc
--rw-r--r--   0        0        0    44061 2023-07-05 20:19:20.929378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/test/gmock-generated-matchers_test.cc
--rw-r--r--   0        0        0    25225 2023-07-05 20:19:20.929378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/test/gmock-internal-utils_test.cc
--rw-r--r--   0        0        0   221497 2023-07-05 20:19:20.933378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/test/gmock-matchers_test.cc
--rw-r--r--   0        0        0    24389 2023-07-05 20:19:20.933378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/test/gmock-more-actions_test.cc
--rw-r--r--   0        0        0    15340 2023-07-05 20:19:20.933378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/test/gmock-nice-strict_test.cc
--rw-r--r--   0        0        0     2020 2023-07-05 20:19:20.933378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/test/gmock-port_test.cc
--rw-r--r--   0        0        0    74777 2023-07-05 20:19:20.933378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/test/gmock-spec-builders_test.cc
--rw-r--r--   0        0        0     2587 2023-07-05 20:19:20.933378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/test/gmock_all_test.cc
--rw-r--r--   0        0        0     3323 2023-07-05 20:19:20.933378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/test/gmock_ex_test.cc
--rwxr-xr-x   0        0        0     4384 2023-07-05 20:19:20.933378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/test/gmock_leak_test.py
--rw-r--r--   0        0        0     3273 2023-07-05 20:19:20.933378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/test/gmock_leak_test_.cc
--rw-r--r--   0        0        0     1950 2023-07-05 20:19:20.933378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/test/gmock_link2_test.cc
--rw-r--r--   0        0        0     1950 2023-07-05 20:19:20.933378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/test/gmock_link_test.cc
--rw-r--r--   0        0        0    19572 2023-07-05 20:19:20.933378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/test/gmock_link_test.h
--rwxr-xr-x   0        0        0     6105 2023-07-05 20:19:20.933378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/test/gmock_output_test.py
--rw-r--r--   0        0        0     8640 2023-07-05 20:19:20.933378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/test/gmock_output_test_.cc
--rw-r--r--   0        0        0    13612 2023-07-05 20:19:20.933378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/test/gmock_output_test_golden.txt
--rw-r--r--   0        0        0     9323 2023-07-05 20:19:20.933378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/test/gmock_stress_test.cc
--rw-r--r--   0        0        0     6661 2023-07-05 20:19:20.933378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/test/gmock_test.cc
--rwxr-xr-x   0        0        0     3667 2023-07-05 20:19:20.933378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/test/gmock_test_utils.py
--rw-r--r--   0        0        0     6645 2023-07-05 20:19:20.933378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/CHANGES
--rw-r--r--   0        0        0    11363 2023-07-05 20:19:20.933378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/CMakeLists.txt
--rw-r--r--   0        0        0     1358 2023-07-05 20:19:20.933378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/CONTRIBUTORS
--rw-r--r--   0        0        0     1475 2023-07-05 20:19:20.933378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/LICENSE
--rw-r--r--   0        0        0    11553 2023-07-05 20:19:20.933378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/Makefile.am
--rw-r--r--   0        0        0    14263 2023-07-05 20:19:20.933378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/README.md
--rw-r--r--   0        0        0      336 2023-07-05 20:19:20.933378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/cmake/gtest.pc.in
--rw-r--r--   0        0        0      359 2023-07-05 20:19:20.933378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/cmake/gtest_main.pc.in
--rw-r--r--   0        0        0    12013 2023-07-05 20:19:20.933378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/cmake/internal_utils.cmake
--rw-r--r--   0        0        0    10623 2023-07-05 20:19:20.933378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/codegear/gtest.cbproj
--rw-r--r--   0        0        0     2061 2023-07-05 20:19:20.933378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/codegear/gtest.groupproj
--rw-r--r--   0        0        0     1903 2023-07-05 20:19:20.933378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/codegear/gtest_all.cc
--rw-r--r--   0        0        0     2033 2023-07-05 20:19:20.933378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/codegear/gtest_link.cc
--rw-r--r--   0        0        0     8662 2023-07-05 20:19:20.933378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/codegear/gtest_main.cbproj
--rw-r--r--   0        0        0     8778 2023-07-05 20:19:20.933378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/codegear/gtest_unittest.cbproj
--rw-r--r--   0        0        0     2574 2023-07-05 20:19:20.933378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/configure.ac
--rw-r--r--   0        0        0     3996 2023-07-05 20:19:20.933378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/docs/Pkgconfig.md
--rw-r--r--   0        0        0     6958 2023-07-05 20:19:20.933378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/docs/PumpManual.md
--rw-r--r--   0        0        0     8246 2023-07-05 20:19:20.933378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/docs/XcodeGuide.md
--rw-r--r--   0        0        0    93685 2023-07-05 20:19:20.937379 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/docs/advanced.md
--rw-r--r--   0        0        0    47943 2023-07-05 20:19:20.937379 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/docs/faq.md
--rw-r--r--   0        0        0    26445 2023-07-05 20:19:20.937379 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/docs/primer.md
--rw-r--r--   0        0        0     1329 2023-07-05 20:19:20.937379 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/docs/samples.md
--rw-r--r--   0        0        0    14349 2023-07-05 20:19:20.937379 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/include/gtest/gtest-death-test.h
--rw-r--r--   0        0        0     9197 2023-07-05 20:19:20.937379 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/include/gtest/gtest-message.h
--rw-r--r--   0        0        0    77427 2023-07-05 20:19:20.937379 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/include/gtest/gtest-param-test.h
--rw-r--r--   0        0        0    19875 2023-07-05 20:19:20.937379 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/include/gtest/gtest-param-test.h.pump
--rw-r--r--   0        0        0    39278 2023-07-05 20:19:20.937379 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/include/gtest/gtest-printers.h
--rw-r--r--   0        0        0     9939 2023-07-05 20:19:20.937379 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/include/gtest/gtest-spi.h
--rw-r--r--   0        0        0     6509 2023-07-05 20:19:20.937379 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/include/gtest/gtest-test-part.h
--rw-r--r--   0        0        0    10500 2023-07-05 20:19:20.937379 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/include/gtest/gtest-typed-test.h
--rw-r--r--   0        0        0    88660 2023-07-05 20:19:20.937379 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/include/gtest/gtest.h
--rw-r--r--   0        0        0    14908 2023-07-05 20:19:20.937379 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/include/gtest/gtest_pred_impl.h
--rw-r--r--   0        0        0     2527 2023-07-05 20:19:20.937379 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/include/gtest/gtest_prod.h
--rw-r--r--   0        0        0     3066 2023-07-05 20:19:20.937379 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/include/gtest/internal/custom/gtest-port.h
--rw-r--r--   0        0        0     2099 2023-07-05 20:19:20.937379 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/include/gtest/internal/custom/gtest-printers.h
--rw-r--r--   0        0        0     2192 2023-07-05 20:19:20.937379 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/include/gtest/internal/custom/gtest.h
--rw-r--r--   0        0        0    11192 2023-07-05 20:19:20.937379 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/include/gtest/internal/gtest-death-test-internal.h
--rw-r--r--   0        0        0     9558 2023-07-05 20:19:20.937379 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/include/gtest/internal/gtest-filepath.h
--rw-r--r--   0        0        0    48549 2023-07-05 20:19:20.937379 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/include/gtest/internal/gtest-internal.h
--rw-r--r--   0        0        0     8424 2023-07-05 20:19:20.937379 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/include/gtest/internal/gtest-linked_ptr.h
--rw-r--r--   0        0        0   192179 2023-07-05 20:19:20.937379 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/include/gtest/internal/gtest-param-util-generated.h
--rw-r--r--   0        0        0     8901 2023-07-05 20:19:20.937379 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/include/gtest/internal/gtest-param-util-generated.h.pump
--rw-r--r--   0        0        0    27669 2023-07-05 20:19:20.941378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/include/gtest/internal/gtest-param-util.h
--rw-r--r--   0        0        0     3723 2023-07-05 20:19:20.941378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/include/gtest/internal/gtest-port-arch.h
--rw-r--r--   0        0        0    95013 2023-07-05 20:19:20.941378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/include/gtest/internal/gtest-port.h
--rw-r--r--   0        0        0     6907 2023-07-05 20:19:20.941378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/include/gtest/internal/gtest-string.h
--rw-r--r--   0        0        0    28617 2023-07-05 20:19:20.941378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/include/gtest/internal/gtest-tuple.h
--rw-r--r--   0        0        0     9620 2023-07-05 20:19:20.941378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/include/gtest/internal/gtest-tuple.h.pump
--rw-r--r--   0        0        0   186354 2023-07-05 20:19:20.941378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/include/gtest/internal/gtest-type-util.h
--rw-r--r--   0        0        0    10005 2023-07-05 20:19:20.941378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/include/gtest/internal/gtest-type-util.h.pump
--rw-r--r--   0        0        0    13302 2023-07-05 20:19:20.941378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/m4/acx_pthread.m4
--rw-r--r--   0        0        0     3217 2023-07-05 20:19:20.941378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/m4/gtest.m4
--rw-r--r--   0        0        0     2753 2023-07-05 20:19:20.941378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/make/Makefile
--rw-r--r--   0        0        0     3491 2023-07-05 20:19:20.941378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/msvc/2010/gtest-md.sln
--rw-r--r--   0        0        0     8417 2023-07-05 20:19:20.941378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/msvc/2010/gtest-md.vcxproj
--rw-r--r--   0        0        0      691 2023-07-05 20:19:20.941378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/msvc/2010/gtest-md.vcxproj.filters
--rw-r--r--   0        0        0     3467 2023-07-05 20:19:20.941378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/msvc/2010/gtest.sln
--rw-r--r--   0        0        0     8425 2023-07-05 20:19:20.941378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/msvc/2010/gtest.vcxproj
--rw-r--r--   0        0        0      691 2023-07-05 20:19:20.941378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/msvc/2010/gtest.vcxproj.filters
--rw-r--r--   0        0        0     8605 2023-07-05 20:19:20.941378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/msvc/2010/gtest_main-md.vcxproj
--rw-r--r--   0        0        0      692 2023-07-05 20:19:20.941378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/msvc/2010/gtest_main-md.vcxproj.filters
--rw-r--r--   0        0        0     8884 2023-07-05 20:19:20.941378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/msvc/2010/gtest_main.vcxproj
--rw-r--r--   0        0        0      692 2023-07-05 20:19:20.941378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/msvc/2010/gtest_main.vcxproj.filters
--rw-r--r--   0        0        0    11669 2023-07-05 20:19:20.941378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/msvc/2010/gtest_prod_test-md.vcxproj
--rw-r--r--   0        0        0      934 2023-07-05 20:19:20.941378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/msvc/2010/gtest_prod_test-md.vcxproj.filters
--rw-r--r--   0        0        0    11302 2023-07-05 20:19:20.941378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/msvc/2010/gtest_prod_test.vcxproj
--rw-r--r--   0        0        0      934 2023-07-05 20:19:20.941378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/msvc/2010/gtest_prod_test.vcxproj.filters
--rw-r--r--   0        0        0    11067 2023-07-05 20:19:20.941378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/msvc/2010/gtest_unittest-md.vcxproj
--rw-r--r--   0        0        0      697 2023-07-05 20:19:20.941378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/msvc/2010/gtest_unittest-md.vcxproj.filters
--rw-r--r--   0        0        0    10704 2023-07-05 20:19:20.941378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/msvc/2010/gtest_unittest.vcxproj
--rw-r--r--   0        0        0      697 2023-07-05 20:19:20.941378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/msvc/2010/gtest_unittest.vcxproj.filters
--rw-r--r--   0        0        0     4294 2023-07-05 20:19:20.941378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/samples/prime_tables.h
--rw-r--r--   0        0        0     2503 2023-07-05 20:19:20.941378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/samples/sample1.cc
--rw-r--r--   0        0        0     1937 2023-07-05 20:19:20.941378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/samples/sample1.h
--rw-r--r--   0        0        0     5023 2023-07-05 20:19:20.941378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/samples/sample10_unittest.cc
--rw-r--r--   0        0        0     5156 2023-07-05 20:19:20.941378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/samples/sample1_unittest.cc
--rw-r--r--   0        0        0     2298 2023-07-05 20:19:20.941378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/samples/sample2.cc
--rw-r--r--   0        0        0     3006 2023-07-05 20:19:20.941378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/samples/sample2.h
--rw-r--r--   0        0        0     3953 2023-07-05 20:19:20.941378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/samples/sample2_unittest.cc
--rw-r--r--   0        0        0     5365 2023-07-05 20:19:20.941378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/samples/sample3-inl.h
--rw-r--r--   0        0        0     5398 2023-07-05 20:19:20.941378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/samples/sample3_unittest.cc
--rw-r--r--   0        0        0     1927 2023-07-05 20:19:20.941378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/samples/sample4.cc
--rw-r--r--   0        0        0     2083 2023-07-05 20:19:20.941378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/samples/sample4.h
--rw-r--r--   0        0        0     1939 2023-07-05 20:19:20.941378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/samples/sample4_unittest.cc
--rw-r--r--   0        0        0     6616 2023-07-05 20:19:20.941378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/samples/sample5_unittest.cc
--rw-r--r--   0        0        0     9016 2023-07-05 20:19:20.941378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/samples/sample6_unittest.cc
--rw-r--r--   0        0        0     4654 2023-07-05 20:19:20.941378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/samples/sample7_unittest.cc
--rw-r--r--   0        0        0     6968 2023-07-05 20:19:20.941378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/samples/sample8_unittest.cc
--rw-r--r--   0        0        0     5948 2023-07-05 20:19:20.941378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/samples/sample9_unittest.cc
--rw-r--r--   0        0        0     2919 2023-07-05 20:19:20.941378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/scripts/common.py
--rwxr-xr-x   0        0        0     8896 2023-07-05 20:19:20.941378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/scripts/fuse_gtest_files.py
--rwxr-xr-x   0        0        0    21850 2023-07-05 20:19:20.941378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/scripts/gen_gtest_pred_impl.py
--rwxr-xr-x   0        0        0    10087 2023-07-05 20:19:20.941378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/scripts/gtest-config.in
--rwxr-xr-x   0        0        0    23673 2023-07-05 20:19:20.941378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/scripts/pump.py
--rwxr-xr-x   0        0        0     6132 2023-07-05 20:19:20.941378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/scripts/release_docs.py
--rw-r--r--   0        0        0     1802 2023-07-05 20:19:20.941378 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/scripts/test/Makefile
--rwxr-xr-x   0        0        0    51025 2023-07-05 20:19:20.945379 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/scripts/upload.py
--rwxr-xr-x   0        0        0     2851 2023-07-05 20:19:20.945379 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/scripts/upload_gtest.py
--rw-r--r--   0        0        0     2173 2023-07-05 20:19:20.945379 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/src/gtest-all.cc
--rw-r--r--   0        0        0    56716 2023-07-05 20:19:20.945379 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/src/gtest-death-test.cc
--rw-r--r--   0        0        0    14507 2023-07-05 20:19:20.945379 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/src/gtest-filepath.cc
--rw-r--r--   0        0        0    45140 2023-07-05 20:19:20.945379 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/src/gtest-internal-inl.h
--rw-r--r--   0        0        0    43284 2023-07-05 20:19:20.945379 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/src/gtest-port.cc
--rw-r--r--   0        0        0    15205 2023-07-05 20:19:20.945379 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/src/gtest-printers.cc
--rw-r--r--   0        0        0     3831 2023-07-05 20:19:20.945379 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/src/gtest-test-part.cc
--rw-r--r--   0        0        0     3961 2023-07-05 20:19:20.945379 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/src/gtest-typed-test.cc
--rw-r--r--   0        0        0   213031 2023-07-05 20:19:20.945379 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/src/gtest.cc
--rw-r--r--   0        0        0     1767 2023-07-05 20:19:20.945379 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/src/gtest_main.cc
--rw-r--r--   0        0        0     9762 2023-07-05 20:19:20.945379 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/BUILD.bazel
--rw-r--r--   0        0        0     3679 2023-07-05 20:19:20.945379 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest-death-test_ex_test.cc
--rw-r--r--   0        0        0    44749 2023-07-05 20:19:20.949379 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest-death-test_test.cc
--rw-r--r--   0        0        0    22712 2023-07-05 20:19:20.949379 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest-filepath_test.cc
--rw-r--r--   0        0        0     4125 2023-07-05 20:19:20.949379 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest-linked_ptr_test.cc
--rw-r--r--   0        0        0     9844 2023-07-05 20:19:20.949379 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest-listener_test.cc
--rw-r--r--   0        0        0     5302 2023-07-05 20:19:20.949379 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest-message_test.cc
--rw-r--r--   0        0        0     7672 2023-07-05 20:19:20.949379 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest-options_test.cc
--rw-r--r--   0        0        0     2820 2023-07-05 20:19:20.949379 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest-param-test2_test.cc
--rw-r--r--   0        0        0    40385 2023-07-05 20:19:20.949379 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest-param-test_test.cc
--rw-r--r--   0        0        0     2296 2023-07-05 20:19:20.949379 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest-param-test_test.h
--rw-r--r--   0        0        0    40423 2023-07-05 20:19:20.949379 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest-port_test.cc
--rw-r--r--   0        0        0    56551 2023-07-05 20:19:20.949379 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest-printers_test.cc
--rw-r--r--   0        0        0     7282 2023-07-05 20:19:20.949379 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest-test-part_test.cc
--rw-r--r--   0        0        0     9250 2023-07-05 20:19:20.949379 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest-tuple_test.cc
--rw-r--r--   0        0        0     2054 2023-07-05 20:19:20.949379 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest-typed-test2_test.cc
--rw-r--r--   0        0        0    12330 2023-07-05 20:19:20.949379 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest-typed-test_test.cc
--rw-r--r--   0        0        0     2485 2023-07-05 20:19:20.949379 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest-typed-test_test.h
--rw-r--r--   0        0        0    13207 2023-07-05 20:19:20.949379 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest-unittest-api_test.cc
--rw-r--r--   0        0        0     2203 2023-07-05 20:19:20.949379 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_all_test.cc
--rw-r--r--   0        0        0     3946 2023-07-05 20:19:20.949379 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_assert_by_exception_test.cc
--rwxr-xr-x   0        0        0     7327 2023-07-05 20:19:20.949379 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_break_on_failure_unittest.py
--rw-r--r--   0        0        0     3283 2023-07-05 20:19:20.949379 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_break_on_failure_unittest_.cc
--rwxr-xr-x   0        0        0     9890 2023-07-05 20:19:20.949379 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_catch_exceptions_test.py
--rw-r--r--   0        0        0     8874 2023-07-05 20:19:20.949379 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_catch_exceptions_test_.cc
--rwxr-xr-x   0        0        0     4911 2023-07-05 20:19:20.949379 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_color_test.py
--rw-r--r--   0        0        0     2548 2023-07-05 20:19:20.949379 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_color_test_.cc
--rwxr-xr-x   0        0        0     4038 2023-07-05 20:19:20.949379 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_env_var_test.py
--rw-r--r--   0        0        0     3515 2023-07-05 20:19:20.949379 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_env_var_test_.cc
--rw-r--r--   0        0        0     6508 2023-07-05 20:19:20.949379 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_environment_test.cc
--rwxr-xr-x   0        0        0    21397 2023-07-05 20:19:20.949379 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_filter_unittest.py
--rw-r--r--   0        0        0     3507 2023-07-05 20:19:20.949379 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_filter_unittest_.cc
--rwxr-xr-x   0        0        0     5868 2023-07-05 20:19:20.949379 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_help_test.py
--rw-r--r--   0        0        0     2131 2023-07-05 20:19:20.949379 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_help_test_.cc
--rw-r--r--   0        0        0     5527 2023-07-05 20:19:20.949379 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_json_outfiles_test.py
--rw-r--r--   0        0        0    20882 2023-07-05 20:19:20.949379 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_json_output_unittest.py
--rw-r--r--   0        0        0     2411 2023-07-05 20:19:20.949379 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_json_test_utils.py
--rwxr-xr-x   0        0        0     6537 2023-07-05 20:19:20.949379 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_list_tests_unittest.py
--rw-r--r--   0        0        0     4710 2023-07-05 20:19:20.949379 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_list_tests_unittest_.cc
--rw-r--r--   0        0        0     1884 2023-07-05 20:19:20.949379 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_main_unittest.cc
--rw-r--r--   0        0        0     2447 2023-07-05 20:19:20.949379 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_no_test_unittest.cc
--rwxr-xr-x   0        0        0    12437 2023-07-05 20:19:20.949379 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_output_test.py
--rw-r--r--   0        0        0    33338 2023-07-05 20:19:20.949379 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_output_test_.cc
--rw-r--r--   0        0        0    30233 2023-07-05 20:19:20.949379 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_output_test_golden_lin.txt
--rw-r--r--   0        0        0    77378 2023-07-05 20:19:20.949379 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_pred_impl_unittest.cc
--rw-r--r--   0        0        0     4298 2023-07-05 20:19:20.949379 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_premature_exit_test.cc
--rw-r--r--   0        0        0     2196 2023-07-05 20:19:20.949379 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_prod_test.cc
--rw-r--r--   0        0        0     7571 2023-07-05 20:19:20.949379 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_repeat_test.cc
--rwxr-xr-x   0        0        0    12549 2023-07-05 20:19:20.949379 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_shuffle_test.py
--rw-r--r--   0        0        0     3306 2023-07-05 20:19:20.949379 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_shuffle_test_.cc
--rw-r--r--   0        0        0     2221 2023-07-05 20:19:20.949379 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_sole_header_test.cc
--rw-r--r--   0        0        0     9381 2023-07-05 20:19:20.949379 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_stress_test.cc
--rwxr-xr-x   0        0        0    10825 2023-07-05 20:19:20.953379 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_test_utils.py
--rw-r--r--   0        0        0     2520 2023-07-05 20:19:20.953379 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_testbridge_test.py
--rw-r--r--   0        0        0     1965 2023-07-05 20:19:20.953379 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_testbridge_test_.cc
--rw-r--r--   0        0        0     3444 2023-07-05 20:19:20.953379 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_throw_on_failure_ex_test.cc
--rwxr-xr-x   0        0        0     5766 2023-07-05 20:19:20.953379 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_throw_on_failure_test.py
--rw-r--r--   0        0        0     3104 2023-07-05 20:19:20.953379 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_throw_on_failure_test_.cc
--rwxr-xr-x   0        0        0     2513 2023-07-05 20:19:20.953379 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_uninitialized_test.py
--rw-r--r--   0        0        0     1921 2023-07-05 20:19:20.953379 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_uninitialized_test_.cc
--rw-r--r--   0        0        0   251334 2023-07-05 20:19:20.953379 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_unittest.cc
--rw-r--r--   0        0        0     1968 2023-07-05 20:19:20.953379 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_xml_outfile1_test_.cc
--rw-r--r--   0        0        0     1968 2023-07-05 20:19:20.953379 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_xml_outfile2_test_.cc
--rwxr-xr-x   0        0        0     5593 2023-07-05 20:19:20.953379 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_xml_outfiles_test.py
--rwxr-xr-x   0        0        0    17080 2023-07-05 20:19:20.953379 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_xml_output_unittest.py
--rw-r--r--   0        0        0     6100 2023-07-05 20:19:20.953379 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_xml_output_unittest_.cc
--rwxr-xr-x   0        0        0     9221 2023-07-05 20:19:20.953379 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_xml_test_utils.py
--rw-r--r--   0        0        0     1718 2023-07-05 20:19:20.953379 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/production.cc
--rw-r--r--   0        0        0     2158 2023-07-05 20:19:20.953379 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/production.h
--rw-r--r--   0        0        0      983 2023-07-05 20:19:20.953379 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/xcode/Config/DebugProject.xcconfig
--rw-r--r--   0        0        0      551 2023-07-05 20:19:20.953379 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/xcode/Config/FrameworkTarget.xcconfig
--rw-r--r--   0        0        0     1199 2023-07-05 20:19:20.953379 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/xcode/Config/General.xcconfig
--rw-r--r--   0        0        0      993 2023-07-05 20:19:20.953379 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/xcode/Config/ReleaseProject.xcconfig
--rw-r--r--   0        0        0      587 2023-07-05 20:19:20.953379 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/xcode/Config/StaticLibraryTarget.xcconfig
--rw-r--r--   0        0        0      238 2023-07-05 20:19:20.953379 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/xcode/Config/TestTarget.xcconfig
--rw-r--r--   0        0        0     1010 2023-07-05 20:19:20.953379 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/xcode/Resources/Info.plist
--rw-r--r--   0        0        0      846 2023-07-05 20:19:20.953379 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/xcode/Samples/FrameworkSample/Info.plist
--rw-r--r--   0        0        0    16060 2023-07-05 20:19:20.953379 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/xcode/Samples/FrameworkSample/WidgetFramework.xcodeproj/project.pbxproj
--rw-r--r--   0        0        0     2354 2023-07-05 20:19:20.953379 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/xcode/Samples/FrameworkSample/runtests.sh
--rw-r--r--   0        0        0     2307 2023-07-05 20:19:20.953379 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/xcode/Samples/FrameworkSample/widget.cc
--rw-r--r--   0        0        0     2270 2023-07-05 20:19:20.953379 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/xcode/Samples/FrameworkSample/widget.h
--rw-r--r--   0        0        0     2669 2023-07-05 20:19:20.953379 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/xcode/Samples/FrameworkSample/widget_test.cc
--rw-r--r--   0        0        0     2587 2023-07-05 20:19:20.953379 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/xcode/Scripts/runtests.sh
--rwxr-xr-x   0        0        0     4535 2023-07-05 20:19:20.953379 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/xcode/Scripts/versiongenerate.py
--rw-r--r--   0        0        0    54223 2023-07-05 20:19:20.953379 cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/xcode/gtest.xcodeproj/project.pbxproj
--rwxr-xr-x   0        0        0     3294 2023-07-05 20:19:19.053353 cornflakes-3.3.7/inst/ext/rapidjson/travis-doxygen.sh
--rw-r--r--   0        0        0       45 2023-07-05 20:19:17.565333 cornflakes-3.3.7/inst/ext/strtk/.git
--rw-r--r--   0        0        0      347 2023-07-05 20:19:20.965379 cornflakes-3.3.7/inst/ext/strtk/.travis.yml
--rw-r--r--   0        0        0     7507 2023-07-05 20:19:20.965379 cornflakes-3.3.7/inst/ext/strtk/Makefile
--rw-r--r--   0        0        0     3590 2023-07-05 20:19:20.965379 cornflakes-3.3.7/inst/ext/strtk/readme.txt
--rw-r--r--   0        0        0   885153 2023-07-05 20:19:20.969379 cornflakes-3.3.7/inst/ext/strtk/strtk.hpp
--rw-r--r--   0        0        0     7614 2023-07-05 20:19:20.969379 cornflakes-3.3.7/inst/ext/strtk/strtk_bloom_filter_example.cpp
--rw-r--r--   0        0        0     2568 2023-07-05 20:19:20.969379 cornflakes-3.3.7/inst/ext/strtk/strtk_combinations.cpp
--rw-r--r--   0        0        0     2101 2023-07-05 20:19:20.969379 cornflakes-3.3.7/inst/ext/strtk/strtk_combinator_example.cpp
--rw-r--r--   0        0        0     5881 2023-07-05 20:19:20.969379 cornflakes-3.3.7/inst/ext/strtk/strtk_converters_example.cpp
--rw-r--r--   0        0        0    72459 2023-07-05 20:19:20.969379 cornflakes-3.3.7/inst/ext/strtk/strtk_examples.cpp
--rw-r--r--   0        0        0     3988 2023-07-05 20:19:20.969379 cornflakes-3.3.7/inst/ext/strtk/strtk_glober.cpp
--rw-r--r--   0        0        0     4339 2023-07-05 20:19:20.969379 cornflakes-3.3.7/inst/ext/strtk/strtk_hexview.cpp
--rw-r--r--   0        0        0     3730 2023-07-05 20:19:20.969379 cornflakes-3.3.7/inst/ext/strtk/strtk_ipv4_parser.cpp
--rw-r--r--   0        0        0    14409 2023-07-05 20:19:20.969379 cornflakes-3.3.7/inst/ext/strtk/strtk_keyvalue_example.cpp
--rw-r--r--   0        0        0     4938 2023-07-05 20:19:20.969379 cornflakes-3.3.7/inst/ext/strtk/strtk_nth_combination_example.cpp
--rw-r--r--   0        0        0     4843 2023-07-05 20:19:20.969379 cornflakes-3.3.7/inst/ext/strtk/strtk_numstats.cpp
--rw-r--r--   0        0        0    27214 2023-07-05 20:19:20.969379 cornflakes-3.3.7/inst/ext/strtk/strtk_parse_test.cpp
--rw-r--r--   0        0        0     5133 2023-07-05 20:19:20.969379 cornflakes-3.3.7/inst/ext/strtk/strtk_period_parser.cpp
--rw-r--r--   0        0        0     2547 2023-07-05 20:19:20.969379 cornflakes-3.3.7/inst/ext/strtk/strtk_random_line.cpp
--rw-r--r--   0        0        0     2372 2023-07-05 20:19:20.969379 cornflakes-3.3.7/inst/ext/strtk/strtk_randomizer.cpp
--rw-r--r--   0        0        0     6261 2023-07-05 20:19:20.969379 cornflakes-3.3.7/inst/ext/strtk/strtk_search_trie_example.cpp
--rw-r--r--   0        0        0    32474 2023-07-05 20:19:20.969379 cornflakes-3.3.7/inst/ext/strtk/strtk_serializer_example.cpp
--rw-r--r--   0        0        0     2364 2023-07-05 20:19:20.969379 cornflakes-3.3.7/inst/ext/strtk/strtk_text_parser_example01.cpp
--rw-r--r--   0        0        0     3811 2023-07-05 20:19:20.969379 cornflakes-3.3.7/inst/ext/strtk/strtk_text_parser_example02.cpp
--rw-r--r--   0        0        0    31242 2023-07-05 20:19:20.969379 cornflakes-3.3.7/inst/ext/strtk/strtk_tokengrid_example.cpp
--rw-r--r--   0        0        0    52321 2023-07-05 20:19:20.969379 cornflakes-3.3.7/inst/ext/strtk/strtk_tokenizer_cmp.cpp
--rw-r--r--   0        0        0   131409 2023-07-05 20:19:20.969379 cornflakes-3.3.7/inst/ext/strtk/strtk_tokenizer_test.cpp
--rw-r--r--   0        0        0     4174 2023-07-05 20:19:20.969379 cornflakes-3.3.7/inst/ext/strtk/strtk_wordfreq.cpp
--rw-r--r--   0        0        0     4528 2023-07-05 20:19:15.781308 cornflakes-3.3.7/pyproject.toml
--rw-r--r--   0        0        0     5586 1970-01-01 00:00:00.000000 cornflakes-3.3.7/setup.py
--rw-r--r--   0        0        0     5055 1970-01-01 00:00:00.000000 cornflakes-3.3.7/PKG-INFO
+-rwxr-xr-x   0        0        0    11310 2023-07-20 13:04:19.735167 cornflakes-3.3.8/LICENSE
+-rwxr-xr-x   0        0        0     4787 2023-07-20 13:04:19.735167 cornflakes-3.3.8/README.rst
+-rwxr-xr-x   0        0        0     1945 2023-07-20 13:04:19.735167 cornflakes-3.3.8/build.py
+-rwxr-xr-x   0        0        0      705 2023-07-20 13:04:19.735167 cornflakes-3.3.8/cornflakes/__init__.py
+-rwxr-xr-x   0        0        0      116 2023-07-20 13:04:19.735167 cornflakes-3.3.8/cornflakes/__main__.py
+-rwxr-xr-x   0        0        0      251 2023-07-20 13:04:19.735167 cornflakes-3.3.8/cornflakes/builder/__init__.py
+-rwxr-xr-x   0        0        0     4515 2023-07-20 13:04:19.735167 cornflakes-3.3.8/cornflakes/builder/_generate_config_module.py
+-rw-r--r--   0        0        0     2580 2023-07-20 13:04:19.735167 cornflakes-3.3.8/cornflakes/builder/_generate_enum_module.py
+-rw-r--r--   0        0        0     2583 2023-07-20 13:04:19.735167 cornflakes-3.3.8/cornflakes/cli/__init__.py
+-rwxr-xr-x   0        0        0      793 2023-07-20 13:04:19.735167 cornflakes-3.3.8/cornflakes/common/__init__.py
+-rw-r--r--   0        0        0     6071 2023-07-20 13:04:19.735167 cornflakes-3.3.8/cornflakes/common/_check_type.py
+-rw-r--r--   0        0        0     2663 2023-07-20 13:04:19.735167 cornflakes-3.3.8/cornflakes/common/_datetime_ms.py
+-rwxr-xr-x   0        0        0     1583 2023-07-20 13:04:19.735167 cornflakes-3.3.8/cornflakes/common/_default_ca_path.py
+-rwxr-xr-x   0        0        0      250 2023-07-20 13:04:19.735167 cornflakes-3.3.8/cornflakes/common/_extract_var_names.py
+-rw-r--r--   0        0        0     2583 2023-07-20 13:04:19.735167 cornflakes-3.3.8/cornflakes/common/_patch_module.py
+-rw-r--r--   0        0        0      469 2023-07-20 13:04:19.735167 cornflakes-3.3.8/cornflakes/common/_recursive_update.py
+-rwxr-xr-x   0        0        0      817 2023-07-20 13:04:19.735167 cornflakes-3.3.8/cornflakes/common/_type_to_str.py
+-rw-r--r--   0        0        0      347 2023-07-20 13:04:19.735167 cornflakes-3.3.8/cornflakes/common/_unquoted_string.py
+-rwxr-xr-x   0        0        0      606 2023-07-20 13:04:19.735167 cornflakes-3.3.8/cornflakes/decorator/__init__.py
+-rw-r--r--   0        0        0      872 2023-07-20 13:04:19.735167 cornflakes-3.3.8/cornflakes/decorator/_funcat.py
+-rw-r--r--   0        0        0     3146 2023-07-20 13:04:19.735167 cornflakes-3.3.8/cornflakes/decorator/_indexer.py
+-rw-r--r--   0        0        0     6555 2023-07-20 13:04:19.735167 cornflakes-3.3.8/cornflakes/decorator/_wrap_kwargs.py
+-rw-r--r--   0        0        0      395 2023-07-20 13:04:19.735167 cornflakes-3.3.8/cornflakes/decorator/_wrap_partial.py
+-rwxr-xr-x   0        0        0      677 2023-07-20 13:04:19.735167 cornflakes-3.3.8/cornflakes/decorator/click/__init__.py
+-rwxr-xr-x   0        0        0     3418 2023-07-20 13:04:19.735167 cornflakes-3.3.8/cornflakes/decorator/click/_click_cli.py
+-rw-r--r--   0        0        0      278 2023-07-20 13:04:19.735167 cornflakes-3.3.8/cornflakes/decorator/click/helper/__init__.py
+-rw-r--r--   0        0        0     1524 2023-07-20 13:04:19.735167 cornflakes-3.3.8/cornflakes/decorator/click/helper/_click_param_type_parser.py
+-rw-r--r--   0        0        0      317 2023-07-20 13:04:19.735167 cornflakes-3.3.8/cornflakes/decorator/click/helper/_get_command_name.py
+-rwxr-xr-x   0        0        0      606 2023-07-20 13:04:19.735167 cornflakes-3.3.8/cornflakes/decorator/click/options/__init__.py
+-rw-r--r--   0        0        0      933 2023-07-20 13:04:19.735167 cornflakes-3.3.8/cornflakes/decorator/click/options/_auto_fill_option_groups.py
+-rwxr-xr-x   0        0        0     1338 2023-07-20 13:04:19.735167 cornflakes-3.3.8/cornflakes/decorator/click/options/_bg_process.py
+-rwxr-xr-x   0        0        0     9411 2023-07-20 13:04:19.735167 cornflakes-3.3.8/cornflakes/decorator/click/options/_config_option.py
+-rwxr-xr-x   0        0        0      593 2023-07-20 13:04:19.735167 cornflakes-3.3.8/cornflakes/decorator/click/options/_global.py
+-rwxr-xr-x   0        0        0      849 2023-07-20 13:04:19.735167 cornflakes-3.3.8/cornflakes/decorator/click/options/_verbose.py
+-rwxr-xr-x   0        0        0     2642 2023-07-20 13:04:19.735167 cornflakes-3.3.8/cornflakes/decorator/click/rich/__init__.py
+-rwxr-xr-x   0        0        0      385 2023-07-20 13:04:19.735167 cornflakes-3.3.8/cornflakes/decorator/click/rich/_rich_argument.py
+-rwxr-xr-x   0        0        0    23605 2023-07-20 13:04:19.735167 cornflakes-3.3.8/cornflakes/decorator/click/rich/_rich_click.py
+-rwxr-xr-x   0        0        0     1968 2023-07-20 13:04:19.735167 cornflakes-3.3.8/cornflakes/decorator/click/rich/_rich_command.py
+-rwxr-xr-x   0        0        0     5319 2023-07-20 13:04:19.735167 cornflakes-3.3.8/cornflakes/decorator/click/rich/_rich_config.py
+-rwxr-xr-x   0        0        0     6004 2023-07-20 13:04:19.735167 cornflakes-3.3.8/cornflakes/decorator/click/rich/_rich_global_option_wrapper.py
+-rwxr-xr-x   0        0        0     3581 2023-07-20 13:04:19.735167 cornflakes-3.3.8/cornflakes/decorator/click/rich/_rich_group.py
+-rw-r--r--   0        0        0     1197 2023-07-20 13:04:19.735167 cornflakes-3.3.8/cornflakes/decorator/dataclasses/__init__.py
+-rwxr-xr-x   0        0        0     1065 2023-07-20 13:04:19.735167 cornflakes-3.3.8/cornflakes/decorator/dataclasses/_add_dataclass_slots.py
+-rwxr-xr-x   0        0        0    14187 2023-07-20 13:04:19.735167 cornflakes-3.3.8/cornflakes/decorator/dataclasses/_dataclass.py
+-rwxr-xr-x   0        0        0     1089 2023-07-20 13:04:19.735167 cornflakes-3.3.8/cornflakes/decorator/dataclasses/_enforce_types.py
+-rwxr-xr-x   0        0        0    19310 2023-07-20 13:04:19.735167 cornflakes-3.3.8/cornflakes/decorator/dataclasses/_field.py
+-rwxr-xr-x   0        0        0     4939 2023-07-20 13:04:19.735167 cornflakes-3.3.8/cornflakes/decorator/dataclasses/_helper.py
+-rw-r--r--   0        0        0     2798 2023-07-20 13:04:19.735167 cornflakes-3.3.8/cornflakes/decorator/dataclasses/_validate.py
+-rwxr-xr-x   0        0        0      439 2023-07-20 13:04:19.735167 cornflakes-3.3.8/cornflakes/decorator/dataclasses/config/__init__.py
+-rwxr-xr-x   0        0        0    11889 2023-07-20 13:04:19.739167 cornflakes-3.3.8/cornflakes/decorator/dataclasses/config/_config.py
+-rwxr-xr-x   0        0        0     5651 2023-07-20 13:04:19.739167 cornflakes-3.3.8/cornflakes/decorator/dataclasses/config/_config_group.py
+-rwxr-xr-x   0        0        0      914 2023-07-20 13:04:19.739167 cornflakes-3.3.8/cornflakes/decorator/dataclasses/config/_dict.py
+-rwxr-xr-x   0        0        0     3737 2023-07-20 13:04:19.739167 cornflakes-3.3.8/cornflakes/decorator/dataclasses/config/_ini.py
+-rw-r--r--   0        0        0     4369 2023-07-20 13:04:19.739167 cornflakes-3.3.8/cornflakes/decorator/dataclasses/config/_init_config.py
+-rw-r--r--   0        0        0     3220 2023-07-20 13:04:19.739167 cornflakes-3.3.8/cornflakes/decorator/dataclasses/config/_init_config_group.py
+-rwxr-xr-x   0        0        0     7538 2023-07-20 13:04:19.739167 cornflakes-3.3.8/cornflakes/decorator/dataclasses/config/_load_config.py
+-rwxr-xr-x   0        0        0     2358 2023-07-20 13:04:19.739167 cornflakes-3.3.8/cornflakes/decorator/dataclasses/config/_load_config_group.py
+-rwxr-xr-x   0        0        0      350 2023-07-20 13:04:19.739167 cornflakes-3.3.8/cornflakes/decorator/dataclasses/config/_write_config.py
+-rwxr-xr-x   0        0        0     1722 2023-07-20 13:04:19.739167 cornflakes-3.3.8/cornflakes/decorator/dataclasses/config/_yaml.py
+-rw-r--r--   0        0        0      143 2023-07-20 13:04:19.739167 cornflakes-3.3.8/cornflakes/decorator/dataclasses/validator/__init__.py
+-rw-r--r--   0        0        0    24723 2023-07-20 13:04:19.739167 cornflakes-3.3.8/cornflakes/decorator/dataclasses/validator/url.py
+-rw-r--r--   0        0        0      181 2023-07-20 13:04:19.739167 cornflakes-3.3.8/cornflakes/decorator/datalite/__init__.py
+-rw-r--r--   0        0        0     8350 2023-07-20 13:04:19.739167 cornflakes-3.3.8/cornflakes/decorator/datalite/commons.py
+-rw-r--r--   0        0        0      555 2023-07-20 13:04:19.739167 cornflakes-3.3.8/cornflakes/decorator/datalite/constraints.py
+-rw-r--r--   0        0        0     3820 2023-07-20 13:04:19.739167 cornflakes-3.3.8/cornflakes/decorator/datalite/datalite_decorator.py
+-rw-r--r--   0        0        0     6431 2023-07-20 13:04:19.739167 cornflakes-3.3.8/cornflakes/decorator/datalite/fetch.py
+-rw-r--r--   0        0        0     4652 2023-07-20 13:04:19.739167 cornflakes-3.3.8/cornflakes/decorator/datalite/mass_actions.py
+-rw-r--r--   0        0        0     6344 2023-07-20 13:04:19.739167 cornflakes-3.3.8/cornflakes/decorator/datalite/migrations.py
+-rw-r--r--   0        0        0     1555 2023-07-20 13:04:19.739167 cornflakes-3.3.8/cornflakes/decorator/datalite/type_mapping.py
+-rw-r--r--   0        0        0     1854 2023-07-20 13:04:19.739167 cornflakes-3.3.8/cornflakes/decorator/string_builder.py
+-rwxr-xr-x   0        0        0      189 2023-07-20 13:04:19.739167 cornflakes-3.3.8/cornflakes/logging/__init__.py
+-rwxr-xr-x   0        0        0     6374 2023-07-20 13:04:19.739167 cornflakes-3.3.8/cornflakes/logging/logger.py
+-rw-r--r--   0        0        0      207 2023-07-20 13:04:19.739167 cornflakes-3.3.8/cornflakes/packaging/__init__.py
+-rw-r--r--   0        0        0     2473 2023-07-20 13:04:19.739167 cornflakes-3.3.8/cornflakes/packaging/bump_version.py
+-rw-r--r--   0        0        0     2786 2023-07-20 13:04:19.739167 cornflakes-3.3.8/cornflakes/packaging/update_deps.py
+-rwxr-xr-x   0        0        0      110 2023-07-20 13:04:19.739167 cornflakes-3.3.8/cornflakes/parser/__init__.py
+-rwxr-xr-x   0        0        0     4970 2023-07-20 13:04:19.739167 cornflakes-3.3.8/cornflakes/parser/_yaml.py
+-rw-r--r--   0        0        0       57 2023-07-20 13:04:19.739167 cornflakes-3.3.8/cornflakes/py.typed
+-rwxr-xr-x   0        0        0     9980 2023-07-20 13:04:19.739167 cornflakes-3.3.8/cornflakes/types.py
+-rw-r--r--   0        0        0     6261 2023-07-20 13:04:19.739167 cornflakes-3.3.8/inst/_cornflakes/bindings.cpp
+-rw-r--r--   0        0        0      422 2023-07-20 13:04:19.739167 cornflakes-3.3.8/inst/_cornflakes/bindings.hpp
+-rw-r--r--   0        0        0     3914 2023-07-20 13:04:19.739167 cornflakes-3.3.8/inst/_cornflakes/cross_endian.h
+-rwxr-xr-x   0        0        0   129827 2023-07-20 13:04:19.739167 cornflakes-3.3.8/inst/_cornflakes/datetime_utils.hpp
+-rwxr-xr-x   0        0        0     2667 2023-07-20 13:04:19.739167 cornflakes-3.3.8/inst/_cornflakes/digest.cpp
+-rw-r--r--   0        0        0      805 2023-07-20 13:04:19.739167 cornflakes-3.3.8/inst/_cornflakes/digest.hpp
+-rw-r--r--   0        0        0    18739 2023-07-20 13:04:19.739167 cornflakes-3.3.8/inst/_cornflakes/ini.cpp
+-rw-r--r--   0        0        0     1032 2023-07-20 13:04:19.739167 cornflakes-3.3.8/inst/_cornflakes/ini.hpp
+-rw-r--r--   0        0        0    28105 2023-07-20 13:04:19.739167 cornflakes-3.3.8/inst/_cornflakes/string_operations.cpp
+-rw-r--r--   0        0        0     9263 2023-07-20 13:04:19.739167 cornflakes-3.3.8/inst/_cornflakes/string_operations.hpp
+-rw-r--r--   0        0        0     2825 2023-07-20 13:04:19.739167 cornflakes-3.3.8/inst/_cornflakes/system_operations.cpp
+-rwxr-xr-x   0        0        0     1201 2023-07-20 13:04:19.739167 cornflakes-3.3.8/inst/_cornflakes/system_operations.hpp
+-rw-r--r--   0        0        0       52 2023-07-20 13:04:20.243174 cornflakes-3.3.8/inst/ext/hash-library/.git
+-rw-r--r--   0        0        0      861 2023-07-20 13:04:22.327205 cornflakes-3.3.8/inst/ext/hash-library/LICENSE
+-rw-r--r--   0        0        0    29030 2023-07-20 13:04:22.327205 cornflakes-3.3.8/inst/ext/hash-library/crc32.cpp
+-rw-r--r--   0        0        0     1736 2023-07-20 13:04:22.327205 cornflakes-3.3.8/inst/ext/hash-library/crc32.h
+-rw-r--r--   0        0        0     3163 2023-07-20 13:04:22.327205 cornflakes-3.3.8/inst/ext/hash-library/digest.cpp
+-rw-r--r--   0        0        0      723 2023-07-20 13:04:22.327205 cornflakes-3.3.8/inst/ext/hash-library/hash.h
+-rw-r--r--   0        0        0     2726 2023-07-20 13:04:22.327205 cornflakes-3.3.8/inst/ext/hash-library/hmac.h
+-rw-r--r--   0        0        0     8204 2023-07-20 13:04:22.327205 cornflakes-3.3.8/inst/ext/hash-library/keccak.cpp
+-rw-r--r--   0        0        0     2103 2023-07-20 13:04:22.327205 cornflakes-3.3.8/inst/ext/hash-library/keccak.h
+-rw-r--r--   0        0        0    10806 2023-07-20 13:04:22.327205 cornflakes-3.3.8/inst/ext/hash-library/md5.cpp
+-rw-r--r--   0        0        0     1921 2023-07-20 13:04:22.327205 cornflakes-3.3.8/inst/ext/hash-library/md5.h
+-rw-r--r--   0        0        0     1758 2023-07-20 13:04:22.327205 cornflakes-3.3.8/inst/ext/hash-library/readme.md
+-rw-r--r--   0        0        0     8393 2023-07-20 13:04:22.327205 cornflakes-3.3.8/inst/ext/hash-library/sha1.cpp
+-rw-r--r--   0        0        0     1940 2023-07-20 13:04:22.327205 cornflakes-3.3.8/inst/ext/hash-library/sha1.h
+-rw-r--r--   0        0        0    14195 2023-07-20 13:04:22.327205 cornflakes-3.3.8/inst/ext/hash-library/sha256.cpp
+-rw-r--r--   0        0        0     1968 2023-07-20 13:04:22.327205 cornflakes-3.3.8/inst/ext/hash-library/sha256.h
+-rw-r--r--   0        0        0     8175 2023-07-20 13:04:22.327205 cornflakes-3.3.8/inst/ext/hash-library/sha3.cpp
+-rw-r--r--   0        0        0     2051 2023-07-20 13:04:22.327205 cornflakes-3.3.8/inst/ext/hash-library/sha3.h
+-rw-r--r--   0        0        0     1611 2023-07-20 13:04:22.327205 cornflakes-3.3.8/inst/ext/hash-library/tests/github-issue2.cpp
+-rw-r--r--   0        0        0      405 2023-07-20 13:04:22.327205 cornflakes-3.3.8/inst/ext/hash-library/tests/github-issue6.cpp
+-rw-r--r--   0        0        0    47981 2023-07-20 13:04:22.327205 cornflakes-3.3.8/inst/ext/hash-library/tests/tests.cpp
+-rw-r--r--   0        0        0     1271 2023-07-20 13:04:23.519224 cornflakes-3.3.8/inst/ext/pybind11/.appveyor.yml
+-rw-r--r--   0        0        0      996 2023-07-20 13:04:23.519224 cornflakes-3.3.8/inst/ext/pybind11/.clang-format
+-rw-r--r--   0        0        0     2605 2023-07-20 13:04:23.519224 cornflakes-3.3.8/inst/ext/pybind11/.clang-tidy
+-rw-r--r--   0        0        0     2196 2023-07-20 13:04:23.519224 cornflakes-3.3.8/inst/ext/pybind11/.cmake-format.yaml
+-rw-r--r--   0        0        0     1308 2023-07-20 13:04:23.519224 cornflakes-3.3.8/inst/ext/pybind11/.codespell-ignore-lines
+-rw-r--r--   0        0        0       48 2023-07-20 13:04:20.955185 cornflakes-3.3.8/inst/ext/pybind11/.git
+-rw-r--r--   0        0        0       18 2023-07-20 13:04:23.519224 cornflakes-3.3.8/inst/ext/pybind11/.gitattributes
+-rw-r--r--   0        0        0      182 2023-07-20 13:04:23.519224 cornflakes-3.3.8/inst/ext/pybind11/.github/CODEOWNERS
+-rw-r--r--   0        0        0    15284 2023-07-20 13:04:23.519224 cornflakes-3.3.8/inst/ext/pybind11/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0     2561 2023-07-20 13:04:23.519224 cornflakes-3.3.8/inst/ext/pybind11/.github/ISSUE_TEMPLATE/bug-report.yml
+-rw-r--r--   0        0        0      328 2023-07-20 13:04:23.519224 cornflakes-3.3.8/inst/ext/pybind11/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      162 2023-07-20 13:04:23.519224 cornflakes-3.3.8/inst/ext/pybind11/.github/dependabot.yml
+-rw-r--r--   0        0        0      116 2023-07-20 13:04:23.519224 cornflakes-3.3.8/inst/ext/pybind11/.github/labeler.yml
+-rw-r--r--   0        0        0       50 2023-07-20 13:04:23.519224 cornflakes-3.3.8/inst/ext/pybind11/.github/labeler_merged.yml
+-rw-r--r--   0        0        0      668 2023-07-20 13:04:23.519224 cornflakes-3.3.8/inst/ext/pybind11/.github/matchers/pylint.json
+-rw-r--r--   0        0        0      645 2023-07-20 13:04:23.519224 cornflakes-3.3.8/inst/ext/pybind11/.github/pull_request_template.md
+-rw-r--r--   0        0        0    32023 2023-07-20 13:04:23.519224 cornflakes-3.3.8/inst/ext/pybind11/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     2127 2023-07-20 13:04:23.519224 cornflakes-3.3.8/inst/ext/pybind11/.github/workflows/configure.yml
+-rw-r--r--   0        0        0     1460 2023-07-20 13:04:23.519224 cornflakes-3.3.8/inst/ext/pybind11/.github/workflows/format.yml
+-rw-r--r--   0        0        0      559 2023-07-20 13:04:23.519224 cornflakes-3.3.8/inst/ext/pybind11/.github/workflows/labeler.yml
+-rw-r--r--   0        0        0     2558 2023-07-20 13:04:23.519224 cornflakes-3.3.8/inst/ext/pybind11/.github/workflows/pip.yml
+-rw-r--r--   0        0        0     2865 2023-07-20 13:04:23.519224 cornflakes-3.3.8/inst/ext/pybind11/.github/workflows/upstream.yml
+-rw-r--r--   0        0        0      502 2023-07-20 13:04:23.519224 cornflakes-3.3.8/inst/ext/pybind11/.gitignore
+-rw-r--r--   0        0        0     3588 2023-07-20 13:04:23.519224 cornflakes-3.3.8/inst/ext/pybind11/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       62 2023-07-20 13:04:23.519224 cornflakes-3.3.8/inst/ext/pybind11/.readthedocs.yml
+-rw-r--r--   0        0        0    11983 2023-07-20 13:04:23.519224 cornflakes-3.3.8/inst/ext/pybind11/CMakeLists.txt
+-rw-r--r--   0        0        0     1684 2023-07-20 13:04:23.519224 cornflakes-3.3.8/inst/ext/pybind11/LICENSE
+-rw-r--r--   0        0        0      235 2023-07-20 13:04:23.519224 cornflakes-3.3.8/inst/ext/pybind11/MANIFEST.in
+-rw-r--r--   0        0        0     7686 2023-07-20 13:04:23.519224 cornflakes-3.3.8/inst/ext/pybind11/README.rst
+-rw-r--r--   0        0        0      607 2023-07-20 13:04:23.519224 cornflakes-3.3.8/inst/ext/pybind11/docs/Doxyfile
+-rw-r--r--   0        0        0     7417 2023-07-20 13:04:23.519224 cornflakes-3.3.8/inst/ext/pybind11/docs/Makefile
+-rw-r--r--   0        0        0       37 2023-07-20 13:04:23.519224 cornflakes-3.3.8/inst/ext/pybind11/docs/_static/css/custom.css
+-rw-r--r--   0        0        0     3937 2023-07-20 13:04:23.519224 cornflakes-3.3.8/inst/ext/pybind11/docs/advanced/cast/chrono.rst
+-rw-r--r--   0        0        0     3429 2023-07-20 13:04:23.523223 cornflakes-3.3.8/inst/ext/pybind11/docs/advanced/cast/custom.rst
+-rw-r--r--   0        0        0    14283 2023-07-20 13:04:23.523223 cornflakes-3.3.8/inst/ext/pybind11/docs/advanced/cast/eigen.rst
+-rw-r--r--   0        0        0     3889 2023-07-20 13:04:23.523223 cornflakes-3.3.8/inst/ext/pybind11/docs/advanced/cast/functional.rst
+-rw-r--r--   0        0        0     1556 2023-07-20 13:04:23.523223 cornflakes-3.3.8/inst/ext/pybind11/docs/advanced/cast/index.rst
+-rw-r--r--   0        0        0    12371 2023-07-20 13:04:23.523223 cornflakes-3.3.8/inst/ext/pybind11/docs/advanced/cast/overview.rst
+-rw-r--r--   0        0        0     9586 2023-07-20 13:04:23.523223 cornflakes-3.3.8/inst/ext/pybind11/docs/advanced/cast/stl.rst
+-rw-r--r--   0        0        0     8863 2023-07-20 13:04:23.523223 cornflakes-3.3.8/inst/ext/pybind11/docs/advanced/cast/strings.rst
+-rw-r--r--   0        0        0    47796 2023-07-20 13:04:23.523223 cornflakes-3.3.8/inst/ext/pybind11/docs/advanced/classes.rst
+-rw-r--r--   0        0        0     8453 2023-07-20 13:04:23.523223 cornflakes-3.3.8/inst/ext/pybind11/docs/advanced/embedding.rst
+-rw-r--r--   0        0        0    17796 2023-07-20 13:04:23.523223 cornflakes-3.3.8/inst/ext/pybind11/docs/advanced/exceptions.rst
+-rw-r--r--   0        0        0    26729 2023-07-20 13:04:23.523223 cornflakes-3.3.8/inst/ext/pybind11/docs/advanced/functions.rst
+-rw-r--r--   0        0        0    15651 2023-07-20 13:04:23.523223 cornflakes-3.3.8/inst/ext/pybind11/docs/advanced/misc.rst
+-rw-r--r--   0        0        0      278 2023-07-20 13:04:23.523223 cornflakes-3.3.8/inst/ext/pybind11/docs/advanced/pycpp/index.rst
+-rw-r--r--   0        0        0    17161 2023-07-20 13:04:23.523223 cornflakes-3.3.8/inst/ext/pybind11/docs/advanced/pycpp/numpy.rst
+-rw-r--r--   0        0        0     9030 2023-07-20 13:04:23.523223 cornflakes-3.3.8/inst/ext/pybind11/docs/advanced/pycpp/object.rst
+-rw-r--r--   0        0        0     5710 2023-07-20 13:04:23.523223 cornflakes-3.3.8/inst/ext/pybind11/docs/advanced/pycpp/utilities.rst
+-rw-r--r--   0        0        0     6377 2023-07-20 13:04:23.523223 cornflakes-3.3.8/inst/ext/pybind11/docs/advanced/smart_ptrs.rst
+-rw-r--r--   0        0        0     9240 2023-07-20 13:04:23.523223 cornflakes-3.3.8/inst/ext/pybind11/docs/basics.rst
+-rw-r--r--   0        0        0     2856 2023-07-20 13:04:23.523223 cornflakes-3.3.8/inst/ext/pybind11/docs/benchmark.py
+-rw-r--r--   0        0        0     3168 2023-07-20 13:04:23.523223 cornflakes-3.3.8/inst/ext/pybind11/docs/benchmark.rst
+-rw-r--r--   0        0        0   114174 2023-07-20 13:04:23.523223 cornflakes-3.3.8/inst/ext/pybind11/docs/changelog.rst
+-rw-r--r--   0        0        0    16380 2023-07-20 13:04:23.523223 cornflakes-3.3.8/inst/ext/pybind11/docs/classes.rst
+-rw-r--r--   0        0        0      273 2023-07-20 13:04:23.523223 cornflakes-3.3.8/inst/ext/pybind11/docs/cmake/index.rst
+-rw-r--r--   0        0        0    25777 2023-07-20 13:04:23.523223 cornflakes-3.3.8/inst/ext/pybind11/docs/compiling.rst
+-rw-r--r--   0        0        0    11574 2023-07-20 13:04:23.523223 cornflakes-3.3.8/inst/ext/pybind11/docs/conf.py
+-rw-r--r--   0        0        0    13177 2023-07-20 13:04:23.523223 cornflakes-3.3.8/inst/ext/pybind11/docs/faq.rst
+-rw-r--r--   0        0        0      613 2023-07-20 13:04:23.523223 cornflakes-3.3.8/inst/ext/pybind11/docs/index.rst
+-rw-r--r--   0        0        0     3277 2023-07-20 13:04:23.523223 cornflakes-3.3.8/inst/ext/pybind11/docs/installing.rst
+-rw-r--r--   0        0        0     3079 2023-07-20 13:04:23.523223 cornflakes-3.3.8/inst/ext/pybind11/docs/limitations.rst
+-rw-r--r--   0        0        0    61034 2023-07-20 13:04:23.523223 cornflakes-3.3.8/inst/ext/pybind11/docs/pybind11-logo.png
+-rw-r--r--   0        0        0    44653 2023-07-20 13:04:23.523223 cornflakes-3.3.8/inst/ext/pybind11/docs/pybind11_vs_boost_python1.png
+-rw-r--r--   0        0        0    87708 2023-07-20 13:04:23.527224 cornflakes-3.3.8/inst/ext/pybind11/docs/pybind11_vs_boost_python1.svg
+-rw-r--r--   0        0        0    41121 2023-07-20 13:04:23.527224 cornflakes-3.3.8/inst/ext/pybind11/docs/pybind11_vs_boost_python2.png
+-rw-r--r--   0        0        0    85853 2023-07-20 13:04:23.527224 cornflakes-3.3.8/inst/ext/pybind11/docs/pybind11_vs_boost_python2.svg
+-rw-r--r--   0        0        0     2647 2023-07-20 13:04:23.527224 cornflakes-3.3.8/inst/ext/pybind11/docs/reference.rst
+-rw-r--r--   0        0        0     4414 2023-07-20 13:04:23.527224 cornflakes-3.3.8/inst/ext/pybind11/docs/release.rst
+-rw-r--r--   0        0        0      149 2023-07-20 13:04:23.527224 cornflakes-3.3.8/inst/ext/pybind11/docs/requirements.txt
+-rw-r--r--   0        0        0    23489 2023-07-20 13:04:23.527224 cornflakes-3.3.8/inst/ext/pybind11/docs/upgrade.rst
+-rw-r--r--   0        0        0    23959 2023-07-20 13:04:23.527224 cornflakes-3.3.8/inst/ext/pybind11/include/pybind11/attr.h
+-rw-r--r--   0        0        0     7069 2023-07-20 13:04:23.527224 cornflakes-3.3.8/inst/ext/pybind11/include/pybind11/buffer_info.h
+-rw-r--r--   0        0        0    65952 2023-07-20 13:04:23.527224 cornflakes-3.3.8/inst/ext/pybind11/include/pybind11/cast.h
+-rw-r--r--   0        0        0     8458 2023-07-20 13:04:23.527224 cornflakes-3.3.8/inst/ext/pybind11/include/pybind11/chrono.h
+-rw-r--r--   0        0        0      120 2023-07-20 13:04:23.527224 cornflakes-3.3.8/inst/ext/pybind11/include/pybind11/common.h
+-rw-r--r--   0        0        0     2096 2023-07-20 13:04:23.527224 cornflakes-3.3.8/inst/ext/pybind11/include/pybind11/complex.h
+-rw-r--r--   0        0        0    28518 2023-07-20 13:04:23.527224 cornflakes-3.3.8/inst/ext/pybind11/include/pybind11/detail/class.h
+-rw-r--r--   0        0        0    52990 2023-07-20 13:04:23.527224 cornflakes-3.3.8/inst/ext/pybind11/include/pybind11/detail/common.h
+-rw-r--r--   0        0        0     5491 2023-07-20 13:04:23.527224 cornflakes-3.3.8/inst/ext/pybind11/include/pybind11/detail/descr.h
+-rw-r--r--   0        0        0    17869 2023-07-20 13:04:23.527224 cornflakes-3.3.8/inst/ext/pybind11/include/pybind11/detail/init.h
+-rw-r--r--   0        0        0    26498 2023-07-20 13:04:23.527224 cornflakes-3.3.8/inst/ext/pybind11/include/pybind11/detail/internals.h
+-rw-r--r--   0        0        0    42613 2023-07-20 13:04:23.527224 cornflakes-3.3.8/inst/ext/pybind11/include/pybind11/detail/type_caster_base.h
+-rw-r--r--   0        0        0     1625 2023-07-20 13:04:23.527224 cornflakes-3.3.8/inst/ext/pybind11/include/pybind11/detail/typeid.h
+-rw-r--r--   0        0        0    31450 2023-07-20 13:04:23.527224 cornflakes-3.3.8/inst/ext/pybind11/include/pybind11/eigen/matrix.h
+-rw-r--r--   0        0        0    18140 2023-07-20 13:04:23.527224 cornflakes-3.3.8/inst/ext/pybind11/include/pybind11/eigen/tensor.h
+-rw-r--r--   0        0        0      316 2023-07-20 13:04:23.527224 cornflakes-3.3.8/inst/ext/pybind11/include/pybind11/eigen.h
+-rw-r--r--   0        0        0    13475 2023-07-20 13:04:23.531224 cornflakes-3.3.8/inst/ext/pybind11/include/pybind11/embed.h
+-rw-r--r--   0        0        0     4731 2023-07-20 13:04:23.531224 cornflakes-3.3.8/inst/ext/pybind11/include/pybind11/eval.h
+-rw-r--r--   0        0        0     5002 2023-07-20 13:04:23.531224 cornflakes-3.3.8/inst/ext/pybind11/include/pybind11/functional.h
+-rw-r--r--   0        0        0     8262 2023-07-20 13:04:23.531224 cornflakes-3.3.8/inst/ext/pybind11/include/pybind11/gil.h
+-rw-r--r--   0        0        0     8862 2023-07-20 13:04:23.531224 cornflakes-3.3.8/inst/ext/pybind11/include/pybind11/iostream.h
+-rw-r--r--   0        0        0    79416 2023-07-20 13:04:23.531224 cornflakes-3.3.8/inst/ext/pybind11/include/pybind11/numpy.h
+-rw-r--r--   0        0        0     9103 2023-07-20 13:04:23.531224 cornflakes-3.3.8/inst/ext/pybind11/include/pybind11/operators.h
+-rw-r--r--   0        0        0     2734 2023-07-20 13:04:23.531224 cornflakes-3.3.8/inst/ext/pybind11/include/pybind11/options.h
+-rw-r--r--   0        0        0   126420 2023-07-20 13:04:23.531224 cornflakes-3.3.8/inst/ext/pybind11/include/pybind11/pybind11.h
+-rw-r--r--   0        0        0    94641 2023-07-20 13:04:23.531224 cornflakes-3.3.8/inst/ext/pybind11/include/pybind11/pytypes.h
+-rw-r--r--   0        0        0     4185 2023-07-20 13:04:23.531224 cornflakes-3.3.8/inst/ext/pybind11/include/pybind11/stl/filesystem.h
+-rw-r--r--   0        0        0    15399 2023-07-20 13:04:23.531224 cornflakes-3.3.8/inst/ext/pybind11/include/pybind11/stl.h
+-rw-r--r--   0        0        0    29824 2023-07-20 13:04:23.531224 cornflakes-3.3.8/inst/ext/pybind11/include/pybind11/stl_bind.h
+-rw-r--r--   0        0        0     2765 2023-07-20 13:04:23.531224 cornflakes-3.3.8/inst/ext/pybind11/noxfile.py
+-rw-r--r--   0        0        0      429 2023-07-20 13:04:23.531224 cornflakes-3.3.8/inst/ext/pybind11/pybind11/__init__.py
+-rw-r--r--   0        0        0     1544 2023-07-20 13:04:23.531224 cornflakes-3.3.8/inst/ext/pybind11/pybind11/__main__.py
+-rw-r--r--   0        0        0      233 2023-07-20 13:04:23.531224 cornflakes-3.3.8/inst/ext/pybind11/pybind11/_version.py
+-rw-r--r--   0        0        0     1207 2023-07-20 13:04:23.531224 cornflakes-3.3.8/inst/ext/pybind11/pybind11/commands.py
+-rw-r--r--   0        0        0        0 2023-07-20 13:04:23.531224 cornflakes-3.3.8/inst/ext/pybind11/pybind11/py.typed
+-rw-r--r--   0        0        0    17631 2023-07-20 13:04:23.531224 cornflakes-3.3.8/inst/ext/pybind11/pybind11/setup_helpers.py
+-rw-r--r--   0        0        0     2316 2023-07-20 13:04:23.531224 cornflakes-3.3.8/inst/ext/pybind11/pyproject.toml
+-rw-r--r--   0        0        0     1452 2023-07-20 13:04:23.531224 cornflakes-3.3.8/inst/ext/pybind11/setup.cfg
+-rw-r--r--   0        0        0     4877 2023-07-20 13:04:23.531224 cornflakes-3.3.8/inst/ext/pybind11/setup.py
+-rw-r--r--   0        0        0    21675 2023-07-20 13:04:23.531224 cornflakes-3.3.8/inst/ext/pybind11/tests/CMakeLists.txt
+-rw-r--r--   0        0        0     5625 2023-07-20 13:04:23.531224 cornflakes-3.3.8/inst/ext/pybind11/tests/conftest.py
+-rw-r--r--   0        0        0    11736 2023-07-20 13:04:23.531224 cornflakes-3.3.8/inst/ext/pybind11/tests/constructor_stats.h
+-rw-r--r--   0        0        0     3578 2023-07-20 13:04:23.531224 cornflakes-3.3.8/inst/ext/pybind11/tests/cross_module_gil_utils.cpp
+-rw-r--r--   0        0        0     1776 2023-07-20 13:04:23.531224 cornflakes-3.3.8/inst/ext/pybind11/tests/cross_module_interleaved_error_already_set.cpp
+-rw-r--r--   0        0        0      396 2023-07-20 13:04:23.531224 cornflakes-3.3.8/inst/ext/pybind11/tests/eigen_tensor_avoid_stl_array.cpp
+-rw-r--r--   0        0        0      926 2023-07-20 13:04:23.531224 cornflakes-3.3.8/inst/ext/pybind11/tests/env.py
+-rw-r--r--   0        0        0        0 2023-07-20 13:04:23.531224 cornflakes-3.3.8/inst/ext/pybind11/tests/extra_python_package/pytest.ini
+-rw-r--r--   0        0        0     8294 2023-07-20 13:04:23.531224 cornflakes-3.3.8/inst/ext/pybind11/tests/extra_python_package/test_files.py
+-rw-r--r--   0        0        0        0 2023-07-20 13:04:23.531224 cornflakes-3.3.8/inst/ext/pybind11/tests/extra_setuptools/pytest.ini
+-rw-r--r--   0        0        0     4153 2023-07-20 13:04:23.531224 cornflakes-3.3.8/inst/ext/pybind11/tests/extra_setuptools/test_setuphelper.py
+-rw-r--r--   0        0        0     2847 2023-07-20 13:04:23.531224 cornflakes-3.3.8/inst/ext/pybind11/tests/local_bindings.h
+-rw-r--r--   0        0        0     5743 2023-07-20 13:04:23.531224 cornflakes-3.3.8/inst/ext/pybind11/tests/object.h
+-rw-r--r--   0        0        0     6264 2023-07-20 13:04:23.535224 cornflakes-3.3.8/inst/ext/pybind11/tests/pybind11_cross_module_tests.cpp
+-rw-r--r--   0        0        0     4517 2023-07-20 13:04:23.535224 cornflakes-3.3.8/inst/ext/pybind11/tests/pybind11_tests.cpp
+-rw-r--r--   0        0        0     2685 2023-07-20 13:04:23.535224 cornflakes-3.3.8/inst/ext/pybind11/tests/pybind11_tests.h
+-rw-r--r--   0        0        0      768 2023-07-20 13:04:23.535224 cornflakes-3.3.8/inst/ext/pybind11/tests/pytest.ini
+-rw-r--r--   0        0        0      600 2023-07-20 13:04:23.535224 cornflakes-3.3.8/inst/ext/pybind11/tests/requirements.txt
+-rw-r--r--   0        0        0      855 2023-07-20 13:04:23.535224 cornflakes-3.3.8/inst/ext/pybind11/tests/test_async.cpp
+-rw-r--r--   0        0        0      536 2023-07-20 13:04:23.535224 cornflakes-3.3.8/inst/ext/pybind11/tests/test_async.py
+-rw-r--r--   0        0        0     8567 2023-07-20 13:04:23.535224 cornflakes-3.3.8/inst/ext/pybind11/tests/test_buffers.cpp
+-rw-r--r--   0        0        0     4848 2023-07-20 13:04:23.535224 cornflakes-3.3.8/inst/ext/pybind11/tests/test_buffers.py
+-rw-r--r--   0        0        0    16025 2023-07-20 13:04:23.535224 cornflakes-3.3.8/inst/ext/pybind11/tests/test_builtin_casters.cpp
+-rw-r--r--   0        0        0    17243 2023-07-20 13:04:23.535224 cornflakes-3.3.8/inst/ext/pybind11/tests/test_builtin_casters.py
+-rw-r--r--   0        0        0     4118 2023-07-20 13:04:23.535224 cornflakes-3.3.8/inst/ext/pybind11/tests/test_call_policies.cpp
+-rw-r--r--   0        0        0     6549 2023-07-20 13:04:23.535224 cornflakes-3.3.8/inst/ext/pybind11/tests/test_call_policies.py
+-rw-r--r--   0        0        0    10858 2023-07-20 13:04:23.535224 cornflakes-3.3.8/inst/ext/pybind11/tests/test_callbacks.cpp
+-rw-r--r--   0        0        0     6796 2023-07-20 13:04:23.535224 cornflakes-3.3.8/inst/ext/pybind11/tests/test_callbacks.py
+-rw-r--r--   0        0        0     3370 2023-07-20 13:04:23.535224 cornflakes-3.3.8/inst/ext/pybind11/tests/test_chrono.cpp
+-rw-r--r--   0        0        0     5691 2023-07-20 13:04:23.535224 cornflakes-3.3.8/inst/ext/pybind11/tests/test_chrono.py
+-rw-r--r--   0        0        0    24874 2023-07-20 13:04:23.535224 cornflakes-3.3.8/inst/ext/pybind11/tests/test_class.cpp
+-rw-r--r--   0        0        0    14757 2023-07-20 13:04:23.535224 cornflakes-3.3.8/inst/ext/pybind11/tests/test_class.py
+-rw-r--r--   0        0        0     2639 2023-07-20 13:04:23.535224 cornflakes-3.3.8/inst/ext/pybind11/tests/test_cmake_build/CMakeLists.txt
+-rw-r--r--   0        0        0      673 2023-07-20 13:04:23.535224 cornflakes-3.3.8/inst/ext/pybind11/tests/test_cmake_build/embed.cpp
+-rw-r--r--   0        0        0     1171 2023-07-20 13:04:23.535224 cornflakes-3.3.8/inst/ext/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt
+-rw-r--r--   0        0        0     1293 2023-07-20 13:04:23.535224 cornflakes-3.3.8/inst/ext/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt
+-rw-r--r--   0        0        0     1685 2023-07-20 13:04:23.535224 cornflakes-3.3.8/inst/ext/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt
+-rw-r--r--   0        0        0      152 2023-07-20 13:04:23.535224 cornflakes-3.3.8/inst/ext/pybind11/tests/test_cmake_build/main.cpp
+-rw-r--r--   0        0        0     1353 2023-07-20 13:04:23.535224 cornflakes-3.3.8/inst/ext/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt
+-rw-r--r--   0        0        0     1163 2023-07-20 13:04:23.535224 cornflakes-3.3.8/inst/ext/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt
+-rw-r--r--   0        0        0     1368 2023-07-20 13:04:23.535224 cornflakes-3.3.8/inst/ext/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt
+-rw-r--r--   0        0        0      198 2023-07-20 13:04:23.535224 cornflakes-3.3.8/inst/ext/pybind11/tests/test_cmake_build/test.py
+-rw-r--r--   0        0        0     3831 2023-07-20 13:04:23.535224 cornflakes-3.3.8/inst/ext/pybind11/tests/test_const_name.cpp
+-rw-r--r--   0        0        0      593 2023-07-20 13:04:23.535224 cornflakes-3.3.8/inst/ext/pybind11/tests/test_const_name.py
+-rw-r--r--   0        0        0     5615 2023-07-20 13:04:23.535224 cornflakes-3.3.8/inst/ext/pybind11/tests/test_constants_and_functions.cpp
+-rw-r--r--   0        0        0     1498 2023-07-20 13:04:23.535224 cornflakes-3.3.8/inst/ext/pybind11/tests/test_constants_and_functions.py
+-rw-r--r--   0        0        0    10886 2023-07-20 13:04:23.535224 cornflakes-3.3.8/inst/ext/pybind11/tests/test_copy_move.cpp
+-rw-r--r--   0        0        0     4796 2023-07-20 13:04:23.535224 cornflakes-3.3.8/inst/ext/pybind11/tests/test_copy_move.py
+-rw-r--r--   0        0        0     7280 2023-07-20 13:04:23.535224 cornflakes-3.3.8/inst/ext/pybind11/tests/test_custom_type_casters.cpp
+-rw-r--r--   0        0        0     3992 2023-07-20 13:04:23.535224 cornflakes-3.3.8/inst/ext/pybind11/tests/test_custom_type_casters.py
+-rw-r--r--   0        0        0     1259 2023-07-20 13:04:23.535224 cornflakes-3.3.8/inst/ext/pybind11/tests/test_custom_type_setup.cpp
+-rw-r--r--   0        0        0     1091 2023-07-20 13:04:23.535224 cornflakes-3.3.8/inst/ext/pybind11/tests/test_custom_type_setup.py
+-rw-r--r--   0        0        0     4557 2023-07-20 13:04:23.535224 cornflakes-3.3.8/inst/ext/pybind11/tests/test_docstring_options.cpp
+-rw-r--r--   0        0        0     2423 2023-07-20 13:04:23.535224 cornflakes-3.3.8/inst/ext/pybind11/tests/test_docstring_options.py
+-rw-r--r--   0        0        0    19350 2023-07-20 13:04:23.535224 cornflakes-3.3.8/inst/ext/pybind11/tests/test_eigen_matrix.cpp
+-rw-r--r--   0        0        0    29028 2023-07-20 13:04:23.535224 cornflakes-3.3.8/inst/ext/pybind11/tests/test_eigen_matrix.py
+-rw-r--r--   0        0        0      473 2023-07-20 13:04:23.535224 cornflakes-3.3.8/inst/ext/pybind11/tests/test_eigen_tensor.cpp
+-rw-r--r--   0        0        0    10590 2023-07-20 13:04:23.535224 cornflakes-3.3.8/inst/ext/pybind11/tests/test_eigen_tensor.inl
+-rw-r--r--   0        0        0     9414 2023-07-20 13:04:23.535224 cornflakes-3.3.8/inst/ext/pybind11/tests/test_eigen_tensor.py
+-rw-r--r--   0        0        0     1798 2023-07-20 13:04:23.535224 cornflakes-3.3.8/inst/ext/pybind11/tests/test_embed/CMakeLists.txt
+-rw-r--r--   0        0        0     1315 2023-07-20 13:04:23.535224 cornflakes-3.3.8/inst/ext/pybind11/tests/test_embed/catch.cpp
+-rw-r--r--   0        0        0      543 2023-07-20 13:04:23.535224 cornflakes-3.3.8/inst/ext/pybind11/tests/test_embed/external_module.cpp
+-rw-r--r--   0        0        0    17410 2023-07-20 13:04:23.535224 cornflakes-3.3.8/inst/ext/pybind11/tests/test_embed/test_interpreter.cpp
+-rw-r--r--   0        0        0      237 2023-07-20 13:04:23.535224 cornflakes-3.3.8/inst/ext/pybind11/tests/test_embed/test_interpreter.py
+-rw-r--r--   0        0        0      275 2023-07-20 13:04:23.535224 cornflakes-3.3.8/inst/ext/pybind11/tests/test_embed/test_trampoline.py
+-rw-r--r--   0        0        0     5722 2023-07-20 13:04:23.535224 cornflakes-3.3.8/inst/ext/pybind11/tests/test_enum.cpp
+-rw-r--r--   0        0        0     8939 2023-07-20 13:04:23.535224 cornflakes-3.3.8/inst/ext/pybind11/tests/test_enum.py
+-rw-r--r--   0        0        0     3168 2023-07-20 13:04:23.535224 cornflakes-3.3.8/inst/ext/pybind11/tests/test_eval.cpp
+-rw-r--r--   0        0        0     1143 2023-07-20 13:04:23.539224 cornflakes-3.3.8/inst/ext/pybind11/tests/test_eval.py
+-rw-r--r--   0        0        0      119 2023-07-20 13:04:23.539224 cornflakes-3.3.8/inst/ext/pybind11/tests/test_eval_call.py
+-rw-r--r--   0        0        0    12082 2023-07-20 13:04:23.539224 cornflakes-3.3.8/inst/ext/pybind11/tests/test_exceptions.cpp
+-rw-r--r--   0        0        0      399 2023-07-20 13:04:23.539224 cornflakes-3.3.8/inst/ext/pybind11/tests/test_exceptions.h
+-rw-r--r--   0        0        0    13001 2023-07-20 13:04:23.539224 cornflakes-3.3.8/inst/ext/pybind11/tests/test_exceptions.py
+-rw-r--r--   0        0        0    18155 2023-07-20 13:04:23.539224 cornflakes-3.3.8/inst/ext/pybind11/tests/test_factory_constructors.cpp
+-rw-r--r--   0        0        0    16491 2023-07-20 13:04:23.539224 cornflakes-3.3.8/inst/ext/pybind11/tests/test_factory_constructors.py
+-rw-r--r--   0        0        0     5311 2023-07-20 13:04:23.539224 cornflakes-3.3.8/inst/ext/pybind11/tests/test_gil_scoped.cpp
+-rw-r--r--   0        0        0     8507 2023-07-20 13:04:23.539224 cornflakes-3.3.8/inst/ext/pybind11/tests/test_gil_scoped.py
+-rw-r--r--   0        0        0     3960 2023-07-20 13:04:23.539224 cornflakes-3.3.8/inst/ext/pybind11/tests/test_iostream.cpp
+-rw-r--r--   0        0        0     7202 2023-07-20 13:04:23.539224 cornflakes-3.3.8/inst/ext/pybind11/tests/test_iostream.py
+-rw-r--r--   0        0        0     9444 2023-07-20 13:04:23.539224 cornflakes-3.3.8/inst/ext/pybind11/tests/test_kwargs_and_defaults.cpp
+-rw-r--r--   0        0        0    13600 2023-07-20 13:04:23.539224 cornflakes-3.3.8/inst/ext/pybind11/tests/test_kwargs_and_defaults.py
+-rw-r--r--   0        0        0     4401 2023-07-20 13:04:23.539224 cornflakes-3.3.8/inst/ext/pybind11/tests/test_local_bindings.cpp
+-rw-r--r--   0        0        0     8054 2023-07-20 13:04:23.539224 cornflakes-3.3.8/inst/ext/pybind11/tests/test_local_bindings.py
+-rw-r--r--   0        0        0    21388 2023-07-20 13:04:23.539224 cornflakes-3.3.8/inst/ext/pybind11/tests/test_methods_and_attributes.cpp
+-rw-r--r--   0        0        0    18105 2023-07-20 13:04:23.539224 cornflakes-3.3.8/inst/ext/pybind11/tests/test_methods_and_attributes.py
+-rw-r--r--   0        0        0     4121 2023-07-20 13:04:23.539224 cornflakes-3.3.8/inst/ext/pybind11/tests/test_modules.cpp
+-rw-r--r--   0        0        0     3963 2023-07-20 13:04:23.539224 cornflakes-3.3.8/inst/ext/pybind11/tests/test_modules.py
+-rw-r--r--   0        0        0    12305 2023-07-20 13:04:23.539224 cornflakes-3.3.8/inst/ext/pybind11/tests/test_multiple_inheritance.cpp
+-rw-r--r--   0        0        0    11874 2023-07-20 13:04:23.539224 cornflakes-3.3.8/inst/ext/pybind11/tests/test_multiple_inheritance.py
+-rw-r--r--   0        0        0    19861 2023-07-20 13:04:23.539224 cornflakes-3.3.8/inst/ext/pybind11/tests/test_numpy_array.cpp
+-rw-r--r--   0        0        0    20414 2023-07-20 13:04:23.539224 cornflakes-3.3.8/inst/ext/pybind11/tests/test_numpy_array.py
+-rw-r--r--   0        0        0    21114 2023-07-20 13:04:23.539224 cornflakes-3.3.8/inst/ext/pybind11/tests/test_numpy_dtypes.cpp
+-rw-r--r--   0        0        0    14272 2023-07-20 13:04:23.539224 cornflakes-3.3.8/inst/ext/pybind11/tests/test_numpy_dtypes.py
+-rw-r--r--   0        0        0     4487 2023-07-20 13:04:23.539224 cornflakes-3.3.8/inst/ext/pybind11/tests/test_numpy_vectorize.cpp
+-rw-r--r--   0        0        0     9658 2023-07-20 13:04:23.539224 cornflakes-3.3.8/inst/ext/pybind11/tests/test_numpy_vectorize.py
+-rw-r--r--   0        0        0     2777 2023-07-20 13:04:23.539224 cornflakes-3.3.8/inst/ext/pybind11/tests/test_opaque_types.cpp
+-rw-r--r--   0        0        0     1847 2023-07-20 13:04:23.539224 cornflakes-3.3.8/inst/ext/pybind11/tests/test_opaque_types.py
+-rw-r--r--   0        0        0     9132 2023-07-20 13:04:23.539224 cornflakes-3.3.8/inst/ext/pybind11/tests/test_operator_overloading.cpp
+-rw-r--r--   0        0        0     4332 2023-07-20 13:04:23.539224 cornflakes-3.3.8/inst/ext/pybind11/tests/test_operator_overloading.py
+-rw-r--r--   0        0        0     6719 2023-07-20 13:04:23.539224 cornflakes-3.3.8/inst/ext/pybind11/tests/test_pickling.cpp
+-rw-r--r--   0        0        0     2720 2023-07-20 13:04:23.539224 cornflakes-3.3.8/inst/ext/pybind11/tests/test_pickling.py
+-rw-r--r--   0        0        0    30750 2023-07-20 13:04:23.539224 cornflakes-3.3.8/inst/ext/pybind11/tests/test_pytypes.cpp
+-rw-r--r--   0        0        0    23629 2023-07-20 13:04:23.539224 cornflakes-3.3.8/inst/ext/pybind11/tests/test_pytypes.py
+-rw-r--r--   0        0        0    21153 2023-07-20 13:04:23.539224 cornflakes-3.3.8/inst/ext/pybind11/tests/test_sequences_and_iterators.cpp
+-rw-r--r--   0        0        0     8039 2023-07-20 13:04:23.539224 cornflakes-3.3.8/inst/ext/pybind11/tests/test_sequences_and_iterators.py
+-rw-r--r--   0        0        0    18898 2023-07-20 13:04:23.539224 cornflakes-3.3.8/inst/ext/pybind11/tests/test_smart_ptr.cpp
+-rw-r--r--   0        0        0     9530 2023-07-20 13:04:23.539224 cornflakes-3.3.8/inst/ext/pybind11/tests/test_smart_ptr.py
+-rw-r--r--   0        0        0    21587 2023-07-20 13:04:23.539224 cornflakes-3.3.8/inst/ext/pybind11/tests/test_stl.cpp
+-rw-r--r--   0        0        0    12232 2023-07-20 13:04:23.539224 cornflakes-3.3.8/inst/ext/pybind11/tests/test_stl.py
+-rw-r--r--   0        0        0     4622 2023-07-20 13:04:23.539224 cornflakes-3.3.8/inst/ext/pybind11/tests/test_stl_binders.cpp
+-rw-r--r--   0        0        0     9138 2023-07-20 13:04:23.539224 cornflakes-3.3.8/inst/ext/pybind11/tests/test_stl_binders.py
+-rw-r--r--   0        0        0     4617 2023-07-20 13:04:23.539224 cornflakes-3.3.8/inst/ext/pybind11/tests/test_tagbased_polymorphic.cpp
+-rw-r--r--   0        0        0      741 2023-07-20 13:04:23.539224 cornflakes-3.3.8/inst/ext/pybind11/tests/test_tagbased_polymorphic.py
+-rw-r--r--   0        0        0     1855 2023-07-20 13:04:23.539224 cornflakes-3.3.8/inst/ext/pybind11/tests/test_thread.cpp
+-rw-r--r--   0        0        0      826 2023-07-20 13:04:23.539224 cornflakes-3.3.8/inst/ext/pybind11/tests/test_thread.py
+-rw-r--r--   0        0        0      603 2023-07-20 13:04:23.539224 cornflakes-3.3.8/inst/ext/pybind11/tests/test_union.cpp
+-rw-r--r--   0        0        0      148 2023-07-20 13:04:23.539224 cornflakes-3.3.8/inst/ext/pybind11/tests/test_union.py
+-rw-r--r--   0        0        0    22991 2023-07-20 13:04:23.543224 cornflakes-3.3.8/inst/ext/pybind11/tests/test_virtual_functions.cpp
+-rw-r--r--   0        0        0    12913 2023-07-20 13:04:23.543224 cornflakes-3.3.8/inst/ext/pybind11/tests/test_virtual_functions.py
+-rw-r--r--   0        0        0     3226 2023-07-20 13:04:23.543224 cornflakes-3.3.8/inst/ext/pybind11/tests/valgrind-numpy-scipy.supp
+-rw-r--r--   0        0        0     2657 2023-07-20 13:04:23.543224 cornflakes-3.3.8/inst/ext/pybind11/tests/valgrind-python.supp
+-rw-r--r--   0        0        0     2449 2023-07-20 13:04:23.543224 cornflakes-3.3.8/inst/ext/pybind11/tools/FindCatch.cmake
+-rw-r--r--   0        0        0     3105 2023-07-20 13:04:23.543224 cornflakes-3.3.8/inst/ext/pybind11/tools/FindEigen3.cmake
+-rw-r--r--   0        0        0    11190 2023-07-20 13:04:23.543224 cornflakes-3.3.8/inst/ext/pybind11/tools/FindPythonLibsNew.cmake
+-rw-r--r--   0        0        0      817 2023-07-20 13:04:23.543224 cornflakes-3.3.8/inst/ext/pybind11/tools/JoinPaths.cmake
+-rwxr-xr-x   0        0        0     1423 2023-07-20 13:04:23.543224 cornflakes-3.3.8/inst/ext/pybind11/tools/check-style.sh
+-rw-r--r--   0        0        0      952 2023-07-20 13:04:23.543224 cornflakes-3.3.8/inst/ext/pybind11/tools/cmake_uninstall.cmake.in
+-rw-r--r--   0        0        0     1117 2023-07-20 13:04:23.543224 cornflakes-3.3.8/inst/ext/pybind11/tools/codespell_ignore_lines_from_errors.py
+-rw-r--r--   0        0        0     1031 2023-07-20 13:04:23.543224 cornflakes-3.3.8/inst/ext/pybind11/tools/libsize.py
+-rwxr-xr-x   0        0        0     1311 2023-07-20 13:04:23.543224 cornflakes-3.3.8/inst/ext/pybind11/tools/make_changelog.py
+-rw-r--r--   0        0        0      196 2023-07-20 13:04:23.543224 cornflakes-3.3.8/inst/ext/pybind11/tools/pybind11.pc.in
+-rw-r--r--   0        0        0    14033 2023-07-20 13:04:23.543224 cornflakes-3.3.8/inst/ext/pybind11/tools/pybind11Common.cmake
+-rw-r--r--   0        0        0     6930 2023-07-20 13:04:23.543224 cornflakes-3.3.8/inst/ext/pybind11/tools/pybind11Config.cmake.in
+-rw-r--r--   0        0        0     8960 2023-07-20 13:04:23.543224 cornflakes-3.3.8/inst/ext/pybind11/tools/pybind11NewTools.cmake
+-rw-r--r--   0        0        0     8361 2023-07-20 13:04:23.543224 cornflakes-3.3.8/inst/ext/pybind11/tools/pybind11Tools.cmake
+-rw-r--r--   0        0        0       94 2023-07-20 13:04:23.543224 cornflakes-3.3.8/inst/ext/pybind11/tools/pyproject.toml
+-rw-r--r--   0        0        0     2104 2023-07-20 13:04:23.543224 cornflakes-3.3.8/inst/ext/pybind11/tools/setup_global.py.in
+-rw-r--r--   0        0        0     1234 2023-07-20 13:04:23.543224 cornflakes-3.3.8/inst/ext/pybind11/tools/setup_main.py.in
+-rw-r--r--   0        0        0       49 2023-07-20 13:04:21.731196 cornflakes-3.3.8/inst/ext/rapidjson/.git
+-rw-r--r--   0        0        0      450 2023-07-20 13:04:24.591248 cornflakes-3.3.8/inst/ext/rapidjson/.gitattributes
+-rw-r--r--   0        0        0      404 2023-07-20 13:04:24.591248 cornflakes-3.3.8/inst/ext/rapidjson/.gitignore
+-rw-r--r--   0        0        0      104 2023-07-20 13:04:24.591248 cornflakes-3.3.8/inst/ext/rapidjson/.gitmodules
+-rw-r--r--   0        0        0     6312 2023-07-20 13:04:24.591248 cornflakes-3.3.8/inst/ext/rapidjson/.travis.yml
+-rw-r--r--   0        0        0     6818 2023-07-20 13:04:24.591248 cornflakes-3.3.8/inst/ext/rapidjson/CHANGELOG.md
+-rw-r--r--   0        0        0    10429 2023-07-20 13:04:24.591248 cornflakes-3.3.8/inst/ext/rapidjson/CMakeLists.txt
+-rw-r--r--   0        0        0      828 2023-07-20 13:04:24.591248 cornflakes-3.3.8/inst/ext/rapidjson/CMakeModules/FindGTestSrc.cmake
+-rw-r--r--   0        0        0      229 2023-07-20 13:04:24.591248 cornflakes-3.3.8/inst/ext/rapidjson/RapidJSON.pc.in
+-rw-r--r--   0        0        0      983 2023-07-20 13:04:24.591248 cornflakes-3.3.8/inst/ext/rapidjson/RapidJSONConfig.cmake.in
+-rw-r--r--   0        0        0      469 2023-07-20 13:04:24.591248 cornflakes-3.3.8/inst/ext/rapidjson/RapidJSONConfigVersion.cmake.in
+-rw-r--r--   0        0        0     2662 2023-07-20 13:04:24.591248 cornflakes-3.3.8/inst/ext/rapidjson/appveyor.yml
+-rw-r--r--   0        0        0        5 2023-07-20 13:04:24.591248 cornflakes-3.3.8/inst/ext/rapidjson/bin/data/abcde.txt
+-rw-r--r--   0        0        0      603 2023-07-20 13:04:24.591248 cornflakes-3.3.8/inst/ext/rapidjson/bin/data/glossary.json
+-rw-r--r--   0        0        0      898 2023-07-20 13:04:24.591248 cornflakes-3.3.8/inst/ext/rapidjson/bin/data/menu.json
+-rw-r--r--   0        0        0      103 2023-07-20 13:04:24.591248 cornflakes-3.3.8/inst/ext/rapidjson/bin/data/readme.txt
+-rw-r--r--   0        0        0   687491 2023-07-20 13:04:24.591248 cornflakes-3.3.8/inst/ext/rapidjson/bin/data/sample.json
+-rw-r--r--   0        0        0     3554 2023-07-20 13:04:24.591248 cornflakes-3.3.8/inst/ext/rapidjson/bin/data/webapp.json
+-rw-r--r--   0        0        0      626 2023-07-20 13:04:24.591248 cornflakes-3.3.8/inst/ext/rapidjson/bin/data/widget.json
+-rw-r--r--   0        0        0     4375 2023-07-20 13:04:24.591248 cornflakes-3.3.8/inst/ext/rapidjson/bin/draft-04/schema
+-rw-r--r--   0        0        0      368 2023-07-20 13:04:24.591248 cornflakes-3.3.8/inst/ext/rapidjson/bin/encodings/utf16be.json
+-rw-r--r--   0        0        0      370 2023-07-20 13:04:24.591248 cornflakes-3.3.8/inst/ext/rapidjson/bin/encodings/utf16bebom.json
+-rw-r--r--   0        0        0      368 2023-07-20 13:04:24.591248 cornflakes-3.3.8/inst/ext/rapidjson/bin/encodings/utf16le.json
+-rw-r--r--   0        0        0      370 2023-07-20 13:04:24.591248 cornflakes-3.3.8/inst/ext/rapidjson/bin/encodings/utf16lebom.json
+-rw-r--r--   0        0        0      736 2023-07-20 13:04:24.591248 cornflakes-3.3.8/inst/ext/rapidjson/bin/encodings/utf32be.json
+-rw-r--r--   0        0        0      740 2023-07-20 13:04:24.591248 cornflakes-3.3.8/inst/ext/rapidjson/bin/encodings/utf32bebom.json
+-rw-r--r--   0        0        0      736 2023-07-20 13:04:24.591248 cornflakes-3.3.8/inst/ext/rapidjson/bin/encodings/utf32le.json
+-rw-r--r--   0        0        0      740 2023-07-20 13:04:24.591248 cornflakes-3.3.8/inst/ext/rapidjson/bin/encodings/utf32lebom.json
+-rw-r--r--   0        0        0      322 2023-07-20 13:04:24.591248 cornflakes-3.3.8/inst/ext/rapidjson/bin/encodings/utf8.json
+-rw-r--r--   0        0        0      325 2023-07-20 13:04:24.591248 cornflakes-3.3.8/inst/ext/rapidjson/bin/encodings/utf8bom.json
+-rw-r--r--   0        0        0       60 2023-07-20 13:04:24.591248 cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonchecker/fail1.json
+-rw-r--r--   0        0        0       58 2023-07-20 13:04:24.591248 cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonchecker/fail10.json
+-rw-r--r--   0        0        0       29 2023-07-20 13:04:24.591248 cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonchecker/fail11.json
+-rw-r--r--   0        0        0       31 2023-07-20 13:04:24.591248 cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonchecker/fail12.json
+-rw-r--r--   0        0        0       43 2023-07-20 13:04:24.591248 cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonchecker/fail13.json
+-rw-r--r--   0        0        0       31 2023-07-20 13:04:24.591248 cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonchecker/fail14.json
+-rw-r--r--   0        0        0       34 2023-07-20 13:04:24.591248 cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonchecker/fail15.json
+-rw-r--r--   0        0        0        8 2023-07-20 13:04:24.591248 cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonchecker/fail16.json
+-rw-r--r--   0        0        0       34 2023-07-20 13:04:24.591248 cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonchecker/fail17.json
+-rw-r--r--   0        0        0       50 2023-07-20 13:04:24.591248 cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonchecker/fail18.json
+-rw-r--r--   0        0        0       22 2023-07-20 13:04:24.595248 cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonchecker/fail19.json
+-rw-r--r--   0        0        0       17 2023-07-20 13:04:24.595248 cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonchecker/fail2.json
+-rw-r--r--   0        0        0       23 2023-07-20 13:04:24.595248 cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonchecker/fail20.json
+-rw-r--r--   0        0        0       32 2023-07-20 13:04:24.595248 cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonchecker/fail21.json
+-rw-r--r--   0        0        0       33 2023-07-20 13:04:24.595248 cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonchecker/fail22.json
+-rw-r--r--   0        0        0       20 2023-07-20 13:04:24.595248 cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonchecker/fail23.json
+-rw-r--r--   0        0        0       16 2023-07-20 13:04:24.595248 cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonchecker/fail24.json
+-rw-r--r--   0        0        0       29 2023-07-20 13:04:24.595248 cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonchecker/fail25.json
+-rw-r--r--   0        0        0       38 2023-07-20 13:04:24.595248 cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonchecker/fail26.json
+-rw-r--r--   0        0        0       14 2023-07-20 13:04:24.595248 cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonchecker/fail27.json
+-rw-r--r--   0        0        0       15 2023-07-20 13:04:24.595248 cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonchecker/fail28.json
+-rw-r--r--   0        0        0        4 2023-07-20 13:04:24.595248 cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonchecker/fail29.json
+-rw-r--r--   0        0        0       37 2023-07-20 13:04:24.595248 cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonchecker/fail3.json
+-rw-r--r--   0        0        0        5 2023-07-20 13:04:24.595248 cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonchecker/fail30.json
+-rw-r--r--   0        0        0        7 2023-07-20 13:04:24.595248 cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonchecker/fail31.json
+-rw-r--r--   0        0        0       40 2023-07-20 13:04:24.595248 cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonchecker/fail32.json
+-rw-r--r--   0        0        0       12 2023-07-20 13:04:24.595248 cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonchecker/fail33.json
+-rw-r--r--   0        0        0       16 2023-07-20 13:04:24.595248 cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonchecker/fail4.json
+-rw-r--r--   0        0        0       24 2023-07-20 13:04:24.595248 cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonchecker/fail5.json
+-rw-r--r--   0        0        0       26 2023-07-20 13:04:24.595248 cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonchecker/fail6.json
+-rw-r--r--   0        0        0       26 2023-07-20 13:04:24.595248 cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonchecker/fail7.json
+-rw-r--r--   0        0        0       16 2023-07-20 13:04:24.595248 cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonchecker/fail8.json
+-rw-r--r--   0        0        0       22 2023-07-20 13:04:24.595248 cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonchecker/fail9.json
+-rw-r--r--   0        0        0     1441 2023-07-20 13:04:24.595248 cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonchecker/pass1.json
+-rw-r--r--   0        0        0       52 2023-07-20 13:04:24.595248 cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonchecker/pass2.json
+-rw-r--r--   0        0        0      148 2023-07-20 13:04:24.595248 cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonchecker/pass3.json
+-rw-r--r--   0        0        0      173 2023-07-20 13:04:24.595248 cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonchecker/readme.txt
+-rw-r--r--   0        0        0        5 2023-07-20 13:04:24.595248 cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonschema/.gitignore
+-rw-r--r--   0        0        0       98 2023-07-20 13:04:24.595248 cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonschema/.travis.yml
+-rw-r--r--   0        0        0     1057 2023-07-20 13:04:24.595248 cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonschema/LICENSE
+-rw-r--r--   0        0        0     4787 2023-07-20 13:04:24.595248 cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonschema/README.md
+-rwxr-xr-x   0        0        0     9059 2023-07-20 13:04:24.595248 cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonschema/bin/jsonschema_suite
+-rw-r--r--   0        0        0       25 2023-07-20 13:04:24.595248 cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonschema/remotes/folder/folderInteger.json
+-rw-r--r--   0        0        0       25 2023-07-20 13:04:24.595248 cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonschema/remotes/integer.json
+-rw-r--r--   0        0        0      110 2023-07-20 13:04:24.595248 cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonschema/remotes/subSchemas.json
+-rw-r--r--   0        0        0     2257 2023-07-20 13:04:24.595248 cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonschema/tests/draft3/additionalItems.json
+-rw-r--r--   0        0        0     2745 2023-07-20 13:04:24.595248 cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonschema/tests/draft3/additionalProperties.json
+-rw-r--r--   0        0        0     1273 2023-07-20 13:04:24.595248 cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonschema/tests/draft3/default.json
+-rw-r--r--   0        0        0     2989 2023-07-20 13:04:24.595248 cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonschema/tests/draft3/dependencies.json
+-rw-r--r--   0        0        0     1936 2023-07-20 13:04:24.595248 cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonschema/tests/draft3/disallow.json
+-rw-r--r--   0        0        0     1544 2023-07-20 13:04:24.595248 cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonschema/tests/draft3/divisibleBy.json
+-rw-r--r--   0        0        0     1964 2023-07-20 13:04:24.595248 cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonschema/tests/draft3/enum.json
+-rw-r--r--   0        0        0     2591 2023-07-20 13:04:24.595248 cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonschema/tests/draft3/extends.json
+-rw-r--r--   0        0        0     1136 2023-07-20 13:04:24.595248 cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonschema/tests/draft3/items.json
+-rw-r--r--   0        0        0      706 2023-07-20 13:04:24.595248 cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonschema/tests/draft3/maxItems.json
+-rw-r--r--   0        0        0      895 2023-07-20 13:04:24.595248 cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonschema/tests/draft3/maxLength.json
+-rw-r--r--   0        0        0     1063 2023-07-20 13:04:24.595248 cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonschema/tests/draft3/maximum.json
+-rw-r--r--   0        0        0      693 2023-07-20 13:04:24.595248 cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonschema/tests/draft3/minItems.json
+-rw-r--r--   0        0        0      886 2023-07-20 13:04:24.595248 cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonschema/tests/draft3/minLength.json
+-rw-r--r--   0        0        0     1063 2023-07-20 13:04:24.595248 cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonschema/tests/draft3/minimum.json
+-rw-r--r--   0        0        0     3075 2023-07-20 13:04:24.595248 cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonschema/tests/draft3/optional/bignum.json
+-rw-r--r--   0        0        0     6751 2023-07-20 13:04:24.595248 cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonschema/tests/draft3/optional/format.json
+-rw-r--r--   0        0        0      463 2023-07-20 13:04:24.595248 cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonschema/tests/draft3/optional/jsregex.json
+-rw-r--r--   0        0        0      384 2023-07-20 13:04:24.595248 cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonschema/tests/draft3/optional/zeroTerminatedFloats.json
+-rw-r--r--   0        0        0      857 2023-07-20 13:04:24.595248 cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonschema/tests/draft3/pattern.json
+-rw-r--r--   0        0        0     3365 2023-07-20 13:04:24.595248 cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonschema/tests/draft3/patternProperties.json
+-rw-r--r--   0        0        0     2881 2023-07-20 13:04:24.595248 cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonschema/tests/draft3/properties.json
+-rw-r--r--   0        0        0     4385 2023-07-20 13:04:24.595248 cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonschema/tests/draft3/ref.json
+-rw-r--r--   0        0        0     1961 2023-07-20 13:04:24.595248 cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonschema/tests/draft3/refRemote.json
+-rw-r--r--   0        0        0     1282 2023-07-20 13:04:24.595248 cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonschema/tests/draft3/required.json
+-rw-r--r--   0        0        0    13217 2023-07-20 13:04:24.595248 cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonschema/tests/draft3/type.json
+-rw-r--r--   0        0        0     2613 2023-07-20 13:04:24.595248 cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonschema/tests/draft3/uniqueItems.json
+-rw-r--r--   0        0        0     2282 2023-07-20 13:04:24.595248 cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonschema/tests/draft4/additionalItems.json
+-rw-r--r--   0        0        0     2745 2023-07-20 13:04:24.595248 cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonschema/tests/draft4/additionalProperties.json
+-rw-r--r--   0        0        0     3025 2023-07-20 13:04:24.595248 cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonschema/tests/draft4/allOf.json
+-rw-r--r--   0        0        0     1608 2023-07-20 13:04:24.595248 cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonschema/tests/draft4/anyOf.json
+-rw-r--r--   0        0        0     1273 2023-07-20 13:04:24.595248 cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonschema/tests/draft4/default.json
+-rw-r--r--   0        0        0      854 2023-07-20 13:04:24.595248 cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonschema/tests/draft4/definitions.json
+-rw-r--r--   0        0        0     3139 2023-07-20 13:04:24.595248 cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonschema/tests/draft4/dependencies.json
+-rw-r--r--   0        0        0     1975 2023-07-20 13:04:24.595248 cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonschema/tests/draft4/enum.json
+-rw-r--r--   0        0        0     1136 2023-07-20 13:04:24.595248 cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonschema/tests/draft4/items.json
+-rw-r--r--   0        0        0      706 2023-07-20 13:04:24.595248 cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonschema/tests/draft4/maxItems.json
+-rw-r--r--   0        0        0      896 2023-07-20 13:04:24.595248 cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonschema/tests/draft4/maxLength.json
+-rw-r--r--   0        0        0      759 2023-07-20 13:04:24.595248 cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonschema/tests/draft4/maxProperties.json
+-rw-r--r--   0        0        0     1063 2023-07-20 13:04:24.595248 cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonschema/tests/draft4/maximum.json
+-rw-r--r--   0        0        0      693 2023-07-20 13:04:24.595248 cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonschema/tests/draft4/minItems.json
+-rw-r--r--   0        0        0      886 2023-07-20 13:04:24.595248 cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonschema/tests/draft4/minLength.json
+-rw-r--r--   0        0        0      725 2023-07-20 13:04:24.595248 cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonschema/tests/draft4/minProperties.json
+-rw-r--r--   0        0        0     1063 2023-07-20 13:04:24.595248 cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonschema/tests/draft4/minimum.json
+-rw-r--r--   0        0        0     1525 2023-07-20 13:04:24.595248 cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonschema/tests/draft4/multipleOf.json
+-rw-r--r--   0        0        0     2266 2023-07-20 13:04:24.595248 cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonschema/tests/draft4/not.json
+-rw-r--r--   0        0        0     1607 2023-07-20 13:04:24.595248 cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonschema/tests/draft4/oneOf.json
+-rw-r--r--   0        0        0     3075 2023-07-20 13:04:24.595248 cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonschema/tests/draft4/optional/bignum.json
+-rw-r--r--   0        0        0     4608 2023-07-20 13:04:24.595248 cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonschema/tests/draft4/optional/format.json
+-rw-r--r--   0        0        0      384 2023-07-20 13:04:24.595248 cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonschema/tests/draft4/optional/zeroTerminatedFloats.json
+-rw-r--r--   0        0        0      857 2023-07-20 13:04:24.595248 cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonschema/tests/draft4/pattern.json
+-rw-r--r--   0        0        0     3365 2023-07-20 13:04:24.595248 cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonschema/tests/draft4/patternProperties.json
+-rw-r--r--   0        0        0     2881 2023-07-20 13:04:24.595248 cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonschema/tests/draft4/properties.json
+-rw-r--r--   0        0        0     4366 2023-07-20 13:04:24.595248 cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonschema/tests/draft4/ref.json
+-rw-r--r--   0        0        0     1961 2023-07-20 13:04:24.595248 cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonschema/tests/draft4/refRemote.json
+-rw-r--r--   0        0        0      923 2023-07-20 13:04:24.595248 cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonschema/tests/draft4/required.json
+-rw-r--r--   0        0        0     9298 2023-07-20 13:04:24.595248 cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonschema/tests/draft4/type.json
+-rw-r--r--   0        0        0     2613 2023-07-20 13:04:24.595248 cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonschema/tests/draft4/uniqueItems.json
+-rw-r--r--   0        0        0      134 2023-07-20 13:04:24.595248 cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonschema/tox.ini
+-rw-r--r--   0        0        0    30003 2023-07-20 13:04:24.595248 cornflakes-3.3.8/inst/ext/rapidjson/bin/types/alotofkeys.json
+-rw-r--r--   0        0        0      849 2023-07-20 13:04:24.595248 cornflakes-3.3.8/inst/ext/rapidjson/bin/types/booleans.json
+-rw-r--r--   0        0        0     1698 2023-07-20 13:04:24.595248 cornflakes-3.3.8/inst/ext/rapidjson/bin/types/floats.json
+-rw-r--r--   0        0        0     4202 2023-07-20 13:04:24.595248 cornflakes-3.3.8/inst/ext/rapidjson/bin/types/guids.json
+-rw-r--r--   0        0        0     1098 2023-07-20 13:04:24.595248 cornflakes-3.3.8/inst/ext/rapidjson/bin/types/integers.json
+-rw-r--r--   0        0        0    15142 2023-07-20 13:04:24.595248 cornflakes-3.3.8/inst/ext/rapidjson/bin/types/mixed.json
+-rw-r--r--   0        0        0      802 2023-07-20 13:04:24.595248 cornflakes-3.3.8/inst/ext/rapidjson/bin/types/nulls.json
+-rw-r--r--   0        0        0    33764 2023-07-20 13:04:24.595248 cornflakes-3.3.8/inst/ext/rapidjson/bin/types/paragraphs.json
+-rw-r--r--   0        0        0       86 2023-07-20 13:04:24.595248 cornflakes-3.3.8/inst/ext/rapidjson/bin/types/readme.txt
+-rw-r--r--   0        0        0     3150 2023-07-20 13:04:24.595248 cornflakes-3.3.8/inst/ext/rapidjson/bin/unittestschema/address.json
+-rw-r--r--   0        0        0       84 2023-07-20 13:04:24.595248 cornflakes-3.3.8/inst/ext/rapidjson/bin/unittestschema/allOf_address.json
+-rw-r--r--   0        0        0       84 2023-07-20 13:04:24.595248 cornflakes-3.3.8/inst/ext/rapidjson/bin/unittestschema/anyOf_address.json
+-rw-r--r--   0        0        0     1315 2023-07-20 13:04:24.595248 cornflakes-3.3.8/inst/ext/rapidjson/bin/unittestschema/idandref.json
+-rw-r--r--   0        0        0       84 2023-07-20 13:04:24.595248 cornflakes-3.3.8/inst/ext/rapidjson/bin/unittestschema/oneOf_address.json
+-rw-r--r--   0        0        0     2175 2023-07-20 13:04:24.595248 cornflakes-3.3.8/inst/ext/rapidjson/contrib/natvis/LICENSE
+-rw-r--r--   0        0        0      678 2023-07-20 13:04:24.595248 cornflakes-3.3.8/inst/ext/rapidjson/contrib/natvis/README.md
+-rw-r--r--   0        0        0     2729 2023-07-20 13:04:24.595248 cornflakes-3.3.8/inst/ext/rapidjson/contrib/natvis/rapidjson.natvis
+-rw-r--r--   0        0        0     1052 2023-07-20 13:04:24.595248 cornflakes-3.3.8/inst/ext/rapidjson/doc/CMakeLists.txt
+-rw-r--r--   0        0        0   103393 2023-07-20 13:04:24.599248 cornflakes-3.3.8/inst/ext/rapidjson/doc/Doxyfile.in
+-rw-r--r--   0        0        0   103478 2023-07-20 13:04:24.599248 cornflakes-3.3.8/inst/ext/rapidjson/doc/Doxyfile.zh-cn.in
+-rw-r--r--   0        0        0      912 2023-07-20 13:04:24.599248 cornflakes-3.3.8/inst/ext/rapidjson/doc/diagram/architecture.dot
+-rw-r--r--   0        0        0    16569 2023-07-20 13:04:24.599248 cornflakes-3.3.8/inst/ext/rapidjson/doc/diagram/architecture.png
+-rw-r--r--   0        0        0     2239 2023-07-20 13:04:24.599248 cornflakes-3.3.8/inst/ext/rapidjson/doc/diagram/insituparsing.dot
+-rw-r--r--   0        0        0    37281 2023-07-20 13:04:24.599248 cornflakes-3.3.8/inst/ext/rapidjson/doc/diagram/insituparsing.png
+-rw-r--r--   0        0        0     1915 2023-07-20 13:04:24.599248 cornflakes-3.3.8/inst/ext/rapidjson/doc/diagram/iterative-parser-states-diagram.dot
+-rw-r--r--   0        0        0    92378 2023-07-20 13:04:24.599248 cornflakes-3.3.8/inst/ext/rapidjson/doc/diagram/iterative-parser-states-diagram.png
+-rw-r--r--   0        0        0      176 2023-07-20 13:04:24.599248 cornflakes-3.3.8/inst/ext/rapidjson/doc/diagram/makefile
+-rw-r--r--   0        0        0      935 2023-07-20 13:04:24.599248 cornflakes-3.3.8/inst/ext/rapidjson/doc/diagram/move1.dot
+-rw-r--r--   0        0        0    16081 2023-07-20 13:04:24.599248 cornflakes-3.3.8/inst/ext/rapidjson/doc/diagram/move1.png
+-rw-r--r--   0        0        0     1502 2023-07-20 13:04:24.599248 cornflakes-3.3.8/inst/ext/rapidjson/doc/diagram/move2.dot
+-rw-r--r--   0        0        0    41517 2023-07-20 13:04:24.599248 cornflakes-3.3.8/inst/ext/rapidjson/doc/diagram/move2.png
+-rw-r--r--   0        0        0     1454 2023-07-20 13:04:24.599248 cornflakes-3.3.8/inst/ext/rapidjson/doc/diagram/move3.dot
+-rw-r--r--   0        0        0    36371 2023-07-20 13:04:24.599248 cornflakes-3.3.8/inst/ext/rapidjson/doc/diagram/move3.png
+-rw-r--r--   0        0        0     1427 2023-07-20 13:04:24.599248 cornflakes-3.3.8/inst/ext/rapidjson/doc/diagram/normalparsing.dot
+-rw-r--r--   0        0        0    32887 2023-07-20 13:04:24.599248 cornflakes-3.3.8/inst/ext/rapidjson/doc/diagram/normalparsing.png
+-rw-r--r--   0        0        0     1435 2023-07-20 13:04:24.599248 cornflakes-3.3.8/inst/ext/rapidjson/doc/diagram/simpledom.dot
+-rw-r--r--   0        0        0    43670 2023-07-20 13:04:24.599248 cornflakes-3.3.8/inst/ext/rapidjson/doc/diagram/simpledom.png
+-rw-r--r--   0        0        0     1456 2023-07-20 13:04:24.599248 cornflakes-3.3.8/inst/ext/rapidjson/doc/diagram/tutorial.dot
+-rw-r--r--   0        0        0    44634 2023-07-20 13:04:24.599248 cornflakes-3.3.8/inst/ext/rapidjson/doc/diagram/tutorial.png
+-rw-r--r--   0        0        0     1775 2023-07-20 13:04:24.599248 cornflakes-3.3.8/inst/ext/rapidjson/doc/diagram/utilityclass.dot
+-rw-r--r--   0        0        0    99993 2023-07-20 13:04:24.599248 cornflakes-3.3.8/inst/ext/rapidjson/doc/diagram/utilityclass.png
+-rw-r--r--   0        0        0    15464 2023-07-20 13:04:24.599248 cornflakes-3.3.8/inst/ext/rapidjson/doc/dom.md
+-rw-r--r--   0        0        0    15393 2023-07-20 13:04:24.599248 cornflakes-3.3.8/inst/ext/rapidjson/doc/dom.zh-cn.md
+-rw-r--r--   0        0        0     6708 2023-07-20 13:04:24.599248 cornflakes-3.3.8/inst/ext/rapidjson/doc/encoding.md
+-rw-r--r--   0        0        0     6860 2023-07-20 13:04:24.599248 cornflakes-3.3.8/inst/ext/rapidjson/doc/encoding.zh-cn.md
+-rw-r--r--   0        0        0    15364 2023-07-20 13:04:24.603248 cornflakes-3.3.8/inst/ext/rapidjson/doc/faq.md
+-rw-r--r--   0        0        0    15030 2023-07-20 13:04:24.603248 cornflakes-3.3.8/inst/ext/rapidjson/doc/faq.zh-cn.md
+-rw-r--r--   0        0        0     5063 2023-07-20 13:04:24.603248 cornflakes-3.3.8/inst/ext/rapidjson/doc/features.md
+-rw-r--r--   0        0        0     4805 2023-07-20 13:04:24.603248 cornflakes-3.3.8/inst/ext/rapidjson/doc/features.zh-cn.md
+-rw-r--r--   0        0        0    22426 2023-07-20 13:04:24.603248 cornflakes-3.3.8/inst/ext/rapidjson/doc/internals.md
+-rw-r--r--   0        0        0    21956 2023-07-20 13:04:24.603248 cornflakes-3.3.8/inst/ext/rapidjson/doc/internals.zh-cn.md
+-rw-r--r--   0        0        0     5259 2023-07-20 13:04:24.603248 cornflakes-3.3.8/inst/ext/rapidjson/doc/logo/rapidjson.png
+-rw-r--r--   0        0        0     4230 2023-07-20 13:04:24.603248 cornflakes-3.3.8/inst/ext/rapidjson/doc/logo/rapidjson.svg
+-rw-r--r--   0        0        0     6090 2023-07-20 13:04:24.603248 cornflakes-3.3.8/inst/ext/rapidjson/doc/misc/DoxygenLayout.xml
+-rw-r--r--   0        0        0     6572 2023-07-20 13:04:24.603248 cornflakes-3.3.8/inst/ext/rapidjson/doc/misc/doxygenextra.css
+-rw-r--r--   0        0        0      256 2023-07-20 13:04:24.603248 cornflakes-3.3.8/inst/ext/rapidjson/doc/misc/footer.html
+-rw-r--r--   0        0        0     1137 2023-07-20 13:04:24.603248 cornflakes-3.3.8/inst/ext/rapidjson/doc/misc/header.html
+-rw-r--r--   0        0        0      363 2023-07-20 13:04:24.603248 cornflakes-3.3.8/inst/ext/rapidjson/doc/npm.md
+-rw-r--r--   0        0        0     1268 2023-07-20 13:04:24.603248 cornflakes-3.3.8/inst/ext/rapidjson/doc/performance.md
+-rw-r--r--   0        0        0     1236 2023-07-20 13:04:24.603248 cornflakes-3.3.8/inst/ext/rapidjson/doc/performance.zh-cn.md
+-rw-r--r--   0        0        0     8883 2023-07-20 13:04:24.603248 cornflakes-3.3.8/inst/ext/rapidjson/doc/pointer.md
+-rw-r--r--   0        0        0     8532 2023-07-20 13:04:24.603248 cornflakes-3.3.8/inst/ext/rapidjson/doc/pointer.zh-cn.md
+-rw-r--r--   0        0        0    21276 2023-07-20 13:04:24.603248 cornflakes-3.3.8/inst/ext/rapidjson/doc/sax.md
+-rw-r--r--   0        0        0    19967 2023-07-20 13:04:24.603248 cornflakes-3.3.8/inst/ext/rapidjson/doc/sax.zh-cn.md
+-rw-r--r--   0        0        0    18222 2023-07-20 13:04:24.603248 cornflakes-3.3.8/inst/ext/rapidjson/doc/schema.md
+-rw-r--r--   0        0        0     9765 2023-07-20 13:04:24.603248 cornflakes-3.3.8/inst/ext/rapidjson/doc/schema.zh-cn.md
+-rw-r--r--   0        0        0    14531 2023-07-20 13:04:24.603248 cornflakes-3.3.8/inst/ext/rapidjson/doc/stream.md
+-rw-r--r--   0        0        0    14325 2023-07-20 13:04:24.603248 cornflakes-3.3.8/inst/ext/rapidjson/doc/stream.zh-cn.md
+-rw-r--r--   0        0        0    22121 2023-07-20 13:04:24.603248 cornflakes-3.3.8/inst/ext/rapidjson/doc/tutorial.md
+-rw-r--r--   0        0        0    21546 2023-07-20 13:04:24.603248 cornflakes-3.3.8/inst/ext/rapidjson/doc/tutorial.zh-cn.md
+-rw-r--r--   0        0        0      229 2023-07-20 13:04:24.603248 cornflakes-3.3.8/inst/ext/rapidjson/docker/debian/Dockerfile
+-rw-r--r--   0        0        0      982 2023-07-20 13:04:24.603248 cornflakes-3.3.8/inst/ext/rapidjson/example/CMakeLists.txt
+-rw-r--r--   0        0        0     7130 2023-07-20 13:04:24.603248 cornflakes-3.3.8/inst/ext/rapidjson/example/archiver/archiver.cpp
+-rw-r--r--   0        0        0     3567 2023-07-20 13:04:24.603248 cornflakes-3.3.8/inst/ext/rapidjson/example/archiver/archiver.h
+-rw-r--r--   0        0        0     6862 2023-07-20 13:04:24.603248 cornflakes-3.3.8/inst/ext/rapidjson/example/archiver/archivertest.cpp
+-rw-r--r--   0        0        0     2577 2023-07-20 13:04:24.603248 cornflakes-3.3.8/inst/ext/rapidjson/example/capitalize/capitalize.cpp
+-rw-r--r--   0        0        0     1015 2023-07-20 13:04:24.603248 cornflakes-3.3.8/inst/ext/rapidjson/example/condense/condense.cpp
+-rw-r--r--   0        0        0     4979 2023-07-20 13:04:24.603248 cornflakes-3.3.8/inst/ext/rapidjson/example/filterkey/filterkey.cpp
+-rw-r--r--   0        0        0     5946 2023-07-20 13:04:24.603248 cornflakes-3.3.8/inst/ext/rapidjson/example/filterkeydom/filterkeydom.cpp
+-rw-r--r--   0        0        0     6022 2023-07-20 13:04:24.603248 cornflakes-3.3.8/inst/ext/rapidjson/example/jsonx/jsonx.cpp
+-rw-r--r--   0        0        0     9461 2023-07-20 13:04:24.603248 cornflakes-3.3.8/inst/ext/rapidjson/example/lookaheadparser/lookaheadparser.cpp
+-rw-r--r--   0        0        0     2814 2023-07-20 13:04:24.603248 cornflakes-3.3.8/inst/ext/rapidjson/example/messagereader/messagereader.cpp
+-rw-r--r--   0        0        0     5150 2023-07-20 13:04:24.603248 cornflakes-3.3.8/inst/ext/rapidjson/example/parsebyparts/parsebyparts.cpp
+-rw-r--r--   0        0        0     1019 2023-07-20 13:04:24.603248 cornflakes-3.3.8/inst/ext/rapidjson/example/pretty/pretty.cpp
+-rw-r--r--   0        0        0     2245 2023-07-20 13:04:24.603248 cornflakes-3.3.8/inst/ext/rapidjson/example/prettyauto/prettyauto.cpp
+-rw-r--r--   0        0        0     8706 2023-07-20 13:04:24.603248 cornflakes-3.3.8/inst/ext/rapidjson/example/schemavalidator/schemavalidator.cpp
+-rw-r--r--   0        0        0     4590 2023-07-20 13:04:24.603248 cornflakes-3.3.8/inst/ext/rapidjson/example/serialize/serialize.cpp
+-rw-r--r--   0        0        0      685 2023-07-20 13:04:24.603248 cornflakes-3.3.8/inst/ext/rapidjson/example/simpledom/simpledom.cpp
+-rw-r--r--   0        0        0     2259 2023-07-20 13:04:24.603248 cornflakes-3.3.8/inst/ext/rapidjson/example/simplepullreader/simplepullreader.cpp
+-rw-r--r--   0        0        0     1868 2023-07-20 13:04:24.603248 cornflakes-3.3.8/inst/ext/rapidjson/example/simplereader/simplereader.cpp
+-rw-r--r--   0        0        0     1031 2023-07-20 13:04:24.603248 cornflakes-3.3.8/inst/ext/rapidjson/example/simplewriter/simplewriter.cpp
+-rw-r--r--   0        0        0     1610 2023-07-20 13:04:24.603248 cornflakes-3.3.8/inst/ext/rapidjson/example/sortkeys/sortkeys.cpp
+-rw-r--r--   0        0        0      943 2023-07-20 13:04:24.603248 cornflakes-3.3.8/inst/ext/rapidjson/example/traverseaspointer.cpp
+-rw-r--r--   0        0        0     6263 2023-07-20 13:04:24.603248 cornflakes-3.3.8/inst/ext/rapidjson/example/tutorial/tutorial.cpp
+-rw-r--r--   0        0        0    22592 2023-07-20 13:04:24.603248 cornflakes-3.3.8/inst/ext/rapidjson/include/rapidjson/allocators.h
+-rw-r--r--   0        0        0     2260 2023-07-20 13:04:24.607248 cornflakes-3.3.8/inst/ext/rapidjson/include/rapidjson/cursorstreamwrapper.h
+-rw-r--r--   0        0        0   133763 2023-07-20 13:04:24.607248 cornflakes-3.3.8/inst/ext/rapidjson/include/rapidjson/document.h
+-rw-r--r--   0        0        0    10660 2023-07-20 13:04:24.607248 cornflakes-3.3.8/inst/ext/rapidjson/include/rapidjson/encodedstream.h
+-rw-r--r--   0        0        0    29260 2023-07-20 13:04:24.607248 cornflakes-3.3.8/inst/ext/rapidjson/include/rapidjson/encodings.h
+-rw-r--r--   0        0        0    13025 2023-07-20 13:04:24.607248 cornflakes-3.3.8/inst/ext/rapidjson/include/rapidjson/error/en.h
+-rw-r--r--   0        0        0    13353 2023-07-20 13:04:24.607248 cornflakes-3.3.8/inst/ext/rapidjson/include/rapidjson/error/error.h
+-rw-r--r--   0        0        0     2980 2023-07-20 13:04:24.607248 cornflakes-3.3.8/inst/ext/rapidjson/include/rapidjson/filereadstream.h
+-rw-r--r--   0        0        0     3125 2023-07-20 13:04:24.607248 cornflakes-3.3.8/inst/ext/rapidjson/include/rapidjson/filewritestream.h
+-rw-r--r--   0        0        0     4013 2023-07-20 13:04:24.607248 cornflakes-3.3.8/inst/ext/rapidjson/include/rapidjson/fwd.h
+-rw-r--r--   0        0        0     9271 2023-07-20 13:04:24.607248 cornflakes-3.3.8/inst/ext/rapidjson/include/rapidjson/internal/biginteger.h
+-rw-r--r--   0        0        0     2045 2023-07-20 13:04:24.607248 cornflakes-3.3.8/inst/ext/rapidjson/include/rapidjson/internal/clzll.h
+-rw-r--r--   0        0        0    11559 2023-07-20 13:04:24.607248 cornflakes-3.3.8/inst/ext/rapidjson/include/rapidjson/internal/diyfp.h
+-rw-r--r--   0        0        0     8473 2023-07-20 13:04:24.607248 cornflakes-3.3.8/inst/ext/rapidjson/include/rapidjson/internal/dtoa.h
+-rw-r--r--   0        0        0     2973 2023-07-20 13:04:24.607248 cornflakes-3.3.8/inst/ext/rapidjson/include/rapidjson/internal/ieee754.h
+-rw-r--r--   0        0        0    10110 2023-07-20 13:04:24.607248 cornflakes-3.3.8/inst/ext/rapidjson/include/rapidjson/internal/itoa.h
+-rw-r--r--   0        0        0     6620 2023-07-20 13:04:24.607248 cornflakes-3.3.8/inst/ext/rapidjson/include/rapidjson/internal/meta.h
+-rw-r--r--   0        0        0     3574 2023-07-20 13:04:24.607248 cornflakes-3.3.8/inst/ext/rapidjson/include/rapidjson/internal/pow10.h
+-rw-r--r--   0        0        0    26120 2023-07-20 13:04:24.607248 cornflakes-3.3.8/inst/ext/rapidjson/include/rapidjson/internal/regex.h
+-rw-r--r--   0        0        0     7163 2023-07-20 13:04:24.607248 cornflakes-3.3.8/inst/ext/rapidjson/include/rapidjson/internal/stack.h
+-rw-r--r--   0        0        0     2726 2023-07-20 13:04:24.607248 cornflakes-3.3.8/inst/ext/rapidjson/include/rapidjson/internal/strfunc.h
+-rw-r--r--   0        0        0     9045 2023-07-20 13:04:24.607248 cornflakes-3.3.8/inst/ext/rapidjson/include/rapidjson/internal/strtod.h
+-rw-r--r--   0        0        0     1398 2023-07-20 13:04:24.607248 cornflakes-3.3.8/inst/ext/rapidjson/include/rapidjson/internal/swap.h
+-rw-r--r--   0        0        0     4061 2023-07-20 13:04:24.607248 cornflakes-3.3.8/inst/ext/rapidjson/include/rapidjson/istreamwrapper.h
+-rw-r--r--   0        0        0     2539 2023-07-20 13:04:24.607248 cornflakes-3.3.8/inst/ext/rapidjson/include/rapidjson/memorybuffer.h
+-rw-r--r--   0        0        0     2646 2023-07-20 13:04:24.607248 cornflakes-3.3.8/inst/ext/rapidjson/include/rapidjson/memorystream.h
+-rw-r--r--   0        0        0     8372 2023-07-20 13:04:24.607248 cornflakes-3.3.8/inst/ext/rapidjson/include/rapidjson/msinttypes/inttypes.h
+-rw-r--r--   0        0        0     9386 2023-07-20 13:04:24.607248 cornflakes-3.3.8/inst/ext/rapidjson/include/rapidjson/msinttypes/stdint.h
+-rw-r--r--   0        0        0     2310 2023-07-20 13:04:24.607248 cornflakes-3.3.8/inst/ext/rapidjson/include/rapidjson/ostreamwrapper.h
+-rw-r--r--   0        0        0    63132 2023-07-20 13:04:24.607248 cornflakes-3.3.8/inst/ext/rapidjson/include/rapidjson/pointer.h
+-rw-r--r--   0        0        0    10518 2023-07-20 13:04:24.607248 cornflakes-3.3.8/inst/ext/rapidjson/include/rapidjson/prettywriter.h
+-rw-r--r--   0        0        0    25585 2023-07-20 13:04:24.607248 cornflakes-3.3.8/inst/ext/rapidjson/include/rapidjson/rapidjson.h
+-rw-r--r--   0        0        0    94332 2023-07-20 13:04:24.607248 cornflakes-3.3.8/inst/ext/rapidjson/include/rapidjson/reader.h
+-rw-r--r--   0        0        0   146796 2023-07-20 13:04:24.607248 cornflakes-3.3.8/inst/ext/rapidjson/include/rapidjson/schema.h
+-rw-r--r--   0        0        0     6732 2023-07-20 13:04:24.607248 cornflakes-3.3.8/inst/ext/rapidjson/include/rapidjson/stream.h
+-rw-r--r--   0        0        0     3972 2023-07-20 13:04:24.607248 cornflakes-3.3.8/inst/ext/rapidjson/include/rapidjson/stringbuffer.h
+-rw-r--r--   0        0        0    19752 2023-07-20 13:04:24.611248 cornflakes-3.3.8/inst/ext/rapidjson/include/rapidjson/uri.h
+-rw-r--r--   0        0        0    26856 2023-07-20 13:04:24.611248 cornflakes-3.3.8/inst/ext/rapidjson/include/rapidjson/writer.h
+-rw-r--r--   0        0        0       94 2023-07-20 13:04:24.611248 cornflakes-3.3.8/inst/ext/rapidjson/include_dirs.js
+-rw-r--r--   0        0        0      355 2023-07-20 13:04:24.611248 cornflakes-3.3.8/inst/ext/rapidjson/library.json
+-rw-r--r--   0        0        0     5152 2023-07-20 13:04:24.611248 cornflakes-3.3.8/inst/ext/rapidjson/license.txt
+-rw-r--r--   0        0        0      561 2023-07-20 13:04:24.611248 cornflakes-3.3.8/inst/ext/rapidjson/package.json
+-rw-r--r--   0        0        0     3407 2023-07-20 13:04:24.611248 cornflakes-3.3.8/inst/ext/rapidjson/rapidjson.autopkg
+-rw-r--r--   0        0        0    11146 2023-07-20 13:04:24.611248 cornflakes-3.3.8/inst/ext/rapidjson/readme.md
+-rw-r--r--   0        0        0     8795 2023-07-20 13:04:24.611248 cornflakes-3.3.8/inst/ext/rapidjson/readme.zh-cn.md
+-rw-r--r--   0        0        0      491 2023-07-20 13:04:24.611248 cornflakes-3.3.8/inst/ext/rapidjson/test/CMakeLists.txt
+-rw-r--r--   0        0        0      834 2023-07-20 13:04:24.611248 cornflakes-3.3.8/inst/ext/rapidjson/test/perftest/CMakeLists.txt
+-rw-r--r--   0        0        0    35467 2023-07-20 13:04:24.611248 cornflakes-3.3.8/inst/ext/rapidjson/test/perftest/misctest.cpp
+-rw-r--r--   0        0        0      975 2023-07-20 13:04:24.611248 cornflakes-3.3.8/inst/ext/rapidjson/test/perftest/perftest.cpp
+-rw-r--r--   0        0        0     5756 2023-07-20 13:04:24.611248 cornflakes-3.3.8/inst/ext/rapidjson/test/perftest/perftest.h
+-rw-r--r--   0        0        0     4456 2023-07-20 13:04:24.611248 cornflakes-3.3.8/inst/ext/rapidjson/test/perftest/platformtest.cpp
+-rw-r--r--   0        0        0    16302 2023-07-20 13:04:24.611248 cornflakes-3.3.8/inst/ext/rapidjson/test/perftest/rapidjsontest.cpp
+-rw-r--r--   0        0        0     7218 2023-07-20 13:04:24.611248 cornflakes-3.3.8/inst/ext/rapidjson/test/perftest/schematest.cpp
+-rw-r--r--   0        0        0     3060 2023-07-20 13:04:24.611248 cornflakes-3.3.8/inst/ext/rapidjson/test/unittest/CMakeLists.txt
+-rw-r--r--   0        0        0     9040 2023-07-20 13:04:24.611248 cornflakes-3.3.8/inst/ext/rapidjson/test/unittest/allocatorstest.cpp
+-rw-r--r--   0        0        0     4420 2023-07-20 13:04:24.611248 cornflakes-3.3.8/inst/ext/rapidjson/test/unittest/bigintegertest.cpp
+-rw-r--r--   0        0        0     1092 2023-07-20 13:04:24.611248 cornflakes-3.3.8/inst/ext/rapidjson/test/unittest/clzlltest.cpp
+-rw-r--r--   0        0        0     3733 2023-07-20 13:04:24.611248 cornflakes-3.3.8/inst/ext/rapidjson/test/unittest/cursorstreamwrappertest.cpp
+-rw-r--r--   0        0        0    21279 2023-07-20 13:04:24.611248 cornflakes-3.3.8/inst/ext/rapidjson/test/unittest/documenttest.cpp
+-rw-r--r--   0        0        0     3441 2023-07-20 13:04:24.611248 cornflakes-3.3.8/inst/ext/rapidjson/test/unittest/dtoatest.cpp
+-rw-r--r--   0        0        0    12004 2023-07-20 13:04:24.611248 cornflakes-3.3.8/inst/ext/rapidjson/test/unittest/encodedstreamtest.cpp
+-rw-r--r--   0        0        0    19344 2023-07-20 13:04:24.611248 cornflakes-3.3.8/inst/ext/rapidjson/test/unittest/encodingstest.cpp
+-rw-r--r--   0        0        0     4389 2023-07-20 13:04:24.611248 cornflakes-3.3.8/inst/ext/rapidjson/test/unittest/filestreamtest.cpp
+-rw-r--r--   0        0        0     5837 2023-07-20 13:04:24.611248 cornflakes-3.3.8/inst/ext/rapidjson/test/unittest/fwdtest.cpp
+-rw-r--r--   0        0        0     5419 2023-07-20 13:04:24.611248 cornflakes-3.3.8/inst/ext/rapidjson/test/unittest/istreamwrappertest.cpp
+-rw-r--r--   0        0        0     3956 2023-07-20 13:04:24.611248 cornflakes-3.3.8/inst/ext/rapidjson/test/unittest/itoatest.cpp
+-rw-r--r--   0        0        0     4753 2023-07-20 13:04:24.611248 cornflakes-3.3.8/inst/ext/rapidjson/test/unittest/jsoncheckertest.cpp
+-rw-r--r--   0        0        0     2401 2023-07-20 13:04:24.611248 cornflakes-3.3.8/inst/ext/rapidjson/test/unittest/namespacetest.cpp
+-rw-r--r--   0        0        0     2481 2023-07-20 13:04:24.611248 cornflakes-3.3.8/inst/ext/rapidjson/test/unittest/ostreamwrappertest.cpp
+-rw-r--r--   0        0        0     1457 2023-07-20 13:04:24.611248 cornflakes-3.3.8/inst/ext/rapidjson/test/unittest/platformtest.cpp
+-rw-r--r--   0        0        0    62776 2023-07-20 13:04:24.611248 cornflakes-3.3.8/inst/ext/rapidjson/test/unittest/pointertest.cpp
+-rw-r--r--   0        0        0    10350 2023-07-20 13:04:24.611248 cornflakes-3.3.8/inst/ext/rapidjson/test/unittest/prettywritertest.cpp
+-rw-r--r--   0        0        0    98539 2023-07-20 13:04:24.611248 cornflakes-3.3.8/inst/ext/rapidjson/test/unittest/readertest.cpp
+-rw-r--r--   0        0        0    17263 2023-07-20 13:04:24.611248 cornflakes-3.3.8/inst/ext/rapidjson/test/unittest/regextest.cpp
+-rw-r--r--   0        0        0   150825 2023-07-20 13:04:24.611248 cornflakes-3.3.8/inst/ext/rapidjson/test/unittest/schematest.cpp
+-rw-r--r--   0        0        0     7121 2023-07-20 13:04:24.611248 cornflakes-3.3.8/inst/ext/rapidjson/test/unittest/simdtest.cpp
+-rw-r--r--   0        0        0     1316 2023-07-20 13:04:24.611248 cornflakes-3.3.8/inst/ext/rapidjson/test/unittest/strfunctest.cpp
+-rw-r--r--   0        0        0     5544 2023-07-20 13:04:24.611248 cornflakes-3.3.8/inst/ext/rapidjson/test/unittest/stringbuffertest.cpp
+-rw-r--r--   0        0        0     4256 2023-07-20 13:04:24.611248 cornflakes-3.3.8/inst/ext/rapidjson/test/unittest/strtodtest.cpp
+-rw-r--r--   0        0        0     1527 2023-07-20 13:04:24.611248 cornflakes-3.3.8/inst/ext/rapidjson/test/unittest/unittest.cpp
+-rw-r--r--   0        0        0     3979 2023-07-20 13:04:24.611248 cornflakes-3.3.8/inst/ext/rapidjson/test/unittest/unittest.h
+-rw-r--r--   0        0        0    28512 2023-07-20 13:04:24.611248 cornflakes-3.3.8/inst/ext/rapidjson/test/unittest/uritest.cpp
+-rw-r--r--   0        0        0    57574 2023-07-20 13:04:24.611248 cornflakes-3.3.8/inst/ext/rapidjson/test/unittest/valuetest.cpp
+-rw-r--r--   0        0        0    17932 2023-07-20 13:04:24.615249 cornflakes-3.3.8/inst/ext/rapidjson/test/unittest/writertest.cpp
+-rw-r--r--   0        0        0      369 2023-07-20 13:04:24.615249 cornflakes-3.3.8/inst/ext/rapidjson/test/valgrind.supp
+-rw-r--r--   0        0        0       80 2023-07-20 13:04:25.435267 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/.git
+-rw-r--r--   0        0        0      595 2023-07-20 13:04:26.947302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/.gitignore
+-rw-r--r--   0        0        0     2591 2023-07-20 13:04:26.947302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/.travis.yml
+-rw-r--r--   0        0        0     4940 2023-07-20 13:04:26.947302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/BUILD.bazel
+-rw-r--r--   0        0        0     1220 2023-07-20 13:04:26.947302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/CMakeLists.txt
+-rw-r--r--   0        0        0     6738 2023-07-20 13:04:26.947302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1475 2023-07-20 13:04:26.947302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/LICENSE
+-rw-r--r--   0        0        0      315 2023-07-20 13:04:26.947302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/Makefile.am
+-rw-r--r--   0        0        0     4501 2023-07-20 13:04:26.947302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/README.md
+-rw-r--r--   0        0        0      213 2023-07-20 13:04:26.947302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/WORKSPACE
+-rw-r--r--   0        0        0     3405 2023-07-20 13:04:26.947302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/appveyor.yml
+-rwxr-xr-x   0        0        0     1751 2023-07-20 13:04:26.947302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/ci/build-linux-autotools.sh
+-rwxr-xr-x   0        0        0     1674 2023-07-20 13:04:26.947302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/ci/build-linux-bazel.sh
+-rwxr-xr-x   0        0        0     1922 2023-07-20 13:04:26.947302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/ci/env-linux.sh
+-rwxr-xr-x   0        0        0     1852 2023-07-20 13:04:26.947302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/ci/env-osx.sh
+-rwxr-xr-x   0        0        0     2220 2023-07-20 13:04:26.947302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/ci/get-nprocessors.sh
+-rwxr-xr-x   0        0        0     2229 2023-07-20 13:04:26.947302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/ci/install-linux.sh
+-rwxr-xr-x   0        0        0     1688 2023-07-20 13:04:26.947302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/ci/install-osx.sh
+-rwxr-xr-x   0        0        0     2093 2023-07-20 13:04:26.947302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/ci/log-config.sh
+-rwxr-xr-x   0        0        0     1310 2023-07-20 13:04:26.947302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/ci/travis.sh
+-rw-r--r--   0        0        0      461 2023-07-20 13:04:26.947302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/configure.ac
+-rw-r--r--   0        0        0     5559 2023-07-20 13:04:26.947302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/CHANGES
+-rw-r--r--   0        0        0     9463 2023-07-20 13:04:26.947302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/CMakeLists.txt
+-rw-r--r--   0        0        0     1369 2023-07-20 13:04:26.947302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/CONTRIBUTORS
+-rw-r--r--   0        0        0     1475 2023-07-20 13:04:26.947302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/LICENSE
+-rw-r--r--   0        0        0     7627 2023-07-20 13:04:26.947302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/Makefile.am
+-rw-r--r--   0        0        0    13045 2023-07-20 13:04:26.947302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/README.md
+-rw-r--r--   0        0        0        0 2023-07-20 13:04:26.947302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/build-aux/.keep
+-rw-r--r--   0        0        0      336 2023-07-20 13:04:26.947302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/cmake/gmock.pc.in
+-rw-r--r--   0        0        0      343 2023-07-20 13:04:26.947302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/cmake/gmock_main.pc.in
+-rw-r--r--   0        0        0     6260 2023-07-20 13:04:26.947302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/configure.ac
+-rw-r--r--   0        0        0    28266 2023-07-20 13:04:26.947302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/docs/CheatSheet.md
+-rw-r--r--   0        0        0   128053 2023-07-20 13:04:26.947302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/docs/CookBook.md
+-rw-r--r--   0        0        0     9924 2023-07-20 13:04:26.951302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/docs/DesignDoc.md
+-rw-r--r--   0        0        0      838 2023-07-20 13:04:26.951302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/docs/Documentation.md
+-rw-r--r--   0        0        0    30079 2023-07-20 13:04:26.951302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/docs/ForDummies.md
+-rw-r--r--   0        0        0    23329 2023-07-20 13:04:26.951302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/docs/FrequentlyAskedQuestions.md
+-rw-r--r--   0        0        0     1528 2023-07-20 13:04:26.951302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/docs/KnownIssues.md
+-rw-r--r--   0        0        0    42948 2023-07-20 13:04:26.951302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/include/gmock/gmock-actions.h
+-rw-r--r--   0        0        0     5820 2023-07-20 13:04:26.951302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/include/gmock/gmock-cardinalities.h
+-rw-r--r--   0        0        0   114405 2023-07-20 13:04:26.951302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/include/gmock/gmock-generated-actions.h
+-rw-r--r--   0        0        0    27848 2023-07-20 13:04:26.951302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/include/gmock/gmock-generated-actions.h.pump
+-rw-r--r--   0        0        0    74779 2023-07-20 13:04:26.951302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/include/gmock/gmock-generated-function-mockers.h
+-rw-r--r--   0        0        0    11740 2023-07-20 13:04:26.951302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/include/gmock/gmock-generated-function-mockers.h.pump
+-rw-r--r--   0        0        0    90816 2023-07-20 13:04:26.951302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/include/gmock/gmock-generated-matchers.h
+-rw-r--r--   0        0        0    21921 2023-07-20 13:04:26.951302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/include/gmock/gmock-generated-matchers.h.pump
+-rw-r--r--   0        0        0    18419 2023-07-20 13:04:26.951302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/include/gmock/gmock-generated-nice-strict.h
+-rw-r--r--   0        0        0     6598 2023-07-20 13:04:26.951302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/include/gmock/gmock-generated-nice-strict.h.pump
+-rw-r--r--   0        0        0   190280 2023-07-20 13:04:26.955302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/include/gmock/gmock-matchers.h
+-rw-r--r--   0        0        0     9377 2023-07-20 13:04:26.955302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/include/gmock/gmock-more-actions.h
+-rw-r--r--   0        0        0     3357 2023-07-20 13:04:26.955302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/include/gmock/gmock-more-matchers.h
+-rw-r--r--   0        0        0    72839 2023-07-20 13:04:26.955302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/include/gmock/gmock-spec-builders.h
+-rw-r--r--   0        0        0     3683 2023-07-20 13:04:26.955302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/include/gmock/gmock.h
+-rw-r--r--   0        0        0      329 2023-07-20 13:04:26.955302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/include/gmock/internal/custom/gmock-generated-actions.h
+-rw-r--r--   0        0        0      415 2023-07-20 13:04:26.955302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/include/gmock/internal/custom/gmock-generated-actions.h.pump
+-rw-r--r--   0        0        0     2000 2023-07-20 13:04:26.955302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/include/gmock/internal/custom/gmock-matchers.h
+-rw-r--r--   0        0        0     2159 2023-07-20 13:04:26.955302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/include/gmock/internal/custom/gmock-port.h
+-rw-r--r--   0        0        0    11633 2023-07-20 13:04:26.955302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/include/gmock/internal/gmock-generated-internal-utils.h
+-rw-r--r--   0        0        0     4926 2023-07-20 13:04:26.955302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/include/gmock/internal/gmock-generated-internal-utils.h.pump
+-rw-r--r--   0        0        0    22618 2023-07-20 13:04:26.955302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/include/gmock/internal/gmock-internal-utils.h
+-rw-r--r--   0        0        0     3867 2023-07-20 13:04:26.955302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/include/gmock/internal/gmock-port.h
+-rw-r--r--   0        0        0     3681 2023-07-20 13:04:26.955302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/make/Makefile
+-rw-r--r--   0        0        0     1788 2023-07-20 13:04:26.955302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/msvc/2005/gmock.sln
+-rw-r--r--   0        0        0     3993 2023-07-20 13:04:26.955302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/msvc/2005/gmock.vcproj
+-rw-r--r--   0        0        0      349 2023-07-20 13:04:26.955302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/msvc/2005/gmock_config.vsprops
+-rw-r--r--   0        0        0     3992 2023-07-20 13:04:26.955302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/msvc/2005/gmock_main.vcproj
+-rw-r--r--   0        0        0     4251 2023-07-20 13:04:26.955302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/msvc/2005/gmock_test.vcproj
+-rw-r--r--   0        0        0     2751 2023-07-20 13:04:26.955302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/msvc/2010/gmock.sln
+-rw-r--r--   0        0        0     8485 2023-07-20 13:04:26.955302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/msvc/2010/gmock.vcxproj
+-rw-r--r--   0        0        0      697 2023-07-20 13:04:26.955302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/msvc/2010/gmock_config.props
+-rw-r--r--   0        0        0     8722 2023-07-20 13:04:26.955302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/msvc/2010/gmock_main.vcxproj
+-rw-r--r--   0        0        0     9648 2023-07-20 13:04:26.955302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/msvc/2010/gmock_test.vcxproj
+-rw-r--r--   0        0        0     2698 2023-07-20 13:04:26.955302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/msvc/2015/gmock.sln
+-rw-r--r--   0        0        0     8274 2023-07-20 13:04:26.955302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/msvc/2015/gmock.vcxproj
+-rw-r--r--   0        0        0      677 2023-07-20 13:04:26.955302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/msvc/2015/gmock_config.props
+-rw-r--r--   0        0        0     8505 2023-07-20 13:04:26.955302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/msvc/2015/gmock_main.vcxproj
+-rw-r--r--   0        0        0     9406 2023-07-20 13:04:26.955302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/msvc/2015/gmock_test.vcxproj
+-rwxr-xr-x   0        0        0     8658 2023-07-20 13:04:26.955302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/scripts/fuse_gmock_files.py
+-rw-r--r--   0        0        0    11386 2023-07-20 13:04:26.955302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/scripts/generator/LICENSE
+-rw-r--r--   0        0        0     1327 2023-07-20 13:04:26.955302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/scripts/generator/README
+-rw-r--r--   0        0        0     4216 2023-07-20 13:04:26.955302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/scripts/generator/README.cppclean
+-rwxr-xr-x   0        0        0        0 2023-07-20 13:04:26.955302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/scripts/generator/cpp/__init__.py
+-rwxr-xr-x   0        0        0    62772 2023-07-20 13:04:26.955302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/scripts/generator/cpp/ast.py
+-rwxr-xr-x   0        0        0     8293 2023-07-20 13:04:26.955302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/scripts/generator/cpp/gmock_class.py
+-rwxr-xr-x   0        0        0    11356 2023-07-20 13:04:26.955302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/scripts/generator/cpp/gmock_class_test.py
+-rwxr-xr-x   0        0        0     2004 2023-07-20 13:04:26.955302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/scripts/generator/cpp/keywords.py
+-rwxr-xr-x   0        0        0     9752 2023-07-20 13:04:26.955302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/scripts/generator/cpp/tokenize.py
+-rwxr-xr-x   0        0        0     1153 2023-07-20 13:04:26.955302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/scripts/generator/cpp/utils.py
+-rwxr-xr-x   0        0        0     1091 2023-07-20 13:04:26.955302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/scripts/generator/gmock_gen.py
+-rwxr-xr-x   0        0        0    11167 2023-07-20 13:04:26.955302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/scripts/gmock-config.in
+-rwxr-xr-x   0        0        0    24131 2023-07-20 13:04:26.955302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/scripts/gmock_doctor.py
+-rwxr-xr-x   0        0        0    51024 2023-07-20 13:04:26.959302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/scripts/upload.py
+-rwxr-xr-x   0        0        0     2833 2023-07-20 13:04:26.959302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/scripts/upload_gmock.py
+-rw-r--r--   0        0        0     2150 2023-07-20 13:04:26.959302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/src/gmock-all.cc
+-rw-r--r--   0        0        0     5300 2023-07-20 13:04:26.959302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/src/gmock-cardinalities.cc
+-rw-r--r--   0        0        0     7665 2023-07-20 13:04:26.959302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/src/gmock-internal-utils.cc
+-rw-r--r--   0        0        0    21845 2023-07-20 13:04:26.959302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/src/gmock-matchers.cc
+-rw-r--r--   0        0        0    32771 2023-07-20 13:04:26.959302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/src/gmock-spec-builders.cc
+-rw-r--r--   0        0        0     7930 2023-07-20 13:04:26.959302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/src/gmock.cc
+-rw-r--r--   0        0        0     2593 2023-07-20 13:04:26.959302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/src/gmock_main.cc
+-rw-r--r--   0        0        0     3159 2023-07-20 13:04:26.959302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/test/BUILD.bazel
+-rw-r--r--   0        0        0    50479 2023-07-20 13:04:26.959302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/test/gmock-actions_test.cc
+-rw-r--r--   0        0        0    12329 2023-07-20 13:04:26.959302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/test/gmock-cardinalities_test.cc
+-rw-r--r--   0        0        0    41272 2023-07-20 13:04:26.959302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/test/gmock-generated-actions_test.cc
+-rw-r--r--   0        0        0    20021 2023-07-20 13:04:26.959302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/test/gmock-generated-function-mockers_test.cc
+-rw-r--r--   0        0        0     5320 2023-07-20 13:04:26.959302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/test/gmock-generated-internal-utils_test.cc
+-rw-r--r--   0        0        0    44061 2023-07-20 13:04:26.959302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/test/gmock-generated-matchers_test.cc
+-rw-r--r--   0        0        0    25225 2023-07-20 13:04:26.959302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/test/gmock-internal-utils_test.cc
+-rw-r--r--   0        0        0   221497 2023-07-20 13:04:26.959302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/test/gmock-matchers_test.cc
+-rw-r--r--   0        0        0    24389 2023-07-20 13:04:26.959302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/test/gmock-more-actions_test.cc
+-rw-r--r--   0        0        0    15340 2023-07-20 13:04:26.959302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/test/gmock-nice-strict_test.cc
+-rw-r--r--   0        0        0     2020 2023-07-20 13:04:26.959302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/test/gmock-port_test.cc
+-rw-r--r--   0        0        0    74777 2023-07-20 13:04:26.959302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/test/gmock-spec-builders_test.cc
+-rw-r--r--   0        0        0     2587 2023-07-20 13:04:26.963302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/test/gmock_all_test.cc
+-rw-r--r--   0        0        0     3323 2023-07-20 13:04:26.963302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/test/gmock_ex_test.cc
+-rwxr-xr-x   0        0        0     4384 2023-07-20 13:04:26.963302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/test/gmock_leak_test.py
+-rw-r--r--   0        0        0     3273 2023-07-20 13:04:26.963302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/test/gmock_leak_test_.cc
+-rw-r--r--   0        0        0     1950 2023-07-20 13:04:26.963302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/test/gmock_link2_test.cc
+-rw-r--r--   0        0        0     1950 2023-07-20 13:04:26.963302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/test/gmock_link_test.cc
+-rw-r--r--   0        0        0    19572 2023-07-20 13:04:26.963302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/test/gmock_link_test.h
+-rwxr-xr-x   0        0        0     6105 2023-07-20 13:04:26.963302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/test/gmock_output_test.py
+-rw-r--r--   0        0        0     8640 2023-07-20 13:04:26.963302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/test/gmock_output_test_.cc
+-rw-r--r--   0        0        0    13612 2023-07-20 13:04:26.963302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/test/gmock_output_test_golden.txt
+-rw-r--r--   0        0        0     9323 2023-07-20 13:04:26.963302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/test/gmock_stress_test.cc
+-rw-r--r--   0        0        0     6661 2023-07-20 13:04:26.963302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/test/gmock_test.cc
+-rwxr-xr-x   0        0        0     3667 2023-07-20 13:04:26.963302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/test/gmock_test_utils.py
+-rw-r--r--   0        0        0     6645 2023-07-20 13:04:26.963302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/CHANGES
+-rw-r--r--   0        0        0    11363 2023-07-20 13:04:26.963302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/CMakeLists.txt
+-rw-r--r--   0        0        0     1358 2023-07-20 13:04:26.963302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/CONTRIBUTORS
+-rw-r--r--   0        0        0     1475 2023-07-20 13:04:26.963302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/LICENSE
+-rw-r--r--   0        0        0    11553 2023-07-20 13:04:26.963302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/Makefile.am
+-rw-r--r--   0        0        0    14263 2023-07-20 13:04:26.963302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/README.md
+-rw-r--r--   0        0        0      336 2023-07-20 13:04:26.963302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/cmake/gtest.pc.in
+-rw-r--r--   0        0        0      359 2023-07-20 13:04:26.963302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/cmake/gtest_main.pc.in
+-rw-r--r--   0        0        0    12013 2023-07-20 13:04:26.963302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/cmake/internal_utils.cmake
+-rw-r--r--   0        0        0    10623 2023-07-20 13:04:26.963302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/codegear/gtest.cbproj
+-rw-r--r--   0        0        0     2061 2023-07-20 13:04:26.963302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/codegear/gtest.groupproj
+-rw-r--r--   0        0        0     1903 2023-07-20 13:04:26.963302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/codegear/gtest_all.cc
+-rw-r--r--   0        0        0     2033 2023-07-20 13:04:26.963302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/codegear/gtest_link.cc
+-rw-r--r--   0        0        0     8662 2023-07-20 13:04:26.963302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/codegear/gtest_main.cbproj
+-rw-r--r--   0        0        0     8778 2023-07-20 13:04:26.963302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/codegear/gtest_unittest.cbproj
+-rw-r--r--   0        0        0     2574 2023-07-20 13:04:26.963302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/configure.ac
+-rw-r--r--   0        0        0     3996 2023-07-20 13:04:26.963302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/docs/Pkgconfig.md
+-rw-r--r--   0        0        0     6958 2023-07-20 13:04:26.963302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/docs/PumpManual.md
+-rw-r--r--   0        0        0     8246 2023-07-20 13:04:26.963302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/docs/XcodeGuide.md
+-rw-r--r--   0        0        0    93685 2023-07-20 13:04:26.963302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/docs/advanced.md
+-rw-r--r--   0        0        0    47943 2023-07-20 13:04:26.963302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/docs/faq.md
+-rw-r--r--   0        0        0    26445 2023-07-20 13:04:26.963302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/docs/primer.md
+-rw-r--r--   0        0        0     1329 2023-07-20 13:04:26.963302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/docs/samples.md
+-rw-r--r--   0        0        0    14349 2023-07-20 13:04:26.963302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/include/gtest/gtest-death-test.h
+-rw-r--r--   0        0        0     9197 2023-07-20 13:04:26.963302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/include/gtest/gtest-message.h
+-rw-r--r--   0        0        0    77427 2023-07-20 13:04:26.963302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/include/gtest/gtest-param-test.h
+-rw-r--r--   0        0        0    19875 2023-07-20 13:04:26.963302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/include/gtest/gtest-param-test.h.pump
+-rw-r--r--   0        0        0    39278 2023-07-20 13:04:26.963302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/include/gtest/gtest-printers.h
+-rw-r--r--   0        0        0     9939 2023-07-20 13:04:26.963302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/include/gtest/gtest-spi.h
+-rw-r--r--   0        0        0     6509 2023-07-20 13:04:26.963302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/include/gtest/gtest-test-part.h
+-rw-r--r--   0        0        0    10500 2023-07-20 13:04:26.967302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/include/gtest/gtest-typed-test.h
+-rw-r--r--   0        0        0    88660 2023-07-20 13:04:26.967302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/include/gtest/gtest.h
+-rw-r--r--   0        0        0    14908 2023-07-20 13:04:26.967302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/include/gtest/gtest_pred_impl.h
+-rw-r--r--   0        0        0     2527 2023-07-20 13:04:26.967302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/include/gtest/gtest_prod.h
+-rw-r--r--   0        0        0     3066 2023-07-20 13:04:26.967302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/include/gtest/internal/custom/gtest-port.h
+-rw-r--r--   0        0        0     2099 2023-07-20 13:04:26.967302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/include/gtest/internal/custom/gtest-printers.h
+-rw-r--r--   0        0        0     2192 2023-07-20 13:04:26.967302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/include/gtest/internal/custom/gtest.h
+-rw-r--r--   0        0        0    11192 2023-07-20 13:04:26.967302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/include/gtest/internal/gtest-death-test-internal.h
+-rw-r--r--   0        0        0     9558 2023-07-20 13:04:26.967302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/include/gtest/internal/gtest-filepath.h
+-rw-r--r--   0        0        0    48549 2023-07-20 13:04:26.967302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/include/gtest/internal/gtest-internal.h
+-rw-r--r--   0        0        0     8424 2023-07-20 13:04:26.967302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/include/gtest/internal/gtest-linked_ptr.h
+-rw-r--r--   0        0        0   192179 2023-07-20 13:04:26.967302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/include/gtest/internal/gtest-param-util-generated.h
+-rw-r--r--   0        0        0     8901 2023-07-20 13:04:26.967302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/include/gtest/internal/gtest-param-util-generated.h.pump
+-rw-r--r--   0        0        0    27669 2023-07-20 13:04:26.967302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/include/gtest/internal/gtest-param-util.h
+-rw-r--r--   0        0        0     3723 2023-07-20 13:04:26.967302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/include/gtest/internal/gtest-port-arch.h
+-rw-r--r--   0        0        0    95013 2023-07-20 13:04:26.967302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/include/gtest/internal/gtest-port.h
+-rw-r--r--   0        0        0     6907 2023-07-20 13:04:26.967302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/include/gtest/internal/gtest-string.h
+-rw-r--r--   0        0        0    28617 2023-07-20 13:04:26.967302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/include/gtest/internal/gtest-tuple.h
+-rw-r--r--   0        0        0     9620 2023-07-20 13:04:26.967302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/include/gtest/internal/gtest-tuple.h.pump
+-rw-r--r--   0        0        0   186354 2023-07-20 13:04:26.971302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/include/gtest/internal/gtest-type-util.h
+-rw-r--r--   0        0        0    10005 2023-07-20 13:04:26.971302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/include/gtest/internal/gtest-type-util.h.pump
+-rw-r--r--   0        0        0    13302 2023-07-20 13:04:26.971302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/m4/acx_pthread.m4
+-rw-r--r--   0        0        0     3217 2023-07-20 13:04:26.971302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/m4/gtest.m4
+-rw-r--r--   0        0        0     2753 2023-07-20 13:04:26.971302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/make/Makefile
+-rw-r--r--   0        0        0     3491 2023-07-20 13:04:26.971302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/msvc/2010/gtest-md.sln
+-rw-r--r--   0        0        0     8417 2023-07-20 13:04:26.971302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/msvc/2010/gtest-md.vcxproj
+-rw-r--r--   0        0        0      691 2023-07-20 13:04:26.971302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/msvc/2010/gtest-md.vcxproj.filters
+-rw-r--r--   0        0        0     3467 2023-07-20 13:04:26.971302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/msvc/2010/gtest.sln
+-rw-r--r--   0        0        0     8425 2023-07-20 13:04:26.971302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/msvc/2010/gtest.vcxproj
+-rw-r--r--   0        0        0      691 2023-07-20 13:04:26.971302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/msvc/2010/gtest.vcxproj.filters
+-rw-r--r--   0        0        0     8605 2023-07-20 13:04:26.971302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/msvc/2010/gtest_main-md.vcxproj
+-rw-r--r--   0        0        0      692 2023-07-20 13:04:26.971302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/msvc/2010/gtest_main-md.vcxproj.filters
+-rw-r--r--   0        0        0     8884 2023-07-20 13:04:26.971302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/msvc/2010/gtest_main.vcxproj
+-rw-r--r--   0        0        0      692 2023-07-20 13:04:26.971302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/msvc/2010/gtest_main.vcxproj.filters
+-rw-r--r--   0        0        0    11669 2023-07-20 13:04:26.971302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/msvc/2010/gtest_prod_test-md.vcxproj
+-rw-r--r--   0        0        0      934 2023-07-20 13:04:26.971302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/msvc/2010/gtest_prod_test-md.vcxproj.filters
+-rw-r--r--   0        0        0    11302 2023-07-20 13:04:26.971302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/msvc/2010/gtest_prod_test.vcxproj
+-rw-r--r--   0        0        0      934 2023-07-20 13:04:26.971302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/msvc/2010/gtest_prod_test.vcxproj.filters
+-rw-r--r--   0        0        0    11067 2023-07-20 13:04:26.971302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/msvc/2010/gtest_unittest-md.vcxproj
+-rw-r--r--   0        0        0      697 2023-07-20 13:04:26.971302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/msvc/2010/gtest_unittest-md.vcxproj.filters
+-rw-r--r--   0        0        0    10704 2023-07-20 13:04:26.971302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/msvc/2010/gtest_unittest.vcxproj
+-rw-r--r--   0        0        0      697 2023-07-20 13:04:26.971302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/msvc/2010/gtest_unittest.vcxproj.filters
+-rw-r--r--   0        0        0     4294 2023-07-20 13:04:26.971302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/samples/prime_tables.h
+-rw-r--r--   0        0        0     2503 2023-07-20 13:04:26.971302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/samples/sample1.cc
+-rw-r--r--   0        0        0     1937 2023-07-20 13:04:26.971302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/samples/sample1.h
+-rw-r--r--   0        0        0     5023 2023-07-20 13:04:26.971302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/samples/sample10_unittest.cc
+-rw-r--r--   0        0        0     5156 2023-07-20 13:04:26.971302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/samples/sample1_unittest.cc
+-rw-r--r--   0        0        0     2298 2023-07-20 13:04:26.971302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/samples/sample2.cc
+-rw-r--r--   0        0        0     3006 2023-07-20 13:04:26.971302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/samples/sample2.h
+-rw-r--r--   0        0        0     3953 2023-07-20 13:04:26.971302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/samples/sample2_unittest.cc
+-rw-r--r--   0        0        0     5365 2023-07-20 13:04:26.971302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/samples/sample3-inl.h
+-rw-r--r--   0        0        0     5398 2023-07-20 13:04:26.971302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/samples/sample3_unittest.cc
+-rw-r--r--   0        0        0     1927 2023-07-20 13:04:26.971302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/samples/sample4.cc
+-rw-r--r--   0        0        0     2083 2023-07-20 13:04:26.971302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/samples/sample4.h
+-rw-r--r--   0        0        0     1939 2023-07-20 13:04:26.971302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/samples/sample4_unittest.cc
+-rw-r--r--   0        0        0     6616 2023-07-20 13:04:26.971302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/samples/sample5_unittest.cc
+-rw-r--r--   0        0        0     9016 2023-07-20 13:04:26.971302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/samples/sample6_unittest.cc
+-rw-r--r--   0        0        0     4654 2023-07-20 13:04:26.971302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/samples/sample7_unittest.cc
+-rw-r--r--   0        0        0     6968 2023-07-20 13:04:26.971302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/samples/sample8_unittest.cc
+-rw-r--r--   0        0        0     5948 2023-07-20 13:04:26.971302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/samples/sample9_unittest.cc
+-rw-r--r--   0        0        0     2919 2023-07-20 13:04:26.971302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/scripts/common.py
+-rwxr-xr-x   0        0        0     8896 2023-07-20 13:04:26.971302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/scripts/fuse_gtest_files.py
+-rwxr-xr-x   0        0        0    21850 2023-07-20 13:04:26.971302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/scripts/gen_gtest_pred_impl.py
+-rwxr-xr-x   0        0        0    10087 2023-07-20 13:04:26.971302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/scripts/gtest-config.in
+-rwxr-xr-x   0        0        0    23673 2023-07-20 13:04:26.971302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/scripts/pump.py
+-rwxr-xr-x   0        0        0     6132 2023-07-20 13:04:26.971302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/scripts/release_docs.py
+-rw-r--r--   0        0        0     1802 2023-07-20 13:04:26.971302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/scripts/test/Makefile
+-rwxr-xr-x   0        0        0    51025 2023-07-20 13:04:26.971302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/scripts/upload.py
+-rwxr-xr-x   0        0        0     2851 2023-07-20 13:04:26.971302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/scripts/upload_gtest.py
+-rw-r--r--   0        0        0     2173 2023-07-20 13:04:26.971302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/src/gtest-all.cc
+-rw-r--r--   0        0        0    56716 2023-07-20 13:04:26.971302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/src/gtest-death-test.cc
+-rw-r--r--   0        0        0    14507 2023-07-20 13:04:26.971302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/src/gtest-filepath.cc
+-rw-r--r--   0        0        0    45140 2023-07-20 13:04:26.971302 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/src/gtest-internal-inl.h
+-rw-r--r--   0        0        0    43284 2023-07-20 13:04:26.975303 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/src/gtest-port.cc
+-rw-r--r--   0        0        0    15205 2023-07-20 13:04:26.975303 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/src/gtest-printers.cc
+-rw-r--r--   0        0        0     3831 2023-07-20 13:04:26.975303 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/src/gtest-test-part.cc
+-rw-r--r--   0        0        0     3961 2023-07-20 13:04:26.975303 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/src/gtest-typed-test.cc
+-rw-r--r--   0        0        0   213031 2023-07-20 13:04:26.975303 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/src/gtest.cc
+-rw-r--r--   0        0        0     1767 2023-07-20 13:04:26.975303 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/src/gtest_main.cc
+-rw-r--r--   0        0        0     9762 2023-07-20 13:04:26.975303 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/BUILD.bazel
+-rw-r--r--   0        0        0     3679 2023-07-20 13:04:26.975303 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest-death-test_ex_test.cc
+-rw-r--r--   0        0        0    44749 2023-07-20 13:04:26.975303 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest-death-test_test.cc
+-rw-r--r--   0        0        0    22712 2023-07-20 13:04:26.975303 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest-filepath_test.cc
+-rw-r--r--   0        0        0     4125 2023-07-20 13:04:26.975303 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest-linked_ptr_test.cc
+-rw-r--r--   0        0        0     9844 2023-07-20 13:04:26.975303 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest-listener_test.cc
+-rw-r--r--   0        0        0     5302 2023-07-20 13:04:26.975303 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest-message_test.cc
+-rw-r--r--   0        0        0     7672 2023-07-20 13:04:26.975303 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest-options_test.cc
+-rw-r--r--   0        0        0     2820 2023-07-20 13:04:26.975303 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest-param-test2_test.cc
+-rw-r--r--   0        0        0    40385 2023-07-20 13:04:26.975303 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest-param-test_test.cc
+-rw-r--r--   0        0        0     2296 2023-07-20 13:04:26.975303 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest-param-test_test.h
+-rw-r--r--   0        0        0    40423 2023-07-20 13:04:26.975303 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest-port_test.cc
+-rw-r--r--   0        0        0    56551 2023-07-20 13:04:26.975303 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest-printers_test.cc
+-rw-r--r--   0        0        0     7282 2023-07-20 13:04:26.975303 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest-test-part_test.cc
+-rw-r--r--   0        0        0     9250 2023-07-20 13:04:26.975303 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest-tuple_test.cc
+-rw-r--r--   0        0        0     2054 2023-07-20 13:04:26.975303 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest-typed-test2_test.cc
+-rw-r--r--   0        0        0    12330 2023-07-20 13:04:26.975303 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest-typed-test_test.cc
+-rw-r--r--   0        0        0     2485 2023-07-20 13:04:26.975303 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest-typed-test_test.h
+-rw-r--r--   0        0        0    13207 2023-07-20 13:04:26.975303 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest-unittest-api_test.cc
+-rw-r--r--   0        0        0     2203 2023-07-20 13:04:26.975303 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_all_test.cc
+-rw-r--r--   0        0        0     3946 2023-07-20 13:04:26.979303 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_assert_by_exception_test.cc
+-rwxr-xr-x   0        0        0     7327 2023-07-20 13:04:26.979303 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_break_on_failure_unittest.py
+-rw-r--r--   0        0        0     3283 2023-07-20 13:04:26.979303 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_break_on_failure_unittest_.cc
+-rwxr-xr-x   0        0        0     9890 2023-07-20 13:04:26.979303 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_catch_exceptions_test.py
+-rw-r--r--   0        0        0     8874 2023-07-20 13:04:26.979303 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_catch_exceptions_test_.cc
+-rwxr-xr-x   0        0        0     4911 2023-07-20 13:04:26.979303 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_color_test.py
+-rw-r--r--   0        0        0     2548 2023-07-20 13:04:26.979303 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_color_test_.cc
+-rwxr-xr-x   0        0        0     4038 2023-07-20 13:04:26.979303 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_env_var_test.py
+-rw-r--r--   0        0        0     3515 2023-07-20 13:04:26.979303 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_env_var_test_.cc
+-rw-r--r--   0        0        0     6508 2023-07-20 13:04:26.979303 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_environment_test.cc
+-rwxr-xr-x   0        0        0    21397 2023-07-20 13:04:26.979303 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_filter_unittest.py
+-rw-r--r--   0        0        0     3507 2023-07-20 13:04:26.979303 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_filter_unittest_.cc
+-rwxr-xr-x   0        0        0     5868 2023-07-20 13:04:26.979303 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_help_test.py
+-rw-r--r--   0        0        0     2131 2023-07-20 13:04:26.979303 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_help_test_.cc
+-rw-r--r--   0        0        0     5527 2023-07-20 13:04:26.979303 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_json_outfiles_test.py
+-rw-r--r--   0        0        0    20882 2023-07-20 13:04:26.979303 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_json_output_unittest.py
+-rw-r--r--   0        0        0     2411 2023-07-20 13:04:26.979303 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_json_test_utils.py
+-rwxr-xr-x   0        0        0     6537 2023-07-20 13:04:26.979303 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_list_tests_unittest.py
+-rw-r--r--   0        0        0     4710 2023-07-20 13:04:26.979303 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_list_tests_unittest_.cc
+-rw-r--r--   0        0        0     1884 2023-07-20 13:04:26.979303 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_main_unittest.cc
+-rw-r--r--   0        0        0     2447 2023-07-20 13:04:26.979303 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_no_test_unittest.cc
+-rwxr-xr-x   0        0        0    12437 2023-07-20 13:04:26.979303 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_output_test.py
+-rw-r--r--   0        0        0    33338 2023-07-20 13:04:26.979303 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_output_test_.cc
+-rw-r--r--   0        0        0    30233 2023-07-20 13:04:26.979303 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_output_test_golden_lin.txt
+-rw-r--r--   0        0        0    77378 2023-07-20 13:04:26.979303 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_pred_impl_unittest.cc
+-rw-r--r--   0        0        0     4298 2023-07-20 13:04:26.979303 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_premature_exit_test.cc
+-rw-r--r--   0        0        0     2196 2023-07-20 13:04:26.979303 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_prod_test.cc
+-rw-r--r--   0        0        0     7571 2023-07-20 13:04:26.979303 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_repeat_test.cc
+-rwxr-xr-x   0        0        0    12549 2023-07-20 13:04:26.979303 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_shuffle_test.py
+-rw-r--r--   0        0        0     3306 2023-07-20 13:04:26.979303 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_shuffle_test_.cc
+-rw-r--r--   0        0        0     2221 2023-07-20 13:04:26.979303 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_sole_header_test.cc
+-rw-r--r--   0        0        0     9381 2023-07-20 13:04:26.979303 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_stress_test.cc
+-rwxr-xr-x   0        0        0    10825 2023-07-20 13:04:26.979303 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_test_utils.py
+-rw-r--r--   0        0        0     2520 2023-07-20 13:04:26.979303 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_testbridge_test.py
+-rw-r--r--   0        0        0     1965 2023-07-20 13:04:26.979303 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_testbridge_test_.cc
+-rw-r--r--   0        0        0     3444 2023-07-20 13:04:26.979303 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_throw_on_failure_ex_test.cc
+-rwxr-xr-x   0        0        0     5766 2023-07-20 13:04:26.979303 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_throw_on_failure_test.py
+-rw-r--r--   0        0        0     3104 2023-07-20 13:04:26.979303 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_throw_on_failure_test_.cc
+-rwxr-xr-x   0        0        0     2513 2023-07-20 13:04:26.979303 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_uninitialized_test.py
+-rw-r--r--   0        0        0     1921 2023-07-20 13:04:26.979303 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_uninitialized_test_.cc
+-rw-r--r--   0        0        0   251334 2023-07-20 13:04:26.979303 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_unittest.cc
+-rw-r--r--   0        0        0     1968 2023-07-20 13:04:26.979303 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_xml_outfile1_test_.cc
+-rw-r--r--   0        0        0     1968 2023-07-20 13:04:26.979303 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_xml_outfile2_test_.cc
+-rwxr-xr-x   0        0        0     5593 2023-07-20 13:04:26.979303 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_xml_outfiles_test.py
+-rwxr-xr-x   0        0        0    17080 2023-07-20 13:04:26.983303 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_xml_output_unittest.py
+-rw-r--r--   0        0        0     6100 2023-07-20 13:04:26.983303 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_xml_output_unittest_.cc
+-rwxr-xr-x   0        0        0     9221 2023-07-20 13:04:26.983303 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_xml_test_utils.py
+-rw-r--r--   0        0        0     1718 2023-07-20 13:04:26.983303 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/production.cc
+-rw-r--r--   0        0        0     2158 2023-07-20 13:04:26.983303 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/production.h
+-rw-r--r--   0        0        0      983 2023-07-20 13:04:26.983303 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/xcode/Config/DebugProject.xcconfig
+-rw-r--r--   0        0        0      551 2023-07-20 13:04:26.983303 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/xcode/Config/FrameworkTarget.xcconfig
+-rw-r--r--   0        0        0     1199 2023-07-20 13:04:26.983303 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/xcode/Config/General.xcconfig
+-rw-r--r--   0        0        0      993 2023-07-20 13:04:26.983303 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/xcode/Config/ReleaseProject.xcconfig
+-rw-r--r--   0        0        0      587 2023-07-20 13:04:26.983303 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/xcode/Config/StaticLibraryTarget.xcconfig
+-rw-r--r--   0        0        0      238 2023-07-20 13:04:26.983303 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/xcode/Config/TestTarget.xcconfig
+-rw-r--r--   0        0        0     1010 2023-07-20 13:04:26.983303 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/xcode/Resources/Info.plist
+-rw-r--r--   0        0        0      846 2023-07-20 13:04:26.983303 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/xcode/Samples/FrameworkSample/Info.plist
+-rw-r--r--   0        0        0    16060 2023-07-20 13:04:26.983303 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/xcode/Samples/FrameworkSample/WidgetFramework.xcodeproj/project.pbxproj
+-rw-r--r--   0        0        0     2354 2023-07-20 13:04:26.983303 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/xcode/Samples/FrameworkSample/runtests.sh
+-rw-r--r--   0        0        0     2307 2023-07-20 13:04:26.983303 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/xcode/Samples/FrameworkSample/widget.cc
+-rw-r--r--   0        0        0     2270 2023-07-20 13:04:26.983303 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/xcode/Samples/FrameworkSample/widget.h
+-rw-r--r--   0        0        0     2669 2023-07-20 13:04:26.983303 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/xcode/Samples/FrameworkSample/widget_test.cc
+-rw-r--r--   0        0        0     2587 2023-07-20 13:04:26.983303 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/xcode/Scripts/runtests.sh
+-rwxr-xr-x   0        0        0     4535 2023-07-20 13:04:26.983303 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/xcode/Scripts/versiongenerate.py
+-rw-r--r--   0        0        0    54223 2023-07-20 13:04:26.983303 cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/xcode/gtest.xcodeproj/project.pbxproj
+-rwxr-xr-x   0        0        0     3294 2023-07-20 13:04:24.615249 cornflakes-3.3.8/inst/ext/rapidjson/travis-doxygen.sh
+-rw-r--r--   0        0        0       45 2023-07-20 13:04:22.319204 cornflakes-3.3.8/inst/ext/strtk/.git
+-rw-r--r--   0        0        0      347 2023-07-20 13:04:26.991303 cornflakes-3.3.8/inst/ext/strtk/.travis.yml
+-rw-r--r--   0        0        0     7507 2023-07-20 13:04:26.991303 cornflakes-3.3.8/inst/ext/strtk/Makefile
+-rw-r--r--   0        0        0     3590 2023-07-20 13:04:26.991303 cornflakes-3.3.8/inst/ext/strtk/readme.txt
+-rw-r--r--   0        0        0   885153 2023-07-20 13:04:26.995303 cornflakes-3.3.8/inst/ext/strtk/strtk.hpp
+-rw-r--r--   0        0        0     7614 2023-07-20 13:04:26.995303 cornflakes-3.3.8/inst/ext/strtk/strtk_bloom_filter_example.cpp
+-rw-r--r--   0        0        0     2568 2023-07-20 13:04:26.995303 cornflakes-3.3.8/inst/ext/strtk/strtk_combinations.cpp
+-rw-r--r--   0        0        0     2101 2023-07-20 13:04:26.995303 cornflakes-3.3.8/inst/ext/strtk/strtk_combinator_example.cpp
+-rw-r--r--   0        0        0     5881 2023-07-20 13:04:26.995303 cornflakes-3.3.8/inst/ext/strtk/strtk_converters_example.cpp
+-rw-r--r--   0        0        0    72459 2023-07-20 13:04:26.995303 cornflakes-3.3.8/inst/ext/strtk/strtk_examples.cpp
+-rw-r--r--   0        0        0     3988 2023-07-20 13:04:26.995303 cornflakes-3.3.8/inst/ext/strtk/strtk_glober.cpp
+-rw-r--r--   0        0        0     4339 2023-07-20 13:04:26.995303 cornflakes-3.3.8/inst/ext/strtk/strtk_hexview.cpp
+-rw-r--r--   0        0        0     3730 2023-07-20 13:04:26.995303 cornflakes-3.3.8/inst/ext/strtk/strtk_ipv4_parser.cpp
+-rw-r--r--   0        0        0    14409 2023-07-20 13:04:26.995303 cornflakes-3.3.8/inst/ext/strtk/strtk_keyvalue_example.cpp
+-rw-r--r--   0        0        0     4938 2023-07-20 13:04:26.995303 cornflakes-3.3.8/inst/ext/strtk/strtk_nth_combination_example.cpp
+-rw-r--r--   0        0        0     4843 2023-07-20 13:04:26.995303 cornflakes-3.3.8/inst/ext/strtk/strtk_numstats.cpp
+-rw-r--r--   0        0        0    27214 2023-07-20 13:04:26.995303 cornflakes-3.3.8/inst/ext/strtk/strtk_parse_test.cpp
+-rw-r--r--   0        0        0     5133 2023-07-20 13:04:26.995303 cornflakes-3.3.8/inst/ext/strtk/strtk_period_parser.cpp
+-rw-r--r--   0        0        0     2547 2023-07-20 13:04:26.995303 cornflakes-3.3.8/inst/ext/strtk/strtk_random_line.cpp
+-rw-r--r--   0        0        0     2372 2023-07-20 13:04:26.995303 cornflakes-3.3.8/inst/ext/strtk/strtk_randomizer.cpp
+-rw-r--r--   0        0        0     6261 2023-07-20 13:04:26.995303 cornflakes-3.3.8/inst/ext/strtk/strtk_search_trie_example.cpp
+-rw-r--r--   0        0        0    32474 2023-07-20 13:04:26.995303 cornflakes-3.3.8/inst/ext/strtk/strtk_serializer_example.cpp
+-rw-r--r--   0        0        0     2364 2023-07-20 13:04:26.995303 cornflakes-3.3.8/inst/ext/strtk/strtk_text_parser_example01.cpp
+-rw-r--r--   0        0        0     3811 2023-07-20 13:04:26.995303 cornflakes-3.3.8/inst/ext/strtk/strtk_text_parser_example02.cpp
+-rw-r--r--   0        0        0    31242 2023-07-20 13:04:26.995303 cornflakes-3.3.8/inst/ext/strtk/strtk_tokengrid_example.cpp
+-rw-r--r--   0        0        0    52321 2023-07-20 13:04:26.995303 cornflakes-3.3.8/inst/ext/strtk/strtk_tokenizer_cmp.cpp
+-rw-r--r--   0        0        0   131409 2023-07-20 13:04:26.999303 cornflakes-3.3.8/inst/ext/strtk/strtk_tokenizer_test.cpp
+-rw-r--r--   0        0        0     4174 2023-07-20 13:04:26.999303 cornflakes-3.3.8/inst/ext/strtk/strtk_wordfreq.cpp
+-rw-r--r--   0        0        0     4611 2023-07-20 13:04:19.743167 cornflakes-3.3.8/pyproject.toml
+-rw-r--r--   0        0        0     6411 1970-01-01 00:00:00.000000 cornflakes-3.3.8/setup.py
+-rw-r--r--   0        0        0     5815 1970-01-01 00:00:00.000000 cornflakes-3.3.8/PKG-INFO
```

### Comparing `cornflakes-3.3.7/LICENSE` & `cornflakes-3.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/README.rst` & `cornflakes-3.3.8/README.rst`

 * *Files 13% similar despite different names*

```diff
@@ -37,30 +37,38 @@
 
    pip install cornflakes
 
 .. code::
 
     pip install git+https://github.com/semmjon/cornflakes
 
+.. warning::
+    Please be careful when using this Python module. Currently it is only developed / tested by me, which is why it has a high update / change rate. I'm actually trying to be compatible with implementations, but I can't guarantee this at the moment. The module is currently still in a beta state and is not recommended for productive use.
+
+    In the near future I plan to revise the documentation / examples and write an introductory blog article, as I find implemented features and planned ideas to be quite cool and useful (and don't see them in any other package or find them to be quite user-friendly).
+
 Information
 -----------
 
 The Python module "cornflakes" was started as a hobby project and offers an alternative to Pydantic for managing configurations and data structures. It allows creating generic and easy to manage configurations for your project. Unlike Pydantic, which is based on inheritance, "cornflakes" uses a decorator (similar to dataclass) to map data structures.
 
 In addition to a dataclass decorator with additional functionality, there is also a config decorator. This makes it possible to read the dataclass from configuration files. This can be very useful if you want to save your application configurations to a file.
 
 The module also has a click wrapper that simplifies the implementation of command line applications. By integrating the Rich module, the application is additionally equipped with colors and other functions.
 
 There are other useful methods in the base of the module that are generally useful for Python development. These can help you develop your projects faster and more efficiently.
 
 Short Term RoadMap:
 ~~~~~~~~~~~~~~~~~~~~
 
+- Change Code Annotations
+    - remove Any annotations if possible
+    - change Protocol Annotations to specific type classes
 - Enrich json methods
-- Fix / Test the to_<file-format> Methods
+- Fix / Test the to_<file-format> Methods (specially yaml)
 
 Development
 -----------
 
 Prerequisites
 ~~~~~~~~~~~~~
```

### Comparing `cornflakes-3.3.7/cornflakes/builder/_generate_config_module.py` & `cornflakes-3.3.8/cornflakes/builder/_generate_config_module.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,21 +4,20 @@
 import inspect
 import logging
 import os
 import sysconfig
 from types import ModuleType
 from typing import Dict, List, Optional, Union
 
-from cornflakes.common import unquoted_string
-from cornflakes.decorator import field
-from cornflakes.decorator.config import config_files, config_group, is_config
-from cornflakes.decorator.types import ConfigArguments, Loader
+from cornflakes.decorator.dataclasses import config_files, field, is_config
+from cornflakes.decorator.dataclasses.config import config_group
+from cornflakes.types import Constants, Loader
 
-TEMPLATE = '''"""Template Module."""
-from cornflakes import config_group
+TEMPLATE = f'''"""Template Module."""
+from {import_module("cornflakes.decorator.dataclasses").__name__} import config_group
 
 
 @config_group
 class Config:
     """Template Class."""
 
     # modules
@@ -29,64 +28,58 @@
 
 
 def generate_config_module(  # noqa: C901
     source_module: Union[ModuleType, str],
     source_config: Optional[Union[Dict[str, Union[List[str], str]], List[str], str]] = None,
     target_module_file: Optional[str] = None,
     class_name: Optional[str] = None,
-    loader: Loader = Loader.FILE_LOADER,
+    loader: Loader = Loader.FILE,
     module_description: str = "Automatically generated Default Config.",
     class_description: str = "Main config class of the module.",
     *args,
     **kwargs,
 ):
     """Module with function to generate automatically config group module."""
     declaration = []
     ini_config_objects = {}
     imports = []
     extra_imports = []
-    files = kwargs.get(ConfigArguments.files.name, [])
+    files = kwargs.get(Constants.config_decorator_args.FILES, [])
     files = files if isinstance(files, list) else [files]
     os.environ["CORNFLAKES_GENERATING_CONFIG_MODULE"] = "True"
 
-    if ConfigArguments.files.name not in kwargs:
-        kwargs.update({ConfigArguments.files.name: source_config})
-
-    if not target_module_file:
-        target_module_file = f'{source_module.__name__.replace(".", "/")}/default.py'
+    if Constants.config_decorator_args.FILES not in kwargs:
+        kwargs.update({Constants.config_decorator_args.FILES: source_config})
 
     template = TEMPLATE  # create copy of template
 
     if class_name:
         template = template.replace("Config", class_name)
 
     template = template.replace("Template Module.", module_description)
     template = template.replace("Template Class.", class_description)
 
+    if isinstance(source_module, str):
+        source_module = import_module(source_module)
+
+    if not target_module_file:
+        target_module_file = f'{source_module.__name__.replace(".", "/")}/default.py'
+
     # Write Template to prevent import errors
     with open(target_module_file, "w") as file:
         file.write(template)
 
-    if isinstance(source_module, str):
-        source_module = import_module(source_module)
-
     for cfg_name, cfg_class in inspect.getmembers(source_module):
         if is_dataclass(cfg_class) and inspect.isclass(cfg_class) and is_config(cfg_class):
             cfg = getattr(cfg_class, str(loader.value))(files=source_config)
             ini_config_objects.update(cfg)
             imports.append(cfg_name)
             files.extend([file for file in config_files(cfg_class) if file and file not in files])
 
-    if ConfigArguments.filter_function.name in kwargs:
-        filter_function = kwargs.pop(ConfigArguments.filter_function.name)
-        kwargs[ConfigArguments.filter_function.name] = unquoted_string(filter_function.__name__)
-        extra_imports.append(f"from {filter_function.__module__} import {filter_function.__name__}")
-
     logging.debug(f"Found configs: {imports}")
-
     declaration.extend(
         [
             (
                 f"{cfg_name}: List[{cfg[0].__class__.__name__}] = "
                 f"{field.__name__}(default_factory={cfg.__class__.__name__})"
                 if isinstance(cfg, list)
                 else f"{cfg_name}: {cfg.__class__.__name__} = {field.__name__}(default_factory={cfg.__class__.__name__})"
```

### Comparing `cornflakes-3.3.7/cornflakes/builder/_generate_enum_module.py` & `cornflakes-3.3.8/cornflakes/builder/_generate_enum_module.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from types import ModuleType
 from typing import Any, Dict, List, Optional, Union
 
 
 def generate_enum_module(
     title: Optional[str],
     sources: Union[str, List[str], Dict[str, Any], ModuleType],
-    target_module_file: Optional[str],
+    target_module_file: str,
     module_description: Optional[str] = None,
     class_description: Optional[str] = None,
     comments: Optional[Union[Dict[str, str], List[str]]] = None,
 ):
     """Generate Schema Types Enum from datahub module."""
     if isinstance(sources, list):
         enum = {re.sub(r"([a-z])([A-Z])", "\\1_\\2", key).replace(".", "_").upper(): f"{key!r}" for key in sources}
@@ -42,28 +42,28 @@
             for idx, comment in enumerate(comments):
                 key = list(enum.keys())[idx]
                 enum[key] = f"{enum[key]}  # {comment}"
         elif isinstance(comments, dict):
             for key, comment in comments.items():
                 enum[key] = f"{enum[key]}  # {comment}"
 
-    enum = [f"{key} = {value}" for key, value in enum.items()]
-    enum = """
+    enum_list = [f"{key} = {value}" for key, value in enum.items()]
+    enum_str = """
     """.join(
-        enum
+        enum_list
     )
 
     module_description = f'''"""{module_description}"""''' if module_description else ""  # noqa: B907
     class_description = f'''"""{class_description}"""''' if class_description else ""  # noqa: B907
 
     module = f'''{f"""{module_description}
 """ if module_description else ""}from enum import Enum
-{f"""import {sources.__name__}
-""" if not isinstance(sources, (list, dict)) else ""}
+{"" if isinstance(sources, (list, dict)) else f"""import {sources.__name__}
+ """}
 
 class {title}(Enum):
     {f"""{class_description}
-    """ if class_description else ""}{enum}
+    """ if class_description else ""}{enum_str}
 '''
 
     with open(target_module_file, "w") as f:
         f.write(module)
```

### Comparing `cornflakes-3.3.7/cornflakes/cli/__init__.py` & `cornflakes-3.3.8/cornflakes/cli/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Command-line interface."""
 from cornflakes.decorator import click_cli
 from cornflakes.decorator.click import bg_process_option, verbose_option
 
 
 @click_cli(
+    config=None,
     OPTION_GROUPS={
         **{
             command: [
                 {
                     "name": "Basic Options",
                     "options": [
                         "--name",
@@ -21,22 +22,15 @@
                         "--background-process",
                     ],
                 },
             ]
             for command in ["cornflakes", "cornflakes create"]
         },
     },
-    COMMAND_GROUPS={
-        "cornflakes": [
-            {
-                "name": "Test Commands",
-                "commands": ["print"],
-            },
-        ]
-    },
+    COMMAND_GROUPS={},
     CONTEXT_SETTINGS={"help_option_names": ["-h", "--help"]},
     HEADER_LOGO="""[blue]
  ██████╗ ██████╗ ██████╗ ███╗   ██╗███████╗██╗      █████╗ ██╗  ██╗███████╗ ███████╗
 ██╔════╝██╔═══██╗██╔══██╗████╗  ██║██╔════╝██║     ██╔══██╗██║ ██╔╝██╔════╝ ██╔════╝
 ██║     ██║   ██║██████╔╝██╔██╗ ██║█████╗  ██║     ███████║█████╔╝ █████╗   ███████╗
 ██║     ██║   ██║██╔══██╗██║╚██╗██║██╔══╝  ██║     ██╔══██║██╔═██╗ ██╔══╝   ╚════██║
 ╚██████╗╚██████╔╝██║  ██║██║ ╚████║██║     ███████╗██║  ██║██║  ██╗███████╗ ███████║
```

### Comparing `cornflakes-3.3.7/cornflakes/common/__init__.py` & `cornflakes-3.3.8/cornflakes/common/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,23 @@
 """cornflakes common module.
 __________________________________
 """  # noqa: RST303 D205
+from cornflakes.common._check_type import check_type, get_actual_type
 from cornflakes.common._default_ca_path import default_ca_path
 from cornflakes.common._extract_var_names import extract_var_names
 from cornflakes.common._patch_module import patch_module
+from cornflakes.common._recursive_update import recursive_update
 from cornflakes.common._type_to_str import type_to_str
-from cornflakes.common._types import datetime_ms, unquoted_string
+from cornflakes.common._datetime_ms import datetime_ms
+from cornflakes.common._unquoted_string import unquoted_string
 
 __all__ = [
     "default_ca_path",
     "type_to_str",
-    "datetime_ms",
     "extract_var_names",
-    "unquoted_string",
     "patch_module",
+    "check_type",
+    "get_actual_type",
+    "recursive_update",
+    "datetime_ms",
+    "unquoted_string",
 ]
```

### Comparing `cornflakes-3.3.7/cornflakes/common/_default_ca_path.py` & `cornflakes-3.3.8/cornflakes/common/_default_ca_path.py`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/cornflakes/common/_patch_module.py` & `cornflakes-3.3.8/cornflakes/common/_patch_module.py`

 * *Files 20% similar despite different names*

```diff
@@ -17,26 +17,34 @@
     for cls in bound_to.__mro__:
         descriptor = vars(cls).get(name)
         if descriptor is not None:
             return isinstance(descriptor, classmethod)
     return False
 
 
-def _patch_module(m):
+patch_modules: list = []
+
+
+def _patch_module(
+    m,
+):
     """Method to overwrite module variables in a generic way.
 
     1. Overwrite names from submodules declared in __all__ to parent module.
     2. Overwrite doc_string and adds auto summary with objects defined in __all__.
     """
     for obj in [getattr(m, x, None) for x in getattr(m, "__all__", [key for key, _ in getmembers(m)])]:
         if not obj:
             continue
         if ismodule(obj):
             _patch_module(obj)
             for sub_m in iter_modules(getattr(obj, "__path__", [])):
+                if f"{obj.__name__}.{sub_m.name}" in patch_modules:
+                    continue
+                patch_modules.append(f"{obj.__name__}.{sub_m.name}")
                 _patch_module(import_module(f"{obj.__name__}.{sub_m.name}"))
             return
         if not isclassmethod(obj):
             try:
                 obj.__module__ = getattr(m, "__name__", "")
             except Exception as e:
                 logging.debug(e)
@@ -60,9 +68,12 @@
     2. Overwrite doc_string and adds auto summary with objects defined in __all__.
     """
     if os.environ.get("CORNFLAKES_GENERATING_CONFIG_MODULE", "") == "True" or module in __pached_modules:
         return
     __pached_modules.append(module)
     m = import_module(module)
     for sub_m in iter_modules(getattr(m, "__path__", [])):
+        if f"{m.__name__}.{sub_m.name}" in patch_modules:
+            continue
+        patch_modules.append(f"{m.__name__}.{sub_m.name}")
         _patch_module(import_module(f"{m.__name__}.{sub_m.name}"))
     _patch_module(m)
```

### Comparing `cornflakes-3.3.7/cornflakes/common/_type_to_str.py` & `cornflakes-3.3.8/cornflakes/common/_type_to_str.py`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/cornflakes/common/_types.py` & `cornflakes-3.3.8/cornflakes/common/_datetime_ms.py`

 * *Files 16% similar despite different names*

```diff
@@ -45,20 +45,18 @@
             self.millisecond,
         ]
         if datetime_list[-1] == 0:
             del datetime_list[-1]
         if datetime_list[-1] == 0:
             del datetime_list[-1]
         datetime_str = f"datetime_ms({', '.join(map(str, datetime_list))})"
-        if self.tzinfo is not None:
-            if datetime_str[-1:] == ")":
-                datetime_str = datetime_str[:-1] + ", tzinfo=%r" % self.tzinfo + ")"
-        if self.fold:
-            if datetime_str[-1:] == ")":
-                datetime_str = datetime_str[:-1] + ", fold=1)"
+        if self.tzinfo is not None and datetime_str[-1:] == ")":
+            datetime_str = datetime_str[:-1] + ", tzinfo=%r" % self.tzinfo + ")"
+        if self.fold and datetime_str[-1:] == ")":
+            datetime_str = f"{datetime_str[:-1]}, fold=1)"
         return datetime_str
 
     @property
     def millisecond(self) -> int:
         """Milliseconds of datetime.
 
         :return: milliseconds
@@ -79,20 +77,7 @@
     minute: Optional[int] = 0,
     second: Optional[int] = 0,
     millisecond: Optional[int] = 0,
     tzinfo: Optional[datetime.tzinfo] = None,
 ) -> DatetimeMS:
     """Create Instance of :meth:`cornflakes.common.DatetimeMS`."""
     return cast(DatetimeMS, DatetimeMS(year, month, day, hour, minute, second, millisecond, tzinfo))  # camelcase
-
-
-class UnquotedString(str):
-    """String Wrapper with overwritten repr Function to not quote."""
-
-    def __repr__(self):
-        """String Wrapper with overwritten repr Function to not quote."""
-        return self
-
-
-def unquoted_string(x: str):
-    """Create Instance of :meth:`cornflakes.common.UnquotedString`."""
-    return UnquotedString(x)
```

### Comparing `cornflakes-3.3.7/cornflakes/decorator/_add_dataclass_slots.py` & `cornflakes-3.3.8/cornflakes/decorator/dataclasses/_add_dataclass_slots.py`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/cornflakes/decorator/_funcat.py` & `cornflakes-3.3.8/cornflakes/decorator/_funcat.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,23 @@
-from typing import Literal
+from cornflakes.decorator._wrap_kwargs import wrap_kwargs
+from cornflakes.types import FuncatTypes
 
 
-def funcat(func, *f_args, funcat_where: Literal["after", "before", "wrap"] = "after", **f_kwargs):
+def funcat(func, *f_args, where: FuncatTypes = FuncatTypes.AFTER, **f_kwargs):
     """Prepend a functionality."""
 
     def decorator(original_func):
+        @wrap_kwargs(original_func)
         def new_func(*args, **kwargs):
-            if funcat_where == "wrap":
+            if where == FuncatTypes.WRAP:
                 func(*f_args, **f_kwargs)
                 result = original_func(*args, **kwargs)
                 func(*f_args, **f_kwargs)
                 return result
-            elif funcat_where == "before":
+            elif where == FuncatTypes.BEFORE:
                 func(*f_args, **f_kwargs)
                 return original_func(*args, **kwargs)
             else:
                 result = original_func(*args, **kwargs)
                 func(*f_args, **f_kwargs)
                 return result
```

### Comparing `cornflakes-3.3.7/cornflakes/decorator/_indexer.py` & `cornflakes-3.3.8/cornflakes/decorator/_indexer.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,55 +1,70 @@
 from dataclasses import dataclass, field
-from typing import Dict, Optional, Type, TypeVar
+from typing import Callable, Dict, Optional, Protocol, Type, TypeVar, runtime_checkable
 
 T = TypeVar("T")
 
 
 def is_index(obj):
     """Returns True if the given object is an index type."""
     return getattr(getattr(obj, "__class__", {}), "__name__", "")[-6:] == "_Index"
 
 
+@runtime_checkable
+class IndexInstance(Protocol):
+    """Protocol for Index instances."""
+
+    reset: Callable[[], None]
+
+
 @dataclass
 class IndexCounter:
     """Indexer Class."""
 
     name: str = ""
     start: int = 0
     index: int = field(default=0, init=False)
     type: Optional[Type] = field(default=None, init=False)
 
     def __post_init__(self):
         """Initialize the dataclass object."""
-        self.type = type(f"{self.name}_Index", (int,), {})
+        self.type = type(
+            f"{IndexInstance.__name__}.{self.name}_Index",
+            (
+                IndexInstance,
+                int,
+            ),
+            {},
+        )
 
         self.start = self.start - 1
         self.index = self.start
 
         def new(cls, value=None):
             if isinstance(value, int) and self.index == self.start:
                 self.start = value - 1
                 self.index = self.start
             self.index += 1
-            return int.__new__(cls, int(self.index))
+            return int.__new__(cls, self.index)
 
         self.type.__new__ = new
-        self.type.reset = lambda: self.reset()
+        self.type.reset = lambda x=self: self.reset()
         self.is_index = True
 
     def reset(self):
         """Resets the index."""
-        if not self.index == self.start:
+        if self.index != self.start:
             self.index = self.start
 
 
 class Index(int):
     """Indexer Class."""
 
     indices: Dict[str, IndexCounter] = {}
+    is_group_indexing: bool = False
 
     def __new__(cls, start=None, *args, **kwds):
         """Constructor.
 
         This only exists to give a better error message in case
         someone tries to subclass a special typing object (not a good idea).
         """
@@ -74,11 +89,20 @@
 
     @classmethod
     def __class_getitem__(cls, key):
         """Return an Index instance with the given name."""
         return cls.get_index(key)
 
     @classmethod
+    def group_indexing(cls):
+        """Set group indexing."""
+        Index.reset()
+        # print(f"Switch group indexing from {cls.is_group_indexing} to {not cls.is_group_indexing}")
+        cls.is_group_indexing = not cls.is_group_indexing
+        Index.reset()
+
+    @classmethod
     def reset(cls):
         """Reset all indices to their initial values."""
-        for index in cls.indices.values():
-            index.reset()
+        if not cls.is_group_indexing:
+            for index in cls.indices.values():
+                index.reset()
```

### Comparing `cornflakes-3.3.7/cornflakes/decorator/_wrap_kwargs.py` & `cornflakes-3.3.8/cornflakes/decorator/_wrap_kwargs.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,21 @@
-import dataclasses
 from dataclasses import dataclass, field
 from functools import wraps
-import inspect
 from inspect import Parameter, Signature, signature
 from typing import Any, Callable, Dict, List, Optional
 
-_HAS_DEFAULT_FACTORY = getattr(dataclasses, "_HAS_DEFAULT_FACTORY", None)
-Empty = getattr(inspect, "_empty", None)
+from cornflakes.types import HAS_DEFAULT_FACTORY, INSPECT_EMPTY, WITHOUT_DEFAULT
 
 
 def _not_excluded(default):
-    return default != _HAS_DEFAULT_FACTORY
+    return default != HAS_DEFAULT_FACTORY
 
 
 def _not_empty(x):
-    return x != Empty
+    return x not in [INSPECT_EMPTY, WITHOUT_DEFAULT]
 
 
 def _check_default(default):
     return _not_empty(default) and _not_excluded(default)
 
 
 def _check_annotation(annotation):
@@ -30,15 +27,16 @@
     """KwargsWrapper Class."""
 
     wrapped_sig: Optional[Signature] = field(default=None, init=False)
     key_names_no_default: List[str] = field(default_factory=list, init=False)
     key_names: List[str] = field(default_factory=list, init=False)
     arg_names: List[str] = field(default_factory=list, init=False)
     kwarg_names: List[str] = field(default_factory=list, init=False)
-    wrapped: Optional[Callable[..., Any]] = field(default=None)
+    wrapped: Callable[..., object]
+    overwrites: Dict[str, Any] = field(default_factory=dict)
     key_params: List[Parameter] = field(default_factory=list)
     key_params_no_default: List[Parameter] = field(default_factory=list)
     arg_params: List[Parameter] = field(default_factory=list)
     kwarg_params: List[Parameter] = field(default_factory=list)
 
     @property
     def _names(self):
@@ -87,14 +85,25 @@
             for idx, param in enumerate(self._params)
             if _check_annotation(param.annotation)
         }
 
     def _update_params(self, parameters):
         for name, param in parameters.items():
             if name not in self._names:
+                if _check_default(self.overwrites.get(param.name, INSPECT_EMPTY)):
+                    self.key_names.append(name)
+                    self.key_params.append(
+                        Parameter(
+                            param.name,
+                            kind=param.kind,
+                            default=self.overwrites.get(name),
+                            annotation=param.annotation,
+                        )
+                    )
+                    continue
                 if _check_default(param.default):
                     self.key_names.append(name)
                     self.key_params.append(param)
                     continue
                 if param.kind == Parameter.VAR_POSITIONAL:
                     self.arg_names.append(name)
                     self.arg_params.append(param)
@@ -119,15 +128,21 @@
                     if _check_annotation(param.annotation)
                     else self._params[param_idx].annotation,
                 )
                 continue
             self._params[param_idx] = Parameter(
                 param.name,
                 kind=param.kind,
-                default=param.default if _check_default(param.default) else self._params[param_idx].default,
+                default=(
+                    param.default
+                    if _check_default(param.default)
+                    else
+                    # self.overwrites.get(param.name) if _check_default(self.overwrites.get(param.name, INSPECT_EMPTY)) else
+                    self._params[param_idx].default
+                ),
                 annotation=param.annotation
                 if _check_annotation(param.annotation)
                 else self._params[param_idx].annotation,
             )
 
     def __post_init__(self):
         """Initialize the Class."""
@@ -147,15 +162,15 @@
             wrapper_str,
             locals(),
             ldict,
         )
         return wraps(self.wrapped)(ldict["wrap_kwargs"])
 
 
-def wrap_kwargs(wrapped) -> Callable[..., Any]:
+def wrap_kwargs(wrapped, **overwrites) -> Callable[..., Any]:
     """Function Decorator that can update all passed arguments (that can be a variable) of function."""
-    kwargs_wrapper = KwargsWrapper(wrapped)
+    kwargs_wrapper = KwargsWrapper(wrapped=wrapped, overwrites=overwrites)
 
     def wrapper(func):
         return kwargs_wrapper.wrap(func)
 
     return wrapper
```

### Comparing `cornflakes-3.3.7/cornflakes/decorator/click/__init__.py` & `cornflakes-3.3.8/cornflakes/decorator/click/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """Click Extension for better CLI.
 __________________________________
 See referenced Code at https://github.com/ewels/rich-click.git
 """  # noqa: RST303 D205
 from cornflakes.decorator.click._click_cli import click_cli
-from cornflakes.decorator.click.options import auto_option, bg_process_option, global_option, verbose_option
+from cornflakes.decorator.click.options import config_option, bg_process_option, global_option, verbose_option
 from cornflakes.decorator.click.rich import RichArg, RichCommand, RichConfig, RichGroup, argument, command, group
 
 __all__ = [
     "global_option",
     "verbose_option",
     "bg_process_option",
-    "auto_option",
+    "config_option",
     "group",
     "command",
     "argument",
     "RichArg",
     "RichGroup",
     "RichCommand",
     "RichConfig",
```

### Comparing `cornflakes-3.3.7/cornflakes/decorator/click/_click_cli.py` & `cornflakes-3.3.8/cornflakes/decorator/click/_click_cli.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from importlib.metadata import version
 from inspect import getfile
 import logging
-from typing import Any, Callable, Optional, Union, cast
+from typing import TYPE_CHECKING, Any, Callable, Optional, TypeVar, Union, cast
 
 import click
-from click import BaseCommand, Command, Group, style, version_option
+from click import style, version_option
 
 from cornflakes.decorator.click.rich import (
     RichArg,
     RichCommand,
     RichConfig,
     RichGroup,
     argument,
     command,
     group,
     group_command,
     group_group,
 )
-from cornflakes.decorator.types import Config, Loader
 from cornflakes.logging.logger import setup_logging
+from cornflakes.types import Loader
 
 RICH_CLICK_PATCHED = False
 
 
 def patch_click():
     """Patch click to use rich extensions."""
     global RICH_CLICK_PATCHED
@@ -34,75 +34,78 @@
         click.Command = RichCommand
         click.Argument = RichArg
         click.Group.command = group_command
         click.Group.group = group_group
         RICH_CLICK_PATCHED = True
 
 
+_T = TypeVar("_T")
+
+AnyCallable = Callable[..., Any]
+
+
 def click_cli(  # noqa: C901
-    callback: Optional[Callable] = None,
-    config: Optional[Union[RichConfig, Config, Any]] = None,
+    callback: Optional[Any] = None,
+    config: Optional[RichConfig] = None,
     files: Optional[str] = None,
-    loader: Loader = Loader.DICT_LOADER,
+    loader: Loader = Loader.DICT,
     default_log_level: int = logging.INFO,
     as_command: bool = False,
     *args,
     **kwargs,
-) -> Union[
-    Callable[[Any], Callable[..., Union[BaseCommand, RichGroup]]],
-    Callable[..., Union[BaseCommand, Group, RichGroup, Command, RichCommand]],
-]:
+):
     """Function that creates generic click CLI Object."""
     patch_click()
     setup_logging(default_level=default_log_level)
     if not config:
         if not files:
             config = RichConfig(*args, **kwargs)
-        elif loader in [Loader.INI_LOADER, Loader.YAML_LOADER]:
+        elif loader in [Loader.INI, Loader.YAML]:
             config = getattr(RichConfig, str(loader.name))(*args, **kwargs).popitem()[1]
         elif ".ini" in files:
             config = RichConfig.from_ini(files, *args, **kwargs).popitem()[1]
         elif ".yaml" in files:
             config = RichConfig.from_yaml(files, *args, **kwargs).popitem()[1]
         else:
             config = RichConfig(*args, **kwargs)
 
-    config = cast(RichConfig, config)
-
-    def cli_wrapper(w_callback: Callable) -> Callable[..., Union[BaseCommand, Group, RichGroup, Command, RichCommand]]:
+    def cli_wrapper(w_callback: Any):
         if not callable(w_callback):
             return w_callback
 
         module = getfile(w_callback)
 
         if hasattr(w_callback, "__module__"):
             module = w_callback.__module__.split(".", 1)[0]
             if module != "__main__":
                 __version = version(module)
 
-        if as_command:
-            cli: Union[BaseCommand, Command, RichCommand] = command(module, config=config)(w_callback)
-        else:
-            cli: Union[BaseCommand, Group, RichGroup] = group(module, config=config)(w_callback)
-        if config.VERSION_INFO:
+        module = module.replace("_", "-")
+
+        cli: Union[RichCommand, RichGroup] = (
+            command(module, config=config)(w_callback) if as_command else group(module, config=config)(w_callback)
+        )
+
+        if TYPE_CHECKING:
+            cli = cast(RichCommand, cli) if as_command else cast(RichGroup, cli)
+
+        if cast(RichConfig, config).VERSION_INFO:
             name = w_callback.__qualname__
             __version = "0.0.1"
 
             version_args = {
                 "prog_name": name,
                 "version": __version,
                 "message": style(
                     f"\033[95m{module}\033" f"[0m \033[95m" f"Version\033[0m: \033[1m" f"{__version}\033[0m"
                 ),
             }
-            cli: Any = version_option(**version_args)(cli)
+            cli = version_option(**version_args)(cli)  # type: ignore
 
         if cli.config.GLOBAL_OPTIONS:
             for option_obj in cli.config.GLOBAL_OPTIONS:
                 cli.params.extend(option_obj.params)
-        if config.CONTEXT_SETTINGS:
-            cli.context_settings = config.CONTEXT_SETTINGS
+        if cast(RichConfig, config).CONTEXT_SETTINGS:
+            cli.context_settings = cast(RichConfig, config).CONTEXT_SETTINGS
         return cli
 
-    if callback:
-        return cli_wrapper(callback)
-    return cli_wrapper
+    return cli_wrapper(callback) if callback else cli_wrapper
```

### Comparing `cornflakes-3.3.7/cornflakes/decorator/click/options/_bg_process.py` & `cornflakes-3.3.8/cornflakes/decorator/click/options/_bg_process.py`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/cornflakes/decorator/click/options/_global.py` & `cornflakes-3.3.8/cornflakes/decorator/click/options/_global.py`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/cornflakes/decorator/click/options/_verbose.py` & `cornflakes-3.3.8/cornflakes/decorator/click/options/_verbose.py`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/cornflakes/decorator/click/rich/__init__.py` & `cornflakes-3.3.8/cornflakes/decorator/click/rich/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,73 +1,70 @@
 """cornflakes.click.rich Module."""
-from typing import Callable, Any, Optional, Union
+from typing import Callable, Optional, Union, Any
 
 from click import argument as click_argument
 from click import command as click_command
-from click import group as click_group, Command, Group
+from click import group as click_group, Command, Group, BaseCommand, Argument
 
 from cornflakes.decorator.click.rich._rich_argument import RichArg
 from cornflakes.decorator.click.rich._rich_command import RichCommand
 from cornflakes.decorator.click.rich._rich_config import RichConfig
 from cornflakes.decorator.click.rich._rich_global_option_wrapper import rich_global_option_wrapper
 from cornflakes.decorator.click.rich._rich_group import RichGroup
 
-F = Callable[..., Union[RichCommand, RichGroup, RichArg, Any]]
 
+AnyCallable = Callable[..., Any]
 
-def group(*args, cls=RichGroup, **kwargs) -> F:  # type: ignore
+
+def group(*args, cls=RichGroup, **kwargs) -> Callable[[Union[AnyCallable, RichGroup]], RichGroup]:  # type: ignore
     """Group decorator function.
 
     Defines the group() function so that it uses the RichGroup class by default.
     """
     return rich_global_option_wrapper(click_group, *args, cls=cls, **kwargs)
 
 
-def command(*args, cls=RichCommand, **kwargs) -> F:  # type: ignore
+def command(*args, cls=RichCommand, **kwargs) -> Callable[[Union[AnyCallable, Command, Group, RichCommand, RichGroup]], RichCommand]:  # type: ignore
     """Command decorator function.
 
     Defines the command() function so that it uses the RichCommand class by default.
     """
     return rich_global_option_wrapper(click_command, *args, cls=cls, **kwargs)
 
 
-def argument(*args, cls=RichArg, **kwargs) -> F:  # type: ignore
+def argument(*args, cls=RichArg, **kwargs) -> Callable[..., Union[Argument, RichArg]]:  # type: ignore
     """Command decorator function.
 
     Defines the command() function so that it uses the RichCommand class by default.
     """
     return click_argument(*args, cls=cls, **kwargs)
 
 
-def group_command(self, name: Optional[str], cmd: Union[Command, RichCommand, Any] = None):
+def group_command(self, name: Optional[str], cmd: Optional[Union[BaseCommand, Command, RichCommand]] = None):
     """Decorator to register a RichCommand with this group."""
 
     def wrapper(callback):
         """Wrapper function for the decorator."""
         new_command = command(name=name, config=self.config)(callback)
         self.add_command(new_command, name)
         return new_command
 
-    if cmd:
-        return wrapper(cmd)
-    return wrapper
+    return wrapper(cmd) if cmd else wrapper
 
 
-def group_group(self, name: Optional[str], cmd: Union[Group, RichGroup, Any] = None):
+def group_group(self, name: Optional[str], cmd: Optional[Union[Group, RichGroup]] = None):
     """Decorator to register a RichGroup with this group."""
 
     def wrapper(callback):
         """Wrapper function for the decorator."""
         new_group = group(name=name, config=self.config)(callback)
         self.add_command(new_group, name)
         return new_group
 
-    if cmd:
-        return wrapper(cmd)
-    return wrapper
+    return wrapper(cmd) if cmd else wrapper
 
 
 __all__ = [
     "RichConfig",
     "RichGroup",
     "RichCommand",
     "RichArg",
```

### Comparing `cornflakes-3.3.7/cornflakes/decorator/click/rich/_rich_click.py` & `cornflakes-3.3.8/cornflakes/decorator/click/rich/_rich_click.py`

 * *Files 5% similar despite different names*

```diff
@@ -212,24 +212,20 @@
 
     # Environment variable AFTER help text
     if getattr(param, "show_envvar", None) and not config.OPTION_ENVVAR_FIRST and envvar is not None:
         items.append(Text(config.ENVVAR_STRING.format(envvar), style=config.STYLE_OPTION_ENVVAR))
 
     # Default value
     if getattr(param, "show_default", None):
-        # param.default is the value, but click is a bit clever in choosing what to show here
-        # eg. --debug/--no-debug, default=False will show up as [default: no-debug] instead of [default: False]
-        # To avoid duplicating loads of code, let's just pull out the string from click with a regex
-        # Example outputs from param.get_help_record(ctx)[-1] are:
-        #     [default: foo]
-        #     [env var: EMAIL, EMAIL_ADDRESS; default: foo]
-        default_str_match = re.search(r"\[(?:.+; )?default: (.*)\]", typing.cast(list, param.get_help_record(ctx))[-1])
-        if default_str_match:
+        if default_str_match := re.search(
+            r"\[(?:.+; )?default: (.*)\]",
+            typing.cast(list, param.get_help_record(ctx))[-1],
+        ):
             # Don't show the required string, as we show that afterwards anyway
-            default_str = default_str_match.group(1).replace("; required", "")
+            default_str = default_str_match[1].replace("; required", "")
             items.append(
                 Text(
                     config.DEFAULT_STRING.format(default_str),
                     style=config.STYLE_OPTION_DEFAULT,
                 )
             )
 
@@ -271,15 +267,15 @@
 
 
 def rich_format_help(
     obj: Union[click.Command, click.Group],
     ctx: click.Context,
     formatter: click.HelpFormatter,
     config: RichConfig,
-    console: Console = None,
+    console: typing.Optional[Console] = None,
 ) -> None:
     """Print nicely formatted help text using rich.
 
     Based on original code from rich-click, by @willmcgugan.
     https://github.com/Textualize/rich-cli/blob/8a2767c7a340715fc6fbf4930ace717b9b2fc5e5/src/rich_cli/__main__.py#L162-L236
 
     Replacement for the click function format_help().
@@ -438,24 +434,27 @@
             options_rows.append(rows)
 
         if len(options_rows) > 0:
             t_styles = {
                 "show_lines": config.STYLE_OPTIONS_TABLE_SHOW_LINES,
                 "leading": config.STYLE_OPTIONS_TABLE_LEADING,
                 "box": config.STYLE_OPTIONS_TABLE_BOX,
+                "header_style": config.STYLE_OPTIONS_TABLE_HEADER_STYLE,
                 "border_style": config.STYLE_OPTIONS_TABLE_BORDER_STYLE,
                 "row_styles": config.STYLE_OPTIONS_TABLE_ROW_STYLES,
                 "pad_edge": config.STYLE_OPTIONS_TABLE_PAD_EDGE,
+                "show_edge": config.STYLE_OPTIONS_TABLE_SHOW_EDGE,
                 "padding": config.STYLE_OPTIONS_TABLE_PADDING,
             }
             t_styles.update(option_group.get("table_styles", {}))  # type: ignore
             box_style = getattr(box, t_styles.pop("box"), None)  # type: ignore
             options_table = Table(
                 highlight=True,
                 show_header=False,
+                show_footer=False,
                 expand=True,
                 box=box_style,
                 **t_styles,  # type: ignore
             )
             # Strip the required column if none are required
             if all([x[0] == "" for x in options_rows]):
                 options_rows = [x[1:] for x in options_rows]
@@ -544,15 +543,15 @@
     # Footer text if we have it
     if config.FOOTER_TEXT:
         console.print(
             Padding(_make_rich_text(config.FOOTER_TEXT, config=config, style=config.STYLE_FOOTER_TEXT), (1, 1, 0, 1))
         )
 
 
-def rich_format_error(self: click.ClickException, config: RichConfig, console: Console = None):
+def rich_format_error(self: click.ClickException, config: RichConfig, console: typing.Optional[Console] = None):
     """Print richly formatted click errors.
 
     Called by custom exception handler to print richly formatted click errors.
     Mimics original click.ClickException.echo() function but with rich formatting.
 
     Args:
         click.ClickException: Click exception to format.
@@ -583,12 +582,12 @@
             title_align=config.ALIGN_ERRORS_PANEL,  # type: ignore
         )
     )
     if config.ERRORS_EPILOGUE:
         console.print(config.ERRORS_EPILOGUE)
 
 
-def rich_abort_error(config: RichConfig, console: Console = None) -> None:
+def rich_abort_error(config: RichConfig, console: typing.Optional[Console] = None) -> None:
     """Print richly formatted abort error."""
     if not console:
         console = get_rich_console(config=config)
     console.print(config.ABORTED_TEXT, style=config.STYLE_ABORTED)
```

### Comparing `cornflakes-3.3.7/cornflakes/decorator/click/rich/_rich_command.py` & `cornflakes-3.3.8/cornflakes/decorator/click/rich/_rich_command.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import sys
-from typing import Any, List
+from typing import Any, List, Optional
 
 from click import ClickException, Command, Context, HelpFormatter, Parameter, exceptions
 
 from cornflakes.decorator.click.rich._rich_click import rich_abort_error, rich_format_error, rich_format_help
 from cornflakes.decorator.click.rich._rich_config import RichConfig as RichConfig
 
 
@@ -17,19 +17,21 @@
     standalone_mode = False
     params: List[Parameter]
     allow_extra_args = True
     allow_interspersed_args = False
     ignore_unknown_options = False
     name = ""
     context_settings: dict
+    parent = None
+    config: RichConfig
 
     def callback(self):
         """Callback method with is wrapped over the command."""
 
-    def __init__(self, config: RichConfig = None, *args, **kwargs):
+    def __init__(self, config: Optional[RichConfig] = None, *args, **kwargs):
         """Init function of RichGroup with extra config argument."""
         if not config:
             config = RichConfig()
         super().__init__(*args, **kwargs)
         self.config = config
         self.console = None
```

### Comparing `cornflakes-3.3.7/cornflakes/decorator/click/rich/_rich_config.py` & `cornflakes-3.3.8/cornflakes/decorator/click/rich/_rich_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from dataclasses import field
 from os import getenv
-from typing import Dict, List, Literal, Optional, Protocol, Tuple, Union
+from typing import TYPE_CHECKING, Dict, List, Literal, Optional, Protocol, Tuple, Union
 
 from click import Option
 
-from cornflakes.decorator.config import config
+from cornflakes.decorator.dataclasses.config import config
 
 
 class GlobalOption(Protocol):
     """GlobalOption Protocol which requires params."""
 
     params: List[Option]
 
 
-@config
+@config(init=True)
 class RichConfig:
     """DataClass for click config-values."""
 
     # Default styles
     STYLE_OPTION: str = "bold cyan"
     STYLE_ARGUMENT: str = "bold cyan"
     STYLE_SWITCH: str = "bold green"
@@ -38,34 +38,38 @@
     STYLE_REQUIRED_LONG: str = "dim red"
     STYLE_OPTIONS_PANEL_BORDER: str = "dim"
     ALIGN_OPTIONS_PANEL: str = "left"
     STYLE_OPTIONS_TABLE_SHOW_LINES: bool = False
     STYLE_OPTIONS_TABLE_LEADING: int = 0
     STYLE_OPTIONS_TABLE_PAD_EDGE: bool = False
     STYLE_OPTIONS_TABLE_PADDING: Tuple[int, int] = (0, 1)
+    STYLE_OPTIONS_TABLE_SHOW_EDGE: bool = True
     STYLE_OPTIONS_TABLE_BOX: str = ""
-    STYLE_OPTIONS_TABLE_ROW_STYLES: List[str] = None
-    STYLE_OPTIONS_TABLE_BORDER_STYLE: str = None
+    STYLE_OPTIONS_TABLE_ROW_STYLES: Optional[List[str]] = None
+    STYLE_OPTIONS_TABLE_HEADER_STYLE: str = "table.header"
+    STYLE_OPTIONS_TABLE_BORDER_STYLE: Optional[str] = None
     STYLE_COMMANDS_PANEL_BORDER: str = "dim"
     ALIGN_COMMANDS_PANEL: str = "left"
     STYLE_COMMANDS_TABLE_SHOW_LINES: bool = False
     STYLE_COMMANDS_TABLE_LEADING: int = 0
     STYLE_COMMANDS_TABLE_PAD_EDGE: bool = False
     STYLE_COMMANDS_TABLE_PADDING: Tuple[int, int] = (0, 1)
     STYLE_COMMANDS_TABLE_BOX: str = ""
-    STYLE_COMMANDS_TABLE_ROW_STYLES: List[str] = None
-    STYLE_COMMANDS_TABLE_BORDER_STYLE: List[str] = None
+    STYLE_COMMANDS_TABLE_ROW_STYLES: Optional[List[str]] = None
+    STYLE_COMMANDS_TABLE_BORDER_STYLE: Optional[List[str]] = None
     STYLE_ERRORS_PANEL_BORDER: str = "red"
     ALIGN_ERRORS_PANEL: str = "left"
     STYLE_ERRORS_SUGGESTION: str = "dim"
     STYLE_ABORTED: str = "red"
-    MAX_WIDTH = int(getenv("TERMINAL_WIDTH")) if getenv("TERMINAL_WIDTH") else None  # type: ignore
+    MAX_WIDTH: Optional[int] = int(getenv("TERMINAL_WIDTH")) if getenv("TERMINAL_WIDTH") else None  # type: ignore
     COLOR_SYSTEM: Optional[Literal["auto", "standard", "256", "truecolor", "windows"]] = "auto"
     # Set to None to disable colors
-    FORCE_TERMINAL = True if getenv("GITHUB_ACTIONS") or getenv("FORCE_COLOR") or getenv("PY_COLORS") else None
+    FORCE_TERMINAL: Optional[bool] = (
+        True if getenv("GITHUB_ACTIONS") or getenv("FORCE_COLOR") or getenv("PY_COLORS") else None
+    )
 
     # Fixed strings
     HEADER_TEXT: Optional[str] = None
     HEADER_LOGO: Optional[str] = None
     FOOTER_TEXT: Optional[str] = None
     DEPRECATED_STRING: str = "(Deprecated) "
     DEFAULT_STRING: str = "[default: {}]"
@@ -85,15 +89,15 @@
     # Behaviours
     SHOW_ARGUMENTS: bool = True  # Show positional arguments
     SHOW_METAVARS_COLUMN: bool = True  # Show a column with the option metavar (eg. INTEGER)
     APPEND_METAVARS_HELP: bool = False  # Append metavar (eg. [TEXT]) after the help text
     APPEND_METAVARS_REQUIRED: bool = False  # Append metavar REQUIRED_LONG_STRING (eg. [required]) after the help text
     GROUP_ARGUMENTS_OPTIONS: bool = False  # Show arguments with options instead of in own panel
     OPTION_ENVVAR_FIRST: bool = False  # Show env vars before option help text instead of avert
-    USE_RST: bool = True  # Parse help strings as reStructuredText
+    USE_RST: bool = False  # Parse help strings as reStructuredText
     SHOW_RST_ERRORS: bool = False  # Show errors when parsing reStructuredText
     USE_MARKDOWN: bool = False  # Parse help strings as markdown
     USE_MARKDOWN_EMOJI: bool = True  # Parse emoji codes in markdown :smile:
     USE_RICH_MARKUP: bool = False  # Parse help strings for rich markup (eg. [red]my text[/])
     CODE_THEME: str = "monokai"  # Theme for code blocks in reStructuredText and Markdown
     # Define sorted groups of panels to display subcommands
     USE_CLICK_SHORT_HELP: bool = False  # Use click's default function to truncate help text
@@ -103,7 +107,17 @@
     CONTEXT_SETTINGS: Dict[str, List[Dict[str, Union[str, List[str]]]]] = field(default_factory=dict)
 
     COMMAND_GROUPS: Dict[str, List[Dict[str, Union[str, List[str]]]]] = field(default_factory=dict)
     # Define sorted groups of panels to display options and arguments
     OPTION_GROUPS: Dict[str, List[Dict[str, Union[str, List[str]]]]] = field(default_factory=dict)
     # Add basic global options (verbose)
     GLOBAL_OPTIONS: List[GlobalOption] = field(default_factory=list)
+
+    if TYPE_CHECKING:
+
+        @staticmethod
+        def from_ini(*args, **kwargs):
+            ...
+
+        @staticmethod
+        def from_yaml(*args, **kwargs):
+            ...
```

### Comparing `cornflakes-3.3.7/cornflakes/decorator/click/rich/_rich_group.py` & `cornflakes-3.3.8/cornflakes/decorator/click/rich/_rich_group.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import sys
 from typing import Any, Dict, List, Optional, Union
 
 from click import ClickException, Command, Context, Group, HelpFormatter, Parameter, exceptions
 
+from cornflakes.common import recursive_update
+from cornflakes.decorator.click.helper import get_command_name
 from cornflakes.decorator.click.rich._rich_click import (
     get_rich_console,
     rich_abort_error,
     rich_format_error,
     rich_format_help,
 )
 from cornflakes.decorator.click.rich._rich_command import RichCommand
@@ -22,43 +24,53 @@
 
     command_class = RichCommand
     group_class = type
     params: List[Parameter]
     name = ""
     context_settings: dict
     commands: Dict[str, Union[Command, RichCommand]]
+    config: RichConfig
 
     def callback(self):
         """Callback method with is wrapped over the command group."""
 
     def add_command(self, cmd: Union[Command, RichCommand, Group, Any], name: Optional[str] = None) -> None:
         """Registers another :class:`Command` with this group.
 
         If the name is not provided, the name of the command is used.
         """
+        setattr(cmd, "parent", self)
         Group.add_command(self, cmd, name)
 
-    def __init__(self, config: RichConfig = None, *args, **kwargs):
+    def __init__(self, config: Optional[RichConfig] = None, *args, **kwargs):
         """Init function of RichGroup with extra config argument."""
         if not config:
             config = RichConfig()
         super().__init__(*args, **kwargs)
         self.config = config
         self.console = get_rich_console(config=self.config)
 
     def __pass_config(self, config=None, console=None):
-        if config:
-            for _group in self.commands.values():
-                if isinstance(_group, RichGroup) and _group:
-                    _group.__pass_config(config, console)
-                _group.config = config
-                _group.console = console if console else get_rich_console(_group.config)
-                if _group.config.GLOBAL_OPTIONS:
-                    for option_obj in _group.config.GLOBAL_OPTIONS:
-                        _group.params.extend(option_obj.params)
+        if not config:
+            return
+        for _group in self.commands.values():
+            _group.parent = self
+            if isinstance(_group, RichGroup) and _group:
+                _group.__pass_config(config, console)
+            _group.config = config
+            _group.console = console or get_rich_console(_group.config)
+            if _group.config.GLOBAL_OPTIONS:
+                for option_obj in _group.config.GLOBAL_OPTIONS:
+                    _group.params.extend(option_obj.params)
+
+            # fill the auto-options if exists
+            command = get_command_name(_group)
+            if hasattr(_group, "__option_groups__") and len(getattr(_group, "__option_groups__", {})):
+                update_dict = {command: _group.__option_groups__}
+                recursive_update(_group.config.OPTION_GROUPS, update_dict, merge_lists=True)
 
     def main(self, *args, standalone_mode: bool = True, **kwargs) -> Any:  # noqa: C901
         """Main function of RichGroup."""
         try:
             self.__pass_config(self.config, self.console)
             rv = super().main(*args, standalone_mode=False, **kwargs)  # type: ignore
             if not standalone_mode:
```

### Comparing `cornflakes-3.3.7/cornflakes/decorator/config/_load_config.py` & `cornflakes-3.3.8/cornflakes/decorator/dataclasses/config/_load_config.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,196 +1,195 @@
 from collections import OrderedDict
-from dataclasses import MISSING
 from functools import partial
 import logging
 import re
-from typing import Any, Callable, Dict, List, Optional, Union
+from typing import Any, Dict, List, Optional, Union
 
 from cornflakes import ini_load
-from cornflakes.decorator.dataclass.helper import (
+from cornflakes.decorator.dataclasses._helper import (
     dataclass_fields,
+    dc_slot_missing_default,
     is_config_list,
-    is_multi_config,
+    is_use_regex,
     normalized_class_name,
     pass_section_name,
 )
-from cornflakes.decorator.types import WITHOUT_DEFAULT, Config, LoaderMethod
-
-
-def _none_omit(obj: list):
-    return [v for v in obj if v is not None]
-
-
-def _default_filter_method(x: Any):
-    return True
 
 
 def create_file_loader(  # noqa: C901
-    cls: Union[Config, Any],
-    loader: LoaderMethod = ini_load,  # type: ignore
+    cls,
+    _loader_callback=ini_load,  # type: ignore
+    _instantiate: bool = True,
 ):
     """Config decorator to parse Ini Files and implements from_file method to config-classes.
 
+    :param _instantiate: If True, the config class will be initialized with the parsed config dict.
     :param cls: Config class
-    :param loader: Config Loader (ini_load, yaml_load)
+    :param _loader_callback: Config Loader (ini_load, yaml_load)
 
     :returns: wrapped class or the wrapper itself with the custom default arguments if the config class is not
     """
-    required_keys = [
-        key
-        for key, f in dataclass_fields(cls).items()
-        if (f.default_factory == WITHOUT_DEFAULT) or (f.default_factory == MISSING and f.default == MISSING)
-    ]  # type: ignore
-
-    keys = {key: getattr(f, "alias", key) or key for key, f in dataclass_fields(cls).items()}
-
-    def create_config(config: dict, allow_empty=None, filter_function=None, **cls_kwargs):
-        if not filter_function:
-            filter_function = _default_filter_method
-        if not config and allow_empty:
-            return
-        config.update(cls_kwargs)
-        error_args = [key for key in config if key not in dataclass_fields(cls)]
+    required_keys = [key for key, f in dataclass_fields(cls).items() if dc_slot_missing_default(f)]  # type: ignore
+
+    keys = {key: getattr(f, "aliases", key) or key for key, f in dataclass_fields(cls).items()}
+
+    def _create_config(config_args: dict, allow_empty=None, **cls_kwargs) -> Optional[Union[dict, Any]]:
+        if not config_args and allow_empty:
+            return None
+        config_args.update(cls_kwargs)
+        error_args = [key for key in config_args if key not in [*dataclass_fields(cls)]]
         if error_args:
             logging.debug(f"Some variables in **{cls.__name__}** have no annotation or are not defined!")
             logging.debug(f"Please check Args: {error_args}")
 
         #  config_instance
-        config_instance = cls(**{key: value for key, value in config.items() if key in dataclass_fields(cls)})
-        if filter_function(config_instance):
-            return config_instance
+        if _instantiate:
+            return cls(
+                **{key: value for key, value in config_args.items() if key in dataclass_fields(cls)},
+                _load_default=False,
+            )
+        return {key: value for key, value in config_args.items() if key in dataclass_fields(cls)}
 
-    def _check_required_fields(config_dict):
+    def _check_required_fields(config_args) -> dict:
         return {
             section: config
-            for section, config in config_dict.items()
-            if not any([True for key in required_keys if key not in config.keys()])
+            for section, config in config_args.items()
+            if not any(True for key in required_keys if key not in config.keys())
         }
 
-    def _check_any_key_in_fields(config_dict):
+    def _check_any_key_in_fields(config_args) -> dict:
         return {
             section: config
-            for section, config in config_dict.items()
-            if any([key in dataclass_fields(cls).keys() for key in config.keys()])
+            for section, config in config_args.items()
+            if any(key in dataclass_fields(cls).keys() for key in config.keys())
         }
 
-    def _check_config_dict(config_dict):
-        config_dict = _check_required_fields(config_dict)
-        config_dict = _check_any_key_in_fields(config_dict)
-        config_dict = _rename_default_section(config_dict)
-        return config_dict
-
-    def _rename_default_section(config_dict):
-        if None not in config_dict:
-            return config_dict
-        config_dict["default"] = config_dict.pop(None)
-        return config_dict
+    def _check_config_dict(config_args) -> dict:
+        config_args = _check_required_fields(config_args)
+        config_args = _check_any_key_in_fields(config_args)
+        config_args = _rename_default_section(config_args)
+        return config_args or {}
+
+    def _rename_default_section(config_args) -> dict:
+        if None not in config_args:
+            return config_args
+        config_args["default"] = config_args.pop(None)
+        return config_args or {}
 
     def from_file(
-        files: Optional[Union[List[str], str]] = None,
-        sections: Optional[Union[List[str], str]] = None,
+        files: Optional[List[str]] = None,
+        sections: Optional[List[str]] = None,
         config_dict: Optional[Dict[str, Any]] = None,
-        filter_function: Optional[Callable[[Config], bool]] = None,
         eval_env: Optional[bool] = None,
         allow_empty: Optional[bool] = None,
         **slot_kwargs,
-    ) -> Union[Config, Any]:
+    ):
         """Config parser from ini files.
 
         :param files: Default config files
         :param sections: Default config sections
         :param config_dict: Config dictionary to pass already loaded configs
         :param slot_kwargs: Default configs to overwrite passed class
-        :param filter_function: Optional filter method for config
         :param eval_env: Flag to evaluate environment variables into default values.
         :param allow_empty: Flag that allows empty config result -> e.g. emtpy list
 
         :returns: Nested Lists of Config Classes
         """
         if not sections:
             sections = cls.__config_sections__
         if not files:
             files = cls.__config_files__
-        if not filter_function:
-            filter_function = cls.__config_filter_function__ or _default_filter_method
         if not eval_env:
             eval_env = cls.__eval_env__
         if not allow_empty:
             allow_empty = cls.__allow_empty_config__
 
-        _create_config = partial(create_config, allow_empty=allow_empty, filter_function=filter_function)
+        create_config = partial(_create_config, allow_empty=allow_empty)
 
         pass_sections = pass_section_name(cls)
 
         def get_section_kwargs(section):
             return {**slot_kwargs, **({"section_name": section} if pass_sections else {})}
 
-        if not is_multi_config(cls) and isinstance(sections, str):
-            logging.debug(f"Load ini from file: {files} - section: {sections} for config {cls.__name__}")
+        if not is_use_regex(cls) and sections and len(sections) == 1:
+            section = sections[0]
+            logging.debug(f"Load ini from file: {files} - section: {section} for config {cls.__name__}")
 
             if not config_dict:
                 config_dict = OrderedDict(
-                    loader(files={None: files}, sections=sections, keys=keys, defaults=None, eval_env=eval_env)
+                    _loader_callback(files={None: files}, sections=section, keys=keys, defaults=None, eval_env=eval_env)
                 )
                 config_dict = _check_config_dict(config_dict)
-                logging.debug(f"Read config with sections: {config_dict.keys()}")
 
-            if not sections and config_dict.keys():
-                sections = config_dict.popitem()[0] or normalized_class_name(cls)
+            if not section and config_dict.keys():
+                section = config_dict.popitem()[0] or normalized_class_name(cls)
+
+            config = create_config(config_dict.get(section, {}), **get_section_kwargs(section))
 
-            config = _create_config(config_dict.get(sections, {}), **get_section_kwargs(sections))
             if not config:
-                return {sections: _create_config({}, **get_section_kwargs(sections))}
-            return {sections: config}
+                return {section: create_config({}, **get_section_kwargs(section))}
+            return {section: config}
 
         if not config_dict:
             if cls.__chain_files__:
-                config_dict = OrderedDict(loader(files={None: files}, sections=None, keys=keys, eval_env=eval_env))
+                config_dict = OrderedDict(
+                    _loader_callback(files={None: files}, sections=None, keys=keys, eval_env=eval_env)
+                )
             else:
-                raw_config_dict = OrderedDict(loader(files=files, sections=None, keys=keys, eval_env=eval_env))
+                raw_config_dict = OrderedDict(
+                    _loader_callback(files=files, sections=None, keys=keys, eval_env=eval_env)
+                )
                 config_dict = {}
                 for file_name, section_config in raw_config_dict.items():
                     for section_name, config in section_config.items():
                         config_dict[f"{file_name}:{section_name or normalized_class_name(cls)}"] = config
                 config_dict = _check_config_dict(config_dict)
 
             logging.debug(f"Read config with sections: {config_dict.keys()}")
 
         regex = f'({"|".join(sections) if isinstance(sections, list) else sections or ""})'
-        logging.debug(f"Load all configs that mach **{regex}**")
-
+        logging.debug(f"Load all configs that match regex: `{regex}`")
         config_dict = {
             section: config
             for section, config in config_dict.items()
             if bool(re.match(regex, section.split(":", 1).pop() or ""))
         }
+
         if not is_config_list(cls):
             return {
                 section.split(":", 1).pop(): config
                 for section, config in {
-                    section: _create_config(
+                    section: create_config(
                         config_dict.get(section, {}), **get_section_kwargs(section.split(":", 1).pop())
                     )
                     for section in config_dict
                 }.items()
                 if config
             } or {
-                normalized_class_name(cls): _create_config({}, **slot_kwargs)  # no matches
+                normalized_class_name(cls): create_config({}, **slot_kwargs)  # no matches
             }
 
         return {
             normalized_class_name(cls): (
                 list(
                     _none_omit(
                         [
-                            _create_config(
+                            create_config(
                                 config_dict.get(section, {}), **get_section_kwargs(section.split(":", 1).pop())
                             )
                             for section in config_dict
                         ]
                     ),
                 )
-                or _none_omit([_create_config({}, **slot_kwargs)] * is_config_list(cls))
+                or _none_omit([create_config({}, **slot_kwargs)] * is_config_list(cls))
             )
         }
 
     return from_file
+
+
+def _none_omit(obj: list):
+    return [v for v in obj if v is not None]
+
+
+def _default_filter_method(x: Any):
+    return True
```

### Comparing `cornflakes-3.3.7/cornflakes/decorator/config/_load_config_group.py` & `cornflakes-3.3.8/cornflakes/decorator/dataclasses/config/_init_config_group.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,70 +1,97 @@
-# from collections import OrderedDict
 import logging
-from typing import Any, Callable, Optional, Union
+from typing import List, Optional
 
-from cornflakes.decorator.dataclass.helper import is_config, is_config_list
-from cornflakes.decorator.types import ConfigArgument, ConfigGroup
+from cornflakes.decorator._wrap_kwargs import wrap_kwargs
+from cornflakes.decorator.dataclasses._helper import (
+    config_files,
+    config_sections,
+    dataclass_fields,
+    fields,
+    is_allow_empty,
+    is_config,
+    is_config_list,
+    is_eval_env,
+)
+
+
+def _load_config_kwargs(
+    cls,
+    files: Optional[List[str]] = None,
+    sections: Optional[List[str]] = None,
+    eval_env: Optional[bool] = None,
+    allow_empty: Optional[bool] = False,
+    **kwargs,
+):
+    """Create default config arguments for a config-group class."""
+    _files = files if isinstance(files, list) else [str(files)] if files else config_files(cls)
+    default_config: dict = {}
+
+    if not _files:
+        return kwargs
+
+    sections = sections if isinstance(sections, list) else [str(sections)] if sections else config_sections(cls)
+    eval_env = eval_env or is_eval_env(cls)
+    allow_empty = allow_empty or is_allow_empty(cls)
+
+    for slot in fields(cls):
+        slot_class = slot.type
+        if is_config_list(slot_class):
+            slot_class = slot.type.__args__[0]
+
+        if is_config(slot_class):
+            slot_config = slot_class.from_file(
+                files=_files,
+                sections=sections,
+                eval_env=eval_env,
+                allow_empty=allow_empty,
+                **kwargs,
+            )
+            default_config.update(slot_config)
+
+    if error_args := [key for key in default_config if key not in dataclass_fields(cls)]:
+        logging.debug(f"The variables {error_args} in **{cls.__name__}** are not defined!")
+        logging.debug("Use generate_group in build script to auto generate the config group!")
+
+    return default_config
+
+
+def wrap_init_config_group(cls):
+    # Index.reset()
+    # Index.group_indexing()
+    # default_config = _load_config_kwargs(cls)
+    # Index.group_indexing()
+    # Index.reset()
+    # prepare special slot types (e.g. Index)
+    # default_config = evaluate_default_configs(cls, default_config)
+    def pre_init_wrapper(init):
+        @wrap_kwargs(init)
+        def wrapper(
+            self,
+            files: Optional[List[str]] = None,
+            sections: Optional[List[str]] = None,
+            eval_env: Optional[bool] = None,
+            allow_empty: Optional[bool] = False,
+            **kwargs,
+        ):
+            # changed_kwargs = {
+            #     key: value for key, value in kwargs.items() if repr(value) != repr(default_config.get(key))
+            # }
+
+            # if not changed_kwargs:
+            #     return init(self, **kwargs.copy())
+
+            files = files if isinstance(files, list) else [str(files)] if files else config_files(cls)
+
+            if not files:
+                return init(self, **kwargs)
+
+            sections = sections if isinstance(sections, list) else [str(sections)] if sections else config_sections(cls)
+            eval_env = eval_env or is_eval_env(cls)
+            allow_empty = allow_empty or is_allow_empty(cls)
+            return init(self, **_load_config_kwargs(cls, files, sections, eval_env, allow_empty, **kwargs))
 
+        return wrapper
 
-def create_group_loader(cls) -> Callable[..., Union[ConfigGroup, Any]]:
-    """Config decorator to parse Ini Files and implements from_file method to config-group-classes.
+    setattr(cls, "__init__", pre_init_wrapper(cls.__init__))
 
-    :param cls: Config class
-
-    :returns: wrapped class or the wrapper itself with the custom default arguments if the config group class is not
-    """
-
-    def from_file(
-        files: ConfigArgument = None,
-        sections: ConfigArgument = None,
-        config_dict: ConfigArgument = None,
-        filter_function: ConfigArgument = None,
-        eval_env: Optional[bool] = None,
-        allow_empty: Optional[bool] = None,
-        *slot_args,
-        **slot_kwargs,
-    ) -> Union[ConfigGroup, Any]:
-        """Config parser from config files.
-
-        :param files: Default config files
-        :param sections: Default config sections
-        :param config_dict: Config dictionary to pass already loaded configs
-        :param slot_kwargs: Default configs to overwrite passed class
-        :param filter_function: Optional filter method for config
-        :param eval_env: Flag to evaluate environment variables into default values.
-        :param allow_empty: Flag that allows empty config result -> e.g. emtpy list
-        :param slot_args: Default configs to overwrite passed class
-        :param slot_kwargs: Default configs to overwrite passed class
-
-        :returns: Nested Lists of Config Classes
-
-        """
-        if not files:
-            files = cls.__config_files__
-
-        # if not config_dict:
-        #     config_dict = OrderedDict(loader({None: files}, eval_env=eval_env))
-        #     print(config_dict)
-        # logging.debug(f"Read config with sections: {config_dict.keys()}")
-        for slot_class in list(getattr(cls, "__annotations__", {}).values())[len(slot_args) :]:
-            if is_config_list(slot_class):
-                slot_class = slot_class.__args__[0]
-            if is_config(slot_class):
-                slot_kwargs.update(
-                    slot_class.from_file(
-                        files=files,
-                        sections=sections,
-                        config_dict=config_dict,
-                        filter_function=filter_function or cls.__config_filter_function__,
-                        eval_env=eval_env,
-                        allow_empty=allow_empty or cls.__allow_empty_config__,
-                    )
-                )
-        error_args = [key for key in slot_kwargs if key not in cls.__dataclass_fields__]
-        if error_args:
-            logging.debug(f"The variables {error_args} in **{cls.__name__}** are not defined!")
-            logging.debug("Use generate_group in build script to auto generate the config group!")
-
-        return cls(*slot_args, **{key: value for key, value in slot_kwargs.items() if key not in error_args})
-
-    return from_file  # class not dependent method
+    return cls
```

### Comparing `cornflakes-3.3.7/cornflakes/decorator/config/dict.py` & `cornflakes-3.3.8/cornflakes/decorator/dataclasses/config/_dict.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import os
 from typing import Any, Callable, Dict, List, Optional, Union
 
-from cornflakes.decorator.config._load_config import create_file_loader
-from cornflakes.decorator.types import Config
+from cornflakes.decorator.dataclasses.config._load_config import create_file_loader
+from cornflakes.types import Config
 
 
 def create_dict_file_loader(
-    cls: Union[Config, Any],
+    cls,
 ) -> Callable[..., Dict[str, Optional[Union[Config, List[Config], Any]]]]:
     """Method to create file loader for passed dict."""
 
     def from_dict(*args, config_dict=None, **kwargs) -> Dict[str, Optional[Union[Config, List[Config], Any]]]:
         if not config_dict:
             config_dict = {}
         default_kwargs = {}
         if cls.__eval_env__:
             default_kwargs.update(
-                {key: os.environ[key] for key in cls.__dataclass_fields__.keys() if key in os.environ.keys()}
+                {key: os.environ[key] for key in cls.__dataclass_fields__.keys() if key in os.environ}
             )
         default_kwargs.update(kwargs)
-        return create_file_loader(cls=cls)(*args, config_dict=config_dict, **default_kwargs)
+        return create_file_loader(cls=cls, _instantiate=True)(*args, config_dict=config_dict, **default_kwargs)
 
     return from_dict
```

### Comparing `cornflakes-3.3.7/cornflakes/decorator/config/ini.py` & `cornflakes-3.3.8/cornflakes/decorator/dataclasses/config/_ini.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,38 +1,46 @@
 import logging
-from typing import Any, Optional, Union
+from typing import Callable, Dict, List, Optional, Union
 
 from cornflakes import ini_load
 from cornflakes.common import type_to_str
-from cornflakes.decorator.config._load_config import create_file_loader
-from cornflakes.decorator.config._write_config import write_config
-from cornflakes.decorator.dataclass.helper import get_not_ignored_slots, is_config
-from cornflakes.decorator.types import Config
+from cornflakes.decorator.dataclasses._helper import get_not_ignored_slots, is_config
+from cornflakes.decorator.dataclasses.config._load_config import create_file_loader
+from cornflakes.decorator.dataclasses.config._write_config import write_config
+from cornflakes.types import Config
 
 
 def _parse_config_list(cfg, cfg_name: str, title: str):
     _ini_bytes = bytearray()
     is_list = isinstance(cfg, list)
     if is_config(cfg) and not is_list:
-        return cfg.to_ini_bytes(cfg_name)
+        return to_ini_bytes(cfg, cfg_name)
     elif is_list:
         for n, sub_cfg in enumerate(cfg):
-            sub_cfg_name = f"{cfg_name}_{n}"
-            if is_config(sub_cfg) and (hasattr(sub_cfg, "section_name") or hasattr(sub_cfg, "__config_sections__")):
+            sub_cfg_name = cfg_name
+            if is_config(sub_cfg) and (
+                getattr(sub_cfg, "section_name", None) or getattr(sub_cfg, "__config_sections__", None)
+            ):
                 # if sub_cfg contains a section_name, use it instead of the default
                 sub_cfg_name = getattr(sub_cfg, "section_name", sub_cfg.__config_sections__)
+                if isinstance(sub_cfg_name, (list, tuple)):
+                    sub_cfg_name = sub_cfg_name[0]
+
+            if not sub_cfg_name:
+                sub_cfg_name = f"{cfg_name}_{n}"
+
             _ini_bytes.extend(_parse_config_list(sub_cfg, sub_cfg_name, title))
         return _ini_bytes
     else:
         logging.warning(f"The Value {cfg_name} of {title} be in a child config class!")
         return b""
 
 
 def to_ini_bytes(
-    self, title: Optional[str] = None
+    self, title: str
 ) -> Optional[bytearray]:  # TODO: implement more type_to_str feature -> date format etc.
     """Method to write an instance of the main config class of the module into a ini bytearray."""
     _ini_bytes = bytearray()
     has_lists = isinstance(self, list)
     if is_config(self) and not has_lists:
         _ini_bytes.extend(bytes(f"[{title}]\n", "utf-8"))
         _ini_bytes.extend(
@@ -61,24 +69,24 @@
 
 
 def to_ini(self, out_cfg: Optional[str] = None) -> Optional[bytearray]:
     """Method to write an instance of the main config class of the module into an ini file."""
     title = getattr(self, "section_name", getattr(self, "__config_sections__", self.__class__.__name__.lower()))
     if isinstance(title, (list, tuple)):
         title = title[0]
-    return write_config(self.to_ini_bytes(title), out_cfg)
+    return write_config(bytearray(to_ini_bytes(self, title) or b""), out_cfg)
 
 
 def create_ini_file_loader(
-    cls: Union[Config, Any],
-):
+    cls,
+) -> Callable[..., Dict[str, Optional[Union[Config, List[Config]]]]]:
     """Method to create file loader for ini files."""
 
-    def from_ini(*args, **kwargs):
-        return create_file_loader(cls=cls, loader=ini_load)(*args, **kwargs)  # type: ignore
+    def from_ini(*args, **kwargs) -> Dict[str, Optional[Union[Config, List[Config]]]]:
+        return create_file_loader(cls=cls, _loader_callback=ini_load, _instantiate=True)(*args, **kwargs)  # type: ignore
 
     return from_ini
 
 
 # def create_ini_group_loader(
 #     cls=None,
 # ) -> Callable[..., ConfigGroup]:
```

### Comparing `cornflakes-3.3.7/cornflakes/decorator/config/yaml.py` & `cornflakes-3.3.8/cornflakes/decorator/dataclasses/config/_yaml.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,55 +1,43 @@
-from typing import Any, Callable, Dict, List, Optional, Type, Union
+from typing import Callable, Dict, List, Optional, Type, Union
 
 import yaml
 from yaml import SafeLoader, UnsafeLoader
 
-from cornflakes.decorator.config._load_config import create_file_loader
-from cornflakes.decorator.config._write_config import write_config
-from cornflakes.decorator.types import Config
+from cornflakes.decorator.dataclasses.config._load_config import create_file_loader
+from cornflakes.decorator.dataclasses.config._write_config import write_config
 from cornflakes.parser import yaml_load
+from cornflakes.types import Config
 
 
 def specific_yaml_loader(loader: Union[Type[SafeLoader], Type[UnsafeLoader]] = SafeLoader):
     """Wrapper method to predefine yaml loader parameter."""
 
     def _yaml_loader(*args, **kwargs):
         return yaml_load(*args, loader=loader, **kwargs)
 
     return _yaml_loader
 
 
-def to_yaml_bytes(self, *args, **kwargs) -> Optional[bytearray]:
+def to_yaml_bytes(self, *args, **kwargs) -> bytes:
     """Method to write an instance of the main config class of the module into a yaml bytearray."""
     return yaml.dump({self.__class__.__name__.lower(): self.to_dict()}, *args, **kwargs).encode("utf-8")
 
 
-def to_yaml(self, out_cfg: Optional[str] = None, *args, **kwargs) -> Optional[bytearray]:
+def to_yaml(self, *args, out_cfg: Optional[str] = None, **kwargs) -> Optional[bytearray]:
     """Method to write an instance of the main config class of the module into a yaml file."""
     # TODO: More Tests for nested Objects
-    return write_config(self.to_yaml_bytes(*args, **kwargs), out_cfg)
+    return write_config(bytearray(to_yaml_bytes(self, *args, **kwargs)), out_cfg)
 
 
 def create_yaml_file_loader(
-    cls: Union[Config, Any],
+    cls,
 ) -> Callable[..., Dict[str, Optional[Union[Config, List[Config]]]]]:
     """Method to create file loader for yaml files."""
 
     def from_yaml(
         *args, loader: Union[Type[SafeLoader], Type[UnsafeLoader]] = SafeLoader, **kwargs
     ) -> Dict[str, Optional[Union[Config, List[Config]]]]:
-        _from_yaml = create_file_loader(cls=cls, loader=specific_yaml_loader(loader=loader))  # type: ignore
+        _from_yaml = create_file_loader(cls=cls, _loader_callback=specific_yaml_loader(loader=loader))  # type: ignore
         return _from_yaml(*args, **kwargs)
 
     return from_yaml
-
-
-# def create_yaml_group_loader(
-#     cls=None,
-# ) -> Callable[..., ConfigGroup]:
-#     """Method to create file loader for yaml files."""
-#
-#     def from_yaml(*args, loader: Union[Type[SafeLoader], Type[UnsafeLoader]] = SafeLoader, **kwargs) -> ConfigGroup:
-#         _from_yaml = create_group_loader(cls=cls, loader=specific_yaml_loader(loader=loader))  # type: ignore
-#         return _from_yaml(*args, **kwargs)
-#
-#     return from_yaml
```

### Comparing `cornflakes-3.3.7/cornflakes/decorator/dataclass/_enforce_types.py` & `cornflakes-3.3.8/cornflakes/decorator/datalite/commons.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,199 +1,244 @@
-import inspect
-from contextlib import suppress
-from dataclasses import MISSING, is_dataclass
-from itertools import chain
-from os import environ
-from typing import Any, Callable, Optional, Union, get_args
-
-from _cornflakes import eval_type
-from cornflakes.common import extract_var_names
-from cornflakes.decorator._wrap_kwargs import wrap_kwargs
-from cornflakes.decorator.dataclass.helper import dataclass_fields
-from cornflakes.decorator.types import WITHOUT_DEFAULT, Config, ConfigGroup, DataclassProtocol
-
-# from types import GenericAlias
-# import typing
-#
-# t_UnionGenericAlias = getattr(typing, "_UnionGenericAlias", None)
-# t_GenericAlias = getattr(typing, "_GenericAlias", None)
-#
-#
-# def get_types_from_typing(t) -> Union[List, Any]:
-#     result = []
-#
-#     def recursive(t):
-#         if type(t) in (t_UnionGenericAlias, t_GenericAlias):
-#             for arg in t.__args__:
-#                 recursive(arg)
-#         elif type(t) is GenericAlias:
-#             result.append(t.__subclasshook__.__self__)
-#         else:
-#             result.append(t)
-#
-#     recursive(t)
-#     if len(result) == 1:
-#         return result[0]
-#     return result
+from dataclasses import Field
+from datetime import date, datetime, time
+from decimal import Decimal
+from enum import Enum
+from inspect import isclass
+from ipaddress import IPv4Address, IPv6Address
+import json
+import pickle
+import re
+import sqlite3 as sql
+from typing import Any, Callable, Dict, Generator, List, Optional, Tuple, Type, Union
+from uuid import UUID
+
+from cornflakes.decorator.dataclasses import dataclass_fields
+from cornflakes.decorator.datalite.constraints import Unique
+
+
+def str_to_bool(s: str) -> bool:
+    if s.lower() == "true":
+        return True
+    elif s.lower() == "false":
+        return False
+    else:
+        raise ValueError("String does not represent a boolean value")
+
+
+def default_formatter(x: Any) -> Any:
+    return x
+
+
+def uuid_formatter(x: UUID) -> bytes:
+    return x.bytes
+
+
+def generator_formatter(_: "Generator") -> None:
+    raise ValueError("Generators cannot be serialized to SQLite")
+
 
 SpecialForm = type(Optional)
 
-_empty = getattr(inspect, "_empty", None)
+type_table: Dict[Union[Optional[type], Any], str] = {
+    None: "NULL",
+    type(None): "NULL",
+    int: "INTEGER",
+    float: "REAL",
+    str: "TEXT",
+    bytes: "BLOB",
+    bool: "INTEGER",
+    datetime: "TIMESTAMP",
+    date: "DATE",
+    time: "TIME",
+    Decimal: "NUMERIC",
+    # additional types
+    tuple: "JSON",
+    Tuple: "JSON",
+    list: "JSON",
+    List: "JSON",
+    dict: "JSON",
+    Dict: "JSON",
+    IPv4Address: "TEXT",
+    IPv6Address: "TEXT",
+    Enum: "TEXT",
+    complex: "TEXT",
+    set: "TEXT",
+    frozenset: "TEXT",
+    bytearray: "BLOB",
+    memoryview: "BLOB",
+    slice: "TEXT",
+    range: "TEXT",
+    classmethod: "BLOB",
+    Any: "BLOB",
+    Type: "TEXT",
+    Callable: "BLOB",
+    Generator: "TEXT",
+    Optional: "BLOB",
+    Union: "BLOB",
+    UUID: "TEXT",
+}
+
+type_table.update(
+    {
+        Unique[getattr(key, "__args__", type(None))]  # type: ignore
+        if isinstance(key, SpecialForm)
+        else Unique[key]: f"{value}" + ("" if isinstance(key, SpecialForm) else " NOT NULL UNIQUE")  # type: ignore
+        for key, value in type_table.items()
+    }
+)
 
+validator_table: Dict[str, Union[Callable[[Any], Any], Type]] = {
+    "NULL": type(None),
+    "INTEGER": int,
+    "REAL": float,
+    "TEXT": str,
+    "BLOB": lambda x: bytes(x) if isinstance(x, (bytes, bytearray)) else x,
+    "TIMESTAMP": lambda x: isinstance(x, datetime) and str(x) or "NULL",
+    "DATE": lambda x: isinstance(x, date) and str(x) or "NULL",
+    "TIME": lambda x: isinstance(x, time) and str(x) or "NULL",
+    "NUMERIC": lambda x: Decimal(str(x)),
+}
+
+formatter_table: Dict[Union[Type, Any], Any] = {
+    int: str,
+    float: str,
+    Decimal: str,
+    str: str,
+    bytes: lambda x: re.sub('(^"|"$)', "", json.dumps(str(x)[2:-1])),
+    type(None): lambda _: "",
+    bool: lambda x: str(int(x)),
+    UUID: str,
+    # additional formatters
+    tuple: lambda x: json.dumps(list(x)),
+    Tuple: lambda x: json.dumps(list(x)),
+    list: lambda x: json.dumps(x),
+    List: lambda x: json.dumps(x),
+    dict: lambda x: json.dumps(x),
+    Dict: lambda x: json.dumps(x),
+    datetime: lambda x: str(x),
+    date: lambda x: str(x),
+    time: lambda x: str(x),
+    IPv4Address: lambda x: re.sub('(^"|"$)', "", json.dumps(str(x))),
+    IPv6Address: lambda x: re.sub('(^"|"$)', "", json.dumps(str(x))),
+    Enum: lambda x: re.sub('(^"|"$)', "", json.dumps(x.value)),
+    complex: lambda x: re.sub('(^"|"$)', "", json.dumps(str(x))),
+    set: lambda x: list(x),
+    frozenset: lambda x: list(x),
+    bytearray: lambda x: '"' + str(bytes(x)).replace("b'", "")[:-1] + '"',
+    memoryview: lambda x: '"' + str(bytes(x)).replace("b'", "")[:-1] + '"',
+    slice: lambda x: json.dumps(f"{x.start}:{x.stop}:{x.step}"),
+    range: lambda x: json.dumps(f"{x.start}:{x.stop}:{x.step}"),
+    classmethod: lambda x: str(x),
+    Any: lambda x: pickle.dumps(x),
+    Type: lambda x: json.dumps(x.__name__),
+    Callable: lambda x: pickle.dumps(x),
+    Generator: lambda x: list(x),
+    Optional: lambda x: pickle.dumps(x),
+    Union: lambda x: pickle.dumps(x),
+}
 
-def enforce_types(config: Union[DataclassProtocol, Config, ConfigGroup, Any], validate=False):  # noqa: C901
-    """Adds a simple decorator enforce_types that enables enforcing strict typing on a function or dataclass using annotations.
 
-    Works with collection types and subtypes for example Dict[str, Tuple[int, int]], and with special types as Optional and Any.
-    Base Reference: https://github.com/matchawine/python-enforce-typing
+def _convert_type(type_hint: Optional[type], type_overload: Optional[Dict[Optional[type], str]] = None) -> str:
     """
-    validators = {
-        key: validator
-        for key, value in config.__dataclass_fields__.items()
-        if callable(validator := getattr(value, "validator", key))
-    }
+    Given a Python type, return the str name of its
+    SQLlite equivalent.
+    :param type_hint: A Python type, or None.
+    :param type_overload: A type table to overload the custom type table.
+    :return: The str name of the sql type.
+    >>> _convert_type(int)
+    'INTEGER'
+    """
+    if type_overload is None:
+        type_overload = type_table
+    try:
+        actual_type: Any = getattr(type_hint, "__origin__", getattr(type_hint, "type", type_hint))
+        if isinstance(actual_type, SpecialForm):
+            actual_type = getattr(type_hint, "__args__", type_hint)
+        if isclass(actual_type) and issubclass(actual_type, Enum):
+            actual_type = Enum
+        if isinstance(actual_type, list) or isinstance(actual_type, tuple):
+            actual_type = next(item for item in actual_type if not isinstance(item, type(None)))
+        return type_overload[actual_type]
+    except KeyError:
+        raise TypeError("Requested type not in the default or overloaded type table.")
+
+
+def _validate_sql_type(value, db_type):
+    """Validate and format value for insertion into SQLite."""
+    if value is None:
+        return ""
+    return validator_table[db_type](value)
 
-    required_keys = [
-        key
-        for key, f in dataclass_fields(config).items()
-        if (f.default_factory == WITHOUT_DEFAULT) or (f.default_factory == MISSING and f.default == MISSING)
-    ]
-
-    def _check_type(type_hint: Any, key, value, skip=False):
-        if isinstance(type_hint, type(None)):
-            return
-
-        if isinstance(type_hint, SpecialForm):
-            return value
-
-        if inspect.isclass(type_hint) and isinstance(value, type_hint):
-            return value
-
-        if is_dataclass(type_hint) and isinstance(value, dict):
-            return type_hint(**value)
-
-        with suppress(KeyError):
-            actual_type: Any = getattr(type_hint, "__origin__", getattr(type_hint, "type", type_hint))
-
-            if isinstance(actual_type, SpecialForm):
-                actual_type = getattr(type_hint, "__args__", type_hint)
-
-            if actual_type == str:
-                return str(value or "")  # fix default string is not 'None'
-
-            if isinstance(actual_type, list) or isinstance(actual_type, tuple):
-                actual_types = (
-                    [t for t in actual_type if t is not None]
-                    if value
-                    else [type(None)]
-                    if type(None) in actual_type
-                    else actual_type
-                )
-                if not any(inspect.isclass(t) for t in actual_types):
-                    if value not in actual_types:
-                        if skip:
-                            return
-                        raise TypeError(
-                            f"Expected any of {actual_types!r} for attribute {key!r} but received type {type(value)!r})."
-                        )
-                    actual_types = [type(t) for t in actual_types]
-                values = [_check_type(t, key, value, skip=True) for t in actual_types]
-                if not any(values) and type(None) in actual_types:
-                    return None
-                if not any(values):
-                    if skip:
-                        return
-                    raise TypeError(
-                        f"Expected any of {actual_types!r} for attribute {key!r} but received type {type(value)!r})."
-                    )
-                return next(item for item in values if item is not None)
-
-            if actual_type in [list, tuple]:
-                if not isinstance(value, (list, tuple)):
-                    if skip:
-                        return
-                    raise TypeError(
-                        f"Expected type {type_hint!r} for attribute {key!r} but received type {type(value)!r})."
-                    )
-                actual_types = [t for t in get_args(type_hint) if t is not None] or [str] if value else [type(None)]
-                return actual_type(chain([_check_type(t, key, val) for val in value for t in actual_types]))
-
-            if inspect.isbuiltin(actual_type) or inspect.isfunction(actual_type):
-                return actual_type(value)
-
-            if not inspect.isclass(actual_type):
-                return _check_type(actual_type, key, value)
-
-            if not isinstance(value, actual_type):
-                try:
-                    if not validate:
-                        if skip:
-                            return
-                        raise TypeError(
-                            f"Expected type {type_hint!r} for attribute {key!r} but received type {type(value)!r})."
-                        )
-                    return actual_type(value)  # type: ignore
-                except Exception as exc:
-                    if skip:
-                        return
-                    raise Exception(
-                        f"\n{exc}\n"
-                        f"Expected type {type_hint!r} for attribute {key!r} but received type {type(value)!r})."
-                    ) from exc
-
-            return value
-
-    def _get_env_vars():
-        return {key: eval_type(environ[key]) for key in config.__dataclass_fields__.keys() if key in environ.keys()}
-
-    def _validate(self, values, key, callback: Callable[..., Any]):
-        try:
-            co_varnames = extract_var_names(callback)
-            kwargs = {}
-            kwargs.update(co_varnames)
-            kwargs.update({"self": self, "values": values, "key": key})
-            kwargs.update(values)
-            kwargs = {key: value for key, value in kwargs.items() if key in co_varnames.keys() and value is not _empty}
-            if len(missing := [key for key in co_varnames.keys() if key not in kwargs.keys()]) > 1:
-                raise TypeError(f"Argument not provided: {missing})")
-            if len(missing) == 1:
-                return callback(values.pop(key), **kwargs)
-            return callback(**kwargs)
-        except Exception as exc:
-            raise Exception(f"Failed to validate {key} with {callback}!") from exc
-
-    def _process_validator(self, values, validators: dict, **kwargs):
-        return {
-            key: _validate(self, values, key, callback) for key, callback in validators.items() if key in kwargs.keys()
-        }
-
-    def _process_type_checking(**kwargs):
-        return {
-            key: _check_type(getattr(config, "__annotations__", {})[key], key, value)
-            for key, value in kwargs.items()
-            if key in config.__dataclass_fields__.keys()
-        }
-
-    def decorate(func):
-        @wrap_kwargs(func)
-        def wrapper(self, *args, **kwargs):
-            argument_names = func.__code__.co_varnames[1:]
-            argument_values = args[: len(argument_names)]
-            kwargs.update(dict(zip(argument_names, argument_values)))  # noqa: B905
-            default_kwargs = {}
-            default_kwargs.update(kwargs)
-            if self.__eval_env__:
-                default_kwargs.update(_get_env_vars())
-
-            default_kwargs.update(_process_validator(self, default_kwargs, validators, **default_kwargs))
-
-            default_kwargs.update(_process_type_checking(**default_kwargs))
-            default_kwargs.pop("self", None)
-            if missing_keys := [key for key in required_keys if key not in default_kwargs.keys()]:
-                raise ValueError(f"Missing required values for keys {missing_keys}")
-            return func(self, **default_kwargs)  # type: ignore
 
-        return wrapper
+def _convert_sql_format(value: Any) -> Union[str, int]:
+    """
+    Given a Python value, convert to string representation
+    of the equivalent SQL datatype.
+    :param value: A value, ie: a literal, a variable etc.
+    :return: The string representation of the SQL equivalent.
+    >>> _convert_sql_format(1)
+    '1'
+    >>> _convert_sql_format("John Smith")
+    'John Smith'
+    """
+    try:
+        type_hint = type(value)
+        actual_type: Any = getattr(type_hint, "__origin__", getattr(type_hint, "type", type_hint))
+        if isinstance(actual_type, SpecialForm):
+            actual_type = getattr(type_hint, "__args__", type_hint)
+        if isclass(actual_type) and issubclass(actual_type, Enum):
+            actual_type = Enum
+        return formatter_table[actual_type](value)
+    except KeyError:
+        raise TypeError("Requested type not in the default or overloaded type table.")
 
-    config.__init__ = decorate(config.__init__)
 
-    return config
+def _get_table_cols(cur: sql.Cursor, table_name: str) -> List[str]:
+    """
+    Get the column data of a table.
+
+    :param cur: Cursor in database.
+    :param table_name: Name of the table.
+    :return: the information about columns.
+    """
+    cur.execute(f"PRAGMA table_info({table_name});")
+    return [row_info[1] for row_info in cur.fetchall()][1:]
+
+
+def _get_default(default_object: object, type_overload: Dict[Optional[type], str], db_type: str) -> str:
+    """
+    Check if the field's default object is filled,
+    if filled return the string to be put in the,
+    database.
+    :param default_object: The default field of the field.
+    :param type_overload: Type overload table.
+    :return: The string to be put on the table statement,
+    empty string if no string is necessary.
+    """
+    if type(default_object) in type_overload:
+        value = _convert_sql_format(_validate_sql_type(default_object, db_type))
+        if db_type in ["TEXT", "DATE", "TIMESTAMP", "TIME"]:
+            return f" DEFAULT '{value}'"
+        return f" DEFAULT {value}"
+    return ""
+
+
+def _create_table(class_: type, cursor: sql.Cursor, type_overload: Optional[Dict[Optional[type], str]] = None) -> None:
+    """
+    Create the table for a specific dataclass given
+    :param class_: A dataclass.
+    :param cursor: Current cursor instance.
+    :param type_overload: Overload the Python -> SQLDatatype table
+    with a custom table, this is that custom table.
+    :return: None.
+    """
+    if not type_overload:
+        type_overload = type_table
+    fields: List[Field] = [dataclass_fields(class_)[key] for key in dataclass_fields(class_).keys()]
+    fields.sort(key=lambda field: field.name)  # Since dictionaries *may* be unsorted.
+    sql_fields = ", ".join(
+        f"{field.name} {_convert_type(field.type, type_overload)}"
+        f"{_get_default(field.default, type_overload, _convert_type(field.type, type_overload))}"
+        for field in fields
+    )
+    sql_fields = "obj_id INTEGER PRIMARY KEY AUTOINCREMENT, " + sql_fields
+    cursor.execute(f"CREATE TABLE IF NOT EXISTS {class_.__name__.lower()} ({sql_fields});")
```

### Comparing `cornflakes-3.3.7/cornflakes/decorator/dataclass/_field.py` & `cornflakes-3.3.8/cornflakes/decorator/dataclasses/_field.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,12 @@
 from dataclasses import Field as DataclassField
 from dataclasses import MISSING
-from typing import Any, Callable, List, Optional, Union
+from typing import Any, Callable, List, Optional, Union, cast
 
-from cornflakes.decorator.types import WITHOUT_DEFAULT, _WithoutDefault
-
-_MISSING_TYPE = type(MISSING)
-
-
-# TODO: add init_var_trigger -> like alias to call the validator method and pass the values
+from cornflakes.types import MISSING_TYPE, WITHOUT_DEFAULT, WITHOUT_DEFAULT_TYPE
 
 
 class Field(DataclassField):
     """Instances of dataclasses Field wrapped for configs.
 
     Info:
        currently only supported arguments are:
@@ -23,15 +18,15 @@
         *getattr(
             DataclassField,
             "__slots__",
             (),
         ),
         "validator",
         "ignore",
-        "alias",
+        "aliases",
         "title",
         "description",
         "exclude",
         "include",
         "const",
         "gt",
         "ge",
@@ -50,24 +45,24 @@
         "regex",
         "discriminator",
         "extra",
     )
 
     def __init__(
         self,
-        default: Union[_MISSING_TYPE, Any] = MISSING,
-        default_factory: Union[_MISSING_TYPE, _WithoutDefault, Callable[..., Any]] = MISSING,
+        default: Union[MISSING_TYPE, Any] = MISSING,
+        default_factory: Union[MISSING_TYPE, WITHOUT_DEFAULT_TYPE, Callable[..., Any]] = MISSING,
         init: Optional[bool] = True,
         repr: Optional[bool] = True,
-        hash: Optional[Union[bool, _MISSING_TYPE]] = None,
+        hash: Optional[Union[bool, MISSING_TYPE]] = None,
         compare: Optional[bool] = True,
         metadata: Any = None,
-        kw_only: Union[_MISSING_TYPE, bool] = MISSING,
-        validator: Optional[Union[Callable[[str], Any], _MISSING_TYPE]] = MISSING,
-        alias: Optional[Union[List[str], str]] = None,
+        kw_only: Union[MISSING_TYPE, bool] = MISSING,
+        validator: Optional[Union[Callable[[str], Any], MISSING_TYPE]] = MISSING,
+        aliases: Optional[Union[List[str], str]] = None,
         ignore: Optional[bool] = False,
         title: Optional[str] = None,
         description: Optional[str] = None,
         exclude: Optional[Union[str, List[str]]] = None,
         include: Optional[Union[str, List[str]]] = None,
         const: Optional[bool] = None,
         gt: Optional[Union[int, float]] = None,
@@ -95,15 +90,15 @@
         :param init: Field will be included in __init__ method.
         :param repr: Field will be included in __repr__ method.
         :param hash: Field will be included in __hash__ method.
         :param compare: Field will be included in __eq__ method.
         :param metadata: Field will be included in metadata.
         :param kw_only: Field will be included in __init__ method as keyword only.
         :param validator: Validator for field.
-        :param alias: Aliases for config data (will be used to read from config files).
+        :param aliases: Aliases for config data (will be used to read from config files).
         :param ignore: Field will be ignored when writing to_ini etc.
         :param title: Can be any string, used in the schema.
         :param description: can be any string, used in the schema.
         :param exclude: exclude this field while dumping. Takes same values as
                 the ``include`` and ``exclude`` arguments on the ``.dict`` method.
         :param include: include this field while dumping. Takes same values as the
                 ``include`` and ``exclude`` arguments on the ``.dict`` method.
@@ -141,17 +136,25 @@
         :param discriminator: only useful with a (discriminated a.k.a. tagged) `Union` of sub models with a common field.
                 The `discriminator` is the name of this common field to shorten validation and improve generated schema
         :param repr: show this field in the representation
         :param extra: any additional keyword arguments will be added as is to the schema
 
         Returns: None
         """
-        self.validator = validator
+        if isinstance(validator, MISSING_TYPE) or not callable(validator):
+
+            def validator_decorator(func) -> Any:
+                self.validator = func
+                return func
+
+            self.validator = validator_decorator
+        else:
+            self.validator = validator
         self.ignore = ignore
-        self.alias = alias
+        self.aliases = aliases
         self.title = title
         self.description = description
         self.exclude = exclude
         self.include = include
         self.const = const
         self.gt = gt
         self.ge = ge
@@ -205,15 +208,15 @@
                 ("kw_only", self.kw_only),  # type: ignore
             )
             if key in Field.__init__.__code__.co_varnames
         }
         return self.__class__(
             **dc_field_args,
             validator=self.validator,
-            alias=self.alias,
+            aliases=self.aliases,
             ignore=self.ignore,
             title=self.title,
             description=self.description,
             exclude=self.exclude,
             include=self.include,
             const=self.const,
             gt=self.gt,
@@ -240,15 +243,15 @@
 
         :return: Field repr
         """
         return (
             f"{DataclassField.__repr__(self)[:-1]}, "
             f"validator={self.validator!r}, "
             f"ignore={self.ignore!r}, "
-            f"alias={self.alias!r}, "
+            f"aliases={self.aliases!r}, "
             f"title={self.title!r}, "
             f"description={self.description!r}, "
             f"exclude={self.exclude!r}, "
             f"include={self.include!r}, "
             f"const={self.const!r}, "
             f"gt={self.gt!r}, "
             f"ge={self.ge!r}, "
@@ -266,25 +269,27 @@
             f"allow_mutation={self.allow_mutation!r}, "
             f"regex={self.regex!r}, "
             f"discriminator={self.discriminator!r})"
         )
 
 
 def field(
+    attr: Optional[Union[Field, Any]] = None,
+    /,
     *,
-    default: Union[_MISSING_TYPE, Any] = MISSING,
-    default_factory: Union[_MISSING_TYPE, _WithoutDefault, Callable[..., Any]] = MISSING,
+    default: Union["MISSING_TYPE", Any] = MISSING,
+    default_factory: Union[MISSING_TYPE, WITHOUT_DEFAULT_TYPE, Callable[..., Any]] = MISSING,
     init: Optional[bool] = True,
     repr: Optional[bool] = True,
-    hash: Optional[Union[bool, _MISSING_TYPE]] = None,
+    hash: Optional[Union[bool, MISSING_TYPE]] = None,
     compare: Optional[bool] = True,
     metadata: Any = None,
-    kw_only: Union[_MISSING_TYPE, bool] = MISSING,
-    validator: Optional[Union[Callable[[str], Any], _MISSING_TYPE]] = MISSING,
-    alias: Optional[Union[List[str], str]] = None,
+    kw_only: Union[MISSING_TYPE, bool] = MISSING,
+    validator: Optional[Union[Callable[[str], Any], MISSING_TYPE]] = MISSING,
+    aliases: Optional[Union[List[str], str]] = None,
     ignore: Optional[bool] = False,
     title: Optional[str] = None,
     description: Optional[str] = None,
     exclude: Optional[Union[str, List[str]]] = None,
     include: Optional[Union[str, List[str]]] = None,
     const: Optional[bool] = None,
     gt: Optional[Union[int, float]] = None,
@@ -301,32 +306,33 @@
     min_length: Optional[int] = None,
     max_length: Optional[int] = None,
     allow_mutation: Optional[bool] = True,
     regex: Optional[str] = None,
     discriminator: Optional[str] = None,
     no_default: bool = False,
     **extra: Any,
-) -> Union[DataclassField, Any]:
+):
     """This function is used instead of exposing Field creation directly.
 
     So that a type checker can be told (via overloads) that this is a function whose type depends on its parameters.
     This function is used instead of exposing Field creation directly,
     so that a type checker can be told (via overloads) that this is a
     function whose type depends on its parameters.
 
+    :param attr: Attribute name on the class to be used to store the field.
     :param default: Default value for field.
     :param default_factory: Default factory for field.
     :param init: Field will be included in __init__ method.
     :param repr: Field will be included in __repr__ method.
     :param hash: Field will be included in __hash__ method.
     :param compare: Field will be included in __eq__ method.
     :param metadata: Field will be included in metadata.
     :param kw_only: Field will be included in __init__ method as keyword only.
     :param validator: Validator for field.
-    :param alias: Aliases for config data (will be used to read from config files).
+    :param aliases: Aliases for config data (will be used to read from config files).
     :param ignore: Field will be ignored when writing to_ini etc.
     :param title: Can be any string, used in the schema.
     :param description: can be any string, used in the schema.
     :param exclude: exclude this field while dumping. Takes same values as
             the ``include`` and ``exclude`` arguments on the ``.dict`` method.
     :param include: include this field while dumping. Takes same values as the
             ``include`` and ``exclude`` arguments on the ``.dict`` method.
@@ -371,25 +377,29 @@
     :raises ValueError: if both default and default_factory are specified.
     """
     if default is not MISSING and default_factory is not MISSING:
         raise ValueError("cannot specify both default and default_factory")
 
     if default is MISSING and default_factory is MISSING and no_default:
         default_factory = WITHOUT_DEFAULT
-    new_field = Field(
+
+    if attr:
+        return cast(Field, attr)
+
+    return Field(
         default=default,
         default_factory=default_factory,
         init=init,
         repr=repr,
         hash=hash,
         compare=compare,
         metadata=metadata,
         kw_only=kw_only,
         validator=validator,
-        alias=alias,
+        aliases=aliases,
         ignore=ignore,
         title=title,
         description=description,
         exclude=exclude,
         include=include,
         const=const,
         gt=gt,
@@ -406,8 +416,7 @@
         min_length=min_length,
         max_length=max_length,
         allow_mutation=allow_mutation,
         regex=regex,
         discriminator=discriminator,
         **extra,
     )
-    return new_field
```

### Comparing `cornflakes-3.3.7/cornflakes/decorator/dataclass/helper.py` & `cornflakes-3.3.8/cornflakes/decorator/dataclasses/_helper.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,92 +1,145 @@
 """Dataclass helper functions used by the custom dataclass decorator."""
-from dataclasses import Field
+import dataclasses
+from dataclasses import fields as dc_fields
+from os import environ
 import re
-from typing import Any, Dict, Optional, Union
 
-from cornflakes.decorator.dataclass._field import Field as CField
-from cornflakes.decorator.types import Config, ConfigArgument, ConfigGroup, DataclassProtocol, Loader
+from _cornflakes import eval_type
+
+from cornflakes.decorator._indexer import IndexInstance
+from cornflakes.types import MISSING_TYPE, WITHOUT_DEFAULT_TYPE, Constants
 
 
 def is_config(cls):
     """Method to return flag that class is a config class."""
-    return hasattr(cls, "__config_sections__")
+    return hasattr(cls, Constants.config_decorator.SECTIONS)
 
 
 def is_group(cls):
     """Method to return flag that class is a config group class."""
-    return not is_config(cls) and hasattr(cls, "__config_files__")
+    return not is_config(cls) and hasattr(cls, Constants.config_decorator.FILES)
 
 
-def config_files(cls) -> ConfigArgument:
+def config_files(cls):
     """Method to return class __config_files__."""
-    return getattr(cls, "__config_files__", [])
+    return getattr(cls, Constants.config_decorator.FILES, [])
+
+
+def config_sections(cls):
+    """Method to return class __config_sections__."""
+    return getattr(cls, Constants.config_decorator.SECTIONS, [])
 
 
-def dataclass_fields(cls: Union[Config, ConfigGroup, DataclassProtocol, Any]) -> Dict[str, Union[Field, CField]]:
+def dataclass_fields(cls):
     """Method to return dataclass fields."""
-    return getattr(cls, "__dataclass_fields__", {})
+    return getattr(cls, Constants.dataclass_decorator.FIELDS, {})
+
+
+def dataclass_validators(cls):
+    """Method to return dataclass validators."""
+    return getattr(cls, Constants.dataclass_decorator.VALIDATORS, {})
+
 
+def dataclass_required_keys(cls):
+    """Method to return dataclass required keys."""
+    return getattr(cls, Constants.dataclass_decorator.REQUIRED_KEYS, {})
 
-def dict_factory(cls: Union[Config, ConfigGroup, DataclassProtocol, Any]) -> Any:
+
+def is_eval_env(cls):
+    """Method to return flag that class is a eval env class."""
+    return getattr(cls, Constants.dataclass_decorator.EVAL_ENV, False)
+
+
+def dict_factory(cls):
     """Method to return class __dict_factory__."""
     # dict_factory_method = getattr(cls, "__dict_factory__", dict)
     #
     # # check if any field in class is a memoryview type
     # if any([f.type == memoryview for f in dataclass_fields(cls).values()]):
     #     # if so, return a dict factory that converts memoryview to bytes
     #     def dict_factory_wrapper(obj):
     #         """Method to convert memoryview to bytes."""
     #         return dict_factory_method({k: bytes(v) if isinstance(v, memoryview) else v for k, v in obj})
     #
     #     return dict_factory_wrapper
-    return getattr(cls, "__dict_factory__", dict)
+    return getattr(cls, Constants.dataclass_decorator.DICT_FACTORY, dict)
+
+
+def evaluate_default_configs(cls, config):
+    """Method to evaluate default configs."""
+    # if is_validated(cls):
+    #     return config
+
+    for key, field in dataclass_fields(cls).items():
+        if isinstance(field.type, IndexInstance):
+            config.pop(key, None)
+    return config
+
+
+def is_validated(cls):
+    """Method to return flag that class is a validated class."""
+    return getattr(cls, Constants.config_decorator.VALIDATE, False)
 
 
 def normalized_class_name(cls):
     """Method to return class name normalized."""
     return re.sub(r"([a-z])([A-Z])", "\\1_\\2", cls.__name__).lower()
 
 
-def tuple_factory(cls: Union[Config, ConfigGroup, DataclassProtocol, Any]) -> Any:
+def tuple_factory(cls):
     """Method to return class __tuple_factory__."""
-    return getattr(cls, "__tuple_factory__", tuple)
+    return getattr(cls, Constants.dataclass_decorator.TUPLE_FACTORY, tuple)
 
 
 def is_config_list(cls):
     """Method to return flag that the object is a list of configs."""
-    return getattr(cls, "__config_list__", False) or (
-        hasattr(cls, "__args__") and getattr(cls.__args__[0], "__config_list__", False)
+    return getattr(cls, Constants.config_decorator.IS_LIST, False) or (
+        hasattr(cls, "__args__") and getattr(cls.__args__[0], Constants.config_decorator.IS_LIST, False)
     )
 
 
 def get_not_ignored_slots(cls):
     """Method to return slots that are not ignored fields."""
-    return [slot for slot in getattr(cls, "__dataclass_fields__", {}).keys() if slot not in cls.__ignored_slots__]
+    return [
+        slot
+        for slot in getattr(cls, Constants.dataclass_decorator.FIELDS, {}).keys()
+        if slot not in cls.__ignored_slots__
+    ]
 
 
-def is_multi_config(cls):
+def is_use_regex(cls):
     """Method to return flag that the config class can be empty."""
-    return getattr(cls, "__multi_config__", False)
+    return getattr(cls, Constants.config_decorator.USE_REGEX, False)
 
 
 def is_allow_empty(cls):
     """Method to return flag that the config class can be empty."""
-    return getattr(cls, "__allow_empty_config__", False)
+    return getattr(cls, Constants.config_decorator.ALLOW_EMPTY, False)
 
 
 def pass_section_name(cls):
     """Method to return flag that the config has section_name in slots, so that the section title is passed in."""
-    return "section_name" in cls.__dataclass_fields__.keys()
+    return Constants.config_decorator.SECTION_NAME_KEY in getattr(cls, Constants.dataclass_decorator.FIELDS, {})
 
 
-def get_default_loader(files: Optional[list] = None):
-    """Method to get the default loader from filenames."""
-    return (
-        Loader.DICT_LOADER
-        if not files
-        else Loader.INI_LOADER
-        if files[0][-3:] == "ini"
-        else Loader.YAML_LOADER
-        if files[0][-3:] == "yaml"
-        else Loader.DICT_LOADER
-    )
+def dc_slot_missing_default(slot):
+    """Checks if the dataclass has a default / default_factory."""
+    return isinstance(slot.default, WITHOUT_DEFAULT_TYPE) or isinstance(slot.default_factory, WITHOUT_DEFAULT_TYPE)
+
+
+def default(slot):
+    """Method to get the default value of the dataclass."""
+    return slot.default_factory if isinstance(slot.default, (MISSING_TYPE, WITHOUT_DEFAULT_TYPE)) else slot.default
+
+
+def get_env_vars(dc_cls):
+    """Method to get the environment variables for the dataclass."""
+    return {key: eval_type(environ[key]) for key in dc_cls.__dataclass_fields__.keys() if key in environ.keys()}
+
+
+def fields(class_or_instance):
+    """Patched method of the dataclasses fields method to ignore the custom dataclass."""
+    return dc_fields(class_or_instance)
+
+
+dataclasses.fields = fields
```

### Comparing `cornflakes-3.3.7/cornflakes/decorator/dataclass/validator/url.py` & `cornflakes-3.3.8/cornflakes/decorator/dataclasses/validator/url.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from dataclasses import InitVar, fields
 from typing import Any, Optional, cast
 from urllib.parse import ParseResult, parse_qs, urlparse, urlunparse
 
 import validators
 
-from cornflakes.decorator.dataclass._dataclass import dataclass as data
-from cornflakes.decorator.dataclass._dataclass import to_tuple
-from cornflakes.decorator.dataclass._field import field
+from cornflakes.decorator.dataclasses._dataclass import dataclass as data
+from cornflakes.decorator.dataclasses._dataclass import to_tuple
+from cornflakes.decorator.dataclasses._field import field
 
 
-@data(
+@data(  # type: ignore
     slots=True,
     frozen=False,
-    tuple_factory=lambda self, x: urlunparse(x[:6]),  # unparse to string
     dict_factory=lambda self, x: str(self),  # to string -> tuple -> unparse to string
+    tuple_factory=lambda self, x: urlunparse(x[:6]),  # unparse to string
 )
 class AnyUrl:
     """Database URL.
 
     :cvar url: URL to init the whole object (will be overwritten with other args).
     :cvar scheme: The scheme of the url
     :cvar netloc: user / pw / host and port of the url
@@ -30,15 +30,15 @@
     :cvar port: url port (overwrites the netloc)
     :cvar username: url username (overwrites the netloc)
     :cvar password: url password (overwrites the netloc)
     :cvar tld: url tld if it is valid
     :cvar valid: validators.url validation result
     """
 
-    url: InitVar[Optional[str]] = None
+    url: InitVar[Optional[str]] = field(default=None)
     scheme: str = field(default="", init=True)
     netloc: str = field(default="", init=True)
     path: str = field(default="", init=True)
     query: str = field(default="", init=True)
     params: str = field(default="", init=True)
     query_args: dict = field(default_factory=dict, init=True)
     fragment: str = field(default="", init=True)
@@ -70,23 +70,24 @@
                 f"{self.username or parsed.username}:{self.password or parsed.password}@"
                 if (self.username or parsed.username) and (self.password or parsed.password)
                 else f"{self.token or parsed.username}@"
                 if self.token or parsed.username
                 else ""
             )
             port = f":{self.port or parsed.port}" if self.port or parsed.port else ""
-            hostname = self.hostname if self.hostname else parsed.hostname
+            hostname = self.hostname or parsed.hostname
             self.netloc = f"{login}{hostname}{port}"
         parsed = urlparse(to_tuple(self))
         self.query_args.update(parse_qs(parsed.query))
         self.__init_parsed(parsed, overwrite=True)
-        tld = self.hostname[::-1].split(".", 1)[0][::-1]
-        if tld in VALID_ZONES:
-            self.tld = tld
-        self.valid = validators.url(self.hostname)
+        if self.hostname:
+            tld = self.hostname[::-1].split(".", 1)[0][::-1]
+            if tld in VALID_ZONES:
+                self.tld = tld
+        self.valid = validators.url(self.hostname or "")
         self.token = self.token or self.password or self.username
 
     def __str__(self) -> str:
         """Any url string."""
         return to_tuple(self)
```

### Comparing `cornflakes-3.3.7/cornflakes/decorator/datalite/constraints.py` & `cornflakes-3.3.8/cornflakes/decorator/datalite/constraints.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,13 +11,13 @@
 
 class ConstraintFailedError(Exception):
     """
     This exception is raised when a Constraint fails.
     """
 
 
-Unique = Union[Tuple[T], T]
+Unique = Union[Tuple[T], T]  # type: ignore
 """
 Dataclass fields hinted with this type signals
     datalite that the bound column of this
     field in the table is NOT NULL and UNIQUE.
 """
```

### Comparing `cornflakes-3.3.7/cornflakes/decorator/datalite/datalite_decorator.py` & `cornflakes-3.3.8/cornflakes/decorator/datalite/datalite_decorator.py`

 * *Files 8% similar despite different names*

```diff
@@ -87,13 +87,13 @@
         if type_overload is not None:
             types_table.update(type_overload)
         with sql.connect(db_path) as con:
             cur: sql.Cursor = con.cursor()
             _create_table(dataclass_, cur, types_table)
         setattr(dataclass_, "db_path", db_path)  # We add the path of the database to class itself.
         setattr(dataclass_, "types_table", types_table)  # We add the type table for migration.
-        dataclass_.create_entry = _create_entry
-        dataclass_.remove_entry = _remove_entry
-        dataclass_.update_entry = _update_entry
+        setattr(dataclass_, "create_entry", _create_entry)  # We add the path of the
+        setattr(dataclass_, "remove_entry", _remove_entry)  #
+        setattr(dataclass_, "update_entry", _update_entry)
         return dataclass_
 
     return decorator
```

### Comparing `cornflakes-3.3.7/cornflakes/decorator/datalite/fetch.py` & `cornflakes-3.3.8/cornflakes/decorator/datalite/fetch.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import sqlite3 as sql
 from typing import Any, List, Tuple
 
-from ..dataclass.helper import dataclass_fields
-from .commons import _convert_sql_format, _get_table_cols
+from cornflakes.decorator.dataclasses import dataclass_fields
+from cornflakes.decorator.datalite.commons import _convert_sql_format, _get_table_cols
 
 
 def _insert_pagination(query: str, page: int, element_count: int) -> str:
     """
     Insert the pagination arguments if page number is given.
 
     :param query: Query to insert to
@@ -82,15 +82,15 @@
     Convert a given record fetched from an SQL instance to a Python Object of given class_.
 
     :param class_: Class type to convert the record to.
     :param record: Record to get data from.
     :param field_names: Field names of the class.
     :return: the created object.
     """
-    kwargs = dict(zip(field_names, record[1:]))
+    kwargs = dict(zip(field_names, record[1:]))  # type: ignore
     field_types = {key: value.type for key, value in dataclass_fields(class_).items()}
     for key in kwargs:
         if field_types[key] == bytes:
             kwargs[key] = bytes(kwargs[key], encoding="utf-8")
     obj_id = record[0]
     obj = class_(**kwargs)
     setattr(obj, "obj_id", obj_id)
```

### Comparing `cornflakes-3.3.7/cornflakes/decorator/datalite/mass_actions.py` & `cornflakes-3.3.8/cornflakes/decorator/datalite/mass_actions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 This module includes functions to insert multiple records
 to a bound database at one time, with one time open and closing
 of the database file.
 """
 from dataclasses import asdict
 import sqlite3 as sql
-from typing import List, Tuple, TypeVar, Union
+from typing import Any, List, Tuple, TypeVar, Union
 from warnings import warn
 
 from cornflakes.decorator.datalite.commons import _convert_sql_format, _create_table
 from cornflakes.decorator.datalite.constraints import ConstraintFailedError
 
 T = TypeVar("T")
 
@@ -48,15 +48,15 @@
         warn(
             "Memory protections are turned off, " "if operations are interrupted, file may get corrupt.", RuntimeWarning
         )
         cur.execute("PRAGMA synchronous = OFF")
         cur.execute("PRAGMA journal_mode = MEMORY")
 
 
-def _mass_insert(objects: Union[List[T], Tuple[T]], db_name: str, protect_memory: bool = True) -> None:
+def _mass_insert(objects: Union[List[Any], Tuple[Any]], db_name: str, protect_memory: bool = True) -> None:
     """
     Insert multiple records into an SQLite3 database.
 
     :param objects: Objects to insert.
     :param db_name: Name of the database to insert.
     :param protect_memory: Whether memory or not
         protections are on or off.
@@ -69,15 +69,15 @@
 
     for i, obj in enumerate(objects):
         kv_pairs = asdict(obj).items()
         setattr(obj, "obj_id", first_index + i + 1)
         sql_queries.append(
             f"INSERT INTO {table_name}("
             + f"{', '.join(item[0] for item in kv_pairs)})"
-            + f" VALUES ({', '.join(_convert_sql_format(item[1]) for item in kv_pairs)});"
+            + f" VALUES ({', '.join(str(_convert_sql_format(item[1])) for item in kv_pairs)});"
         )
     with sql.connect(db_name) as con:
         cur: sql.Cursor = con.cursor()
         try:
             _toggle_memory_protection(cur, protect_memory)
             cur.execute("SELECT 'obj_id' FROM ? ORDER BY 'obj_id' DESC LIMIT 1", (table_name,))
             # TODO: Check if this is needed.
```

### Comparing `cornflakes-3.3.7/cornflakes/decorator/datalite/migrations.py` & `cornflakes-3.3.8/cornflakes/decorator/datalite/migrations.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,54 +3,54 @@
 definitions change. This functions deal with Schema Migrations.
 """
 from dataclasses import Field
 from os.path import exists
 import sqlite3 as sql
 from typing import Dict, List, Optional, Tuple, Union
 
-from cornflakes.decorator.dataclass import Field as CField
-from cornflakes.decorator.dataclass.helper import dataclass_fields
+from cornflakes.decorator.dataclasses import Field as CField
+from cornflakes.decorator.dataclasses import dataclass_fields
 from cornflakes.decorator.datalite.commons import _create_table, _get_table_cols
 
 
 def _get_db_table(class_: type) -> Tuple[str, str]:
     """
     Check if the class is a datalite class, the database exists
     and the table exists. Return database and table names.
 
     :param class_: A datalite class.
     :return: A tuple of database and table names.
     """
-    database_name: str = getattr(class_, "db_path", None)
+    database_name = getattr(class_, "db_path", None)
     if not database_name:
         raise TypeError(f"{class_.__name__} is not a datalite class.")
     table_name: str = class_.__name__.lower()
     if not exists(database_name):
         raise FileNotFoundError(f"{database_name} does not exist")
     with sql.connect(database_name) as con:
         cur: sql.Cursor = con.cursor()
         cur.execute("SELECT count(*) FROM sqlite_master WHERE type='table' AND name=?;", (table_name,))
         count: int = int(cur.fetchone()[0])
     if not count:
         raise FileExistsError(f"Table, {table_name}, already exists.")
     return database_name, table_name
 
 
-def _get_table_column_names(database_name: str, table_name: str) -> Tuple[str]:
+def _get_table_column_names(database_name: str, table_name: str) -> Tuple[str, ...]:
     """
     Get the column names of table.
 
     :param database_name: Name of the database the table
         resides in.
     :param table_name: Name of the table.
     :return: A tuple holding the column names of the table.
     """
     with sql.connect(database_name) as con:
         cur: sql.Cursor = con.cursor()
-        cols: List[str] = _get_table_cols(cur, table_name)
+        cols = _get_table_cols(cur, table_name)
     return tuple(cols)
 
 
 def _copy_records(database_name: str, table_name: str):
     """
     Copy all records from a table.
 
@@ -79,15 +79,15 @@
     with sql.connect(database_name) as con:
         cur: sql.Cursor = con.cursor()
         cur.execute("DROP TABLE ?;", (table_name,))
         con.commit()
 
 
 def _modify_records(
-    data, col_to_del: Tuple[str], col_to_add: Tuple[str], flow: Dict[str, str]
+    data, col_to_del: Tuple[str, ...], col_to_add: Tuple[str, ...], flow: Dict[str, str]
 ) -> List[Dict[str, Optional[str]]]:
     """
     Modify the asdict records in accordance
         with schema migration rules provided.
 
     :param data: Data kept as asdict in tuple.
     :param col_to_del: Column names to delete.
@@ -112,15 +112,20 @@
             if key_to_add not in record_mod:
                 record_mod[key_to_add] = None
         records.append(record_mod)
     return records
 
 
 def _migrate_records(
-    class_: type, database_name: str, data, col_to_del: Tuple[str], col_to_add: Tuple[str], flow: Dict[str, str]
+    class_: type,
+    database_name: str,
+    data,
+    col_to_del: Tuple[str, ...],
+    col_to_add: Tuple[str, ...],
+    flow: Dict[str, str],
 ) -> None:
     """
     Migrate the records into the modified table.
 
     :param class_: Class of the entries.
     :param database_name: Name of the database.
     :param data: Data, asdict tuple.
@@ -139,31 +144,35 @@
         del record["obj_id"]
         keys_to_delete = [key for key in record if record[key] is None]
         for key in keys_to_delete:
             del record[key]
         class_(**record).create_entry()
 
 
-def basic_migrate(cls: type, column_transfer: Optional[dict] = None) -> None:
+def basic_migrate(cls: type, column_transfer: Dict[str, str]) -> None:
     """
     Given a class, compare its previous table,
     delete the fields that no longer exist,
     create new columns for new fields. If the
     column_flow parameter is given, migrate elements
     from previous column to the new ones. It should be
     noted that, the obj_ids do not persist.
 
     :param cls: Datalite class to migrate.
     :param column_transfer: A dictionary showing which
         columns will be copied to new ones.
     :return: None.
     """
     database_name, table_name = _get_db_table(cls)
-    table_column_names: Tuple[str] = _get_table_column_names(database_name, table_name)
+    table_column_names: Tuple[str, ...] = _get_table_column_names(database_name, table_name)
     values = dataclass_fields(cls).values()
-    data_fields: Tuple[Union[Field, CField], ...] = tuple(field for field in values)
-    data_field_names: Tuple[str] = tuple(field.name for field in data_fields)
-    columns_to_be_deleted: Tuple[str] = tuple(column for column in table_column_names if column not in data_field_names)
-    columns_to_be_added: Tuple[str] = tuple(column for column in data_field_names if column not in table_column_names)
+    data_fields: Tuple[Union[Field, CField], ...] = tuple(values)
+    data_field_names: Tuple[str, ...] = tuple(field.name for field in data_fields)
+    columns_to_be_deleted: Tuple[str, ...] = tuple(
+        column for column in table_column_names if column not in data_field_names
+    )
+    columns_to_be_added: Tuple[str, ...] = tuple(
+        column for column in data_field_names if column not in table_column_names
+    )
     records = _copy_records(database_name, table_name)
     _drop_table(database_name, table_name)
     _migrate_records(cls, database_name, records, columns_to_be_deleted, columns_to_be_added, column_transfer)
```

### Comparing `cornflakes-3.3.7/cornflakes/decorator/datalite/type_mapping.py` & `cornflakes-3.3.8/cornflakes/decorator/datalite/type_mapping.py`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/cornflakes/decorator/string_builder.py` & `cornflakes-3.3.8/cornflakes/decorator/string_builder.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,10 +39,8 @@
             return False
 
 
 def string_builder(callback=None, *args, **kwargs):
     def wrapper(c):
         return _StringMethodConcatenation(c, *args, **kwargs)
 
-    if callback:
-        return wrapper(callback)
-    return wrapper
+    return wrapper(callback) if callback else wrapper
```

### Comparing `cornflakes-3.3.7/cornflakes/logging/logger.py` & `cornflakes-3.3.8/cornflakes/logging/logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,39 +78,38 @@
         if isinstance(logging.root, logging.Logger):
             logging.root.setLevel(default_level or logging.root.level)
 
 
 class LoggerMetaClass(type):
     """LoggerMetaClass used for  metaclass."""
 
-    def __new__(mcs, classname, bases, class_dict):  # noqa: N804
+    def __new__(cls, classname, bases, class_dict):  # noqa: N804
         """Method __new__ for LoggerMetaClass."""
         new_class_dict = {}
         for attribute_name, attribute in class_dict.items():
             if isinstance(attribute, FunctionType):
                 # replace it with a wrapped version
                 attribute = attach_log(attribute)
             new_class_dict[attribute_name] = attribute
-        mcs.logger = logging.getLogger(classname)
-        return type.__new__(mcs, classname, bases, new_class_dict)
+        cls.logger = logging.getLogger(classname)
+        return type.__new__(cls, classname, bases, new_class_dict)
 
 
 class LoggerProtocol(Protocol):
     """LoggerProtocol used for Type Annotation."""
 
     logger: logging.Logger
 
 
 def __wrap_class(
     w_obj,
     log_level: Optional[int] = None,
 ):
     w_obj.logger = logging.getLogger(f"{w_obj.__module__}.{w_obj.__name__}")
     w_obj.logger.addHandler(logging.root.handlers[0])
-    w_obj.logger.__cornflakes__ = True
     w_obj.logger.setLevel(log_level or logging.root.level)
 
     if w_obj.logger.level == logging.DEBUG:
         for attribute_name, attribute in w_obj.__dict__.items():
             if isinstance(attribute, FunctionType):
                 # replace it with a wrapped version
                 attribute = attach_log(
@@ -123,15 +122,14 @@
 
 def __wrap_function(
     w_obj,
     log_level: Optional[int] = None,
 ):
     logger = logging.getLogger(f"{w_obj.__module__}.{w_obj.__qualname__}")
     logger.addHandler(logging.root.handlers[0])
-    logger.__cornflakes__ = True
     logger.setLevel(log_level or logging.root.level)
     if logger.level != logging.DEBUG:
         return w_obj
 
     @wraps(w_obj)
     def wrapper(*args, **kwargs):
         call_signature = ", ".join([repr(a) for a in args] + [f"{k}={v!r}" for k, v in kwargs.items()])
@@ -165,15 +163,10 @@
     if default_level:
         setup_logging(default_path, default_level, env_key, force=True)
 
     def obj_wrapper(w_obj) -> Union[LoggerProtocol, Callable[..., Any]]:
         if isclass(w_obj):
             return __wrap_class(w_obj, log_level)
 
-        if callable(w_obj):
-            return __wrap_function(w_obj, log_level)
+        return __wrap_function(w_obj, log_level) if callable(w_obj) else obj
 
-        return obj
-
-    if not obj:
-        return obj_wrapper
-    return obj_wrapper(obj)
+    return obj_wrapper(obj) if obj else obj_wrapper
```

### Comparing `cornflakes-3.3.7/cornflakes/packaging/bump_version.py` & `cornflakes-3.3.8/cornflakes/packaging/bump_version.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 #!/usr/bin/env python
 
 import os
+import pathlib
 import subprocess
 import sys
 
 from click import Choice
 from packaging import version
 
 from cornflakes.cli import cli
@@ -50,17 +51,15 @@
     new_version = version.Version(f"{major}.{minor}.{patch}")
 
     # Update the version in Python files
     for root, dirs, files in os.walk("."):
         for file in files:
             if file.endswith(".py"):
                 file_path = os.path.join(root, file)
-                with open(file_path) as f:
-                    content = f.read()
-
+                content = pathlib.Path(file_path).read_text()
                 # Check if the file contains the string "# <<FORCE_BUMP>>"
                 if "# <<FORCE_BUMP>>" in content:
                     # Increment the version number in the file
                     content = content.replace(parsed_version.public, str(new_version))
 
                     with open(file_path, "w") as f:
                         f.write(content)
```

### Comparing `cornflakes-3.3.7/cornflakes/parser/_yaml.py` & `cornflakes-3.3.8/cornflakes/parser/_yaml.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,30 +1,21 @@
-import collections.abc
 from os import environ
 from os.path import abspath, expanduser
 from typing import Any, Dict, List, Optional, Type, Union, cast
 
 import yaml
 from yaml import SafeLoader, UnsafeLoader
 
-
-def _update(d, u):
-    for k, v in u.items():
-        if isinstance(v, collections.abc.Mapping):
-            d[k] = _update(d.get(k, {}), v)
-        else:
-            d[k] = v
-    return d
+from cornflakes.common import recursive_update
 
 
 def _get_updated_key(config: Dict, values: List[str], defaults: Dict):
     result = None
     for value in values:
-        key = config.get(value, defaults.get(value, None))
-        if key:
+        if key := config.get(value, defaults.get(value)):
             result = key
     return result
 
 
 def _get_values(config, value: Union[str, List[str]], defaults: Dict):
     return (
         config
@@ -49,23 +40,23 @@
     keys: dict,
     defaults: dict,
 ) -> dict:
     new_config: dict = {}
     for section_key, section_names in sections.items():
         if not section_key:
             if isinstance(section_names, str):
-                _update(new_config, _get_section(config.get(section_names, {}), keys, defaults))
+                recursive_update(new_config, _get_section(config.get(section_names, {}), keys, defaults))
                 continue
             for section in section_names:
-                _update(new_config, _get_section(config.get(section, {}), keys, defaults))
+                recursive_update(new_config, _get_section(config.get(section, {}), keys, defaults))
         if isinstance(section_names, str):
-            _update(new_config, {section_key: _get_section(config.get(section_names, {}), keys, defaults)})
+            recursive_update(new_config, {section_key: _get_section(config.get(section_names, {}), keys, defaults)})
             continue
         for section in section_names:
-            _update(new_config, {section_key: _get_section(config.get(section, {}), keys, defaults)})
+            recursive_update(new_config, {section_key: _get_section(config.get(section, {}), keys, defaults)})
     return new_config
 
 
 def _yaml_read(
     file: str,
     sections: dict,
     keys: dict,
@@ -96,15 +87,15 @@
         or {}
     )  # dict
 
 
 def yaml_load(
     files: Union[str, List[str], Dict[Optional[str], Union[str, List[str]]]],
     sections: Optional[Union[str, List[str], Dict[Optional[str], Union[str, List[str]]]]] = None,
-    keys: Optional[Union[str, List[str], Dict[Optional[str], Union[str, List[str]]]]] = None,
+    keys: Optional[Union[str, List[str], Dict[str, Union[str, List[str]]]]] = None,
     defaults: Optional[Union[str, List[str], Dict[str, Any]]] = None,
     eval_env: bool = False,
     loader: Optional[Union[Type[SafeLoader], Type[UnsafeLoader]]] = None,
 ):
     """Yaml Wrapper for reading yaml files in a generic way."""
     files = _to_map(files)
     sections = _to_map(sections)
@@ -134,22 +125,22 @@
             }
         )
 
     config: dict = {}
     for file_key, file_names in files.items():
         if not file_key:
             if isinstance(file_names, str):
-                _update(config, _yaml_read(file_names, sections, keys, defaults, loader))
+                recursive_update(config, _yaml_read(file_names, sections, keys, defaults, loader))
                 return config
 
             for file in file_names:
-                _update(config, _yaml_read(file, sections, keys, defaults, loader))
+                recursive_update(config, _yaml_read(file, sections, keys, defaults, loader))
                 return config
 
         if isinstance(file_names, str):
-            _update(config, {file_key: _yaml_read(file_names, sections, keys, defaults, loader)})
+            recursive_update(config, {file_key: _yaml_read(file_names, sections, keys, defaults, loader)})
             return config
 
         for file in file_names:
-            _update(config, {file_key: _yaml_read(file, sections, keys, defaults, loader)})
+            recursive_update(config, {file_key: _yaml_read(file, sections, keys, defaults, loader)})
 
     return config
```

### Comparing `cornflakes-3.3.7/inst/_cornflakes/bindings.cpp` & `cornflakes-3.3.8/inst/_cornflakes/bindings.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/_cornflakes/cross_endian.h` & `cornflakes-3.3.8/inst/_cornflakes/cross_endian.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/_cornflakes/datetime_utils.hpp` & `cornflakes-3.3.8/inst/_cornflakes/datetime_utils.hpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/_cornflakes/digest.cpp` & `cornflakes-3.3.8/inst/_cornflakes/digest.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/_cornflakes/digest.hpp` & `cornflakes-3.3.8/inst/_cornflakes/digest.hpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/_cornflakes/ini.cpp` & `cornflakes-3.3.8/inst/_cornflakes/ini.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/_cornflakes/ini.hpp` & `cornflakes-3.3.8/inst/_cornflakes/ini.hpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/_cornflakes/string_operations.cpp` & `cornflakes-3.3.8/inst/_cornflakes/string_operations.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/_cornflakes/string_operations.hpp` & `cornflakes-3.3.8/inst/_cornflakes/string_operations.hpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/_cornflakes/system_operations.cpp` & `cornflakes-3.3.8/inst/_cornflakes/system_operations.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,15 @@
   if (value.at(0) == '.' && value.at(1) == '/') {
     value.erase(0, 2);
   }
   if (value.at(0) == '~') {
     char *home = std::getenv("HOME");
     if (home != NULL) {
       value.erase(0, 1);
-      value.insert(0, std::string(home) + "/");
+      value.insert(0, std::string(home));
     }
   }
   return value;
 }
 
 std::string read_file(const std::string &file) {
   try {
```

### Comparing `cornflakes-3.3.7/inst/_cornflakes/system_operations.hpp` & `cornflakes-3.3.8/inst/_cornflakes/system_operations.hpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/hash-library/LICENSE` & `cornflakes-3.3.8/inst/ext/hash-library/LICENSE`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/hash-library/crc32.cpp` & `cornflakes-3.3.8/inst/ext/hash-library/crc32.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/hash-library/crc32.h` & `cornflakes-3.3.8/inst/ext/hash-library/crc32.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/hash-library/digest.cpp` & `cornflakes-3.3.8/inst/ext/hash-library/digest.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/hash-library/hash.h` & `cornflakes-3.3.8/inst/ext/hash-library/hash.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/hash-library/hmac.h` & `cornflakes-3.3.8/inst/ext/hash-library/hmac.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/hash-library/keccak.cpp` & `cornflakes-3.3.8/inst/ext/hash-library/keccak.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/hash-library/keccak.h` & `cornflakes-3.3.8/inst/ext/hash-library/keccak.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/hash-library/md5.cpp` & `cornflakes-3.3.8/inst/ext/hash-library/md5.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/hash-library/md5.h` & `cornflakes-3.3.8/inst/ext/hash-library/md5.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/hash-library/readme.md` & `cornflakes-3.3.8/inst/ext/hash-library/readme.md`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/hash-library/sha1.cpp` & `cornflakes-3.3.8/inst/ext/hash-library/sha1.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/hash-library/sha1.h` & `cornflakes-3.3.8/inst/ext/hash-library/sha1.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/hash-library/sha256.cpp` & `cornflakes-3.3.8/inst/ext/hash-library/sha256.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/hash-library/sha256.h` & `cornflakes-3.3.8/inst/ext/hash-library/sha256.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/hash-library/sha3.cpp` & `cornflakes-3.3.8/inst/ext/hash-library/sha3.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/hash-library/sha3.h` & `cornflakes-3.3.8/inst/ext/hash-library/sha3.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/hash-library/tests/github-issue2.cpp` & `cornflakes-3.3.8/inst/ext/hash-library/tests/github-issue2.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/hash-library/tests/tests.cpp` & `cornflakes-3.3.8/inst/ext/hash-library/tests/tests.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/.appveyor.yml` & `cornflakes-3.3.8/inst/ext/pybind11/.appveyor.yml`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/.clang-format` & `cornflakes-3.3.8/inst/ext/pybind11/.clang-format`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/.clang-tidy` & `cornflakes-3.3.8/inst/ext/pybind11/.clang-tidy`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/.cmake-format.yaml` & `cornflakes-3.3.8/inst/ext/pybind11/.cmake-format.yaml`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/.codespell-ignore-lines` & `cornflakes-3.3.8/inst/ext/pybind11/.codespell-ignore-lines`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/.github/CONTRIBUTING.md` & `cornflakes-3.3.8/inst/ext/pybind11/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/.github/ISSUE_TEMPLATE/bug-report.yml` & `cornflakes-3.3.8/inst/ext/pybind11/.github/ISSUE_TEMPLATE/bug-report.yml`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/.github/matchers/pylint.json` & `cornflakes-3.3.8/inst/ext/pybind11/.github/matchers/pylint.json`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/.github/pull_request_template.md` & `cornflakes-3.3.8/inst/ext/pybind11/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/.github/workflows/ci.yml` & `cornflakes-3.3.8/inst/ext/pybind11/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/.github/workflows/configure.yml` & `cornflakes-3.3.8/inst/ext/pybind11/.github/workflows/configure.yml`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/.github/workflows/format.yml` & `cornflakes-3.3.8/inst/ext/pybind11/.github/workflows/format.yml`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/.github/workflows/labeler.yml` & `cornflakes-3.3.8/inst/ext/pybind11/.github/workflows/labeler.yml`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/.github/workflows/pip.yml` & `cornflakes-3.3.8/inst/ext/pybind11/.github/workflows/pip.yml`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/.github/workflows/upstream.yml` & `cornflakes-3.3.8/inst/ext/pybind11/.github/workflows/upstream.yml`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/.pre-commit-config.yaml` & `cornflakes-3.3.8/inst/ext/pybind11/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/CMakeLists.txt` & `cornflakes-3.3.8/inst/ext/pybind11/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/LICENSE` & `cornflakes-3.3.8/inst/ext/pybind11/LICENSE`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/README.rst` & `cornflakes-3.3.8/inst/ext/pybind11/README.rst`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/docs/Doxyfile` & `cornflakes-3.3.8/inst/ext/pybind11/docs/Doxyfile`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/docs/Makefile` & `cornflakes-3.3.8/inst/ext/pybind11/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/docs/advanced/cast/chrono.rst` & `cornflakes-3.3.8/inst/ext/pybind11/docs/advanced/cast/chrono.rst`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/docs/advanced/cast/custom.rst` & `cornflakes-3.3.8/inst/ext/pybind11/docs/advanced/cast/custom.rst`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/docs/advanced/cast/eigen.rst` & `cornflakes-3.3.8/inst/ext/pybind11/docs/advanced/cast/eigen.rst`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/docs/advanced/cast/functional.rst` & `cornflakes-3.3.8/inst/ext/pybind11/docs/advanced/cast/functional.rst`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/docs/advanced/cast/index.rst` & `cornflakes-3.3.8/inst/ext/pybind11/docs/advanced/cast/index.rst`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/docs/advanced/cast/overview.rst` & `cornflakes-3.3.8/inst/ext/pybind11/docs/advanced/cast/overview.rst`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/docs/advanced/cast/stl.rst` & `cornflakes-3.3.8/inst/ext/pybind11/docs/advanced/cast/stl.rst`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/docs/advanced/cast/strings.rst` & `cornflakes-3.3.8/inst/ext/pybind11/docs/advanced/cast/strings.rst`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/docs/advanced/classes.rst` & `cornflakes-3.3.8/inst/ext/pybind11/docs/advanced/classes.rst`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/docs/advanced/embedding.rst` & `cornflakes-3.3.8/inst/ext/pybind11/docs/advanced/embedding.rst`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/docs/advanced/exceptions.rst` & `cornflakes-3.3.8/inst/ext/pybind11/docs/advanced/exceptions.rst`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/docs/advanced/functions.rst` & `cornflakes-3.3.8/inst/ext/pybind11/docs/advanced/functions.rst`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/docs/advanced/misc.rst` & `cornflakes-3.3.8/inst/ext/pybind11/docs/advanced/misc.rst`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/docs/advanced/pycpp/numpy.rst` & `cornflakes-3.3.8/inst/ext/pybind11/docs/advanced/pycpp/numpy.rst`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/docs/advanced/pycpp/object.rst` & `cornflakes-3.3.8/inst/ext/pybind11/docs/advanced/pycpp/object.rst`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/docs/advanced/pycpp/utilities.rst` & `cornflakes-3.3.8/inst/ext/pybind11/docs/advanced/pycpp/utilities.rst`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/docs/advanced/smart_ptrs.rst` & `cornflakes-3.3.8/inst/ext/pybind11/docs/advanced/smart_ptrs.rst`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/docs/basics.rst` & `cornflakes-3.3.8/inst/ext/pybind11/docs/basics.rst`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/docs/benchmark.py` & `cornflakes-3.3.8/inst/ext/pybind11/docs/benchmark.py`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/docs/benchmark.rst` & `cornflakes-3.3.8/inst/ext/pybind11/docs/benchmark.rst`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/docs/changelog.rst` & `cornflakes-3.3.8/inst/ext/pybind11/docs/changelog.rst`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/docs/classes.rst` & `cornflakes-3.3.8/inst/ext/pybind11/docs/classes.rst`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/docs/compiling.rst` & `cornflakes-3.3.8/inst/ext/pybind11/docs/compiling.rst`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/docs/conf.py` & `cornflakes-3.3.8/inst/ext/pybind11/docs/conf.py`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/docs/faq.rst` & `cornflakes-3.3.8/inst/ext/pybind11/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/docs/index.rst` & `cornflakes-3.3.8/inst/ext/pybind11/docs/index.rst`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/docs/installing.rst` & `cornflakes-3.3.8/inst/ext/pybind11/docs/installing.rst`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/docs/limitations.rst` & `cornflakes-3.3.8/inst/ext/pybind11/docs/limitations.rst`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/docs/pybind11-logo.png` & `cornflakes-3.3.8/inst/ext/pybind11/docs/pybind11-logo.png`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/docs/pybind11_vs_boost_python1.png` & `cornflakes-3.3.8/inst/ext/pybind11/docs/pybind11_vs_boost_python1.png`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/docs/pybind11_vs_boost_python1.svg` & `cornflakes-3.3.8/inst/ext/pybind11/docs/pybind11_vs_boost_python1.svg`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/docs/pybind11_vs_boost_python2.png` & `cornflakes-3.3.8/inst/ext/pybind11/docs/pybind11_vs_boost_python2.png`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/docs/pybind11_vs_boost_python2.svg` & `cornflakes-3.3.8/inst/ext/pybind11/docs/pybind11_vs_boost_python2.svg`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/docs/reference.rst` & `cornflakes-3.3.8/inst/ext/pybind11/docs/reference.rst`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/docs/release.rst` & `cornflakes-3.3.8/inst/ext/pybind11/docs/release.rst`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/docs/upgrade.rst` & `cornflakes-3.3.8/inst/ext/pybind11/docs/upgrade.rst`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/include/pybind11/attr.h` & `cornflakes-3.3.8/inst/ext/pybind11/include/pybind11/attr.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/include/pybind11/buffer_info.h` & `cornflakes-3.3.8/inst/ext/pybind11/include/pybind11/buffer_info.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/include/pybind11/cast.h` & `cornflakes-3.3.8/inst/ext/pybind11/include/pybind11/cast.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/include/pybind11/chrono.h` & `cornflakes-3.3.8/inst/ext/pybind11/include/pybind11/chrono.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/include/pybind11/complex.h` & `cornflakes-3.3.8/inst/ext/pybind11/include/pybind11/complex.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/include/pybind11/detail/class.h` & `cornflakes-3.3.8/inst/ext/pybind11/include/pybind11/detail/class.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/include/pybind11/detail/common.h` & `cornflakes-3.3.8/inst/ext/pybind11/include/pybind11/detail/common.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/include/pybind11/detail/descr.h` & `cornflakes-3.3.8/inst/ext/pybind11/include/pybind11/detail/descr.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/include/pybind11/detail/init.h` & `cornflakes-3.3.8/inst/ext/pybind11/include/pybind11/detail/init.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/include/pybind11/detail/internals.h` & `cornflakes-3.3.8/inst/ext/pybind11/include/pybind11/detail/internals.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/include/pybind11/detail/type_caster_base.h` & `cornflakes-3.3.8/inst/ext/pybind11/include/pybind11/detail/type_caster_base.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/include/pybind11/detail/typeid.h` & `cornflakes-3.3.8/inst/ext/pybind11/include/pybind11/detail/typeid.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/include/pybind11/eigen/matrix.h` & `cornflakes-3.3.8/inst/ext/pybind11/include/pybind11/eigen/matrix.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/include/pybind11/eigen/tensor.h` & `cornflakes-3.3.8/inst/ext/pybind11/include/pybind11/eigen/tensor.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/include/pybind11/embed.h` & `cornflakes-3.3.8/inst/ext/pybind11/include/pybind11/embed.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/include/pybind11/eval.h` & `cornflakes-3.3.8/inst/ext/pybind11/include/pybind11/eval.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/include/pybind11/functional.h` & `cornflakes-3.3.8/inst/ext/pybind11/include/pybind11/functional.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/include/pybind11/gil.h` & `cornflakes-3.3.8/inst/ext/pybind11/include/pybind11/gil.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/include/pybind11/iostream.h` & `cornflakes-3.3.8/inst/ext/pybind11/include/pybind11/iostream.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/include/pybind11/numpy.h` & `cornflakes-3.3.8/inst/ext/pybind11/include/pybind11/numpy.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/include/pybind11/operators.h` & `cornflakes-3.3.8/inst/ext/pybind11/include/pybind11/operators.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/include/pybind11/options.h` & `cornflakes-3.3.8/inst/ext/pybind11/include/pybind11/options.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/include/pybind11/pybind11.h` & `cornflakes-3.3.8/inst/ext/pybind11/include/pybind11/pybind11.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/include/pybind11/pytypes.h` & `cornflakes-3.3.8/inst/ext/pybind11/include/pybind11/pytypes.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/include/pybind11/stl/filesystem.h` & `cornflakes-3.3.8/inst/ext/pybind11/include/pybind11/stl/filesystem.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/include/pybind11/stl.h` & `cornflakes-3.3.8/inst/ext/pybind11/include/pybind11/stl.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/include/pybind11/stl_bind.h` & `cornflakes-3.3.8/inst/ext/pybind11/include/pybind11/stl_bind.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/noxfile.py` & `cornflakes-3.3.8/inst/ext/pybind11/noxfile.py`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/pybind11/__main__.py` & `cornflakes-3.3.8/inst/ext/pybind11/pybind11/__main__.py`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/pybind11/commands.py` & `cornflakes-3.3.8/inst/ext/pybind11/pybind11/commands.py`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/pybind11/setup_helpers.py` & `cornflakes-3.3.8/inst/ext/pybind11/pybind11/setup_helpers.py`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/pyproject.toml` & `cornflakes-3.3.8/inst/ext/pybind11/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/setup.cfg` & `cornflakes-3.3.8/inst/ext/pybind11/setup.cfg`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/setup.py` & `cornflakes-3.3.8/inst/ext/pybind11/setup.py`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/tests/CMakeLists.txt` & `cornflakes-3.3.8/inst/ext/pybind11/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/tests/conftest.py` & `cornflakes-3.3.8/inst/ext/pybind11/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/tests/constructor_stats.h` & `cornflakes-3.3.8/inst/ext/pybind11/tests/constructor_stats.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/tests/cross_module_gil_utils.cpp` & `cornflakes-3.3.8/inst/ext/pybind11/tests/cross_module_gil_utils.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/tests/cross_module_interleaved_error_already_set.cpp` & `cornflakes-3.3.8/inst/ext/pybind11/tests/cross_module_interleaved_error_already_set.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/tests/env.py` & `cornflakes-3.3.8/inst/ext/pybind11/tests/env.py`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/tests/extra_python_package/test_files.py` & `cornflakes-3.3.8/inst/ext/pybind11/tests/extra_python_package/test_files.py`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/tests/extra_setuptools/test_setuphelper.py` & `cornflakes-3.3.8/inst/ext/pybind11/tests/extra_setuptools/test_setuphelper.py`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/tests/local_bindings.h` & `cornflakes-3.3.8/inst/ext/pybind11/tests/local_bindings.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/tests/object.h` & `cornflakes-3.3.8/inst/ext/pybind11/tests/object.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/tests/pybind11_cross_module_tests.cpp` & `cornflakes-3.3.8/inst/ext/pybind11/tests/pybind11_cross_module_tests.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/tests/pybind11_tests.cpp` & `cornflakes-3.3.8/inst/ext/pybind11/tests/pybind11_tests.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/tests/pybind11_tests.h` & `cornflakes-3.3.8/inst/ext/pybind11/tests/pybind11_tests.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/tests/pytest.ini` & `cornflakes-3.3.8/inst/ext/pybind11/tests/pytest.ini`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/tests/requirements.txt` & `cornflakes-3.3.8/inst/ext/pybind11/tests/requirements.txt`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/tests/test_async.cpp` & `cornflakes-3.3.8/inst/ext/pybind11/tests/test_async.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/tests/test_async.py` & `cornflakes-3.3.8/inst/ext/pybind11/tests/test_async.py`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/tests/test_buffers.cpp` & `cornflakes-3.3.8/inst/ext/pybind11/tests/test_buffers.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/tests/test_buffers.py` & `cornflakes-3.3.8/inst/ext/pybind11/tests/test_buffers.py`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/tests/test_builtin_casters.cpp` & `cornflakes-3.3.8/inst/ext/pybind11/tests/test_builtin_casters.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/tests/test_builtin_casters.py` & `cornflakes-3.3.8/inst/ext/pybind11/tests/test_builtin_casters.py`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/tests/test_call_policies.cpp` & `cornflakes-3.3.8/inst/ext/pybind11/tests/test_call_policies.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/tests/test_call_policies.py` & `cornflakes-3.3.8/inst/ext/pybind11/tests/test_call_policies.py`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/tests/test_callbacks.cpp` & `cornflakes-3.3.8/inst/ext/pybind11/tests/test_callbacks.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/tests/test_callbacks.py` & `cornflakes-3.3.8/inst/ext/pybind11/tests/test_callbacks.py`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/tests/test_chrono.cpp` & `cornflakes-3.3.8/inst/ext/pybind11/tests/test_chrono.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/tests/test_chrono.py` & `cornflakes-3.3.8/inst/ext/pybind11/tests/test_chrono.py`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/tests/test_class.cpp` & `cornflakes-3.3.8/inst/ext/pybind11/tests/test_class.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/tests/test_class.py` & `cornflakes-3.3.8/inst/ext/pybind11/tests/test_class.py`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/tests/test_cmake_build/CMakeLists.txt` & `cornflakes-3.3.8/inst/ext/pybind11/tests/test_cmake_build/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/tests/test_cmake_build/embed.cpp` & `cornflakes-3.3.8/inst/ext/pybind11/tests/test_cmake_build/embed.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt` & `cornflakes-3.3.8/inst/ext/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt` & `cornflakes-3.3.8/inst/ext/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt` & `cornflakes-3.3.8/inst/ext/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt` & `cornflakes-3.3.8/inst/ext/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt` & `cornflakes-3.3.8/inst/ext/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt` & `cornflakes-3.3.8/inst/ext/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/tests/test_const_name.cpp` & `cornflakes-3.3.8/inst/ext/pybind11/tests/test_const_name.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/tests/test_const_name.py` & `cornflakes-3.3.8/inst/ext/pybind11/tests/test_const_name.py`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/tests/test_constants_and_functions.cpp` & `cornflakes-3.3.8/inst/ext/pybind11/tests/test_constants_and_functions.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/tests/test_constants_and_functions.py` & `cornflakes-3.3.8/inst/ext/pybind11/tests/test_constants_and_functions.py`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/tests/test_copy_move.cpp` & `cornflakes-3.3.8/inst/ext/pybind11/tests/test_copy_move.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/tests/test_copy_move.py` & `cornflakes-3.3.8/inst/ext/pybind11/tests/test_copy_move.py`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/tests/test_custom_type_casters.cpp` & `cornflakes-3.3.8/inst/ext/pybind11/tests/test_custom_type_casters.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/tests/test_custom_type_casters.py` & `cornflakes-3.3.8/inst/ext/pybind11/tests/test_custom_type_casters.py`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/tests/test_custom_type_setup.cpp` & `cornflakes-3.3.8/inst/ext/pybind11/tests/test_custom_type_setup.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/tests/test_custom_type_setup.py` & `cornflakes-3.3.8/inst/ext/pybind11/tests/test_custom_type_setup.py`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/tests/test_docstring_options.cpp` & `cornflakes-3.3.8/inst/ext/pybind11/tests/test_docstring_options.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/tests/test_docstring_options.py` & `cornflakes-3.3.8/inst/ext/pybind11/tests/test_docstring_options.py`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/tests/test_eigen_matrix.cpp` & `cornflakes-3.3.8/inst/ext/pybind11/tests/test_eigen_matrix.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/tests/test_eigen_matrix.py` & `cornflakes-3.3.8/inst/ext/pybind11/tests/test_eigen_matrix.py`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/tests/test_eigen_tensor.inl` & `cornflakes-3.3.8/inst/ext/pybind11/tests/test_eigen_tensor.inl`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/tests/test_eigen_tensor.py` & `cornflakes-3.3.8/inst/ext/pybind11/tests/test_eigen_tensor.py`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/tests/test_embed/CMakeLists.txt` & `cornflakes-3.3.8/inst/ext/pybind11/tests/test_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/tests/test_embed/catch.cpp` & `cornflakes-3.3.8/inst/ext/pybind11/tests/test_embed/catch.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/tests/test_embed/external_module.cpp` & `cornflakes-3.3.8/inst/ext/pybind11/tests/test_embed/external_module.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/tests/test_embed/test_interpreter.cpp` & `cornflakes-3.3.8/inst/ext/pybind11/tests/test_embed/test_interpreter.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/tests/test_enum.cpp` & `cornflakes-3.3.8/inst/ext/pybind11/tests/test_enum.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/tests/test_enum.py` & `cornflakes-3.3.8/inst/ext/pybind11/tests/test_enum.py`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/tests/test_eval.cpp` & `cornflakes-3.3.8/inst/ext/pybind11/tests/test_eval.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/tests/test_eval.py` & `cornflakes-3.3.8/inst/ext/pybind11/tests/test_eval.py`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/tests/test_exceptions.cpp` & `cornflakes-3.3.8/inst/ext/pybind11/tests/test_exceptions.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/tests/test_exceptions.py` & `cornflakes-3.3.8/inst/ext/pybind11/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/tests/test_factory_constructors.cpp` & `cornflakes-3.3.8/inst/ext/pybind11/tests/test_factory_constructors.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/tests/test_factory_constructors.py` & `cornflakes-3.3.8/inst/ext/pybind11/tests/test_factory_constructors.py`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/tests/test_gil_scoped.cpp` & `cornflakes-3.3.8/inst/ext/pybind11/tests/test_gil_scoped.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/tests/test_gil_scoped.py` & `cornflakes-3.3.8/inst/ext/pybind11/tests/test_gil_scoped.py`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/tests/test_iostream.cpp` & `cornflakes-3.3.8/inst/ext/pybind11/tests/test_iostream.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/tests/test_iostream.py` & `cornflakes-3.3.8/inst/ext/pybind11/tests/test_iostream.py`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/tests/test_kwargs_and_defaults.cpp` & `cornflakes-3.3.8/inst/ext/pybind11/tests/test_kwargs_and_defaults.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/tests/test_kwargs_and_defaults.py` & `cornflakes-3.3.8/inst/ext/pybind11/tests/test_kwargs_and_defaults.py`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/tests/test_local_bindings.cpp` & `cornflakes-3.3.8/inst/ext/pybind11/tests/test_local_bindings.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/tests/test_local_bindings.py` & `cornflakes-3.3.8/inst/ext/pybind11/tests/test_local_bindings.py`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/tests/test_methods_and_attributes.cpp` & `cornflakes-3.3.8/inst/ext/pybind11/tests/test_methods_and_attributes.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/tests/test_methods_and_attributes.py` & `cornflakes-3.3.8/inst/ext/pybind11/tests/test_methods_and_attributes.py`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/tests/test_modules.cpp` & `cornflakes-3.3.8/inst/ext/pybind11/tests/test_modules.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/tests/test_modules.py` & `cornflakes-3.3.8/inst/ext/pybind11/tests/test_modules.py`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/tests/test_multiple_inheritance.cpp` & `cornflakes-3.3.8/inst/ext/pybind11/tests/test_multiple_inheritance.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/tests/test_multiple_inheritance.py` & `cornflakes-3.3.8/inst/ext/pybind11/tests/test_multiple_inheritance.py`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/tests/test_numpy_array.cpp` & `cornflakes-3.3.8/inst/ext/pybind11/tests/test_numpy_array.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/tests/test_numpy_array.py` & `cornflakes-3.3.8/inst/ext/pybind11/tests/test_numpy_array.py`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/tests/test_numpy_dtypes.cpp` & `cornflakes-3.3.8/inst/ext/pybind11/tests/test_numpy_dtypes.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/tests/test_numpy_dtypes.py` & `cornflakes-3.3.8/inst/ext/pybind11/tests/test_numpy_dtypes.py`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/tests/test_numpy_vectorize.cpp` & `cornflakes-3.3.8/inst/ext/pybind11/tests/test_numpy_vectorize.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/tests/test_numpy_vectorize.py` & `cornflakes-3.3.8/inst/ext/pybind11/tests/test_numpy_vectorize.py`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/tests/test_opaque_types.cpp` & `cornflakes-3.3.8/inst/ext/pybind11/tests/test_opaque_types.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/tests/test_opaque_types.py` & `cornflakes-3.3.8/inst/ext/pybind11/tests/test_opaque_types.py`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/tests/test_operator_overloading.cpp` & `cornflakes-3.3.8/inst/ext/pybind11/tests/test_operator_overloading.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/tests/test_operator_overloading.py` & `cornflakes-3.3.8/inst/ext/pybind11/tests/test_operator_overloading.py`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/tests/test_pickling.cpp` & `cornflakes-3.3.8/inst/ext/pybind11/tests/test_pickling.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/tests/test_pickling.py` & `cornflakes-3.3.8/inst/ext/pybind11/tests/test_pickling.py`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/tests/test_pytypes.cpp` & `cornflakes-3.3.8/inst/ext/pybind11/tests/test_pytypes.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/tests/test_pytypes.py` & `cornflakes-3.3.8/inst/ext/pybind11/tests/test_pytypes.py`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/tests/test_sequences_and_iterators.cpp` & `cornflakes-3.3.8/inst/ext/pybind11/tests/test_sequences_and_iterators.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/tests/test_sequences_and_iterators.py` & `cornflakes-3.3.8/inst/ext/pybind11/tests/test_sequences_and_iterators.py`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/tests/test_smart_ptr.cpp` & `cornflakes-3.3.8/inst/ext/pybind11/tests/test_smart_ptr.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/tests/test_smart_ptr.py` & `cornflakes-3.3.8/inst/ext/pybind11/tests/test_smart_ptr.py`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/tests/test_stl.cpp` & `cornflakes-3.3.8/inst/ext/pybind11/tests/test_stl.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/tests/test_stl.py` & `cornflakes-3.3.8/inst/ext/pybind11/tests/test_stl.py`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/tests/test_stl_binders.cpp` & `cornflakes-3.3.8/inst/ext/pybind11/tests/test_stl_binders.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/tests/test_stl_binders.py` & `cornflakes-3.3.8/inst/ext/pybind11/tests/test_stl_binders.py`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/tests/test_tagbased_polymorphic.cpp` & `cornflakes-3.3.8/inst/ext/pybind11/tests/test_tagbased_polymorphic.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/tests/test_tagbased_polymorphic.py` & `cornflakes-3.3.8/inst/ext/pybind11/tests/test_tagbased_polymorphic.py`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/tests/test_thread.cpp` & `cornflakes-3.3.8/inst/ext/pybind11/tests/test_thread.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/tests/test_thread.py` & `cornflakes-3.3.8/inst/ext/pybind11/tests/test_thread.py`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/tests/test_union.cpp` & `cornflakes-3.3.8/inst/ext/pybind11/tests/test_union.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/tests/test_virtual_functions.cpp` & `cornflakes-3.3.8/inst/ext/pybind11/tests/test_virtual_functions.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/tests/test_virtual_functions.py` & `cornflakes-3.3.8/inst/ext/pybind11/tests/test_virtual_functions.py`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/tests/valgrind-numpy-scipy.supp` & `cornflakes-3.3.8/inst/ext/pybind11/tests/valgrind-numpy-scipy.supp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/tests/valgrind-python.supp` & `cornflakes-3.3.8/inst/ext/pybind11/tests/valgrind-python.supp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/tools/FindCatch.cmake` & `cornflakes-3.3.8/inst/ext/pybind11/tools/FindCatch.cmake`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/tools/FindEigen3.cmake` & `cornflakes-3.3.8/inst/ext/pybind11/tools/FindEigen3.cmake`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/tools/FindPythonLibsNew.cmake` & `cornflakes-3.3.8/inst/ext/pybind11/tools/FindPythonLibsNew.cmake`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/tools/JoinPaths.cmake` & `cornflakes-3.3.8/inst/ext/pybind11/tools/JoinPaths.cmake`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/tools/check-style.sh` & `cornflakes-3.3.8/inst/ext/pybind11/tools/check-style.sh`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/tools/cmake_uninstall.cmake.in` & `cornflakes-3.3.8/inst/ext/pybind11/tools/cmake_uninstall.cmake.in`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/tools/codespell_ignore_lines_from_errors.py` & `cornflakes-3.3.8/inst/ext/pybind11/tools/codespell_ignore_lines_from_errors.py`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/tools/libsize.py` & `cornflakes-3.3.8/inst/ext/pybind11/tools/libsize.py`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/tools/make_changelog.py` & `cornflakes-3.3.8/inst/ext/pybind11/tools/make_changelog.py`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/tools/pybind11Common.cmake` & `cornflakes-3.3.8/inst/ext/pybind11/tools/pybind11Common.cmake`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/tools/pybind11Config.cmake.in` & `cornflakes-3.3.8/inst/ext/pybind11/tools/pybind11Config.cmake.in`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/tools/pybind11NewTools.cmake` & `cornflakes-3.3.8/inst/ext/pybind11/tools/pybind11NewTools.cmake`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/tools/pybind11Tools.cmake` & `cornflakes-3.3.8/inst/ext/pybind11/tools/pybind11Tools.cmake`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/tools/setup_global.py.in` & `cornflakes-3.3.8/inst/ext/pybind11/tools/setup_global.py.in`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/pybind11/tools/setup_main.py.in` & `cornflakes-3.3.8/inst/ext/pybind11/tools/setup_main.py.in`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/.travis.yml` & `cornflakes-3.3.8/inst/ext/rapidjson/.travis.yml`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/CHANGELOG.md` & `cornflakes-3.3.8/inst/ext/rapidjson/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/CMakeLists.txt` & `cornflakes-3.3.8/inst/ext/rapidjson/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/CMakeModules/FindGTestSrc.cmake` & `cornflakes-3.3.8/inst/ext/rapidjson/CMakeModules/FindGTestSrc.cmake`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/RapidJSONConfig.cmake.in` & `cornflakes-3.3.8/inst/ext/rapidjson/RapidJSONConfig.cmake.in`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/appveyor.yml` & `cornflakes-3.3.8/inst/ext/rapidjson/appveyor.yml`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/bin/data/glossary.json` & `cornflakes-3.3.8/inst/ext/rapidjson/bin/data/glossary.json`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/bin/data/menu.json` & `cornflakes-3.3.8/inst/ext/rapidjson/bin/data/menu.json`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/bin/data/sample.json` & `cornflakes-3.3.8/inst/ext/rapidjson/bin/data/sample.json`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/bin/data/webapp.json` & `cornflakes-3.3.8/inst/ext/rapidjson/bin/data/webapp.json`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/bin/data/widget.json` & `cornflakes-3.3.8/inst/ext/rapidjson/bin/data/widget.json`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/bin/draft-04/schema` & `cornflakes-3.3.8/inst/ext/rapidjson/bin/draft-04/schema`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/bin/encodings/utf32be.json` & `cornflakes-3.3.8/inst/ext/rapidjson/bin/encodings/utf32be.json`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/bin/encodings/utf32bebom.json` & `cornflakes-3.3.8/inst/ext/rapidjson/bin/encodings/utf32bebom.json`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/bin/encodings/utf32le.json` & `cornflakes-3.3.8/inst/ext/rapidjson/bin/encodings/utf32le.json`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/bin/encodings/utf32lebom.json` & `cornflakes-3.3.8/inst/ext/rapidjson/bin/encodings/utf32lebom.json`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonchecker/pass1.json` & `cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonchecker/pass1.json`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonschema/LICENSE` & `cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonschema/LICENSE`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonschema/README.md` & `cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonschema/README.md`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonschema/bin/jsonschema_suite` & `cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonschema/bin/jsonschema_suite`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonschema/tests/draft3/additionalItems.json` & `cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonschema/tests/draft3/additionalItems.json`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonschema/tests/draft3/additionalProperties.json` & `cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonschema/tests/draft3/additionalProperties.json`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonschema/tests/draft3/default.json` & `cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonschema/tests/draft3/default.json`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonschema/tests/draft3/dependencies.json` & `cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonschema/tests/draft3/dependencies.json`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonschema/tests/draft3/disallow.json` & `cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonschema/tests/draft3/disallow.json`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonschema/tests/draft3/divisibleBy.json` & `cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonschema/tests/draft3/divisibleBy.json`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonschema/tests/draft3/enum.json` & `cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonschema/tests/draft3/enum.json`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonschema/tests/draft3/extends.json` & `cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonschema/tests/draft3/extends.json`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonschema/tests/draft3/items.json` & `cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonschema/tests/draft3/items.json`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonschema/tests/draft3/maxItems.json` & `cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonschema/tests/draft3/maxItems.json`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonschema/tests/draft3/maxLength.json` & `cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonschema/tests/draft3/maxLength.json`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonschema/tests/draft3/maximum.json` & `cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonschema/tests/draft3/maximum.json`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonschema/tests/draft3/minItems.json` & `cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonschema/tests/draft3/minItems.json`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonschema/tests/draft3/minLength.json` & `cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonschema/tests/draft3/minLength.json`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonschema/tests/draft3/minimum.json` & `cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonschema/tests/draft3/minimum.json`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonschema/tests/draft3/optional/bignum.json` & `cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonschema/tests/draft3/optional/bignum.json`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonschema/tests/draft3/optional/format.json` & `cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonschema/tests/draft3/optional/format.json`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonschema/tests/draft3/pattern.json` & `cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonschema/tests/draft3/pattern.json`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonschema/tests/draft3/patternProperties.json` & `cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonschema/tests/draft3/patternProperties.json`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonschema/tests/draft3/properties.json` & `cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonschema/tests/draft3/properties.json`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonschema/tests/draft3/ref.json` & `cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonschema/tests/draft3/ref.json`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonschema/tests/draft3/refRemote.json` & `cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonschema/tests/draft3/refRemote.json`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonschema/tests/draft3/required.json` & `cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonschema/tests/draft3/required.json`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonschema/tests/draft3/type.json` & `cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonschema/tests/draft3/type.json`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonschema/tests/draft3/uniqueItems.json` & `cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonschema/tests/draft3/uniqueItems.json`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonschema/tests/draft4/additionalItems.json` & `cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonschema/tests/draft4/additionalItems.json`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonschema/tests/draft4/additionalProperties.json` & `cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonschema/tests/draft4/additionalProperties.json`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonschema/tests/draft4/allOf.json` & `cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonschema/tests/draft4/allOf.json`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonschema/tests/draft4/anyOf.json` & `cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonschema/tests/draft4/anyOf.json`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonschema/tests/draft4/default.json` & `cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonschema/tests/draft4/default.json`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonschema/tests/draft4/definitions.json` & `cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonschema/tests/draft4/definitions.json`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonschema/tests/draft4/dependencies.json` & `cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonschema/tests/draft4/dependencies.json`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonschema/tests/draft4/enum.json` & `cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonschema/tests/draft4/enum.json`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonschema/tests/draft4/items.json` & `cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonschema/tests/draft4/items.json`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonschema/tests/draft4/maxItems.json` & `cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonschema/tests/draft4/maxItems.json`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonschema/tests/draft4/maxLength.json` & `cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonschema/tests/draft4/maxLength.json`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonschema/tests/draft4/maxProperties.json` & `cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonschema/tests/draft4/maxProperties.json`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonschema/tests/draft4/maximum.json` & `cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonschema/tests/draft4/maximum.json`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonschema/tests/draft4/minItems.json` & `cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonschema/tests/draft4/minItems.json`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonschema/tests/draft4/minLength.json` & `cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonschema/tests/draft4/minLength.json`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonschema/tests/draft4/minProperties.json` & `cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonschema/tests/draft4/minProperties.json`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonschema/tests/draft4/minimum.json` & `cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonschema/tests/draft4/minimum.json`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonschema/tests/draft4/multipleOf.json` & `cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonschema/tests/draft4/multipleOf.json`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonschema/tests/draft4/not.json` & `cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonschema/tests/draft4/not.json`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonschema/tests/draft4/oneOf.json` & `cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonschema/tests/draft4/oneOf.json`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonschema/tests/draft4/optional/bignum.json` & `cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonschema/tests/draft4/optional/bignum.json`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonschema/tests/draft4/optional/format.json` & `cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonschema/tests/draft4/optional/format.json`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonschema/tests/draft4/pattern.json` & `cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonschema/tests/draft4/pattern.json`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonschema/tests/draft4/patternProperties.json` & `cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonschema/tests/draft4/patternProperties.json`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonschema/tests/draft4/properties.json` & `cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonschema/tests/draft4/properties.json`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonschema/tests/draft4/ref.json` & `cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonschema/tests/draft4/ref.json`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonschema/tests/draft4/refRemote.json` & `cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonschema/tests/draft4/refRemote.json`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonschema/tests/draft4/required.json` & `cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonschema/tests/draft4/required.json`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonschema/tests/draft4/type.json` & `cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonschema/tests/draft4/type.json`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/bin/jsonschema/tests/draft4/uniqueItems.json` & `cornflakes-3.3.8/inst/ext/rapidjson/bin/jsonschema/tests/draft4/uniqueItems.json`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/bin/types/alotofkeys.json` & `cornflakes-3.3.8/inst/ext/rapidjson/bin/types/alotofkeys.json`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/bin/types/floats.json` & `cornflakes-3.3.8/inst/ext/rapidjson/bin/types/floats.json`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/bin/types/guids.json` & `cornflakes-3.3.8/inst/ext/rapidjson/bin/types/guids.json`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/bin/types/integers.json` & `cornflakes-3.3.8/inst/ext/rapidjson/bin/types/integers.json`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/bin/types/mixed.json` & `cornflakes-3.3.8/inst/ext/rapidjson/bin/types/mixed.json`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/bin/types/paragraphs.json` & `cornflakes-3.3.8/inst/ext/rapidjson/bin/types/paragraphs.json`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/bin/unittestschema/address.json` & `cornflakes-3.3.8/inst/ext/rapidjson/bin/unittestschema/address.json`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/bin/unittestschema/idandref.json` & `cornflakes-3.3.8/inst/ext/rapidjson/bin/unittestschema/idandref.json`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/contrib/natvis/LICENSE` & `cornflakes-3.3.8/inst/ext/rapidjson/contrib/natvis/LICENSE`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/contrib/natvis/README.md` & `cornflakes-3.3.8/inst/ext/rapidjson/contrib/natvis/README.md`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/contrib/natvis/rapidjson.natvis` & `cornflakes-3.3.8/inst/ext/rapidjson/contrib/natvis/rapidjson.natvis`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/doc/CMakeLists.txt` & `cornflakes-3.3.8/inst/ext/rapidjson/doc/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/doc/Doxyfile.in` & `cornflakes-3.3.8/inst/ext/rapidjson/doc/Doxyfile.in`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/doc/Doxyfile.zh-cn.in` & `cornflakes-3.3.8/inst/ext/rapidjson/doc/Doxyfile.zh-cn.in`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/doc/diagram/architecture.dot` & `cornflakes-3.3.8/inst/ext/rapidjson/doc/diagram/architecture.dot`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/doc/diagram/architecture.png` & `cornflakes-3.3.8/inst/ext/rapidjson/doc/diagram/architecture.png`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/doc/diagram/insituparsing.dot` & `cornflakes-3.3.8/inst/ext/rapidjson/doc/diagram/insituparsing.dot`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/doc/diagram/insituparsing.png` & `cornflakes-3.3.8/inst/ext/rapidjson/doc/diagram/insituparsing.png`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/doc/diagram/iterative-parser-states-diagram.dot` & `cornflakes-3.3.8/inst/ext/rapidjson/doc/diagram/iterative-parser-states-diagram.dot`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/doc/diagram/iterative-parser-states-diagram.png` & `cornflakes-3.3.8/inst/ext/rapidjson/doc/diagram/iterative-parser-states-diagram.png`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/doc/diagram/move1.dot` & `cornflakes-3.3.8/inst/ext/rapidjson/doc/diagram/move1.dot`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/doc/diagram/move1.png` & `cornflakes-3.3.8/inst/ext/rapidjson/doc/diagram/move1.png`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/doc/diagram/move2.dot` & `cornflakes-3.3.8/inst/ext/rapidjson/doc/diagram/move2.dot`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/doc/diagram/move2.png` & `cornflakes-3.3.8/inst/ext/rapidjson/doc/diagram/move2.png`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/doc/diagram/move3.dot` & `cornflakes-3.3.8/inst/ext/rapidjson/doc/diagram/move3.dot`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/doc/diagram/move3.png` & `cornflakes-3.3.8/inst/ext/rapidjson/doc/diagram/move3.png`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/doc/diagram/normalparsing.dot` & `cornflakes-3.3.8/inst/ext/rapidjson/doc/diagram/normalparsing.dot`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/doc/diagram/normalparsing.png` & `cornflakes-3.3.8/inst/ext/rapidjson/doc/diagram/normalparsing.png`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/doc/diagram/simpledom.dot` & `cornflakes-3.3.8/inst/ext/rapidjson/doc/diagram/simpledom.dot`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/doc/diagram/simpledom.png` & `cornflakes-3.3.8/inst/ext/rapidjson/doc/diagram/simpledom.png`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/doc/diagram/tutorial.dot` & `cornflakes-3.3.8/inst/ext/rapidjson/doc/diagram/tutorial.dot`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/doc/diagram/tutorial.png` & `cornflakes-3.3.8/inst/ext/rapidjson/doc/diagram/tutorial.png`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/doc/diagram/utilityclass.dot` & `cornflakes-3.3.8/inst/ext/rapidjson/doc/diagram/utilityclass.dot`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/doc/diagram/utilityclass.png` & `cornflakes-3.3.8/inst/ext/rapidjson/doc/diagram/utilityclass.png`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/doc/dom.md` & `cornflakes-3.3.8/inst/ext/rapidjson/doc/dom.md`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/doc/dom.zh-cn.md` & `cornflakes-3.3.8/inst/ext/rapidjson/doc/dom.zh-cn.md`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/doc/encoding.md` & `cornflakes-3.3.8/inst/ext/rapidjson/doc/encoding.md`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/doc/encoding.zh-cn.md` & `cornflakes-3.3.8/inst/ext/rapidjson/doc/encoding.zh-cn.md`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/doc/faq.md` & `cornflakes-3.3.8/inst/ext/rapidjson/doc/faq.md`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/doc/faq.zh-cn.md` & `cornflakes-3.3.8/inst/ext/rapidjson/doc/faq.zh-cn.md`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/doc/features.md` & `cornflakes-3.3.8/inst/ext/rapidjson/doc/features.md`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/doc/features.zh-cn.md` & `cornflakes-3.3.8/inst/ext/rapidjson/doc/features.zh-cn.md`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/doc/internals.md` & `cornflakes-3.3.8/inst/ext/rapidjson/doc/internals.md`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/doc/internals.zh-cn.md` & `cornflakes-3.3.8/inst/ext/rapidjson/doc/internals.zh-cn.md`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/doc/logo/rapidjson.png` & `cornflakes-3.3.8/inst/ext/rapidjson/doc/logo/rapidjson.png`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/doc/logo/rapidjson.svg` & `cornflakes-3.3.8/inst/ext/rapidjson/doc/logo/rapidjson.svg`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/doc/misc/DoxygenLayout.xml` & `cornflakes-3.3.8/inst/ext/rapidjson/doc/misc/DoxygenLayout.xml`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/doc/misc/doxygenextra.css` & `cornflakes-3.3.8/inst/ext/rapidjson/doc/misc/doxygenextra.css`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/doc/misc/header.html` & `cornflakes-3.3.8/inst/ext/rapidjson/doc/misc/header.html`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/doc/performance.md` & `cornflakes-3.3.8/inst/ext/rapidjson/doc/performance.md`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/doc/performance.zh-cn.md` & `cornflakes-3.3.8/inst/ext/rapidjson/doc/performance.zh-cn.md`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/doc/pointer.md` & `cornflakes-3.3.8/inst/ext/rapidjson/doc/pointer.md`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/doc/pointer.zh-cn.md` & `cornflakes-3.3.8/inst/ext/rapidjson/doc/pointer.zh-cn.md`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/doc/sax.md` & `cornflakes-3.3.8/inst/ext/rapidjson/doc/sax.md`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/doc/sax.zh-cn.md` & `cornflakes-3.3.8/inst/ext/rapidjson/doc/sax.zh-cn.md`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/doc/schema.md` & `cornflakes-3.3.8/inst/ext/rapidjson/doc/schema.md`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/doc/schema.zh-cn.md` & `cornflakes-3.3.8/inst/ext/rapidjson/doc/schema.zh-cn.md`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/doc/stream.md` & `cornflakes-3.3.8/inst/ext/rapidjson/doc/stream.md`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/doc/stream.zh-cn.md` & `cornflakes-3.3.8/inst/ext/rapidjson/doc/stream.zh-cn.md`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/doc/tutorial.md` & `cornflakes-3.3.8/inst/ext/rapidjson/doc/tutorial.md`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/doc/tutorial.zh-cn.md` & `cornflakes-3.3.8/inst/ext/rapidjson/doc/tutorial.zh-cn.md`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/example/CMakeLists.txt` & `cornflakes-3.3.8/inst/ext/rapidjson/example/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/example/archiver/archiver.cpp` & `cornflakes-3.3.8/inst/ext/rapidjson/example/archiver/archiver.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/example/archiver/archiver.h` & `cornflakes-3.3.8/inst/ext/rapidjson/example/archiver/archiver.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/example/archiver/archivertest.cpp` & `cornflakes-3.3.8/inst/ext/rapidjson/example/archiver/archivertest.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/example/capitalize/capitalize.cpp` & `cornflakes-3.3.8/inst/ext/rapidjson/example/capitalize/capitalize.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/example/condense/condense.cpp` & `cornflakes-3.3.8/inst/ext/rapidjson/example/condense/condense.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/example/filterkey/filterkey.cpp` & `cornflakes-3.3.8/inst/ext/rapidjson/example/filterkey/filterkey.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/example/filterkeydom/filterkeydom.cpp` & `cornflakes-3.3.8/inst/ext/rapidjson/example/filterkeydom/filterkeydom.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/example/jsonx/jsonx.cpp` & `cornflakes-3.3.8/inst/ext/rapidjson/example/jsonx/jsonx.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/example/lookaheadparser/lookaheadparser.cpp` & `cornflakes-3.3.8/inst/ext/rapidjson/example/lookaheadparser/lookaheadparser.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/example/messagereader/messagereader.cpp` & `cornflakes-3.3.8/inst/ext/rapidjson/example/messagereader/messagereader.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/example/parsebyparts/parsebyparts.cpp` & `cornflakes-3.3.8/inst/ext/rapidjson/example/parsebyparts/parsebyparts.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/example/pretty/pretty.cpp` & `cornflakes-3.3.8/inst/ext/rapidjson/example/pretty/pretty.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/example/prettyauto/prettyauto.cpp` & `cornflakes-3.3.8/inst/ext/rapidjson/example/prettyauto/prettyauto.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/example/schemavalidator/schemavalidator.cpp` & `cornflakes-3.3.8/inst/ext/rapidjson/example/schemavalidator/schemavalidator.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/example/serialize/serialize.cpp` & `cornflakes-3.3.8/inst/ext/rapidjson/example/serialize/serialize.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/example/simpledom/simpledom.cpp` & `cornflakes-3.3.8/inst/ext/rapidjson/example/simpledom/simpledom.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/example/simplepullreader/simplepullreader.cpp` & `cornflakes-3.3.8/inst/ext/rapidjson/example/simplepullreader/simplepullreader.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/example/simplereader/simplereader.cpp` & `cornflakes-3.3.8/inst/ext/rapidjson/example/simplereader/simplereader.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/example/simplewriter/simplewriter.cpp` & `cornflakes-3.3.8/inst/ext/rapidjson/example/simplewriter/simplewriter.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/example/sortkeys/sortkeys.cpp` & `cornflakes-3.3.8/inst/ext/rapidjson/example/sortkeys/sortkeys.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/example/traverseaspointer.cpp` & `cornflakes-3.3.8/inst/ext/rapidjson/example/traverseaspointer.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/example/tutorial/tutorial.cpp` & `cornflakes-3.3.8/inst/ext/rapidjson/example/tutorial/tutorial.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/include/rapidjson/allocators.h` & `cornflakes-3.3.8/inst/ext/rapidjson/include/rapidjson/allocators.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/include/rapidjson/cursorstreamwrapper.h` & `cornflakes-3.3.8/inst/ext/rapidjson/include/rapidjson/cursorstreamwrapper.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/include/rapidjson/document.h` & `cornflakes-3.3.8/inst/ext/rapidjson/include/rapidjson/document.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/include/rapidjson/encodedstream.h` & `cornflakes-3.3.8/inst/ext/rapidjson/include/rapidjson/encodedstream.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/include/rapidjson/encodings.h` & `cornflakes-3.3.8/inst/ext/rapidjson/include/rapidjson/encodings.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/include/rapidjson/error/en.h` & `cornflakes-3.3.8/inst/ext/rapidjson/include/rapidjson/error/en.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/include/rapidjson/error/error.h` & `cornflakes-3.3.8/inst/ext/rapidjson/include/rapidjson/error/error.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/include/rapidjson/filereadstream.h` & `cornflakes-3.3.8/inst/ext/rapidjson/include/rapidjson/filereadstream.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/include/rapidjson/filewritestream.h` & `cornflakes-3.3.8/inst/ext/rapidjson/include/rapidjson/filewritestream.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/include/rapidjson/fwd.h` & `cornflakes-3.3.8/inst/ext/rapidjson/include/rapidjson/fwd.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/include/rapidjson/internal/biginteger.h` & `cornflakes-3.3.8/inst/ext/rapidjson/include/rapidjson/internal/biginteger.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/include/rapidjson/internal/clzll.h` & `cornflakes-3.3.8/inst/ext/rapidjson/include/rapidjson/internal/clzll.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/include/rapidjson/internal/diyfp.h` & `cornflakes-3.3.8/inst/ext/rapidjson/include/rapidjson/internal/diyfp.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/include/rapidjson/internal/dtoa.h` & `cornflakes-3.3.8/inst/ext/rapidjson/include/rapidjson/internal/dtoa.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/include/rapidjson/internal/ieee754.h` & `cornflakes-3.3.8/inst/ext/rapidjson/include/rapidjson/internal/ieee754.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/include/rapidjson/internal/itoa.h` & `cornflakes-3.3.8/inst/ext/rapidjson/include/rapidjson/internal/itoa.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/include/rapidjson/internal/meta.h` & `cornflakes-3.3.8/inst/ext/rapidjson/include/rapidjson/internal/meta.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/include/rapidjson/internal/pow10.h` & `cornflakes-3.3.8/inst/ext/rapidjson/include/rapidjson/internal/pow10.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/include/rapidjson/internal/regex.h` & `cornflakes-3.3.8/inst/ext/rapidjson/include/rapidjson/internal/regex.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/include/rapidjson/internal/stack.h` & `cornflakes-3.3.8/inst/ext/rapidjson/include/rapidjson/internal/stack.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/include/rapidjson/internal/strfunc.h` & `cornflakes-3.3.8/inst/ext/rapidjson/include/rapidjson/internal/strfunc.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/include/rapidjson/internal/strtod.h` & `cornflakes-3.3.8/inst/ext/rapidjson/include/rapidjson/internal/strtod.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/include/rapidjson/internal/swap.h` & `cornflakes-3.3.8/inst/ext/rapidjson/include/rapidjson/internal/swap.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/include/rapidjson/istreamwrapper.h` & `cornflakes-3.3.8/inst/ext/rapidjson/include/rapidjson/istreamwrapper.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/include/rapidjson/memorybuffer.h` & `cornflakes-3.3.8/inst/ext/rapidjson/include/rapidjson/memorybuffer.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/include/rapidjson/memorystream.h` & `cornflakes-3.3.8/inst/ext/rapidjson/include/rapidjson/memorystream.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/include/rapidjson/msinttypes/inttypes.h` & `cornflakes-3.3.8/inst/ext/rapidjson/include/rapidjson/msinttypes/inttypes.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/include/rapidjson/msinttypes/stdint.h` & `cornflakes-3.3.8/inst/ext/rapidjson/include/rapidjson/msinttypes/stdint.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/include/rapidjson/ostreamwrapper.h` & `cornflakes-3.3.8/inst/ext/rapidjson/include/rapidjson/ostreamwrapper.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/include/rapidjson/pointer.h` & `cornflakes-3.3.8/inst/ext/rapidjson/include/rapidjson/pointer.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/include/rapidjson/prettywriter.h` & `cornflakes-3.3.8/inst/ext/rapidjson/include/rapidjson/prettywriter.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/include/rapidjson/rapidjson.h` & `cornflakes-3.3.8/inst/ext/rapidjson/include/rapidjson/rapidjson.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/include/rapidjson/reader.h` & `cornflakes-3.3.8/inst/ext/rapidjson/include/rapidjson/reader.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/include/rapidjson/schema.h` & `cornflakes-3.3.8/inst/ext/rapidjson/include/rapidjson/schema.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/include/rapidjson/stream.h` & `cornflakes-3.3.8/inst/ext/rapidjson/include/rapidjson/stream.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/include/rapidjson/stringbuffer.h` & `cornflakes-3.3.8/inst/ext/rapidjson/include/rapidjson/stringbuffer.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/include/rapidjson/uri.h` & `cornflakes-3.3.8/inst/ext/rapidjson/include/rapidjson/uri.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/include/rapidjson/writer.h` & `cornflakes-3.3.8/inst/ext/rapidjson/include/rapidjson/writer.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/license.txt` & `cornflakes-3.3.8/inst/ext/rapidjson/license.txt`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/package.json` & `cornflakes-3.3.8/inst/ext/rapidjson/package.json`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/rapidjson.autopkg` & `cornflakes-3.3.8/inst/ext/rapidjson/rapidjson.autopkg`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/readme.md` & `cornflakes-3.3.8/inst/ext/rapidjson/readme.md`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/readme.zh-cn.md` & `cornflakes-3.3.8/inst/ext/rapidjson/readme.zh-cn.md`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/test/perftest/CMakeLists.txt` & `cornflakes-3.3.8/inst/ext/rapidjson/test/perftest/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/test/perftest/misctest.cpp` & `cornflakes-3.3.8/inst/ext/rapidjson/test/perftest/misctest.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/test/perftest/perftest.cpp` & `cornflakes-3.3.8/inst/ext/rapidjson/test/perftest/perftest.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/test/perftest/perftest.h` & `cornflakes-3.3.8/inst/ext/rapidjson/test/perftest/perftest.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/test/perftest/platformtest.cpp` & `cornflakes-3.3.8/inst/ext/rapidjson/test/perftest/platformtest.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/test/perftest/rapidjsontest.cpp` & `cornflakes-3.3.8/inst/ext/rapidjson/test/perftest/rapidjsontest.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/test/perftest/schematest.cpp` & `cornflakes-3.3.8/inst/ext/rapidjson/test/perftest/schematest.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/test/unittest/CMakeLists.txt` & `cornflakes-3.3.8/inst/ext/rapidjson/test/unittest/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/test/unittest/allocatorstest.cpp` & `cornflakes-3.3.8/inst/ext/rapidjson/test/unittest/allocatorstest.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/test/unittest/bigintegertest.cpp` & `cornflakes-3.3.8/inst/ext/rapidjson/test/unittest/bigintegertest.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/test/unittest/clzlltest.cpp` & `cornflakes-3.3.8/inst/ext/rapidjson/test/unittest/clzlltest.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/test/unittest/cursorstreamwrappertest.cpp` & `cornflakes-3.3.8/inst/ext/rapidjson/test/unittest/cursorstreamwrappertest.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/test/unittest/documenttest.cpp` & `cornflakes-3.3.8/inst/ext/rapidjson/test/unittest/documenttest.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/test/unittest/dtoatest.cpp` & `cornflakes-3.3.8/inst/ext/rapidjson/test/unittest/dtoatest.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/test/unittest/encodedstreamtest.cpp` & `cornflakes-3.3.8/inst/ext/rapidjson/test/unittest/encodedstreamtest.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/test/unittest/encodingstest.cpp` & `cornflakes-3.3.8/inst/ext/rapidjson/test/unittest/encodingstest.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/test/unittest/filestreamtest.cpp` & `cornflakes-3.3.8/inst/ext/rapidjson/test/unittest/filestreamtest.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/test/unittest/fwdtest.cpp` & `cornflakes-3.3.8/inst/ext/rapidjson/test/unittest/fwdtest.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/test/unittest/istreamwrappertest.cpp` & `cornflakes-3.3.8/inst/ext/rapidjson/test/unittest/istreamwrappertest.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/test/unittest/itoatest.cpp` & `cornflakes-3.3.8/inst/ext/rapidjson/test/unittest/itoatest.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/test/unittest/jsoncheckertest.cpp` & `cornflakes-3.3.8/inst/ext/rapidjson/test/unittest/jsoncheckertest.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/test/unittest/namespacetest.cpp` & `cornflakes-3.3.8/inst/ext/rapidjson/test/unittest/namespacetest.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/test/unittest/ostreamwrappertest.cpp` & `cornflakes-3.3.8/inst/ext/rapidjson/test/unittest/ostreamwrappertest.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/test/unittest/platformtest.cpp` & `cornflakes-3.3.8/inst/ext/rapidjson/test/unittest/platformtest.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/test/unittest/pointertest.cpp` & `cornflakes-3.3.8/inst/ext/rapidjson/test/unittest/pointertest.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/test/unittest/prettywritertest.cpp` & `cornflakes-3.3.8/inst/ext/rapidjson/test/unittest/prettywritertest.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/test/unittest/readertest.cpp` & `cornflakes-3.3.8/inst/ext/rapidjson/test/unittest/readertest.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/test/unittest/regextest.cpp` & `cornflakes-3.3.8/inst/ext/rapidjson/test/unittest/regextest.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/test/unittest/schematest.cpp` & `cornflakes-3.3.8/inst/ext/rapidjson/test/unittest/schematest.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/test/unittest/simdtest.cpp` & `cornflakes-3.3.8/inst/ext/rapidjson/test/unittest/simdtest.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/test/unittest/strfunctest.cpp` & `cornflakes-3.3.8/inst/ext/rapidjson/test/unittest/strfunctest.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/test/unittest/stringbuffertest.cpp` & `cornflakes-3.3.8/inst/ext/rapidjson/test/unittest/stringbuffertest.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/test/unittest/strtodtest.cpp` & `cornflakes-3.3.8/inst/ext/rapidjson/test/unittest/strtodtest.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/test/unittest/unittest.cpp` & `cornflakes-3.3.8/inst/ext/rapidjson/test/unittest/unittest.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/test/unittest/unittest.h` & `cornflakes-3.3.8/inst/ext/rapidjson/test/unittest/unittest.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/test/unittest/uritest.cpp` & `cornflakes-3.3.8/inst/ext/rapidjson/test/unittest/uritest.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/test/unittest/valuetest.cpp` & `cornflakes-3.3.8/inst/ext/rapidjson/test/unittest/valuetest.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/test/unittest/writertest.cpp` & `cornflakes-3.3.8/inst/ext/rapidjson/test/unittest/writertest.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/.gitignore` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/.gitignore`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/.travis.yml` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/.travis.yml`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/BUILD.bazel` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/BUILD.bazel`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/CMakeLists.txt` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/CONTRIBUTING.md` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/LICENSE` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/LICENSE`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/README.md` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/README.md`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/appveyor.yml` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/appveyor.yml`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/ci/build-linux-autotools.sh` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/ci/build-linux-autotools.sh`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/ci/build-linux-bazel.sh` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/ci/build-linux-bazel.sh`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/ci/env-linux.sh` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/ci/env-linux.sh`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/ci/env-osx.sh` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/ci/env-osx.sh`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/ci/get-nprocessors.sh` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/ci/get-nprocessors.sh`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/ci/install-linux.sh` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/ci/install-linux.sh`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/ci/install-osx.sh` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/ci/install-osx.sh`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/ci/log-config.sh` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/ci/log-config.sh`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/ci/travis.sh` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/ci/travis.sh`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/CHANGES` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/CHANGES`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/CMakeLists.txt` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/CONTRIBUTORS` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/CONTRIBUTORS`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/LICENSE` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/LICENSE`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/Makefile.am` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/Makefile.am`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/README.md` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/README.md`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/configure.ac` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/configure.ac`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/docs/CheatSheet.md` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/docs/CheatSheet.md`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/docs/CookBook.md` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/docs/CookBook.md`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/docs/DesignDoc.md` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/docs/DesignDoc.md`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/docs/Documentation.md` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/docs/Documentation.md`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/docs/ForDummies.md` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/docs/ForDummies.md`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/docs/FrequentlyAskedQuestions.md` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/docs/FrequentlyAskedQuestions.md`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/docs/KnownIssues.md` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/docs/KnownIssues.md`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/include/gmock/gmock-actions.h` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/include/gmock/gmock-actions.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/include/gmock/gmock-cardinalities.h` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/include/gmock/gmock-cardinalities.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/include/gmock/gmock-generated-actions.h` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/include/gmock/gmock-generated-actions.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/include/gmock/gmock-generated-actions.h.pump` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/include/gmock/gmock-generated-actions.h.pump`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/include/gmock/gmock-generated-function-mockers.h` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/include/gmock/gmock-generated-function-mockers.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/include/gmock/gmock-generated-function-mockers.h.pump` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/include/gmock/gmock-generated-function-mockers.h.pump`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/include/gmock/gmock-generated-matchers.h` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/include/gmock/gmock-generated-matchers.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/include/gmock/gmock-generated-matchers.h.pump` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/include/gmock/gmock-generated-matchers.h.pump`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/include/gmock/gmock-generated-nice-strict.h` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/include/gmock/gmock-generated-nice-strict.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/include/gmock/gmock-generated-nice-strict.h.pump` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/include/gmock/gmock-generated-nice-strict.h.pump`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/include/gmock/gmock-matchers.h` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/include/gmock/gmock-matchers.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/include/gmock/gmock-more-actions.h` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/include/gmock/gmock-more-actions.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/include/gmock/gmock-more-matchers.h` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/include/gmock/gmock-more-matchers.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/include/gmock/gmock-spec-builders.h` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/include/gmock/gmock-spec-builders.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/include/gmock/gmock.h` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/include/gmock/gmock.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/include/gmock/internal/custom/gmock-matchers.h` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/include/gmock/internal/custom/gmock-matchers.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/include/gmock/internal/custom/gmock-port.h` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/include/gmock/internal/custom/gmock-port.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/include/gmock/internal/gmock-generated-internal-utils.h` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/include/gmock/internal/gmock-generated-internal-utils.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/include/gmock/internal/gmock-generated-internal-utils.h.pump` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/include/gmock/internal/gmock-generated-internal-utils.h.pump`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/include/gmock/internal/gmock-internal-utils.h` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/include/gmock/internal/gmock-internal-utils.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/include/gmock/internal/gmock-port.h` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/include/gmock/internal/gmock-port.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/make/Makefile` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/make/Makefile`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/msvc/2005/gmock.sln` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/msvc/2005/gmock.sln`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/msvc/2005/gmock.vcproj` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/msvc/2005/gmock.vcproj`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/msvc/2005/gmock_main.vcproj` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/msvc/2005/gmock_main.vcproj`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/msvc/2005/gmock_test.vcproj` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/msvc/2005/gmock_test.vcproj`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/msvc/2010/gmock.sln` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/msvc/2010/gmock.sln`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/msvc/2010/gmock.vcxproj` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/msvc/2010/gmock.vcxproj`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/msvc/2010/gmock_config.props` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/msvc/2010/gmock_config.props`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/msvc/2010/gmock_main.vcxproj` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/msvc/2010/gmock_main.vcxproj`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/msvc/2010/gmock_test.vcxproj` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/msvc/2010/gmock_test.vcxproj`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/msvc/2015/gmock.sln` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/msvc/2015/gmock.sln`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/msvc/2015/gmock.vcxproj` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/msvc/2015/gmock.vcxproj`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/msvc/2015/gmock_config.props` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/msvc/2015/gmock_config.props`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/msvc/2015/gmock_main.vcxproj` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/msvc/2015/gmock_main.vcxproj`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/msvc/2015/gmock_test.vcxproj` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/msvc/2015/gmock_test.vcxproj`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/scripts/fuse_gmock_files.py` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/scripts/fuse_gmock_files.py`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/scripts/generator/LICENSE` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/scripts/generator/LICENSE`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/scripts/generator/README` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/scripts/generator/README`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/scripts/generator/README.cppclean` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/scripts/generator/README.cppclean`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/scripts/generator/cpp/ast.py` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/scripts/generator/cpp/ast.py`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/scripts/generator/cpp/gmock_class.py` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/scripts/generator/cpp/gmock_class.py`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/scripts/generator/cpp/gmock_class_test.py` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/scripts/generator/cpp/gmock_class_test.py`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/scripts/generator/cpp/keywords.py` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/scripts/generator/cpp/keywords.py`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/scripts/generator/cpp/tokenize.py` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/scripts/generator/cpp/tokenize.py`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/scripts/generator/cpp/utils.py` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/scripts/generator/cpp/utils.py`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/scripts/generator/gmock_gen.py` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/scripts/generator/gmock_gen.py`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/scripts/gmock-config.in` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/scripts/gmock-config.in`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/scripts/gmock_doctor.py` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/scripts/gmock_doctor.py`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/scripts/upload.py` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/scripts/upload.py`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/scripts/upload_gmock.py` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/scripts/upload_gmock.py`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/src/gmock-all.cc` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/src/gmock-all.cc`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/src/gmock-cardinalities.cc` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/src/gmock-cardinalities.cc`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/src/gmock-internal-utils.cc` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/src/gmock-internal-utils.cc`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/src/gmock-matchers.cc` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/src/gmock-matchers.cc`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/src/gmock-spec-builders.cc` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/src/gmock-spec-builders.cc`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/src/gmock.cc` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/src/gmock.cc`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/src/gmock_main.cc` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/src/gmock_main.cc`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/test/BUILD.bazel` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/test/BUILD.bazel`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/test/gmock-actions_test.cc` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/test/gmock-actions_test.cc`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/test/gmock-cardinalities_test.cc` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/test/gmock-cardinalities_test.cc`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/test/gmock-generated-actions_test.cc` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/test/gmock-generated-actions_test.cc`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/test/gmock-generated-function-mockers_test.cc` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/test/gmock-generated-function-mockers_test.cc`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/test/gmock-generated-internal-utils_test.cc` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/test/gmock-generated-internal-utils_test.cc`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/test/gmock-generated-matchers_test.cc` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/test/gmock-generated-matchers_test.cc`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/test/gmock-internal-utils_test.cc` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/test/gmock-internal-utils_test.cc`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/test/gmock-matchers_test.cc` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/test/gmock-matchers_test.cc`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/test/gmock-more-actions_test.cc` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/test/gmock-more-actions_test.cc`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/test/gmock-nice-strict_test.cc` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/test/gmock-nice-strict_test.cc`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/test/gmock-port_test.cc` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/test/gmock-port_test.cc`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/test/gmock-spec-builders_test.cc` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/test/gmock-spec-builders_test.cc`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/test/gmock_all_test.cc` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/test/gmock_all_test.cc`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/test/gmock_ex_test.cc` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/test/gmock_ex_test.cc`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/test/gmock_leak_test.py` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/test/gmock_leak_test.py`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/test/gmock_leak_test_.cc` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/test/gmock_leak_test_.cc`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/test/gmock_link2_test.cc` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/test/gmock_link2_test.cc`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/test/gmock_link_test.cc` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/test/gmock_link_test.cc`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/test/gmock_link_test.h` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/test/gmock_link_test.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/test/gmock_output_test.py` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/test/gmock_output_test.py`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/test/gmock_output_test_.cc` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/test/gmock_output_test_.cc`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/test/gmock_output_test_golden.txt` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/test/gmock_output_test_golden.txt`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/test/gmock_stress_test.cc` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/test/gmock_stress_test.cc`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/test/gmock_test.cc` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/test/gmock_test.cc`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googlemock/test/gmock_test_utils.py` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googlemock/test/gmock_test_utils.py`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/CHANGES` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/CHANGES`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/CMakeLists.txt` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/CONTRIBUTORS` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/CONTRIBUTORS`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/LICENSE` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/LICENSE`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/Makefile.am` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/Makefile.am`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/README.md` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/README.md`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/cmake/internal_utils.cmake` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/cmake/internal_utils.cmake`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/codegear/gtest.cbproj` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/codegear/gtest.cbproj`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/codegear/gtest.groupproj` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/codegear/gtest.groupproj`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/codegear/gtest_all.cc` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/codegear/gtest_all.cc`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/codegear/gtest_link.cc` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/codegear/gtest_link.cc`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/codegear/gtest_main.cbproj` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/codegear/gtest_main.cbproj`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/codegear/gtest_unittest.cbproj` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/codegear/gtest_unittest.cbproj`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/configure.ac` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/configure.ac`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/docs/Pkgconfig.md` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/docs/Pkgconfig.md`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/docs/PumpManual.md` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/docs/PumpManual.md`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/docs/XcodeGuide.md` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/docs/XcodeGuide.md`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/docs/advanced.md` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/docs/advanced.md`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/docs/faq.md` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/docs/faq.md`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/docs/primer.md` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/docs/primer.md`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/docs/samples.md` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/docs/samples.md`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/include/gtest/gtest-death-test.h` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/include/gtest/gtest-death-test.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/include/gtest/gtest-message.h` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/include/gtest/gtest-message.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/include/gtest/gtest-param-test.h` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/include/gtest/gtest-param-test.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/include/gtest/gtest-param-test.h.pump` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/include/gtest/gtest-param-test.h.pump`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/include/gtest/gtest-printers.h` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/include/gtest/gtest-printers.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/include/gtest/gtest-spi.h` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/include/gtest/gtest-spi.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/include/gtest/gtest-test-part.h` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/include/gtest/gtest-test-part.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/include/gtest/gtest-typed-test.h` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/include/gtest/gtest-typed-test.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/include/gtest/gtest.h` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/include/gtest/gtest.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/include/gtest/gtest_pred_impl.h` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/include/gtest/gtest_pred_impl.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/include/gtest/gtest_prod.h` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/include/gtest/gtest_prod.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/include/gtest/internal/custom/gtest-port.h` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/include/gtest/internal/custom/gtest-port.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/include/gtest/internal/custom/gtest-printers.h` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/include/gtest/internal/custom/gtest-printers.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/include/gtest/internal/custom/gtest.h` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/include/gtest/internal/custom/gtest.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/include/gtest/internal/gtest-death-test-internal.h` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/include/gtest/internal/gtest-death-test-internal.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/include/gtest/internal/gtest-filepath.h` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/include/gtest/internal/gtest-filepath.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/include/gtest/internal/gtest-internal.h` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/include/gtest/internal/gtest-internal.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/include/gtest/internal/gtest-linked_ptr.h` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/include/gtest/internal/gtest-linked_ptr.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/include/gtest/internal/gtest-param-util-generated.h` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/include/gtest/internal/gtest-param-util-generated.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/include/gtest/internal/gtest-param-util-generated.h.pump` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/include/gtest/internal/gtest-param-util-generated.h.pump`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/include/gtest/internal/gtest-param-util.h` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/include/gtest/internal/gtest-param-util.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/include/gtest/internal/gtest-port-arch.h` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/include/gtest/internal/gtest-port-arch.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/include/gtest/internal/gtest-port.h` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/include/gtest/internal/gtest-port.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/include/gtest/internal/gtest-string.h` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/include/gtest/internal/gtest-string.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/include/gtest/internal/gtest-tuple.h` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/include/gtest/internal/gtest-tuple.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/include/gtest/internal/gtest-tuple.h.pump` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/include/gtest/internal/gtest-tuple.h.pump`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/include/gtest/internal/gtest-type-util.h` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/include/gtest/internal/gtest-type-util.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/include/gtest/internal/gtest-type-util.h.pump` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/include/gtest/internal/gtest-type-util.h.pump`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/m4/acx_pthread.m4` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/m4/acx_pthread.m4`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/m4/gtest.m4` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/m4/gtest.m4`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/make/Makefile` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/make/Makefile`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/msvc/2010/gtest-md.sln` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/msvc/2010/gtest-md.sln`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/msvc/2010/gtest-md.vcxproj` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/msvc/2010/gtest-md.vcxproj`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/msvc/2010/gtest-md.vcxproj.filters` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/msvc/2010/gtest-md.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/msvc/2010/gtest.sln` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/msvc/2010/gtest.sln`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/msvc/2010/gtest.vcxproj` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/msvc/2010/gtest.vcxproj`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/msvc/2010/gtest.vcxproj.filters` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/msvc/2010/gtest.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/msvc/2010/gtest_main-md.vcxproj` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/msvc/2010/gtest_main-md.vcxproj`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/msvc/2010/gtest_main-md.vcxproj.filters` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/msvc/2010/gtest_main-md.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/msvc/2010/gtest_main.vcxproj` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/msvc/2010/gtest_main.vcxproj`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/msvc/2010/gtest_main.vcxproj.filters` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/msvc/2010/gtest_main.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/msvc/2010/gtest_prod_test-md.vcxproj` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/msvc/2010/gtest_prod_test-md.vcxproj`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/msvc/2010/gtest_prod_test-md.vcxproj.filters` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/msvc/2010/gtest_prod_test-md.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/msvc/2010/gtest_prod_test.vcxproj` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/msvc/2010/gtest_prod_test.vcxproj`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/msvc/2010/gtest_prod_test.vcxproj.filters` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/msvc/2010/gtest_prod_test.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/msvc/2010/gtest_unittest-md.vcxproj` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/msvc/2010/gtest_unittest-md.vcxproj`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/msvc/2010/gtest_unittest-md.vcxproj.filters` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/msvc/2010/gtest_unittest-md.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/msvc/2010/gtest_unittest.vcxproj` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/msvc/2010/gtest_unittest.vcxproj`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/msvc/2010/gtest_unittest.vcxproj.filters` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/msvc/2010/gtest_unittest.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/samples/prime_tables.h` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/samples/prime_tables.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/samples/sample1.cc` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/samples/sample1.cc`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/samples/sample1.h` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/samples/sample1.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/samples/sample10_unittest.cc` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/samples/sample10_unittest.cc`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/samples/sample1_unittest.cc` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/samples/sample1_unittest.cc`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/samples/sample2.cc` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/samples/sample2.cc`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/samples/sample2.h` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/samples/sample2.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/samples/sample2_unittest.cc` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/samples/sample2_unittest.cc`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/samples/sample3-inl.h` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/samples/sample3-inl.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/samples/sample3_unittest.cc` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/samples/sample3_unittest.cc`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/samples/sample4.cc` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/samples/sample4.cc`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/samples/sample4.h` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/samples/sample4.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/samples/sample4_unittest.cc` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/samples/sample4_unittest.cc`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/samples/sample5_unittest.cc` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/samples/sample5_unittest.cc`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/samples/sample6_unittest.cc` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/samples/sample6_unittest.cc`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/samples/sample7_unittest.cc` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/samples/sample7_unittest.cc`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/samples/sample8_unittest.cc` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/samples/sample8_unittest.cc`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/samples/sample9_unittest.cc` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/samples/sample9_unittest.cc`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/scripts/common.py` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/scripts/common.py`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/scripts/fuse_gtest_files.py` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/scripts/fuse_gtest_files.py`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/scripts/gen_gtest_pred_impl.py` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/scripts/gen_gtest_pred_impl.py`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/scripts/gtest-config.in` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/scripts/gtest-config.in`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/scripts/pump.py` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/scripts/pump.py`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/scripts/release_docs.py` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/scripts/release_docs.py`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/scripts/test/Makefile` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/scripts/test/Makefile`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/scripts/upload.py` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/scripts/upload.py`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/scripts/upload_gtest.py` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/scripts/upload_gtest.py`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/src/gtest-all.cc` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/src/gtest-all.cc`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/src/gtest-death-test.cc` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/src/gtest-death-test.cc`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/src/gtest-filepath.cc` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/src/gtest-filepath.cc`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/src/gtest-internal-inl.h` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/src/gtest-internal-inl.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/src/gtest-port.cc` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/src/gtest-port.cc`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/src/gtest-printers.cc` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/src/gtest-printers.cc`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/src/gtest-test-part.cc` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/src/gtest-test-part.cc`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/src/gtest-typed-test.cc` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/src/gtest-typed-test.cc`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/src/gtest.cc` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/src/gtest.cc`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/src/gtest_main.cc` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/src/gtest_main.cc`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/BUILD.bazel` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/BUILD.bazel`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest-death-test_ex_test.cc` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest-death-test_ex_test.cc`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest-death-test_test.cc` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest-death-test_test.cc`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest-filepath_test.cc` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest-filepath_test.cc`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest-linked_ptr_test.cc` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest-linked_ptr_test.cc`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest-listener_test.cc` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest-listener_test.cc`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest-message_test.cc` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest-message_test.cc`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest-options_test.cc` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest-options_test.cc`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest-param-test2_test.cc` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest-param-test2_test.cc`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest-param-test_test.cc` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest-param-test_test.cc`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest-param-test_test.h` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest-param-test_test.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest-port_test.cc` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest-port_test.cc`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest-printers_test.cc` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest-printers_test.cc`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest-test-part_test.cc` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest-test-part_test.cc`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest-tuple_test.cc` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest-tuple_test.cc`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest-typed-test2_test.cc` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest-typed-test2_test.cc`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest-typed-test_test.cc` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest-typed-test_test.cc`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest-typed-test_test.h` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest-typed-test_test.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest-unittest-api_test.cc` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest-unittest-api_test.cc`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_all_test.cc` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_all_test.cc`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_assert_by_exception_test.cc` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_assert_by_exception_test.cc`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_break_on_failure_unittest.py` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_break_on_failure_unittest.py`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_break_on_failure_unittest_.cc` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_break_on_failure_unittest_.cc`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_catch_exceptions_test.py` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_catch_exceptions_test.py`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_catch_exceptions_test_.cc` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_catch_exceptions_test_.cc`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_color_test.py` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_color_test.py`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_color_test_.cc` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_color_test_.cc`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_env_var_test.py` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_env_var_test.py`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_env_var_test_.cc` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_env_var_test_.cc`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_environment_test.cc` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_environment_test.cc`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_filter_unittest.py` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_filter_unittest.py`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_filter_unittest_.cc` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_filter_unittest_.cc`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_help_test.py` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_help_test.py`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_help_test_.cc` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_help_test_.cc`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_json_outfiles_test.py` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_json_outfiles_test.py`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_json_output_unittest.py` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_json_output_unittest.py`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_json_test_utils.py` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_json_test_utils.py`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_list_tests_unittest.py` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_list_tests_unittest.py`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_list_tests_unittest_.cc` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_list_tests_unittest_.cc`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_main_unittest.cc` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_main_unittest.cc`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_no_test_unittest.cc` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_no_test_unittest.cc`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_output_test.py` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_output_test.py`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_output_test_.cc` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_output_test_.cc`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_output_test_golden_lin.txt` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_output_test_golden_lin.txt`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_pred_impl_unittest.cc` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_pred_impl_unittest.cc`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_premature_exit_test.cc` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_premature_exit_test.cc`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_prod_test.cc` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_prod_test.cc`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_repeat_test.cc` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_repeat_test.cc`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_shuffle_test.py` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_shuffle_test.py`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_shuffle_test_.cc` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_shuffle_test_.cc`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_sole_header_test.cc` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_sole_header_test.cc`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_stress_test.cc` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_stress_test.cc`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_test_utils.py` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_test_utils.py`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_testbridge_test.py` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_testbridge_test.py`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_testbridge_test_.cc` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_testbridge_test_.cc`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_throw_on_failure_ex_test.cc` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_throw_on_failure_ex_test.cc`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_throw_on_failure_test.py` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_throw_on_failure_test.py`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_throw_on_failure_test_.cc` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_throw_on_failure_test_.cc`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_uninitialized_test.py` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_uninitialized_test.py`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_uninitialized_test_.cc` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_uninitialized_test_.cc`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_unittest.cc` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_unittest.cc`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_xml_outfile1_test_.cc` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_xml_outfile1_test_.cc`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_xml_outfile2_test_.cc` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_xml_outfile2_test_.cc`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_xml_outfiles_test.py` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_xml_outfiles_test.py`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_xml_output_unittest.py` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_xml_output_unittest.py`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_xml_output_unittest_.cc` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_xml_output_unittest_.cc`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_xml_test_utils.py` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/gtest_xml_test_utils.py`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/production.cc` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/production.cc`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/test/production.h` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/test/production.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/xcode/Config/DebugProject.xcconfig` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/xcode/Config/DebugProject.xcconfig`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/xcode/Config/FrameworkTarget.xcconfig` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/xcode/Config/FrameworkTarget.xcconfig`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/xcode/Config/General.xcconfig` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/xcode/Config/General.xcconfig`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/xcode/Config/ReleaseProject.xcconfig` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/xcode/Config/ReleaseProject.xcconfig`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/xcode/Config/StaticLibraryTarget.xcconfig` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/xcode/Config/StaticLibraryTarget.xcconfig`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/xcode/Resources/Info.plist` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/xcode/Resources/Info.plist`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/xcode/Samples/FrameworkSample/Info.plist` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/xcode/Samples/FrameworkSample/Info.plist`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/xcode/Samples/FrameworkSample/WidgetFramework.xcodeproj/project.pbxproj` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/xcode/Samples/FrameworkSample/WidgetFramework.xcodeproj/project.pbxproj`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/xcode/Samples/FrameworkSample/runtests.sh` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/xcode/Samples/FrameworkSample/runtests.sh`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/xcode/Samples/FrameworkSample/widget.cc` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/xcode/Samples/FrameworkSample/widget.cc`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/xcode/Samples/FrameworkSample/widget.h` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/xcode/Samples/FrameworkSample/widget.h`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/xcode/Samples/FrameworkSample/widget_test.cc` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/xcode/Samples/FrameworkSample/widget_test.cc`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/xcode/Scripts/runtests.sh` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/xcode/Scripts/runtests.sh`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/xcode/Scripts/versiongenerate.py` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/xcode/Scripts/versiongenerate.py`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/thirdparty/gtest/googletest/xcode/gtest.xcodeproj/project.pbxproj` & `cornflakes-3.3.8/inst/ext/rapidjson/thirdparty/gtest/googletest/xcode/gtest.xcodeproj/project.pbxproj`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/rapidjson/travis-doxygen.sh` & `cornflakes-3.3.8/inst/ext/rapidjson/travis-doxygen.sh`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/strtk/Makefile` & `cornflakes-3.3.8/inst/ext/strtk/Makefile`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/strtk/readme.txt` & `cornflakes-3.3.8/inst/ext/strtk/readme.txt`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/strtk/strtk.hpp` & `cornflakes-3.3.8/inst/ext/strtk/strtk.hpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/strtk/strtk_bloom_filter_example.cpp` & `cornflakes-3.3.8/inst/ext/strtk/strtk_bloom_filter_example.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/strtk/strtk_combinations.cpp` & `cornflakes-3.3.8/inst/ext/strtk/strtk_combinations.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/strtk/strtk_combinator_example.cpp` & `cornflakes-3.3.8/inst/ext/strtk/strtk_combinator_example.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/strtk/strtk_converters_example.cpp` & `cornflakes-3.3.8/inst/ext/strtk/strtk_converters_example.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/strtk/strtk_examples.cpp` & `cornflakes-3.3.8/inst/ext/strtk/strtk_examples.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/strtk/strtk_glober.cpp` & `cornflakes-3.3.8/inst/ext/strtk/strtk_glober.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/strtk/strtk_hexview.cpp` & `cornflakes-3.3.8/inst/ext/strtk/strtk_hexview.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/strtk/strtk_ipv4_parser.cpp` & `cornflakes-3.3.8/inst/ext/strtk/strtk_ipv4_parser.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/strtk/strtk_keyvalue_example.cpp` & `cornflakes-3.3.8/inst/ext/strtk/strtk_keyvalue_example.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/strtk/strtk_nth_combination_example.cpp` & `cornflakes-3.3.8/inst/ext/strtk/strtk_nth_combination_example.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/strtk/strtk_numstats.cpp` & `cornflakes-3.3.8/inst/ext/strtk/strtk_numstats.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/strtk/strtk_parse_test.cpp` & `cornflakes-3.3.8/inst/ext/strtk/strtk_parse_test.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/strtk/strtk_period_parser.cpp` & `cornflakes-3.3.8/inst/ext/strtk/strtk_period_parser.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/strtk/strtk_random_line.cpp` & `cornflakes-3.3.8/inst/ext/strtk/strtk_random_line.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/strtk/strtk_randomizer.cpp` & `cornflakes-3.3.8/inst/ext/strtk/strtk_randomizer.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/strtk/strtk_search_trie_example.cpp` & `cornflakes-3.3.8/inst/ext/strtk/strtk_search_trie_example.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/strtk/strtk_serializer_example.cpp` & `cornflakes-3.3.8/inst/ext/strtk/strtk_serializer_example.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/strtk/strtk_text_parser_example01.cpp` & `cornflakes-3.3.8/inst/ext/strtk/strtk_text_parser_example01.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/strtk/strtk_text_parser_example02.cpp` & `cornflakes-3.3.8/inst/ext/strtk/strtk_text_parser_example02.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/strtk/strtk_tokengrid_example.cpp` & `cornflakes-3.3.8/inst/ext/strtk/strtk_tokengrid_example.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/strtk/strtk_tokenizer_cmp.cpp` & `cornflakes-3.3.8/inst/ext/strtk/strtk_tokenizer_cmp.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/strtk/strtk_tokenizer_test.cpp` & `cornflakes-3.3.8/inst/ext/strtk/strtk_tokenizer_test.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/inst/ext/strtk/strtk_wordfreq.cpp` & `cornflakes-3.3.8/inst/ext/strtk/strtk_wordfreq.cpp`

 * *Files identical despite different names*

### Comparing `cornflakes-3.3.7/pyproject.toml` & `cornflakes-3.3.8/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cornflakes"
-version = "3.3.7"  # <<FORCE_BUMP>>
+version = "3.3.8"  # <<FORCE_BUMP>>
 description = "Create generic any easy way to manage Configs for your project"
 authors = ["Semjon Geist <semjon.geist@ionos.com>"]
 license = "Apache2.0"
 readme = "README.rst"
 homepage = "https://github.com/sgeist/cornflakes"
 repository = "https://github.com/sgeist/cornflakes"
 documentation = "https://cornflakes.readthedocs.io"
@@ -23,23 +23,23 @@
 ]
 exclude = [
     { path = "cornflakes/__pycache__" }
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
-PyYAML = "^5.4.1"
+PyYAML = "^6.0.1"
 toml = "^0.10.2"
 rich-rst = "^1.1.7"
 click = "^8.1.3"
-rich = ">=12.6,<14.0"
-types-pyyaml = "^6.0.12.10"
+rich = "13.4.2"
 validators = "^0.20.0"
+typing-extensions = "^4.7.1"
 
-[tool.poetry.group.dev.dependencies]
+[tool.poetry.dev-dependencies]
 autoflake = "^2.2.0"
 pytest = ">= 7.3.1"
 coverage = {extras = ["toml"], version = ">=5.3"}
 safety = ">=1.9.0"
 typeguard = ">=2.12.0"
 xdoctest = {extras = ["colors"], version = ">=0.15.0"}
 sphinx = ">=4.0.2"
@@ -75,19 +75,21 @@
 nox = "^2023.4.22"
 nox-poetry = "^1.0.2"
 compiledb = "^0.10.1"
 isort = "^5.12.0"
 virtualenv = "^20.23.1"
 pybind11 = "^2.10.4"
 pydantic = {extras = ["dotenv"], version = "^2.0"}
-markdown-it-py = "^2.2.0"
+markdown-it-py = ">=2.2,<4.0"
 clang-format = "^16.0.6"
 clang-tidy = "^15.0.2.1"
 cpplint = "^1.6.1"
 pydantic-settings = "^2.0.0"
+types-pyyaml = "^6.0.12.10"
+types-toml = "^0.10.8.6"
 
 
 [tool.poetry.scripts]
 cornflakes = "cornflakes.__main__:main"
 
 #[[tool.poetry.source]]
 #name = "cornflakes"
@@ -155,24 +157,27 @@
 [tool.poetry.build]
 script = "build.py"
 generate-setup-file = true
 
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
+    "pybind11",
+    "setuptools",
+    "packaging",
     "wheel",
     "ninja",
     "cmake>=3.12",
     "docutils",
-    "pybind11",
-    "setuptools"
 #    "fastentrypoints"
 ]
 #build-backend = "setuptools.build_meta"
 build-backend = "poetry.core.masonry.api"
+use-pep517 = true
+
 
 [tool.pytest.ini_options]
 pythonpath = ["src"]
 minversion = "6.0"
 addopts = ["-ra", "--showlocals", "--strict-markers", "--strict-config"]
 xfail_strict = true
 filterwarnings = ["error"]
```

### Comparing `cornflakes-3.3.7/setup.py` & `cornflakes-3.3.8/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,44 +4,45 @@
 packages = \
 ['cornflakes',
  'cornflakes.builder',
  'cornflakes.cli',
  'cornflakes.common',
  'cornflakes.decorator',
  'cornflakes.decorator.click',
+ 'cornflakes.decorator.click.helper',
  'cornflakes.decorator.click.options',
  'cornflakes.decorator.click.rich',
- 'cornflakes.decorator.config',
- 'cornflakes.decorator.dataclass',
- 'cornflakes.decorator.dataclass.validator',
+ 'cornflakes.decorator.dataclasses',
+ 'cornflakes.decorator.dataclasses.config',
+ 'cornflakes.decorator.dataclasses.validator',
  'cornflakes.decorator.datalite',
  'cornflakes.logging',
  'cornflakes.packaging',
  'cornflakes.parser']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['PyYAML>=5.4.1,<6.0.0',
+['PyYAML>=6.0.1,<7.0.0',
  'click>=8.1.3,<9.0.0',
  'rich-rst>=1.1.7,<2.0.0',
- 'rich>=12.6,<14.0',
+ 'rich==13.4.2',
  'toml>=0.10.2,<0.11.0',
- 'types-pyyaml>=6.0.12.10,<7.0.0.0',
+ 'typing-extensions>=4.7.1,<5.0.0',
  'validators>=0.20.0,<0.21.0']
 
 entry_points = \
 {'console_scripts': ['cornflakes = cornflakes.__main__:main']}
 
 setup_kwargs = {
     'name': 'cornflakes',
-    'version': '3.3.7',
+    'version': '3.3.8',
     'description': 'Create generic any easy way to manage Configs for your project',
-    'long_description': '.. image:: https://github.com/semmjon/cornflakes/blob/main/assets/cornflakes.png?raw=true\n   :height: 400 px\n   :width: 400 px\n   :alt: cornflakes logo\n   :align: center\n\n==========\n\n|PyPI| |Python Version| |License| |Read the Docs| |Build| |Tests| |Codecov|\n\n.. |PyPI| image:: https://img.shields.io/pypi/v/cornflakes.svg\n   :target: https://pypi.org/project/cornflakes/\n   :alt: PyPI\n.. |Python Version| image:: https://img.shields.io/pypi/pyversions/cornflakes\n   :target: https://pypi.org/project/cornflakes\n   :alt: Python Version\n.. |License| image:: https://img.shields.io/github/license/semmjon/cornflakes\n   :target: https://opensource.org/licenses/Apache2.0\n   :alt: License\n.. |Read the Docs| image:: https://img.shields.io/readthedocs/cornflakes/latest.svg?label=Read%20the%20Docs\n   :target: https://cornflakes.readthedocs.io\n   :alt: Read the documentation at https://cornflakes.readthedocs.io\n.. |Build| image:: https://github.com/semmjon/cornflakes/workflows/Build%20cornflakes%20Package/badge.svg\n   :target: https://github.com/semmjon/cornflakes/actions?workflow=Package\n   :alt: Build Package Status\n.. |Tests| image:: https://github.com/semmjon/cornflakes/workflows/Run%20cornflakes%20Tests/badge.svg\n   :target: https://github.com/semmjon/cornflakes/actions?workflow=Tests\n   :alt: Run Tests Status\n.. |Codecov| image:: https://codecov.io/gh/semmjon/cornflakes/branch/release-1.4.5/graph/badge.svg\n   :target: https://codecov.io/gh/semmjon/cornflakes\n   :alt: Codecov\n.. |Pre-Commit-CI| image:: https://results.pre-commit.ci/badge/github/sgeist-ionos/cornflakes/main.svg\n   :target: https://results.pre-commit.ci/latest/github/sgeist-ionos/cornflakes/main\n   :alt: pre-commit.ci status\n\n.. code::\n\n   pip install cornflakes\n\n.. code::\n\n    pip install git+https://github.com/semmjon/cornflakes\n\nInformation\n-----------\n\nThe Python module "cornflakes" was started as a hobby project and offers an alternative to Pydantic for managing configurations and data structures. It allows creating generic and easy to manage configurations for your project. Unlike Pydantic, which is based on inheritance, "cornflakes" uses a decorator (similar to dataclass) to map data structures.\n\nIn addition to a dataclass decorator with additional functionality, there is also a config decorator. This makes it possible to read the dataclass from configuration files. This can be very useful if you want to save your application configurations to a file.\n\nThe module also has a click wrapper that simplifies the implementation of command line applications. By integrating the Rich module, the application is additionally equipped with colors and other functions.\n\nThere are other useful methods in the base of the module that are generally useful for Python development. These can help you develop your projects faster and more efficiently.\n\nShort Term RoadMap:\n~~~~~~~~~~~~~~~~~~~~\n\n- Enrich json methods\n- Fix / Test the to_<file-format> Methods\n\nDevelopment\n-----------\n\nPrerequisites\n~~~~~~~~~~~~~\n\n-  A compiler with C++17 support\n-  Pip 10+ or CMake >= 3.4 (or 3.8+ on Windows, which was the first version to support VS 2015)\n-  Python 3.8+\n-  doxygen\n-  cppcheck\n-  clang-tools-extra or clang-tidy\n-  ..\n\nCommands\n~~~~~~~~~~~~\n\nJust clone this repository and pip install. Note the ``--recursive``\noption which is needed for the pybind11 submodule:\n\n.. code::\n\n   git clone --recursive https://gitlab.blubblub.tech/sgeist/cornflakes.git\n\nInstall the package using makefiles:\n\n.. code::\n\n   make install\n\nBuild dist using makefiles:\n\n.. code::\n\n   make dist\n\nRun tests (pytest) using makefiles:\n\n.. code::\n\n   make test\n\n\nRun all tests using makefiles:\n\n.. code::\n\n   make test-all\n\nRun lint using makefiles:\n\n.. code::\n\n   make lint\n\nCreate dev venv:\n\n.. code::\n\n   python -m venv .venv\n   source .venv/bin/activate\n   pip install ninja pre-commit poetry\n\nInstall pre-commit:\n\n.. code::\n\n   pre-commit install\n\nUpdate pre-commit:\n\n.. code::\n\n   pre-commit update -a\n\nRun pre-commit:\n\n.. code::\n\n   pre-commit run -a\n',
+    'long_description': '.. image:: https://github.com/semmjon/cornflakes/blob/main/assets/cornflakes.png?raw=true\n   :height: 400 px\n   :width: 400 px\n   :alt: cornflakes logo\n   :align: center\n\n==========\n\n|PyPI| |Python Version| |License| |Read the Docs| |Build| |Tests| |Codecov|\n\n.. |PyPI| image:: https://img.shields.io/pypi/v/cornflakes.svg\n   :target: https://pypi.org/project/cornflakes/\n   :alt: PyPI\n.. |Python Version| image:: https://img.shields.io/pypi/pyversions/cornflakes\n   :target: https://pypi.org/project/cornflakes\n   :alt: Python Version\n.. |License| image:: https://img.shields.io/github/license/semmjon/cornflakes\n   :target: https://opensource.org/licenses/Apache2.0\n   :alt: License\n.. |Read the Docs| image:: https://img.shields.io/readthedocs/cornflakes/latest.svg?label=Read%20the%20Docs\n   :target: https://cornflakes.readthedocs.io\n   :alt: Read the documentation at https://cornflakes.readthedocs.io\n.. |Build| image:: https://github.com/semmjon/cornflakes/workflows/Build%20cornflakes%20Package/badge.svg\n   :target: https://github.com/semmjon/cornflakes/actions?workflow=Package\n   :alt: Build Package Status\n.. |Tests| image:: https://github.com/semmjon/cornflakes/workflows/Run%20cornflakes%20Tests/badge.svg\n   :target: https://github.com/semmjon/cornflakes/actions?workflow=Tests\n   :alt: Run Tests Status\n.. |Codecov| image:: https://codecov.io/gh/semmjon/cornflakes/branch/release-1.4.5/graph/badge.svg\n   :target: https://codecov.io/gh/semmjon/cornflakes\n   :alt: Codecov\n.. |Pre-Commit-CI| image:: https://results.pre-commit.ci/badge/github/sgeist-ionos/cornflakes/main.svg\n   :target: https://results.pre-commit.ci/latest/github/sgeist-ionos/cornflakes/main\n   :alt: pre-commit.ci status\n\n.. code::\n\n   pip install cornflakes\n\n.. code::\n\n    pip install git+https://github.com/semmjon/cornflakes\n\n.. warning::\n    Please be careful when using this Python module. Currently it is only developed / tested by me, which is why it has a high update / change rate. I\'m actually trying to be compatible with implementations, but I can\'t guarantee this at the moment. The module is currently still in a beta state and is not recommended for productive use.\n\n    In the near future I plan to revise the documentation / examples and write an introductory blog article, as I find implemented features and planned ideas to be quite cool and useful (and don\'t see them in any other package or find them to be quite user-friendly).\n\nInformation\n-----------\n\nThe Python module "cornflakes" was started as a hobby project and offers an alternative to Pydantic for managing configurations and data structures. It allows creating generic and easy to manage configurations for your project. Unlike Pydantic, which is based on inheritance, "cornflakes" uses a decorator (similar to dataclass) to map data structures.\n\nIn addition to a dataclass decorator with additional functionality, there is also a config decorator. This makes it possible to read the dataclass from configuration files. This can be very useful if you want to save your application configurations to a file.\n\nThe module also has a click wrapper that simplifies the implementation of command line applications. By integrating the Rich module, the application is additionally equipped with colors and other functions.\n\nThere are other useful methods in the base of the module that are generally useful for Python development. These can help you develop your projects faster and more efficiently.\n\nShort Term RoadMap:\n~~~~~~~~~~~~~~~~~~~~\n\n- Change Code Annotations\n    - remove Any annotations if possible\n    - change Protocol Annotations to specific type classes\n- Enrich json methods\n- Fix / Test the to_<file-format> Methods (specially yaml)\n\nDevelopment\n-----------\n\nPrerequisites\n~~~~~~~~~~~~~\n\n-  A compiler with C++17 support\n-  Pip 10+ or CMake >= 3.4 (or 3.8+ on Windows, which was the first version to support VS 2015)\n-  Python 3.8+\n-  doxygen\n-  cppcheck\n-  clang-tools-extra or clang-tidy\n-  ..\n\nCommands\n~~~~~~~~~~~~\n\nJust clone this repository and pip install. Note the ``--recursive``\noption which is needed for the pybind11 submodule:\n\n.. code::\n\n   git clone --recursive https://gitlab.blubblub.tech/sgeist/cornflakes.git\n\nInstall the package using makefiles:\n\n.. code::\n\n   make install\n\nBuild dist using makefiles:\n\n.. code::\n\n   make dist\n\nRun tests (pytest) using makefiles:\n\n.. code::\n\n   make test\n\n\nRun all tests using makefiles:\n\n.. code::\n\n   make test-all\n\nRun lint using makefiles:\n\n.. code::\n\n   make lint\n\nCreate dev venv:\n\n.. code::\n\n   python -m venv .venv\n   source .venv/bin/activate\n   pip install ninja pre-commit poetry\n\nInstall pre-commit:\n\n.. code::\n\n   pre-commit install\n\nUpdate pre-commit:\n\n.. code::\n\n   pre-commit update -a\n\nRun pre-commit:\n\n.. code::\n\n   pre-commit run -a\n',
     'author': 'Semjon Geist',
     'author_email': 'semjon.geist@ionos.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/sgeist/cornflakes',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `cornflakes-3.3.7/PKG-INFO` & `cornflakes-3.3.8/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: cornflakes
-Version: 3.3.7
+Version: 3.3.8
 Summary: Create generic any easy way to manage Configs for your project
 Home-page: https://github.com/sgeist/cornflakes
 License: Apache2.0
 Author: Semjon Geist
 Author-email: semjon.geist@ionos.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
-Requires-Dist: PyYAML (>=5.4.1,<6.0.0)
+Requires-Dist: PyYAML (>=6.0.1,<7.0.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
-Requires-Dist: rich (>=12.6,<14.0)
+Requires-Dist: rich (==13.4.2)
 Requires-Dist: rich-rst (>=1.1.7,<2.0.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
-Requires-Dist: types-pyyaml (>=6.0.12.10,<7.0.0.0)
+Requires-Dist: typing-extensions (>=4.7.1,<5.0.0)
 Requires-Dist: validators (>=0.20.0,<0.21.0)
 Project-URL: Documentation, https://cornflakes.readthedocs.io
 Project-URL: Repository, https://github.com/sgeist/cornflakes
 Description-Content-Type: text/x-rst
 
 .. image:: https://github.com/semmjon/cornflakes/blob/main/assets/cornflakes.png?raw=true
    :height: 400 px
@@ -63,30 +63,38 @@
 
    pip install cornflakes
 
 .. code::
 
     pip install git+https://github.com/semmjon/cornflakes
 
+.. warning::
+    Please be careful when using this Python module. Currently it is only developed / tested by me, which is why it has a high update / change rate. I'm actually trying to be compatible with implementations, but I can't guarantee this at the moment. The module is currently still in a beta state and is not recommended for productive use.
+
+    In the near future I plan to revise the documentation / examples and write an introductory blog article, as I find implemented features and planned ideas to be quite cool and useful (and don't see them in any other package or find them to be quite user-friendly).
+
 Information
 -----------
 
 The Python module "cornflakes" was started as a hobby project and offers an alternative to Pydantic for managing configurations and data structures. It allows creating generic and easy to manage configurations for your project. Unlike Pydantic, which is based on inheritance, "cornflakes" uses a decorator (similar to dataclass) to map data structures.
 
 In addition to a dataclass decorator with additional functionality, there is also a config decorator. This makes it possible to read the dataclass from configuration files. This can be very useful if you want to save your application configurations to a file.
 
 The module also has a click wrapper that simplifies the implementation of command line applications. By integrating the Rich module, the application is additionally equipped with colors and other functions.
 
 There are other useful methods in the base of the module that are generally useful for Python development. These can help you develop your projects faster and more efficiently.
 
 Short Term RoadMap:
 ~~~~~~~~~~~~~~~~~~~~
 
+- Change Code Annotations
+    - remove Any annotations if possible
+    - change Protocol Annotations to specific type classes
 - Enrich json methods
-- Fix / Test the to_<file-format> Methods
+- Fix / Test the to_<file-format> Methods (specially yaml)
 
 Development
 -----------
 
 Prerequisites
 ~~~~~~~~~~~~~
```

