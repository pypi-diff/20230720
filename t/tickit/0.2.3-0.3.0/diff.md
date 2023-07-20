# Comparing `tmp/tickit-0.2.3.tar.gz` & `tmp/tickit-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tickit-0.2.3.tar", last modified: Fri Jul 14 10:47:06 2023, max compression
+gzip compressed data, was "tickit-0.3.0.tar", last modified: Thu Jul 20 14:54:59 2023, max compression
```

## Comparing `tickit-0.2.3.tar` & `tickit-0.3.0.tar`

### file list

```diff
@@ -1,258 +1,257 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:47:06.613619 tickit-0.2.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:47:06.557618 tickit-0.2.3/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-07-14 10:46:55.000000 tickit-0.2.3/.devcontainer/devcontainer.json
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-14 10:46:55.000000 tickit-0.2.3/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-14 10:46:55.000000 tickit-0.2.3/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:47:06.557618 tickit-0.2.3/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-07-14 10:46:55.000000 tickit-0.2.3/.github/CONTRIBUTING.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:47:06.533618 tickit-0.2.3/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:47:06.557618 tickit-0.2.3/.github/actions/install_requirements/
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-07-14 10:46:55.000000 tickit-0.2.3/.github/actions/install_requirements/action.yml
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-07-14 10:46:55.000000 tickit-0.2.3/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:47:06.561618 tickit-0.2.3/.github/pages/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-14 10:46:55.000000 tickit-0.2.3/.github/pages/index.html
--rwxr-xr-x   0 runner    (1001) docker     (123)     3023 2023-07-14 10:46:55.000000 tickit-0.2.3/.github/pages/make_switcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:47:06.561618 tickit-0.2.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     6583 2023-07-14 10:46:55.000000 tickit-0.2.3/.github/workflows/code.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-07-14 10:46:55.000000 tickit-0.2.3/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-07-14 10:46:55.000000 tickit-0.2.3/.github/workflows/docs_clean.yml
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-07-14 10:46:55.000000 tickit-0.2.3/.github/workflows/linkcheck.yml
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-07-14 10:46:55.000000 tickit-0.2.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-07-14 10:46:55.000000 tickit-0.2.3/.gitlab-ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-14 10:46:55.000000 tickit-0.2.3/.gitremotes
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-14 10:46:55.000000 tickit-0.2.3/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:47:06.565618 tickit-0.2.3/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-14 10:46:55.000000 tickit-0.2.3/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-07-14 10:46:55.000000 tickit-0.2.3/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-07-14 10:46:55.000000 tickit-0.2.3/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-14 10:46:55.000000 tickit-0.2.3/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-07-14 10:46:55.000000 tickit-0.2.3/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-14 10:46:55.000000 tickit-0.2.3/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-14 10:46:55.000000 tickit-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18626 2023-07-14 10:47:06.613619 tickit-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-07-14 10:46:55.000000 tickit-0.2.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-14 10:46:55.000000 tickit-0.2.3/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:47:06.565618 tickit-0.2.3/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:47:06.565618 tickit-0.2.3/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-14 10:46:55.000000 tickit-0.2.3/docs/_static/theme_overrides.css
--rw-r--r--   0 runner    (1001) docker     (123)     7037 2023-07-14 10:46:55.000000 tickit-0.2.3/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:47:06.565618 tickit-0.2.3/docs/developer/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:47:06.569619 tickit-0.2.3/docs/developer/explanations/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:47:06.569619 tickit-0.2.3/docs/developer/explanations/decisions/
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-07-14 10:46:55.000000 tickit-0.2.3/docs/developer/explanations/decisions/0001-record-architecture-decisions.rst
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-14 10:46:55.000000 tickit-0.2.3/docs/developer/explanations/decisions.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3696 2023-07-14 10:46:55.000000 tickit-0.2.3/docs/developer/explanations/framework-details.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-07-14 10:46:55.000000 tickit-0.2.3/docs/developer/explanations/how-component-updates-are-ordered.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-07-14 10:46:55.000000 tickit-0.2.3/docs/developer/explanations/why-tickit.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:47:06.573619 tickit-0.2.3/docs/developer/how-to/
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-07-14 10:46:55.000000 tickit-0.2.3/docs/developer/how-to/build-docs.rst
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-14 10:46:55.000000 tickit-0.2.3/docs/developer/how-to/contribute.rst
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-07-14 10:46:55.000000 tickit-0.2.3/docs/developer/how-to/lint.rst
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-14 10:46:55.000000 tickit-0.2.3/docs/developer/how-to/make-release.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-07-14 10:46:55.000000 tickit-0.2.3/docs/developer/how-to/pin-requirements.rst
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-14 10:46:55.000000 tickit-0.2.3/docs/developer/how-to/run-tests.rst
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-14 10:46:55.000000 tickit-0.2.3/docs/developer/how-to/static-analysis.rst
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-07-14 10:46:55.000000 tickit-0.2.3/docs/developer/how-to/test-container.rst
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-07-14 10:46:55.000000 tickit-0.2.3/docs/developer/how-to/update-tools.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-07-14 10:46:55.000000 tickit-0.2.3/docs/developer/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:47:06.573619 tickit-0.2.3/docs/developer/reference/
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-07-14 10:46:55.000000 tickit-0.2.3/docs/developer/reference/standards.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:47:06.573619 tickit-0.2.3/docs/developer/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-07-14 10:46:55.000000 tickit-0.2.3/docs/developer/tutorials/dev-install.rst
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-14 10:46:55.000000 tickit-0.2.3/docs/genindex.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:47:06.577618 tickit-0.2.3/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)     8272 2023-07-14 10:46:55.000000 tickit-0.2.3/docs/images/example-systems.drawio.svg
--rw-r--r--   0 runner    (1001) docker     (123)     5278 2023-07-14 10:46:55.000000 tickit-0.2.3/docs/images/tickit-create-device-amplifier.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-07-14 10:46:55.000000 tickit-0.2.3/docs/images/tickit-device-simulation-cpt.svg
--rw-r--r--   0 runner    (1001) docker     (123)   343434 2023-07-14 10:46:55.000000 tickit-0.2.3/docs/images/tickit-logo.ico
--rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-07-14 10:46:55.000000 tickit-0.2.3/docs/images/tickit-logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)    17845 2023-07-14 10:46:55.000000 tickit-0.2.3/docs/images/tickit-overview-full.svg
--rw-r--r--   0 runner    (1001) docker     (123)    12678 2023-07-14 10:46:55.000000 tickit-0.2.3/docs/images/tickit-simple-dag.svg
--rw-r--r--   0 runner    (1001) docker     (123)    11518 2023-07-14 10:46:55.000000 tickit-0.2.3/docs/images/tickit-simple-overview-with-system-simulation.svg
--rw-r--r--   0 runner    (1001) docker     (123)     9897 2023-07-14 10:46:55.000000 tickit-0.2.3/docs/images/tickit-simple-overview.svg
--rw-r--r--   0 runner    (1001) docker     (123)     5632 2023-07-14 10:46:55.000000 tickit-0.2.3/docs/images/tickit-simple-simulation.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7636 2023-07-14 10:46:55.000000 tickit-0.2.3/docs/images/tickit-system-simulation-cpt.svg
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-14 10:46:55.000000 tickit-0.2.3/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:47:06.577618 tickit-0.2.3/docs/user/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:47:06.585619 tickit-0.2.3/docs/user/explanations/
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-07-14 10:46:55.000000 tickit-0.2.3/docs/user/explanations/adapters.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-07-14 10:46:55.000000 tickit-0.2.3/docs/user/explanations/components.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-07-14 10:46:55.000000 tickit-0.2.3/docs/user/explanations/devices.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-07-14 10:46:55.000000 tickit-0.2.3/docs/user/explanations/framework-summary.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-07-14 10:46:55.000000 tickit-0.2.3/docs/user/explanations/glossary.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-07-14 10:46:55.000000 tickit-0.2.3/docs/user/explanations/wiring.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:47:06.585619 tickit-0.2.3/docs/user/how-to/
--rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-07-14 10:46:55.000000 tickit-0.2.3/docs/user/how-to/use-command-wrappers.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4837 2023-07-14 10:46:55.000000 tickit-0.2.3/docs/user/how-to/use-epics-adapter.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-07-14 10:46:55.000000 tickit-0.2.3/docs/user/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:47:06.585619 tickit-0.2.3/docs/user/reference/
--rw-r--r--   0 runner    (1001) docker     (123)     8651 2023-07-14 10:46:55.000000 tickit-0.2.3/docs/user/reference/api.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:47:06.585619 tickit-0.2.3/docs/user/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)     7128 2023-07-14 10:46:55.000000 tickit-0.2.3/docs/user/tutorials/create-a-device.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-07-14 10:46:55.000000 tickit-0.2.3/docs/user/tutorials/creating-a-simulation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-07-14 10:46:55.000000 tickit-0.2.3/docs/user/tutorials/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-07-14 10:46:55.000000 tickit-0.2.3/docs/user/tutorials/running-a-simulation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8332 2023-07-14 10:46:55.000000 tickit-0.2.3/docs/user/tutorials/use-composed-adapter.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:47:06.537618 tickit-0.2.3/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:47:06.589619 tickit-0.2.3/examples/configs/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-14 10:46:55.000000 tickit-0.2.3/examples/configs/amplifier.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-14 10:46:55.000000 tickit-0.2.3/examples/configs/counter.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-14 10:46:55.000000 tickit-0.2.3/examples/configs/http-and-zeromq-devices.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-14 10:46:55.000000 tickit-0.2.3/examples/configs/http-device.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-14 10:46:55.000000 tickit-0.2.3/examples/configs/isolated-device.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-14 10:46:55.000000 tickit-0.2.3/examples/configs/nested.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-14 10:46:55.000000 tickit-0.2.3/examples/configs/shutter.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-14 10:46:55.000000 tickit-0.2.3/examples/configs/sunk-tcp.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-14 10:46:55.000000 tickit-0.2.3/examples/configs/sunk-trampoline.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:47:06.593619 tickit-0.2.3/examples/devices/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 10:46:55.000000 tickit-0.2.3/examples/devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3860 2023-07-14 10:46:55.000000 tickit-0.2.3/examples/devices/amplifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-07-14 10:46:55.000000 tickit-0.2.3/examples/devices/counter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-07-14 10:46:55.000000 tickit-0.2.3/examples/devices/http_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     4709 2023-07-14 10:46:55.000000 tickit-0.2.3/examples/devices/isolated_device.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-14 10:46:55.000000 tickit-0.2.3/examples/devices/isolated_record.db
--rw-r--r--   0 runner    (1001) docker     (123)     8530 2023-07-14 10:46:55.000000 tickit-0.2.3/examples/devices/remote_controlled.py
--rw-r--r--   0 runner    (1001) docker     (123)     6850 2023-07-14 10:46:55.000000 tickit-0.2.3/examples/devices/shutter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4109 2023-07-14 10:46:55.000000 tickit-0.2.3/examples/devices/trampoline.py
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-07-14 10:46:55.000000 tickit-0.2.3/examples/devices/zeromq_push_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     3847 2023-07-14 10:46:55.000000 tickit-0.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 10:47:06.613619 tickit-0.2.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:47:06.541618 tickit-0.2.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:47:06.593619 tickit-0.2.3/src/tickit/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-14 10:46:55.000000 tickit-0.2.3/src/tickit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-14 10:46:55.000000 tickit-0.2.3/src/tickit/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-14 10:47:06.000000 tickit-0.2.3/src/tickit/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:47:06.597619 tickit-0.2.3/src/tickit/adapters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 10:46:55.000000 tickit-0.2.3/src/tickit/adapters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-07-14 10:46:55.000000 tickit-0.2.3/src/tickit/adapters/composed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:47:06.597619 tickit-0.2.3/src/tickit/adapters/epicsadapter/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-14 10:46:55.000000 tickit-0.2.3/src/tickit/adapters/epicsadapter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-07-14 10:46:55.000000 tickit-0.2.3/src/tickit/adapters/epicsadapter/adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-07-14 10:46:55.000000 tickit-0.2.3/src/tickit/adapters/epicsadapter/ioc_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-07-14 10:46:55.000000 tickit-0.2.3/src/tickit/adapters/httpadapter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:47:06.597619 tickit-0.2.3/src/tickit/adapters/interpreters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 10:46:55.000000 tickit-0.2.3/src/tickit/adapters/interpreters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:47:06.597619 tickit-0.2.3/src/tickit/adapters/interpreters/command/
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-14 10:46:55.000000 tickit-0.2.3/src/tickit/adapters/interpreters/command/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-07-14 10:46:55.000000 tickit-0.2.3/src/tickit/adapters/interpreters/command/command_interpreter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-07-14 10:46:55.000000 tickit-0.2.3/src/tickit/adapters/interpreters/command/regex_command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:47:06.597619 tickit-0.2.3/src/tickit/adapters/interpreters/endpoints/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 10:46:55.000000 tickit-0.2.3/src/tickit/adapters/interpreters/endpoints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-07-14 10:46:55.000000 tickit-0.2.3/src/tickit/adapters/interpreters/endpoints/http_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-14 10:46:55.000000 tickit-0.2.3/src/tickit/adapters/interpreters/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:47:06.597619 tickit-0.2.3/src/tickit/adapters/interpreters/wrappers/
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-14 10:46:55.000000 tickit-0.2.3/src/tickit/adapters/interpreters/wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-07-14 10:46:55.000000 tickit-0.2.3/src/tickit/adapters/interpreters/wrappers/beheading_interpreter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-07-14 10:46:55.000000 tickit-0.2.3/src/tickit/adapters/interpreters/wrappers/joining_interpreter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-07-14 10:46:55.000000 tickit-0.2.3/src/tickit/adapters/interpreters/wrappers/splitting_interpreter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:47:06.601619 tickit-0.2.3/src/tickit/adapters/servers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 10:46:55.000000 tickit-0.2.3/src/tickit/adapters/servers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-07-14 10:46:55.000000 tickit-0.2.3/src/tickit/adapters/servers/tcp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:47:06.601619 tickit-0.2.3/src/tickit/adapters/zeromq/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 10:46:55.000000 tickit-0.2.3/src/tickit/adapters/zeromq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-07-14 10:46:55.000000 tickit-0.2.3/src/tickit/adapters/zeromq/push_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-07-14 10:46:55.000000 tickit-0.2.3/src/tickit/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:47:06.601619 tickit-0.2.3/src/tickit/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 10:46:55.000000 tickit-0.2.3/src/tickit/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-07-14 10:46:55.000000 tickit-0.2.3/src/tickit/core/adapter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:47:06.601619 tickit-0.2.3/src/tickit/core/components/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 10:46:55.000000 tickit-0.2.3/src/tickit/core/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5872 2023-07-14 10:46:55.000000 tickit-0.2.3/src/tickit/core/components/component.py
--rw-r--r--   0 runner    (1001) docker     (123)     3417 2023-07-14 10:46:55.000000 tickit-0.2.3/src/tickit/core/components/device_simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4402 2023-07-14 10:46:55.000000 tickit-0.2.3/src/tickit/core/components/system_simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-07-14 10:46:55.000000 tickit-0.2.3/src/tickit/core/device.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:47:06.601619 tickit-0.2.3/src/tickit/core/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 10:46:55.000000 tickit-0.2.3/src/tickit/core/management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11048 2023-07-14 10:46:55.000000 tickit-0.2.3/src/tickit/core/management/event_router.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:47:06.605619 tickit-0.2.3/src/tickit/core/management/schedulers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 10:46:55.000000 tickit-0.2.3/src/tickit/core/management/schedulers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6514 2023-07-14 10:46:55.000000 tickit-0.2.3/src/tickit/core/management/schedulers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5803 2023-07-14 10:46:55.000000 tickit-0.2.3/src/tickit/core/management/schedulers/master.py
--rw-r--r--   0 runner    (1001) docker     (123)     7209 2023-07-14 10:46:55.000000 tickit-0.2.3/src/tickit/core/management/schedulers/slave.py
--rw-r--r--   0 runner    (1001) docker     (123)     6135 2023-07-14 10:46:55.000000 tickit-0.2.3/src/tickit/core/management/ticker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-07-14 10:46:55.000000 tickit-0.2.3/src/tickit/core/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:47:06.605619 tickit-0.2.3/src/tickit/core/state_interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-14 10:46:55.000000 tickit-0.2.3/src/tickit/core/state_interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6055 2023-07-14 10:46:55.000000 tickit-0.2.3/src/tickit/core/state_interfaces/internal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-07-14 10:46:55.000000 tickit-0.2.3/src/tickit/core/state_interfaces/kafka.py
--rw-r--r--   0 runner    (1001) docker     (123)     5905 2023-07-14 10:46:55.000000 tickit-0.2.3/src/tickit/core/state_interfaces/state_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-07-14 10:46:55.000000 tickit-0.2.3/src/tickit/core/typedefs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:47:06.605619 tickit-0.2.3/src/tickit/devices/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 10:46:55.000000 tickit-0.2.3/src/tickit/devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4016 2023-07-14 10:46:55.000000 tickit-0.2.3/src/tickit/devices/iobox.py
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-07-14 10:46:55.000000 tickit-0.2.3/src/tickit/devices/sink.py
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-07-14 10:46:55.000000 tickit-0.2.3/src/tickit/devices/source.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:47:06.605619 tickit-0.2.3/src/tickit/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 10:46:55.000000 tickit-0.2.3/src/tickit/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-14 10:46:55.000000 tickit-0.2.3/src/tickit/utils/byte_format.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:47:06.605619 tickit-0.2.3/src/tickit/utils/compat/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 10:46:55.000000 tickit-0.2.3/src/tickit/utils/compat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-07-14 10:46:55.000000 tickit-0.2.3/src/tickit/utils/compat/functools_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-14 10:46:55.000000 tickit-0.2.3/src/tickit/utils/compat/typing_compat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:47:06.605619 tickit-0.2.3/src/tickit/utils/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 10:46:55.000000 tickit-0.2.3/src/tickit/utils/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-07-14 10:46:55.000000 tickit-0.2.3/src/tickit/utils/configuration/configurable.py
--rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-07-14 10:46:55.000000 tickit-0.2.3/src/tickit/utils/configuration/loading.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-14 10:46:55.000000 tickit-0.2.3/src/tickit/utils/singleton.py
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-07-14 10:46:55.000000 tickit-0.2.3/src/tickit/utils/topic_naming.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:47:06.597619 tickit-0.2.3/src/tickit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18626 2023-07-14 10:47:06.000000 tickit-0.2.3/src/tickit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7180 2023-07-14 10:47:06.000000 tickit-0.2.3/src/tickit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 10:47:06.000000 tickit-0.2.3/src/tickit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-14 10:47:06.000000 tickit-0.2.3/src/tickit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-14 10:47:06.000000 tickit-0.2.3/src/tickit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-14 10:47:06.000000 tickit-0.2.3/src/tickit.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:47:06.605619 tickit-0.2.3/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:47:06.605619 tickit-0.2.3/tests/adapters/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:47:06.605619 tickit-0.2.3/tests/adapters/interpreters/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:47:06.609619 tickit-0.2.3/tests/adapters/interpreters/command/
--rw-r--r--   0 runner    (1001) docker     (123)     4766 2023-07-14 10:46:55.000000 tickit-0.2.3/tests/adapters/interpreters/command/test_command_interpreter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-07-14 10:46:55.000000 tickit-0.2.3/tests/adapters/interpreters/command/test_regex_command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:47:06.609619 tickit-0.2.3/tests/adapters/interpreters/endpoints/
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-07-14 10:46:55.000000 tickit-0.2.3/tests/adapters/interpreters/endpoints/test_http_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-14 10:46:55.000000 tickit-0.2.3/tests/adapters/interpreters/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:47:06.609619 tickit-0.2.3/tests/adapters/interpreters/wrappers/
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-14 10:46:55.000000 tickit-0.2.3/tests/adapters/interpreters/wrappers/test_beheading_interpreter.py
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-07-14 10:46:55.000000 tickit-0.2.3/tests/adapters/interpreters/wrappers/test_joining_interpreter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5992 2023-07-14 10:46:55.000000 tickit-0.2.3/tests/adapters/interpreters/wrappers/test_splitting_interpreter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:47:06.609619 tickit-0.2.3/tests/adapters/servers/
--rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-07-14 10:46:55.000000 tickit-0.2.3/tests/adapters/servers/test_tcp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:47:06.609619 tickit-0.2.3/tests/adapters/test_epicsadapter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 10:46:55.000000 tickit-0.2.3/tests/adapters/test_epicsadapter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4937 2023-07-14 10:46:55.000000 tickit-0.2.3/tests/adapters/test_epicsadapter/test_epics_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     9216 2023-07-14 10:46:55.000000 tickit-0.2.3/tests/adapters/test_httpadapter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:47:06.609619 tickit-0.2.3/tests/adapters/zeromq/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 10:46:55.000000 tickit-0.2.3/tests/adapters/zeromq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-07-14 10:46:55.000000 tickit-0.2.3/tests/adapters/zeromq/test_push_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-07-14 10:46:55.000000 tickit-0.2.3/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:47:06.609619 tickit-0.2.3/tests/core/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:47:06.609619 tickit-0.2.3/tests/core/components/
--rw-r--r--   0 runner    (1001) docker     (123)     4204 2023-07-14 10:46:55.000000 tickit-0.2.3/tests/core/components/test_component.py
--rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-07-14 10:46:55.000000 tickit-0.2.3/tests/core/components/test_device_simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4833 2023-07-14 10:46:55.000000 tickit-0.2.3/tests/core/components/test_system_simulation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:47:06.609619 tickit-0.2.3/tests/core/management/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:47:06.609619 tickit-0.2.3/tests/core/management/schedulers/
--rw-r--r--   0 runner    (1001) docker     (123)     3774 2023-07-14 10:46:55.000000 tickit-0.2.3/tests/core/management/schedulers/test_base_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6419 2023-07-14 10:46:55.000000 tickit-0.2.3/tests/core/management/schedulers/test_master_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6405 2023-07-14 10:46:55.000000 tickit-0.2.3/tests/core/management/schedulers/test_slave_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)    18354 2023-07-14 10:46:55.000000 tickit-0.2.3/tests/core/management/test_event_router.py
--rw-r--r--   0 runner    (1001) docker     (123)     6239 2023-07-14 10:46:55.000000 tickit-0.2.3/tests/core/management/test_ticker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:47:06.613619 tickit-0.2.3/tests/core/state_interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)     4109 2023-07-14 10:46:55.000000 tickit-0.2.3/tests/core/state_interfaces/test_internal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-07-14 10:46:55.000000 tickit-0.2.3/tests/core/state_interfaces/test_kafka.py
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-14 10:46:55.000000 tickit-0.2.3/tests/core/state_interfaces/test_state_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-07-14 10:46:55.000000 tickit-0.2.3/tests/core/test_device.py
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-14 10:46:55.000000 tickit-0.2.3/tests/core/test_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-07-14 10:46:55.000000 tickit-0.2.3/tests/core/test_typedefs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:47:06.613619 tickit-0.2.3/tests/devices/
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-07-14 10:46:55.000000 tickit-0.2.3/tests/devices/test_iobox.py
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-14 10:46:55.000000 tickit-0.2.3/tests/devices/test_sink.py
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-14 10:46:55.000000 tickit-0.2.3/tests/devices/test_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-07-14 10:46:55.000000 tickit-0.2.3/tests/test_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:47:06.613619 tickit-0.2.3/tests/utils/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:47:06.613619 tickit-0.2.3/tests/utils/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-07-14 10:46:55.000000 tickit-0.2.3/tests/utils/configuration/test_loading.py
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-07-14 10:46:55.000000 tickit-0.2.3/tests/utils/test_byte_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-07-14 10:46:55.000000 tickit-0.2.3/tests/utils/test_configurable.py
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-14 10:46:55.000000 tickit-0.2.3/tests/utils/test_singleton.py
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-14 10:46:55.000000 tickit-0.2.3/tests/utils/test_topic_naming.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:59.756579 tickit-0.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:59.724578 tickit-0.3.0/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-07-20 14:54:49.000000 tickit-0.3.0/.devcontainer/devcontainer.json
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-20 14:54:49.000000 tickit-0.3.0/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-20 14:54:49.000000 tickit-0.3.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:59.724578 tickit-0.3.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-07-20 14:54:49.000000 tickit-0.3.0/.github/CONTRIBUTING.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:59.716578 tickit-0.3.0/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:59.724578 tickit-0.3.0/.github/actions/install_requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-07-20 14:54:49.000000 tickit-0.3.0/.github/actions/install_requirements/action.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-07-20 14:54:49.000000 tickit-0.3.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:59.724578 tickit-0.3.0/.github/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-20 14:54:49.000000 tickit-0.3.0/.github/pages/index.html
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3023 2023-07-20 14:54:49.000000 tickit-0.3.0/.github/pages/make_switcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:59.724578 tickit-0.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     6403 2023-07-20 14:54:49.000000 tickit-0.3.0/.github/workflows/code.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-07-20 14:54:49.000000 tickit-0.3.0/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-07-20 14:54:49.000000 tickit-0.3.0/.github/workflows/docs_clean.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-07-20 14:54:49.000000 tickit-0.3.0/.github/workflows/linkcheck.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-07-20 14:54:49.000000 tickit-0.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-07-20 14:54:49.000000 tickit-0.3.0/.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-20 14:54:49.000000 tickit-0.3.0/.gitremotes
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-20 14:54:49.000000 tickit-0.3.0/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:59.724578 tickit-0.3.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-20 14:54:49.000000 tickit-0.3.0/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-07-20 14:54:49.000000 tickit-0.3.0/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-07-20 14:54:49.000000 tickit-0.3.0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-20 14:54:49.000000 tickit-0.3.0/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-07-20 14:54:49.000000 tickit-0.3.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-20 14:54:49.000000 tickit-0.3.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-20 14:54:49.000000 tickit-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18613 2023-07-20 14:54:59.756579 tickit-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5105 2023-07-20 14:54:49.000000 tickit-0.3.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-20 14:54:49.000000 tickit-0.3.0/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:59.724578 tickit-0.3.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:59.728578 tickit-0.3.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-20 14:54:49.000000 tickit-0.3.0/docs/_static/theme_overrides.css
+-rw-r--r--   0 runner    (1001) docker     (123)     7037 2023-07-20 14:54:49.000000 tickit-0.3.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:59.728578 tickit-0.3.0/docs/developer/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:59.728578 tickit-0.3.0/docs/developer/explanations/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:59.728578 tickit-0.3.0/docs/developer/explanations/decisions/
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-07-20 14:54:49.000000 tickit-0.3.0/docs/developer/explanations/decisions/0001-record-architecture-decisions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-20 14:54:49.000000 tickit-0.3.0/docs/developer/explanations/decisions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3696 2023-07-20 14:54:49.000000 tickit-0.3.0/docs/developer/explanations/framework-details.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-07-20 14:54:49.000000 tickit-0.3.0/docs/developer/explanations/how-component-updates-are-ordered.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-07-20 14:54:49.000000 tickit-0.3.0/docs/developer/explanations/why-tickit.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:59.728578 tickit-0.3.0/docs/developer/how-to/
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-07-20 14:54:49.000000 tickit-0.3.0/docs/developer/how-to/build-docs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-20 14:54:49.000000 tickit-0.3.0/docs/developer/how-to/contribute.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-07-20 14:54:49.000000 tickit-0.3.0/docs/developer/how-to/lint.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-20 14:54:49.000000 tickit-0.3.0/docs/developer/how-to/make-release.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-07-20 14:54:49.000000 tickit-0.3.0/docs/developer/how-to/pin-requirements.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-20 14:54:49.000000 tickit-0.3.0/docs/developer/how-to/run-tests.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-20 14:54:49.000000 tickit-0.3.0/docs/developer/how-to/static-analysis.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-07-20 14:54:49.000000 tickit-0.3.0/docs/developer/how-to/test-container.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-07-20 14:54:49.000000 tickit-0.3.0/docs/developer/how-to/update-tools.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-07-20 14:54:49.000000 tickit-0.3.0/docs/developer/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:59.728578 tickit-0.3.0/docs/developer/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-07-20 14:54:49.000000 tickit-0.3.0/docs/developer/reference/standards.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:59.728578 tickit-0.3.0/docs/developer/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-07-20 14:54:49.000000 tickit-0.3.0/docs/developer/tutorials/dev-install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-20 14:54:49.000000 tickit-0.3.0/docs/genindex.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:59.732578 tickit-0.3.0/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     8272 2023-07-20 14:54:49.000000 tickit-0.3.0/docs/images/example-systems.drawio.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5278 2023-07-20 14:54:49.000000 tickit-0.3.0/docs/images/tickit-create-device-amplifier.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-07-20 14:54:49.000000 tickit-0.3.0/docs/images/tickit-device-simulation-cpt.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   343434 2023-07-20 14:54:49.000000 tickit-0.3.0/docs/images/tickit-logo.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-07-20 14:54:49.000000 tickit-0.3.0/docs/images/tickit-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    17845 2023-07-20 14:54:49.000000 tickit-0.3.0/docs/images/tickit-overview-full.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    12678 2023-07-20 14:54:49.000000 tickit-0.3.0/docs/images/tickit-simple-dag.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    11518 2023-07-20 14:54:49.000000 tickit-0.3.0/docs/images/tickit-simple-overview-with-system-simulation.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     9897 2023-07-20 14:54:49.000000 tickit-0.3.0/docs/images/tickit-simple-overview.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5632 2023-07-20 14:54:49.000000 tickit-0.3.0/docs/images/tickit-simple-simulation.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7636 2023-07-20 14:54:49.000000 tickit-0.3.0/docs/images/tickit-system-simulation-cpt.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-20 14:54:49.000000 tickit-0.3.0/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:59.732578 tickit-0.3.0/docs/user/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:59.732578 tickit-0.3.0/docs/user/explanations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-07-20 14:54:49.000000 tickit-0.3.0/docs/user/explanations/adapters.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-07-20 14:54:49.000000 tickit-0.3.0/docs/user/explanations/components.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-07-20 14:54:49.000000 tickit-0.3.0/docs/user/explanations/devices.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-07-20 14:54:49.000000 tickit-0.3.0/docs/user/explanations/framework-summary.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-07-20 14:54:49.000000 tickit-0.3.0/docs/user/explanations/glossary.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-07-20 14:54:49.000000 tickit-0.3.0/docs/user/explanations/wiring.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:59.732578 tickit-0.3.0/docs/user/how-to/
+-rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-07-20 14:54:49.000000 tickit-0.3.0/docs/user/how-to/use-command-wrappers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4837 2023-07-20 14:54:49.000000 tickit-0.3.0/docs/user/how-to/use-epics-adapter.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-07-20 14:54:49.000000 tickit-0.3.0/docs/user/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:59.732578 tickit-0.3.0/docs/user/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)     8651 2023-07-20 14:54:49.000000 tickit-0.3.0/docs/user/reference/api.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:59.736578 tickit-0.3.0/docs/user/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)     7218 2023-07-20 14:54:49.000000 tickit-0.3.0/docs/user/tutorials/create-a-device.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-07-20 14:54:49.000000 tickit-0.3.0/docs/user/tutorials/creating-a-simulation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-07-20 14:54:49.000000 tickit-0.3.0/docs/user/tutorials/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-07-20 14:54:49.000000 tickit-0.3.0/docs/user/tutorials/running-a-simulation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8360 2023-07-20 14:54:49.000000 tickit-0.3.0/docs/user/tutorials/use-composed-adapter.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:59.716578 tickit-0.3.0/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:59.736578 tickit-0.3.0/examples/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-20 14:54:49.000000 tickit-0.3.0/examples/configs/amplifier.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-20 14:54:49.000000 tickit-0.3.0/examples/configs/counter.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-20 14:54:49.000000 tickit-0.3.0/examples/configs/http-and-zeromq-devices.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-20 14:54:49.000000 tickit-0.3.0/examples/configs/http-device.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-20 14:54:49.000000 tickit-0.3.0/examples/configs/isolated-device.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-20 14:54:49.000000 tickit-0.3.0/examples/configs/nested.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-20 14:54:49.000000 tickit-0.3.0/examples/configs/shutter.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-20 14:54:49.000000 tickit-0.3.0/examples/configs/sunk-tcp.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-20 14:54:49.000000 tickit-0.3.0/examples/configs/sunk-trampoline.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:59.736578 tickit-0.3.0/examples/devices/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:49.000000 tickit-0.3.0/examples/devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3880 2023-07-20 14:54:49.000000 tickit-0.3.0/examples/devices/amplifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-07-20 14:54:49.000000 tickit-0.3.0/examples/devices/counter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-07-20 14:54:49.000000 tickit-0.3.0/examples/devices/http_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4730 2023-07-20 14:54:49.000000 tickit-0.3.0/examples/devices/isolated_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-20 14:54:49.000000 tickit-0.3.0/examples/devices/isolated_record.db
+-rw-r--r--   0 runner    (1001) docker     (123)     8507 2023-07-20 14:54:49.000000 tickit-0.3.0/examples/devices/remote_controlled.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6827 2023-07-20 14:54:49.000000 tickit-0.3.0/examples/devices/shutter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4104 2023-07-20 14:54:49.000000 tickit-0.3.0/examples/devices/trampoline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-07-20 14:54:49.000000 tickit-0.3.0/examples/devices/zeromq_push_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3780 2023-07-20 14:54:49.000000 tickit-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 14:54:59.756579 tickit-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:59.716578 tickit-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:59.740579 tickit-0.3.0/src/tickit/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-20 14:54:49.000000 tickit-0.3.0/src/tickit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-20 14:54:49.000000 tickit-0.3.0/src/tickit/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-20 14:54:59.000000 tickit-0.3.0/src/tickit/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:59.740579 tickit-0.3.0/src/tickit/adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:49.000000 tickit-0.3.0/src/tickit/adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-07-20 14:54:49.000000 tickit-0.3.0/src/tickit/adapters/composed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:59.740579 tickit-0.3.0/src/tickit/adapters/epicsadapter/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-20 14:54:49.000000 tickit-0.3.0/src/tickit/adapters/epicsadapter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-07-20 14:54:49.000000 tickit-0.3.0/src/tickit/adapters/epicsadapter/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-07-20 14:54:49.000000 tickit-0.3.0/src/tickit/adapters/epicsadapter/ioc_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-07-20 14:54:49.000000 tickit-0.3.0/src/tickit/adapters/httpadapter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:59.740579 tickit-0.3.0/src/tickit/adapters/interpreters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:49.000000 tickit-0.3.0/src/tickit/adapters/interpreters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:59.740579 tickit-0.3.0/src/tickit/adapters/interpreters/command/
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-20 14:54:49.000000 tickit-0.3.0/src/tickit/adapters/interpreters/command/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3532 2023-07-20 14:54:49.000000 tickit-0.3.0/src/tickit/adapters/interpreters/command/command_interpreter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-07-20 14:54:49.000000 tickit-0.3.0/src/tickit/adapters/interpreters/command/regex_command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:59.740579 tickit-0.3.0/src/tickit/adapters/interpreters/endpoints/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:49.000000 tickit-0.3.0/src/tickit/adapters/interpreters/endpoints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-07-20 14:54:49.000000 tickit-0.3.0/src/tickit/adapters/interpreters/endpoints/http_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-20 14:54:49.000000 tickit-0.3.0/src/tickit/adapters/interpreters/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:59.744578 tickit-0.3.0/src/tickit/adapters/interpreters/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-20 14:54:49.000000 tickit-0.3.0/src/tickit/adapters/interpreters/wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-07-20 14:54:49.000000 tickit-0.3.0/src/tickit/adapters/interpreters/wrappers/beheading_interpreter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-07-20 14:54:49.000000 tickit-0.3.0/src/tickit/adapters/interpreters/wrappers/joining_interpreter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-07-20 14:54:49.000000 tickit-0.3.0/src/tickit/adapters/interpreters/wrappers/splitting_interpreter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:59.744578 tickit-0.3.0/src/tickit/adapters/servers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:49.000000 tickit-0.3.0/src/tickit/adapters/servers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-07-20 14:54:49.000000 tickit-0.3.0/src/tickit/adapters/servers/tcp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:59.744578 tickit-0.3.0/src/tickit/adapters/zeromq/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:49.000000 tickit-0.3.0/src/tickit/adapters/zeromq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-07-20 14:54:49.000000 tickit-0.3.0/src/tickit/adapters/zeromq/push_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-07-20 14:54:49.000000 tickit-0.3.0/src/tickit/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:59.744578 tickit-0.3.0/src/tickit/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:49.000000 tickit-0.3.0/src/tickit/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-07-20 14:54:49.000000 tickit-0.3.0/src/tickit/core/adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:59.744578 tickit-0.3.0/src/tickit/core/components/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:49.000000 tickit-0.3.0/src/tickit/core/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5844 2023-07-20 14:54:49.000000 tickit-0.3.0/src/tickit/core/components/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3417 2023-07-20 14:54:49.000000 tickit-0.3.0/src/tickit/core/components/device_simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-07-20 14:54:49.000000 tickit-0.3.0/src/tickit/core/components/system_simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-07-20 14:54:49.000000 tickit-0.3.0/src/tickit/core/device.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:59.744578 tickit-0.3.0/src/tickit/core/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:49.000000 tickit-0.3.0/src/tickit/core/management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11021 2023-07-20 14:54:49.000000 tickit-0.3.0/src/tickit/core/management/event_router.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:59.744578 tickit-0.3.0/src/tickit/core/management/schedulers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:49.000000 tickit-0.3.0/src/tickit/core/management/schedulers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6428 2023-07-20 14:54:49.000000 tickit-0.3.0/src/tickit/core/management/schedulers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5972 2023-07-20 14:54:49.000000 tickit-0.3.0/src/tickit/core/management/schedulers/master.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7209 2023-07-20 14:54:49.000000 tickit-0.3.0/src/tickit/core/management/schedulers/slave.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6135 2023-07-20 14:54:49.000000 tickit-0.3.0/src/tickit/core/management/ticker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-07-20 14:54:49.000000 tickit-0.3.0/src/tickit/core/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-07-20 14:54:49.000000 tickit-0.3.0/src/tickit/core/simulation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:59.748578 tickit-0.3.0/src/tickit/core/state_interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-20 14:54:49.000000 tickit-0.3.0/src/tickit/core/state_interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6055 2023-07-20 14:54:49.000000 tickit-0.3.0/src/tickit/core/state_interfaces/internal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-07-20 14:54:49.000000 tickit-0.3.0/src/tickit/core/state_interfaces/kafka.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5628 2023-07-20 14:54:49.000000 tickit-0.3.0/src/tickit/core/state_interfaces/state_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-07-20 14:54:49.000000 tickit-0.3.0/src/tickit/core/typedefs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:59.748578 tickit-0.3.0/src/tickit/devices/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:49.000000 tickit-0.3.0/src/tickit/devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-07-20 14:54:49.000000 tickit-0.3.0/src/tickit/devices/iobox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-07-20 14:54:49.000000 tickit-0.3.0/src/tickit/devices/sink.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-07-20 14:54:49.000000 tickit-0.3.0/src/tickit/devices/source.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:59.748578 tickit-0.3.0/src/tickit/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:49.000000 tickit-0.3.0/src/tickit/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-07-20 14:54:49.000000 tickit-0.3.0/src/tickit/utils/byte_format.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:59.748578 tickit-0.3.0/src/tickit/utils/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:49.000000 tickit-0.3.0/src/tickit/utils/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-20 14:54:49.000000 tickit-0.3.0/src/tickit/utils/configuration/loading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-07-20 14:54:49.000000 tickit-0.3.0/src/tickit/utils/configuration/tagged_union.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-20 14:54:49.000000 tickit-0.3.0/src/tickit/utils/singleton.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-07-20 14:54:49.000000 tickit-0.3.0/src/tickit/utils/topic_naming.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:59.740579 tickit-0.3.0/src/tickit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18613 2023-07-20 14:54:59.000000 tickit-0.3.0/src/tickit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7139 2023-07-20 14:54:59.000000 tickit-0.3.0/src/tickit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 14:54:59.000000 tickit-0.3.0/src/tickit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-20 14:54:59.000000 tickit-0.3.0/src/tickit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-20 14:54:59.000000 tickit-0.3.0/src/tickit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-20 14:54:59.000000 tickit-0.3.0/src/tickit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:59.748578 tickit-0.3.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:59.748578 tickit-0.3.0/tests/adapters/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:59.748578 tickit-0.3.0/tests/adapters/interpreters/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:59.748578 tickit-0.3.0/tests/adapters/interpreters/command/
+-rw-r--r--   0 runner    (1001) docker     (123)     4766 2023-07-20 14:54:49.000000 tickit-0.3.0/tests/adapters/interpreters/command/test_command_interpreter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-07-20 14:54:49.000000 tickit-0.3.0/tests/adapters/interpreters/command/test_regex_command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:59.748578 tickit-0.3.0/tests/adapters/interpreters/endpoints/
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-07-20 14:54:49.000000 tickit-0.3.0/tests/adapters/interpreters/endpoints/test_http_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-20 14:54:49.000000 tickit-0.3.0/tests/adapters/interpreters/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:59.752579 tickit-0.3.0/tests/adapters/interpreters/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-20 14:54:49.000000 tickit-0.3.0/tests/adapters/interpreters/wrappers/test_beheading_interpreter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-07-20 14:54:49.000000 tickit-0.3.0/tests/adapters/interpreters/wrappers/test_joining_interpreter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5992 2023-07-20 14:54:49.000000 tickit-0.3.0/tests/adapters/interpreters/wrappers/test_splitting_interpreter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:59.752579 tickit-0.3.0/tests/adapters/servers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-07-20 14:54:49.000000 tickit-0.3.0/tests/adapters/servers/test_tcp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:59.752579 tickit-0.3.0/tests/adapters/test_epicsadapter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:49.000000 tickit-0.3.0/tests/adapters/test_epicsadapter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4937 2023-07-20 14:54:49.000000 tickit-0.3.0/tests/adapters/test_epicsadapter/test_epics_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9216 2023-07-20 14:54:49.000000 tickit-0.3.0/tests/adapters/test_httpadapter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:59.752579 tickit-0.3.0/tests/adapters/zeromq/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:49.000000 tickit-0.3.0/tests/adapters/zeromq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-07-20 14:54:49.000000 tickit-0.3.0/tests/adapters/zeromq/test_push_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-07-20 14:54:49.000000 tickit-0.3.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:59.752579 tickit-0.3.0/tests/core/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:59.752579 tickit-0.3.0/tests/core/components/
+-rw-r--r--   0 runner    (1001) docker     (123)     4204 2023-07-20 14:54:49.000000 tickit-0.3.0/tests/core/components/test_component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-07-20 14:54:49.000000 tickit-0.3.0/tests/core/components/test_device_simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4833 2023-07-20 14:54:49.000000 tickit-0.3.0/tests/core/components/test_system_simulation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:59.752579 tickit-0.3.0/tests/core/management/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:59.752579 tickit-0.3.0/tests/core/management/schedulers/
+-rw-r--r--   0 runner    (1001) docker     (123)     3774 2023-07-20 14:54:49.000000 tickit-0.3.0/tests/core/management/schedulers/test_base_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6419 2023-07-20 14:54:49.000000 tickit-0.3.0/tests/core/management/schedulers/test_master_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6405 2023-07-20 14:54:49.000000 tickit-0.3.0/tests/core/management/schedulers/test_slave_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18354 2023-07-20 14:54:49.000000 tickit-0.3.0/tests/core/management/test_event_router.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6239 2023-07-20 14:54:49.000000 tickit-0.3.0/tests/core/management/test_ticker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-20 14:54:49.000000 tickit-0.3.0/tests/core/sim.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:59.756579 tickit-0.3.0/tests/core/state_interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)     4109 2023-07-20 14:54:49.000000 tickit-0.3.0/tests/core/state_interfaces/test_internal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-07-20 14:54:49.000000 tickit-0.3.0/tests/core/state_interfaces/test_kafka.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-20 14:54:49.000000 tickit-0.3.0/tests/core/state_interfaces/test_state_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-07-20 14:54:49.000000 tickit-0.3.0/tests/core/test_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-20 14:54:49.000000 tickit-0.3.0/tests/core/test_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5822 2023-07-20 14:54:49.000000 tickit-0.3.0/tests/core/test_simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-07-20 14:54:49.000000 tickit-0.3.0/tests/core/test_typedefs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:59.756579 tickit-0.3.0/tests/devices/
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-07-20 14:54:49.000000 tickit-0.3.0/tests/devices/test_iobox.py
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-20 14:54:49.000000 tickit-0.3.0/tests/devices/test_sink.py
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-20 14:54:49.000000 tickit-0.3.0/tests/devices/test_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-07-20 14:54:49.000000 tickit-0.3.0/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:59.756579 tickit-0.3.0/tests/utils/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:54:59.756579 tickit-0.3.0/tests/utils/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-07-20 14:54:49.000000 tickit-0.3.0/tests/utils/configuration/test_loading.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-07-20 14:54:49.000000 tickit-0.3.0/tests/utils/test_byte_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-07-20 14:54:49.000000 tickit-0.3.0/tests/utils/test_configurable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-20 14:54:49.000000 tickit-0.3.0/tests/utils/test_singleton.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-20 14:54:49.000000 tickit-0.3.0/tests/utils/test_topic_naming.py
```

### Comparing `tickit-0.2.3/.devcontainer/devcontainer.json` & `tickit-0.3.0/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `tickit-0.2.3/.github/CONTRIBUTING.rst` & `tickit-0.3.0/.github/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `tickit-0.2.3/.github/actions/install_requirements/action.yml` & `tickit-0.3.0/.github/actions/install_requirements/action.yml`

 * *Files identical despite different names*

### Comparing `tickit-0.2.3/.github/dependabot.yml` & `tickit-0.3.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `tickit-0.2.3/.github/pages/make_switcher.py` & `tickit-0.3.0/.github/pages/make_switcher.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.3/.github/workflows/code.yml` & `tickit-0.3.0/.github/workflows/code.yml`

 * *Files 3% similar despite different names*

```diff
@@ -31,21 +31,16 @@
 
   test:
     if: github.event_name != 'pull_request' || github.event.pull_request.head.repo.full_name != github.repository
     strategy:
       fail-fast: false
       matrix:
         os: ["ubuntu-latest"] # can add windows-latest, macos-latest
-        python: ["3.8", "3.9", "3.10"]
-        install: ["-e .[dev]"]
-        # Make one version be non-editable to test both paths of version code
-        include:
-          - os: "ubuntu-latest"
-            python: "3.8"
-            install: ".[dev]"
+        python: ["3.9", "3.10"]
+        install: [".[dev]", "-e .[dev]"]
 
     runs-on: ${{ matrix.os }}
     env:
       # https://github.com/pytest-dev/pytest/issues/2042
       PY_IGNORE_IMPORTMISMATCH: "1"
 
     steps:
```

### Comparing `tickit-0.2.3/.github/workflows/docs.yml` & `tickit-0.3.0/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `tickit-0.2.3/.github/workflows/docs_clean.yml` & `tickit-0.3.0/.github/workflows/docs_clean.yml`

 * *Files identical despite different names*

### Comparing `tickit-0.2.3/.github/workflows/linkcheck.yml` & `tickit-0.3.0/.github/workflows/linkcheck.yml`

 * *Files identical despite different names*

### Comparing `tickit-0.2.3/.gitignore` & `tickit-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `tickit-0.2.3/.gitlab-ci.yml` & `tickit-0.3.0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `tickit-0.2.3/.vscode/launch.json` & `tickit-0.3.0/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `tickit-0.2.3/.vscode/settings.json` & `tickit-0.3.0/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `tickit-0.2.3/CHANGELOG.rst` & `tickit-0.3.0/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `tickit-0.2.3/Dockerfile` & `tickit-0.3.0/Dockerfile`

 * *Files identical despite different names*

### Comparing `tickit-0.2.3/LICENSE` & `tickit-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tickit-0.2.3/PKG-INFO` & `tickit-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tickit
-Version: 0.2.3
+Version: 0.3.0
 Summary: Event-based device simulation framework
 Author-email: Callum Forrester <callum.forrester@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -204,18 +204,17 @@
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
         
 Project-URL: GitHub, https://github.com/dls-controls/tickit
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
 License-File: LICENSE
 
 tickit
 ======
 
@@ -237,21 +236,23 @@
 A simulation is defined using a yaml file, in which the graphing of the required
 components is denoted. This file defines a **Counter** device named **counter** and
 a **Sink** device named **counter_sink**. The output **_value** of **counter** is wired
 to the input of **counter_sink**.
 
 .. code-block:: yaml
 
-    - examples.devices.counter.Counter:
-        name: counter
-        inputs: {}
-    - tickit.devices.sink.Sink:
-        name: counter_sink
-        inputs:
-          input: counter:_value
+    - type: examples.devices.counter.Counter
+      name: counter
+      inputs: {}
+    - type: tickit.devices.sink.Sink
+      name: counter_sink
+      inputs:
+        input:
+          component: counter
+          port: _value
 
 
 This file is executed to run the simulation.
 
 .. code-block:: bash
 
     python -m tickit all examples/configs/counter.yaml
```

### Comparing `tickit-0.2.3/README.rst` & `tickit-0.3.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -19,21 +19,23 @@
 A simulation is defined using a yaml file, in which the graphing of the required
 components is denoted. This file defines a **Counter** device named **counter** and
 a **Sink** device named **counter_sink**. The output **_value** of **counter** is wired
 to the input of **counter_sink**.
 
 .. code-block:: yaml
 
-    - examples.devices.counter.Counter:
-        name: counter
-        inputs: {}
-    - tickit.devices.sink.Sink:
-        name: counter_sink
-        inputs:
-          input: counter:_value
+    - type: examples.devices.counter.Counter
+      name: counter
+      inputs: {}
+    - type: tickit.devices.sink.Sink
+      name: counter_sink
+      inputs:
+        input:
+          component: counter
+          port: _value
 
 
 This file is executed to run the simulation.
 
 .. code-block:: bash
 
     python -m tickit all examples/configs/counter.yaml
```

### Comparing `tickit-0.2.3/docs/_static/theme_overrides.css` & `tickit-0.3.0/docs/_static/theme_overrides.css`

 * *Files identical despite different names*

### Comparing `tickit-0.2.3/docs/conf.py` & `tickit-0.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.3/docs/developer/explanations/decisions.rst` & `tickit-0.3.0/docs/developer/explanations/decisions.rst`

 * *Files identical despite different names*

### Comparing `tickit-0.2.3/docs/developer/explanations/framework-details.rst` & `tickit-0.3.0/docs/developer/explanations/framework-details.rst`

 * *Files identical despite different names*

### Comparing `tickit-0.2.3/docs/developer/explanations/how-component-updates-are-ordered.rst` & `tickit-0.3.0/docs/developer/explanations/how-component-updates-are-ordered.rst`

 * *Files identical despite different names*

### Comparing `tickit-0.2.3/docs/developer/explanations/why-tickit.rst` & `tickit-0.3.0/docs/developer/explanations/why-tickit.rst`

 * *Files identical despite different names*

### Comparing `tickit-0.2.3/docs/developer/how-to/build-docs.rst` & `tickit-0.3.0/docs/developer/how-to/build-docs.rst`

 * *Files identical despite different names*

### Comparing `tickit-0.2.3/docs/developer/how-to/lint.rst` & `tickit-0.3.0/docs/developer/how-to/lint.rst`

 * *Files identical despite different names*

### Comparing `tickit-0.2.3/docs/developer/how-to/make-release.rst` & `tickit-0.3.0/docs/developer/how-to/make-release.rst`

 * *Files identical despite different names*

### Comparing `tickit-0.2.3/docs/developer/how-to/pin-requirements.rst` & `tickit-0.3.0/docs/developer/how-to/pin-requirements.rst`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
 The files are created using ``pip freeze`` and will contain a full list
 of the dependencies and sub-dependencies with pinned versions.
 
 You can download any of these files by clicking on them. It is best to use
 the one that ran with the lowest Python version as this is more likely to
 be compatible with all the versions of Python in the test matrix.
-i.e. ``requirements-test-ubuntu-latest-3.8.txt`` in this example.
+i.e. ``requirements-test-ubuntu-latest-3.9.txt`` in this example.
 
 Applying the lock file
 ----------------------
 
 To apply a lockfile:
 
 - copy the requirements file you have downloaded to the root of your
```

### Comparing `tickit-0.2.3/docs/developer/how-to/test-container.rst` & `tickit-0.3.0/docs/developer/how-to/test-container.rst`

 * *Files identical despite different names*

### Comparing `tickit-0.2.3/docs/developer/how-to/update-tools.rst` & `tickit-0.3.0/docs/developer/how-to/update-tools.rst`

 * *Files identical despite different names*

### Comparing `tickit-0.2.3/docs/developer/index.rst` & `tickit-0.3.0/docs/developer/index.rst`

 * *Files identical despite different names*

### Comparing `tickit-0.2.3/docs/developer/reference/standards.rst` & `tickit-0.3.0/docs/developer/reference/standards.rst`

 * *Files identical despite different names*

### Comparing `tickit-0.2.3/docs/developer/tutorials/dev-install.rst` & `tickit-0.3.0/docs/developer/tutorials/dev-install.rst`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
     $ git clone git://github.com/dls-controls/tickit.git
 
 Install dependencies
 --------------------
 
 You can choose to either develop on the host machine using a `venv` (which
-requires python 3.8 or later) or to run in a container under `VSCode
+requires python 3.9 or later) or to run in a container under `VSCode
 <https://code.visualstudio.com/>`_
 
 .. tab-set::
 
     .. tab-item:: Local virtualenv
 
         .. code::
```

### Comparing `tickit-0.2.3/docs/images/example-systems.drawio.svg` & `tickit-0.3.0/docs/images/example-systems.drawio.svg`

 * *Files identical despite different names*

### Comparing `tickit-0.2.3/docs/images/tickit-create-device-amplifier.svg` & `tickit-0.3.0/docs/images/tickit-create-device-amplifier.svg`

 * *Files identical despite different names*

### Comparing `tickit-0.2.3/docs/images/tickit-device-simulation-cpt.svg` & `tickit-0.3.0/docs/images/tickit-device-simulation-cpt.svg`

 * *Files identical despite different names*

### Comparing `tickit-0.2.3/docs/images/tickit-logo.ico` & `tickit-0.3.0/docs/images/tickit-logo.ico`

 * *Files identical despite different names*

### Comparing `tickit-0.2.3/docs/images/tickit-logo.svg` & `tickit-0.3.0/docs/images/tickit-logo.svg`

 * *Files identical despite different names*

### Comparing `tickit-0.2.3/docs/images/tickit-overview-full.svg` & `tickit-0.3.0/docs/images/tickit-overview-full.svg`

 * *Files identical despite different names*

### Comparing `tickit-0.2.3/docs/images/tickit-simple-dag.svg` & `tickit-0.3.0/docs/images/tickit-simple-dag.svg`

 * *Files identical despite different names*

### Comparing `tickit-0.2.3/docs/images/tickit-simple-overview-with-system-simulation.svg` & `tickit-0.3.0/docs/images/tickit-simple-overview-with-system-simulation.svg`

 * *Files identical despite different names*

### Comparing `tickit-0.2.3/docs/images/tickit-simple-overview.svg` & `tickit-0.3.0/docs/images/tickit-simple-overview.svg`

 * *Files identical despite different names*

### Comparing `tickit-0.2.3/docs/images/tickit-simple-simulation.svg` & `tickit-0.3.0/docs/images/tickit-simple-simulation.svg`

 * *Files identical despite different names*

### Comparing `tickit-0.2.3/docs/images/tickit-system-simulation-cpt.svg` & `tickit-0.3.0/docs/images/tickit-system-simulation-cpt.svg`

 * *Files identical despite different names*

### Comparing `tickit-0.2.3/docs/index.rst` & `tickit-0.3.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `tickit-0.2.3/docs/user/explanations/adapters.rst` & `tickit-0.3.0/docs/user/explanations/adapters.rst`

 * *Files identical despite different names*

### Comparing `tickit-0.2.3/docs/user/explanations/components.rst` & `tickit-0.3.0/docs/user/explanations/components.rst`

 * *Files 14% similar despite different names*

```diff
@@ -33,36 +33,44 @@
 allowing for the construction of reasonably complex systems.
 
 System simulations can be nested inside other components in the config so that
 the master scheduler's wiring is correct, for example:
 
 .. code-block:: yaml
 
-    - examples.devices.trampoline.RandomTrampoline:
-        name: random_trampoline
-        inputs: {}
-        callback_period: 10000000000
-    - tickit.core.components.system_simulation.SystemSimulation:
-        name: internal_tickit
-        inputs:
-          input_1: random_trampoline:output
-        components:
-          - tickit.devices.sink.Sink:
-              name: internal_sink
-              inputs:
-                sink_1: external:input_1
-          - examples.devices.remote_controlled.RemoteControlled:
-              name: internal_tcp_controlled
-              inputs: {}
-        expose:
-          output_1: internal_tcp_controlled:observed
-    - tickit.devices.sink.Sink:
-        name: external_sink
-        inputs:
-          sink_1: internal_tickit:output_1
+    - type: examples.devices.trampoline.RandomTrampoline
+      name: random_trampoline
+      inputs: {}
+      callback_period: 10000000000
+    - type: tickit.core.components.system_simulation.SystemSimulation
+      name: internal_tickit
+      inputs:
+        input_1:
+          component: random_trampoline
+          port: output
+      components:
+        - type: tickit.devices.sink.Sink
+          name: internal_sink
+          inputs:
+            sink_1:
+              component: external
+              port: input_1
+        - type: examples.devices.remote_controlled.RemoteControlled
+          name: internal_tcp_controlled
+          inputs: {}
+      expose:
+        output_1:
+          component: internal_tcp_controlled
+          port: observed
+    - type: tickit.devices.sink.Sink
+      name: external_sink
+      inputs:
+        sink_1:
+          component: internal_tickit
+          port: output_1
 
 (See `SystemSimulationComponent`.)
 
 The Overall Simulation
 -------------------------------
 
 A simulation containing both types of component will look something like this:
```

### Comparing `tickit-0.2.3/docs/user/explanations/devices.rst` & `tickit-0.3.0/docs/user/explanations/devices.rst`

 * *Files identical despite different names*

### Comparing `tickit-0.2.3/docs/user/explanations/framework-summary.rst` & `tickit-0.3.0/docs/user/explanations/framework-summary.rst`

 * *Files identical despite different names*

### Comparing `tickit-0.2.3/docs/user/explanations/glossary.rst` & `tickit-0.3.0/docs/user/explanations/glossary.rst`

 * *Files identical despite different names*

### Comparing `tickit-0.2.3/docs/user/explanations/wiring.rst` & `tickit-0.3.0/docs/user/explanations/wiring.rst`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,17 @@
 
 This wiring is achieved with a configuration yaml file which is passed to the
 scheduler when starting a simulation. Here we see an example trampoline device
 which outputs random numbers, and a sink taking that output as an input:
 
 .. code-block:: yaml
 
-    - examples.devices.trampoline.RandomTrampoline:
-        name: rand_tramp
-        inputs: {}
-        callback_period: 1000000000
-    - tickit.devices.sink.Sink:
-        name: tramp_sink
-        inputs:
-          input: rand_tramp:output
+    - type: examples.devices.trampoline.RandomTrampoline
+      name: rand_tramp
+      inputs: {}
+      callback_period: 1000000000
+    - type: tickit.devices.sink.Sink
+      name: tramp_sink
+      inputs:
+        input:
+          component: rand_tramp
+          port: output
```

### Comparing `tickit-0.2.3/docs/user/how-to/use-command-wrappers.rst` & `tickit-0.3.0/docs/user/how-to/use-command-wrappers.rst`

 * *Files identical despite different names*

### Comparing `tickit-0.2.3/docs/user/how-to/use-epics-adapter.rst` & `tickit-0.3.0/docs/user/how-to/use-epics-adapter.rst`

 * *Files identical despite different names*

### Comparing `tickit-0.2.3/docs/user/index.rst` & `tickit-0.3.0/docs/user/index.rst`

 * *Files identical despite different names*

### Comparing `tickit-0.2.3/docs/user/reference/api.rst` & `tickit-0.3.0/docs/user/reference/api.rst`

 * *Files 4% similar despite different names*

```diff
@@ -282,18 +282,18 @@
         ----------------------------
 
     .. automodule:: tickit.utils.configuration
 
         ``tickit.utils.configuration``
         ------------------------------
 
-        .. automodule:: tickit.utils.configuration.configurable
+        .. automodule:: tickit.utils.configuration.tagged_union
             :members:
 
-            ``tickit.utils.configuration.configurable``
+            ``tickit.utils.configuration.tagged_union``
             -------------------------------------------
 
         .. automodule:: tickit.utils.configuration.loading
             :members:
 
             ``tickit.utils.configuration.loading``
             --------------------------------------
```

### Comparing `tickit-0.2.3/docs/user/tutorials/create-a-device.rst` & `tickit-0.3.0/docs/user/tutorials/create-a-device.rst`

 * *Files 2% similar despite different names*

```diff
@@ -114,21 +114,21 @@
 device, and defines any default initial configuration values. As well as this, we
 overwrite the magic method `__call__()`, which returns a `DeviceSimulation` object.
 This object takes the component name, as well as its device. We will return to this
 if the device requires any adapters to control it externally.
 
 .. code-block:: python
 
-    from dataclasses import dataclass
+    import pydantic.v1.dataclasses
 
     from tickit.core.components.component import Component, ComponentConfig
     from tickit.core.components.device_simulation import DeviceSimulation
 
 
-    @dataclass
+    @pydantic.v1.dataclasses.dataclass
     class Amplifier(ComponentConfig):
         initial_amplification: float
 
         def __call__(self) -> Component:
             return DeviceSimulation(
                 name=self.name,
                 device=AmplifierDevice(
@@ -143,27 +143,31 @@
 In order to use the device we must first create a simulation configuration yaml
 file. This file will be used to set up our simulation and will consist of: a
 `Source`, named source, which will produce a constant input signal; our amplifier;
 and a `Sink`, named sink, which will receive the amplified signal.
 
 .. code-block:: yaml
 
-    - tickit.devices.source.Source:
-        name: source
-        inputs: {}
-        value: 10.0
-    - amp.Amplifier:
-        name: amp
-        inputs:
-          initial_signal: source:value
-        initial_amplification: 2.0
-    - tickit.devices.sink.Sink:
-        name: sink
-        inputs:
-          input: amp:amplified_signal
+    - type: tickit.devices.source.Source
+      name: source
+      inputs: {}
+      value: 10.0
+    - type: amp.Amplifier
+      name: amp
+      inputs:
+        initial_signal:
+          component: source
+          port: value
+      initial_amplification: 2.0
+    - type: tickit.devices.sink.Sink
+      name: sink
+      inputs:
+        input:
+          component: amp
+          port: amplified_signal
 
 
 Where in ``amp.Amplifier`` ``amp`` is the name of the ``.py`` file the amplifier
 is written in, and Amplifier is the name of the `ComponentConfig` for the amplifier.
 
 .. seealso::
     See the :doc:`Creating a Simulation<../tutorials/creating-a-simulation>` tutorial for a walk-through of creating simulation
```

### Comparing `tickit-0.2.3/docs/user/tutorials/creating-a-simulation.rst` & `tickit-0.3.0/docs/user/tutorials/creating-a-simulation.rst`

 * *Files 6% similar despite different names*

```diff
@@ -22,31 +22,33 @@
 In this example our first device shall be a ``RandomTrampoline`` with a callback_period
 of :math:`1s` or :math:`10^9n\s` named ``rand_tramp`` with no adapters - denoted
 in YAML by ``[]`` - and with no mapped inputs - denoted in YAML by ``{}``. As such
 we may extend our config, as:
 
 .. code-block:: yaml
 
-    - examples.devices.trampoline.RandomTrampoline:
-        name: rand_tramp
-        inputs: {}
+    - type: examples.devices.trampoline.RandomTrampoline
+      name: rand_tramp
+      inputs: {}
 
 We will now add a `Sink` device. This device will be named ``tramp_sink``, will have
 no adapters but will take the ``output`` value of ``rand_tramp`` as ``input``. As
 such we may extend our config, as:
 
 .. code-block:: yaml
 
-    - examples.devices.trampoline.RandomTrampoline:
-        name: rand_tramp
-        inputs: {}
-    - tickit.devices.sink.Sink:
-        name: tramp_sink
-        inputs:
-          input: rand_tramp:output
+    - type: examples.devices.trampoline.RandomTrampoline
+      name: rand_tramp
+      inputs: {}
+    - type: tickit.devices.sink.Sink
+      name: tramp_sink
+      inputs:
+        input:
+          component rand_tramp
+          port: output
 
 Running the Simulation
 ----------------------
 
 Finally, we likely wish to run the simulation, this may be performed by running the
 following command:
```

### Comparing `tickit-0.2.3/docs/user/tutorials/installation.rst` & `tickit-0.3.0/docs/user/tutorials/installation.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Installation
 ============
 
 Check your version of python
 ----------------------------
 
-You will need python 3.8 or later. You can check your version of python by
+You will need python 3.9 or later. You can check your version of python by
 typing into a terminal::
 
     $ python3 --version
 
 
 Create a virtual environment
 ----------------------------
```

### Comparing `tickit-0.2.3/docs/user/tutorials/running-a-simulation.rst` & `tickit-0.3.0/docs/user/tutorials/running-a-simulation.rst`

 * *Files identical despite different names*

### Comparing `tickit-0.2.3/docs/user/tutorials/use-composed-adapter.rst` & `tickit-0.3.0/docs/user/tutorials/use-composed-adapter.rst`

 * *Files 1% similar despite different names*

```diff
@@ -96,15 +96,15 @@
     from tickit.adapters.interpreters.command.command_interpreter import CommandInterpreter
     from tickit.adapters.interpreters.command.regex_command import RegexCommand
     from tickit.adapters.servers.tcp import TcpServer
     from tickit.utils.byte_format import ByteFormat
 
 
     class AmplifierAdapter(ComposedAdapter):
-    device: AmplifierDevice
+        device: AmplifierDevice
 
         def __init__(
             self,
             host: str = "localhost",
             port: int = 25565,
         ) -> None:
             super().__init__(
@@ -126,15 +126,15 @@
 
 In order to now use this adapter to control our device we need to include it in
 our amplifier `ComponentConfig`. To do this we simply add it to the arguments of
 `DeviceSimulation`.
 
 .. code-block:: python
 
-    @dataclass
+    @pydantic.v1.dataclasses.dataclass
     class Amplifier(ComponentConfig):
         initial_amplification: int
 
         def __call__(self) -> Component:
             return DeviceSimulation(
                 name=self.name,
                 device=AmplifierDevice(
```

### Comparing `tickit-0.2.3/examples/configs/nested.yaml` & `tickit-0.3.0/examples/configs/nested.yaml`

 * *Files 25% similar despite different names*

```diff
@@ -1,22 +1,30 @@
-- examples.devices.trampoline.RandomTrampoline:
-    name: random_trampoline
-    inputs: {}
-    callback_period: 10000000000
-- tickit.core.components.system_simulation.SystemSimulation:
-    name: internal_tickit
-    inputs:
-      input_1: random_trampoline:output
-    components:
-      - tickit.devices.sink.Sink:
-          name: internal_sink
-          inputs:
-            sink_1: external:input_1
-      - examples.devices.remote_controlled.RemoteControlled:
-          name: internal_tcp_controlled
-          inputs: {}
-    expose:
-      output_1: internal_tcp_controlled:observed
-- tickit.devices.sink.Sink:
-    name: external_sink
-    inputs:
-      sink_1: internal_tickit:output_1
+- type: examples.devices.trampoline.RandomTrampoline
+  name: random_trampoline
+  inputs: {}
+  callback_period: 10000000000
+- type: tickit.core.components.system_simulation.SystemSimulation
+  name: internal_tickit
+  inputs:
+    input_1:
+      component: random_trampoline
+      port: output
+  components:
+    - type: tickit.devices.sink.Sink
+      name: internal_sink
+      inputs:
+        sink_1:
+          component: external
+          port: input_1
+    - type: examples.devices.remote_controlled.RemoteControlled
+      name: internal_tcp_controlled
+      inputs: {}
+  expose:
+    output_1:
+      component: internal_tcp_controlled
+      port: observed
+- type: tickit.devices.sink.Sink
+  name: external_sink
+  inputs:
+    sink_1:
+      component: internal_tickit
+      port: output_1
```

### Comparing `tickit-0.2.3/examples/devices/amplifier.py` & `tickit-0.3.0/examples/devices/amplifier.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-from dataclasses import dataclass
-
+import pydantic.v1.dataclasses
 from typing_extensions import TypedDict
 
 from tickit.adapters.composed import ComposedAdapter
 from tickit.adapters.interpreters.command.command_interpreter import CommandInterpreter
 from tickit.adapters.interpreters.command.regex_command import RegexCommand
 from tickit.adapters.servers.tcp import TcpServer
 from tickit.core.components.component import Component, ComponentConfig
@@ -85,15 +84,15 @@
 
         Args:
             amplification (float): The desired value of amplification.
         """
         self.device.amplification = amplification
 
 
-@dataclass
+@pydantic.v1.dataclasses.dataclass
 class Amplifier(ComponentConfig):
     """Amplifier you can set the amplification value of over TCP."""
 
     initial_amplification: int
 
     def __call__(self) -> Component:  # noqa: D102
         return DeviceSimulation(
```

### Comparing `tickit-0.2.3/examples/devices/counter.py` & `tickit-0.3.0/examples/devices/counter.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import logging
-from dataclasses import dataclass
+from typing import TypedDict
+
+import pydantic.v1.dataclasses
 
 from tickit.core.components.component import Component, ComponentConfig
 from tickit.core.components.device_simulation import DeviceSimulation
 from tickit.core.device import Device, DeviceUpdate
 from tickit.core.typedefs import SimTime
-from tickit.utils.compat.typing_compat import TypedDict
 
 LOGGER = logging.getLogger(__name__)
 
 
-@dataclass
+@pydantic.v1.dataclasses.dataclass
 class Counter(ComponentConfig):
     """Simulation of simple counting device."""
 
     def __call__(self) -> Component:  # noqa: D102
         return DeviceSimulation(name=self.name, device=CounterDevice())
```

### Comparing `tickit-0.2.3/examples/devices/http_device.py` & `tickit-0.3.0/examples/devices/http_device.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-from dataclasses import dataclass
-
+import pydantic.v1.dataclasses
 from aiohttp import web
 
 from tickit.adapters.httpadapter import HttpAdapter
 from tickit.adapters.interpreters.endpoints.http_endpoint import HttpEndpoint
 from tickit.core.components.component import Component, ComponentConfig
 from tickit.core.components.device_simulation import DeviceSimulation
 from tickit.devices.iobox import IoBoxDevice
@@ -40,16 +39,16 @@
             web.Response: [description]
         """
         address = request.match_info["address"]
         value = self.device.read(address)
         return web.json_response({address: value})
 
 
-@dataclass
-class ExampleHttpDevice(ComponentConfig):
+@pydantic.v1.dataclasses.dataclass
+class ExampleHTTPDevice(ComponentConfig):
     """Example HTTP device."""
 
     host: str = "localhost"
     port: int = 8080
 
     def __call__(self) -> Component:  # noqa: D102
         return DeviceSimulation(
```

### Comparing `tickit-0.2.3/examples/devices/isolated_device.py` & `tickit-0.3.0/examples/devices/isolated_device.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from dataclasses import dataclass
 from typing import TypedDict
 
+import pydantic.v1.dataclasses
 from softioc import builder
 
 from tickit.adapters.composed import ComposedAdapter
 from tickit.adapters.epicsadapter.adapter import EpicsAdapter
 from tickit.adapters.interpreters.command.command_interpreter import CommandInterpreter
 from tickit.adapters.interpreters.command.regex_command import RegexCommand
 from tickit.adapters.servers.tcp import TcpServer
@@ -112,15 +112,15 @@
 
     def on_db_load(self) -> None:
         """Customises records that have been loaded in to suit the simulation."""
         builder.aOut("VALUE", initial_value=self.device.value, on_update=self.callback)
         self.link_input_on_interrupt(builder.aIn("VALUE_RBV"), self.device.get_value)
 
 
-@dataclass
+@pydantic.v1.dataclasses.dataclass
 class IsolatedBox(ComponentConfig):
     """Isolated box device you can change the value of either over TCP or via EPICS."""
 
     initial_value: float
     port: int
     ioc_name: str
     host: str = "localhost"
```

### Comparing `tickit-0.2.3/examples/devices/remote_controlled.py` & `tickit-0.3.0/examples/devices/remote_controlled.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import asyncio
 import logging
 import struct
-from dataclasses import dataclass
-from typing import AsyncIterable, Optional
+from typing import AsyncIterable, Optional, TypedDict
+
+import pydantic.v1.dataclasses
 
 from tickit.adapters.composed import ComposedAdapter
 from tickit.adapters.interpreters.command import CommandInterpreter, RegexCommand
 from tickit.adapters.servers.tcp import TcpServer
 from tickit.core.adapter import Server
 from tickit.core.components.component import Component, ComponentConfig
 from tickit.core.components.device_simulation import DeviceSimulation
 from tickit.core.device import Device, DeviceUpdate
 from tickit.core.typedefs import SimTime
 from tickit.utils.byte_format import ByteFormat
-from tickit.utils.compat.typing_compat import TypedDict
 
 LOGGER = logging.getLogger(__name__)
 
 
 class RemoteControlledDevice(Device):
     """A trivial toy device which is controlled by an adapter."""
 
@@ -219,15 +219,15 @@
                 specified number of times with a fixed delay.
         """
         for i in range(1, int(n)):
             await asyncio.sleep(1.0)
             yield f"Observed is {self.device.observed}".encode("utf-8")
 
 
-@dataclass
+@pydantic.v1.dataclasses.dataclass
 class RemoteControlled(ComponentConfig):
     """Thing you can poke over TCP."""
 
     format: ByteFormat = ByteFormat(b"%b\r\n")
 
     def __call__(self) -> Component:  # noqa: D102
         return DeviceSimulation(
```

### Comparing `tickit-0.2.3/examples/devices/shutter.py` & `tickit-0.3.0/examples/devices/shutter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-from dataclasses import dataclass
 from random import random
-from typing import Optional
+from typing import Optional, TypedDict
+
+import pydantic.v1.dataclasses
 
 from tickit.adapters.composed import ComposedAdapter
 from tickit.adapters.interpreters.command.command_interpreter import CommandInterpreter
 from tickit.adapters.interpreters.command.regex_command import RegexCommand
 from tickit.adapters.servers.tcp import TcpServer
 from tickit.core.components.component import Component, ComponentConfig
 from tickit.core.components.device_simulation import DeviceSimulation
 from tickit.core.device import Device, DeviceUpdate
 from tickit.core.typedefs import SimTime
 from tickit.utils.byte_format import ByteFormat
-from tickit.utils.compat.typing_compat import TypedDict
 
 
 class ShutterDevice(Device):
     """A toy device which downscales flux according to a set position.
 
     A toy device which produces an output flux which is downscaled from the input flux
     according to an internal state position. The position may be altered by setting new
@@ -150,15 +150,15 @@
         Args:
             target (str): The target position of the shutter.
         """
         self.device.target_position = float(target)
         self.device.last_time = None
 
 
-@dataclass
+@pydantic.v1.dataclasses.dataclass
 class Shutter(ComponentConfig):
     """Shutter you can open or close over TCP."""
 
     default_position: float
     initial_position: Optional[float] = None
     host: str = "localhost"
     port: int = 25565
```

### Comparing `tickit-0.2.3/examples/devices/trampoline.py` & `tickit-0.3.0/examples/devices/trampoline.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import logging
-from dataclasses import dataclass
 from random import randint
+from typing import TypedDict
+
+import pydantic.v1.dataclasses
 
 from tickit.core.components.component import Component, ComponentConfig
 from tickit.core.components.device_simulation import DeviceSimulation
 from tickit.core.device import Device, DeviceUpdate
 from tickit.core.typedefs import SimTime
-from tickit.utils.compat.typing_compat import TypedDict
 
 LOGGER = logging.getLogger(__name__)
 
 
 class TrampolineDevice(Device):
     """A trivial toy device which requests a callback every update."""
 
@@ -87,15 +88,15 @@
         LOGGER.debug(f"Boing! (delta: {time}, inputs: {inputs}, output: {output})")
         return DeviceUpdate(
             RandomTrampolineDevice.Outputs(output=output),
             SimTime(time + self.callback_period),
         )
 
 
-@dataclass
+@pydantic.v1.dataclasses.dataclass
 class RandomTrampoline(ComponentConfig):
     """Random thing that goes boing."""
 
     callback_period: int = int(1e9)
 
     def __call__(self) -> Component:  # noqa: D102
         return DeviceSimulation(
```

### Comparing `tickit-0.2.3/examples/devices/zeromq_push_device.py` & `tickit-0.3.0/examples/devices/zeromq_push_device.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,12 @@
-from dataclasses import dataclass, field
+from dataclasses import field
 from typing import Optional, Set
 
+import pydantic.v1.dataclasses
+
 from tickit.adapters.zeromq.push_adapter import (
     SocketFactory,
     ZeroMqPushAdapter,
     create_zmq_push_socket,
 )
 from tickit.core.components.component import Component, ComponentConfig
 from tickit.core.components.device_simulation import DeviceSimulation
@@ -29,15 +31,15 @@
 
     def after_update(self):
         for address in self._addresses_to_publish:
             value = self.device.read(address)
             self.send_message([{address: value}])
 
 
-@dataclass
+@pydantic.v1.dataclasses.dataclass
 class ExampleZeroMqPusher(ComponentConfig):
     """Device that can publish writes to its memory over a zeromq socket."""
 
     host: str = "127.0.0.1"
     port: int = 5555
     addresses_to_publish: Set[str] = field(default_factory=lambda: {"foo", "bar"})
```

### Comparing `tickit-0.2.3/pyproject.toml` & `tickit-0.3.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -3,37 +3,35 @@
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tickit"
 classifiers = [
     "Development Status :: 4 - Beta",
     "License :: OSI Approved :: Apache Software License",
-    "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
 ]
 description = "Event-based device simulation framework"
 dependencies = [
     "aiohttp",
     "aiokafka",
     "aiozmq",
-    "apischema==0.16.1",
     "immutables",
-    "pydantic",
+    "pydantic>=2.0",
     "pyyaml",
     "pyzmq",
     "softioc",
     "typing_extensions",
     "click==8.1.3",
 
 ] # Add project dependencies here, e.g. ["click", "numpy"]
 dynamic = ["version"]
 license.file = "LICENSE"
 readme = "README.rst"
-requires-python = ">=3.8"
+requires-python = ">=3.9"
 
 [project.optional-dependencies]
 dev = [
     "black",
     "mypy",
     "flake8-isort",
     "Flake8-pyproject",
@@ -124,16 +122,16 @@
 [tox]
 skipsdist=True
 
 [testenv:{pre-commit,mypy,pytest,docs}]
 # Don't create a virtualenv for the command, requires tox-direct plugin
 direct = True
 passenv = *
-allowlist_externals = 
-    pytest 
+allowlist_externals =
+    pytest
     pre-commit
     mypy
     sphinx-build
     sphinx-autobuild
 commands =
     pytest: pytest {posargs}
     mypy: mypy src tests {posargs}
```

### Comparing `tickit-0.2.3/src/tickit/adapters/composed.py` & `tickit-0.3.0/src/tickit/adapters/composed.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.3/src/tickit/adapters/epicsadapter/adapter.py` & `tickit-0.3.0/src/tickit/adapters/epicsadapter/adapter.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.3/src/tickit/adapters/epicsadapter/ioc_manager.py` & `tickit-0.3.0/src/tickit/adapters/epicsadapter/ioc_manager.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.3/src/tickit/adapters/httpadapter.py` & `tickit-0.3.0/src/tickit/adapters/httpadapter.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.3/src/tickit/adapters/interpreters/command/command_interpreter.py` & `tickit-0.3.0/src/tickit/adapters/interpreters/command/command_interpreter.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,22 @@
 from abc import abstractmethod
 from inspect import getmembers
-from typing import AnyStr, AsyncIterable, Optional, Sequence, Tuple, get_type_hints
+from typing import (
+    AnyStr,
+    AsyncIterable,
+    Optional,
+    Protocol,
+    Sequence,
+    Tuple,
+    get_type_hints,
+    runtime_checkable,
+)
 
 from tickit.adapters.interpreters.utils import wrap_as_async_iterable
 from tickit.core.adapter import Adapter, Interpreter
-from tickit.utils.compat.typing_compat import Protocol, runtime_checkable
 
 
 @runtime_checkable
 class Command(Protocol):
     """An interface for interpretable commands."""
 
     #: A flag which indicates whether calling of the method should trigger an interrupt
```

### Comparing `tickit-0.2.3/src/tickit/adapters/interpreters/command/regex_command.py` & `tickit-0.3.0/src/tickit/adapters/interpreters/command/regex_command.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.3/src/tickit/adapters/interpreters/endpoints/http_endpoint.py` & `tickit-0.3.0/src/tickit/adapters/interpreters/endpoints/http_endpoint.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.3/src/tickit/adapters/interpreters/utils.py` & `tickit-0.3.0/src/tickit/adapters/interpreters/utils.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.3/src/tickit/adapters/interpreters/wrappers/beheading_interpreter.py` & `tickit-0.3.0/src/tickit/adapters/interpreters/wrappers/beheading_interpreter.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.3/src/tickit/adapters/interpreters/wrappers/joining_interpreter.py` & `tickit-0.3.0/src/tickit/adapters/interpreters/wrappers/joining_interpreter.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.3/src/tickit/adapters/interpreters/wrappers/splitting_interpreter.py` & `tickit-0.3.0/src/tickit/adapters/interpreters/wrappers/splitting_interpreter.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.3/src/tickit/adapters/servers/tcp.py` & `tickit-0.3.0/src/tickit/adapters/servers/tcp.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.3/src/tickit/adapters/zeromq/push_adapter.py` & `tickit-0.3.0/src/tickit/adapters/zeromq/push_adapter.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.3/src/tickit/cli.py` & `tickit-0.3.0/src/tickit/cli.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 import asyncio
 import logging
+from typing import Iterable, Optional, Set
 
 import click
 from click.core import Context
 
-from tickit.core.management.event_router import InverseWiring
-from tickit.core.management.schedulers.master import MasterScheduler
-from tickit.core.runner import run_all_forever
-from tickit.core.state_interfaces.state_interface import get_interface, interfaces
-from tickit.utils.configuration.loading import read_configs
+from tickit.core.simulation import build_simulation
+from tickit.core.state_interfaces.state_interface import interfaces
+from tickit.core.typedefs import ComponentID
 
 
 @click.group(invoke_without_command=True)
 @click.version_option()
 @click.option(
     "--log-level",
     default="DEBUG",
@@ -29,62 +28,67 @@
     """
     logging.basicConfig(level=log_level)
 
     if ctx.invoked_subcommand is None:
         click.echo(main.get_help(ctx))
 
 
-@main.command(help="run a single simulated component")
-@click.argument("component")
+@main.command(help="run one or more components without a scheduler")
+@click.argument("components", nargs=-1)
 @click.argument("config_path")
 @click.option("--backend", default="kafka", type=click.Choice(list(interfaces(True))))
-def component(config_path: str, component: str, backend: str) -> None:
-    """Runs a single simulated component from a configuration file.
+def components(
+    config_path: str, components: Iterable[ComponentID], backend: str
+) -> None:
+    """Runs one or more simulated components from a configuration file.
+
+    If you pass it no componentID arguments it will run all of the components in the
+    configuration file.
 
     Args:
         config_path (str): The path to the configuration file.
-        component (str): The name of the component to be run.
+        components (Iterable[ComponentID]): The name of the components to be run,
+        seperated by whitespace. If none are provided, all components will be run.
         backend (str): The message broker to be used.
     """
-    configs = read_configs(config_path)
-    config = [config for config in configs if config.name == component]
-    assert len(config) == 1, f"Expected only one component {component}"
-    asyncio.run(run_all_forever([config[0]().run_forever(*get_interface(backend))]))
+    components_to_run: Optional[Set[ComponentID]]
+    if components == ():
+        components_to_run = None
+    else:
+        components_to_run = set(components)
+
+    asyncio.run(
+        build_simulation(
+            config_path,
+            backend,
+            include_schedulers=False,
+            components_to_run=components_to_run,
+        ).run()
+    )
 
 
 @main.command(help="run the simulation scheduler")
 @click.argument("config_path")
 @click.option("--backend", default="kafka", type=click.Choice(list(interfaces(True))))
 def scheduler(config_path: str, backend: str) -> None:
     """Runs the simulation master scheduler from a configuration file.
 
     Args:
         config_path (str): The path to the configuration file.
         backend (str): The message broker to be used.
     """
-    configs = read_configs(config_path)
-    inverse_wiring = InverseWiring.from_component_configs(configs)
-    scheduler = MasterScheduler(inverse_wiring, *get_interface(backend))
-    asyncio.run(run_all_forever([scheduler.run_forever()]))
+    asyncio.run(build_simulation(config_path, backend, include_components=False).run())
 
 
 @main.command(help="run a collection of devices with a scheduler")
 @click.argument("config_path")
 @click.option(
     "--backend", default="internal", type=click.Choice(list(interfaces(False)))
 )
 def all(config_path: str, backend: str) -> None:
     """Runs all components and the master scheduler from a configuration file.
 
     Args:
         config_path (str): The path to the configuration file.
         backend (str): The message broker to be used.
     """
-    configs = read_configs(config_path)
-    inverse_wiring = InverseWiring.from_component_configs(configs)
-    scheduler = MasterScheduler(inverse_wiring, *get_interface(backend))
-    asyncio.run(
-        run_all_forever(
-            [config().run_forever(*get_interface(backend)) for config in configs]
-            + [scheduler.run_forever()]
-        )
-    )
+    asyncio.run(build_simulation(config_path, backend).run())
```

### Comparing `tickit-0.2.3/src/tickit/core/adapter.py` & `tickit-0.3.0/src/tickit/core/adapter.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,30 +9,28 @@
     Tuple,
     TypeVar,
 )
 
 from typing_extensions import Protocol
 
 from tickit.core.device import Device
-from tickit.utils.configuration.configurable import as_tagged_union
 
 #: Message type
 T = TypeVar("T")
 
 
 # https://github.com/python/mypy/issues/708#issuecomment-647124281
 class RaiseInterrupt(Protocol):
     """A raise_interrupt function that should be passed to `Adapter`."""
 
     async def __call__(self) -> None:
         """The actual call signature."""
         pass
 
 
-@as_tagged_union
 class Adapter:
     """An interface for types which implement device adapters."""
 
     device: Device
     raise_interrupt: RaiseInterrupt
 
     def __getattr__(self, name: str) -> Any:
@@ -55,15 +53,14 @@
         self.device = device
         self.raise_interrupt = raise_interrupt
 
     def after_update(self):
         """A method which is called immediately after the device updates."""
 
 
-@as_tagged_union
 class Interpreter(ABC, Generic[T]):
     """An interface for types which handle messages received by an adapter."""
 
     @abstractmethod
     async def handle(
         self, adapter: Adapter, message: T
     ) -> Tuple[AsyncIterable[T], bool]:
@@ -79,15 +76,14 @@
 
         Returns:
             Tuple[AsyncIterable[T], bool]: A tuple containing both an asynchronous
                 iterable of reply messages and an interrupt flag.
         """
 
 
-@as_tagged_union
 class Server(Generic[T]):
     """An interface for types which implement an external messaging protocol."""
 
     async def run_forever(
         self,
         on_connect: Callable[[], AsyncIterable[Optional[T]]],
         handler: Callable[[T], Awaitable[AsyncIterable[Optional[T]]]],
```

### Comparing `tickit-0.2.3/src/tickit/core/components/component.py` & `tickit-0.3.0/src/tickit/core/components/component.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 import asyncio
 import logging
 import traceback
 from abc import abstractmethod
 from dataclasses import dataclass
-from typing import Dict, Optional, Type, Union
+from typing import Dict, Optional, Type
+
+import pydantic.v1.dataclasses
 
 from tickit.core.state_interfaces.state_interface import StateConsumer, StateProducer
 from tickit.core.typedefs import (
     Changes,
     ComponentException,
     ComponentID,
+    ComponentInput,
+    ComponentOutput,
     ComponentPort,
     Input,
     Interrupt,
     Output,
     PortID,
     SimTime,
     StopComponent,
 )
-from tickit.utils.configuration.configurable import as_tagged_union
+from tickit.utils.configuration.tagged_union import as_tagged_union
 from tickit.utils.topic_naming import input_topic, output_topic
 
 LOGGER = logging.getLogger(__name__)
 
 
-@dataclass  # type: ignore
-@as_tagged_union
+@dataclass
 class Component:
     """An interface for types which implement stand-alone simulation components.
 
     An interface for types which implement stand-alone simulation components.
     Components define the top level building blocks of a tickit simulation (examples
     include the DeviceSimulation which host a device and corresponding adapter or a
     SystemSimulation which hosts a SlaveScheduler and internal Components).
@@ -50,16 +53,16 @@
         Args:
             time (SimTime): The current simulation time (in nanoseconds).
             changes (Changes): A mapping of changed component inputs and their new
                 values.
         """
 
 
-@dataclass  # type: ignore
 @as_tagged_union
+@pydantic.v1.dataclasses.dataclass
 class ComponentConfig:
     """A data container for component configuration.
 
     A data container for component configuration which acts as a named union of
     subclasses to facilitate automatic deserialization.
     """
 
@@ -71,22 +74,22 @@
         """Create the component from the given config."""
         raise NotImplementedError(self)
 
 
 class BaseComponent(Component):
     """A base class for components, implementing state interface related methods."""
 
-    state_consumer: StateConsumer[Union[Input, StopComponent]]
-    state_producer: StateProducer[Union[Interrupt, Output, ComponentException]]
+    state_consumer: StateConsumer[ComponentInput]
+    state_producer: StateProducer[ComponentOutput]
 
-    async def handle_input(self, message: Union[Input, StopComponent]):
+    async def handle_input(self, message: ComponentInput):
         """Call on_tick when an input is received.
 
         Args:
-            message (Union[Input, StopComponent])): An immutable data container for any
+            message (ComponentInput): An immutable data container for any
                 message a component receives.
         """
         if isinstance(message, Input):
             LOGGER.debug(f"{self.name} got {message}")
             try:
                 await asyncio.gather(
                     self.on_tick(message.time, message.changes), return_exceptions=False
```

### Comparing `tickit-0.2.3/src/tickit/core/components/device_simulation.py` & `tickit-0.3.0/src/tickit/core/components/device_simulation.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.3/src/tickit/core/components/system_simulation.py` & `tickit-0.3.0/src/tickit/core/components/system_simulation.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import asyncio
 import logging
 from dataclasses import dataclass, field
 from typing import Dict, List, Type
 
+import pydantic.v1.dataclasses
+
 from tickit.core.components.component import BaseComponent, Component, ComponentConfig
 from tickit.core.management.event_router import InverseWiring
 from tickit.core.management.schedulers.slave import SlaveScheduler
 from tickit.core.runner import run_all
 from tickit.core.state_interfaces.state_interface import StateConsumer, StateProducer
 from tickit.core.typedefs import Changes, ComponentID, ComponentPort, PortID, SimTime
 from tickit.utils.topic_naming import output_topic
@@ -94,20 +96,19 @@
         Cancels long running adapter tasks associated with the component.
         """
         LOGGER.debug(f"Stopping {self.name}")
         for task in self._tasks:
             task.cancel()
 
 
-@dataclass
+@pydantic.v1.dataclasses.dataclass
 class SystemSimulation(ComponentConfig):
     """Simulation of a nested set of components."""
 
     name: ComponentID
-    inputs: Dict[PortID, ComponentPort]
     components: List[ComponentConfig]
     expose: Dict[PortID, ComponentPort]
 
     def __call__(self) -> Component:  # noqa: D102
         return SystemSimulationComponent(
             name=self.name,
             components=self.components,
```

### Comparing `tickit-0.2.3/src/tickit/core/device.py` & `tickit-0.3.0/src/tickit/core/device.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
 from typing import Generic, Hashable, Mapping, Optional, TypeVar
 
 from tickit.core.typedefs import SimTime
-from tickit.utils.configuration.configurable import as_tagged_union
 
 #: A bound typevar for mappings of device inputs
 InMap = TypeVar("InMap", bound=Mapping[str, Hashable])
 #: A bound typevar for mappings of device outputs
 OutMap = TypeVar("OutMap", bound=Mapping[str, Hashable])
 
 
@@ -20,15 +19,14 @@
         call_at: The simulation time at which the component requests to be awoken.
     """
 
     outputs: OutMap
     call_at: Optional[SimTime]
 
 
-@as_tagged_union
 class Device(ABC, Generic[InMap, OutMap]):
     """An interface for types which implement simulated devices."""
 
     @abstractmethod
     def update(self, time: SimTime, inputs: InMap) -> DeviceUpdate[OutMap]:
         """Implements device behaviour according to the time and its inputs.
```

### Comparing `tickit-0.2.3/src/tickit/core/management/event_router.py` & `tickit-0.3.0/src/tickit/core/management/event_router.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from collections import defaultdict, deque
+from functools import cached_property
 from typing import DefaultDict, Dict, Iterable, Mapping, Optional, Set, Union, overload
 
 from tickit.core.components.component import ComponentConfig
 from tickit.core.typedefs import ComponentID, ComponentPort, PortID
-from tickit.utils.compat.functools_compat import cached_property
 
 #: A mapping of component output ports to component input ports with defaults
 Default_Wiring_Struct = DefaultDict[
     ComponentID, DefaultDict[PortID, Set[ComponentPort]]
 ]
 #: A mapping of component output ports to component input ports
 Wiring_Struct = Dict[ComponentID, Dict[PortID, Set[ComponentPort]]]
```

### Comparing `tickit-0.2.3/src/tickit/core/management/schedulers/base.py` & `tickit-0.3.0/src/tickit/core/management/schedulers/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 
 from tickit.core.management.event_router import InverseWiring, Wiring
 from tickit.core.management.ticker import Ticker
 from tickit.core.state_interfaces import StateConsumer, StateProducer
 from tickit.core.typedefs import (
     ComponentException,
     ComponentID,
+    ComponentInput,
+    ComponentOutput,
     Input,
     Interrupt,
     Output,
     SimTime,
     StopComponent,
 )
 from tickit.utils.topic_naming import input_topic, output_topic
@@ -63,17 +65,15 @@
 
         Args:
             input (Input): The input to be included in the message sent to the
                 component.
         """
         await self.state_producer.produce(input_topic(input.target), input)
 
-    async def handle_message(
-        self, message: Union[Interrupt, Output, ComponentException]
-    ) -> None:
+    async def handle_message(self, message: ComponentOutput) -> None:
         """Handle messages received by the state consumer.
 
         An asynchronous callback which handles Interrupt, Output and ComponentException
         messages received by the state consumer. For Outputs, changes are propagated
         and wakeups scheduled if required. For interrupts handling is deferred. For
         exceptions, a StopComponent message is produced to each component in the system
         to facilitate shut down.
@@ -96,23 +96,21 @@
         """Instantiates and configures the ticker and state interfaces.
 
         An asynchronous setup method which creates a ticker, a state consumer which is
         subscribed to the output topics of each component in the system, a state
         producer to produce component inputs.
         """
         self.ticker = Ticker(self._wiring, self.update_component)
-        self.state_consumer: StateConsumer[
-            Union[Interrupt, Output, ComponentException]
-        ] = self._state_consumer_cls(self.handle_message)
+        self.state_consumer: StateConsumer[ComponentOutput] = self._state_consumer_cls(
+            self.handle_message
+        )
         await self.state_consumer.subscribe(
             {output_topic(component) for component in self.ticker.components}
         )
-        self.state_producer: StateProducer[
-            Union[Input, StopComponent, ComponentException]
-        ] = self._state_producer_cls()
+        self.state_producer: StateProducer[ComponentInput] = self._state_producer_cls()
 
     def add_wakeup(self, component: ComponentID, when: SimTime) -> None:
         """Adds a wakeup to the mapping.
 
         Args:
             component (ComponentID): The component which should be updated.
             when (SimTime): The simulation time at which the update should occur.
```

### Comparing `tickit-0.2.3/src/tickit/core/management/schedulers/master.py` & `tickit-0.3.0/src/tickit/core/management/schedulers/master.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,14 +36,15 @@
             simulation_speed (float): The rate at which simulation time progresses with
                 respect to real world time. Defaults to 1.0.
         """
         super().__init__(wiring, state_consumer, state_producer)
 
         self._initial_time = SimTime(initial_time)
         self.simulation_speed = simulation_speed
+        self.running = asyncio.Event()
 
     async def setup(self) -> None:
         """Performs base setup and creates an awaitable flag to indicate new wakeups."""
         await super().setup()
         self.new_wakeup: asyncio.Event = asyncio.Event()
 
     def add_wakeup(self, component: ComponentID, when: SimTime) -> None:
@@ -58,23 +59,26 @@
         """
         super().add_wakeup(component, when)
         self.new_wakeup.set()
 
     async def run_forever(self) -> None:
         """Perform initial tick then continuously schedule ticks according to wakeups.
 
-        An asynchronous method which initially performs setup and an initial tick in
-        which all components are updated, subsequently ticks are performed as requested
-        by components of the simulation according to the simulation speed.
+        An asynchronous method which initially performs setup, sets the event to
+        signify the simulation is running, and performs an initial tick in which all
+        components are updated. Subsequent ticks are performed as requested by
+        components of the simulation according to the simulation speed.
         """
         await self.setup()
+        self.running.set()
         await self._do_initial_tick()
         while not self.error.is_set():
             await self._do_tick()
         LOGGER.debug("Stopping Master Scheduler")
+        self.running.clear()
 
     async def _do_initial_tick(self):
         """Performs the initial tick of the system."""
         await self.ticker(
             self._initial_time,
             self.ticker.components,
         )
@@ -84,16 +88,16 @@
         """Continuously schedules ticks according to wakeups."""
         if not self.wakeups:
             await self.new_wakeup.wait()
         components, when = self.get_first_wakeups()
         assert when is not None
         self.new_wakeup.clear()
 
-        current: asyncio.Future = asyncio.sleep(self.sleep_time(when))
         new = asyncio.create_task(self.new_wakeup.wait())
+        current = asyncio.create_task(asyncio.sleep(self.sleep_time(when)))
         which, _ = await asyncio.wait(
             [current, new], return_when=asyncio.tasks.FIRST_COMPLETED
         )
 
         if new in which:
             return
```

### Comparing `tickit-0.2.3/src/tickit/core/management/schedulers/slave.py` & `tickit-0.3.0/src/tickit/core/management/schedulers/slave.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.3/src/tickit/core/management/ticker.py` & `tickit-0.3.0/src/tickit/core/management/ticker.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.3/src/tickit/core/runner.py` & `tickit-0.3.0/src/tickit/core/runner.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.3/src/tickit/core/state_interfaces/internal.py` & `tickit-0.3.0/src/tickit/core/state_interfaces/internal.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.3/src/tickit/core/state_interfaces/kafka.py` & `tickit-0.3.0/src/tickit/core/state_interfaces/kafka.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.3/src/tickit/core/state_interfaces/state_interface.py` & `tickit-0.3.0/src/tickit/core/state_interfaces/state_interface.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,21 @@
-import sys
-from typing import Awaitable, Callable, Dict, Iterable, Set, Tuple, Type, TypeVar
+from typing import (
+    Awaitable,
+    Callable,
+    Dict,
+    Iterable,
+    Protocol,
+    Set,
+    Tuple,
+    Type,
+    TypeVar,
+    runtime_checkable,
+)
 from warnings import warn
 
-# TODO: Investigate why import from tickit.utils.compat.typing_compat causes mypy error
-# See mypy issue for details: https://github.com/python/mypy/issues/10851
-if sys.version_info >= (3, 8):
-    from typing import Protocol, runtime_checkable
-elif sys.version_info >= (3, 5):
-    from typing_extensions import Protocol, runtime_checkable
-
 #: A consumable value
 C = TypeVar("C", covariant=True)
 #: A producible value
 P = TypeVar("P", contravariant=True)
 
 
 @runtime_checkable
```

### Comparing `tickit-0.2.3/src/tickit/core/typedefs.py` & `tickit-0.3.0/src/tickit/core/typedefs.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from dataclasses import dataclass
-from typing import Hashable, Iterator, Mapping, NewType, Optional
+from typing import Hashable, Iterator, Mapping, NewType, Optional, Union
 
-from apischema import deserializer, serializer
 from immutables import Map
 
 #: An identifier which specifies the component
 ComponentID = NewType("ComponentID", str)
 #: An identifier which specifies the input/output port of a component
 PortID = NewType("PortID", str)
 #: A mapping of PortID to component input/output property
@@ -27,39 +26,14 @@
         """A string representation of the object of format component:port.
 
         Returns:
             str: A string representation of the object of format component:port.
         """
         return ":".join((self.component, self.port))
 
-    @serializer
-    def serialize(self) -> str:
-        """Returns a string of component:port.
-
-        An apischema serialization method which returns a string of component:port.
-
-        Returns:
-            str: The serialized ComponentPort, in format component:port.
-        """
-        return str(self)
-
-    @deserializer
-    @staticmethod
-    def deserialize(data: str) -> "ComponentPort":
-        """Builds a ComponentPort from a string of component:port.
-
-        An apischema deserialization method which builds a ComponentPort from a string
-        of component:port.
-
-        Returns:
-            ComponentPort: The deserialized ComponentPort.
-        """
-        component, port = data.split(":")
-        return ComponentPort(ComponentID(component), PortID(port))
-
     def __iter__(self) -> Iterator:
         """An iterator which returns (component, port).
 
         Returns:
             Iterator: An iterator containing (component, port).
         """
         return (x for x in (self.component, self.port))
@@ -122,7 +96,11 @@
     Args:
         component: The Component which raised an exception.
     """
 
     source: ComponentID
     error: Exception
     traceback: str
+
+
+ComponentOutput = Union[Interrupt, Output, ComponentException]
+ComponentInput = Union[Input, StopComponent, ComponentException]
```

### Comparing `tickit-0.2.3/src/tickit/devices/iobox.py` & `tickit-0.3.0/src/tickit/devices/iobox.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import logging
-from typing import Any, Dict, Generic, List, Tuple, TypeVar
+from typing import Any, Dict, Generic, List, Tuple, TypedDict, TypeVar
 
+import pydantic.v1.dataclasses
 from typing_extensions import NotRequired
 
 from tickit.core.components.component import Component, ComponentConfig
 from tickit.core.components.device_simulation import DeviceSimulation
 from tickit.core.device import Device, DeviceUpdate
 from tickit.core.typedefs import SimTime
-from tickit.utils.compat.typing_compat import TypedDict
 
 LOGGER = logging.getLogger(__name__)
 
 A = TypeVar("A")
 V = TypeVar("V")
 
 
@@ -116,14 +116,15 @@
         while self._change_buffer:
             addr, value = self._change_buffer.pop()
             self._memory[addr] = value
             updates.append((addr, value))
         return DeviceUpdate(IoBoxDevice.Outputs(updates=updates), None)
 
 
+@pydantic.v1.dataclasses.dataclass
 class IoBox(ComponentConfig):
     """Arbitrary box of key-value pairs."""
 
     def __call__(self) -> Component:  # noqa: D102
         return DeviceSimulation(
             name=self.name,
             device=IoBoxDevice(),
```

### Comparing `tickit-0.2.3/src/tickit/devices/sink.py` & `tickit-0.3.0/src/tickit/devices/source.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,44 +1,56 @@
 import logging
-from typing import Any
+from typing import Any, TypedDict
+
+import pydantic.v1.dataclasses
 
 from tickit.core.components.component import Component, ComponentConfig
 from tickit.core.components.device_simulation import DeviceSimulation
 from tickit.core.device import Device, DeviceUpdate
 from tickit.core.typedefs import SimTime
-from tickit.utils.compat.typing_compat import TypedDict
 
 LOGGER = logging.getLogger(__name__)
 
 
-class SinkDevice(Device):
-    """A simple device which can take any input and produces no output."""
+class SourceDevice(Device):
+    """A simple device which produces a pre-configured value."""
+
+    #: An empty typed mapping of device inputs
+    Inputs: TypedDict = TypedDict("Inputs", {})
+    #: A typed mapping containing the 'value' output value
+    Outputs: TypedDict = TypedDict("Outputs", {"value": Any})
+
+    def __init__(self, value: Any) -> None:
+        """A constructor of the source, which takes the pre-configured output value.
 
-    #: A typed mapping containing the 'input' input value
-    Inputs: TypedDict = TypedDict("Inputs", {"input": Any})
-    #: An empty typed mapping of device outputs
-    Outputs: TypedDict = TypedDict("Outputs", {})
+        Args:
+            value (Any): A pre-configured output value.
+        """
+        self.value = value
 
     def update(self, time: SimTime, inputs: Inputs) -> DeviceUpdate[Outputs]:
-        """The update method which logs the inputs and produces no outputs.
+        """The update method which produces the pre-configured output value.
 
         Args:
             time (SimTime): The current simulation time (in nanoseconds).
             inputs (State): A mapping of inputs to the device and their values.
 
         Returns:
             DeviceUpdate[Outputs]:
-                The produced update event which never contains any changes, and never
-                requests a callback.
+                The produced update event which contains the pre-configured value, and
+                never requests a callback.
         """
-        LOGGER.debug(f"Sunk { {k: v for k, v in inputs.items()} }")
-        return DeviceUpdate(SinkDevice.Outputs(), None)
+        LOGGER.debug(f"Sourced {self.value}")
+        return DeviceUpdate(SourceDevice.Outputs(value=self.value), None)
+
 
+@pydantic.v1.dataclasses.dataclass
+class Source(ComponentConfig):
+    """Source of a fixed value."""
 
-class Sink(ComponentConfig):
-    """Arbitrary value sink that logs the value."""
+    value: Any
 
     def __call__(self) -> Component:  # noqa: D102
         return DeviceSimulation(
             name=self.name,
-            device=SinkDevice(),
+            device=SourceDevice(self.value),
         )
```

### Comparing `tickit-0.2.3/src/tickit/utils/topic_naming.py` & `tickit-0.3.0/src/tickit/utils/topic_naming.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.3/src/tickit.egg-info/PKG-INFO` & `tickit-0.3.0/src/tickit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tickit
-Version: 0.2.3
+Version: 0.3.0
 Summary: Event-based device simulation framework
 Author-email: Callum Forrester <callum.forrester@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -204,18 +204,17 @@
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
         
 Project-URL: GitHub, https://github.com/dls-controls/tickit
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
 License-File: LICENSE
 
 tickit
 ======
 
@@ -237,21 +236,23 @@
 A simulation is defined using a yaml file, in which the graphing of the required
 components is denoted. This file defines a **Counter** device named **counter** and
 a **Sink** device named **counter_sink**. The output **_value** of **counter** is wired
 to the input of **counter_sink**.
 
 .. code-block:: yaml
 
-    - examples.devices.counter.Counter:
-        name: counter
-        inputs: {}
-    - tickit.devices.sink.Sink:
-        name: counter_sink
-        inputs:
-          input: counter:_value
+    - type: examples.devices.counter.Counter
+      name: counter
+      inputs: {}
+    - type: tickit.devices.sink.Sink
+      name: counter_sink
+      inputs:
+        input:
+          component: counter
+          port: _value
 
 
 This file is executed to run the simulation.
 
 .. code-block:: bash
 
     python -m tickit all examples/configs/counter.yaml
```

### Comparing `tickit-0.2.3/src/tickit.egg-info/SOURCES.txt` & `tickit-0.3.0/src/tickit.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -121,14 +121,15 @@
 src/tickit/adapters/servers/tcp.py
 src/tickit/adapters/zeromq/__init__.py
 src/tickit/adapters/zeromq/push_adapter.py
 src/tickit/core/__init__.py
 src/tickit/core/adapter.py
 src/tickit/core/device.py
 src/tickit/core/runner.py
+src/tickit/core/simulation.py
 src/tickit/core/typedefs.py
 src/tickit/core/components/__init__.py
 src/tickit/core/components/component.py
 src/tickit/core/components/device_simulation.py
 src/tickit/core/components/system_simulation.py
 src/tickit/core/management/__init__.py
 src/tickit/core/management/event_router.py
@@ -145,20 +146,17 @@
 src/tickit/devices/iobox.py
 src/tickit/devices/sink.py
 src/tickit/devices/source.py
 src/tickit/utils/__init__.py
 src/tickit/utils/byte_format.py
 src/tickit/utils/singleton.py
 src/tickit/utils/topic_naming.py
-src/tickit/utils/compat/__init__.py
-src/tickit/utils/compat/functools_compat.py
-src/tickit/utils/compat/typing_compat.py
 src/tickit/utils/configuration/__init__.py
-src/tickit/utils/configuration/configurable.py
 src/tickit/utils/configuration/loading.py
+src/tickit/utils/configuration/tagged_union.py
 tests/conftest.py
 tests/test_cli.py
 tests/adapters/test_httpadapter.py
 tests/adapters/interpreters/test_utils.py
 tests/adapters/interpreters/command/test_command_interpreter.py
 tests/adapters/interpreters/command/test_regex_command.py
 tests/adapters/interpreters/endpoints/test_http_endpoint.py
@@ -166,16 +164,18 @@
 tests/adapters/interpreters/wrappers/test_joining_interpreter.py
 tests/adapters/interpreters/wrappers/test_splitting_interpreter.py
 tests/adapters/servers/test_tcp.py
 tests/adapters/test_epicsadapter/__init__.py
 tests/adapters/test_epicsadapter/test_epics_adapter.py
 tests/adapters/zeromq/__init__.py
 tests/adapters/zeromq/test_push_adapter.py
+tests/core/sim.yaml
 tests/core/test_device.py
 tests/core/test_runner.py
+tests/core/test_simulation.py
 tests/core/test_typedefs.py
 tests/core/components/test_component.py
 tests/core/components/test_device_simulation.py
 tests/core/components/test_system_simulation.py
 tests/core/management/test_event_router.py
 tests/core/management/test_ticker.py
 tests/core/management/schedulers/test_base_scheduler.py
```

### Comparing `tickit-0.2.3/tests/adapters/interpreters/command/test_command_interpreter.py` & `tickit-0.3.0/tests/adapters/interpreters/command/test_command_interpreter.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.3/tests/adapters/interpreters/command/test_regex_command.py` & `tickit-0.3.0/tests/adapters/interpreters/command/test_regex_command.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.3/tests/adapters/interpreters/endpoints/test_http_endpoint.py` & `tickit-0.3.0/tests/adapters/interpreters/endpoints/test_http_endpoint.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.3/tests/adapters/interpreters/test_utils.py` & `tickit-0.3.0/tests/adapters/interpreters/test_utils.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.3/tests/adapters/interpreters/wrappers/test_beheading_interpreter.py` & `tickit-0.3.0/tests/adapters/interpreters/wrappers/test_beheading_interpreter.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.3/tests/adapters/interpreters/wrappers/test_joining_interpreter.py` & `tickit-0.3.0/tests/adapters/interpreters/wrappers/test_joining_interpreter.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.3/tests/adapters/interpreters/wrappers/test_splitting_interpreter.py` & `tickit-0.3.0/tests/adapters/interpreters/wrappers/test_splitting_interpreter.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.3/tests/adapters/servers/test_tcp.py` & `tickit-0.3.0/tests/adapters/servers/test_tcp.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.3/tests/adapters/test_epicsadapter/test_epics_adapter.py` & `tickit-0.3.0/tests/adapters/test_epicsadapter/test_epics_adapter.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.3/tests/adapters/test_httpadapter.py` & `tickit-0.3.0/tests/adapters/test_httpadapter.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.3/tests/adapters/zeromq/test_push_adapter.py` & `tickit-0.3.0/tests/adapters/zeromq/test_push_adapter.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.3/tests/conftest.py` & `tickit-0.3.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.3/tests/core/components/test_component.py` & `tickit-0.3.0/tests/core/components/test_component.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.3/tests/core/components/test_device_simulation.py` & `tickit-0.3.0/tests/core/components/test_device_simulation.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.3/tests/core/components/test_system_simulation.py` & `tickit-0.3.0/tests/core/components/test_system_simulation.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.3/tests/core/management/schedulers/test_base_scheduler.py` & `tickit-0.3.0/tests/core/management/schedulers/test_base_scheduler.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.3/tests/core/management/schedulers/test_master_scheduler.py` & `tickit-0.3.0/tests/core/management/schedulers/test_master_scheduler.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.3/tests/core/management/schedulers/test_slave_scheduler.py` & `tickit-0.3.0/tests/core/management/schedulers/test_slave_scheduler.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.3/tests/core/management/test_event_router.py` & `tickit-0.3.0/tests/core/management/test_event_router.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.3/tests/core/management/test_ticker.py` & `tickit-0.3.0/tests/core/management/test_ticker.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.3/tests/core/state_interfaces/test_internal.py` & `tickit-0.3.0/tests/core/state_interfaces/test_internal.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.3/tests/core/state_interfaces/test_kafka.py` & `tickit-0.3.0/tests/core/state_interfaces/test_kafka.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.3/tests/core/state_interfaces/test_state_interface.py` & `tickit-0.3.0/tests/core/state_interfaces/test_state_interface.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.3/tests/core/test_typedefs.py` & `tickit-0.3.0/tests/core/test_typedefs.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.3/tests/devices/test_iobox.py` & `tickit-0.3.0/tests/devices/test_iobox.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.3/tests/devices/test_sink.py` & `tickit-0.3.0/tests/devices/test_sink.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.3/tests/devices/test_source.py` & `tickit-0.3.0/tests/devices/test_source.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.3/tests/utils/configuration/test_loading.py` & `tickit-0.3.0/tests/utils/configuration/test_loading.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-from typing import Any, Callable, Iterable, Type
+from typing import Iterable
 
+import pydantic.v1.dataclasses
 import pytest
-from apischema.conversions.conversions import Conversion
 from mock import Mock, create_autospec, patch
 from mock.mock import mock_open
 
 from tickit.core.components.component import ComponentConfig
 from tickit.core.typedefs import ComponentID, ComponentPort, PortID
-from tickit.utils.configuration.loading import importing_conversion, read_configs
+from tickit.utils.configuration.loading import read_configs
 
 
 @pytest.fixture
 def mock_component_config_type() -> Mock:
     return create_autospec(ComponentConfig, instance=False)
 
 
@@ -20,65 +20,37 @@
     with patch.dict(
         "tickit.utils.configuration.loading.is_tagged_union",
         {mock_component_config_type: True},
     ) as mock:
         yield mock
 
 
-def test_importing_conversion(
-    mock_component_config_type: Type[ComponentConfig], patch_tagged_union_dict
-):
-    conversion = importing_conversion(mock_component_config_type)
-    assert isinstance(conversion, Conversion)
-    assert conversion.target == mock_component_config_type
-
-
-def test_importing_conversion_when_is_not_tagged_union(
-    mock_component_config_type: Type[ComponentConfig],
-):
-    conversion = importing_conversion(mock_component_config_type)
-    assert conversion == []
-
-
+@pydantic.v1.dataclasses.dataclass
 class MockConfig(ComponentConfig):
     pass
 
     def __call__(self):
         return Mock()
 
 
 @pytest.fixture
-def patch_apischema_deserialize() -> Iterable[Mock]:
+def patch_pydantic_deserialize() -> Iterable[Mock]:
     with patch(
-        "tickit.utils.configuration.loading.deserialize",
+        "tickit.utils.configuration.loading.parse_obj_as",
         autospec=True,
     ) as mock:
         mock.return_value = [
             MockConfig(
                 name=ComponentID("foo"),
                 inputs={PortID("42"): ComponentPort(ComponentID("bar"), PortID("24"))},
             )
         ]
         yield mock
 
 
-def test_conversion(
-    mock_component_config_type,
-    patch_tagged_union_dict,
-    patch_apischema_deserialize: Mock,
-):
-    conversion = importing_conversion(mock_component_config_type)
-    converter: Callable[[Any], Any] = conversion.converter  # type: ignore
-
-    _ = converter({"mock.Mock": 42})
-    patch_apischema_deserialize.assert_called_once_with(
-        Mock, 42, default_conversion=importing_conversion
-    )
-
-
 @pytest.fixture
 def patch_yaml_library() -> Iterable[Mock]:
     with patch("tickit.utils.configuration.loading.yaml", autospec=True) as mock:
         yield mock
 
 
 @pytest.fixture
@@ -89,11 +61,11 @@
         new=mock_open(read_data=blank_yaml),
     ) as mock:
         yield mock
 
 
 def test_read_configs(
     patch_builtins_open: Mock,
-    patch_apischema_deserialize: Mock,
+    patch_pydantic_deserialize: Mock,
 ):
     configs = read_configs("foo/bar.borg")
     assert isinstance(configs[0], MockConfig)
```

### Comparing `tickit-0.2.3/tests/utils/test_singleton.py` & `tickit-0.3.0/tests/utils/test_singleton.py`

 * *Files identical despite different names*

